# Comparing `tmp/clipcrop-1.0.6.tar.gz` & `tmp/clipcrop-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-1.0.6.tar", last modified: Tue Apr 11 16:50:31 2023, max compression
+gzip compressed data, was "clipcrop-1.0.7.tar", last modified: Tue Apr 11 16:55:37 2023, max compression
```

## Comparing `clipcrop-1.0.6.tar` & `clipcrop-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:50:31.861971 clipcrop-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 16:50:21.000000 clipcrop-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:50:31.861971 clipcrop-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 16:50:21.000000 clipcrop-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:50:31.861971 clipcrop-1.0.6/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:50:21.000000 clipcrop-1.0.6/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-11 16:50:21.000000 clipcrop-1.0.6/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:50:31.861971 clipcrop-1.0.6/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:50:31.000000 clipcrop-1.0.6/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 16:50:31.000000 clipcrop-1.0.6/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:50:31.000000 clipcrop-1.0.6/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:50:31.000000 clipcrop-1.0.6/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 16:50:31.000000 clipcrop-1.0.6/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:50:31.000000 clipcrop-1.0.6/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 16:50:31.861971 clipcrop-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-11 16:50:21.000000 clipcrop-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:55:37.384626 clipcrop-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 16:55:26.000000 clipcrop-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:55:37.384626 clipcrop-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 16:55:26.000000 clipcrop-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:55:37.384626 clipcrop-1.0.7/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:55:26.000000 clipcrop-1.0.7/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-11 16:55:26.000000 clipcrop-1.0.7/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:55:37.384626 clipcrop-1.0.7/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:55:37.000000 clipcrop-1.0.7/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 16:55:37.384626 clipcrop-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-11 16:55:26.000000 clipcrop-1.0.7/setup.py
```

### Comparing `clipcrop-1.0.6/LICENSE` & `clipcrop-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-1.0.6/PKG-INFO` & `clipcrop-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-1.0.6/README.md` & `clipcrop-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `clipcrop-1.0.6/clipcrop/clipcrop.py` & `clipcrop-1.0.7/clipcrop/clipcrop.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
     # model predicts bounding boxes and corresponding COCO classes
     logits = outputs.logits
     bboxes = outputs.pred_boxes
     probas = outputs.logits.softmax(-1)[0, :, :-1] #removing no class as detr maps 
 
     keep = probas.max(-1).values > 0.95
+    print(image.shape[:2])
     outs = self.DFE.post_process(outputs, torch.tensor(image.shape[:2]).unsqueeze(0))
     bboxes_scaled = outs[0]['boxes'][keep].detach().numpy()
     labels = outs[0]['labels'][keep].detach().numpy()
     scores = outs[0]['scores'][keep].detach().numpy()
 
     images_list = []
     for i,j in enumerate(bboxes_scaled):
```

### Comparing `clipcrop-1.0.6/clipcrop.egg-info/PKG-INFO` & `clipcrop-1.0.7/clipcrop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-1.0.6/setup.py` & `clipcrop-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   'numpy',
   'opencv-python'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="1.0.6",
+    version="1.0.7",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

