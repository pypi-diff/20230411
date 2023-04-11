# Comparing `tmp/tdnpathviz-0.1.2-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 377859 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       21 b- defN 22-Sep-08 16:18 tdnpathviz/__init__.py
--rw-rw-rw-  2.0 fat      991 b- defN 22-Jul-21 14:04 tdnpathviz/datasets.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-21 11:58 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat     6871 b- defN 22-Sep-08 15:26 tdnpathviz/visualizations.py
--rw-rw-rw-  2.0 fat  2179525 b- defN 21-Feb-01 10:34 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      327 b- defN 22-Sep-08 16:19 tdnpathviz-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-08 16:19 tdnpathviz-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 22-Sep-08 16:19 tdnpathviz-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      715 b- defN 22-Sep-08 16:19 tdnpathviz-0.1.2.dist-info/RECORD
-9 files, 2188553 bytes uncompressed, 376625 bytes compressed:  82.8%
+Zip file size: 377943 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-11 08:39 tdnpathviz/__init__.py
+-rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
+-rw-rw-rw-  2.0 fat     7226 b- defN 23-Jan-31 11:34 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
+-rw-rw-rw-  2.0 fat      266 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      723 b- defN 23-Apr-11 08:39 tdnpathviz-0.1.2.1.dist-info/RECORD
+9 files, 2188857 bytes uncompressed, 376693 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2'
+__version__ = '0.1.2.1'
```

## tdnpathviz/visualizations.py

```diff
@@ -17,22 +17,25 @@
         r = int(r) % 256
         g = int(g) % 256
         b = int(b) % 256
         ret.append("rgba(" + str(r) + "," + str(g) + "," + str(b) + "," + str(alpha) + ")")
     return ret
 
 
-def plot_first_main_paths(myPathAnalysis, path_column='mypath', id_column='travelid', nb_paths=15):
-    df_agg = myPathAnalysis.result.select([id_column, path_column]).groupby(path_column).count()
+def plot_first_main_paths(myPathAnalysis, path_column='mypath', id_column='travelid', nb_paths=15, print_query=False):
+    if type(myPathAnalysis) != tdml.dataframe.dataframe.DataFrame:
+        df_agg = myPathAnalysis.result.select([id_column, path_column]).groupby(path_column).count()
+    else:
+        df_agg = myPathAnalysis.select([id_column, path_column]).groupby(path_column).count()
 
-    df_agg.shape[0]
+    df_agg._DataFrame__execute_node_and_set_table_name(df_agg._nodeid, df_agg._metaexpr)
 
-    query = f"""SEL 
+    query = f"""SEL
         row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column} DESC) as id
-    ,	REGEXP_REPLACE(lower(A.{path_column}),'\[|\]', '') as str
+    ,	REGEXP_REPLACE(lower(A.{path_column}),'\\[|\\]', '') as str
     ,	count_{id_column} as weight
     FROM {df_agg._table_name} A
     QUALIFY id < {nb_paths}+1"""
 
     df_selection = tdml.DataFrame.from_query(query)
 
     query2 = f"""
@@ -44,16 +47,16 @@
     ,	CC."end"
     ,	sum(CC.weight) as weight
     FROM 
     (
     sel
         B.*
     ,	LAG(id_end,1,0) OVER (PARTITION BY B."path" ORDER BY B."path",B."index") as id_beg
-    ,	B."beg" || '_' || TRIM(CAST(id_beg AS VARCHAR(10))) as node_source
-    ,	B."end" || '_' || TRIM(CAST(id_end AS VARCHAR(10))) as node_target
+    ,	B."beg" || '_' || TRIM(CAST(id_beg AS VARCHAR(200))) as node_source
+    ,	B."end" || '_' || TRIM(CAST(id_end AS VARCHAR(200))) as node_target
     FROM 
     (
         sel 
             A.*
         ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."path",A."index") as id_end
         from (
         SELECT
@@ -65,30 +68,35 @@
         ,	AA.tokennum as "index"
         ,   B.id
         FROM (
 
         SELECT 
             d.*
         FROM TABLE (strtok_split_to_table({df_selection._table_name}.id, {df_selection._table_name}.str, ',')
-        RETURNS (outkey integer, tokennum integer, token varchar(20)character set unicode) ) as d 
+        RETURNS (outkey integer, tokennum integer, token varchar(200)character set unicode) ) as d 
 
         ) AA
         ,{df_selection._table_name} B
         WHERE AA.outkey = B.id
         QUALIFY beg IS NOT NULL
     ) A
     ) B
     --ORDER BY "path","index"
     ) CC
     GROUP BY 1,2,3,4,5
     """
 
+    if print_query:
+        print(query2)
+
     df_ready = tdml.DataFrame.from_query(query2)
 
-    df_ready_local = df_ready.to_pandas().sort_values(by='id')
+    df_ready_local = df_ready.to_pandas()
+
+    df_ready_local = df_ready_local.sort_values(by='id')
 
     labs = dict()
     labels = list(set(df_ready_local.node_source.tolist() + df_ready_local.node_target.tolist()))
 
     for i, label in enumerate(labels):
         labs[label] = i
```

## Comparing `tdnpathviz-0.1.2.dist-info/RECORD` & `tdnpathviz-0.1.2.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tdnpathviz/__init__.py,sha256=r_cKr7sbAG8wXvZQ-5WkC2eXGKMDWp6Xe_hNXu43MT0,21
+tdnpathviz/__init__.py,sha256=t71pzlIjd1QonMO5b4ZVP806yBHz9ClReMYlhnIIZJI,23
 tdnpathviz/datasets.py,sha256=XASLSjLtaHMZq-uPArgCLjbGapxDI2CJ2i0gSu9KW8M,991
 tdnpathviz/utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tdnpathviz/visualizations.py,sha256=G8vxwR-HCu1zoB2rDEZGrk6Ik7BnkWXz0dz8AZnhNao,6871
+tdnpathviz/visualizations.py,sha256=IxsgSLs2wj7vT3StoJ3UAnPjTfoGx898YmWj5EfXqC0,7226
 tdnpathviz/data/train_dataset.csv,sha256=ko9f4sY4Cglvfii921mOnb01gAqP_EOhgKe12UdX9Pg,2179525
-tdnpathviz-0.1.2.dist-info/METADATA,sha256=siad_5WJynn7f0n_jD0qVYa0DCRJ1jro18xcYN28Mfs,327
-tdnpathviz-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tdnpathviz-0.1.2.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
-tdnpathviz-0.1.2.dist-info/RECORD,,
+tdnpathviz-0.1.2.1.dist-info/METADATA,sha256=DSSZWUs09DZKmNeaPA52D4yCMJRTcXG8cU6lqwXuOa0,266
+tdnpathviz-0.1.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tdnpathviz-0.1.2.1.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
+tdnpathviz-0.1.2.1.dist-info/RECORD,,
```

