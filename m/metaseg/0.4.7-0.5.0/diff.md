# Comparing `tmp/metaseg-0.4.7.tar.gz` & `tmp/metaseg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.4.7.tar", last modified: Tue Apr 11 22:04:56 2023, max compression
+gzip compressed data, was "metaseg-0.5.0.tar", last modified: Tue Apr 11 22:23:13 2023, max compression
```

## Comparing `metaseg-0.4.7.tar` & `metaseg-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.084052 metaseg-0.4.7/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.4.7/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.4.7/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3167 2023-04-11 22:04:56.084052 metaseg-0.4.7/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2893 2023-04-11 22:04:13.000000 metaseg-0.4.7/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.077385 metaseg-0.4.7/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-11 22:04:50.000000 metaseg-0.4.7/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.080719 metaseg-0.4.7/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6144 2023-04-11 22:01:41.000000 metaseg-0.4.7/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.080719 metaseg-0.4.7/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.4.7/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.4.7/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.4.7/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.4.7/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.4.7/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.4.7/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.4.7/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3305 2023-04-11 22:01:41.000000 metaseg-0.4.7/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.084052 metaseg-0.4.7/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-11 18:48:27.000000 metaseg-0.4.7/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.4.7/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2332 2023-04-11 22:01:41.000000 metaseg-0.4.7/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.4.7/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.4.7/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.084052 metaseg-0.4.7/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.4.7/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:04:56.077385 metaseg-0.4.7/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3167 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-11 22:04:56.000000 metaseg-0.4.7/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-11 22:04:55.000000 metaseg-0.4.7/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.4.7/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.4.7/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-11 22:04:56.084052 metaseg-0.4.7/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.4.7/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.637373 metaseg-0.5.0/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.5.0/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.5.0/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-11 22:23:13.637373 metaseg-0.5.0/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-11 22:22:18.000000 metaseg-0.5.0/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.630706 metaseg-0.5.0/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-11 22:22:31.000000 metaseg-0.5.0/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.634040 metaseg-0.5.0/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6236 2023-04-11 22:22:49.000000 metaseg-0.5.0/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.634040 metaseg-0.5.0/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.5.0/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.5.0/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.5.0/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.5.0/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.5.0/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.5.0/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.5.0/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3297 2023-04-11 22:22:49.000000 metaseg-0.5.0/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.637373 metaseg-0.5.0/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-11 18:48:27.000000 metaseg-0.5.0/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.5.0/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-11 22:22:49.000000 metaseg-0.5.0/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.5.0/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.5.0/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.637373 metaseg-0.5.0/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.630706 metaseg-0.5.0/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.5.0/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.5.0/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-11 22:23:13.637373 metaseg-0.5.0/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.5.0/setup.py
```

### Comparing `metaseg-0.4.7/LICENSE` & `metaseg-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/PKG-INFO` & `metaseg-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: metaseg
-Version: 0.4.7
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
@@ -74,28 +62,30 @@
     save=False,
 )
 ```
 
 ### SAHI + Segment Anything
 
 ```python
+from metaseg import sahi_sliced_predict, SahiAutoSegmentation
+
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
     detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
     image_size=1280,
     slice_height=256,
     slice_width=256,
     overlap_height_ratio=0.2,
     overlap_width_ratio=0.2,
 )
 
-SahiAutoSegmentation().save_image(
+SahiAutoSegmentation().predict(
     source=image_path,
     model_type="vit_b",
     input_box=boxes,
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.7 Home-page: https://
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
@@ -16,19 +12,19 @@
 SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
 output_path="output.mp4", ) # For manuel box and point selection results =
 SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
 # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
 input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
 200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
-### SAHI + Segment Anything ```python image_path = "test.jpg" boxes =
-sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
-#yolov8, detectron2, mmdetection, torchvision
-detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
-slice_height=256, slice_width=256, overlap_height_ratio=0.2,
-overlap_width_ratio=0.2, ) SahiAutoSegmentation().save_image
-( source=image_path, model_type="vit_b", input_box=boxes,
-multimask_output=False, random_color=False, show=True, save=False, ) ```
-[teaser] # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
-Torchvision models - [x] Support for video and web application(Huggingface
-Spaces) - [x] Support for manual single multi box and point selection - [x]
-Support for pip installation - [x] Support for SAHI library
+### SAHI + Segment Anything ```python from metaseg import sahi_sliced_predict,
+SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
+( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
+mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
+image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
+model_type="vit_b", input_box=boxes, multimask_output=False,
+random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
+[x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x]
+Support for video and web application(Huggingface Spaces) - [x] Support for
+manual single multi box and point selection - [x] Support for pip installation
+- [x] Support for SAHI library
```

### Comparing `metaseg-0.4.7/README.md` & `metaseg-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: metaseg
+Version: 0.5.0
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
@@ -62,28 +74,30 @@
     save=False,
 )
 ```
 
 ### SAHI + Segment Anything
 
 ```python
