# Comparing `tmp/tdnpathviz-0.1.2.1-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 377943 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-11 08:39 tdnpathviz/__init__.py
+Zip file size: 378013 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-11 12:15 tdnpathviz/__init__.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat     7226 b- defN 23-Jan-31 11:34 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat     7584 b- defN 23-Apr-11 12:41 tdnpathviz/visualizations.py
 -rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      266 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      723 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/RECORD
-9 files, 2188857 bytes uncompressed, 376693 bytes compressed:  82.8%
+-rw-rw-rw-  2.0 fat      266 b- defN 23-Apr-11 12:58 tdnpathviz-0.1.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 12:58 tdnpathviz-0.1.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-11 12:58 tdnpathviz-0.1.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      723 b- defN 23-Apr-11 12:58 tdnpathviz-0.1.2.2.dist-info/RECORD
+9 files, 2189215 bytes uncompressed, 376763 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.1.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.1.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.1.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.1.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2.1'
+__version__ = '0.1.2.2'
```

## tdnpathviz/visualizations.py

```diff
@@ -18,25 +18,29 @@
         g = int(g) % 256
         b = int(b) % 256
         ret.append("rgba(" + str(r) + "," + str(g) + "," + str(b) + "," + str(alpha) + ")")
     return ret
 
 
 def plot_first_main_paths(myPathAnalysis, path_column='mypath', id_column='travelid', nb_paths=15, print_query=False):
+
+    if type(id_column) != list:
+        id_column = [id_column]
+
     if type(myPathAnalysis) != tdml.dataframe.dataframe.DataFrame:
-        df_agg = myPathAnalysis.result.select([id_column, path_column]).groupby(path_column).count()
+        df_agg = myPathAnalysis.result.select(id_column+[path_column]).groupby(path_column).count()
     else:
-        df_agg = myPathAnalysis.select([id_column, path_column]).groupby(path_column).count()
+        df_agg = myPathAnalysis.select(id_column+[path_column]).groupby(path_column).count()
 
     df_agg._DataFrame__execute_node_and_set_table_name(df_agg._nodeid, df_agg._metaexpr)
 
     query = f"""SEL
-        row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column} DESC) as id
+        row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column[0]} DESC) as id
     ,	REGEXP_REPLACE(lower(A.{path_column}),'\\[|\\]', '') as str
-    ,	count_{id_column} as weight
+    ,	count_{id_column[0]} as weight
     FROM {df_agg._table_name} A
     QUALIFY id < {nb_paths}+1"""
 
     df_selection = tdml.DataFrame.from_query(query)
 
     query2 = f"""
     sel
@@ -126,44 +130,55 @@
 
     return
 
 def create_all_pathes_views(myPathAnalysis, root_name = 'mytest',
                             schema = tdml.get_context().execute('SELECT DATABASE').fetchall()[0][0],
                             path_column='mypath', id_column='travelid'):
 
+    if type(id_column) != list:
+        id_column = [id_column]
+
     # Create the view of my npath
     npath_view = f"{schema}.{root_name}_NPATH_VIEW"
-    query = f"""
-    REPLACE VIEW  {npath_view} AS
-    {myPathAnalysis.sqlmr_query}
-    """
+
+    try:
+        query = f"""
+        REPLACE VIEW  {npath_view} AS
+        {myPathAnalysis.sqlmr_query}
+        """
+    except Exception as e:
+        print(str(e).split('\n')[0])
+        query = f"""
+        REPLACE VIEW  {npath_view} AS
+        {myPathAnalysis.show_query()}
+        """
     tdml.get_context().execute(query)
     print(f'npath view created : {npath_view}')
 
     # Create the aggregated view of my npath
     aggregated_npath_view = f"{schema}.{root_name}_NPATH_VIEW_AGG"
     query = f"""
     REPLACE VIEW {aggregated_npath_view} AS
     SELECT 
         {path_column}
-    ,   COUNT(*) as count_{id_column}
+    ,   COUNT(*) as count_{id_column[0]}
     FROM {npath_view}
     GROUP BY 1
     """
     tdml.get_context().execute(query)
     print(f'aggregated npath view created : {aggregated_npath_view}')
 
     # Create the cleaned aggregated view of my npath
     clean_aggregated_npath_view = f"{schema}.{root_name}_CLEAN_NPATH_VIEW_AGG"
     query = f"""
     REPLACE VIEW {clean_aggregated_npath_view} AS
     SELECT 
-        row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column} DESC) as id
+        row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column[0]} DESC) as id
     ,	REGEXP_REPLACE(lower(A.{path_column}),'\[|\]', '') as str
-    ,	count_{id_column} as weight
+    ,	count_{id_column[0]} as weight
     FROM {aggregated_npath_view} A"""
     tdml.get_context().execute(query)
     print(f'clean aggregated npath view created : {clean_aggregated_npath_view}')
 
     # Create the graph view of the aggregated npath view
     graph_aggregated_npath_view =  f"{schema}.{root_name}_GRAPH_NPATH_VIEW_AGG"
     query = f"""
```

