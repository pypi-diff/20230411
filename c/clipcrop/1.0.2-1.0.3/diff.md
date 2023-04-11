# Comparing `tmp/clipcrop-1.0.2.tar.gz` & `tmp/clipcrop-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-1.0.2.tar", last modified: Fri Feb  3 11:25:47 2023, max compression
+gzip compressed data, was "clipcrop-1.0.3.tar", last modified: Tue Apr 11 15:33:52 2023, max compression
```

## Comparing `clipcrop-1.0.2.tar` & `clipcrop-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:25:47.556046 clipcrop-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-03 11:25:35.000000 clipcrop-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-03 11:25:47.556046 clipcrop-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-02-03 11:25:35.000000 clipcrop-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:25:47.552046 clipcrop-1.0.2/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:25:35.000000 clipcrop-1.0.2/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-02-03 11:25:35.000000 clipcrop-1.0.2/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:25:47.556046 clipcrop-1.0.2/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-03 11:25:47.000000 clipcrop-1.0.2/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-03 11:25:47.000000 clipcrop-1.0.2/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:25:47.000000 clipcrop-1.0.2/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:25:47.000000 clipcrop-1.0.2/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-03 11:25:47.000000 clipcrop-1.0.2/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-03 11:25:47.000000 clipcrop-1.0.2/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 11:25:47.556046 clipcrop-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-02-03 11:25:35.000000 clipcrop-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:33:52.461389 clipcrop-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 15:33:43.000000 clipcrop-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 15:33:52.461389 clipcrop-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-11 15:33:43.000000 clipcrop-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:33:52.461389 clipcrop-1.0.3/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:33:43.000000 clipcrop-1.0.3/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-11 15:33:43.000000 clipcrop-1.0.3/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:33:52.461389 clipcrop-1.0.3/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 15:33:52.000000 clipcrop-1.0.3/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 15:33:52.461389 clipcrop-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-11 15:33:43.000000 clipcrop-1.0.3/setup.py
```

### Comparing `clipcrop-1.0.2/LICENSE` & `clipcrop-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-1.0.2/PKG-INFO` & `clipcrop-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
@@ -70,11 +70,11 @@
 
 ### Implementation
 
 ```python
 from clipcrop import clipcrop
 clipseg = clipcrop.ClipSeg("/content/input.png", "black colored car")
 segmentor, clipmodel, clipprocessor = clipseg.load_models()
-result = clips.segment_image(segmentor, clipmodel, clipprocessor)
+result = clipseg.segment_image(segmentor, clipmodel, clipprocessor)
 # gives a list of dicitonary of top images and its relative similarity score and you can override this by setting num = 5  to get top 5 etc
 ```
```

### Comparing `clipcrop-1.0.2/README.md` & `clipcrop-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,11 +50,11 @@
 
 ### Implementation
 
 ```python
 from clipcrop import clipcrop
 clipseg = clipcrop.ClipSeg("/content/input.png", "black colored car")
 segmentor, clipmodel, clipprocessor = clipseg.load_models()
-result = clips.segment_image(segmentor, clipmodel, clipprocessor)
+result = clipseg.segment_image(segmentor, clipmodel, clipprocessor)
 # gives a list of dicitonary of top images and its relative similarity score and you can override this by setting num = 5  to get top 5 etc
 ```
```

### Comparing `clipcrop-1.0.2/clipcrop/clipcrop.py` & `clipcrop-1.0.3/clipcrop/clipcrop.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,50 @@
     DFE = DetrFeatureExtractor.from_pretrained('facebook/detr-resnet-50')
     DM = DetrForObjectDetection.from_pretrained('facebook/detr-resnet-50')
     CLIPM = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
     CLIPP = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32")
 
     return DFE, DM, CLIPM, CLIPP
 
+  def captcha(self, DFE, DM, CLIPM, CLIPP, th=0.95):
+    
+    self.th = th
+    self.DFE = DFE
+    self.DM = DM
+    self.CLIPM = CLIPM
+    self.CLIPP = CLIPP
+
+    image = Image.open(self.image_path)
+    inputs = self.DFE(images=image, return_tensors="pt")
+    outputs = self.DM(**inputs)
+
+    # model predicts bounding boxes and corresponding COCO classes
+    logits = outputs.logits
+    bboxes = outputs.pred_boxes
+    probas = outputs.logits.softmax(-1)[0, :, :-1] #removing no class as detr maps 
+
+    keep = probas.max(-1).values > self.th
+    outs = self.DFE.post_process(outputs, torch.tensor(image.size[::-1]).unsqueeze(0))
+    bboxes_scaled = outs[0]['boxes'][keep].detach().numpy()
+    labels = outs[0]['labels'][keep].detach().numpy()
+    scores = outs[0]['scores'][keep].detach().numpy()
+
+    for i,j in enumerate(bboxes_scaled):
+      
+      xmin = int(j[0])
+      ymin = int(j[1])
+      xmax = int(j[2])
+      ymax = int(j[3])
+      
+      im_arr = np.array(image)
+      cv2.rectangle(im_arr, (xmin, ymin), (xmax, ymax), (255,0,0), 2)
+
+    return Image.fromarray(im_arr)
+
+
   def extract_image(self, DFE, DM, CLIPM, CLIPP):
 
     self.DFE = DFE
     self.DM = DM
     self.CLIPM = CLIPM
     self.CLIPP = CLIPP
```

### Comparing `clipcrop-1.0.2/clipcrop.egg-info/PKG-INFO` & `clipcrop-1.0.3/clipcrop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
@@ -70,11 +70,11 @@
 
 ### Implementation
 
 ```python
 from clipcrop import clipcrop
 clipseg = clipcrop.ClipSeg("/content/input.png", "black colored car")
 segmentor, clipmodel, clipprocessor = clipseg.load_models()
-result = clips.segment_image(segmentor, clipmodel, clipprocessor)
+result = clipseg.segment_image(segmentor, clipmodel, clipprocessor)
 # gives a list of dicitonary of top images and its relative similarity score and you can override this by setting num = 5  to get top 5 etc
 ```
```

### Comparing `clipcrop-1.0.2/setup.py` & `clipcrop-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   'numpy',
   'opencv-python'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="1.0.2",
+    version="1.0.3",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

