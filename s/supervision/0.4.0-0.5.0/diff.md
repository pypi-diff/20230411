# Comparing `tmp/supervision-0.4.0.tar.gz` & `tmp/supervision-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervision-0.4.0.tar", last modified: Wed Apr  5 15:19:42 2023, max compression
+gzip compressed data, was "supervision-0.5.0.tar", last modified: Mon Apr 10 21:53:21 2023, max compression
```

## Comparing `supervision-0.4.0.tar` & `supervision-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.771005 supervision-0.4.0/
--rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.4.0/LICENSE.md
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-05 15:19:42.770863 supervision-0.4.0/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.4.0/README.md
--rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-04-05 15:19:42.771060 supervision-0.4.0/setup.cfg
--rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.4.0/setup.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.765146 supervision-0.4.0/supervision/
--rw-r--r--   0 skalskip   (501) staff       (20)      841 2023-04-05 15:18:58.000000 supervision-0.4.0/supervision/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.766213 supervision-0.4.0/supervision/annotation/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-05 15:18:58.000000 supervision-0.4.0/supervision/annotation/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3279 2023-04-05 15:18:58.000000 supervision-0.4.0/supervision/annotation/voc.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.767392 supervision-0.4.0/supervision/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.4.0/supervision/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     4252 2023-03-29 12:10:01.000000 supervision-0.4.0/supervision/detection/annotate.py
--rw-r--r--   0 skalskip   (501) staff       (20)    11678 2023-04-05 15:18:58.000000 supervision-0.4.0/supervision/detection/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     7159 2023-03-23 11:05:51.000000 supervision-0.4.0/supervision/detection/line_counter.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2891 2023-03-14 12:33:54.000000 supervision-0.4.0/supervision/detection/polygon_zone.py
--rw-r--r--   0 skalskip   (501) staff       (20)     4547 2023-03-14 12:33:54.000000 supervision-0.4.0/supervision/detection/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.768125 supervision-0.4.0/supervision/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.4.0/supervision/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.4.0/supervision/draw/color.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.4.0/supervision/draw/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.768703 supervision-0.4.0/supervision/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.4.0/supervision/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.4.0/supervision/geometry/core.py
--rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.4.0/supervision/geometry/utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.769075 supervision-0.4.0/supervision/notebook/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.4.0/supervision/notebook/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     2681 2023-04-05 15:18:58.000000 supervision-0.4.0/supervision/notebook/utils.py
--rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.4.0/supervision/video.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.765948 supervision-0.4.0/supervision.egg-info/
--rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-05 15:19:42.000000 supervision-0.4.0/supervision.egg-info/PKG-INFO
--rw-r--r--   0 skalskip   (501) staff       (20)      961 2023-04-05 15:19:42.000000 supervision-0.4.0/supervision.egg-info/SOURCES.txt
--rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-04-05 15:19:42.000000 supervision-0.4.0/supervision.egg-info/dependency_links.txt
--rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-04-05 15:19:42.000000 supervision-0.4.0/supervision.egg-info/requires.txt
--rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-04-05 15:19:42.000000 supervision-0.4.0/supervision.egg-info/top_level.txt
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.769213 supervision-0.4.0/test/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.4.0/test/__init__.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.769725 supervision-0.4.0/test/detection/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.4.0/test/detection/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     3742 2023-02-12 22:07:08.000000 supervision-0.4.0/test/detection/test_core.py
--rw-r--r--   0 skalskip   (501) staff       (20)     4916 2023-03-14 12:33:54.000000 supervision-0.4.0/test/detection/test_utils.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.770070 supervision-0.4.0/test/draw/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.4.0/test/draw/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.4.0/test/draw/test_color.py
-drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-05 15:19:42.770576 supervision-0.4.0/test/geometry/
--rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.4.0/test/geometry/__init__.py
--rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.4.0/test/geometry/test_dataclasses.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.677195 supervision-0.5.0/
+-rw-r--r--   0 skalskip   (501) staff       (20)     1065 2022-12-02 12:52:46.000000 supervision-0.5.0/LICENSE.md
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-10 21:53:21.677039 supervision-0.5.0/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     4450 2023-03-21 12:38:19.000000 supervision-0.5.0/README.md
+-rw-r--r--   0 skalskip   (501) staff       (20)       38 2023-04-10 21:53:21.677252 supervision-0.5.0/setup.cfg
+-rw-r--r--   0 skalskip   (501) staff       (20)     2220 2023-02-12 22:07:08.000000 supervision-0.5.0/setup.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.671759 supervision-0.5.0/supervision/
+-rw-r--r--   0 skalskip   (501) staff       (20)      876 2023-04-10 21:52:53.000000 supervision-0.5.0/supervision/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.672805 supervision-0.5.0/supervision/annotation/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-05 15:18:58.000000 supervision-0.5.0/supervision/annotation/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3279 2023-04-05 15:18:58.000000 supervision-0.5.0/supervision/annotation/voc.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.673662 supervision-0.5.0/supervision/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.0/supervision/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     6166 2023-04-10 21:52:53.000000 supervision-0.5.0/supervision/detection/annotate.py
+-rw-r--r--   0 skalskip   (501) staff       (20)    14672 2023-04-10 21:52:53.000000 supervision-0.5.0/supervision/detection/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     7159 2023-03-23 11:05:51.000000 supervision-0.5.0/supervision/detection/line_counter.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.673939 supervision-0.5.0/supervision/detection/tools/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-04-10 21:52:53.000000 supervision-0.5.0/supervision/detection/tools/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5058 2023-04-10 21:52:53.000000 supervision-0.5.0/supervision/detection/tools/polygon_zone.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5527 2023-04-10 21:52:53.000000 supervision-0.5.0/supervision/detection/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.674350 supervision-0.5.0/supervision/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.0/supervision/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3675 2023-02-07 18:30:08.000000 supervision-0.5.0/supervision/draw/color.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5147 2023-03-13 13:53:19.000000 supervision-0.5.0/supervision/draw/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.674749 supervision-0.5.0/supervision/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.0/supervision/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1397 2023-02-07 18:30:08.000000 supervision-0.5.0/supervision/geometry/core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)      993 2023-02-07 18:30:08.000000 supervision-0.5.0/supervision/geometry/utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.675146 supervision-0.5.0/supervision/notebook/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.0/supervision/notebook/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     2831 2023-04-10 21:52:53.000000 supervision-0.5.0/supervision/notebook/utils.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     5049 2023-02-07 18:30:08.000000 supervision-0.5.0/supervision/video.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.672524 supervision-0.5.0/supervision.egg-info/
+-rw-r--r--   0 skalskip   (501) staff       (20)     5777 2023-04-10 21:53:21.000000 supervision-0.5.0/supervision.egg-info/PKG-INFO
+-rw-r--r--   0 skalskip   (501) staff       (20)     1007 2023-04-10 21:53:21.000000 supervision-0.5.0/supervision.egg-info/SOURCES.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)        1 2023-04-10 21:53:21.000000 supervision-0.5.0/supervision.egg-info/dependency_links.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)      138 2023-04-10 21:53:21.000000 supervision-0.5.0/supervision.egg-info/requires.txt
+-rw-r--r--   0 skalskip   (501) staff       (20)       17 2023-04-10 21:53:21.000000 supervision-0.5.0/supervision.egg-info/top_level.txt
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.675289 supervision-0.5.0/test/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.0/test/__init__.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.675874 supervision-0.5.0/test/detection/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-02-07 18:30:08.000000 supervision-0.5.0/test/detection/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     3742 2023-02-12 22:07:08.000000 supervision-0.5.0/test/detection/test_core.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     4916 2023-03-14 12:33:54.000000 supervision-0.5.0/test/detection/test_utils.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.676275 supervision-0.5.0/test/draw/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-18 19:18:10.000000 supervision-0.5.0/test/draw/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1097 2023-02-02 10:53:06.000000 supervision-0.5.0/test/draw/test_color.py
+drwxr-xr-x   0 skalskip   (501) staff       (20)        0 2023-04-10 21:53:21.676717 supervision-0.5.0/test/geometry/
+-rw-r--r--   0 skalskip   (501) staff       (20)        0 2023-01-19 00:19:59.000000 supervision-0.5.0/test/geometry/__init__.py
+-rw-r--r--   0 skalskip   (501) staff       (20)     1854 2023-02-07 18:30:08.000000 supervision-0.5.0/test/geometry/test_dataclasses.py
```

### Comparing `supervision-0.4.0/LICENSE.md` & `supervision-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/PKG-INFO` & `supervision-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.4.0
+Version: 0.5.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.4.0 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.5.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.4.0/README.md` & `supervision-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/setup.py` & `supervision-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision/__init__.py` & `supervision-0.5.0/supervision/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 from supervision.annotation.voc import detections_to_voc_xml
-from supervision.detection.annotate import BoxAnnotator
+from supervision.detection.annotate import BoxAnnotator, MaskAnnotator
 from supervision.detection.core import Detections
 from supervision.detection.line_counter import LineZone, LineZoneAnnotator
