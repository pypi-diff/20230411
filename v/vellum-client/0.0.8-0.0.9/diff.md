# Comparing `tmp/vellum-client-0.0.8.tar.gz` & `tmp/vellum-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vellum-client-0.0.8.tar", last modified: Sun Mar 12 00:31:57 2023, max compression
+gzip compressed data, was "dist/vellum-client-0.0.9.tar", last modified: Tue Mar 14 03:47:24 2023, max compression
```

## Comparing `vellum-client-0.0.8.tar` & `vellum-client-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-12 00:31:57.000000 vellum-client-0.0.8/
--rw-r--r--   0 noaflaherty   (501) staff       (20)     1082 2023-02-01 23:37:57.000000 vellum-client-0.0.8/LICENSE
--rw-r--r--   0 noaflaherty   (501) staff       (20)      260 2023-03-12 00:31:57.000000 vellum-client-0.0.8/PKG-INFO
--rw-r--r--   0 noaflaherty   (501) staff       (20)     2091 2023-03-09 19:11:43.000000 vellum-client-0.0.8/README.md
--rw-r--r--   0 noaflaherty   (501) staff       (20)      102 2023-02-01 23:37:57.000000 vellum-client-0.0.8/pyproject.toml
--rw-r--r--   0 noaflaherty   (501) staff       (20)      928 2023-03-12 00:31:57.000000 vellum-client-0.0.8/setup.cfg
--rw-r--r--   0 noaflaherty   (501) staff       (20)      458 2023-03-12 00:29:15.000000 vellum-client-0.0.8/setup.py
-drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum/
--rw-r--r--   0 noaflaherty   (501) staff       (20)      503 2023-03-12 00:31:15.000000 vellum-client-0.0.8/vellum/__init__.py
-drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum/api_resources/
--rw-r--r--   0 noaflaherty   (501) staff       (20)       65 2023-02-01 23:37:57.000000 vellum-client-0.0.8/vellum/api_resources/__init__.py
-drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum/api_resources/abstract/
--rw-r--r--   0 noaflaherty   (501) staff       (20)        0 2023-02-01 23:37:57.000000 vellum-client-0.0.8/vellum/api_resources/abstract/__init__.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)     1042 2023-02-21 03:50:10.000000 vellum-client-0.0.8/vellum/api_resources/abstract/api_resource.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)      555 2023-02-11 20:48:48.000000 vellum-client-0.0.8/vellum/api_resources/abstract/exceptions.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)      473 2023-02-11 20:48:48.000000 vellum-client-0.0.8/vellum/api_resources/abstract/predict_api_resource.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)     1706 2023-02-11 20:48:48.000000 vellum-client-0.0.8/vellum/api_resources/completion_actuals.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)     1674 2023-02-11 20:48:48.000000 vellum-client-0.0.8/vellum/api_resources/generate.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)     1784 2023-03-12 00:20:24.000000 vellum-client-0.0.8/vellum/api_resources/search.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)     4698 2023-03-12 00:19:11.000000 vellum-client-0.0.8/vellum/api_resources/types.py
--rw-r--r--   0 noaflaherty   (501) staff       (20)        0 2023-02-01 23:37:57.000000 vellum-client-0.0.8/vellum/py.typed
-drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum_client.egg-info/
--rw-r--r--   0 noaflaherty   (501) staff       (20)      260 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum_client.egg-info/PKG-INFO
--rw-r--r--   0 noaflaherty   (501) staff       (20)      626 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum_client.egg-info/SOURCES.txt
--rw-r--r--   0 noaflaherty   (501) staff       (20)        1 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum_client.egg-info/dependency_links.txt
--rw-r--r--   0 noaflaherty   (501) staff       (20)       31 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum_client.egg-info/requires.txt
--rw-r--r--   0 noaflaherty   (501) staff       (20)        7 2023-03-12 00:31:57.000000 vellum-client-0.0.8/vellum_client.egg-info/top_level.txt
+drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-14 03:47:24.000000 vellum-client-0.0.9/
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     1082 2023-02-01 23:37:57.000000 vellum-client-0.0.9/LICENSE
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      260 2023-03-14 03:47:24.000000 vellum-client-0.0.9/PKG-INFO
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     3097 2023-03-14 03:39:52.000000 vellum-client-0.0.9/README.md
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      102 2023-02-01 23:37:57.000000 vellum-client-0.0.9/pyproject.toml
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      928 2023-03-14 03:47:24.000000 vellum-client-0.0.9/setup.cfg
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      458 2023-03-14 03:40:17.000000 vellum-client-0.0.9/setup.py
+drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-14 03:47:24.000000 vellum-client-0.0.9/vellum/
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      664 2023-03-14 03:34:13.000000 vellum-client-0.0.9/vellum/__init__.py
+drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-14 03:47:24.000000 vellum-client-0.0.9/vellum/api_resources/
+-rw-r--r--   0 noaflaherty   (501) staff       (20)       65 2023-02-01 23:37:57.000000 vellum-client-0.0.9/vellum/api_resources/__init__.py
+drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-14 03:47:24.000000 vellum-client-0.0.9/vellum/api_resources/abstract/
+-rw-r--r--   0 noaflaherty   (501) staff       (20)        0 2023-02-01 23:37:57.000000 vellum-client-0.0.9/vellum/api_resources/abstract/__init__.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     1042 2023-03-14 03:32:36.000000 vellum-client-0.0.9/vellum/api_resources/abstract/api_resource.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      690 2023-03-14 03:34:13.000000 vellum-client-0.0.9/vellum/api_resources/abstract/documents_api_resource.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      555 2023-02-11 20:48:48.000000 vellum-client-0.0.9/vellum/api_resources/abstract/exceptions.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      473 2023-02-11 20:48:48.000000 vellum-client-0.0.9/vellum/api_resources/abstract/predict_api_resource.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     1706 2023-02-11 20:48:48.000000 vellum-client-0.0.9/vellum/api_resources/completion_actuals.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     1663 2023-03-14 03:09:32.000000 vellum-client-0.0.9/vellum/api_resources/generate.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     1729 2023-03-14 03:09:28.000000 vellum-client-0.0.9/vellum/api_resources/search.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     4916 2023-03-14 03:34:13.000000 vellum-client-0.0.9/vellum/api_resources/types.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)     1996 2023-03-14 03:36:39.000000 vellum-client-0.0.9/vellum/api_resources/upload_document.py
+-rw-r--r--   0 noaflaherty   (501) staff       (20)        0 2023-02-01 23:37:57.000000 vellum-client-0.0.9/vellum/py.typed
+drwxr-xr-x   0 noaflaherty   (501) staff       (20)        0 2023-03-14 03:47:24.000000 vellum-client-0.0.9/vellum_client.egg-info/
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      260 2023-03-14 03:47:23.000000 vellum-client-0.0.9/vellum_client.egg-info/PKG-INFO
+-rw-r--r--   0 noaflaherty   (501) staff       (20)      722 2023-03-14 03:47:24.000000 vellum-client-0.0.9/vellum_client.egg-info/SOURCES.txt
+-rw-r--r--   0 noaflaherty   (501) staff       (20)        1 2023-03-14 03:47:23.000000 vellum-client-0.0.9/vellum_client.egg-info/dependency_links.txt
+-rw-r--r--   0 noaflaherty   (501) staff       (20)       31 2023-03-14 03:47:23.000000 vellum-client-0.0.9/vellum_client.egg-info/requires.txt
+-rw-r--r--   0 noaflaherty   (501) staff       (20)        7 2023-03-14 03:47:23.000000 vellum-client-0.0.9/vellum_client.egg-info/top_level.txt
```

### Comparing `vellum-client-0.0.8/LICENSE` & `vellum-client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vellum-client-0.0.8/README.md` & `vellum-client-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 ### Submitting Actuals
 Submitting actuals is how you provide feedback to Vellum about the quality of the generated text.
 This feedback can be used to measure model quality and improve it over time.
 
 ```python
 import vellum
 
+vellum.api_key = "<YOUR_API_KEY>"
+
 vellum.SubmitCompletionActuals.run(
     deployment_name="customer-service-demo",
     actuals=[
         vellum.CompletionActual(
             id="<id-returned-from-generate-endpoint>",
             quality=1.0,  # 1.0 is good, 0.0 is bad
             text="Sorry, we do not offer refunds.",
@@ -55,14 +57,44 @@
 ```
 
 **Note:** If you don't want to keep track of the ids that Vellum generates, you can include an externalId key in
 the initial generate request. You can then include this externalId when submitting actuals. If you use this
 approach, be sure that the ids you provide truly are unique, or you may get unexpected results.
 
 
