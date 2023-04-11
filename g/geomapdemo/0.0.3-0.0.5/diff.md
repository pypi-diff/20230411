# Comparing `tmp/geomapdemo-0.0.3.tar.gz` & `tmp/geomapdemo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.0.3.tar", last modified: Sat Mar 18 03:15:38 2023, max compression
+gzip compressed data, was "geomapdemo-0.0.5.tar", last modified: Tue Apr 11 21:41:08 2023, max compression
```

## Comparing `geomapdemo-0.0.3.tar` & `geomapdemo-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 03:15:38.050113 geomapdemo-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-18 03:15:27.000000 geomapdemo-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-18 03:15:27.000000 geomapdemo-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-18 03:15:38.050113 geomapdemo-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-18 03:15:27.000000 geomapdemo-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 03:15:38.050113 geomapdemo-0.0.3/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-18 03:15:27.000000 geomapdemo-0.0.3/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-18 03:15:27.000000 geomapdemo-0.0.3/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 03:15:38.050113 geomapdemo-0.0.3/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-18 03:15:37.000000 geomapdemo-0.0.3/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-18 03:15:38.000000 geomapdemo-0.0.3/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 03:15:37.000000 geomapdemo-0.0.3/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 03:15:37.000000 geomapdemo-0.0.3/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-18 03:15:37.000000 geomapdemo-0.0.3/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 03:15:27.000000 geomapdemo-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-18 03:15:38.050113 geomapdemo-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-18 03:15:27.000000 geomapdemo-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 21:41:08.000000 geomapdemo-0.0.5/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 21:41:08.099320 geomapdemo-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-11 21:40:54.000000 geomapdemo-0.0.5/setup.py
```

### Comparing `geomapdemo-0.0.3/LICENSE` & `geomapdemo-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.0.3/PKG-INFO` & `geomapdemo-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.0.3
+Version: 0.0.5
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.0.3/README.md` & `geomapdemo-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.0.3/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.0.5/geomapdemo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.0.3
+Version: 0.0.5
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.0.3/setup.py` & `geomapdemo-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.0.3',
+    version='0.0.5',
     zip_safe=False,
 )
```

