# Comparing `tmp/InCli-0.0.8.tar.gz` & `tmp/InCli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InCli-0.0.8.tar", last modified: Wed Dec  7 11:10:17 2022, max compression
+gzip compressed data, was "InCli-0.0.9.tar", last modified: Wed Dec  7 11:17:32 2022, max compression
```

## Comparing `InCli-0.0.8.tar` & `InCli-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:10:17.190256 InCli-0.0.8/
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:10:17.164111 InCli-0.0.8/InCli/
--rw-r--r--   0 uormaechea   (502) staff       (20)    11566 2022-12-07 10:09:10.000000 InCli-0.0.8/InCli/InCli.py
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:10:17.184220 InCli-0.0.8/InCli/SFAPI/
--rw-r--r--   0 uormaechea   (502) staff       (20)     8047 2022-12-06 00:07:38.000000 InCli-0.0.8/InCli/SFAPI/Sobjects.py
--rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-05 21:22:35.000000 InCli-0.0.8/InCli/SFAPI/__init__.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    18625 2022-12-06 22:52:03.000000 InCli-0.0.8/InCli/SFAPI/debugLogs.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    10877 2022-12-06 00:26:30.000000 InCli-0.0.8/InCli/SFAPI/digitalCommerce.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     4818 2022-12-06 22:29:53.000000 InCli-0.0.8/InCli/SFAPI/digitalCommerceUtil.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2142 2022-12-05 21:52:50.000000 InCli-0.0.8/InCli/SFAPI/file.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2244 2022-12-05 21:42:40.000000 InCli-0.0.8/InCli/SFAPI/jsonFile.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     9921 2022-12-05 21:12:09.000000 InCli-0.0.8/InCli/SFAPI/objectUtil.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     4116 2022-12-06 00:07:38.000000 InCli-0.0.8/InCli/SFAPI/query.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    21128 2022-12-06 22:48:38.000000 InCli-0.0.8/InCli/SFAPI/restClient.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2250 2022-12-05 21:22:33.000000 InCli-0.0.8/InCli/SFAPI/thread.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    11644 2022-12-06 22:30:56.000000 InCli-0.0.8/InCli/SFAPI/utils.py
--rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 08:57:08.000000 InCli-0.0.8/InCli/__init__.py
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:10:17.168531 InCli-0.0.8/InCli.egg-info/
--rw-r--r--   0 uormaechea   (502) staff       (20)      209 2022-12-07 11:10:17.000000 InCli-0.0.8/InCli.egg-info/PKG-INFO
--rw-r--r--   0 uormaechea   (502) staff       (20)      641 2022-12-07 11:10:17.000000 InCli-0.0.8/InCli.egg-info/SOURCES.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)        1 2022-12-07 11:10:17.000000 InCli-0.0.8/InCli.egg-info/dependency_links.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)       43 2022-12-07 11:10:17.000000 InCli-0.0.8/InCli.egg-info/entry_points.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)       30 2022-12-07 11:10:17.000000 InCli-0.0.8/InCli.egg-info/requires.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)        6 2022-12-07 11:10:17.000000 InCli-0.0.8/InCli.egg-info/top_level.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)     1068 2022-12-01 10:54:37.000000 InCli-0.0.8/LICENSE.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)      209 2022-12-07 11:10:17.189745 InCli-0.0.8/PKG-INFO
--rw-r--r--   0 uormaechea   (502) staff       (20)      117 2022-12-01 10:53:51.000000 InCli-0.0.8/README.md
--rw-r--r--   0 uormaechea   (502) staff       (20)      396 2022-12-07 11:10:10.000000 InCli-0.0.8/pyproject.toml
--rw-r--r--   0 uormaechea   (502) staff       (20)       38 2022-12-07 11:10:17.190416 InCli-0.0.8/setup.cfg
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:10:17.188938 InCli-0.0.8/test/
--rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 09:02:19.000000 InCli-0.0.8/test/__init__.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     1553 2022-12-06 22:33:07.000000 InCli-0.0.8/test/test_InCli.py
--rw-r--r--   0 uormaechea   (502) staff       (20)      683 2022-12-05 21:56:14.000000 InCli-0.0.8/test/test_file.py
--rw-r--r--   0 uormaechea   (502) staff       (20)      291 2022-12-05 21:43:56.000000 InCli-0.0.8/test/test_query.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     6341 2022-12-06 22:11:24.000000 InCli-0.0.8/test/test_restClient.py
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.773822 InCli-0.0.9/
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.754355 InCli-0.0.9/InCli/
+-rw-r--r--   0 uormaechea   (502) staff       (20)    11566 2022-12-07 10:09:10.000000 InCli-0.0.9/InCli/InCli.py
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.768408 InCli-0.0.9/InCli/SFAPI/
+-rw-r--r--   0 uormaechea   (502) staff       (20)     8047 2022-12-06 00:07:38.000000 InCli-0.0.9/InCli/SFAPI/Sobjects.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-05 21:22:35.000000 InCli-0.0.9/InCli/SFAPI/__init__.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    18625 2022-12-06 22:52:03.000000 InCli-0.0.9/InCli/SFAPI/debugLogs.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    10877 2022-12-06 00:26:30.000000 InCli-0.0.9/InCli/SFAPI/digitalCommerce.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     4818 2022-12-06 22:29:53.000000 InCli-0.0.9/InCli/SFAPI/digitalCommerceUtil.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     2142 2022-12-05 21:52:50.000000 InCli-0.0.9/InCli/SFAPI/file.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     2244 2022-12-05 21:42:40.000000 InCli-0.0.9/InCli/SFAPI/jsonFile.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     9921 2022-12-05 21:12:09.000000 InCli-0.0.9/InCli/SFAPI/objectUtil.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     4116 2022-12-06 00:07:38.000000 InCli-0.0.9/InCli/SFAPI/query.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    21128 2022-12-06 22:48:38.000000 InCli-0.0.9/InCli/SFAPI/restClient.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     2250 2022-12-05 21:22:33.000000 InCli-0.0.9/InCli/SFAPI/thread.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    11644 2022-12-06 22:30:56.000000 InCli-0.0.9/InCli/SFAPI/utils.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 08:57:08.000000 InCli-0.0.9/InCli/__init__.py
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.758279 InCli-0.0.9/InCli.egg-info/
+-rw-r--r--   0 uormaechea   (502) staff       (20)      209 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/PKG-INFO
+-rw-r--r--   0 uormaechea   (502) staff       (20)      641 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/SOURCES.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)        1 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/dependency_links.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)       43 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/entry_points.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)       20 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/requires.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)        6 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/top_level.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)     1068 2022-12-01 10:54:37.000000 InCli-0.0.9/LICENSE.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)      209 2022-12-07 11:17:32.773342 InCli-0.0.9/PKG-INFO
+-rw-r--r--   0 uormaechea   (502) staff       (20)      117 2022-12-01 10:53:51.000000 InCli-0.0.9/README.md
+-rw-r--r--   0 uormaechea   (502) staff       (20)      384 2022-12-07 11:17:21.000000 InCli-0.0.9/pyproject.toml
+-rw-r--r--   0 uormaechea   (502) staff       (20)       38 2022-12-07 11:17:32.773936 InCli-0.0.9/setup.cfg
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.772301 InCli-0.0.9/test/
+-rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 09:02:19.000000 InCli-0.0.9/test/__init__.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     1553 2022-12-06 22:33:07.000000 InCli-0.0.9/test/test_InCli.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)      683 2022-12-05 21:56:14.000000 InCli-0.0.9/test/test_file.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)      291 2022-12-05 21:43:56.000000 InCli-0.0.9/test/test_query.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     6341 2022-12-06 22:11:24.000000 InCli-0.0.9/test/test_restClient.py
```

### Comparing `InCli-0.0.8/InCli/InCli.py` & `InCli-0.0.9/InCli/InCli.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/Sobjects.py` & `InCli-0.0.9/InCli/SFAPI/Sobjects.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/debugLogs.py` & `InCli-0.0.9/InCli/SFAPI/debugLogs.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/digitalCommerce.py` & `InCli-0.0.9/InCli/SFAPI/digitalCommerce.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/digitalCommerceUtil.py` & `InCli-0.0.9/InCli/SFAPI/digitalCommerceUtil.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/file.py` & `InCli-0.0.9/InCli/SFAPI/file.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/jsonFile.py` & `InCli-0.0.9/InCli/SFAPI/jsonFile.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/objectUtil.py` & `InCli-0.0.9/InCli/SFAPI/objectUtil.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/query.py` & `InCli-0.0.9/InCli/SFAPI/query.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/restClient.py` & `InCli-0.0.9/InCli/SFAPI/restClient.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/thread.py` & `InCli-0.0.9/InCli/SFAPI/thread.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli/SFAPI/utils.py` & `InCli-0.0.9/InCli/SFAPI/utils.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/InCli.egg-info/SOURCES.txt` & `InCli-0.0.9/InCli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/LICENSE.txt` & `InCli-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/test/test_InCli.py` & `InCli-0.0.9/test/test_InCli.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/test/test_file.py` & `InCli-0.0.9/test/test_file.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.8/test/test_restClient.py` & `InCli-0.0.9/test/test_restClient.py`

 * *Files identical despite different names*

