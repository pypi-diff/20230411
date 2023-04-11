# Comparing `tmp/morphqs-0.1.2.tar.gz` & `tmp/morphqs-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphqs-0.1.2.tar", last modified: Thu Mar 30 18:18:59 2023, max compression
+gzip compressed data, was "morphqs-0.1.22.tar", last modified: Tue Apr 11 14:28:42 2023, max compression
```

## Comparing `morphqs-0.1.2.tar` & `morphqs-0.1.22.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.883911 morphqs-0.1.2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.2/LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      924 2023-03-30 18:18:59.882615 morphqs-0.1.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.2/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.826450 morphqs-0.1.2/morphqs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      154 2023-03-29 15:19:51.000000 morphqs-0.1.2/morphqs/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.869945 morphqs-0.1.2/morphqs/components/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.2/morphqs/components/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2023-03-30 18:18:06.000000 morphqs-0.1.2/morphqs/components/ansible.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5908 2023-03-30 17:03:38.000000 morphqs-0.1.2/morphqs/components/integrations.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6361 2023-03-30 18:16:28.000000 morphqs-0.1.2/morphqs/components/uchigheredmsp.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.878601 morphqs-0.1.2/morphqs/logging/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.2/morphqs/logging/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.2/morphqs/logging/loghandler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.2/morphqs/morphclass.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.853906 morphqs-0.1.2/morphqs.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      924 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-03-30 18:18:59.884626 morphqs-0.1.2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1024 2023-03-30 18:18:56.000000 morphqs-0.1.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.148152 morphqs-0.1.22/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.22/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-11 14:28:42.146829 morphqs-0.1.22/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.22/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.080416 morphqs-0.1.22/morphqs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      201 2023-04-07 16:34:53.000000 morphqs-0.1.22/morphqs/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.131799 morphqs-0.1.22/morphqs/components/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.22/morphqs/components/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.22/morphqs/components/ansible.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3444 2023-04-07 16:04:30.000000 morphqs-0.1.22/morphqs/components/integrations.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.22/morphqs/components/uchigheredmsp.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-04-07 16:15:46.000000 morphqs-0.1.22/morphqs/components/usecasedeployment.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.142191 morphqs-0.1.22/morphqs/logging/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.22/morphqs/logging/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.22/morphqs/logging/loghandler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.22/morphqs/morphclass.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.105519 morphqs-0.1.22/morphqs.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-11 14:28:42.148900 morphqs-0.1.22/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-11 14:28:41.000000 morphqs-0.1.22/setup.py
```

### Comparing `morphqs-0.1.2/LICENSE.txt` & `morphqs-0.1.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.2/PKG-INFO` & `morphqs-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.2
+Version: 0.1.22
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.2/morphqs/components/uchigheredmsp.py` & `morphqs-0.1.22/morphqs/components/uchigheredmsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
                                     "code": "jythonTask"
                                 },
                                 "visibility": "private",
                                 "labels": [
                                     "higher_ed_msp", "setup", "demo", "poc", "example"
                                 ],
                                 "taskOptions": {
-                                    "pythonAdditionalPackages": "requests morphcp",
+                                    "pythonAdditionalPackages": "requests morphcp click",
                                     "username": None,
                                     "password": None,
                                     "passwordHash": None,
                                     "pythonBinary": None,
                                     "host": None,
                                     "localScriptGitId": None,
                                     "port": None,
-                                    "pythonArgs": "higher_ed",
+                                    "pythonArgs": "highered",
                                     "localScriptGitRef": None
                                 },
                                 "file": {
                                     "sourceType": "repository",
                                     "contentRef": branch,
                                     "contentPath": hchighered_contentPath,
                                     "repository": {
```

### Comparing `morphqs-0.1.2/morphqs/logging/loghandler.py` & `morphqs-0.1.22/morphqs/logging/loghandler.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.2/morphqs/morphclass.py` & `morphqs-0.1.22/morphqs/morphclass.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.2/morphqs.egg-info/PKG-INFO` & `morphqs-0.1.22/morphqs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.2
+Version: 0.1.22
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.2/setup.py` & `morphqs-0.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Jared Lutgen",
     author_email="jlutgen@morpheusdata.com",
     name='morphqs',
     license="MIT",
     description='Tool utilized to deploy some basic concepts for the Morpheus Data Platform',
-    version='v0.1.2',
+    version='v0.1.22',
     long_description=README,
     url='https://gitlab.com/jaredlutgen/morphqs',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['requests'],
     classifiers=[
         # Trove classifiers
```

