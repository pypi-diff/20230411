# Comparing `tmp/natml-0.0.6.tar.gz` & `tmp/natml-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natml-0.0.6.tar", last modified: Sat Mar 18 19:11:52 2023, max compression
+gzip compressed data, was "natml-0.0.7.tar", last modified: Tue Apr 11 15:21:31 2023, max compression
```

## Comparing `natml-0.0.6.tar` & `natml-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:11:52.532034 natml-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-18 19:11:38.000000 natml-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-18 19:11:52.532034 natml-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-18 19:11:38.000000 natml-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:11:52.528034 natml-0.0.6/natml/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-18 19:11:38.000000 natml-0.0.6/natml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:11:52.532034 natml-0.0.6/natml/api/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-18 19:11:38.000000 natml-0.0.6/natml/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:11:52.532034 natml-0.0.6/natml/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-18 19:11:38.000000 natml-0.0.6/natml/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-18 19:11:38.000000 natml-0.0.6/natml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:11:52.528034 natml-0.0.6/natml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-18 19:11:52.000000 natml-0.0.6/natml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-18 19:11:52.000000 natml-0.0.6/natml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 19:11:52.000000 natml-0.0.6/natml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-18 19:11:52.000000 natml-0.0.6/natml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-18 19:11:52.000000 natml-0.0.6/natml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-18 19:11:52.000000 natml-0.0.6/natml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 19:11:52.532034 natml-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-18 19:11:38.000000 natml-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:21:31.490547 natml-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-11 15:21:18.000000 natml-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-11 15:21:31.490547 natml-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 15:21:18.000000 natml-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:21:31.486547 natml-0.0.7/natml/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-11 15:21:18.000000 natml-0.0.7/natml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:21:31.486547 natml-0.0.7/natml/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-11 15:21:18.000000 natml-0.0.7/natml/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:21:31.486547 natml-0.0.7/natml/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-11 15:21:18.000000 natml-0.0.7/natml/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 15:21:18.000000 natml-0.0.7/natml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:21:31.486547 natml-0.0.7/natml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-11 15:21:31.000000 natml-0.0.7/natml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 15:21:31.000000 natml-0.0.7/natml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:21:31.000000 natml-0.0.7/natml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 15:21:31.000000 natml-0.0.7/natml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 15:21:31.000000 natml-0.0.7/natml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 15:21:31.000000 natml-0.0.7/natml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:21:31.490547 natml-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-11 15:21:18.000000 natml-0.0.7/setup.py
```

### Comparing `natml-0.0.6/LICENSE` & `natml-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `natml-0.0.6/PKG-INFO` & `natml-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: natml
-Version: 0.0.6
+Version: 0.0.7
 Summary: Zero deployment machine learning.
 Home-page: https://natml.ai
 Author: NatML Inc.
 Author-email: hi@natml.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.natml.ai/python
-Project-URL: Source, https://github.com/natmlx/NatML-Py
+Project-URL: Source, https://github.com/natmlx/natml-py
 Description: # NatML
         
         ![NatML](https://raw.githubusercontent.com/natsuite/NatML/main/.media/wall.png)
         
         Zero deployment machine learning.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `natml-0.0.6/natml/api/__init__.py` & `natml-0.0.7/natml/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 from .graph import Graph, GraphFormat, GraphStatus
 from .license import License
 from .normalization import Normalization
 from .prediction import PredictionSession, FeatureInput
 from .predictor import Predictor, PredictorStatus, AccessMode, AspectMode
 from .profile import Profile
 from .session import PredictorSession
-from .upload import UploadType, create_upload_url
+from .upload import Storage, UploadType
 from .user import User
```

### Comparing `natml-0.0.6/natml/api/api.py` & `natml-0.0.7/natml/api/api.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.6/natml/api/endpoint.py` & `natml-0.0.7/natml/api/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from enum import Enum
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 from .api import query
 from .dtype import Dtype
 from .tag import Tag, parse_tag, serialize_tag
