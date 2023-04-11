# Comparing `tmp/aliasmatching-0.2.0.tar.gz` & `tmp/aliasmatching-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliasmatching-0.2.0.tar", last modified: Tue Mar 28 15:25:21 2023, max compression
+gzip compressed data, was "aliasmatching-1.0.0.tar", last modified: Tue Apr 11 14:21:28 2023, max compression
```

## Comparing `aliasmatching-0.2.0.tar` & `aliasmatching-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-03-28 15:25:21.103299 aliasmatching-0.2.0/
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     1075 2023-03-24 07:57:50.000000 aliasmatching-0.2.0/LICENSE
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     1098 2023-03-28 15:25:21.103412 aliasmatching-0.2.0/PKG-INFO
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      587 2023-03-28 15:16:47.000000 aliasmatching-0.2.0/README.md
-drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-03-28 15:25:21.101165 aliasmatching-0.2.0/aliasmatching/
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      116 2023-03-28 15:11:44.000000 aliasmatching-0.2.0/aliasmatching/__init__.py
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     2118 2023-03-28 15:11:44.000000 aliasmatching-0.2.0/aliasmatching/matching.py
-drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-03-28 15:25:21.103057 aliasmatching-0.2.0/aliasmatching/utils/
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      253 2023-03-24 16:05:11.000000 aliasmatching-0.2.0/aliasmatching/utils/__init__.py
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     8816 2023-03-24 16:31:25.000000 aliasmatching-0.2.0/aliasmatching/utils/utils.py
-drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-03-28 15:25:21.102466 aliasmatching-0.2.0/aliasmatching.egg-info/
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     1098 2023-03-28 15:25:21.000000 aliasmatching-0.2.0/aliasmatching.egg-info/PKG-INFO
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      303 2023-03-28 15:25:21.000000 aliasmatching-0.2.0/aliasmatching.egg-info/SOURCES.txt
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)        1 2023-03-28 15:25:21.000000 aliasmatching-0.2.0/aliasmatching.egg-info/dependency_links.txt
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)       14 2023-03-28 15:25:21.000000 aliasmatching-0.2.0/aliasmatching.egg-info/top_level.txt
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      655 2023-03-28 15:00:05.000000 aliasmatching-0.2.0/pyproject.toml
--rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      116 2023-03-28 15:25:21.103825 aliasmatching-0.2.0/setup.cfg
+drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-04-11 14:21:28.025128 aliasmatching-1.0.0/
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     1075 2023-03-24 07:57:50.000000 aliasmatching-1.0.0/LICENSE
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     1098 2023-04-11 14:21:28.025226 aliasmatching-1.0.0/PKG-INFO
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      587 2023-03-28 15:16:47.000000 aliasmatching-1.0.0/README.md
+drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-04-11 14:21:28.022869 aliasmatching-1.0.0/aliasmatching/
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)       85 2023-04-11 13:50:59.000000 aliasmatching-1.0.0/aliasmatching/__init__.py
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     5280 2023-04-11 13:50:51.000000 aliasmatching-1.0.0/aliasmatching/matching.py
+drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-04-11 14:21:28.024781 aliasmatching-1.0.0/aliasmatching/utils/
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      398 2023-04-11 14:08:29.000000 aliasmatching-1.0.0/aliasmatching/utils/__init__.py
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     4755 2023-04-11 13:52:47.000000 aliasmatching-1.0.0/aliasmatching/utils/utils.py
+drwxr-xr-x   0 Farid.Bagirov   (602) staff       (20)        0 2023-04-11 14:21:28.024234 aliasmatching-1.0.0/aliasmatching.egg-info/
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)     1098 2023-04-11 14:21:28.000000 aliasmatching-1.0.0/aliasmatching.egg-info/PKG-INFO
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      303 2023-04-11 14:21:28.000000 aliasmatching-1.0.0/aliasmatching.egg-info/SOURCES.txt
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)        1 2023-04-11 14:21:28.000000 aliasmatching-1.0.0/aliasmatching.egg-info/dependency_links.txt
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)       14 2023-04-11 14:21:28.000000 aliasmatching-1.0.0/aliasmatching.egg-info/top_level.txt
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      655 2023-04-11 14:21:23.000000 aliasmatching-1.0.0/pyproject.toml
+-rw-r--r--   0 Farid.Bagirov   (602) staff       (20)      116 2023-04-11 14:21:28.025795 aliasmatching-1.0.0/setup.cfg
```

### Comparing `aliasmatching-0.2.0/LICENSE` & `aliasmatching-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aliasmatching-0.2.0/PKG-INFO` & `aliasmatching-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliasmatching
-Version: 0.2.0
+Version: 1.0.0
 Summary: alias matching toolkit
 Author-email: Farid <kraalfar@gmail.com>
 Project-URL: Homepage, https://github.com/JetBrains-Research/am
 Project-URL: Docs, https://batcore.readthedocs.io/en/latest/index.html#
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `aliasmatching-0.2.0/README.md` & `aliasmatching-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aliasmatching-0.2.0/aliasmatching.egg-info/PKG-INFO` & `aliasmatching-1.0.0/aliasmatching.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliasmatching
-Version: 0.2.0
+Version: 1.0.0
 Summary: alias matching toolkit
 Author-email: Farid <kraalfar@gmail.com>
 Project-URL: Homepage, https://github.com/JetBrains-Research/am
 Project-URL: Docs, https://batcore.readthedocs.io/en/latest/index.html#
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `aliasmatching-0.2.0/pyproject.toml` & `aliasmatching-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aliasmatching"
-version = "0.2.0"
+version = "1.0.0"
 authors = [
   { name="Farid", email="kraalfar@gmail.com" },
 ]
 description = "alias matching toolkit"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

