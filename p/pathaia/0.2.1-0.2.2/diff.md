# Comparing `tmp/pathaia-0.2.1.tar.gz` & `tmp/pathaia-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PathAIA/PathAIA/dist/tmpzq9kwjrp/pathaia-0.2.1.tar", last modified: Mon Feb 14 09:46:00 2022, max compression
+gzip compressed data, was "/home/runner/work/PathAIA/PathAIA/dist/.tmp-sybdqe43/pathaia-0.2.2.tar", last modified: Tue Apr 11 08:21:38 2023, max compression
```

## Comparing `pathaia-0.2.1.tar` & `pathaia-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-02-14 09:45:48.000000 pathaia-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-02-14 09:46:00.000000 pathaia-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5167 2022-02-14 09:45:48.000000 pathaia-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3752 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/datasets/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/datasets/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    21320 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/datasets/functional_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/datasets/object_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia/graphs/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11849 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/graphs/clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/graphs/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    15860 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/graphs/functional_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/graphs/kruskal.py
--rw-r--r--   0 runner    (1001) docker     (121)    17697 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/graphs/object_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/graphs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia/patches/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    28451 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/functional_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6622 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/object_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4216 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/slide_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/patches/visu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia/semantic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/semantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/semantic/functional_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)    11170 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/util/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     6739 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/util/images.py
--rw-r--r--   0 runner    (1001) docker     (121)    12227 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/util/management.py
--rw-r--r--   0 runner    (1001) docker     (121)     6166 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/util/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     7158 2022-02-14 09:45:48.000000 pathaia-0.2.1/pathaia/util/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-02-14 09:45:59.000000 pathaia-0.2.1/pathaia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 09:45:59.000000 pathaia-0.2.1/pathaia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 09:45:59.000000 pathaia-0.2.1/pathaia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-14 09:46:00.000000 pathaia-0.2.1/pathaia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-14 09:46:00.000000 pathaia-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-02-14 09:45:48.000000 pathaia-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 09:46:00.000000 pathaia-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-14 09:45:48.000000 pathaia-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18276 2022-02-14 09:45:48.000000 pathaia-0.2.1/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-02-14 09:45:48.000000 pathaia-0.2.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-11 08:21:27.000000 pathaia-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-04-11 08:21:38.000000 pathaia-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5167 2023-04-11 08:21:27.000000 pathaia-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21320 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/functional_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/object_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/graphs/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11849 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15868 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/functional_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/kruskal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17649 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5683 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28403 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/functional_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6622 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/slide_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/visu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/semantic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/semantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/semantic/functional_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/util/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11170 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12227 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/management.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6166 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:21:37.000000 pathaia-0.2.2/pathaia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 08:21:38.000000 pathaia-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-04-11 08:21:27.000000 pathaia-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18276 2023-04-11 08:21:27.000000 pathaia-0.2.2/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-04-11 08:21:27.000000 pathaia-0.2.2/tests/helpers.py
```

### Comparing `pathaia-0.2.1/LICENSE` & `pathaia-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/PKG-INFO` & `pathaia-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pathaia
-Version: 0.2.1
+Version: 0.2.2
 Summary: procedures for wsi analysis
 Author: Arnaud Abreu
 Author-email: arnaud.abreu.p@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 # PathAIA
 