+### Uploading Documents to Search Across
+Documents can be uploaded to Vellum via either the UI or this API. Once uploaded and indexed,
+Vellum's Search allows you to perform semantic searches against them.
+Here is an example of how to upload a document from a local file:
+
+```python
+import vellum
+
+vellum.api_key = "<YOUR_API_KEY>"
+
+
+with open("/path/to/your/file.txt", "rb") as file:
+    result = vellum.UploadDocument.run(
+        # File to upload
+        file=file,
+        # Document label
+        label="Human-friendly label for your document",
+        # Unique name of the index to upload to
+        index_name="<your-index-name>",
+        # Optionally include a unique ID from your system to this document later.
+        #   Useful if you want to perform updates later
+        external_id="<your-index-name>",
+        # Optionally include keywords to associate with the document that can be used in hybrid search
+        keywords=[],
+    )
+    
+print(result)
+```
+
+
 ### Performing a Search
 Vellum's Search allows you to upload documents and then perform semantic searches against them.
 Here is an example of how to perform a search:
 
 ```python
 import vellum
```

### Comparing `vellum-client-0.0.8/setup.cfg` & `vellum-client-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `vellum-client-0.0.8/vellum/api_resources/abstract/api_resource.py` & `vellum-client-0.0.9/vellum/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `vellum-client-0.0.8/vellum/api_resources/abstract/exceptions.py` & `vellum-client-0.0.9/vellum/api_resources/abstract/exceptions.py`

 * *Files identical despite different names*

