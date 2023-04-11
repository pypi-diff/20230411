# Comparing `tmp/bintang-0.1.5-py3-none-any.whl.zip` & `tmp/bintang-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 21210 bytes, number of entries: 14
+Zip file size: 21384 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       25 b- defN 22-Sep-15 02:00 bintang/__init__.py
 -rw-rw-rw-  2.0 fat     6439 b- defN 22-Jul-05 11:25 bintang/besqlite.py
 -rw-rw-rw-  2.0 fat     1319 b- defN 22-Dec-22 23:56 bintang/cell.py
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Mar-29 02:17 bintang/column.py
--rw-rw-rw-  2.0 fat    23341 b- defN 23-Apr-07 05:18 bintang/core.py
+-rw-rw-rw-  2.0 fat    23341 b- defN 23-Apr-11 09:18 bintang/core.py
 -rw-rw-rw-  2.0 fat      186 b- defN 23-Feb-13 06:10 bintang/log.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 22-Dec-21 22:40 bintang/row.py
--rw-rw-rw-  2.0 fat    45915 b- defN 23-Apr-07 04:30 bintang/table.py
+-rw-rw-rw-  2.0 fat    47313 b- defN 23-Apr-11 11:28 bintang/table.py
 -rw-rw-rw-  2.0 fat     4981 b- defN 23-Feb-20 03:30 bintang/travdict.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-07 06:22 bintang-0.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-07 06:22 bintang-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-07 06:22 bintang-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-07 06:22 bintang-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1043 b- defN 23-Apr-07 06:22 bintang-0.1.5.dist-info/RECORD
-14 files, 86641 bytes uncompressed, 19510 bytes compressed:  77.5%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1043 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/RECORD
+14 files, 88039 bytes uncompressed, 19684 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: bintang/table.py
 Comment: 
 
 Filename: bintang/travdict.py
 Comment: 
 
-Filename: bintang-0.1.5.dist-info/LICENSE
+Filename: bintang-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: bintang-0.1.5.dist-info/METADATA
+Filename: bintang-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: bintang-0.1.5.dist-info/WHEEL
+Filename: bintang-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: bintang-0.1.5.dist-info/top_level.txt
+Filename: bintang-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: bintang-0.1.5.dist-info/RECORD
+Filename: bintang-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bintang/core.py

```diff
@@ -312,15 +312,15 @@
                         columns.append(cell.value)
                 if Nonecolumn_cnt > 0:
                     log.warning('Warning! Noname column detected!')          
             
             if rownum > 1:
                 for cell in row_cells:
                     values.append(cell.value)
-                self.get_table(table_).insert(columns, values)
+                self.get_table(table_).insert(values, columns)
         if self.__be is not None:
             self.get_table(table_).add_row_into_be()
 
 
     def read_dict(self, dict_obj, tablepaths=[]):
         debug = False
         for tprow in travdict.traverse_dict(dict_obj, tablepaths):
```

## bintang/table.py