@@ -134,9 +132,7 @@
   title={PathAIA},
   author={Abreu, A and .al},
   journal={GitHub. Note: https://github.com/ArnaudAbreu/PathAIA},
   volume={3},
   year={2021}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: pathaia Version: 0.2.1 Summary: procedures for wsi
-analysis Author: Arnaud Abreu Author-email: arnaud.abreu.p@gmail.com License:
-UNKNOWN Platform: UNKNOWN Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: pathaia Version: 0.2.2 Summary: procedures for wsi
+analysis Author: Arnaud Abreu Author-email: arnaud.abreu.p@gmail.com
+Description-Content-Type: text/markdown License-File: LICENSE
           # PathAIA **Simple digital pathology analysis tools.** ---
      Basic_Usage â¢ Advanced_features â¢ Docs â¢ Community â¢ License
    [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pathaia)]
  (https://pypi.org/project/pathaia/) [![PyPI Status](https://badge.fury.io/py/
    pathaia.svg)](https://badge.fury.io/py/pathaia) [![PyPI Status](https://
 pepy.tech/badge/pathaia)](https://pepy.tech/project/pathaia) [![codecov](https:
            //codecov.io/gh/ArnaudAbreu/PathAIA/branch/master/graph/
```

### Comparing `pathaia-0.2.1/README.md` & `pathaia-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/datasets/data.py` & `pathaia-0.2.2/pathaia/datasets/data.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/datasets/errors.py` & `pathaia-0.2.2/pathaia/datasets/errors.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/datasets/functional_api.py` & `pathaia-0.2.2/pathaia/datasets/functional_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/graphs/clustering.py` & `pathaia-0.2.2/pathaia/graphs/clustering.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/graphs/errors.py` & `pathaia-0.2.2/pathaia/graphs/errors.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/graphs/functional_api.py` & `pathaia-0.2.2/pathaia/graphs/functional_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     InvalidNodeProps,
     UnrelatedNode,
     UnknownNodeProperty,
     InvalidTree,
 )
 from .kruskal import UFDS
 import json
-from nptyping import NDArray
-from numbers import Number
+from nptyping import NDArray, Shape, Number
 
 
 def complete_tree(
     parents: Optional[Parenthood] = None, children: Optional[Childhood] = None
 ):
     if parents is None:
         parents = {}
@@ -371,16 +370,16 @@
             )
         dist += weights[node]
     # minus 1 otherwise ancestor is counted twice
     return dist
 
 
 def farthest_point_sampling(
-    coords: NDArray[(Any, Any), Number], n_samples: Union[int, float]
-) -> NDArray[(Any,), np.int32]:
+    coords: NDArray[Shape["N, N"], Number], n_samples: Union[int, float]
+) -> NDArray[Shape["N"], np.int32]:
     """
     Perform farthest points sampling using point coordinates array.
 
     Args:
         coords: array containing point coordinates.
         n_samples: number of point to sample. If a float is given, represents the
             proportion of points used instead.
@@ -398,18 +397,18 @@
         idxs[i] = np.argmax(distances)
         distances = np.minimum(distances, ((coords[idxs[i]] - coords) ** 2).sum(1))
 
     return idxs
 
 
 def random_farthest_point_sampling(
-    coords: NDArray[(Any, Any), Number],
+    coords: NDArray[Shape["N, N"], Number],
     n_farthest_samples: Union[int, float] = 0.3,
     n_random_samples: Union[int, float] = 0.1,
-) -> NDArray[(Any,), np.int32]:
+) -> NDArray[Shape["N"], np.int32]:
     """
     Perform farthest points sampling using point coordinates array followed by random
     sampling .
 
     Args:
         coords: array containing point coordinates.
         n_farthest_samples: number of points to keep using farthest points sampling.
@@ -431,15 +430,15 @@
     random_idxs = np.random.choice(random_idxs, size=n_random_samples, p=probs)
     idxs = np.concatenate((farthest_idxs, random_idxs))
 
     return idxs
 
 
 def get_kneighbors_graph(
-    points: NDArray[(Any, Any), Number],
+    points: NDArray[Shape["N, N"], Number],
     n_farthest_samples: Union[int, float] = 0.3,
     n_random_samples: Union[int, float] = 0.1,
     dmax: int = 500,
     n_neighbors: int = 5,
     n_jobs: Optional[int] = None,
 ) -> spmatrix:
     """
@@ -470,15 +469,15 @@
     A = knn.kneighbors_graph(mode="distance")
     Abool = A.astype(bool) - (A > dmax)
     A = A.multiply(Abool)
     return A.maximum(A.T)
 
 
 def get_nodeprops_edgeprops(
-    A: spmatrix, coords: NDArray[(Any, Any), Number]
+    A: spmatrix, coords: NDArray[Shape["N, N"], Number]
 ) -> Tuple[NodeProperties, EdgeProperties]:
     """
     Get coordinates and distances between edges of a graph as NodeProperties and
     EdgeProperties.
 
     Args:
         A: Sparse distance matrix representing the graph.
