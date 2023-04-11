# Comparing `tmp/metaseg-0.4.5.tar.gz` & `tmp/metaseg-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.4.5.tar", last modified: Tue Apr 11 18:48:31 2023, max compression
+gzip compressed data, was "metaseg-0.4.7.tar", last modified: Tue Apr 11 22:04:56 2023, max compression
```

## Comparing `metaseg-0.4.5.tar` & `metaseg-0.4.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.527831 metaseg-0.4.5/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.5/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.5/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2569 2023-04-11 18:48:31.527831 metaseg-0.4.5/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2295 2023-04-11 18:48:27.000000 metaseg-0.4.5/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.521165 metaseg-0.4.5/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.521165 metaseg-0.4.5/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6142 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.524498 metaseg-0.4.5/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.5/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.5/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.5/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.5/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.5/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.5/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.5/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3107 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.527831 metaseg-0.4.5/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.5/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2089 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.5/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.5/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.527831 metaseg-0.4.5/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.521165 metaseg-0.4.5/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2569 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.5/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.4.5/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-11 18:48:31.531165 metaseg-0.4.5/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.5/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.084052 metaseg-0.4.7/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.7/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.7/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3167 2023-04-11 22:04:56.084052 metaseg-0.4.7/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2893 2023-04-11 22:04:13.000000 metaseg-0.4.7/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.077385 metaseg-0.4.7/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-11 22:04:50.000000 metaseg-0.4.7/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.080719 metaseg-0.4.7/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6144 2023-04-11 22:01:41.000000 metaseg-0.4.7/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.080719 metaseg-0.4.7/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.7/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.7/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.7/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.7/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.7/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.7/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.7/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3305 2023-04-11 22:01:41.000000 metaseg-0.4.7/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.084052 metaseg-0.4.7/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-11 18:48:27.000000 metaseg-0.4.7/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.7/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2332 2023-04-11 22:01:41.000000 metaseg-0.4.7/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.7/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.7/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.084052 metaseg-0.4.7/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.077385 metaseg-0.4.7/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3167 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-11 22:04:56.000000 metaseg-0.4.7/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.7/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.4.7/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-11 22:04:56.084052 metaseg-0.4.7/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.7/setup.py
```

### Comparing `metaseg-0.4.5/LICENSE` & `metaseg-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/PKG-INFO` & `metaseg-0.4.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.5
+Version: 0.4.7
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -34,56 +34,79 @@
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskPredictor().image_predict(
+results = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
+    output_path="output.jpg",
+    show=True,
+    save=False,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskPredictor().video_predict(
+results = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
+    output_path="output.mp4",
 )
 
 # For manuel box and point selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
+results = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
-    input_box=[100, 100, 200, 200], # x,y,w,h
+    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
     multimask_output=False,
-
+    random_color=False,
+    show=True,
+    save=False,
 )
+```
 
-# For multi box selection
+### SAHI + Segment Anything
 
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
-    source="data/brain.png",
-    model_type="vit_l",
-    input_point=None,
-    input_label=None,
-    input_box= [[100, 100, 400, 400]],
-    multimask_output=False,
+```python
+image_path = "test.jpg"
+boxes = sahi_sliced_predict(
+    image_path=image_path,
+    detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
+    detection_model_path="yolov5l6.pt",
+    conf_th=0.25,
+    image_size=1280,
+    slice_height=256,
+    slice_width=256,
+    overlap_height_ratio=0.2,
+    overlap_width_ratio=0.2,
+)
 
+SahiAutoSegmentation().save_image(
+    source=image_path,
+    model_type="vit_b",
+    input_box=boxes,
+    multimask_output=False,
+    random_color=False,
+    show=True,
+    save=False,
 )
 ```
+<img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
+
 # Extra Features
 
 - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
 - [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
 - [x] Support for pip installation
 - [x] Support for SAHI library
```

#### html2text {}

```diff
@@ -1,28 +1,34 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.5 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.7 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
-points_per_side and points_per_batch. # For image autoseg_image =
+points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
-vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
-For video autoseg_video = SegAutoMaskPredictor().video_predict
-( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
-point selection seg_manual_mask_generator = SegManualMaskPredictor
-().image_predict( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
-input_point=[[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100,
-200, 200], # x,y,w,h multimask_output=False, ) # For multi box selection
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict
-( source="data/brain.png", model_type="vit_l", input_point=None,
-input_label=None, input_box= [[100, 100, 400, 400]], multimask_output=False, )
-``` # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
+output_path="output.jpg", show=True, save=False, ) # For video results =
+SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
+output_path="output.mp4", ) # For manuel box and point selection results =
+SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
+# vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
+input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
+200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
+### SAHI + Segment Anything ```python image_path = "test.jpg" boxes =
+sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+#yolov8, detectron2, mmdetection, torchvision
+detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
+slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().save_image
+( source=image_path, model_type="vit_b", input_box=boxes,
+multimask_output=False, random_color=False, show=True, save=False, ) ```
+[teaser] # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
 Torchvision models - [x] Support for video and web application(Huggingface
 Spaces) - [x] Support for manual single multi box and point selection - [x]
 Support for pip installation - [x] Support for SAHI library
```

