# Comparing `tmp/zodiax-0.3.1.tar.gz` & `tmp/zodiax-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodiax-0.3.1.tar", last modified: Fri Mar 24 06:12:44 2023, max compression
+gzip compressed data, was "zodiax-0.3.2.tar", last modified: Tue Apr 11 08:02:37 2023, max compression
```

## Comparing `zodiax-0.3.1.tar` & `zodiax-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-03-24 06:12:44.574335 zodiax-0.3.1/
--rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.3.1/.gitignore
--rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.3.1/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.3.1/MANIFEST.ini
--rw-r--r--   0 louis      (501) staff       (20)      489 2023-03-24 06:12:44.574179 zodiax-0.3.1/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4292 2023-03-20 23:44:32.000000 zodiax-0.3.1/README.md
--rw-r--r--   0 louis      (501) staff       (20)     2992 2023-03-20 01:49:16.000000 zodiax-0.3.1/mkdocs.yml
--rw-r--r--   0 louis      (501) staff       (20)       55 2023-03-09 09:55:10.000000 zodiax-0.3.1/requirements.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-03-24 06:12:44.574385 zodiax-0.3.1/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)     1509 2023-03-20 01:40:07.000000 zodiax-0.3.1/setup.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-03-24 06:12:44.571548 zodiax-0.3.1/tests/
--rw-r--r--   0 louis      (501) staff       (20)     6936 2023-03-22 06:53:45.000000 zodiax-0.3.1/tests/test_base.py
--rw-r--r--   0 louis      (501) staff       (20)      824 2023-03-20 01:40:07.000000 zodiax-0.3.1/tests/test_equinox.py
--rw-r--r--   0 louis      (501) staff       (20)      700 2023-03-20 01:40:07.000000 zodiax-0.3.1/tests/test_optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)      668 2023-03-20 01:40:07.000000 zodiax-0.3.1/tests/test_serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)      366 2023-03-20 01:40:07.000000 zodiax-0.3.1/tests/test_tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-03-24 06:12:44.572459 zodiax-0.3.1/zodiax/
--rw-r--r--   0 louis      (501) staff       (20)      428 2023-03-24 06:11:31.000000 zodiax-0.3.1/zodiax/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    21739 2023-03-22 06:51:07.000000 zodiax-0.3.1/zodiax/base.py
--rw-r--r--   0 louis      (501) staff       (20)     5112 2023-03-20 01:40:07.000000 zodiax-0.3.1/zodiax/equinox.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-03-24 06:12:44.573969 zodiax-0.3.1/zodiax/experimental/
--rw-r--r--   0 louis      (501) staff       (20)      238 2023-03-22 01:43:50.000000 zodiax-0.3.1/zodiax/experimental/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     1290 2023-03-22 01:46:09.000000 zodiax-0.3.1/zodiax/experimental/jit.py
--rw-r--r--   0 louis      (501) staff       (20)    17276 2023-03-22 02:19:04.000000 zodiax-0.3.1/zodiax/experimental/serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2101 2023-03-23 00:20:31.000000 zodiax-0.3.1/zodiax/optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2104 2023-03-20 01:40:07.000000 zodiax-0.3.1/zodiax/tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-03-24 06:12:44.573285 zodiax-0.3.1/zodiax.egg-info/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-03-24 06:12:44.573561 zodiax-0.3.1/zodiax.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.3.1/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.3.1/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)      489 2023-03-24 06:12:44.000000 zodiax-0.3.1/zodiax.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      645 2023-03-24 06:12:44.000000 zodiax-0.3.1/zodiax.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-03-24 06:12:44.000000 zodiax-0.3.1/zodiax.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       49 2023-03-24 06:12:44.000000 zodiax-0.3.1/zodiax.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       27 2023-03-24 06:12:44.000000 zodiax-0.3.1/zodiax.egg-info/top_level.txt
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.631184 zodiax-0.3.2/
+-rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.3.2/.gitignore
+-rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.3.2/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.3.2/MANIFEST.ini
+-rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:02:37.631045 zodiax-0.3.2/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     4292 2023-03-28 01:43:37.000000 zodiax-0.3.2/README.md
+-rw-r--r--   0 louis      (501) staff       (20)     2992 2023-03-20 01:49:16.000000 zodiax-0.3.2/mkdocs.yml
+-rw-r--r--   0 louis      (501) staff       (20)       55 2023-03-09 09:55:10.000000 zodiax-0.3.2/requirements.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-04-11 08:02:37.631225 zodiax-0.3.2/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)     1508 2023-04-11 07:58:40.000000 zodiax-0.3.2/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.628709 zodiax-0.3.2/tests/
+-rw-r--r--   0 louis      (501) staff       (20)     6936 2023-03-22 06:53:45.000000 zodiax-0.3.2/tests/test_base.py
+-rw-r--r--   0 louis      (501) staff       (20)      824 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_equinox.py
+-rw-r--r--   0 louis      (501) staff       (20)      700 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      668 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      366 2023-03-20 01:40:07.000000 zodiax-0.3.2/tests/test_tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.629487 zodiax-0.3.2/zodiax/
+-rw-r--r--   0 louis      (501) staff       (20)      428 2023-04-11 08:00:25.000000 zodiax-0.3.2/zodiax/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    21739 2023-03-22 06:51:07.000000 zodiax-0.3.2/zodiax/base.py
+-rw-r--r--   0 louis      (501) staff       (20)     5112 2023-03-20 01:40:07.000000 zodiax-0.3.2/zodiax/equinox.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.630834 zodiax-0.3.2/zodiax/experimental/
+-rw-r--r--   0 louis      (501) staff       (20)      238 2023-03-22 01:43:50.000000 zodiax-0.3.2/zodiax/experimental/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     1290 2023-03-22 01:46:09.000000 zodiax-0.3.2/zodiax/experimental/jit.py
+-rw-r--r--   0 louis      (501) staff       (20)    17276 2023-03-22 02:19:04.000000 zodiax-0.3.2/zodiax/experimental/serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2101 2023-03-23 00:20:31.000000 zodiax-0.3.2/zodiax/optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2104 2023-03-20 01:40:07.000000 zodiax-0.3.2/zodiax/tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.630132 zodiax-0.3.2/zodiax.egg-info/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:02:37.630447 zodiax-0.3.2/zodiax.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.3.2/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.3.2/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      645 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       49 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       27 2023-04-11 08:02:37.000000 zodiax-0.3.2/zodiax.egg-info/top_level.txt
```

### Comparing `zodiax-0.3.1/LICENSE` & `zodiax-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/README.md` & `zodiax-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/mkdocs.yml` & `zodiax-0.3.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/setup.py` & `zodiax-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 with open('requirements.txt') as f:
     install_requires = f.read().splitlines()
 # 2. What dependencies required to run the unit tests? (i.e. `pytest --remote-data`)
 # tests_require = ['pytest', 'pytest-cov', 'pytest-remotedata']
 
 
 setuptools.setup(
-    python_requires='>=3.10, <4',
+    python_requires='>=3.8, <4',
     name="zodiax",
     version=find_version("zodiax", "__init__.py"),
     description="Equinox extension for scientific programming",
     long_description=long_description,
 
     author="Louis Desdoigts",
     author_email="Louis.Desdoigts@sydney.edu.au",
```

### Comparing `zodiax-0.3.1/tests/test_base.py` & `zodiax-0.3.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/tests/test_equinox.py` & `zodiax-0.3.2/tests/test_equinox.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/tests/test_optimisation.py` & `zodiax-0.3.2/tests/test_optimisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/tests/test_serialisation.py` & `zodiax-0.3.2/tests/test_serialisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/zodiax/base.py` & `zodiax-0.3.2/zodiax/base.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/zodiax/equinox.py` & `zodiax-0.3.2/zodiax/equinox.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/zodiax/experimental/jit.py` & `zodiax-0.3.2/zodiax/experimental/jit.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/zodiax/experimental/serialisation.py` & `zodiax-0.3.2/zodiax/experimental/serialisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/zodiax/optimisation.py` & `zodiax-0.3.2/zodiax/optimisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/zodiax/tree.py` & `zodiax-0.3.2/zodiax/tree.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.1/zodiax.egg-info/SOURCES.txt` & `zodiax-0.3.2/zodiax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