```

### Comparing `pathaia-0.2.1/pathaia/graphs/kruskal.py` & `pathaia-0.2.2/pathaia/graphs/kruskal.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/graphs/object_api.py` & `pathaia-0.2.2/pathaia/graphs/object_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,23 +340,21 @@
         try:
             self.children_[parent].add(child)
         except KeyError:
             self.children_[parent] = {child}
         super().add_edge((parent, child))
 
     def add_children(self, parent: Node, children: Sequence[Node]):
-        edges = set()
         for child in children:
             self.parents_[child] = parent
-            edges.add((parent, child))
+            super().add_edge((parent, child))
         try:
             self.children_[parent] |= set(children)
         except KeyError:
             self.children_[parent] = set(children)
-        super().add_edges(edges)
 
     def add_edges(self, edges: Sequence[Tuple[Node, Union[Node, Sequence[Node]]]]):
         for p, c in edges:
             if isinstance(c, Node):
                 self.add_edge(p, c)
             else:
                 self.add_children(p, c)
```

### Comparing `pathaia-0.2.1/pathaia/graphs/types.py` & `pathaia-0.2.2/pathaia/graphs/types.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/patches/errors.py` & `pathaia-0.2.2/pathaia/patches/errors.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/patches/filters.py` & `pathaia-0.2.2/pathaia/patches/filters.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/patches/functional_api.py` & `pathaia-0.2.2/pathaia/patches/functional_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,21 +146,20 @@
     if len(ancestors) > 0:
         mag = slide.level_downsamples[level]
         shape = Coord(ancestors[0].size_0) / mag
         size_0 = psize * mag
         patches = []
         for ancestor in ancestors:
             # ancestor is a patch
-            rx, ry = ancestor.position
             prefix = ancestor.id
             k = 0
             for patch_coord in regular_grid(shape, interval, psize):
                 k += 1
                 idx = "{}#{}".format(prefix, k)
