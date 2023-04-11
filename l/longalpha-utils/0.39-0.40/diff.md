# Comparing `tmp/longalpha_utils-0.39.tar.gz` & `tmp/longalpha_utils-0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.39.tar", last modified: Sat Mar 11 07:02:32 2023, max compression
+gzip compressed data, was "longalpha_utils-0.40.tar", last modified: Tue Apr 11 15:18:41 2023, max compression
```

## Comparing `longalpha_utils-0.39.tar` & `longalpha_utils-0.40.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 07:02:32.324563 longalpha_utils-0.39/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-11 07:02:32.324563 longalpha_utils-0.39/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 07:02:32.324563 longalpha_utils-0.39/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-11 07:02:22.000000 longalpha_utils-0.39/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-11 07:02:22.000000 longalpha_utils-0.39/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-11 07:02:22.000000 longalpha_utils-0.39/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-03-11 07:02:22.000000 longalpha_utils-0.39/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-03-11 07:02:22.000000 longalpha_utils-0.39/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-11 07:02:22.000000 longalpha_utils-0.39/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 07:02:32.324563 longalpha_utils-0.39/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-11 07:02:32.000000 longalpha_utils-0.39/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-11 07:02:32.000000 longalpha_utils-0.39/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 07:02:32.000000 longalpha_utils-0.39/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-11 07:02:32.000000 longalpha_utils-0.39/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-11 07:02:32.000000 longalpha_utils-0.39/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 07:02:32.324563 longalpha_utils-0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-11 07:02:22.000000 longalpha_utils-0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:41.233597 longalpha_utils-0.40/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 15:18:41.233597 longalpha_utils-0.40/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:41.233597 longalpha_utils-0.40/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-11 15:18:29.000000 longalpha_utils-0.40/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:18:41.233597 longalpha_utils-0.40/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 15:18:41.000000 longalpha_utils-0.40/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:18:41.233597 longalpha_utils-0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-11 15:18:29.000000 longalpha_utils-0.40/setup.py
```

### Comparing `longalpha_utils-0.39/longalpha_utils/messenger.py` & `longalpha_utils-0.40/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.39/longalpha_utils/transfers.py` & `longalpha_utils-0.40/longalpha_utils/transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from minio import Minio
 from pyspark.conf import SparkConf
 from pyspark.sql import SparkSession, DataFrame
 from sqlalchemy import Engine
 from sqlalchemy import create_engine
 from sqlalchemy import text
 
+
 class MinioWrapper:
     def __init__(self, minio_url, minio_access_key, minio_secret_key):
         self.minio_client = Minio(
             endpoint=minio_url,
             access_key=minio_access_key,
             secret_key=minio_secret_key,
             secure=False,
@@ -21,34 +22,45 @@
 
     def fput(
             self,
             file_path,
             bucket_name: str,
             object_name: str,
     ):
+        """
+        put a file to s3
+        Args:
+            file_path: path to the file
+            bucket_name: Minio bucket_name
+            object_name: object name in the minio bucket
+
+        Returns:
+
+        """
         self.minio_client.fput_object(bucket_name=bucket_name, object_name=object_name, file_path=file_path)
 
-    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str, file_format: str) -> None:
+    def put(self, dataframe: pd.DataFrame, bucket_name: str, object_name: str, file_format: str, index=False) -> None:
         """
         put a pandas frame to parquet in s3
 
         Args:
             dataframe: a pandas dataframe
             bucket_name: Minio bucket_name
-            object_name: path + file_name
+            object_name: object name in the minio bucket
             file_format: parquet or pickle
+            index: whether to save the index of the dataframe, only used for parquet
 
 
         Returns:
 
         """
         with tempfile.TemporaryDirectory() as temp_dir:
             path = os.path.join(temp_dir, object_name)
             if file_format == "parquet":
-                dataframe.to_parquet(path)
+                dataframe.to_parquet(path, index=index)
             elif file_format == "pickle":
                 dataframe.to_pickle(path)
             else:
                 raise ValueError("Incorrect file format")
             self.fput(file_path=path, bucket_name=bucket_name, object_name=object_name)
 
     def fget(self, file_path: str, bucket_name: str, object_name: str):
@@ -188,28 +200,30 @@
         .load()
     )
 
 
 def df_to_psql(
         df: pd.DataFrame,
         table_name: str,
+        index=False,
         dtype: Optional[Dict[str, Any]] = None,
         if_exists: str = "append",
         engine: Optional[Engine] = None,
         user_name: Optional[str] = None,
         password: Optional[str] = None,
         host_with_port: Optional[str] = None,
         db_name: Optional[str] = None,
         **kwargs: Any,
 ) -> None:
     """
     write a pandas dataframe to psql
     Args:
         df: pandas dataframe
         table_name: table name to write to psql
+        index: whether to write index to psql
         dtype: data type of column. If a dictionary is used, the keys should be the column names and the values
         should be the SQLAlchemy types or strings for the sqlite3 legacy mode
         if_exists: {‘fail’, ‘replace’, ‘append’}, default ‘append’. How to behave if the table already exists.
         fail: Raise a ValueError. replace: Drop the table before inserting new values append: Insert new values to
         the existing table.
         engine: sqlalchemy engine. If not None, then we will use this engine to write to psql.
         user_name: username of psql
@@ -223,15 +237,15 @@
     """
     if engine is not None and user_name is not None:
         raise ValueError("engine and user_name cannot be both not None")
     if engine is None and user_name is None:
         raise ValueError("engine and user_name cannot be both None")
     if engine is None:
         engine = create_engine(f"postgresql://{user_name}:{password}@{host_with_port}/{db_name}")
-    df.to_sql(table_name, con=engine, index=False, if_exists = if_exists, dtype = dtype, **kwargs)
+    df.to_sql(table_name, con=engine, index=index, if_exists = if_exists, dtype = dtype, **kwargs)
 
 
 def df_from_psql(
         sql: str,
         engine: Optional[Engine] = None,
         user_name: Optional[str] = None,
         password: Optional[str] = None,
```

### Comparing `longalpha_utils-0.39/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.40/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.39/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.40/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.39/setup.py` & `longalpha_utils-0.40/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.39",
+    version="0.40",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

