# Comparing `tmp/meta-reid-3.3.18.tar.gz` & `tmp/meta-reid-3.4.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-reid-3.3.18.tar", last modified: Mon Mar 20 06:17:36 2023, max compression
+gzip compressed data, was "dist/meta-reid-3.4.10.tar", last modified: Tue Apr 11 04:03:19 2023, max compression
```

## Comparing `meta-reid-3.3.18.tar` & `meta-reid-3.4.10.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-20 06:17:36.000000 meta-reid-3.3.18/
--rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-03-20 06:17:36.000000 meta-reid-3.3.18/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-03-13 10:34:15.000000 meta-reid-3.3.18/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-20 06:17:36.000000 meta-reid-3.3.18/meta_reid.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-03-20 06:17:36.000000 meta-reid-3.3.18/meta_reid.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      499 2023-03-20 06:17:36.000000 meta-reid-3.3.18/meta_reid.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-03-20 06:17:36.000000 meta-reid-3.3.18/meta_reid.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       69 2023-03-20 06:17:36.000000 meta-reid-3.3.18/meta_reid.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-03-20 06:17:36.000000 meta-reid-3.3.18/meta_reid.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-03-20 06:17:36.000000 meta-reid-3.3.18/meta_reid.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-20 06:17:36.000000 meta-reid-3.3.18/metareid/
--rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-03-14 03:19:31.000000 meta-reid-3.3.18/metareid/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-20 06:17:36.000000 meta-reid-3.3.18/metareid/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)       83 2023-03-14 03:19:10.000000 meta-reid-3.3.18/metareid/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-03-20 06:12:28.000000 meta-reid-3.3.18/metareid/app/onnx_to_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4229 2023-03-20 02:56:59.000000 meta-reid-3.3.18/metareid/app/reid_inference_trt.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-20 06:17:36.000000 meta-reid-3.3.18/metareid/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)       60 2023-03-20 06:14:45.000000 meta-reid-3.3.18/metareid/model_zoo/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4758 2023-03-13 10:48:35.000000 meta-reid-3.3.18/metareid/model_zoo/trt_engine.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    12524 2023-03-20 06:16:43.000000 meta-reid-3.3.18/metareid/model_zoo/trt_export.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-20 06:17:36.000000 meta-reid-3.3.18/metareid/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       50 2023-03-20 06:14:05.000000 meta-reid-3.3.18/metareid/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      608 2023-03-20 01:47:13.000000 meta-reid-3.3.18/metareid/utils/general.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-reid-3.3.18/metareid/utils/image_batch.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-03-20 06:17:36.000000 meta-reid-3.3.18/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      712 2023-03-20 06:17:00.000000 meta-reid-3.3.18/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-04-11 04:03:19.000000 meta-reid-3.4.10/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-03-13 10:34:15.000000 meta-reid-3.4.10/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/meta_reid.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      499 2023-04-11 04:03:19.000000 meta-reid-3.4.10/meta_reid.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       69 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-11 04:03:18.000000 meta-reid-3.4.10/meta_reid.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-03-14 03:19:31.000000 meta-reid-3.4.10/metareid/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       83 2023-03-14 03:19:10.000000 meta-reid-3.4.10/metareid/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-03-20 06:12:28.000000 meta-reid-3.4.10/metareid/app/onnx_to_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4299 2023-04-10 13:20:47.000000 meta-reid-3.4.10/metareid/app/reid_inference_trt.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       60 2023-03-20 06:14:45.000000 meta-reid-3.4.10/metareid/model_zoo/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4789 2023-04-11 04:01:10.000000 meta-reid-3.4.10/metareid/model_zoo/trt_engine.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    12524 2023-03-20 06:16:43.000000 meta-reid-3.4.10/metareid/model_zoo/trt_export.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-11 04:03:19.000000 meta-reid-3.4.10/metareid/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       50 2023-03-20 06:14:05.000000 meta-reid-3.4.10/metareid/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      608 2023-03-20 01:47:13.000000 meta-reid-3.4.10/metareid/utils/general.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-reid-3.4.10/metareid/utils/image_batch.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-11 04:03:19.000000 meta-reid-3.4.10/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      712 2023-04-11 04:02:20.000000 meta-reid-3.4.10/setup.py
```

### Comparing `meta-reid-3.3.18/metareid/app/onnx_to_trt.py` & `meta-reid-3.4.10/metareid/app/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.3.18/metareid/app/reid_inference_trt.py` & `meta-reid-3.4.10/metareid/app/reid_inference_trt.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,17 @@
         dirs = list_dirs(root_dir)
         for d in dirs:
             self.save_folder(os.path.join(root_dir, d))
 
         self.save_features()
 
     def index(self, features, recall_num=1):
+        if self.query_features is None:
+            return [-1], [0]
+
         if self.use_gpu:
             D, I = self.invert_index.search(features, recall_num)
 
             return I[0].tolist(), D[0].tolist()
         else:
             index_cossim = fast_dot(features, self.query_features.T)
             max_idx = np.argmax(index_cossim, axis=1)
```

### Comparing `meta-reid-3.3.18/metareid/model_zoo/trt_engine.py` & `meta-reid-3.4.10/metareid/model_zoo/trt_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,8 +123,9 @@
         norm = np.linalg.norm(nparray, ord=order, axis=axis, keepdims=True)
         return nparray / (norm + np.finfo(np.float32).eps)
 
     def __del__(self):
         del self._input
         del self._output
         del self._stream
+        self._device_ctx.pop()
         self._device_ctx.detach()  # release device context
```

### Comparing `meta-reid-3.3.18/metareid/model_zoo/trt_export.py` & `meta-reid-3.4.10/metareid/model_zoo/trt_export.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.3.18/metareid/utils/general.py` & `meta-reid-3.4.10/metareid/utils/general.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.3.18/metareid/utils/image_batch.py` & `meta-reid-3.4.10/metareid/utils/image_batch.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.3.18/setup.py` & `meta-reid-3.4.10/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'pycuda',
     'numpy',
     'pillow',
     'tqdm',
     'faiss-gpu'
 ]
 
-__version__ = 'V3.03.18'
+__version__ = 'V3.04.10'
 
 setup(
     name='meta-reid',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvreid',
```