-                position = patch_coord * mag + ry
+                position = patch_coord * mag + ancestor.position
                 patches.append(
                     Patch(
                         id=idx,
                         slidename=slide._filename.split("/")[-1],
                         position=position,
                         level=level,
                         size=psize,
@@ -249,21 +248,20 @@
     slide_filters = listify(slide_filters)
     if len(ancestors) > 0:
         mag = slide.level_downsamples[level]
         shape = Coord(ancestors[0].size_0) / mag
         size_0 = psize * mag
         for ancestor in ancestors:
             # ancestor is a patch
-            rx, ry = ancestor.position
             prefix = ancestor.id
             k = 0
             for patch_coord in regular_grid(shape, interval, psize):
                 k += 1
                 idx = "{}#{}".format(prefix, k)
-                position = patch_coord * mag + ry
+                position = patch_coord * mag + ancestor.position
                 yield Patch(
                     id=idx,
                     slidename=slide._filename.split("/")[-1],
                     position=position,
                     level=level,
                     size=psize,
                     size_0=size_0,
```

### Comparing `pathaia-0.2.1/pathaia/patches/object_api.py` & `pathaia-0.2.2/pathaia/patches/object_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/patches/slide_filters.py` & `pathaia-0.2.2/pathaia/patches/slide_filters.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/patches/visu.py` & `pathaia-0.2.2/pathaia/patches/visu.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,37 +32,38 @@
     Returns:
         Thumbnail image with patches displayed.
 
     """
     # get thumbnail first
     slide_size = Coord(slide.dimensions)
     if size_0 is None:
-        size_0 = Coord(queries[0].size_0)
+        size_0 = Coord(queries[0].size_0) if len(queries) != 0 else Coord(min_res)
     thickness = 2 * (thickness // 2) + 1
     res = slide_size / size_0 * (thickness + cell_size) + thickness
     thumb_w = max(min_res, res.x)
     thumb_h = max(min_res, res.y)
     image = slide.get_thumbnail((thumb_w, thumb_h))
     thumb_size = Coord(image.size)
-    dsr = slide_size[0] / thumb_size[0]
+    dsr_x = slide_size[0] / thumb_size[0]
+    dsr_y = slide_size[1] / thumb_size[1]
     image = numpy.array(image)[:, :, 0:3]
     # get grid
-    grid = 255 * numpy.ones((thumb_size.y, thumb_size.x), numpy.uint8)
+    grid = numpy.zeros((thumb_size.y, thumb_size.x), numpy.uint8)
     for query in queries:
         # position in queries are absolute
-        x, y = query.position / dsr
-        dx, dy = query.size_0 / dsr
+        x, y = round(query.position[0] / dsr_x), round(query.position[1] / dsr_y)
+        dx, dy = round(query.size_0[0] / dsr_x), round(query.size_0[1] / dsr_y)
+        #? startx = numpy.clip(x, 0, thumb_size.x - 1)
         startx = min(x, thumb_size.x - 1)
         starty = min(y, thumb_size.y - 1)
         endx = min(x + dx, thumb_size.x - 1)
         endy = min(y + dy, thumb_size.y - 1)
         # horizontal segments
-        grid[starty, startx:endx] = 0
-        grid[endy, startx:endx] = 0
+        grid[starty, startx:endx] = 1
+        grid[endy - 1, startx:endx] = 1
         # vertical segments
-        grid[starty:endy, startx] = 0
-        grid[starty:endy, endx] = 0
-    grid = grid < 255
+        grid[starty:endy, startx] = 1
+        grid[starty:endy, endx - 1] = 1
     d = disk(thickness//2)
     grid = binary_dilation(grid, d)
     image[grid] = color
     return image
```

### Comparing `pathaia-0.2.1/pathaia/semantic/functional_api.py` & `pathaia-0.2.2/pathaia/semantic/functional_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/util/convert.py` & `pathaia-0.2.2/pathaia/util/convert.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/util/images.py` & `pathaia-0.2.2/pathaia/util/images.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from skimage.io import imread
 from skimage.transform import resize
 from .paths import imfiles_in_folder
 from .types import NDBoolMask, PathLike, NDImage, NDByteImage, Coord
 from ..patches.compat import convert_coords
 import itertools
 from typing import Iterator, List, Tuple, Sequence, Optional, Union, Any
-from nptyping import NDArray
+from nptyping import NDArray, Shape, Float
 
 
 def regular_grid(shape: Coord, interval: Coord, psize: Coord) -> Iterator[Coord]:
     """
     Get a regular grid of position on a slide given its dimensions.
 
     Arguments:
@@ -112,15 +112,15 @@
             yield imfile, imread(imfile)
         else:
             yield imread(imfile)
 
 
 def sample_img(
     image: NDImage, psize: int, spl_per_image: int, mask: NDBoolMask = None
-) -> List[NDArray[(Any,), float]]:
+) -> List[NDArray[Shape["N"], Float]]:
     """
     Split image in patches.
 
     Args:
         image: numpy image to fit on.
         psize: size in pixels of the side of a patch.
         spl_per_image: maximum number of patches to extract in image.
@@ -152,15 +152,15 @@
     positions = positions[0:spl_per_image]
     patches = [img[i : i + psize, j : j + psize].reshape(-1) for i, j in positions]
     return patches
 
 
 def sample_img_sep_channels(
     image: NDByteImage, psize: int, spl_per_image: int, mask: NDBoolMask = None
-) -> Tuple[List[NDArray[(Any,), float]], ...]:
+) -> Tuple[List[NDArray[Shape["N"], Float]], ...]:
     """Fit vocabulary on a single image.
 
     Split image in patches and fit on them.
 
     Args:
         image: numpy image to fit on.
         psize: size in pixels of the side of a patch.
```

### Comparing `pathaia-0.2.1/pathaia/util/management.py` & `pathaia-0.2.2/pathaia/util/management.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/util/paths.py` & `pathaia-0.2.2/pathaia/util/paths.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/pathaia/util/types.py` & `pathaia-0.2.2/pathaia/util/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import (
-    Any,
     Callable,
     Dict,
     Sequence,
     Union,
     NamedTuple,
     Optional,
     List,
     Tuple,
 )
-from nptyping import NDArray
+from nptyping import NDArray, Shape
 import os
 import numpy
 from dataclasses import dataclass
 from openslide import OpenSlide
 from pathlib import Path
 import warnings
 from PIL import Image
+from collections.abc import Iterable
 
 try:
     from cucim import CuImage
 except ImportError:
     pass
 
 
@@ -31,17 +31,19 @@
 
 class Coord(_CoordBase):
     """
     An (x, y) tuple representing integer coordinates.
     If only x is given then takes value (x, x).
     """
 
-    def __new__(cls, x: Union[_CoordBase, int], y: Optional[int] = None):
+    def __new__(cls, x: Union[int, Iterable], y: Optional[int] = None):
         if y is None:
-            if isinstance(x, tuple):
+            if isinstance(x, dict):
+                x, y = x["x"], x["y"]
+            elif isinstance(x, Iterable):
                 x, y = x
             else:
                 y = x
         return super().__new__(cls, int(x), int(y))
 
     def __add__(self, other):
         x, y = self.__class__(other)
@@ -133,36 +135,36 @@
         )
 
 
 Filter = Sequence[Union[str, Callable]]
 FilterList = Union[str, Sequence[Filter], Dict[int, Sequence[Filter]]]
 PathLike = Union[str, os.PathLike]
 
-NDByteImage = NDArray[(Any, Any, 3), numpy.uint8]
-NDFloat32Image = NDArray[(Any, Any, 3), numpy.float32]
-NDFloat64Image = NDArray[(Any, Any, 3), numpy.float64]
+NDByteImage = NDArray[Shape["*, *, 3"], numpy.uint8]
+NDFloat32Image = NDArray[Shape["*, *, 3"], numpy.float32]
+NDFloat64Image = NDArray[Shape["*, *, 3"], numpy.float64]
 NDFloatImage = Union[NDFloat32Image, NDFloat64Image]
 NDImage = Union[NDByteImage, NDFloatImage]
 
-NDByteGrayImage = NDArray[(Any, Any), numpy.uint8]
-NDFloat32GrayImage = NDArray[(Any, Any), numpy.float32]
-NDFloat64GrayImage = NDArray[(Any, Any), numpy.float64]
+NDByteGrayImage = NDArray[Shape["*, *"], numpy.uint8]
+NDFloat32GrayImage = NDArray[Shape["*, *"], numpy.float32]
+NDFloat64GrayImage = NDArray[Shape["*, *"], numpy.float64]
 NDFloatGrayImage = Union[NDFloat32GrayImage, NDFloat64GrayImage]
 NDGrayImage = Union[NDByteGrayImage, NDFloatGrayImage]
 
-NDBoolMask = NDArray[(Any, Any), bool]
-NDBoolMaskBatch = NDArray[(Any, Any, Any), bool]
+NDBoolMask = NDArray[Shape["*, *"], numpy.bool8]
+NDBoolMaskBatch = NDArray[Shape["*, *, *"], numpy.bool8]
 
-NDIntMask2d = NDArray[(Any, Any), int]
-NDIntMask3d = NDArray[(Any, Any, Any), int]
-NDIntMask4d = NDArray[(Any, Any, Any, Any), int]
-
-NDByteImageBatch = NDArray[(Any, Any, Any, 3), numpy.uint8]
-NDFloat32ImageBatch = NDArray[(Any, Any, Any, 3), numpy.float32]
-NDFloat64ImageBatch = NDArray[(Any, Any, Any, 3), numpy.float64]
+NDIntMask2d = NDArray[Shape["*, *"], numpy.int32]
+NDIntMask3d = NDArray[Shape["*, *, *"], numpy.int32]
+NDIntMask4d = NDArray[Shape["*, *, *, *"], numpy.int32]
+
+NDByteImageBatch = NDArray[Shape["*, *, *, 3"], numpy.uint8]
+NDFloat32ImageBatch = NDArray[Shape["*, *, *, 3"], numpy.float32]
+NDFloat64ImageBatch = NDArray[Shape["*, *, *, 3"], numpy.float64]
 NDFloatImageBatch = Union[NDFloat32ImageBatch, NDFloat64ImageBatch]
 NDImageBatch = Union[NDByteImageBatch, NDFloatImageBatch]
 
 RefDataSet = Tuple[List, List]
 SplitDataSet = Dict[Union[int, str], RefDataSet]
 DataSet = Union[RefDataSet, SplitDataSet]
```

### Comparing `pathaia-0.2.1/pathaia.egg-info/PKG-INFO` & `pathaia-0.2.2/pathaia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pathaia
-Version: 0.2.1
+Version: 0.2.2
 Summary: procedures for wsi analysis
 Author: Arnaud Abreu
 Author-email: arnaud.abreu.p@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 # PathAIA
 
@@ -134,9 +132,7 @@
   title={PathAIA},
   author={Abreu, A and .al},
   journal={GitHub. Note: https://github.com/ArnaudAbreu/PathAIA},
   volume={3},
   year={2021}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: pathaia Version: 0.2.1 Summary: procedures for wsi
-analysis Author: Arnaud Abreu Author-email: arnaud.abreu.p@gmail.com License:
-UNKNOWN Platform: UNKNOWN Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: pathaia Version: 0.2.2 Summary: procedures for wsi
+analysis Author: Arnaud Abreu Author-email: arnaud.abreu.p@gmail.com
+Description-Content-Type: text/markdown License-File: LICENSE
           # PathAIA **Simple digital pathology analysis tools.** ---
      Basic_Usage â¢ Advanced_features â¢ Docs â¢ Community â¢ License
    [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pathaia)]
  (https://pypi.org/project/pathaia/) [![PyPI Status](https://badge.fury.io/py/
    pathaia.svg)](https://badge.fury.io/py/pathaia) [![PyPI Status](https://
 pepy.tech/badge/pathaia)](https://pepy.tech/project/pathaia) [![codecov](https:
            //codecov.io/gh/ArnaudAbreu/PathAIA/branch/master/graph/
```

### Comparing `pathaia-0.2.1/pathaia.egg-info/SOURCES.txt` & `pathaia-0.2.2/pathaia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/setup.py` & `pathaia-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from setuptools import setup, find_packages
 # read the contents of your README file
 from os import path
+
+from setuptools import find_packages, setup
+
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="pathaia",
-    version="0.2.1",
+    version="0.2.2",
     description="procedures for wsi analysis",
     author="Arnaud Abreu",
     author_email="arnaud.abreu.p@gmail.com",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
-        "fastcore",
-        "numpy",
-        "tqdm",
-        "openslide-python",
-        "opencv-python",
-        "scikit-image",
-        "matplotlib",
-        "nptyping",
-        "pandas",
+        "fastcore>=1,<2",
+        "numpy>=1,<2",
+        "tqdm>=4,<5",
+        "openslide-python>=3,<4",
+        "opencv-python>=4,<5",
+        "scikit-image>=0.19,<1",
+        "matplotlib>=3,<4",
+        "nptyping>=2,<3",
+        "pandas>=1,<2",
         "dataclasses",
-        "sortedcontainers",
-        "ordered-set",
-		"shapely",
-		"scikit-learn"
+        "sortedcontainers>=2,<3",
+        "ordered-set>=4,<5",
+        "shapely>=1,<2",
+        "scikit-learn>=1,<2",
     ],
     include_package_data=True,
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type="text/markdown",
 )
```

### Comparing `pathaia-0.2.1/tests/data.py` & `pathaia-0.2.2/tests/data.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.1/tests/helpers.py` & `pathaia-0.2.2/tests/helpers.py`

 * *Files identical despite different names*

