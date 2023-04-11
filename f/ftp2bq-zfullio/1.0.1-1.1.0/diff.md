# Comparing `tmp/ftp2bq_zfullio-1.0.1.tar.gz` & `tmp/ftp2bq_zfullio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftp2bq_zfullio-1.0.1.tar", max compression
+gzip compressed data, was "ftp2bq_zfullio-1.1.0.tar", max compression
```

## Comparing `ftp2bq_zfullio-1.0.1.tar` & `ftp2bq_zfullio-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rwxr-xr-x   0        0        0     1069 2022-08-09 03:27:15.960000 ftp2bq_zfullio-1.0.1/LICENSE
--rwxr-xr-x   0        0        0       70 2022-08-09 05:46:01.374285 ftp2bq_zfullio-1.0.1/README.md
--rwxr-xr-x   0        0        0     1197 2023-01-23 04:35:15.145774 ftp2bq_zfullio-1.0.1/pyproject.toml
--rwxr-xr-x   0        0        0       59 2022-08-09 05:58:48.292321 ftp2bq_zfullio-1.0.1/src/ftp2bq_zfullio/__init__.py
--rwxr-xr-x   0        0        0     1325 2023-01-23 04:42:25.758640 ftp2bq_zfullio-1.0.1/src/ftp2bq_zfullio/ftp.py
--rwxr-xr-x   0        0        0     3675 2023-01-23 04:53:02.309340 ftp2bq_zfullio-1.0.1/src/ftp2bq_zfullio/general.py
--rwxr-xr-x   0        0        0     1253 2023-01-23 04:53:02.306007 ftp2bq_zfullio-1.0.1/src/ftp2bq_zfullio/sftp.py
--rw-r--r--   0        0        0      837 2023-01-23 04:56:05.735515 ftp2bq_zfullio-1.0.1/setup.py
--rw-r--r--   0        0        0      580 2023-01-23 04:56:05.736024 ftp2bq_zfullio-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2022-08-09 03:27:15.960000 ftp2bq_zfullio-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0       70 2022-08-09 05:46:01.374285 ftp2bq_zfullio-1.1.0/README.md
+-rwxr-xr-x   0        0        0     1191 2023-04-11 03:28:39.694665 ftp2bq_zfullio-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0       59 2022-08-09 05:58:48.292321 ftp2bq_zfullio-1.1.0/src/ftp2bq_zfullio/__init__.py
+-rwxr-xr-x   0        0        0     1325 2023-01-23 04:42:25.758640 ftp2bq_zfullio-1.1.0/src/ftp2bq_zfullio/ftp.py
+-rwxr-xr-x   0        0        0     3675 2023-01-23 04:53:02.309340 ftp2bq_zfullio-1.1.0/src/ftp2bq_zfullio/general.py
+-rwxr-xr-x   0        0        0     1253 2023-04-11 03:28:20.727649 ftp2bq_zfullio-1.1.0/src/ftp2bq_zfullio/sftp.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 ftp2bq_zfullio-1.1.0/PKG-INFO
```

### Comparing `ftp2bq_zfullio-1.0.1/LICENSE` & `ftp2bq_zfullio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ftp2bq_zfullio-1.0.1/pyproject.toml` & `ftp2bq_zfullio-1.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "ftp2bq_zfullio"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 paramiko = "^3"
-loguru = "^0.6"
-pandas = "^1.5"
-openpyxl = "^3.0"
+loguru = "^0"
+pandas = "^2"
+openpyxl = "^3"
 xmltodict = "^0.13.0"
 bq-easy-zfullio = "^1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `ftp2bq_zfullio-1.0.1/src/ftp2bq_zfullio/ftp.py` & `ftp2bq_zfullio-1.1.0/src/ftp2bq_zfullio/ftp.py`

 * *Files identical despite different names*

### Comparing `ftp2bq_zfullio-1.0.1/src/ftp2bq_zfullio/general.py` & `ftp2bq_zfullio-1.1.0/src/ftp2bq_zfullio/general.py`

 * *Files identical despite different names*

### Comparing `ftp2bq_zfullio-1.0.1/src/ftp2bq_zfullio/sftp.py` & `ftp2bq_zfullio-1.1.0/src/ftp2bq_zfullio/sftp.py`

 * *Files identical despite different names*

### Comparing `ftp2bq_zfullio-1.0.1/PKG-INFO` & `ftp2bq_zfullio-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ftp2bq-zfullio
-Version: 1.0.1
+Version: 1.1.0
 Summary: 
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bq-easy-zfullio (>=1,<2)
-Requires-Dist: loguru (>=0.6,<0.7)
-Requires-Dist: openpyxl (>=3.0,<4.0)
-Requires-Dist: pandas (>=1.5,<2.0)
+Requires-Dist: loguru (>=0,<1)
+Requires-Dist: openpyxl (>=3,<4)
+Requires-Dist: pandas (>=2,<3)
 Requires-Dist: paramiko (>=3,<4)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # (S)FTP to BQ
 
 Экспорт файлов с FTP и SFTP в BigQuery
```

