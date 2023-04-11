# Comparing `tmp/clipcrop-1.0.7.tar.gz` & `tmp/clipcrop-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-1.0.7.tar", last modified: Tue Apr 11 16:55:37 2023, max compression
+gzip compressed data, was "clipcrop-1.0.8.tar", last modified: Tue Apr 11 16:59:17 2023, max compression
```

## Comparing `clipcrop-1.0.7.tar` & `clipcrop-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:55:37.384626 clipcrop-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 16:55:26.000000 clipcrop-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:55:37.384626 clipcrop-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 16:55:26.000000 clipcrop-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:55:37.384626 clipcrop-1.0.7/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:55:26.000000 clipcrop-1.0.7/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-11 16:55:26.000000 clipcrop-1.0.7/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:55:37.384626 clipcrop-1.0.7/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 16:55:37.384626 clipcrop-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-11 16:55:26.000000 clipcrop-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:59:17.067071 clipcrop-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 16:59:07.000000 clipcrop-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:59:17.067071 clipcrop-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 16:59:07.000000 clipcrop-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:59:17.067071 clipcrop-1.0.8/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:59:07.000000 clipcrop-1.0.8/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-11 16:59:07.000000 clipcrop-1.0.8/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:59:17.067071 clipcrop-1.0.8/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:59:17.000000 clipcrop-1.0.8/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 16:59:17.000000 clipcrop-1.0.8/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:59:17.000000 clipcrop-1.0.8/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:59:17.000000 clipcrop-1.0.8/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 16:59:17.000000 clipcrop-1.0.8/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:59:17.000000 clipcrop-1.0.8/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 16:59:17.067071 clipcrop-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-11 16:59:07.000000 clipcrop-1.0.8/setup.py
```

### Comparing `clipcrop-1.0.7/LICENSE` & `clipcrop-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-1.0.7/PKG-INFO` & `clipcrop-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.7
+Version: 1.0.8
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-1.0.7/README.md` & `clipcrop-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `clipcrop-1.0.7/clipcrop/clipcrop.py` & `clipcrop-1.0.8/clipcrop/clipcrop.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     # model predicts bounding boxes and corresponding COCO classes
     logits = outputs.logits
     bboxes = outputs.pred_boxes
     probas = outputs.logits.softmax(-1)[0, :, :-1] #removing no class as detr maps 
 
     keep = probas.max(-1).values > 0.95
-    print(image.shape[:2])
+    print(image.shape)
     outs = self.DFE.post_process(outputs, torch.tensor(image.shape[:2]).unsqueeze(0))
     bboxes_scaled = outs[0]['boxes'][keep].detach().numpy()
     labels = outs[0]['labels'][keep].detach().numpy()
     scores = outs[0]['scores'][keep].detach().numpy()
 
     images_list = []
     for i,j in enumerate(bboxes_scaled):
```

### Comparing `clipcrop-1.0.7/clipcrop.egg-info/PKG-INFO` & `clipcrop-1.0.8/clipcrop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.7
+Version: 1.0.8
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-1.0.7/setup.py` & `clipcrop-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   'numpy',
   'opencv-python'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="1.0.7",
+    version="1.0.8",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

