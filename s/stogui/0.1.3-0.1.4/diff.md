# Comparing `tmp/stogui-0.1.3.tar.gz` & `tmp/stogui-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stogui-0.1.3.tar", last modified: Fri Mar 31 20:57:02 2023, max compression
+gzip compressed data, was "stogui-0.1.4.tar", last modified: Mon Apr 10 22:29:37 2023, max compression
```

## Comparing `stogui-0.1.3.tar` & `stogui-0.1.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.667674 stogui-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-31 20:56:18.000000 stogui-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-31 20:56:18.000000 stogui-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-31 20:57:02.667674 stogui-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 20:56:18.000000 stogui-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-31 20:57:02.667674 stogui-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 20:56:18.000000 stogui-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.643674 stogui-0.1.3/stogui/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.643674 stogui-0.1.3/stogui/pipeline_maker/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.643674 stogui-0.1.3/stogui/pipeline_maker/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.647674 stogui-0.1.3/stogui/pipeline_maker/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.643674 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.655674 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1718475 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  6244744 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    19537 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.655674 stogui-0.1.3/stogui/session_table/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-31 20:57:00.000000 stogui-0.1.3/stogui/session_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.643674 stogui-0.1.3/stogui/session_table/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.655674 stogui-0.1.3/stogui/session_table/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)   197413 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/precache-manifest.7c54318c7bd5436365464b7da16bc9e3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.643674 stogui-0.1.3/stogui/session_table/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.667674 stogui-0.1.3/stogui/session_table/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)  2078175 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  7687550 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    33608 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    85887 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-03-31 20:56:18.000000 stogui-0.1.3/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:57:02.643674 stogui-0.1.3/stogui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-31 20:57:02.000000 stogui-0.1.3/stogui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-31 20:57:02.000000 stogui-0.1.3/stogui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:57:02.000000 stogui-0.1.3/stogui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:57:02.000000 stogui-0.1.3/stogui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 20:57:02.000000 stogui-0.1.3/stogui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 20:57:02.000000 stogui-0.1.3/stogui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.181762 stogui-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 22:28:44.000000 stogui-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 22:28:44.000000 stogui-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 22:29:37.181762 stogui-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 22:28:44.000000 stogui-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 22:29:37.181762 stogui-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 22:28:44.000000 stogui-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.149762 stogui-0.1.4/stogui/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.153762 stogui-0.1.4/stogui/pipeline_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-10 22:29:34.000000 stogui-0.1.4/stogui/pipeline_maker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.149762 stogui-0.1.4/stogui/pipeline_maker/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.153762 stogui-0.1.4/stogui/pipeline_maker/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.149762 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.165762 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1718475 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  6244744 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19537 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.165762 stogui-0.1.4/stogui/session_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.149762 stogui-0.1.4/stogui/session_table/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.165762 stogui-0.1.4/stogui/session_table/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197413 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/precache-manifest.7c54318c7bd5436365464b7da16bc9e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.149762 stogui-0.1.4/stogui/session_table/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.181762 stogui-0.1.4/stogui/session_table/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  2078175 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  7687550 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    33608 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85887 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-10 22:28:44.000000 stogui-0.1.4/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:29:37.153762 stogui-0.1.4/stogui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 22:29:37.000000 stogui-0.1.4/stogui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-10 22:29:37.000000 stogui-0.1.4/stogui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:29:37.000000 stogui-0.1.4/stogui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:29:37.000000 stogui-0.1.4/stogui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 22:29:37.000000 stogui-0.1.4/stogui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 22:29:37.000000 stogui-0.1.4/stogui.egg-info/top_level.txt
```

### Comparing `stogui-0.1.3/LICENSE` & `stogui-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/__init__.py` & `stogui-0.1.4/stogui/pipeline_maker/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,26 +23,26 @@
     def identity(x):
         return x
 
     items = items or []
     steps = steps or []
     serializer = serializer or identity
 
-    serializable_map = {i: serializer(i) for i in items}
+    serialized_items = [serializer(i) for i in items]
+    serialized_steps = [serializer(s) for s in steps]
 
-    _items = list(serializable_map.values())
-    _steps = [serializable_map[s] for s in steps]
-
-    serializable_pipeline = _component_func(items=_items, steps=_steps)
+    serialized_pipeline = _component_func(
+        items=serialized_items, steps=serialized_steps
+    )
     pipeline = (
         [
-            [k for k, v in serializable_map.items() if v == sp][0]
-            for sp in serializable_pipeline
+            next(iter(i for i in items if serializer(i) == s))
+            for s in serialized_pipeline
         ]
-        if serializable_pipeline
+        if serialized_pipeline
         else []
     )
     return pipeline
 
 
 if __name__ == '__main__':
```

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/asset-manifest.json` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/bootstrap.min.css` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/index.html` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/precache-manifest.0a876a512cd852ca08256154cd9ec9e5.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/service-worker.js` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/2.395bb2b5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/main.8b135fc4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map` & `stogui-0.1.4/stogui/pipeline_maker/frontend/build/static/js/runtime-main.44d30fc2.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/__init__.py` & `stogui-0.1.4/stogui/session_table/__init__.py`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/asset-manifest.json` & `stogui-0.1.4/stogui/session_table/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/bootstrap.min.css` & `stogui-0.1.4/stogui/session_table/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/index.html` & `stogui-0.1.4/stogui/session_table/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/precache-manifest.7c54318c7bd5436365464b7da16bc9e3.js` & `stogui-0.1.4/stogui/session_table/frontend/build/precache-manifest.7c54318c7bd5436365464b7da16bc9e3.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/service-worker.js` & `stogui-0.1.4/stogui/session_table/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js` & `stogui-0.1.4/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.LICENSE.txt` & `stogui-0.1.4/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.map` & `stogui-0.1.4/stogui/session_table/frontend/build/static/js/2.ecc75715.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js` & `stogui-0.1.4/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js.map` & `stogui-0.1.4/stogui/session_table/frontend/build/static/js/main.c461c62c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js` & `stogui-0.1.4/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map` & `stogui-0.1.4/stogui/session_table/frontend/build/static/js/runtime-main.44d30fc2.js.map`

 * *Files identical despite different names*

### Comparing `stogui-0.1.3/stogui.egg-info/SOURCES.txt` & `stogui-0.1.4/stogui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

