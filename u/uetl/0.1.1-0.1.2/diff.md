# Comparing `tmp/uetl-0.1.1.tar.gz` & `tmp/uetl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uetl-0.1.1.tar", last modified: Sat Dec 24 18:48:12 2022, max compression
+gzip compressed data, was "uetl-0.1.2.tar", last modified: Tue Apr 11 13:52:56 2023, max compression
```

## Comparing `uetl-0.1.1.tar` & `uetl-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2022-12-24 18:48:12.094461 uetl-0.1.1/
--rw-r--r--   0 andre     (1000) andre     (1000)     1070 2020-04-28 23:16:31.000000 uetl-0.1.1/LICENSE
--rw-r--r--   0 andre     (1000) andre     (1000)       29 2020-04-29 20:31:51.000000 uetl-0.1.1/MANIFEST.in
--rw-rw-r--   0 andre     (1000) andre     (1000)     4235 2022-12-24 18:48:12.094461 uetl-0.1.1/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)     2761 2022-12-24 18:29:35.000000 uetl-0.1.1/README.md
--rw-rw-r--   0 andre     (1000) andre     (1000)       38 2022-12-24 18:48:12.094461 uetl-0.1.1/setup.cfg
--rw-rw-r--   0 andre     (1000) andre     (1000)     1008 2022-12-24 18:32:02.000000 uetl-0.1.1/setup.py
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2022-12-24 18:48:12.094461 uetl-0.1.1/src/
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2022-12-24 18:48:12.094461 uetl-0.1.1/src/uetl.egg-info/
--rw-rw-r--   0 andre     (1000) andre     (1000)     4235 2022-12-24 18:48:11.000000 uetl-0.1.1/src/uetl.egg-info/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)      209 2022-12-24 18:48:11.000000 uetl-0.1.1/src/uetl.egg-info/SOURCES.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        1 2022-12-24 18:48:11.000000 uetl-0.1.1/src/uetl.egg-info/dependency_links.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)       98 2022-12-24 18:48:11.000000 uetl-0.1.1/src/uetl.egg-info/requires.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        5 2022-12-24 18:48:11.000000 uetl-0.1.1/src/uetl.egg-info/top_level.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)    14433 2022-12-24 18:27:50.000000 uetl-0.1.1/src/uetl.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-11 13:52:56.692147 uetl-0.1.2/
+-rw-r--r--   0 andre     (1000) andre     (1000)     1070 2020-04-28 23:16:31.000000 uetl-0.1.2/LICENSE
+-rw-r--r--   0 andre     (1000) andre     (1000)       29 2020-04-29 20:31:51.000000 uetl-0.1.2/MANIFEST.in
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-11 13:52:56.692147 uetl-0.1.2/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)     2763 2022-12-24 18:51:51.000000 uetl-0.1.2/README.md
+-rw-rw-r--   0 andre     (1000) andre     (1000)       38 2023-04-11 13:52:56.692147 uetl-0.1.2/setup.cfg
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1008 2023-04-11 12:46:31.000000 uetl-0.1.2/setup.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-11 13:52:56.692147 uetl-0.1.2/src/
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-11 13:52:56.692147 uetl-0.1.2/src/uetl.egg-info/
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)      209 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/SOURCES.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        1 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/dependency_links.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)       98 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/requires.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        5 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/top_level.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)    14560 2023-04-11 12:44:35.000000 uetl-0.1.2/src/uetl.py
```

### Comparing `uetl-0.1.1/LICENSE` & `uetl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uetl-0.1.1/README.md` & `uetl-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ## 3rd example - Use MssqlSrc.query()
 db = uetl.MssqlSrc('testdb', host, port, base, user, pswd)
 print(
     db.query('select @@version')
 )
 ```
 
-#### MS SQL Source Object
+#### Firebird Source Object
 
 ```python
 import uetl
 import pandas as pd
 
 host = '192.168.1.1'
 port = 3050
```

### Comparing `uetl-0.1.1/setup.py` & `uetl-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='uetl',
-    version='0.1.1',
+    version='0.1.2',
     description='Minimalist python ETL library.',
     py_modules=["uetl"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent",
     ],
```

### Comparing `uetl-0.1.1/src/uetl.py` & `uetl-0.1.2/src/uetl.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 import pandas as pd
 import pandas.io.sql as sqlio
 import sqlalchemy
 import psycopg2
 import fdb
 from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
+from sqlalchemy.sql import text
 
 class DataWarehouse():
     """DataWarehouse class
     """
 
     def __init__(self, name, dbms, host, port, base, user, pswd):
         # Define class attributes
@@ -103,15 +104,15 @@
         if conn == -1:
             # DBMS Unreachable!
             return False
 
         conn.set_isolation_level(ISOLATION_LEVEL_AUTOCOMMIT)
 
         cur = conn.cursor()
-        cur.execute("CREATE DATABASE {}  ;".format(self.base))
+        cur.execute(text("CREATE DATABASE {}  ;".format(self.base)))
 
         conn.close()
 
         return True
 
     def check_table(self, table_name):
         """Check if Data Warehouse's table exists.
@@ -130,20 +131,23 @@
                 True if table exist, or False otherwise
         """
         conn = self.get_conn()
         if conn == -1: # DBMS Unreachable!
             return False
         else:
             cur = conn.cursor()
-            cur.execute("""
-              select exists(
+            cur.execute(
+                text(
+                    """ select exists(
                         select *
                         from information_schema.tables
                         where table_name=%s
-                       )""", (table_name,)
+                       )
+                       """, (table_name,)
+                )
             )
             status = cur.fetchone()[0]
             conn.close()
         return status
 
     def create_tables(self, tables, verbose=False):
         """Creates Data Warehouse's Tables, if it doesn't exist.
@@ -176,15 +180,15 @@
 
                 conn = self.get_conn()
                 if conn == -1: # DBMS Unreachable!
                     print('ERROR: Fail creating tables!')
                     return False
                 else:
                     cur = conn.cursor()
-                    cur.execute(tables[table])
+                    cur.execute(text(tables[table]))
                     conn.commit()
                     if not self.check_table(table): # Fail to create table
                         print('ERROR: Fail creating tables!')
                         return False
                     if(verbose): print('Success!')
                     conn.close()
 
@@ -217,17 +221,17 @@
 
         if conn == -1:
             print("ERROR: query(): Unable to connect to the database.")
             return False
         else:
             cur = conn.cursor()
             if cascade:
-                cur.execute('TRUNCATE {} CASCADE'.format(table_name))
+                cur.execute(text('TRUNCATE {} CASCADE'.format(table_name)))
             else:
-                cur.execute('TRUNCATE {}'.format(table_name))
+                cur.execute(text('TRUNCATE {}'.format(table_name)))
             conn.commit()
             conn.close()
             if(verbose): print('table truncated.')
             return True
 
     def write(self, table_name, df, verbose=False, chunksize=None):
         """Write dataframe to table. Dataframe's Index will be used as a column
```

