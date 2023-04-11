# Comparing `tmp/shootout-opt-0.2.tar.gz` & `tmp/shootout-opt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shootout-opt-0.2.tar", last modified: Tue Apr 11 14:21:25 2023, max compression
+gzip compressed data, was "shootout-opt-0.2.1.tar", last modified: Tue Apr 11 14:43:59 2023, max compression
```

## Comparing `shootout-opt-0.2.tar` & `shootout-opt-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:21:25.770358 shootout-opt-0.2/
--rw-r--r--   0 cohen    (11323) creatis    (500)      183 2023-04-11 14:21:25.769358 shootout-opt-0.2/PKG-INFO
--rw-r--r--   0 cohen    (11323) creatis    (500)       84 2023-04-11 13:15:29.000000 shootout-opt-0.2/pyproject.toml
--rw-r--r--   0 cohen    (11323) creatis    (500)       38 2023-04-11 14:21:25.770358 shootout-opt-0.2/setup.cfg
--rw-r--r--   0 cohen    (11323) creatis    (500)      621 2023-04-11 14:18:12.000000 shootout-opt-0.2/setup.py
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:21:25.766358 shootout-opt-0.2/shootout/
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:21:25.767358 shootout-opt-0.2/shootout/methods/
--rw-r--r--   0 cohen    (11323) creatis    (500)      121 2022-09-01 08:14:10.000000 shootout-opt-0.2/shootout/methods/pipeplines.py
--rw-r--r--   0 cohen    (11323) creatis    (500)      972 2022-07-05 13:34:55.000000 shootout-opt-0.2/shootout/methods/plotters.py
--rw-r--r--   0 cohen    (11323) creatis    (500)    19524 2023-04-11 12:08:25.000000 shootout-opt-0.2/shootout/methods/post_processors.py
--rw-r--r--   0 cohen    (11323) creatis    (500)    10547 2023-04-11 12:08:25.000000 shootout-opt-0.2/shootout/methods/runners.py
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:21:25.768358 shootout-opt-0.2/shootout/tests/
--rw-r--r--   0 cohen    (11323) creatis    (500)        0 2022-09-23 13:27:36.000000 shootout-opt-0.2/shootout/tests/test_plotters.py
--rw-r--r--   0 cohen    (11323) creatis    (500)     2746 2023-04-11 09:42:06.000000 shootout-opt-0.2/shootout/tests/test_post_processors.py
--rw-r--r--   0 cohen    (11323) creatis    (500)     1918 2023-04-11 12:08:25.000000 shootout-opt-0.2/shootout/tests/test_runners.py
-drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:21:25.769358 shootout-opt-0.2/shootout_opt.egg-info/
--rw-r--r--   0 cohen    (11323) creatis    (500)      183 2023-04-11 14:21:25.000000 shootout-opt-0.2/shootout_opt.egg-info/PKG-INFO
--rw-r--r--   0 cohen    (11323) creatis    (500)      428 2023-04-11 14:21:25.000000 shootout-opt-0.2/shootout_opt.egg-info/SOURCES.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)        1 2023-04-11 14:21:25.000000 shootout-opt-0.2/shootout_opt.egg-info/dependency_links.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)       46 2023-04-11 14:21:25.000000 shootout-opt-0.2/shootout_opt.egg-info/requires.txt
--rw-r--r--   0 cohen    (11323) creatis    (500)        9 2023-04-11 14:21:25.000000 shootout-opt-0.2/shootout_opt.egg-info/top_level.txt
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.765065 shootout-opt-0.2.1/
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1072 2023-04-11 14:42:58.000000 shootout-opt-0.2.1/LICENSE
+-rw-r--r--   0 cohen    (11323) creatis    (500)     3228 2023-04-11 14:43:59.764065 shootout-opt-0.2.1/PKG-INFO
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1590 2023-04-11 12:06:25.000000 shootout-opt-0.2.1/README.md
+-rw-r--r--   0 cohen    (11323) creatis    (500)      693 2023-04-11 14:43:47.000000 shootout-opt-0.2.1/pyproject.toml
+-rw-r--r--   0 cohen    (11323) creatis    (500)       38 2023-04-11 14:43:59.765065 shootout-opt-0.2.1/setup.cfg
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.761065 shootout-opt-0.2.1/shootout/
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.762065 shootout-opt-0.2.1/shootout/methods/
+-rw-r--r--   0 cohen    (11323) creatis    (500)      121 2022-09-01 08:14:10.000000 shootout-opt-0.2.1/shootout/methods/pipeplines.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)      972 2022-07-05 13:34:55.000000 shootout-opt-0.2.1/shootout/methods/plotters.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)    19524 2023-04-11 12:08:25.000000 shootout-opt-0.2.1/shootout/methods/post_processors.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)    10547 2023-04-11 12:08:25.000000 shootout-opt-0.2.1/shootout/methods/runners.py
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.763065 shootout-opt-0.2.1/shootout/tests/
+-rw-r--r--   0 cohen    (11323) creatis    (500)        0 2022-09-23 13:27:36.000000 shootout-opt-0.2.1/shootout/tests/test_plotters.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)     2746 2023-04-11 09:42:06.000000 shootout-opt-0.2.1/shootout/tests/test_post_processors.py
+-rw-r--r--   0 cohen    (11323) creatis    (500)     1918 2023-04-11 12:08:25.000000 shootout-opt-0.2.1/shootout/tests/test_runners.py
+drwxr-xr-x   0 cohen    (11323) creatis    (500)        0 2023-04-11 14:43:59.764065 shootout-opt-0.2.1/shootout_opt.egg-info/
+-rw-r--r--   0 cohen    (11323) creatis    (500)     3228 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/PKG-INFO
+-rw-r--r--   0 cohen    (11323) creatis    (500)      437 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)        1 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)       87 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/requires.txt
+-rw-r--r--   0 cohen    (11323) creatis    (500)        9 2023-04-11 14:43:59.000000 shootout-opt-0.2.1/shootout_opt.egg-info/top_level.txt
```

### Comparing `shootout-opt-0.2/shootout/methods/plotters.py` & `shootout-opt-0.2.1/shootout/methods/plotters.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2/shootout/methods/post_processors.py` & `shootout-opt-0.2.1/shootout/methods/post_processors.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2/shootout/methods/runners.py` & `shootout-opt-0.2.1/shootout/methods/runners.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2/shootout/tests/test_post_processors.py` & `shootout-opt-0.2.1/shootout/tests/test_post_processors.py`

 * *Files identical despite different names*

### Comparing `shootout-opt-0.2/shootout/tests/test_runners.py` & `shootout-opt-0.2.1/shootout/tests/test_runners.py`

 * *Files identical despite different names*

