# Comparing `tmp/smooth_trajectory-0.0.6.tar.gz` & `tmp/smooth_trajectory-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smooth_trajectory-0.0.6.tar", last modified: Tue Apr  4 15:19:41 2023, max compression
+gzip compressed data, was "smooth_trajectory-0.1.0.tar", last modified: Tue Apr 11 16:32:54 2023, max compression
```

## Comparing `smooth_trajectory-0.0.6.tar` & `smooth_trajectory-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:19:41.995552 smooth_trajectory-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-04 15:19:41.995552 smooth_trajectory-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-04 15:19:32.000000 smooth_trajectory-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:19:41.995552 smooth_trajectory-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:19:41.995552 smooth_trajectory-0.0.6/smooth_trajectory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:19:32.000000 smooth_trajectory-0.0.6/smooth_trajectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-04 15:19:32.000000 smooth_trajectory-0.0.6/smooth_trajectory/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:19:41.995552 smooth_trajectory-0.0.6/smooth_trajectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-04 15:19:41.000000 smooth_trajectory-0.0.6/smooth_trajectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-04 15:19:41.000000 smooth_trajectory-0.0.6/smooth_trajectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:19:41.000000 smooth_trajectory-0.0.6/smooth_trajectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 15:19:41.000000 smooth_trajectory-0.0.6/smooth_trajectory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:19:41.995552 smooth_trajectory-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-04 15:19:32.000000 smooth_trajectory-0.0.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:32:54.422379 smooth_trajectory-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 16:32:54.422379 smooth_trajectory-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 16:32:44.000000 smooth_trajectory-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:32:54.422379 smooth_trajectory-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:32:54.422379 smooth_trajectory-0.1.0/smooth_trajectory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:32:44.000000 smooth_trajectory-0.1.0/smooth_trajectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-11 16:32:44.000000 smooth_trajectory-0.1.0/smooth_trajectory/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-11 16:32:44.000000 smooth_trajectory-0.1.0/smooth_trajectory/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:32:54.422379 smooth_trajectory-0.1.0/smooth_trajectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 16:32:54.000000 smooth_trajectory-0.1.0/smooth_trajectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-11 16:32:54.000000 smooth_trajectory-0.1.0/smooth_trajectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:32:54.000000 smooth_trajectory-0.1.0/smooth_trajectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 16:32:54.000000 smooth_trajectory-0.1.0/smooth_trajectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 16:32:54.000000 smooth_trajectory-0.1.0/smooth_trajectory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:32:54.422379 smooth_trajectory-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-11 16:32:44.000000 smooth_trajectory-0.1.0/tests/test.py
```

### Comparing `smooth_trajectory-0.0.6/PKG-INFO` & `smooth_trajectory-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth_trajectory
-Version: 0.0.6
+Version: 0.1.0
 Summary: A package for generating straight line trajectories in SE(3) with time scaling for smoothness
 Author-email: Ozan Tokatli <ozan.tokatli@gmail.com>
 Project-URL: Homepage, https://github.com/otokatli/pySmoothTrajectory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `smooth_trajectory-0.0.6/pyproject.toml` & `smooth_trajectory-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smooth_trajectory"
-version = "0.0.6"
+version = "0.1.0"
 authors = [
   { name="Ozan Tokatli", email="ozan.tokatli@gmail.com" },
 ]
 description = "A package for generating straight line trajectories in SE(3) with time scaling for smoothness"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
 ]
+dependencies = [
+    'numpy',
+    'scipy',
+]
 
 [project.urls]
 "Homepage" = "https://github.com/otokatli/pySmoothTrajectory"
```

### Comparing `smooth_trajectory-0.0.6/smooth_trajectory.egg-info/PKG-INFO` & `smooth_trajectory-0.1.0/smooth_trajectory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth-trajectory
-Version: 0.0.6
+Version: 0.1.0
 Summary: A package for generating straight line trajectories in SE(3) with time scaling for smoothness
 Author-email: Ozan Tokatli <ozan.tokatli@gmail.com>
 Project-URL: Homepage, https://github.com/otokatli/pySmoothTrajectory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `smooth_trajectory-0.0.6/tests/test.py` & `smooth_trajectory-0.1.0/tests/test.py`

 * *Files identical despite different names*

