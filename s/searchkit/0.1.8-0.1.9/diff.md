# Comparing `tmp/searchkit-0.1.8.tar.gz` & `tmp/searchkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.1.8.tar", last modified: Fri Jan 27 17:08:55 2023, max compression
+gzip compressed data, was "searchkit-0.1.9.tar", last modified: Fri Jan 27 18:58:57 2023, max compression
```

## Comparing `searchkit-0.1.8.tar` & `searchkit-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 17:08:55.131436 searchkit-0.1.8/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.1.8/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)      142 2023-01-27 17:08:55.131436 searchkit-0.1.8/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      276 2023-01-27 17:08:41.000000 searchkit-0.1.8/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 17:08:55.131436 searchkit-0.1.8/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      100 2023-01-27 10:33:34.000000 searchkit-0.1.8/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    22684 2023-01-27 10:33:34.000000 searchkit-0.1.8/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-27 16:02:47.000000 searchkit-0.1.8/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    30753 2023-01-27 16:17:02.000000 searchkit-0.1.8/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2730 2023-01-24 13:08:12.000000 searchkit-0.1.8/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 17:08:55.131436 searchkit-0.1.8/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)      142 2023-01-27 17:08:55.000000 searchkit-0.1.8/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      298 2023-01-27 17:08:55.000000 searchkit-0.1.8/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-01-27 17:08:55.000000 searchkit-0.1.8/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       47 2023-01-27 17:08:55.000000 searchkit-0.1.8/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-01-27 17:08:55.000000 searchkit-0.1.8/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-01-27 17:08:55.131436 searchkit-0.1.8/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-24 13:08:12.000000 searchkit-0.1.8/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 18:58:57.090677 searchkit-0.1.9/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.1.9/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)      142 2023-01-27 18:58:57.090677 searchkit-0.1.9/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      276 2023-01-27 18:58:39.000000 searchkit-0.1.9/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 18:58:57.090677 searchkit-0.1.9/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      100 2023-01-27 10:33:34.000000 searchkit-0.1.9/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    22684 2023-01-27 10:33:34.000000 searchkit-0.1.9/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-27 16:02:47.000000 searchkit-0.1.9/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    30778 2023-01-27 18:57:39.000000 searchkit-0.1.9/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2730 2023-01-24 13:08:12.000000 searchkit-0.1.9/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 18:58:57.090677 searchkit-0.1.9/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      142 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      298 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       47 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-01-27 18:58:57.090677 searchkit-0.1.9/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-24 13:08:12.000000 searchkit-0.1.9/setup.py
```

### Comparing `searchkit-0.1.8/LICENSE` & `searchkit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.1.8/searchkit/constraints.py` & `searchkit-0.1.9/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.1.8/searchkit/search.py` & `searchkit-0.1.9/searchkit/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,15 +733,16 @@
         # if not os.path.isdir(os.path.join(HotSOSConfig.data_root,
         #                                   'sos_commands')):
         #     log.info("skipping global constraints since data_root is not a "
         #              "sosreport therefore files may be changing")
         #     return offset
 
         for c in self.global_constraints:
-            log.debug("applying task global constraint %s to %s", c, fd.name)
+            log.debug("applying task global constraint %s to %s", c.id,
+                      fd.name)
             _offset = c.apply_to_file(fd)
             if _offset is not None:
                 return _offset
 
         return offset
 
     def apply_single(self, searchdef, line):
```

### Comparing `searchkit-0.1.8/searchkit/utils.py` & `searchkit-0.1.9/searchkit/utils.py`

 * *Files identical despite different names*

