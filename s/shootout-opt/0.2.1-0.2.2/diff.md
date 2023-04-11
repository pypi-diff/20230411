# Comparing `tmp/shootout-opt-0.2.1.tar.gz` & `tmp/shootout-opt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shootout-opt-0.2.1.tar", last modified: Tue Apr 11 14:43:59 2023, max compression
+gzip compressed data, was "shootout-opt-0.2.2.tar", last modified: Tue Apr 11 14:50:51 2023, max compression
```

## Comparing `shootout-opt-0.2.1.tar` & `shootout-opt-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.765065 shootout-opt-0.2.1/
--rw-r--r--   0 cohen    (11323) creatis    (500)     1072 2023-04-11 14:42:58.000000 shootout-opt-0.2.1/LICENSE
--rw-r--r--   0 cohen    (11323) creatis    (500)     3228 2023-04-11 14:43:59.764065 shootout-opt-0.2.1/PKG-INFO
--rw-r--r--   0 cohen    (11323) creatis    (500)     1590 2023-04-11 12:06:25.000000 shootout-opt-0.2.1/README.md
--rw-r--r--   0 cohen    (11323) creatis    (500)      693 2023-04-11 14:43:47.000000 shootout-opt-0.2.1/pyproject.toml
--rw-r--r--   0 cohen    (11323) creatis    (500)       38 2023-04-11 14:43:59.765065 shootout-opt-0.2.1/setup.cfg
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.761065 shootout-opt-0.2.1/shootout/
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.762065 shootout-opt-0.2.1/shootout/methods/
--rw-r--r--   0 cohen    (11323) creatis    (500)      121 2022-09-01 08:14:10.000000 shootout-opt-0.2.1/shootout/methods/pipeplines.py
--rw-r--r--   0 cohen    (11323) creatis    (500)      972 2022-07-05 13:34:55.000000 shootout-opt-0.2.1/shootout/methods/plotters.py
--rw-r--r--   0 cohen    (11323) creatis    (500)    19524 2023-04-11 12:08:25.000000 shootout-opt-0.2.1/shootout/methods/post_processors.py
--rw-r--r--   0 cohen    (11323) creatis    (500)    10547 2023-04-11 12:08:25.000000 shootout-opt-0.2.1/shootout/methods/runners.py
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.763065 shootout-opt-0.2.1/shootout/tests/
--rw-r--r--   0 cohen    (11323) creatis    (500)        0 2022-09-23 13:27:36.000000 shootout-opt-0.2.1/shootout/tests/test_plotters.py
--rw-r--r--   0 cohen    (11323) creatis    (500)     2746 2023-04-11 09:42:06.000000 shootout-opt-0.2.1/shootout/tests/test_post_processors.py
--rw-r--r--   0 cohen    (11323) creatis    (500)     1918 2023-04-11 12:08:25.000000 shootout-opt-0.2.1/shootout/tests/test_runners.py
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.764065 shootout-opt-0.2.1/shootout_opt.egg-info/
--rw-r--r--   0 cohen    (11323) creatis    (500)     3228 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/PKG-INFO
--rw-r--r--   0 cohen    (11323) creatis    (500)      437 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/SOURCES.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)        1 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/dependency_links.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)       87 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/requires.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)        9 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/top_level.txt
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.437531 shootout-opt-0.2.2/
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1072 2023-04-11 14:42:58.000000 shootout-opt-0.2.2/LICENSE
+-rw-r--r--   0 cohen    (11323) creatis    (500)     3268 2023-04-11 14:50:51.436531 shootout-opt-0.2.2/PKG-INFO
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1630 2023-04-11 14:48:11.000000 shootout-opt-0.2.2/README.md
+-rw-r--r--   0 cohen    (11323) creatis    (500)      693 2023-04-11 14:50:42.000000 shootout-opt-0.2.2/pyproject.toml
+-rw-r--r--   0 cohen    (11323) creatis    (500)       38 2023-04-11 14:50:51.437531 shootout-opt-0.2.2/setup.cfg
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.432531 shootout-opt-0.2.2/shootout/
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.434531 shootout-opt-0.2.2/shootout/methods/
+-rw-r--r--   0 cohen    (11323) creatis    (500)      121 2022-09-01 08:14:10.000000 shootout-opt-0.2.2/shootout/methods/pipeplines.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)      972 2022-07-05 13:34:55.000000 shootout-opt-0.2.2/shootout/methods/plotters.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)    19524 2023-04-11 12:08:25.000000 shootout-opt-0.2.2/shootout/methods/post_processors.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)    10547 2023-04-11 12:08:25.000000 shootout-opt-0.2.2/shootout/methods/runners.py
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.435531 shootout-opt-0.2.2/shootout/tests/
+-rw-r--r--   0 cohen    (11323) creatis    (500)        0 2022-09-23 13:27:36.000000 shootout-opt-0.2.2/shootout/tests/test_plotters.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)     2746 2023-04-11 09:42:06.000000 shootout-opt-0.2.2/shootout/tests/test_post_processors.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1918 2023-04-11 12:08:25.000000 shootout-opt-0.2.2/shootout/tests/test_runners.py
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:50:51.436531 shootout-opt-0.2.2/shootout_opt.egg-info/
+-rw-r--r--   0 cohen    (11323) creatis    (500)     3268 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/PKG-INFO
+-rw-r--r--   0 cohen    (11323) creatis    (500)      437 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)        1 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)       87 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/requires.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)        9 2023-04-11 14:50:51.000000 shootout-opt-0.2.2/shootout_opt.egg-info/top_level.txt
```

### Comparing `shootout-opt-0.2.1/LICENSE` & `shootout-opt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.1/PKG-INFO` & `shootout-opt-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootout-opt
-Version: 0.2.1
+Version: 0.2.2
 Summary: Run algorithms, store and compare their outputs
 Author-email: "Jeremy E. Cohen" <jeremy.cohen@cnrs.fr>
 License: MIT License
         
         Copyright (c) 2023 Jeremy E. Cohen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,19 @@
 Plus I am a very chaotic person, changing workflow every single paper. So I needed some tools to balance this entropy and make my life easier.
 
 ## What this does
 - Using a decorator function @run_and_track(), one may run a script many times with user-defined hyperparameters grid; store all the results in clearly formatted pandas dataframe usable by plotly express.
 - provide a few helpful functions for processing this dataframe, to produce interesting comparison plots (convergence plots, who is fastest at given threshold plots)
 
 ## Installation
