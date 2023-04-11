# Comparing `tmp/chattychattybangbang-0.0.4.tar.gz` & `tmp/chattychattybangbang-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattychattybangbang-0.0.4.tar", last modified: Tue Apr 11 15:47:56 2023, max compression
+gzip compressed data, was "chattychattybangbang-0.0.5.tar", last modified: Tue Apr 11 15:52:20 2023, max compression
```

## Comparing `chattychattybangbang-0.0.4.tar` & `chattychattybangbang-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/chattychattybangbang/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvaluesare.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/castigators.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/jsonutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/openaicredentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/openutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/whereami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/chattychattybangbang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/castigateuntilvalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/castigateuntilvaluesare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/castigators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/jsonutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/openaicredentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/openutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/whereami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/setup.py
```

### Comparing `chattychattybangbang-0.0.4/LICENSE` & `chattychattybangbang-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.4/PKG-INFO` & `chattychattybangbang-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattychattybangbang
-Version: 0.0.4
+Version: 0.0.5
 Summary: chat utilities
 Home-page: https://github.com/chattychattybangbang/chattychattybangbang
 Author: chattychattybangbang
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chattychattybangbang-0.0.4/README.md` & `chattychattybangbang-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvalid.py` & `chattychattybangbang-0.0.5/chattychattybangbang/castigateuntilvalid.py`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvaluesare.py` & `chattychattybangbang-0.0.5/chattychattybangbang/castigateuntilvaluesare.py`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.4/chattychattybangbang/validators.py` & `chattychattybangbang-0.0.5/chattychattybangbang/validators.py`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.4/chattychattybangbang.egg-info/PKG-INFO` & `chattychattybangbang-0.0.5/chattychattybangbang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattychattybangbang
-Version: 0.0.4
+Version: 0.0.5
 Summary: chat utilities
 Home-page: https://github.com/chattychattybangbang/chattychattybangbang
 Author: chattychattybangbang
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chattychattybangbang-0.0.4/chattychattybangbang.egg-info/SOURCES.txt` & `chattychattybangbang-0.0.5/chattychattybangbang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.4/setup.py` & `chattychattybangbang-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="chattychattybangbang",
-    version="0.0.4",
+    version="0.0.5",
     description="chat utilities",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/chattychattybangbang/chattychattybangbang",
     author="chattychattybangbang",
     author_email="pcotton@intechinvestments.com",
     license="MIT",
```