### Comparing `metaseg-0.4.5/README.md` & `metaseg-0.4.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -22,56 +22,79 @@
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskPredictor().image_predict(
+results = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
+    output_path="output.jpg",
+    show=True,
+    save=False,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskPredictor().video_predict(
+results = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
+    output_path="output.mp4",
 )
 
 # For manuel box and point selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
+results = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
-    input_box=[100, 100, 200, 200], # x,y,w,h
+    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
     multimask_output=False,
-
+    random_color=False,
+    show=True,
+    save=False,
 )
+```
 
-# For multi box selection
+### SAHI + Segment Anything
 
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
-    source="data/brain.png",
-    model_type="vit_l",
-    input_point=None,
-    input_label=None,
-    input_box= [[100, 100, 400, 400]],
-    multimask_output=False,
+```python
+image_path = "test.jpg"
+boxes = sahi_sliced_predict(
+    image_path=image_path,
+    detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
+    detection_model_path="yolov5l6.pt",
+    conf_th=0.25,
+    image_size=1280,
+    slice_height=256,
+    slice_width=256,
+    overlap_height_ratio=0.2,
+    overlap_width_ratio=0.2,
+)
 
+SahiAutoSegmentation().save_image(
+    source=image_path,
+    model_type="vit_b",
+    input_box=boxes,
+    multimask_output=False,
+    random_color=False,
+    show=True,
+    save=False,
 )
 ```
+<img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
+
 # Extra Features
 
 - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
 - [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
 - [x] Support for pip installation
 - [x] Support for SAHI library
```

#### html2text {}

```diff
@@ -1,24 +1,30 @@
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
-points_per_side and points_per_batch. # For image autoseg_image =
+points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
-vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
-For video autoseg_video = SegAutoMaskPredictor().video_predict
-( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
-point selection seg_manual_mask_generator = SegManualMaskPredictor
-().image_predict( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
-input_point=[[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100,
-200, 200], # x,y,w,h multimask_output=False, ) # For multi box selection
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict
-( source="data/brain.png", model_type="vit_l", input_point=None,
-input_label=None, input_box= [[100, 100, 400, 400]], multimask_output=False, )
-``` # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
+output_path="output.jpg", show=True, save=False, ) # For video results =
+SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
+output_path="output.mp4", ) # For manuel box and point selection results =
+SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
+# vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
+input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
+200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
+### SAHI + Segment Anything ```python image_path = "test.jpg" boxes =
+sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+#yolov8, detectron2, mmdetection, torchvision
+detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
+slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().save_image
+( source=image_path, model_type="vit_b", input_box=boxes,
+multimask_output=False, random_color=False, show=True, save=False, ) ```
+[teaser] # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
 Torchvision models - [x] Support for video and web application(Huggingface
 Spaces) - [x] Support for manual single multi box and point selection - [x]
 Support for pip installation - [x] Support for SAHI library
```

### Comparing `metaseg-0.4.5/metaseg/__init__.py` & `metaseg-0.4.7/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.4.5"
+__version__ = "0.4.7"
```

### Comparing `metaseg-0.4.5/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.4.7/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/generator/build_sam.py` & `metaseg-0.4.7/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/generator/predictor.py` & `metaseg-0.4.7/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/mask_predictor.py` & `metaseg-0.4.7/metaseg/mask_predictor.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 
 import cv2
 import numpy as np
 import torch
 from tqdm import tqdm
 
 from metaseg import SamAutomaticMaskGenerator, SamPredictor, sam_model_registry
-from metaseg.utils import download_model, load_box, load_image, load_mask, load_video, multi_boxes
+from metaseg.utils import download_model, load_box, load_image, load_mask, load_video, multi_boxes,show_image, save_image
 
 
 class SegAutoMaskPredictor:
     def __init__(self):
         self.model = None
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
-        self.save = False
-        self.show = False
 
     def load_model(self, model_type):
         if self.model is None:
             self.model_path = download_model(model_type)
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
         return self.model
 
-    def image_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.png"):
+    def image_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.png", show=False, save=False):
         read_image = load_image(source)
         model = self.load_model(model_type)
         mask_generator = SamAutomaticMaskGenerator(
             model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
         )
 
         masks = mask_generator.generate(read_image)
