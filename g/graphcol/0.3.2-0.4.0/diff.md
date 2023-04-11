# Comparing `tmp/graphcol-0.3.2.tar.gz` & `tmp/graphcol-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphcol-0.3.2.tar", max compression
+gzip compressed data, was "graphcol-0.4.0.tar", max compression
```

## Comparing `graphcol-0.3.2.tar` & `graphcol-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2023-02-21 03:37:42.752867 graphcol-0.3.2/graphcol/__init__.py
--rw-r--r--   0        0        0     2838 2023-02-21 03:24:37.885924 graphcol-0.3.2/graphcol/exatos.py
--rw-r--r--   0        0        0     9339 2023-02-20 22:27:54.565982 graphcol-0.3.2/graphcol/gulosos.py
--rw-r--r--   0        0        0    31354 2023-02-21 03:24:18.161739 graphcol-0.3.2/graphcol/metaheuristicas.py
--rw-r--r--   0        0        0     2853 2023-02-20 22:27:54.565982 graphcol-0.3.2/graphcol/visual.py
--rw-r--r--   0        0        0      502 2023-02-21 03:37:51.136531 graphcol-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 graphcol-0.3.2/setup.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 graphcol-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-11 02:41:34.331640 graphcol-0.4.0/graphcol/__init__.py
+-rw-r--r--   0        0        0     9596 2023-04-11 02:56:47.194557 graphcol-0.4.0/graphcol/exatos.py
+-rw-r--r--   0        0        0     9339 2023-02-20 22:27:54.565982 graphcol-0.4.0/graphcol/gulosos.py
+-rw-r--r--   0        0        0    31354 2023-02-21 03:24:18.161739 graphcol-0.4.0/graphcol/metaheuristicas.py
+-rw-r--r--   0        0        0     2853 2023-02-20 22:27:54.565982 graphcol-0.4.0/graphcol/visual.py
+-rw-r--r--   0        0        0      502 2023-04-11 02:57:01.574780 graphcol-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 graphcol-0.4.0/setup.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 graphcol-0.4.0/PKG-INFO
```

### Comparing `graphcol-0.3.2/graphcol/gulosos.py` & `graphcol-0.4.0/graphcol/gulosos.py`

 * *Files identical despite different names*

### Comparing `graphcol-0.3.2/graphcol/metaheuristicas.py` & `graphcol-0.4.0/graphcol/metaheuristicas.py`

 * *Files identical despite different names*

### Comparing `graphcol-0.3.2/graphcol/visual.py` & `graphcol-0.4.0/graphcol/visual.py`

 * *Files identical despite different names*

### Comparing `graphcol-0.3.2/setup.py` & `graphcol-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cairocffi>=1.3.0,<2.0.0',
  'igraph>=0.9.9,<0.10.0',
  'matplotlib>=3.6.0,<4.0.0',
  'numpy>=1.23.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'graphcol',
-    'version': '0.3.2',
+    'version': '0.4.0',
     'description': '',
     'long_description': 'None',
     'author': 'WLAraujo',
     'author_email': 'lima.wesleyaraujo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `graphcol-0.3.2/PKG-INFO` & `graphcol-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphcol
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 Author: WLAraujo
 Author-email: lima.wesleyaraujo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