```diff
@@ -64,33 +64,41 @@
         return len(self.__rows)
 
     def set_to_sql_colmap(self, columns):
         if isinstance(columns, list):
             return dict(zip(columns, columns))
         elif isinstance(columns, dict):
             return columns
-            
-    def to_sql_str(self, conn, schemaname, table, columns, max_rows = 300):
+        
+
+    def to_sql(self, conn, schema, table, columns, method='prep', max_rows = 1):
+        if method == 'prep':
+            return self.to_sql_prep(conn, schema, table, columns, max_rows=max_rows)
+        elif method =='string':
+            return self.to_sql_string(self, conn, schema, table, columns, max_rows=max_rows)
+
+ 
+    def to_sql_string(self, conn, schema, table, columns, max_rows = 300):
         colmap = self.set_to_sql_colmap(columns)
         src_cols = [x for x in colmap.values()]
         dest_columns = [x for x in colmap.keys()]
        
 
         sql_template = 'INSERT INTO {}.{} ({}) VALUES'
-        str_stmt = sql_template.format(schemaname,table,",".join(['"{}"'.format(x) for x in colmap]))
+        str_stmt = sql_template.format(schema,table,",".join(['"{}"'.format(x) for x in colmap]))
 
-        sql_cols_withtype = self.set_sql_datatype(dest_columns, conn, schemaname, table)
+        sql_cols_withtype = self.set_sql_datatype(dest_columns, conn, schema, table)
         sql_cols_withliteral = self.set_sql_literal(sql_cols_withtype, conn)
         
         # start insert to sql
         cursor = conn.cursor()
         temp_rows = []  
         total_rowcount = 0 # to hold total record affected
         for idx, values in self.iterrows(src_cols, row_type='list'):
-            ## question: can values and d_cols_withliteral align???????
+            ## question: can values and d_cols_withliteral align? dict python 3.7 is ordered and will solve it?
             sql_record = self.gen_sql_literal_record(values, sql_cols_withliteral)
             temp_rows.append(sql_record)
             if len(temp_rows) == max_rows:
                 stmt = str_stmt + ' {}'.format(",".join(temp_rows))
                 #log.debug(stmt)
                 cursor.execute(stmt)
                 total_rowcount += cursor.rowcount
@@ -128,20 +136,20 @@
         columnnames = [column[0] for column in cursor.description]
         tobj = Table('sql_typeinfo')
         for row in sql_type_info_tuple:
             tobj.insert(columnnames, row)        
         return tobj
     
 
-    def set_sql_datatype(self, dest_columns, conn, schemaname, table):
+    def set_sql_datatype(self, dest_columns, conn, schema, table):
         cursor = conn.cursor()
-        sql_columns = cursor.columns(schema=schemaname, table=table)
+        sql_columns = cursor.columns(schema=schema, table=table)
         columns = [column[0] for column in cursor.description]
         tobj = Table('sql_columns_')
-        for row in sql_columns: #cursor.columns(schema=schemaname, table=table):
+        for row in sql_columns: #cursor.columns(schema=schema, table=table):
             tobj.insert(columns, row)
         sql_columns_withtype = {}
         for col in dest_columns:
             _type = tobj.get_value('type_name', where = lambda row: row['column_name']==col)
             sql_columns_withtype[col] = _type
         return sql_columns_withtype
     
@@ -153,51 +161,44 @@
             prefix = sql_typeinfo_tab.get_value('literal_prefix',where=lambda row: row['type_name']==v)
             suffix = sql_typeinfo_tab.get_value('literal_suffix',where=lambda row: row['type_name']==v)
             literals = (prefix,suffix)
             sql_cols_withliteral[k] = literals
         return sql_cols_withliteral
 
 
-    def to_sql(self, conn, schemaname, table, columns, max_rows = 1):
+    def to_sql_prep(self, conn, schema, table, columns, max_rows = 1):
         if max_rows <= len(self): # validate max_row
             mrpb = max_rows # assign max row per batch
         else:
             #log.warning('Warning! max_rows {} set greater than totalrows {}. max_rows set to 1'.format(max_rows, len(self)))
             mrpb = 1
         numof_col = len(columns) # num of columns
 
         colmap = self.set_to_sql_colmap(columns)
         src_cols = [x for x in colmap.values()]
         dest_columns = [x for x in colmap.keys()]
         
         # create as prepared statement
         sql_template = 'INSERT INTO {}.{} ({}) VALUES {}'
         param_markers = self.gen_row_param_markers(numof_col, mrpb)
-        prep_stmt = sql_template.format(schemaname,table,",".join(['"{}"'.format(x) for x in dest_columns]),param_markers)
+        prep_stmt = sql_template.format(schema,table,",".join(['"{}"'.format(x) for x in dest_columns]),param_markers)
         cursor = conn.cursor()
         temp_rows = []
         total_rowcount = 0
         for idx, row in self.iterrows(src_cols, row_type='list'):
             for v in row:
                 temp_rows.append(v)
             if len(temp_rows) == (mrpb * numof_col):
-                try:
-                    cursor.execute(prep_stmt, temp_rows)
-                    total_rowcount += cursor.rowcount
-                except Exception as e:
-                    log.error(e)
-                    log.error('Error!! uploading data to dbms with the following data.')
-                    log.error(prep_stmt)
-                    data = [str(x) for x in temp_rows]
-                    log.error(','.join(data))
+                cursor.execute(prep_stmt, temp_rows)
+                total_rowcount += cursor.rowcount
                 temp_rows.clear()     
         
         if len(temp_rows) > 0: # if any reminder
             param_markers = self.gen_row_param_markers(numof_col, int(len(temp_rows)/numof_col))
-            prep_stmt = sql_template.format(schemaname,table,",".join(['"{}"'.format(x) for x in dest_columns]),param_markers)
+            prep_stmt = sql_template.format(schema,table,",".join(['"{}"'.format(x) for x in dest_columns]),param_markers)
             cursor.execute(prep_stmt, temp_rows)
             total_rowcount += cursor.rowcount
         return total_rowcount        
 
 
     def gen_row_param_markers(self,numof_col,num_row):
         param = "(" + ",".join("?"*numof_col) + ")"
@@ -468,15 +469,42 @@
         elif id is not None and option is None:
             row = Row(id)
         elif id is None and option == 'uuid':
             row = Row(uuid.uuid4())
         return row
 
 
-    def insert(self,columns,values):
+    def insert(self, record, columns=None):
+        """ restrict arguments for record insertion for this function as the followings:
+        1. a pair of columns and its single-row values
+        deprecated2. a pair of columns and its multiple-row values (as a list of tuple)
+        """
+
+        if isinstance(record, dict):
+            row = self.make_row()
+            for idx, (col, val) in enumerate(record.items()):
+                cell = self.make_cell(col,val)
+                row.add_cell(cell) # add to row
+            self.add_row(row)                                    
+        elif isinstance(columns,list) or isinstance(columns,tuple) or isinstance(record,list) or isinstance(record,tuple):
+            row = self.make_row()
+            for idx, col in enumerate(columns):
+                cell = self.make_cell(col,record[idx])
+                row.add_cell(cell) # add to rows
+            if self.__be is not None:
+                self.__temprows.append(json.dumps({v.columnid: v.value for v in row.cells.values()}))
+                if len(self.__temprows) == self.__be.max_row_for_sql_insert:
+                    self.add_row_into_be()
+            else:
+                self.add_row(row)    
+        else:
+            raise ValueError("Arg for record set for dictionary or list/tuple of values with list/tuple of columns.")
+            
+            
+    def insert_old(self,columns,values):
         """ restrict arguments for data insertion for this function as the followings:
         1. a pair of columns and its single-row values
         deprecated2. a pair of columns and its multiple-row values (as a list of tuple)
         """
 
         # if isinstance(values[0],tuple): # if no. 2
         #     for value in values:
```