+from metaseg import sahi_sliced_predict, SahiAutoSegmentation
+
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
     detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
     image_size=1280,
     slice_height=256,
     slice_width=256,
     overlap_height_ratio=0.2,
     overlap_width_ratio=0.2,
 )
 
-SahiAutoSegmentation().save_image(
+SahiAutoSegmentation().predict(
     source=image_path,
     model_type="vit_b",
     input_box=boxes,
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.0 Home-page: https://
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
@@ -12,19 +16,19 @@
 SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
 output_path="output.mp4", ) # For manuel box and point selection results =
 SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
 # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
 input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
 200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
-### SAHI + Segment Anything ```python image_path = "test.jpg" boxes =
-sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
-#yolov8, detectron2, mmdetection, torchvision
-detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
-slice_height=256, slice_width=256, overlap_height_ratio=0.2,
-overlap_width_ratio=0.2, ) SahiAutoSegmentation().save_image
-( source=image_path, model_type="vit_b", input_box=boxes,
-multimask_output=False, random_color=False, show=True, save=False, ) ```
-[teaser] # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
-Torchvision models - [x] Support for video and web application(Huggingface
-Spaces) - [x] Support for manual single multi box and point selection - [x]
-Support for pip installation - [x] Support for SAHI library
+### SAHI + Segment Anything ```python from metaseg import sahi_sliced_predict,
+SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
+( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
+mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
+image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
+model_type="vit_b", input_box=boxes, multimask_output=False,
+random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
+[x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x]
+Support for video and web application(Huggingface Spaces) - [x] Support for
+manual single multi box and point selection - [x] Support for pip installation
+- [x] Support for SAHI library
```

### Comparing `metaseg-0.4.7/metaseg/__init__.py` & `metaseg-0.5.0/metaseg/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.4.7"
+__version__ = "0.5.0"
```

### Comparing `metaseg-0.4.7/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.5.0/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/generator/build_sam.py` & `metaseg-0.5.0/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/generator/predictor.py` & `metaseg-0.5.0/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/mask_predictor.py` & `metaseg-0.5.0/metaseg/mask_predictor.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 
 import cv2
 import numpy as np
 import torch
 from tqdm import tqdm
 
 from metaseg import SamAutomaticMaskGenerator, SamPredictor, sam_model_registry
-from metaseg.utils import download_model, load_box, load_image, load_mask, load_video, multi_boxes,show_image, save_image
+from metaseg.utils import (
+    download_model,
+    load_box,
+    load_image,
+    load_mask,
+    load_video,
+    multi_boxes,
+    save_image,
+    show_image,
+)
 
 
 class SegAutoMaskPredictor:
     def __init__(self):
         self.model = None
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
 
@@ -18,15 +27,25 @@
         if self.model is None:
             self.model_path = download_model(model_type)
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
         return self.model
 
-    def image_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.png", show=False, save=False):
+    def image_predict(
+        self,
+        source,
+        model_type,
+        points_per_side,
+        points_per_batch,
+        min_area,
+        output_path="output.png",
+        show=False,
+        save=False,
+    ):
         read_image = load_image(source)
         model = self.load_model(model_type)
         mask_generator = SamAutomaticMaskGenerator(
             model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
         )
 
         masks = mask_generator.generate(read_image)
@@ -46,20 +65,19 @@
             img = cv2.addWeighted(img, 0.35, np.zeros_like(img), 0.65, 0)
             mask_image = cv2.add(mask_image, img)
 
         combined_mask = cv2.add(read_image, mask_image)
         self.combined_mask = combined_mask
         if show:
             show_image(combined_mask)
-            
+
         if save:
             save_image(output_path=output_path, image=combined_mask)
-        
+
         return masks
-    
 
     def video_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.mp4"):
         cap, out = load_video(source, output_path)
         length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
 
         for _ in tqdm(range(length)):
```

### Comparing `metaseg-0.4.7/metaseg/modeling/common.py` & `metaseg-0.5.0/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/modeling/image_encoder.py` & `metaseg-0.5.0/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/modeling/mask_decoder.py` & `metaseg-0.5.0/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/modeling/prompt_encoder.py` & `metaseg-0.5.0/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/modeling/sam.py` & `metaseg-0.5.0/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/modeling/transformer.py` & `metaseg-0.5.0/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/sahi_predict.py` & `metaseg-0.5.0/metaseg/sahi_predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         input_point=None,
         input_label=None,
         multimask_output=False,
         random_color=False,
         save=False,
         show=True,
     ):
