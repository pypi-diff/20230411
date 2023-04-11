# Comparing `tmp/jaxrie-2.tar.gz` & `tmp/jaxrie-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrie-2.tar", last modified: Tue Apr 11 06:28:50 2023, max compression
+gzip compressed data, was "jaxrie-3.tar", last modified: Tue Apr 11 06:37:21 2023, max compression
```

## Comparing `jaxrie-2.tar` & `jaxrie-3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-2/README.md
--rw-r--r--   0        0        0     3959 2023-04-11 06:28:50.427612 jaxrie-2/pyproject.toml
--rw-r--r--   0        0        0      240 2023-04-11 06:06:22.543202 jaxrie-2/src/jaxrie/__init__.py
--rw-r--r--   0        0        0       18 2023-04-11 06:25:07.371360 jaxrie-2/src/jaxrie/__version__.py
--rw-r--r--   0        0        0      183 2023-04-07 20:42:03.402217 jaxrie-2/src/jaxrie/manifold/__init__.py
--rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-2/src/jaxrie/manifold/base.py
--rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-2/src/jaxrie/manifold/lorentz.py
--rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-2/src/jaxrie/manifold/math.py
--rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-2/src/jaxrie/manifold/stereographic.py
--rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-2/src/jaxrie/modules/__init__.py
--rw-r--r--   0        0        0     4816 2023-04-11 06:13:42.344173 jaxrie-2/src/jaxrie/modules/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-2/src/jaxrie/nets/__init__.py
--rw-r--r--   0        0        0     2342 2023-04-11 06:23:40.424342 jaxrie-2/src/jaxrie/nets/basic.py
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-2/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-3/README.md
+-rw-r--r--   0        0        0     3959 2023-04-11 06:37:21.819071 jaxrie-3/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-04-11 06:06:22.543202 jaxrie-3/src/jaxrie/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-11 06:36:55.909478 jaxrie-3/src/jaxrie/__version__.py
+-rw-r--r--   0        0        0      183 2023-04-07 20:42:03.402217 jaxrie-3/src/jaxrie/manifold/__init__.py
+-rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-3/src/jaxrie/manifold/base.py
+-rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-3/src/jaxrie/manifold/lorentz.py
+-rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-3/src/jaxrie/manifold/math.py
+-rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-3/src/jaxrie/manifold/stereographic.py
+-rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-3/src/jaxrie/modules/__init__.py
+-rw-r--r--   0        0        0     4816 2023-04-11 06:13:42.344173 jaxrie-3/src/jaxrie/modules/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-3/src/jaxrie/nets/__init__.py
+-rw-r--r--   0        0        0     2342 2023-04-11 06:23:40.424342 jaxrie-3/src/jaxrie/nets/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-3/src/jaxrie/py.typed
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-3/PKG-INFO
```

### Comparing `jaxrie-2/pyproject.toml` & `jaxrie-3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     "jaxlib>=0.4.6",
     "dm-haiku>=0.0.9",
     "optax>=0.1.4",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 dynamic = []
-version = "2"
+version = "3"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `jaxrie-2/src/jaxrie/manifold/base.py` & `jaxrie-3/src/jaxrie/manifold/base.py`

 * *Files identical despite different names*

### Comparing `jaxrie-2/src/jaxrie/manifold/lorentz.py` & `jaxrie-3/src/jaxrie/manifold/lorentz.py`

 * *Files identical despite different names*

### Comparing `jaxrie-2/src/jaxrie/manifold/math.py` & `jaxrie-3/src/jaxrie/manifold/math.py`

 * *Files identical despite different names*

### Comparing `jaxrie-2/src/jaxrie/manifold/stereographic.py` & `jaxrie-3/src/jaxrie/manifold/stereographic.py`

 * *Files identical despite different names*

### Comparing `jaxrie-2/src/jaxrie/modules/basic.py` & `jaxrie-3/src/jaxrie/modules/basic.py`

 * *Files identical despite different names*

### Comparing `jaxrie-2/src/jaxrie/nets/basic.py` & `jaxrie-3/src/jaxrie/nets/basic.py`

 * *Files identical despite different names*