-from supervision.detection.polygon_zone import PolygonZone, PolygonZoneAnnotator
-from supervision.detection.utils import generate_2d_mask
+from supervision.detection.tools.polygon_zone import PolygonZone, PolygonZoneAnnotator
+from supervision.detection.utils import generate_2d_mask, mask_to_xyxy
 from supervision.draw.color import Color, ColorPalette
 from supervision.draw.utils import draw_filled_rectangle, draw_polygon, draw_text
 from supervision.geometry.core import Point, Position, Rect
 from supervision.geometry.utils import get_polygon_center
 from supervision.notebook.utils import plot_image, plot_images_grid
 from supervision.video import (
     VideoInfo,
```

### Comparing `supervision-0.4.0/supervision/annotation/voc.py` & `supervision-0.5.0/supervision/annotation/voc.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision/detection/core.py` & `supervision-0.5.0/supervision/detection/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,124 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Iterator, List, Optional, Tuple, Union
+from typing import Any, Iterator, List, Optional, Tuple, Union
 
 import numpy as np
 
-from supervision.detection.utils import non_max_suppression
+from supervision.detection.utils import non_max_suppression, xywh_to_xyxy
 from supervision.geometry.core import Position
 
 
+def _validate_xyxy(xyxy: Any, n: int) -> None:
+    is_valid = isinstance(xyxy, np.ndarray) and xyxy.shape == (n, 4)
+    if not is_valid:
+        raise ValueError("xyxy must be 2d np.ndarray with (n, 4) shape")
+
+
+def _validate_mask(mask: Any, n: int) -> None:
+    is_valid = mask is None or (
+        isinstance(mask, np.ndarray) and len(mask.shape) == 3 and mask.shape[0] == n
+    )
+    if not is_valid:
+        raise ValueError("mask must be 3d np.ndarray with (n, W, H) shape")
+
+
+def _validate_class_id(class_id: Any, n: int) -> None:
+    is_valid = class_id is None or (
+        isinstance(class_id, np.ndarray) and class_id.shape == (n,)
+    )
+    if not is_valid:
+        raise ValueError("class_id must be None or 1d np.ndarray with (n,) shape")
+
+
+def _validate_confidence(confidence: Any, n: int) -> None:
+    is_valid = confidence is None or (
+        isinstance(confidence, np.ndarray) and confidence.shape == (n,)
+    )
+    if not is_valid:
+        raise ValueError("confidence must be None or 1d np.ndarray with (n,) shape")
+
+
+def _validate_tracker_id(tracker_id: Any, n: int) -> None:
+    is_valid = tracker_id is None or (
+        isinstance(tracker_id, np.ndarray) and tracker_id.shape == (n,)
+    )
+    if not is_valid:
+        raise ValueError("tracker_id must be None or 1d np.ndarray with (n,) shape")
+
+
 @dataclass
 class Detections:
     """
     Data class containing information about the detections in a video frame.
 
     Attributes:
         xyxy (np.ndarray): An array of shape `(n, 4)` containing the bounding boxes coordinates in format `[x1, y1, x2, y2]`
+        mask: (Optional[np.ndarray]): An array of shape `(n, W, H)` containing the segmentation masks.
         class_id (Optional[np.ndarray]): An array of shape `(n,)` containing the class ids of the detections.
         confidence (Optional[np.ndarray]): An array of shape `(n,)` containing the confidence scores of the detections.
         tracker_id (Optional[np.ndarray]): An array of shape `(n,)` containing the tracker ids of the detections.
     """
 
     xyxy: np.ndarray
+    mask: np.Optional[np.ndarray] = None
     class_id: Optional[np.ndarray] = None
     confidence: Optional[np.ndarray] = None
     tracker_id: Optional[np.ndarray] = None
 
     def __post_init__(self):
         n = len(self.xyxy)
-        validators = [
-            (isinstance(self.xyxy, np.ndarray) and self.xyxy.shape == (n, 4)),
-            self.class_id is None
-            or (isinstance(self.class_id, np.ndarray) and self.class_id.shape == (n,)),
-            self.confidence is None
-            or (
-                isinstance(self.confidence, np.ndarray)
-                and self.confidence.shape == (n,)
-            ),
-            self.tracker_id is None
-            or (
-                isinstance(self.tracker_id, np.ndarray)
-                and self.tracker_id.shape == (n,)
-            ),
-        ]
-        if not all(validators):
-            raise ValueError(
-                "xyxy must be 2d np.ndarray with (n, 4) shape, "
-                "class_id must be None or 1d np.ndarray with (n,) shape, "
-                "confidence must be None or 1d np.ndarray with (n,) shape, "
-                "tracker_id must be None or 1d np.ndarray with (n,) shape"
-            )
+        _validate_xyxy(xyxy=self.xyxy, n=n)
+        _validate_mask(mask=self.mask, n=n)
+        _validate_class_id(class_id=self.class_id, n=n)
+        _validate_confidence(confidence=self.confidence, n=n)
+        _validate_tracker_id(tracker_id=self.tracker_id, n=n)
 
     def __len__(self):
         """
         Returns the number of detections in the Detections object.
         """
         return len(self.xyxy)
 
     def __iter__(
         self,
-    ) -> Iterator[Tuple[np.ndarray, Optional[float], int, Optional[Union[str, int]]]]:
+    ) -> Iterator[
+        Tuple[
+            np.ndarray,
+            Optional[np.ndarray],
+            Optional[float],
+            Optional[int],
+            Optional[int],
+        ]
+    ]:
         """
-        Iterates over the Detections object and yield a tuple of `(xyxy, confidence, class_id, tracker_id)` for each detection.
+        Iterates over the Detections object and yield a tuple of `(xyxy, mask, confidence, class_id, tracker_id)` for each detection.
         """
         for i in range(len(self.xyxy)):
             yield (
                 self.xyxy[i],
+                self.mask[i] if self.mask is not None else None,
                 self.confidence[i] if self.confidence is not None else None,
                 self.class_id[i] if self.class_id is not None else None,
                 self.tracker_id[i] if self.tracker_id is not None else None,
             )
 
     def __eq__(self, other: Detections):
         return all(
             [
                 np.array_equal(self.xyxy, other.xyxy),
                 any(
                     [
+                        self.mask is None and other.mask is None,
+                        np.array_equal(self.mask, other.mask),
+                    ]
+                ),
+                any(
+                    [
                         self.class_id is None and other.class_id is None,
                         np.array_equal(self.class_id, other.class_id),
                     ]
                 ),
                 any(
                     [
                         self.confidence is None and other.confidence is None,
@@ -109,15 +147,15 @@
 
         Example:
             ```python
             >>> import torch
             >>> from supervision import Detections
 
             >>> model = torch.hub.load('ultralytics/yolov5', 'yolov5s')
-            >>> results = model(frame)
+            >>> results = model(IMAGE)
             >>> detections = Detections.from_yolov5(results)
             ```
         """
         yolov5_detections_predictions = yolov5_results.pred[0].cpu().cpu().numpy()
         return cls(
             xyxy=yolov5_detections_predictions[:, :4],
             confidence=yolov5_detections_predictions[:, 4],
@@ -137,16 +175,16 @@
 
         Example:
             ```python
             >>> from ultralytics import YOLO
             >>> from supervision import Detections
 
             >>> model = YOLO('yolov8s.pt')
-            >>> results = model(frame)[0]
-            >>> detections = Detections.from_yolov8(results)
+            >>> yolov8_results = model(IMAGE)[0]
+            >>> detections = Detections.from_yolov8(yolov8_results)
             ```
         """
         return cls(
             xyxy=yolov8_results.boxes.xyxy.cpu().numpy(),
             confidence=yolov8_results.boxes.conf.cpu().numpy(),
             class_id=yolov8_results.boxes.cls.cpu().numpy().astype(int),
         )
@@ -198,14 +236,45 @@
         return Detections(
             xyxy=np.array(xyxy),
             confidence=np.array(confidence),
             class_id=np.array(class_id).astype(int),
         )
 
     @classmethod
+    def from_sam(cls, sam_result: List[dict]) -> Detections:
+        """
+        Creates a Detections instance from Segment Anything Model (SAM) by Meta AI.
+
+        Args:
+            sam_result (List[dict]): The output Results instance from SAM
+
+        Returns:
+            Detections: A new Detections object.
+
+        Example:
+            ```python
+            >>> from segment_anything import sam_model_registry, SamAutomaticMaskGenerator
+            >>> import supervision as sv
+
+            >>> sam = sam_model_registry[MODEL_TYPE](checkpoint=CHECKPOINT_PATH).to(device=DEVICE)
+            >>> mask_generator = SamAutomaticMaskGenerator(sam)
+            >>> sam_result = mask_generator.generate(IMAGE)
+            >>> detections = sv.Detections.from_sam(sam_result=sam_result)
+            ```
+        """
+        sorted_generated_masks = sorted(
+            sam_result, key=lambda x: x["area"], reverse=True
+        )
+
+        xywh = np.array([mask["bbox"] for mask in sorted_generated_masks])
+        mask = np.array([mask["segmentation"] for mask in sorted_generated_masks])
+
+        return Detections(xyxy=xywh_to_xyxy(boxes_xywh=xywh), mask=mask)
+
+    @classmethod
     def from_coco_annotations(cls, coco_annotation: dict) -> Detections:
         xyxy, class_id = [], []
 
         for annotation in coco_annotation:
             x_min, y_min, width, height = annotation["bbox"]
             xyxy.append([x_min, y_min, x_min + width, y_min + height])
             class_id.append(annotation["category_id"])
@@ -261,14 +330,28 @@
         raise TypeError(
             f"Detections.__getitem__ not supported for index of type {type(index)}."
         )
 
     @property
     def area(self) -> np.ndarray:
         """
+        Calculate the area of each detection in the set of object detections. If masks field is defined property
+        returns are of each mask. If only box is given property return area of each box.
+
+        Returns:
+          np.ndarray: An array of floats containing the area of each detection in the format of `(area_1, area_2, ..., area_n)`, where n is the number of detections.
+        """
+        if self.mask is not None:
+            return np.ndarray([np.sum(mask) for mask in self.mask])
+        else:
+            return self.box_area
+
+    @property
+    def box_area(self) -> np.ndarray:
+        """
         Calculate the area of each bounding box in the set of object detections.
 
         Returns:
             np.ndarray: An array of floats containing the area of each bounding box in the format of `(area_1, area_2, ..., area_n)`, where n is the number of detections.
         """
         return (self.xyxy[:, 3] - self.xyxy[:, 1]) * (self.xyxy[:, 2] - self.xyxy[:, 0])
```

### Comparing `supervision-0.4.0/supervision/detection/line_counter.py` & `supervision-0.5.0/supervision/detection/line_counter.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision/detection/utils.py` & `supervision-0.5.0/supervision/detection/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,7 +111,38 @@
         clipped to fit within the frame resolution.
     """
     result = np.copy(boxes_xyxy)
     width, height = frame_resolution_wh
     result[:, [0, 2]] = result[:, [0, 2]].clip(0, width)
     result[:, [1, 3]] = result[:, [1, 3]].clip(0, height)
     return result
+
+
+def xywh_to_xyxy(boxes_xywh: np.ndarray) -> np.ndarray:
+    xyxy = boxes_xywh.copy()
+    xyxy[:, 2] = boxes_xywh[:, 0] + boxes_xywh[:, 2]
+    xyxy[:, 3] = boxes_xywh[:, 1] + boxes_xywh[:, 3]
+    return xyxy
+
+
+def mask_to_xyxy(masks: np.ndarray) -> np.ndarray:
+    """
+    Converts a 3D `np.array` of 2D bool masks into a 2D `np.array` of bounding boxes.
+
+    Parameters:
+        masks (np.ndarray): A 3D `np.array` of shape `(N, W, H)` containing 2D bool masks
+
+    Returns:
+        np.ndarray: A 2D `np.array` of shape `(N, 4)` containing the bounding boxes `(x_min, y_min, x_max, y_max)` for each mask
+    """
+    n = masks.shape[0]
+    bboxes = np.zeros((n, 4), dtype=int)
+
+    for i, mask in enumerate(masks):
+        rows, cols = np.where(mask)
+
+        if len(rows) > 0 and len(cols) > 0:
+            x_min, x_max = np.min(cols), np.max(cols)
+            y_min, y_max = np.min(rows), np.max(rows)
+            bboxes[i, :] = [x_min, y_min, x_max, y_max]
+
+    return bboxes
```

### Comparing `supervision-0.4.0/supervision/draw/color.py` & `supervision-0.5.0/supervision/draw/color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision/draw/utils.py` & `supervision-0.5.0/supervision/draw/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision/geometry/core.py` & `supervision-0.5.0/supervision/geometry/core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision/geometry/utils.py` & `supervision-0.5.0/supervision/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision/notebook/utils.py` & `supervision-0.5.0/supervision/notebook/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 def plot_image(
-    image: np.ndarray, size: Tuple[int, int] = (10, 10), cmap: Optional[str] = "gray"
+    image: np.ndarray, size: Tuple[int, int] = (12, 12), cmap: Optional[str] = "gray"
 ) -> None:
     """
     Plots image using matplotlib.
 
     Args:
         image (np.ndarray): The frame to be displayed.
         size (Tuple[int, int]): The size of the plot.
@@ -23,37 +23,41 @@
 
         >>> image = cv2.imread("path/to/image.jpg")
 
         %matplotlib inline
         >>> sv.plot_image(image, (16, 16))
         ```
     """
+    plt.figure(figsize=size)
+
     if image.ndim == 2:
-        plt.figure(figsize=size)
         plt.imshow(image, cmap=cmap)
     else:
-        plt.figure(figsize=size)
         plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
+
+    plt.axis("off")
     plt.show()
 
 
 def plot_images_grid(
     images: List[np.ndarray],
     grid_size: Tuple[int, int],
     titles: Optional[List[str]] = None,
     size: Tuple[int, int] = (12, 12),
+    cmap: Optional[str] = "gray",
 ) -> None:
     """
     Plots images in a grid using matplotlib.
 
     Args:
        images (List[np.ndarray]): A list of images as numpy arrays.
        grid_size (Tuple[int, int]): A tuple specifying the number of rows and columns for the grid.
        titles (Optional[List[str]]): A list of titles for each image. Defaults to None.
        size (Tuple[int, int]): A tuple specifying the width and height of the entire plot in inches.
+       cmap (str): the colormap to use for single channel images.
 
     Raises:
        ValueError: If the number of images exceeds the grid size.
 
     Examples:
         ```python
         >>> import cv2
@@ -66,27 +70,28 @@
         >>> images = [image1, image2, image3]
         >>> titles = ["Image 1", "Image 2", "Image 3"]
 
         %matplotlib inline
         >>> plot_images_grid(images, grid_size=(2, 2), titles=titles, figsize=(16, 16))
         ```
     """
-
     nrows, ncols = grid_size
 
     if len(images) > nrows * ncols:
         raise ValueError(
             "The number of images exceeds the grid size. Please increase the grid size or reduce the number of images."
         )
 
     fig, axes = plt.subplots(nrows=nrows, ncols=ncols, figsize=size)
 
     for idx, ax in enumerate(axes.flat):
         if idx < len(images):
-            ax.imshow(cv2.cvtColor(images[idx], cv2.COLOR_BGR2RGB))
+            if images[idx].ndim == 2:
+                ax.imshow(images[idx], cmap=cmap)
+            else:
+                ax.imshow(cv2.cvtColor(images[idx], cv2.COLOR_BGR2RGB))
+
             if titles is not None and idx < len(titles):
                 ax.set_title(titles[idx])
-            ax.axis("off")
-        else:
-            ax.axis("off")
 
+        ax.axis("off")
     plt.show()
```

### Comparing `supervision-0.4.0/supervision/video.py` & `supervision-0.5.0/supervision/video.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/supervision.egg-info/PKG-INFO` & `supervision-0.5.0/supervision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supervision
-Version: 0.4.0
+Version: 0.5.0
 Summary: A set of easy-to-use utils that will come in handy in any Computer Vision project
 Home-page: https://github.com/roboflow/supervision
 Author: Piotr Skalski
 Author-email: piotr.skalski92@gmail.com
 License: MIT
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supervision Version: 0.4.0 Summary: A set of easy-
+Metadata-Version: 2.1 Name: supervision Version: 0.5.0 Summary: A set of easy-
 to-use utils that will come in handy in any Computer Vision project Home-page:
 https://github.com/roboflow/supervision Author: Piotr Skalski Author-email:
 piotr.skalski92@gmail.com License: MIT Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLOv5,YOLOv8,Roboflow Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `supervision-0.4.0/supervision.egg-info/SOURCES.txt` & `supervision-0.5.0/supervision.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 supervision.egg-info/top_level.txt
 supervision/annotation/__init__.py
 supervision/annotation/voc.py
 supervision/detection/__init__.py
 supervision/detection/annotate.py
 supervision/detection/core.py
 supervision/detection/line_counter.py
-supervision/detection/polygon_zone.py
 supervision/detection/utils.py
+supervision/detection/tools/__init__.py
+supervision/detection/tools/polygon_zone.py
 supervision/draw/__init__.py
 supervision/draw/color.py
 supervision/draw/utils.py
 supervision/geometry/__init__.py
 supervision/geometry/core.py
 supervision/geometry/utils.py
 supervision/notebook/__init__.py
```

### Comparing `supervision-0.4.0/test/detection/test_core.py` & `supervision-0.5.0/test/detection/test_core.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/test/detection/test_utils.py` & `supervision-0.5.0/test/detection/test_utils.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/test/draw/test_color.py` & `supervision-0.5.0/test/draw/test_color.py`

 * *Files identical despite different names*

### Comparing `supervision-0.4.0/test/geometry/test_dataclasses.py` & `supervision-0.5.0/test/geometry/test_dataclasses.py`

 * *Files identical despite different names*