-        
+
         read_image = load_image(source)
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
         predictor.set_image(read_image)
 
         if type(input_box[0]) == list:
             input_boxes, new_boxes = multi_boxes(input_box, predictor, read_image)
```

### Comparing `metaseg-0.4.7/metaseg/utils/amg.py` & `metaseg-0.5.0/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/utils/data_utils.py` & `metaseg-0.5.0/metaseg/utils/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,20 @@
 def multi_boxes(boxes, predictor, image):
     import torch
 
     input_boxes = torch.tensor(boxes, device=predictor.device)
     transformed_boxes = predictor.transform.apply_boxes_torch(input_boxes, image.shape[:2])
     return input_boxes, transformed_boxes
 
+
 def show_image(output_image):
     import cv2
-    
+
     cv2.imshow("output", output_image)
     cv2.waitKey(0)
     cv2.destroyAllWindows()
-    
+
+
 def save_image(output_image, output_path):
     import cv2
+
     cv2.imwrite(output_path, output_image)
```

### Comparing `metaseg-0.4.7/metaseg/utils/file_utils.py` & `metaseg-0.5.0/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/utils/onnx.py` & `metaseg-0.5.0/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/utils/transforms.py` & `metaseg-0.5.0/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg/webapp/app.py` & `metaseg-0.5.0/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/metaseg.egg-info/PKG-INFO` & `metaseg-0.5.0/metaseg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.4.7
+Version: 0.5.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -74,28 +74,30 @@
     save=False,
 )
 ```
 
 ### SAHI + Segment Anything
 
 ```python
+from metaseg import sahi_sliced_predict, SahiAutoSegmentation
+
 image_path = "test.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
     detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
     image_size=1280,
     slice_height=256,
     slice_width=256,
     overlap_height_ratio=0.2,
     overlap_width_ratio=0.2,
 )
 
-SahiAutoSegmentation().save_image(
+SahiAutoSegmentation().predict(
     source=image_path,
     model_type="vit_b",
     input_box=boxes,
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.4.7 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -16,19 +16,19 @@
 SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
 output_path="output.mp4", ) # For manuel box and point selection results =
 SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
 # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
 input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
 200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
-### SAHI + Segment Anything ```python image_path = "test.jpg" boxes =
-sahi_sliced_predict( image_path=image_path, detection_model_type="yolov5",
-#yolov8, detectron2, mmdetection, torchvision
-detection_model_path="yolov5l6.pt", conf_th=0.25, image_size=1280,
-slice_height=256, slice_width=256, overlap_height_ratio=0.2,
-overlap_width_ratio=0.2, ) SahiAutoSegmentation().save_image
-( source=image_path, model_type="vit_b", input_box=boxes,
-multimask_output=False, random_color=False, show=True, save=False, ) ```
-[teaser] # Extra Features - [x] Support for Yolov5/8, Detectron2, Mmdetection,
-Torchvision models - [x] Support for video and web application(Huggingface
-Spaces) - [x] Support for manual single multi box and point selection - [x]
-Support for pip installation - [x] Support for SAHI library
+### SAHI + Segment Anything ```python from metaseg import sahi_sliced_predict,
+SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
+( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
+mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
+image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
+model_type="vit_b", input_box=boxes, multimask_output=False,
+random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
+[x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision models - [x]
+Support for video and web application(Huggingface Spaces) - [x] Support for
+manual single multi box and point selection - [x] Support for pip installation
+- [x] Support for SAHI library
```

### Comparing `metaseg-0.4.7/metaseg.egg-info/SOURCES.txt` & `metaseg-0.5.0/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.4.7/setup.py` & `metaseg-0.5.0/setup.py`

 * *Files identical despite different names*

