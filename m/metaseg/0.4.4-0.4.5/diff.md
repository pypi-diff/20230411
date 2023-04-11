# Comparing `tmp/metaseg-0.4.4.tar.gz` & `tmp/metaseg-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.4.4.tar", last modified: Mon Apr 10 19:54:43 2023, max compression
+gzip compressed data, was "metaseg-0.4.5.tar", last modified: Tue Apr 11 18:48:31 2023, max compression
```

## Comparing `metaseg-0.4.4.tar` & `metaseg-0.4.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.552033 metaseg-0.4.4/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.4/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.4/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2557 2023-04-10 19:54:43.552033 metaseg-0.4.4/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2283 2023-04-10 19:41:32.000000 metaseg-0.4.4/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.542033 metaseg-0.4.4/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-10 19:54:13.000000 metaseg-0.4.4/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.548700 metaseg-0.4.4/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7009 2023-04-10 19:54:00.000000 metaseg-0.4.4/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.548700 metaseg-0.4.4/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.4/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.4/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.4/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.4/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.4/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.4/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.4/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1205 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.552033 metaseg-0.4.4/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.4/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.4/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.4/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.552033 metaseg-0.4.4/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.4.4/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-10 19:54:43.545367 metaseg-0.4.4/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2557 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-10 19:54:43.000000 metaseg-0.4.4/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.4/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.4.4/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-10 19:54:43.555367 metaseg-0.4.4/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.4/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.527831 metaseg-0.4.5/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.5/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.5/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2569 2023-04-11 18:48:31.527831 metaseg-0.4.5/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2295 2023-04-11 18:48:27.000000 metaseg-0.4.5/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.521165 metaseg-0.4.5/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.521165 metaseg-0.4.5/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6142 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.524498 metaseg-0.4.5/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.5/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.5/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.5/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.5/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.5/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.5/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.5/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3107 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.527831 metaseg-0.4.5/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.5/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2089 2023-04-11 18:48:27.000000 metaseg-0.4.5/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.5/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.5/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.527831 metaseg-0.4.5/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.4.5/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 18:48:31.521165 metaseg-0.4.5/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2569 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-11 18:48:31.000000 metaseg-0.4.5/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.5/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.4.5/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-11 18:48:31.531165 metaseg-0.4.5/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.5/setup.py
```

### Comparing `metaseg-0.4.4/LICENSE` & `metaseg-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/PKG-INFO` & `metaseg-0.4.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: metaseg
-Version: 0.4.4
-Home-page: https://github.com/kadirnar/segment-anything-pip
-Author: kadirnar
-License: Apache-2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
@@ -34,47 +22,47 @@
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskPredictor().save_image(
+autoseg_image = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskPredictor().save_video(
+autoseg_video = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
 # For manuel box and point selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # x,y,w,h
     multimask_output=False,
 
 )
 
 # For multi box selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
     source="data/brain.png",
     model_type="vit_l",
     input_point=None,
     input_label=None,
     input_box= [[100, 100, 400, 400]],
     multimask_output=False,
```

#### html2text {}

```diff
@@ -1,28 +1,24 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.4 Home-page: https://
-github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image autoseg_image =
-SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
+SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
-For video autoseg_video = SegAutoMaskPredictor().save_video
+For video autoseg_video = SegAutoMaskPredictor().video_predict
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
 points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
-point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
-[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
-x,y,w,h multimask_output=False, ) # For multi box selection
-seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
-brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
-[[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
-Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x] Support
-for video and web application(Huggingface Spaces) - [x] Support for manual
-single multi box and point selection - [x] Support for pip installation - [x]
-Support for SAHI library
+point selection seg_manual_mask_generator = SegManualMaskPredictor
+().image_predict( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
+input_point=[[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100,
+200, 200], # x,y,w,h multimask_output=False, ) # For multi box selection
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict
+( source="data/brain.png", model_type="vit_l", input_point=None,
+input_label=None, input_box= [[100, 100, 400, 400]], multimask_output=False, )
+``` # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
+Torchvision models - [x] Support for video and web application(Huggingface
+Spaces) - [x] Support for manual single multi box and point selection - [x]
+Support for pip installation - [x] Support for SAHI library
```

### Comparing `metaseg-0.4.4/README.md` & `metaseg-0.4.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: metaseg
+Version: 0.4.5
+Home-page: https://github.com/kadirnar/segment-anything-pip
+Author: kadirnar
+License: Apache-2.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: dev
+License-File: LICENSE
+
 <div align="center">
 <h2>
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
@@ -22,47 +34,47 @@
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskPredictor().save_image(
+autoseg_image = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskPredictor().save_video(
+autoseg_video = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
 # For manuel box and point selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # x,y,w,h
     multimask_output=False,
 
 )
 
 # For multi box selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
     source="data/brain.png",
     model_type="vit_l",
     input_point=None,
     input_label=None,
     input_box= [[100, 100, 400, 400]],
     multimask_output=False,
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.5 Home-page: https://
+github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image autoseg_image =
-SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
+SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
-For video autoseg_video = SegAutoMaskPredictor().save_video
+For video autoseg_video = SegAutoMaskPredictor().video_predict
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
 points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
-point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
-[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
-x,y,w,h multimask_output=False, ) # For multi box selection
-seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
-brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
-[[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
-Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x] Support
-for video and web application(Huggingface Spaces) - [x] Support for manual
-single multi box and point selection - [x] Support for pip installation - [x]
-Support for SAHI library
+point selection seg_manual_mask_generator = SegManualMaskPredictor
+().image_predict( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
+input_point=[[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100,
+200, 200], # x,y,w,h multimask_output=False, ) # For multi box selection
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict
+( source="data/brain.png", model_type="vit_l", input_point=None,
+input_label=None, input_box= [[100, 100, 400, 400]], multimask_output=False, )
+``` # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
+Torchvision models - [x] Support for video and web application(Huggingface
+Spaces) - [x] Support for manual single multi box and point selection - [x]
+Support for pip installation - [x] Support for SAHI library
```

### Comparing `metaseg-0.4.4/metaseg/__init__.py` & `metaseg-0.4.5/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
```

### Comparing `metaseg-0.4.4/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.4.5/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/generator/build_sam.py` & `metaseg-0.4.5/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/generator/predictor.py` & `metaseg-0.4.5/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/mask_predictor.py` & `metaseg-0.4.5/metaseg/mask_predictor.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,88 +2,94 @@
 
 import cv2
 import numpy as np
 import torch
 from tqdm import tqdm
 
 from metaseg import SamAutomaticMaskGenerator, SamPredictor, sam_model_registry
-from metaseg.utils import download_model, load_image, load_video
+from metaseg.utils import download_model, load_box, load_image, load_mask, load_video, multi_boxes
 
 
 class SegAutoMaskPredictor:
     def __init__(self):
         self.model = None
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
+        self.save = False
+        self.show = False
 
     def load_model(self, model_type):
         if self.model is None:
             self.model_path = download_model(model_type)
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
         return self.model
 
-    def predict(self, frame, model_type, points_per_side, points_per_batch, min_area):
+    def image_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.png"):
+        read_image = load_image(source)
         model = self.load_model(model_type)
         mask_generator = SamAutomaticMaskGenerator(
             model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
         )
 
-        masks = mask_generator.generate(frame)
-
-        return frame, masks
-
-    def save_image(self, source, model_type, points_per_side, points_per_batch, min_area):
-        read_image = load_image(source)
-        image, anns = self.predict(read_image, model_type, points_per_side, points_per_batch, min_area)
-        if len(anns) == 0:
-            return
+        masks = mask_generator.generate(read_image)
 
-        sorted_anns = sorted(anns, key=(lambda x: x["area"]), reverse=True)
-        mask_image = np.zeros((anns[0]["segmentation"].shape[0], anns[0]["segmentation"].shape[1], 3), dtype=np.uint8)
+        sorted_anns = sorted(masks, key=(lambda x: x["area"]), reverse=True)
+        mask_image = np.zeros((masks[0]["segmentation"].shape[0], masks[0]["segmentation"].shape[1], 3), dtype=np.uint8)
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
         for i, ann in enumerate(sorted_anns):
             m = ann["segmentation"]
             img = np.ones((m.shape[0], m.shape[1], 3), dtype=np.uint8)
             color = colors[i % 256]
             for i in range(3):
                 img[:, :, 0] = color[0]
                 img[:, :, 1] = color[1]
                 img[:, :, 2] = color[2]
             img = cv2.bitwise_and(img, img, mask=m.astype(np.uint8))
             img = cv2.addWeighted(img, 0.35, np.zeros_like(img), 0.65, 0)
             mask_image = cv2.add(mask_image, img)
 
-        combined_mask = cv2.add(image, mask_image)
-        cv2.imwrite("output.jpg", combined_mask)
+        combined_mask = cv2.add(read_image, mask_image)
+        if self.save:
+            cv2.imwrite(output_path, combined_mask)
+
+        if self.show:
+            cv2.imshow("Output", combined_mask)
+            cv2.waitKey(0)
+            cv2.destroyAllWindows()
 
-        return "output.jpg"
+        return output_path
 
-    def save_video(self, source, model_type, points_per_side, points_per_batch, min_area):
-        cap, out = load_video(source)
+    def video_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.mp4"):
+        cap, out = load_video(source, output_path)
         length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
 
         for _ in tqdm(range(length)):
             ret, frame = cap.read()
             if not ret:
                 break
 
-            image, anns = self.predict(frame, model_type, points_per_side, points_per_batch, min_area)
-            if len(anns) == 0:
+            model = self.load_model(model_type)
+            mask_generator = SamAutomaticMaskGenerator(
+                model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
+            )
+            masks = mask_generator.generate(frame)
+
+            if len(masks) == 0:
                 continue
 
-            sorted_anns = sorted(anns, key=(lambda x: x["area"]), reverse=True)
+            sorted_anns = sorted(masks, key=(lambda x: x["area"]), reverse=True)
             mask_image = np.zeros(
-                (anns[0]["segmentation"].shape[0], anns[0]["segmentation"].shape[1], 3), dtype=np.uint8
+                (masks[0]["segmentation"].shape[0], masks[0]["segmentation"].shape[1], 3), dtype=np.uint8
             )
 
             for i, ann in enumerate(sorted_anns):
                 m = ann["segmentation"]
-                color = colors[i % 256]  # Her nesne için farklı bir renk kullan
+                color = colors[i % 256]
                 img = np.zeros((m.shape[0], m.shape[1], 3), dtype=np.uint8)
                 img[:, :, 0] = color[0]
                 img[:, :, 1] = color[1]
                 img[:, :, 2] = color[2]
                 img = cv2.bitwise_and(img, img, mask=m.astype(np.uint8))
                 img = cv2.addWeighted(img, 0.35, np.zeros_like(img), 0.65, 0)
                 mask_image = cv2.add(mask_image, img)
@@ -91,109 +97,77 @@
             combined_mask = cv2.add(frame, mask_image)
             out.write(combined_mask)
 
         out.release()
         cap.release()
         cv2.destroyAllWindows()
 
-        return "output.mp4"
+        return output_path
 
 
 class SegManualMaskPredictor:
     def __init__(self):
         self.model = None
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
+        self.save = False
+        self.show = False
 
     def load_model(self, model_type):
         if self.model is None:
             self.model_path = download_model(model_type)
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
         return self.model
 
-    def load_mask(self, mask, random_color):
-        if random_color:
-            color = np.random.rand(3) * 255
-        else:
-            color = np.array([100, 50, 0])
-
-        h, w = mask.shape[-2:]
-        mask_image = mask.reshape(h, w, 1) * color.reshape(1, 1, -1)
-        mask_image = mask_image.astype(np.uint8)
-        return mask_image
-
-    def load_box(self, box, image):
-        x, y, w, h = int(box[0]), int(box[1]), int(box[2]), int(box[3])
-        cv2.rectangle(image, (x, y), (w, h), (0, 255, 0), 2)
-        return image
-
-    def multi_boxes(self, boxes, predictor, image):
-        input_boxes = torch.tensor(boxes, device=predictor.device)
-        transformed_boxes = predictor.transform.apply_boxes_torch(input_boxes, image.shape[:2])
-        return input_boxes, transformed_boxes
-
-    def predict(
+    def image_predict(
         self,
-        frame,
+        source,
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
+        output_path="output.png",
     ):
+        image = load_image(source)
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
-        predictor.set_image(frame)
+        predictor.set_image(image)
 
         if type(input_box[0]) == list:
-            input_boxes, new_boxes = self.multi_boxes(input_box, predictor, frame)
+            input_boxes, new_boxes = multi_boxes(input_box, predictor, image)
 
             masks, _, _ = predictor.predict_torch(
                 point_coords=None,
                 point_labels=None,
                 boxes=new_boxes,
                 multimask_output=False,
             )
+            for mask in masks:
+                mask_image = load_mask(mask.cpu().numpy(), False)
+
+            for box in input_boxes:
+                image = load_box(box.cpu().numpy(), image)
 
         elif type(input_box[0]) == int:
             input_boxes = np.array(input_box)[None, :]
 
             masks, _, _ = predictor.predict(
                 point_coords=input_point,
                 point_labels=input_label,
                 box=input_boxes,
                 multimask_output=multimask_output,
             )
-
-        return frame, masks, input_boxes
-
-    def save_image(
-        self,
-        source,
-        model_type,
-        input_box=None,
-        input_point=None,
-        input_label=None,
-        multimask_output=False,
-        output_path="v0.jpg",
-    ):
-        read_image = load_image(source)
-        image, anns, boxes = self.predict(read_image, model_type, input_box, input_point, input_label, multimask_output)
-        if len(anns) == 0:
-            return
-
-        if type(input_box[0]) == list:
-            for mask in anns:
-                mask_image = self.load_mask(mask.cpu().numpy(), False)
-
-            for box in boxes:
-                image = self.load_box(box.cpu().numpy(), image)
-
-        elif type(input_box[0]) == int:
-            mask_image = self.load_mask(anns, True)
-            image = self.load_box(input_box, image)
+            mask_image = load_mask(masks, True)
+            image = load_box(input_box, image)
 
         combined_mask = cv2.add(image, mask_image)
-        cv2.imwrite(output_path, combined_mask)
+        if self.save:
+            cv2.imwrite(output_path, combined_mask)
+
+        if self.show:
+            cv2.imshow("Output", combined_mask)
+            cv2.waitKey(0)
+            cv2.destroyAllWindows()
 
         return output_path
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `metaseg-0.4.4/metaseg/modeling/common.py` & `metaseg-0.4.5/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/modeling/image_encoder.py` & `metaseg-0.4.5/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/modeling/mask_decoder.py` & `metaseg-0.4.5/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/modeling/prompt_encoder.py` & `metaseg-0.4.5/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/modeling/sam.py` & `metaseg-0.4.5/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/modeling/transformer.py` & `metaseg-0.4.5/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/utils/amg.py` & `metaseg-0.4.5/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/utils/file_utils.py` & `metaseg-0.4.5/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/utils/onnx.py` & `metaseg-0.4.5/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/utils/transforms.py` & `metaseg-0.4.5/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg/webapp/app.py` & `metaseg-0.4.5/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/metaseg.egg-info/PKG-INFO` & `metaseg-0.4.5/metaseg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.4
+Version: 0.4.5
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -34,47 +34,47 @@
 ```python
 from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskPredictor().save_image(
+autoseg_image = SegAutoMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskPredictor().save_video(
+autoseg_video = SegAutoMaskPredictor().video_predict(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
 # For manuel box and point selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # x,y,w,h
     multimask_output=False,
 
 )
 
 # For multi box selection
 
-seg_manual_mask_generator = SegManualMaskPredictor().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict(
     source="data/brain.png",
     model_type="vit_l",
     input_point=None,
     input_label=None,
     input_box= [[100, 100, 400, 400]],
     multimask_output=False,
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.4 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.4.5 Home-page: https://
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
 points_per_side and points_per_batch. # For image autoseg_image =
-SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
+SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
-For video autoseg_video = SegAutoMaskPredictor().save_video
+For video autoseg_video = SegAutoMaskPredictor().video_predict
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
 points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box and
-point selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[
-[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], #
-x,y,w,h multimask_output=False, ) # For multi box selection
-seg_manual_mask_generator = SegManualMaskPredictor().save_image( source="data/
-brain.png", model_type="vit_l", input_point=None, input_label=None, input_box=
-[[100, 100, 400, 400]], multimask_output=False, ) ``` # Extra Features - [x]
-Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x] Support
-for video and web application(Huggingface Spaces) - [x] Support for manual
-single multi box and point selection - [x] Support for pip installation - [x]
-Support for SAHI library
+point selection seg_manual_mask_generator = SegManualMaskPredictor
+().image_predict( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
+input_point=[[100, 100], [200, 200]], input_label=[0, 1], input_box=[100, 100,
+200, 200], # x,y,w,h multimask_output=False, ) # For multi box selection
+seg_manual_mask_generator = SegManualMaskPredictor().image_predict
+( source="data/brain.png", model_type="vit_l", input_point=None,
+input_label=None, input_box= [[100, 100, 400, 400]], multimask_output=False, )
+``` # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
+Torchvision models - [x] Support for video and web application(Huggingface
+Spaces) - [x] Support for manual single multi box and point selection - [x]
+Support for pip installation - [x] Support for SAHI library
```

### Comparing `metaseg-0.4.4/metaseg.egg-info/SOURCES.txt` & `metaseg-0.4.5/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.4/setup.py` & `metaseg-0.4.5/setup.py`

 * *Files identical despite different names*