## Comparing `bintang-0.1.5.dist-info/LICENSE` & `bintang-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bintang-0.1.5.dist-info/RECORD` & `bintang-0.1.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 bintang/__init__.py,sha256=UIuTaljC0GQNjj4BVS-PnG1uX2B54DR-LKlh14xIHR8,25
 bintang/besqlite.py,sha256=4vfwMAheTgqudMuCH3wlwwWyGJY5aVDd_tmTCiStcJg,6439
 bintang/cell.py,sha256=Zq7hS_ahK2iqIAVfdI2h-ZyHF7bfWpW-HCVcRTqIQaI,1319
 bintang/column.py,sha256=zTMxofr4FXGR95Zcru9G2DlR35e8I3IVifEzOissONM,566
-bintang/core.py,sha256=KfMExfMcDDR5w-qBmHwuYy6atwodpcKvrwpV673FcD4,23341
+bintang/core.py,sha256=1WUG_b9dE-hpgEHkwkxtc1PqpCV3i7WuVyiutIs7JoU,23341
 bintang/log.py,sha256=N6LImpolwYOJn4zW-nEpX6o63gInJKSzsw2NKM9V1sE,186
 bintang/row.py,sha256=I63-FY9p-lxmaeOOutKQbF9-jOPC3fTW-6frTqmzBOc,1385
-bintang/table.py,sha256=RU6ZJ34XOglDvHqGveTxrTubp2hqmo9KZ4tCLJ3x_x0,45915
+bintang/table.py,sha256=n_p6VKfEIfAXJkYKNw882ys4JstCj0aSQCb27HVktBQ,47313
 bintang/travdict.py,sha256=uWy-FHD6OJVbtcODBuyWBxyPz3nLFvGmTA9uCQ4PBVU,4981
-bintang-0.1.5.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
-bintang-0.1.5.dist-info/METADATA,sha256=aV3CCcZkhghwg_cjxc1CtnQGXMW6t4u8uh6BKWLJXz4,249
-bintang-0.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bintang-0.1.5.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
-bintang-0.1.5.dist-info/RECORD,,
+bintang-0.1.6.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
+bintang-0.1.6.dist-info/METADATA,sha256=qpo7RleIbqsiIg0xikdaa8Fvz_CaFbHldfS3lUyzHL4,249
+bintang-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bintang-0.1.6.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
+bintang-0.1.6.dist-info/RECORD,,
```