@@ -45,23 +43,23 @@
                 img[:, :, 1] = color[1]
                 img[:, :, 2] = color[2]
             img = cv2.bitwise_and(img, img, mask=m.astype(np.uint8))
             img = cv2.addWeighted(img, 0.35, np.zeros_like(img), 0.65, 0)
             mask_image = cv2.add(mask_image, img)
 
         combined_mask = cv2.add(read_image, mask_image)
-        if self.save:
-            cv2.imwrite(output_path, combined_mask)
-
-        if self.show:
-            cv2.imshow("Output", combined_mask)
-            cv2.waitKey(0)
-            cv2.destroyAllWindows()
-
-        return output_path
+        self.combined_mask = combined_mask
+        if show:
+            show_image(combined_mask)
+            
+        if save:
+            save_image(output_path=output_path, image=combined_mask)
+        
+        return masks
+    
 
     def video_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.mp4"):
         cap, out = load_video(source, output_path)
         length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
 
         for _ in tqdm(range(length)):
@@ -124,14 +122,17 @@
         source,
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
         output_path="output.png",
+        random_color=False,
+        show=False,
+        save=False,
     ):
         image = load_image(source)
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
         predictor.set_image(image)
 
         if type(input_box[0]) == list:
@@ -140,34 +141,32 @@
             masks, _, _ = predictor.predict_torch(
                 point_coords=None,
                 point_labels=None,
                 boxes=new_boxes,
                 multimask_output=False,
             )
             for mask in masks:
-                mask_image = load_mask(mask.cpu().numpy(), False)
+                mask_image = load_mask(mask.cpu().numpy(), random_color)
 
             for box in input_boxes:
                 image = load_box(box.cpu().numpy(), image)
 
         elif type(input_box[0]) == int:
             input_boxes = np.array(input_box)[None, :]
 
             masks, _, _ = predictor.predict(
                 point_coords=input_point,
                 point_labels=input_label,
                 box=input_boxes,
                 multimask_output=multimask_output,
             )
-            mask_image = load_mask(masks, True)
+            mask_image = load_mask(masks, random_color)
             image = load_box(input_box, image)
 
         combined_mask = cv2.add(image, mask_image)
-        if self.save:
-            cv2.imwrite(output_path, combined_mask)
+        if save:
+            save_image(output_path=output_path, image=combined_mask)
 
-        if self.show:
-            cv2.imshow("Output", combined_mask)
-            cv2.waitKey(0)
-            cv2.destroyAllWindows()
+        if show:
+            show_image(combined_mask)
 
-        return output_path
+        return masks
```

### Comparing `metaseg-0.4.5/metaseg/modeling/common.py` & `metaseg-0.4.7/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/modeling/image_encoder.py` & `metaseg-0.4.7/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/modeling/mask_decoder.py` & `metaseg-0.4.7/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/modeling/prompt_encoder.py` & `metaseg-0.4.7/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/modeling/sam.py` & `metaseg-0.4.7/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/modeling/transformer.py` & `metaseg-0.4.7/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/sahi_predict.py` & `metaseg-0.4.7/metaseg/sahi_predict.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import torch
 
 from metaseg import SamPredictor, sam_model_registry
 from metaseg.utils import download_model, load_image, multi_boxes, plt_load_box, plt_load_mask
 
 
