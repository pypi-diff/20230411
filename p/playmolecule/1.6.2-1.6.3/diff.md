# Comparing `tmp/playmolecule-1.6.2.tar.gz` & `tmp/playmolecule-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.6.2.tar", last modified: Tue Apr 11 13:35:44 2023, max compression
+gzip compressed data, was "playmolecule-1.6.3.tar", last modified: Tue Apr 11 14:00:56 2023, max compression
```

## Comparing `playmolecule-1.6.2.tar` & `playmolecule-1.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:35:44.855669 playmolecule-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-11 13:35:22.000000 playmolecule-1.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 13:35:22.000000 playmolecule-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 13:35:44.855669 playmolecule-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 13:35:22.000000 playmolecule-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:35:44.851669 playmolecule-1.6.2/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32923 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:35:44.855669 playmolecule-1.6.2/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 13:35:22.000000 playmolecule-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:35:44.855669 playmolecule-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 13:35:22.000000 playmolecule-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:00:56.456857 playmolecule-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-11 14:00:44.000000 playmolecule-1.6.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 14:00:44.000000 playmolecule-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 14:00:56.456857 playmolecule-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 14:00:44.000000 playmolecule-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:00:56.456857 playmolecule-1.6.3/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32923 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:00:56.456857 playmolecule-1.6.3/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 14:00:44.000000 playmolecule-1.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:00:56.456857 playmolecule-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 14:00:44.000000 playmolecule-1.6.3/setup.py
```

### Comparing `playmolecule-1.6.2/LICENSE.md` & `playmolecule-1.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/PKG-INFO` & `playmolecule-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.2
+Version: 1.6.3
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.2/playmolecule/__init__.py` & `playmolecule-1.6.3/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/_test_funcs.py` & `playmolecule-1.6.3/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/config.py` & `playmolecule-1.6.3/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/datacenter.py` & `playmolecule-1.6.3/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/devutils.py` & `playmolecule-1.6.3/playmolecule/devutils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/func2argparse.py` & `playmolecule-1.6.3/playmolecule/func2argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,20 +120,27 @@
     sig = inspect.signature(func)
     doc = func.__doc__
     if doc is None:
         raise RuntimeError("Could not find documentation in the function...")
 
     argdocs, description, name = _parse_docs(doc)
 
-    parser = argparse.ArgumentParser(
-        name,
-        description=description,
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        exit_on_error=exit_on_error,
-    )
+    try:
+        parser = argparse.ArgumentParser(
+            name,
+            description=description,
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+            exit_on_error=exit_on_error,
+        )
+    except:
+        parser = argparse.ArgumentParser(
+            name,
+            description=description,
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        )
     if allow_conf_yaml:
         parser.add_argument(
             "--conf",
             help="Configuration YAML file to set all parameters",
             type=open,
             action=lambda *x, **y: LoadFromFile(*x, **y, unmatched_args=unmatched_args),
         )
```

### Comparing `playmolecule-1.6.2/playmolecule/job.py` & `playmolecule-1.6.3/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/jsonlogger.py` & `playmolecule-1.6.3/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/local.py` & `playmolecule-1.6.3/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/playqueue.py` & `playmolecule-1.6.3/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/session.py` & `playmolecule-1.6.3/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule/utils.py` & `playmolecule-1.6.3/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.6.3/playmolecule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.2
+Version: 1.6.3
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.2/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.6.3/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.2/setup.py` & `playmolecule-1.6.3/setup.py`

 * *Files identical despite different names*