-For now, no pip installation is provided. You can clone the repo and run
+The package can be pip installed using
+```python
+pip install shootout-opt
+```
+or by cloning the repo and running
 ```python
 pip install -e .
 ```
 with root in the root folder of this package.
 
 ## TODOS
 - TODO: auto-tests on push on github
```

### Comparing `shootout-opt-0.2.1/README.md` & `shootout-opt-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 Plus I am a very chaotic person, changing workflow every single paper. So I needed some tools to balance this entropy and make my life easier.
 
 ## What this does
 - Using a decorator function @run_and_track(), one may run a script many times with user-defined hyperparameters grid; store all the results in clearly formatted pandas dataframe usable by plotly express.
 - provide a few helpful functions for processing this dataframe, to produce interesting comparison plots (convergence plots, who is fastest at given threshold plots)
 
 ## Installation
-For now, no pip installation is provided. You can clone the repo and run
+The package can be pip installed using
+```python
+pip install shootout-opt
+```
+or by cloning the repo and running
 ```python
 pip install -e .
 ```
 with root in the root folder of this package.
 
 ## TODOS
 - TODO: auto-tests on push on github
```

### Comparing `shootout-opt-0.2.1/pyproject.toml` & `shootout-opt-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shootout-opt"
-version = "0.2.1"
+version = "0.2.2"
 description="Run algorithms, store and compare their outputs"
 authors=[{name= "Jeremy E. Cohen", email = "jeremy.cohen@cnrs.fr"}]
 license={ file = "LICENSE"}
 readme = "README.md"
 keywords = ["numerical optimisation", "visualisation", "python"]
 dependencies = [
     "numpy >= 1.23",
```

### Comparing `shootout-opt-0.2.1/shootout/methods/plotters.py` & `shootout-opt-0.2.2/shootout/methods/plotters.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.1/shootout/methods/post_processors.py` & `shootout-opt-0.2.2/shootout/methods/post_processors.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.1/shootout/methods/runners.py` & `shootout-opt-0.2.2/shootout/methods/runners.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.1/shootout/tests/test_post_processors.py` & `shootout-opt-0.2.2/shootout/tests/test_post_processors.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.1/shootout/tests/test_runners.py` & `shootout-opt-0.2.2/shootout/tests/test_runners.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2.1/shootout_opt.egg-info/PKG-INFO` & `shootout-opt-0.2.2/shootout_opt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shootout-opt
-Version: 0.2.1
+Version: 0.2.2
 Summary: Run algorithms, store and compare their outputs
 Author-email: "Jeremy E. Cohen" <jeremy.cohen@cnrs.fr>
 License: MIT License
         
         Copyright (c) 2023 Jeremy E. Cohen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,19 @@
 Plus I am a very chaotic person, changing workflow every single paper. So I needed some tools to balance this entropy and make my life easier.
 
 ## What this does
 - Using a decorator function @run_and_track(), one may run a script many times with user-defined hyperparameters grid; store all the results in clearly formatted pandas dataframe usable by plotly express.
 - provide a few helpful functions for processing this dataframe, to produce interesting comparison plots (convergence plots, who is fastest at given threshold plots)
 
 ## Installation
-For now, no pip installation is provided. You can clone the repo and run
+The package can be pip installed using
+```python
+pip install shootout-opt
+```
+or by cloning the repo and running
 ```python
 pip install -e .
 ```
 with root in the root folder of this package.
 
 ## TODOS
 - TODO: auto-tests on push on github
```