-from .upload import UploadType, upload_file
+from .upload import Storage, UploadType
 
 class EndpointType (str, Enum):
     """
     Endpoint type.
     """
     Serverless = "SERVERLESS"
     Dedicated = "DEDICATED"
@@ -218,15 +218,15 @@
             acceleration (EndpointAcceleration): Endpoint acceleration.
             access_key (str): NatML access key.
 
         Returns:
             Endpoint: Created endpoint.
         """
         # Upload notebook
-        url = upload_file(notebook, UploadType.Notebook, check_extension=True) if isinstance(notebook, Path) else notebook
+        url = Storage.upload(notebook, UploadType.Notebook, check_extension=True) if isinstance(notebook, Path) else notebook
         # Query
         response = query(f"""
             mutation ($input: CreateEndpointInput!) {{
                 createEndpoint (input: $input) {{
                     variant
                     url
                     type
```

### Comparing `natml-0.0.6/natml/api/graph.py` & `natml-0.0.7/natml/api/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import List, Union
 
 from .api import query
 from .tag import Tag, parse_tag, serialize_tag
-from .upload import UploadType, upload_file
+from .upload import Storage, UploadType
 
 class GraphFormat (str, Enum):
     """
     Graph format.
     """
     CoreML = "COREML"
     ONNX = "ONNX"
@@ -136,15 +136,15 @@
             format (GraphFormat): Target graph format.
             access_key (str): NatML access key.
 
         Returns:
             Graph: Created graph.
         """
         # Upload graph
-        url = upload_file(graph, UploadType.Graph, check_extension=True) if isinstance(graph, Path) else graph
+        url = Storage.upload(graph, UploadType.Graph, check_extension=True) if isinstance(graph, Path) else graph
         # Query
         response = query(f"""
             mutation ($input: CreateGraphInput!) {{
                 createGraph (input: $input) {{
                     variant
                     format
                     status
```

### Comparing `natml-0.0.6/natml/api/license.py` & `natml-0.0.7/natml/api/license.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.6/natml/api/prediction.py` & `natml-0.0.7/natml/api/prediction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,101 @@
 # 
 #   NatML
 #   Copyright © 2023 NatML Inc. All Rights Reserved.
 #
 
 from __future__ import annotations
 from base64 import b64encode
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from io import BytesIO
+from numpy import frombuffer, ndarray
 from PIL import Image
-from typing import Optional, List
+from requests import get
+from typing import List, Optional, Union
+from urllib.request import urlopen
 
 from .api import query
 from .dtype import Dtype
 from .feature import Feature
 
 @dataclass
 class FeatureInput:
     """
-    Prediction feature input.
+    Prediction input feature.
 
     Members:
         name (str): Feature name. This MUST match the input parameter name defined by the predictor endpoint.
         data (str): Feature data URL. This can be a web URL or a data URL.
         type (Dtype): Feature data type.
         shape (list): Feature shape. This MUST be provided for array features.
     """
     name: str
-    data: str
-    type: Dtype
+    data: str = None
+    type: Dtype = None
     shape: Optional[List[int]] = None
+    stringValue: str = None
+    floatValue: float = None
+    floatArray: List[float] = None
+    intValue: int = None
+    intArray: List[int] = None
+    boolValue: bool = None
+    listValue: list = None
+    dictValue: dict = None
+
+    @classmethod
+    def from_value (
+        cls,
+        value: Union[ndarray, str, float, int, bool, list, dict, Image.Image],
+        name: str
+    ) -> FeatureInput:
+        """
+        Create a feature input from a given value.
+        
+        Parameters:
+            value (any): Value.
+            name (str): Feature name.
+
+        Returns:
+            FeatureInput: Feature input.
+        """
+        # Array
+        if isinstance(value, ndarray):
+            encoded_data = b64encode(value).decode("ascii")
+            data = f"data:application/octet-stream;base64,{encoded_data}"
+            return FeatureInput(name, data, value.dtype.name, list(value.shape))
+        # String
+        if isinstance(value, str):
+            return FeatureInput(name, stringValue=value)
+        # Float
+        if isinstance(value, float):
+            return FeatureInput(name, floatValue=value)
+        # Boolean
+        if isinstance(value, bool):
+            return FeatureInput(name, boolValue=value)
+        # Integer
+        if isinstance(value, int):
+            return FeatureInput(name, intValue=value)
+        # List
+        if isinstance(value, list):
+            return FeatureInput(name, listValue=value)
+        # Dict
+        if isinstance(value, dict):
+            return FeatureInput(name, dictValue=value)
+        # Image
+        if isinstance(value, Image.Image):
+            image_buffer = BytesIO()
+            channels = { "L": 1, "RGB": 3, "RGBA": 4 }[value.mode]
+            format = "PNG" if value.mode == "RGBA" else "JPEG"
+            value.save(image_buffer, format=format)
+            encoded_data = b64encode(image_buffer.getvalue()).decode("ascii")
+            data = f"data:{value.get_format_mimetype()};base64,{encoded_data}"
+            shape = [1, value.height, value.width, channels]
+            return FeatureInput(name, data, Dtype.image, shape)
+        # Unsupported
+        raise RuntimeError(f"Cannot create input feature for value {value} of type {type(value)}")
 
 @dataclass
 class PredictionSession:
     """
     Predictor endpoint session.
 
     Members:
@@ -47,43 +110,41 @@
     id: str
     created: str
     results: List[Feature]
     latency: float
     error: str
     logs: str
 
-    def __post_init__ (self):
-        self.results = [Feature(**feature) if isinstance(feature, dict) else feature for feature in self.results]
-
     @classmethod
     def create (
         cls,
         tag: str,
         *features: List[FeatureInput],
-        parse_outputs: bool=True,
+        raw_outputs: bool=False,
         access_key: str=None,
         **inputs,
     ) -> PredictionSession:
         """
         Create an endpoint prediction session.
 
         Parameters:
             tag (str): Endpoint tag.
             features (list): Input features.
-            parse_outputs (bool): Parse output features into Pythonic data types.
+            raw_outputs (bool): Skip parsing output features into Pythonic data types.
             access_key (str): NatML access key.
             inputs (dict): Input features.
 
         Returns:
             PredictionSession: Prediction session.
         """
         # Collect input features
-        input_features = list(features) + [_create_input_feature(key, value) for key, value in inputs.items()]
-        parsed_fields = "\n".join(_FEATURE_KEYS) if parse_outputs else ""
+        input_features = list(features) + [FeatureInput.from_value(value, name) for name, value in inputs.items()]
+        input_features = [asdict(feature) for feature in input_features]
         # Query
+        parsed_fields = "" if raw_outputs else "\n".join(_FEATURE_KEYS)
         response = query(f"""
             mutation ($input: CreatePredictionSessionInput!) {{
                 createPredictionSession (input: $input) {{
                     id
                     created
                     results {{
                         data
@@ -92,54 +153,61 @@
                         {parsed_fields}
                     }}
                     latency
                     error
                     logs
                 }}
             }}""",
-            { "tag": tag, "inputs": input_features },
+            { "tag": tag, "inputs": input_features, "client": "python" },
             access_key=access_key
         )
         # Check session
         session = response["createPredictionSession"]
         if not session:
             return None
         # Parse outputs
-        session["results"] = [_parse_output_feature(feature) for feature in session["results"]] if session["results"] else None
+
+        
+
+        session["results"] = [_parse_output_feature(feature) for feature in session["results"]] if session["results"] and not raw_outputs else session["results"]
         session = PredictionSession(**session)
+
+        print(session)
+
         # Return
         return session
-    
-def _create_input_feature (key: str, value):
-    # Float
-    if isinstance(value, float):
-        return { "name": key, "floatValue": value }
-    # Boolean
-    if isinstance(value, bool):
-        return { "name": key, "boolValue": value }
-    # Integer
-    if isinstance(value, int):
-        return { "name": key, "intValue": value }
-    # String
-    if isinstance(value, str):
-        return { "name": key, "stringValue": value }
-    # Image
-    if isinstance(value, Image.Image):
-        image_buffer = BytesIO()
-        channels = { "L": 1, "RGB": 3, "RGBA": 4 }[value.mode]
-        format = "PNG" if value.mode == "RGBA" else "JPEG"
-        value.save(image_buffer, format=format)
-        encoded_data = b64encode(image_buffer.getvalue()).decode("ascii")
-        return {
-            "name": key,
-            "data": f"data:{value.get_format_mimetype()};base64,{encoded_data}",
-            "type": "image",
-            "shape": [1, value.height, value.width, channels]
-        }
-    # Unsupported
-    raise RuntimeError(f"Cannot create input feature for value {value} of type {type(value)}")
 
-def _parse_output_feature (feature: dict):
+def _parse_output_feature (feature: dict) -> Union[Feature, str, float, int, bool, Image.Image, list, dict]:
+    data, type, shape = feature["data"], feature["type"], feature["shape"]
+    # Handle image
+    if type == Dtype.image:
+        return Image.open(_download_feature_data(data))
+    # Handle non-numeric scalars
     values = [feature.get(key, None) for key in _FEATURE_KEYS]
-    return next((value for value in values if value), feature)
+    scalar = next((value for value in values if value is not None), None)
+    if scalar is not None:
+        return scalar
+    # Handle ndarray
+    ARRAY_TYPES = [
+        Dtype.int8, Dtype.int16, Dtype.int32, Dtype.int64,
+        Dtype.uint8, Dtype.uint16, Dtype.uint32, Dtype.uint64,
+        Dtype.float16, Dtype.float32, Dtype.float64, Dtype.bool
+    ]
+    if type in ARRAY_TYPES:
+        # Create array
+        array = frombuffer(_download_feature_data(data).getbuffer(), dtype=type).reshape(shape)
+        return array if len(shape) > 0 else array.item()
+    # Handle generic feature
+    feature = Feature(**feature)
+    return feature
+
+def _download_feature_data (url: str) -> BytesIO:
+    # Check if data URL
+    if url.startswith("data:"):
+        with urlopen(url) as response:
+            return BytesIO(response.read())
+    # Download
+    response = get(url)
+    result = BytesIO(response.content)
+    return result
 
-_FEATURE_KEYS = ["stringValue", "floatValue", "floatArray", "intValue", "intArray", "boolValue", "boolArray"]
+_FEATURE_KEYS = ["stringValue", "listValue", "dictValue"]
```

### Comparing `natml-0.0.6/natml/api/predictor.py` & `natml-0.0.7/natml/api/predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import List, Optional, Union
 
 from .api import query
 from .audio import AudioFormat
 from .license import License
 from .normalization import Normalization
 from .profile import Profile
-from .upload import UploadType, upload_file
+from .upload import Storage, UploadType
 
 class AccessMode (str, Enum):
     """
     Predictor access mode.
     """
     Public = "PUBLIC"
     Private = "PRIVATE"
@@ -347,15 +347,15 @@
             delete_audio_format (bool): Delete existing audio format.
             access_key (str): NatML access key.
 
         Returns:
             Predictor: Updated predictor.
         """
         # Upload media
-        media = upload_file(media, UploadType.Media, check_extension=True) if isinstance(media, Path) else media
+        media = Storage.upload(media, UploadType.Media, check_extension=True) if isinstance(media, Path) else media
         # Gather inputs
         preserve_keys = [k for k, v in {
             "media": delete_media,
             "labels": delete_labels,
             "normalization": delete_normalization,
             "aspectMode": delete_aspect_mode,
             "audioFormat": delete_audio_format
@@ -442,14 +442,43 @@
             access_key=access_key
         )
         # Return
         result = response["deletePredictor"]
         return result
 
     @classmethod
+    def review (
+        cls,
+        tag: str,
+        access_key: str=None  
+    ) -> List[str]:
+        """
+        Review a draft predictor for any issues that might prevent it from being published.
+
+        Parameters:
+            tag (str): Predictor tag.
+            access_key (str): NatML access key.
+
+        Returns:
+            list: Issues that might prevent the predictor from being published. Empty array means no issues were found.
+        """
+        # Query
+        response = query(f"""
+            mutation ($input: ReviewPredictorInput!) {{
+                reviewPredictor (input: $input)
+            }}
+            """,
+            { "tag": tag },
+            access_key=access_key
+        )
+        # Return
+        result = response["reviewPredictor"]
+        return result
+
+    @classmethod
     def publish (
         cls,
         tag: str,
         access_key: str=None
     ) -> Predictor:
         """
         Publish a draft predictor.
```

### Comparing `natml-0.0.6/natml/api/profile.py` & `natml-0.0.7/natml/api/profile.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.6/natml/api/session.py` & `natml-0.0.7/natml/api/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
                             username
                         }}
                         name
                         description
                         status
                         access
                         license
+                        labels
                         normalization {{
                             mean
                             std
                         }}
                         aspect_mode: aspectMode
                         audio_format: audioFormat {{
                             sample_rate: sampleRate
@@ -82,15 +83,15 @@
                     format
                     flags
                     fingerprint
                     created
                 }}
             }}
             """,
-            { "tag": tag, "format": format },
+            { "tag": tag, "format": format, "client": "python" },
             access_key=access_key
         )
         # Create session
         session = response["createPredictorSession"]
         session = PredictorSession(**session)
         # Return
         return session
```

### Comparing `natml-0.0.6/natml/api/tag.py` & `natml-0.0.7/natml/api/tag.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.6/natml/api/upload.py` & `natml-0.0.7/natml/api/upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,104 @@
 # 
 #   NatML
 #   Copyright © 2023 NatML Inc. All Rights Reserved.
 #
 
 from enum import Enum
+from io import BytesIO
 from mimetypes import guess_type
 from pathlib import Path
 from requests import put
+from typing import Union
 
 from .api import query
 
 class UploadType (str, Enum):
     """
     Upload URL type.
     """
     Demo = "DEMO"
     Feature = "FEATURE"
     Graph = "GRAPH"
     Media = "MEDIA"
     Notebook = "NOTEBOOK"
 
-def create_upload_url (type: UploadType, name: str, key: str=None) -> str:
+class Storage:
     """
-    Create an upload URL.
-
-    Parameters:
-        type (UploadType): Upload type.
-        name (str): File name.
-        key (str): File key. This is useful for grouping related files.
-
-    Returns:
-        str: File upload URL.
-    """
-    response = query(f"""
-        mutation ($input: CreateUploadURLInput!) {{
-            createUploadURL (input: $input)
-        }}
-        """,
-        { "type": type, "name": name, "key": key }
-    )
-    url = response["createUploadURL"]
-    return url
-
-def upload_file (path: Path, type: UploadType, key: str=None, check_extension: bool=True) -> str:
+    Upload and download files.
     """
-    Upload a file and return the URL.
-
-    Parameters:
-        path (Path): File path.
-        type (UploadType): File type.
-        key (str): File key. This is useful for grouping related files.
-        check_extension (bool): Validate file extensions before uploading.
 
-    Returns:
-        str: Upload URL.
-    """
-    EXTENSIONS = {
-        UploadType.Demo: [".data", ".js"],
-        UploadType.Feature: [],
-        UploadType.Graph: [".mlmodel", ".onnx", ".tflite"],
-        UploadType.Media: [".jpg", ".jpeg", ".png", ".gif"],
-        UploadType.Notebook: [".ipynb"],
-    }
-    # Check path
-    if not path.exists():
-        raise RuntimeError(f"Cannot upload {path.name} because the file does not exist")
-    # Check file
-    if not path.is_file():
-        raise RuntimeError(f"Cannot upload {path.name} becaause it does not point to a file")
-    # Check extension
-    if check_extension and path.suffix not in EXTENSIONS[type]:
-        raise RuntimeError(f"Cannot upload {path.name} because it is not a valid {type.name.lower()} file")
-    # Get upload URL
-    mime = guess_type(path, strict=False)[0] or "application/binary"
-    url = create_upload_url(type, path.name, key=key)
-    with open(path, "rb") as f:
-        put(url, data=f, headers={ "Content-Type": mime }).raise_for_status()
-    # Return
-    return url
+    @classmethod
+    def create_upload_url (
+        cls,
+        name: str,
+        type: UploadType,
+        key: str=None
+    ) -> str:
+        """
+        Create an upload URL.
+
+        Parameters:
+            name (str): File name.
+            type (UploadType): Upload type.
+            key (str): File key. This is useful for grouping related files.
+
+        Returns:
+            str: File upload URL.
+        """
+        response = query(f"""
+            mutation ($input: CreateUploadURLInput!) {{
+                createUploadURL (input: $input)
+            }}
+            """,
+            { "type": type, "name": name, "key": key }
+        )
+        url = response["createUploadURL"]
+        return url
+
+    @classmethod
+    def upload ( # INCOMPLETE
+        cls,
+        file: Union[str, Path, BytesIO, bytes],
+        type: UploadType,
+        name: str=None,
+        key: str=None,
+        min_upload_size: int=0,
+        check_extension: bool=True
+    ) -> str:
+        """
+        Upload a file and return the URL.
+
+        Parameters:
+            file (str | Path | BytesIO | bytes): File path.
+            type (UploadType): File type.
+            name (str): File name. This MUST be provided if `file` is not a file path.
+            key (str): File key. This is useful for grouping related files.
+            min_upload_size (int): Minimum file size for file to be uploaded. Files smaller than this limit will be returned as data URLs.
+            check_extension (bool): Validate file extensions before uploading.
+
+        Returns:
+            str: Upload URL.
+        """
+        EXTENSIONS = {
+            UploadType.Demo: [".data", ".js"],
+            UploadType.Feature: [],
+            UploadType.Graph: [".mlmodel", ".onnx", ".tflite"],
+            UploadType.Media: [".jpg", ".jpeg", ".png", ".gif"],
+            UploadType.Notebook: [".ipynb"],
+        }
+        # Check path
+        if not file.exists():
+            raise RuntimeError(f"Cannot upload {file.name} because the file does not exist")
+        # Check file
+        if not file.is_file():
+            raise RuntimeError(f"Cannot upload {file.name} becaause it does not point to a file")
+        # Check extension
+        if check_extension and file.suffix not in EXTENSIONS[type]:
+            raise RuntimeError(f"Cannot upload {file.name} because it is not a valid {type.name.lower()} file")
+        # Get upload URL
+        mime = guess_type(file, strict=False)[0] or "application/octet-stream"
+        url = cls.create_upload_url(file.name, type, key=key)
+        with open(file, "rb") as f:
+            put(url, data=f, headers={ "Content-Type": mime }).raise_for_status()
+        # Return
+        return url
```

### Comparing `natml-0.0.6/natml/api/user.py` & `natml-0.0.7/natml/api/user.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.6/natml/cli/__init__.py` & `natml-0.0.7/natml/cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,43 +2,45 @@
 #   NatML
 #   Copyright © 2023 NatML Inc. All Rights Reserved.
 #
 
 from typer import Typer
 
 from .auth import app as auth_app
+from .demos import app as demos_app
 from .endpoints import app as endpoints_app
 from .graphs import app as graphs_app
-from .misc import main_cli_options
+from .misc import cli_options
 from .predict import predict
 from .predictors import app as predictors_app
 from .users import app as users_app
 from ..version import __version__
 
 # Define CLI
 app = Typer(
     name=f"NatML CLI {__version__}",
     no_args_is_help=True,
     pretty_exceptions_show_locals=False,
     pretty_exceptions_short=True,
 )
 
 # Add top level options
-app.callback()(main_cli_options)
+app.callback()(cli_options)
 
 # Add subcommands
 app.add_typer(auth_app, name="auth", help="Login, logout, and perform other authentication tasks.")
 app.add_typer(predictors_app, name="predictors", help="Manage predictors.")
 app.add_typer(graphs_app, name="graphs", help="Manage predictor graphs.")
 app.add_typer(endpoints_app, name="endpoints", help="Manage predictor endpoints.")
 app.add_typer(users_app, name="users", help="Manage users.")
+app.add_typer(demos_app, name="demos", help="Manage predictor demos.")
 
 # Add top-level commands
 app.command(
     name="predict",
     context_settings={ "allow_extra_args": True, "ignore_unknown_options": True },
-    help="Make a prediction with a predictor endpoint."
+    help="Make a prediction with a predictor."
 )(predict)
 
 # Run
 if __name__ == "__main__":
     app()
```

### Comparing `natml-0.0.6/natml/cli/auth.py` & `natml-0.0.7/natml/cli/auth.py`

 * *Files identical despite different names*

### Comparing `natml-0.0.6/natml/cli/graphs.py` & `natml-0.0.7/natml/cli/graphs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 #   NatML
 #   Copyright © 2023 NatML Inc. All Rights Reserved.
 #
 
 from dataclasses import asdict
 from pathlib import Path
 from rich import print_json
-from typer import Argument, Typer
+from typer import Argument, Context, Option, Typer
 
-from .auth import get_access_key
 from ..api import Graph, GraphFormat, PredictorSession
+from .auth import get_access_key
+from .misc import create_learn_callback
 
 app = Typer(no_args_is_help=True)
 
 @app.command(name="retrieve", help="Retrieve a predictor graph.")
 def retrieve_graph (
     tag: str=Argument(..., help="Graph tag. If the tag does not contain a variant then the variant defaults to `main`."),
     format: GraphFormat=Argument(..., case_sensitive=False, help="Graph format.")
@@ -44,15 +45,24 @@
 def delete_graph (
     tag: str=Argument(..., help="Graph tag. If the tag does not contain a variant then the variant defaults to `main`."),
     format: GraphFormat=Argument(..., case_sensitive=False, help="Graph format.")
 ) -> None:
     result = Graph.delete(tag, format, access_key=get_access_key())
     print_json(data=result)
 
-@app.command(name="predict", help="Create a graph prediction session.")
-def create_predictor_session (
-    tag: str=Argument(..., help="Graph tag. If the tag does not contain a variant then the variant defaults to `main`."),
-    format: GraphFormat=Argument(..., case_sensitive=False, help="Graph format.")
+@app.command(
+    name="predict",
+    context_settings={ "allow_extra_args": True, "ignore_unknown_options": True },
+    help="Make a prediction with a predictor graph."
+)
+def predict ( # INCOMPLETE
+    tag: str = Argument(..., help="Predictor tag."),
+    raw_outputs: bool = Option(False, "--raw-outputs", help="Generate raw output features instead of parsing."),
+    context: Context = 0
 ) -> None:
-    session = PredictorSession.create(tag, format, access_key=get_access_key())
-    session = asdict(session)
-    print_json(data=session)
+    pass
+
+@app.callback()
+def graph_options (
+    learn: bool = Option(None, "--learn", callback=create_learn_callback("https://docs.natml.ai/graph/graphs/type"), help="Learn about predictor graphs in NatML.")
+):
+    pass
```

### Comparing `natml-0.0.6/natml/cli/predictors.py` & `natml-0.0.7/natml/cli/predictors.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 #
 
 from dataclasses import asdict
 from rich import print_json
 from typer import Argument, Option, Typer
 from typing import List, Tuple
 
-from .auth import get_access_key
 from ..api import AccessMode, AspectMode, AudioFormat, License, Normalization, Predictor, PredictorStatus
+from .auth import get_access_key
+from .misc import create_learn_callback
 
 app = Typer(no_args_is_help=True)
 
 @app.command(name="retrieve", help="Retrieve a predictor.")
 def retrieve_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ) -> None:
@@ -95,27 +96,40 @@
         delete_normalization=delete_normalization,
         delete_aspect_mode=delete_aspect_mode,
         delete_audio_format=delete_audio_format,
         access_key=get_access_key()
     )
     print_json(data=asdict(predictor))
 
-@app.command(name="delete", help="Delete a predictor.")
+@app.command(name="delete", help="Delete a draft predictor.")
 def delete_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ) -> None:
     result = Predictor.delete(tag, access_key=get_access_key())
     print_json(data=result)
 
-@app.command(name="publish", help="Publish a predictor.")
+@app.command(name="review", help="Review a draft predictor for any issues that might prevent it from being published.")
+def review_predictor (
+    tag: str=Argument(..., help="Predictor tag.")
+) -> None:
+    result = Predictor.review(tag, access_key=get_access_key())
+    print_json(data=result)
+
+@app.command(name="publish", help="Publish a draft predictor.")
 def publish_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ) -> None:
     predictor = Predictor.publish(tag, access_key=get_access_key())
     print_json(data=asdict(predictor))
 
-@app.command(name="archive", help="Archive a predictor.")
+@app.command(name="archive", help="Archive a published predictor.")
 def archive_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ) -> None:
     predictor = Predictor.archive(tag, access_key=get_access_key())
-    print_json(data=asdict(predictor))
+    print_json(data=asdict(predictor))
+
+@app.callback()
+def predictor_options (
+    learn: bool = Option(None, "--learn", callback=create_learn_callback("https://docs.natml.ai/graph/predictors/type"), help="Learn about predictors in NatML.")
+):
+    pass
```

### Comparing `natml-0.0.6/natml.egg-info/PKG-INFO` & `natml-0.0.7/natml.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: natml
-Version: 0.0.6
+Version: 0.0.7
 Summary: Zero deployment machine learning.
 Home-page: https://natml.ai
 Author: NatML Inc.
 Author-email: hi@natml.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.natml.ai/python
-Project-URL: Source, https://github.com/natmlx/NatML-Py
+Project-URL: Source, https://github.com/natmlx/natml-py
 Description: # NatML
         
         ![NatML](https://raw.githubusercontent.com/natsuite/NatML/main/.media/wall.png)
         
         Zero deployment machine learning.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `natml-0.0.6/natml.egg-info/SOURCES.txt` & `natml-0.0.7/natml.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 natml/api/profile.py
 natml/api/session.py
 natml/api/tag.py
 natml/api/upload.py
 natml/api/user.py
 natml/cli/__init__.py
 natml/cli/auth.py
+natml/cli/demos.py
 natml/cli/endpoints.py
 natml/cli/graphs.py
 natml/cli/misc.py
 natml/cli/predict.py
 natml/cli/predictors.py
 natml/cli/users.py
```

### Comparing `natml-0.0.6/setup.py` & `natml-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     author_email="hi@natml.ai",
     description="Zero deployment machine learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
 	python_requires=">=3.7",
     install_requires=[
+        "filetype",
+        "numpy",
         "Pillow",
         "requests",
         "rich",
         "typer"
     ],
     url="https://natml.ai",
     packages=find_packages(
@@ -47,10 +49,10 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Topic :: Software Development :: Libraries",
     ],
     project_urls={
         "Documentation": "https://docs.natml.ai/python",
-        "Source": "https://github.com/natmlx/NatML-Py"
+        "Source": "https://github.com/natmlx/natml-py"
     },
 )
```

