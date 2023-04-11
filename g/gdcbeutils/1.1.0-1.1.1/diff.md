# Comparing `tmp/gdcbeutils-1.1.0.tar.gz` & `tmp/gdcbeutils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdcbeutils-1.1.0.tar", last modified: Tue Apr 11 00:25:22 2023, max compression
+gzip compressed data, was "gdcbeutils-1.1.1.tar", last modified: Tue Apr 11 00:36:45 2023, max compression
```

## Comparing `gdcbeutils-1.1.0.tar` & `gdcbeutils-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.786495 gdcbeutils-1.1.0/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      678 2023-04-11 00:25:22.785908 gdcbeutils-1.1.0/PKG-INFO
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      715 2023-04-11 00:24:54.000000 gdcbeutils-1.1.0/pyproject.toml
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      114 2023-02-07 10:04:56.000000 gdcbeutils-1.1.0/readme.md
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       38 2023-04-11 00:25:22.786690 gdcbeutils-1.1.0/setup.cfg
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.723754 gdcbeutils-1.1.0/src/
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.734745 gdcbeutils-1.1.0/src/gdcbeutils/
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.741886 gdcbeutils-1.1.0/src/gdcbeutils/AWS/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      260 2023-02-20 13:45:48.000000 gdcbeutils-1.1.0/src/gdcbeutils/AWS/Client.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.752556 gdcbeutils-1.1.0/src/gdcbeutils/AWS/Services/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      168 2023-02-20 13:45:48.000000 gdcbeutils-1.1.0/src/gdcbeutils/AWS/Services/DynamoDb.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     2893 2023-02-20 13:45:48.000000 gdcbeutils-1.1.0/src/gdcbeutils/AWS/Services/ParameterStore.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     3716 2023-02-27 10:10:28.000000 gdcbeutils-1.1.0/src/gdcbeutils/AWS/Services/SimpleQueueService.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.753727 gdcbeutils-1.1.0/src/gdcbeutils/Api/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      202 2023-02-20 13:45:48.000000 gdcbeutils-1.1.0/src/gdcbeutils/Api/__init__.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.755501 gdcbeutils-1.1.0/src/gdcbeutils/Api/mail/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)        0 2023-02-20 13:45:48.000000 gdcbeutils-1.1.0/src/gdcbeutils/Api/mail/__init__.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      115 2023-02-21 12:47:17.000000 gdcbeutils-1.1.0/src/gdcbeutils/__init__.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.762612 gdcbeutils-1.1.0/src/gdcbeutils/database/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       88 2023-02-13 13:51:57.000000 gdcbeutils-1.1.0/src/gdcbeutils/database/__init__.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     4116 2023-02-20 13:45:43.000000 gdcbeutils-1.1.0/src/gdcbeutils/database/mongodb.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     4310 2023-02-28 09:55:09.000000 gdcbeutils-1.1.0/src/gdcbeutils/database/mysqldb.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.769631 gdcbeutils-1.1.0/src/gdcbeutils/database/testing/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      433 2023-02-17 11:13:44.000000 gdcbeutils-1.1.0/src/gdcbeutils/database/testing/__init__.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     4327 2023-04-11 00:24:01.000000 gdcbeutils-1.1.0/src/gdcbeutils/database/testing/context.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     2225 2023-02-20 13:45:43.000000 gdcbeutils-1.1.0/src/gdcbeutils/database/testing/decorator.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.772744 gdcbeutils-1.1.0/src/gdcbeutils/models/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       92 2023-02-08 13:40:48.000000 gdcbeutils-1.1.0/src/gdcbeutils/models/__init__.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.781146 gdcbeutils-1.1.0/src/gdcbeutils/models/pagination/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      154 2023-02-08 13:40:42.000000 gdcbeutils-1.1.0/src/gdcbeutils/models/pagination/__init__.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      761 2023-04-11 00:24:46.000000 gdcbeutils-1.1.0/src/gdcbeutils/models/pagination/paginated.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     1304 2023-02-08 13:37:47.000000 gdcbeutils-1.1.0/src/gdcbeutils/models/pagination/paginated_results.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.784596 gdcbeutils-1.1.0/src/gdcbeutils/parsing/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)        0 2023-02-21 07:44:00.000000 gdcbeutils-1.1.0/src/gdcbeutils/parsing/__init__.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      877 2023-02-21 12:42:34.000000 gdcbeutils-1.1.0/src/gdcbeutils/parsing/date.py
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     1107 2023-02-21 12:48:55.000000 gdcbeutils-1.1.0/src/gdcbeutils/parsing/dict.py
-drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:25:22.740313 gdcbeutils-1.1.0/src/gdcbeutils.egg-info/
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      678 2023-04-11 00:25:22.000000 gdcbeutils-1.1.0/src/gdcbeutils.egg-info/PKG-INFO
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      949 2023-04-11 00:25:22.000000 gdcbeutils-1.1.0/src/gdcbeutils.egg-info/SOURCES.txt
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)        1 2023-04-11 00:25:22.000000 gdcbeutils-1.1.0/src/gdcbeutils.egg-info/dependency_links.txt
--rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       11 2023-04-11 00:25:22.000000 gdcbeutils-1.1.0/src/gdcbeutils.egg-info/top_level.txt
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.795498 gdcbeutils-1.1.1/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      678 2023-04-11 00:36:45.794806 gdcbeutils-1.1.1/PKG-INFO
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      715 2023-04-11 00:36:35.000000 gdcbeutils-1.1.1/pyproject.toml
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      114 2023-02-07 10:04:56.000000 gdcbeutils-1.1.1/readme.md
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       38 2023-04-11 00:36:45.795695 gdcbeutils-1.1.1/setup.cfg
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.755112 gdcbeutils-1.1.1/src/
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.766889 gdcbeutils-1.1.1/src/gdcbeutils/
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.770750 gdcbeutils-1.1.1/src/gdcbeutils/AWS/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      260 2023-02-20 13:45:48.000000 gdcbeutils-1.1.1/src/gdcbeutils/AWS/Client.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.773950 gdcbeutils-1.1.1/src/gdcbeutils/AWS/Services/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      168 2023-02-20 13:45:48.000000 gdcbeutils-1.1.1/src/gdcbeutils/AWS/Services/DynamoDb.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     2893 2023-02-20 13:45:48.000000 gdcbeutils-1.1.1/src/gdcbeutils/AWS/Services/ParameterStore.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     3716 2023-02-27 10:10:28.000000 gdcbeutils-1.1.1/src/gdcbeutils/AWS/Services/SimpleQueueService.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.775923 gdcbeutils-1.1.1/src/gdcbeutils/Api/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      202 2023-02-20 13:45:48.000000 gdcbeutils-1.1.1/src/gdcbeutils/Api/__init__.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.777422 gdcbeutils-1.1.1/src/gdcbeutils/Api/mail/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)        0 2023-02-20 13:45:48.000000 gdcbeutils-1.1.1/src/gdcbeutils/Api/mail/__init__.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      115 2023-02-21 12:47:17.000000 gdcbeutils-1.1.1/src/gdcbeutils/__init__.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.780944 gdcbeutils-1.1.1/src/gdcbeutils/database/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       88 2023-02-13 13:51:57.000000 gdcbeutils-1.1.1/src/gdcbeutils/database/__init__.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     4116 2023-02-20 13:45:43.000000 gdcbeutils-1.1.1/src/gdcbeutils/database/mongodb.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     4310 2023-02-28 09:55:09.000000 gdcbeutils-1.1.1/src/gdcbeutils/database/mysqldb.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.785272 gdcbeutils-1.1.1/src/gdcbeutils/database/testing/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      433 2023-02-17 11:13:44.000000 gdcbeutils-1.1.1/src/gdcbeutils/database/testing/__init__.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     4327 2023-04-11 00:24:01.000000 gdcbeutils-1.1.1/src/gdcbeutils/database/testing/context.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     2225 2023-02-20 13:45:43.000000 gdcbeutils-1.1.1/src/gdcbeutils/database/testing/decorator.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.786190 gdcbeutils-1.1.1/src/gdcbeutils/models/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       92 2023-02-08 13:40:48.000000 gdcbeutils-1.1.1/src/gdcbeutils/models/__init__.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.790013 gdcbeutils-1.1.1/src/gdcbeutils/models/pagination/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      154 2023-02-08 13:40:42.000000 gdcbeutils-1.1.1/src/gdcbeutils/models/pagination/__init__.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      770 2023-04-11 00:36:16.000000 gdcbeutils-1.1.1/src/gdcbeutils/models/pagination/paginated.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     1304 2023-02-08 13:37:47.000000 gdcbeutils-1.1.1/src/gdcbeutils/models/pagination/paginated_results.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.793865 gdcbeutils-1.1.1/src/gdcbeutils/parsing/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)        0 2023-02-21 07:44:00.000000 gdcbeutils-1.1.1/src/gdcbeutils/parsing/__init__.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      877 2023-02-21 12:42:34.000000 gdcbeutils-1.1.1/src/gdcbeutils/parsing/date.py
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)     1107 2023-02-21 12:48:55.000000 gdcbeutils-1.1.1/src/gdcbeutils/parsing/dict.py
+drwxr-xr-x   0 gustavodinizdacorte   (501) staff       (20)        0 2023-04-11 00:36:45.770059 gdcbeutils-1.1.1/src/gdcbeutils.egg-info/
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      678 2023-04-11 00:36:45.000000 gdcbeutils-1.1.1/src/gdcbeutils.egg-info/PKG-INFO
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)      949 2023-04-11 00:36:45.000000 gdcbeutils-1.1.1/src/gdcbeutils.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)        1 2023-04-11 00:36:45.000000 gdcbeutils-1.1.1/src/gdcbeutils.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavodinizdacorte   (501) staff       (20)       11 2023-04-11 00:36:45.000000 gdcbeutils-1.1.1/src/gdcbeutils.egg-info/top_level.txt
```

### Comparing `gdcbeutils-1.1.0/PKG-INFO` & `gdcbeutils-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdcbeutils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple package with utility functions for everyday projects in Python
 Author-email: Gustavo Diniz da Corte <gustavodacorte@gmail.com>
 Project-URL: Homepage, https://github.com/Gdcorte/base-utils-backend-lib
 Project-URL: Bug Tracker, https://github.com/Gdcorte/base-utils-backend-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdcbeutils-1.1.0/pyproject.toml` & `gdcbeutils-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdcbeutils"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Gustavo Diniz da Corte", email="gustavodacorte@gmail.com" },
 ]
 description = "Simple package with utility functions for everyday projects in Python"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/AWS/Services/ParameterStore.py` & `gdcbeutils-1.1.1/src/gdcbeutils/AWS/Services/ParameterStore.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/AWS/Services/SimpleQueueService.py` & `gdcbeutils-1.1.1/src/gdcbeutils/AWS/Services/SimpleQueueService.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/database/mongodb.py` & `gdcbeutils-1.1.1/src/gdcbeutils/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/database/mysqldb.py` & `gdcbeutils-1.1.1/src/gdcbeutils/database/mysqldb.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/database/testing/context.py` & `gdcbeutils-1.1.1/src/gdcbeutils/database/testing/context.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/database/testing/decorator.py` & `gdcbeutils-1.1.1/src/gdcbeutils/database/testing/decorator.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/models/pagination/paginated.py` & `gdcbeutils-1.1.1/src/gdcbeutils/models/pagination/paginated.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from pydantic import BaseModel, validator
 
 
 class Pagination(BaseModel):
     """Defines a pagination model"""
 
-    page: int
-    per_page: int
+    page: int = 1
+    per_page: int = 20
 
     @classmethod
     def from_params(cls, obj: Dict[str, Any] | None = None):
         """Defines a pagination from default parameters"""
         if not obj:
             obj = {}
```

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/models/pagination/paginated_results.py` & `gdcbeutils-1.1.1/src/gdcbeutils/models/pagination/paginated_results.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/parsing/date.py` & `gdcbeutils-1.1.1/src/gdcbeutils/parsing/date.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils/parsing/dict.py` & `gdcbeutils-1.1.1/src/gdcbeutils/parsing/dict.py`

 * *Files identical despite different names*

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils.egg-info/PKG-INFO` & `gdcbeutils-1.1.1/src/gdcbeutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdcbeutils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple package with utility functions for everyday projects in Python
 Author-email: Gustavo Diniz da Corte <gustavodacorte@gmail.com>
 Project-URL: Homepage, https://github.com/Gdcorte/base-utils-backend-lib
 Project-URL: Bug Tracker, https://github.com/Gdcorte/base-utils-backend-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gdcbeutils-1.1.0/src/gdcbeutils.egg-info/SOURCES.txt` & `gdcbeutils-1.1.1/src/gdcbeutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