### Comparing `vellum-client-0.0.8/vellum/api_resources/completion_actuals.py` & `vellum-client-0.0.9/vellum/api_resources/completion_actuals.py`

 * *Files identical despite different names*

### Comparing `vellum-client-0.0.8/vellum/api_resources/generate.py` & `vellum-client-0.0.9/vellum/api_resources/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import asdict
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
 from vellum.api_resources.abstract.predict_api_resource import PredictAPIResource
 from vellum.api_resources.types import GenerateRequest, GenerateResult
 
 
 class Generate(PredictAPIResource):
     api_path = "v1/generate"
```

### Comparing `vellum-client-0.0.8/vellum/api_resources/search.py` & `vellum-client-0.0.9/vellum/api_resources/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import asdict
-from typing import List, Optional
+from typing import Optional
 
 from vellum.api_resources.abstract.predict_api_resource import PredictAPIResource
-from vellum.api_resources.types import CompletionActual, SubmitCompletionActualsResult, SearchOptions, SearchResults
+from vellum.api_resources.types import SearchOptions, SearchResults
 
 
 class Search(PredictAPIResource):
     api_path = "v1/search"
 
     @classmethod
     def run(  # type: ignore
```

### Comparing `vellum-client-0.0.8/vellum/api_resources/types.py` & `vellum-client-0.0.9/vellum/api_resources/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
 
 @dataclass
 class SearchWeights:
     semantic_similarity: float = 0.8
     keywords: float = 0.2
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if sum([self.semantic_similarity, self.keywords]) != 1.0:
             raise ValueError("Weights must sum to 1.0")
 
 
 @dataclass
 class SearchOptions:
     limit: Optional[int] = 3
@@ -161,7 +161,16 @@
 @dataclass
 class SearchResults:
     results: List[SearchResult]
 
     @classmethod
     def from_raw(cls, raw_result: dict) -> SearchResults:
         return dacite.from_dict(data_class=cls, data=raw_result)
+
+
+@dataclass
+class DocumentUploadResult:
+    document_id: str
+
+    @classmethod
+    def from_raw(cls, raw_result: dict) -> DocumentUploadResult:
+        return dacite.from_dict(data_class=cls, data=raw_result)
```

### Comparing `vellum-client-0.0.8/vellum_client.egg-info/SOURCES.txt` & `vellum-client-0.0.9/vellum_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 vellum/__init__.py
 vellum/py.typed
 vellum/api_resources/__init__.py
 vellum/api_resources/completion_actuals.py
 vellum/api_resources/generate.py
 vellum/api_resources/search.py
 vellum/api_resources/types.py
+vellum/api_resources/upload_document.py
 vellum/api_resources/abstract/__init__.py
 vellum/api_resources/abstract/api_resource.py
+vellum/api_resources/abstract/documents_api_resource.py
 vellum/api_resources/abstract/exceptions.py
 vellum/api_resources/abstract/predict_api_resource.py
 vellum_client.egg-info/PKG-INFO
 vellum_client.egg-info/SOURCES.txt
 vellum_client.egg-info/dependency_links.txt
 vellum_client.egg-info/requires.txt
 vellum_client.egg-info/top_level.txt
```

