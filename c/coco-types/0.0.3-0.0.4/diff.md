# Comparing `tmp/coco_types-0.0.3.tar.gz` & `tmp/coco_types-0.0.4.tar.gz`

## Comparing `coco_types-0.0.3.tar` & `coco_types-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 coco_types-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 coco_types-0.0.3/pyrightconfig.json
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 coco_types-0.0.3/pytest.ini
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 coco_types-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 coco_types-0.0.3/requirements-test.txt
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 coco_types-0.0.3/requirements.txt
--rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 coco_types-0.0.3/setup.cfg
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 coco_types-0.0.3/coco_types/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 coco_types-0.0.3/coco_types/coco_keypoints.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 coco_types-0.0.3/coco_types/coco_object_detection.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 coco_types-0.0.3/coco_types/dicts/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 coco_types-0.0.3/coco_types/dicts/coco_keypoints.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 coco_types-0.0.3/coco_types/dicts/coco_object_detection.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 coco_types-0.0.3/tests/test_load_pydantic.py
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 coco_types-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 coco_types-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 coco_types-0.0.3/README.md
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 coco_types-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 coco_types-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 coco_types-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 coco_types-0.0.4/pyrightconfig.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 coco_types-0.0.4/pytest.ini
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 coco_types-0.0.4/requirements-dev.txt
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 coco_types-0.0.4/requirements-test.txt
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 coco_types-0.0.4/requirements.txt
+-rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 coco_types-0.0.4/setup.cfg
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 coco_types-0.0.4/coco_types/__init__.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 coco_types-0.0.4/coco_types/coco_keypoints.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 coco_types-0.0.4/coco_types/coco_object_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coco_types-0.0.4/coco_types/py.typed
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 coco_types-0.0.4/coco_types/dicts/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 coco_types-0.0.4/coco_types/dicts/coco_keypoints.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 coco_types-0.0.4/coco_types/dicts/coco_object_detection.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 coco_types-0.0.4/tests/test_load_pydantic.py
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 coco_types-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 coco_types-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 coco_types-0.0.4/README.md
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 coco_types-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 coco_types-0.0.4/PKG-INFO
```

### Comparing `coco_types-0.0.3/.pre-commit-config.yaml` & `coco_types-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/pyrightconfig.json` & `coco_types-0.0.4/pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/requirements-dev.txt` & `coco_types-0.0.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/requirements-test.txt` & `coco_types-0.0.4/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/setup.cfg` & `coco_types-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/coco_types/__init__.py` & `coco_types-0.0.4/coco_types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 import coco_types.dicts  # pyright: ignore[reportUnusedImport]
 
 from .coco_keypoints import AnnotationKP, CategoryKP, DatasetKP
 from .coco_object_detection import (Annotation, BaseModel, Category, Dataset, EncodedRLE, Image, Info, Licence, RLE,
                                     TPolygon_segmentation)
```

### Comparing `coco_types-0.0.3/coco_types/coco_keypoints.py` & `coco_types-0.0.4/coco_types/coco_keypoints.py`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/coco_types/coco_object_detection.py` & `coco_types-0.0.4/coco_types/coco_object_detection.py`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/coco_types/dicts/coco_object_detection.py` & `coco_types-0.0.4/coco_types/dicts/coco_object_detection.py`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/LICENSE.md` & `coco_types-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/README.md` & `coco_types-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,18 @@
-# coco_utils
+# COCO Types
 
 Note: This package loads the data as is and does not create dictionaries mapping ids to lists of images/annotations/categories.
 
+## Installation
+
+The package is available on pypi [here](https://pypi.org/project/coco-types/), you can install it with:
+```
+pip install coco-types
+```
+
 ## Loading COCO data
 
 You can load COCO dataset labels into Pydantic objects by using the `Dataset` and `DatasetKP` classes.
 
 For an object detection dataset:
 ```python
 import coco_types
```

### Comparing `coco_types-0.0.3/pyproject.toml` & `coco_types-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.3/PKG-INFO` & `coco_types-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coco_types
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for handling COCO datasets types.
 Project-URL: Homepage, https://github.com/hoel-bagard/coco_types
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/coco_types/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE.md
 Keywords: COCO,COCO dataset
@@ -26,18 +26,25 @@
 Requires-Dist: pep8-naming; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
-# coco_utils
+# COCO Types
 
 Note: This package loads the data as is and does not create dictionaries mapping ids to lists of images/annotations/categories.
 
+## Installation
+
+The package is available on pypi [here](https://pypi.org/project/coco-types/), you can install it with:
+```
+pip install coco-types
+```
+
 ## Loading COCO data
 
 You can load COCO dataset labels into Pydantic objects by using the `Dataset` and `DatasetKP` classes.
 
 For an object detection dataset:
 ```python
 import coco_types
```