-def sahi_predict(
+def sahi_sliced_predict(
     image_path,
     detection_model_type,
     detection_model_path,
     conf_th,
     image_size,
     slice_height,
     slice_width,
@@ -47,34 +47,40 @@
     boxes = []
     for i in output:
         boxes.append(i.bbox.to_xyxy())
 
     return boxes
 
 
-class SahiPredictor:
+class SahiAutoSegmentation:
     def __init__(self):
         self.model = None
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
 
     def load_model(self, model_type):
         if self.model is None:
             self.model_path = download_model(model_type)
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
-    def save_image(
+        return self.model
+
+    def predict(
         self,
         source,
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
+        random_color=False,
+        save=False,
+        show=True,
     ):
+        
         read_image = load_image(source)
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
         predictor.set_image(read_image)
 
         if type(input_box[0]) == list:
             input_boxes, new_boxes = multi_boxes(input_box, predictor, read_image)
@@ -95,12 +101,15 @@
                 box=input_boxes,
                 multimask_output=multimask_output,
             )
 
         plt.figure(figsize=(10, 10))
         plt.imshow(read_image)
         for mask in masks:
-            plt_load_mask(mask.cpu().numpy(), plt.gca(), random_color=True)
+            plt_load_mask(mask.cpu().numpy(), plt.gca(), random_color=random_color)
         for box in input_boxes:
             plt_load_box(box.cpu().numpy(), plt.gca())
         plt.axis("off")
-        plt.show()
+        if save:
+            plt.savefig("output.png")
+        if show:
+            plt.show()
```

### Comparing `metaseg-0.4.5/metaseg/utils/amg.py` & `metaseg-0.4.7/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/utils/data_utils.py` & `metaseg-0.4.7/metaseg/utils/data_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,7 +71,18 @@
 
 def multi_boxes(boxes, predictor, image):
     import torch
 
     input_boxes = torch.tensor(boxes, device=predictor.device)
     transformed_boxes = predictor.transform.apply_boxes_torch(input_boxes, image.shape[:2])
     return input_boxes, transformed_boxes
+
+def show_image(output_image):
+    import cv2
+    
+    cv2.imshow("output", output_image)
+    cv2.waitKey(0)
+    cv2.destroyAllWindows()
+    
+def save_image(output_image, output_path):
+    import cv2
+    cv2.imwrite(output_path, output_image)
```

### Comparing `metaseg-0.4.5/metaseg/utils/file_utils.py` & `metaseg-0.4.7/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/utils/onnx.py` & `metaseg-0.4.7/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/utils/transforms.py` & `metaseg-0.4.7/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg/webapp/app.py` & `metaseg-0.4.7/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/metaseg.egg-info/PKG-INFO` & `metaseg-0.4.7/metaseg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.5
+Version: 0.4.7
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -34,56 +34,79 @@
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskPredictor().image_predict(
+results = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
+    output_path="output.jpg",
+    show=True,
+    save=False,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskPredictor().video_predict(
+results = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
+    output_path="output.mp4",
 )
 
 # For manuel box and point selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
+results = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
-    input_box=[100, 100, 200, 200], # x,y,w,h
+    input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
     multimask_output=False,
-
+    random_color=False,
+    show=True,
+    save=False,
 )
+```
 
-# For multi box selection
+### SAHI + Segment Anything
 
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
-    source="data/brain.png",
-    model_type="vit_l",
-    input_point=None,
-    input_label=None,
-    input_box= [[100, 100, 400, 400]],
-    multimask_output=False,
+```python
+image_path = "test.jpg"
+boxes = sahi_sliced_predict(
+    image_path=image_path,
+    detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
+    detection_model_path="yolov5l6.pt",
+    conf_th=0.25,
+    image_size=1280,
+    slice_height=256,
+    slice_width=256,
+    overlap_height_ratio=0.2,
+    overlap_width_ratio=0.2,
+)
 
+SahiAutoSegmentation().save_image(
+    source=image_path,
+    model_type="vit_b",
+    input_box=boxes,
+    multimask_output=False,
+    random_color=False,
+    show=True,
+    save=False,
 )
 ```
+<img width="700" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.5.0/sahi_autoseg.png">
+
 # Extra Features
 
 - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models
 - [x] Support for video and web application(Huggingface Spaces)
 - [x] Support for manual single multi box and point selection
 - [x] Support for pip installation
 - [x] Support for SAHI library
```

#### html2text {}

```diff
@@ -1,28 +1,34 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.5 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.7 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
-points_per_side and points_per_batch. # For image autoseg_image =
+points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
-vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
-For video autoseg_video = SegAutoMaskPredictor().video_predict
-( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
-point selection seg_manual_mask_generator = SegManualMaskPredictor
-().image_predict( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
-input_point=[[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100,
-200, 200], # x,y,w,h multimask_output=False, ) # For multi box selection
-seg_manual_mask_generator = SegManualMaskPredictor().image_predict
-( source="data/brain.png", model_type="vit_l", input_point=None,
-input_label=None, input_box= [[100, 100, 400, 400]], multimask_output=False, )
-``` # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
+output_path="output.jpg", show=True, save=False, ) # For video results =
+SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
+output_path="output.mp4", ) # For manuel box and point selection results =
+SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
+# vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
+input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
+200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
+### SAHI + Segment Anything ```python image_path = "test.jpg" boxes =
+sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
+#yolov8, detectron2, mmdetection, torchvision
+detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
+slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().save_image
+( source=image_path, model_type="vit_b", input_box=boxes,
+multimask_output=False, random_color=False, show=True, save=False, ) ```
+[teaser] # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
 Torchvision models - [x] Support for video and web application(Huggingface
 Spaces) - [x] Support for manual single multi box and point selection - [x]
 Support for pip installation - [x] Support for SAHI library
```

### Comparing `metaseg-0.4.5/metaseg.egg-info/SOURCES.txt` & `metaseg-0.4.7/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.5/setup.py` & `metaseg-0.4.7/setup.py`

 * *Files identical despite different names*

