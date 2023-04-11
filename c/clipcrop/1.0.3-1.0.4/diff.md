# Comparing `tmp/clipcrop-1.0.3.tar.gz` & `tmp/clipcrop-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-1.0.3.tar", last modified: Tue Apr 11 15:33:52 2023, max compression
+gzip compressed data, was "clipcrop-1.0.4.tar", last modified: Tue Apr 11 16:42:18 2023, max compression
```

## Comparing `clipcrop-1.0.3.tar` & `clipcrop-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:33:52.461389 clipcrop-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 15:33:43.000000 clipcrop-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 15:33:52.461389 clipcrop-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 15:33:43.000000 clipcrop-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:33:52.461389 clipcrop-1.0.3/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:33:43.000000 clipcrop-1.0.3/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-11 15:33:43.000000 clipcrop-1.0.3/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:33:52.461389 clipcrop-1.0.3/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 15:33:52.461389 clipcrop-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-11 15:33:43.000000 clipcrop-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:42:18.700143 clipcrop-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 16:42:08.000000 clipcrop-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:42:18.700143 clipcrop-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 16:42:08.000000 clipcrop-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:42:18.700143 clipcrop-1.0.4/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:42:08.000000 clipcrop-1.0.4/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-11 16:42:08.000000 clipcrop-1.0.4/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:42:18.700143 clipcrop-1.0.4/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 16:42:18.000000 clipcrop-1.0.4/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 16:42:18.000000 clipcrop-1.0.4/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:42:18.000000 clipcrop-1.0.4/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:42:18.000000 clipcrop-1.0.4/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 16:42:18.000000 clipcrop-1.0.4/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:42:18.000000 clipcrop-1.0.4/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 16:42:18.700143 clipcrop-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-11 16:42:08.000000 clipcrop-1.0.4/setup.py
```

### Comparing `clipcrop-1.0.3/LICENSE` & `clipcrop-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-1.0.3/PKG-INFO` & `clipcrop-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.3
+Version: 1.0.4
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-1.0.3/README.md` & `clipcrop-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `clipcrop-1.0.3/clipcrop/clipcrop.py` & `clipcrop-1.0.4/clipcrop/clipcrop.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     
     self.th = th
     self.DFE = DFE
     self.DM = DM
     self.CLIPM = CLIPM
     self.CLIPP = CLIPP
 
-    image = Image.open(self.image_path)
+    image = cv2.imread(self.image_path)
     inputs = self.DFE(images=image, return_tensors="pt")
     outputs = self.DM(**inputs)
 
     # model predicts bounding boxes and corresponding COCO classes
     logits = outputs.logits
     bboxes = outputs.pred_boxes
     probas = outputs.logits.softmax(-1)[0, :, :-1] #removing no class as detr maps 
@@ -47,29 +47,27 @@
     for i,j in enumerate(bboxes_scaled):
       
       xmin = int(j[0])
       ymin = int(j[1])
       xmax = int(j[2])
       ymax = int(j[3])
       
-      im_arr = np.array(image)
-      cv2.rectangle(im_arr, (xmin, ymin), (xmax, ymax), (255,0,0), 2)
+      cv2.rectangle(image, (xmin, ymin), (xmax, ymax), (255,0,0), 2)
 
     return Image.fromarray(im_arr)
 
 
   def extract_image(self, DFE, DM, CLIPM, CLIPP):
 
     self.DFE = DFE
     self.DM = DM
     self.CLIPM = CLIPM
     self.CLIPP = CLIPP
 
-    image = Image.open(self.image_path)
-
+    image = cv2.imread(self.image_path)
     inputs = self.DFE(images=image, return_tensors="pt")
     outputs = self.DM(**inputs)
 
     # model predicts bounding boxes and corresponding COCO classes
     logits = outputs.logits
     bboxes = outputs.pred_boxes
     probas = outputs.logits.softmax(-1)[0, :, :-1] #removing no class as detr maps 
@@ -84,18 +82,16 @@
     for i,j in enumerate(bboxes_scaled):
       
       xmin = int(j[0])
       ymin = int(j[1])
       xmax = int(j[2])
       ymax = int(j[3])
 
-      im_arr = np.array(image)
-      roi = im_arr[ymin:ymax, xmin:xmax]
+      roi = image[ymin:ymax, xmin:xmax]
       roi_im = Image.fromarray(roi)
-
       images_list.append(roi_im)
 
     inputs = self.CLIPP(text = [self.text], images=images_list , return_tensors="pt", padding=True)
     outputs = self.CLIPM(**inputs)
     logits_per_image = outputs.logits_per_text
     probs = logits_per_image.softmax(-1)
     l_idx = np.argsort(probs[-1].detach().numpy())[::-1][0:self.num]
```

### Comparing `clipcrop-1.0.3/clipcrop.egg-info/PKG-INFO` & `clipcrop-1.0.4/clipcrop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.3
+Version: 1.0.4
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-1.0.3/setup.py` & `clipcrop-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   'numpy',
   'opencv-python'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="1.0.3",
+    version="1.0.4",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

