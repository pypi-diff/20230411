# Comparing `tmp/alethiometer-1.0.2.tar.gz` & `tmp/alethiometer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.0.2.tar", last modified: Fri Apr  7 18:05:35 2023, max compression
+gzip compressed data, was "alethiometer-1.0.3.tar", last modified: Tue Apr 11 12:17:54 2023, max compression
```

## Comparing `alethiometer-1.0.2.tar` & `alethiometer-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,28 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-07 18:05:35.240055 alethiometer-1.0.2/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.2/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1133 2023-04-07 18:05:35.240055 alethiometer-1.0.2/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      423 2023-04-07 16:53:17.000000 alethiometer-1.0.2/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-07 18:05:35.240055 alethiometer-1.0.2/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1133 2023-04-07 18:05:35.000000 alethiometer-1.0.2/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      205 2023-04-07 18:05:35.000000 alethiometer-1.0.2/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-07 18:05:35.000000 alethiometer-1.0.2/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-07 18:05:35.000000 alethiometer-1.0.2/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-07 18:05:35.000000 alethiometer-1.0.2/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-07 18:05:35.240055 alethiometer-1.0.2/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.2/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.053321 alethiometer-1.0.3/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.3/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1521 2023-04-11 12:17:54.053321 alethiometer-1.0.3/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      812 2023-04-11 12:16:45.000000 alethiometer-1.0.3/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.049321 alethiometer-1.0.3/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.3/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-11 12:12:58.000000 alethiometer-1.0.3/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.053321 alethiometer-1.0.3/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.3/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4252 2023-04-07 18:02:54.000000 alethiometer-1.0.3/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.3/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.3/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.3/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2445 2023-04-11 12:11:31.000000 alethiometer-1.0.3/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.053321 alethiometer-1.0.3/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1162 2023-04-07 15:02:02.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/synflow.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.049321 alethiometer-1.0.3/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1521 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      654 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-11 12:17:54.053321 alethiometer-1.0.3/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.3/setup.py
```

### Comparing `alethiometer-1.0.2/LICENSE` & `alethiometer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.2/setup.py` & `alethiometer-1.0.3/setup.py`

 * *Files identical despite different names*

