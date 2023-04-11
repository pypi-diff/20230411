# Comparing `tmp/intelliprove-1.0.0.tar.gz` & `tmp/intelliprove-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelliprove-1.0.0.tar", max compression
+gzip compressed data, was "intelliprove-1.0.1.tar", max compression
```

## Comparing `intelliprove-1.0.0.tar` & `intelliprove-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1686 2023-03-30 15:25:50.658529 intelliprove-1.0.0/README.md
--rw-r--r--   0        0        0      185 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/__init__.py
--rw-r--r--   0        0        0     5147 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/api_service.py
--rw-r--r--   0        0        0      141 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/exceptions/__init__.py
--rw-r--r--   0        0        0      891 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/exceptions/api.py
--rw-r--r--   0        0        0      790 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/exceptions/media.py
--rw-r--r--   0        0        0      261 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/exceptions/uuid.py
--rw-r--r--   0        0        0     3125 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/intelliprove_api.py
--rw-r--r--   0        0        0      214 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/__init__.py
--rw-r--r--   0        0        0      214 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/dataclasses/__init__.py
--rw-r--r--   0        0        0      642 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/dataclasses/biomarkers.py
--rw-r--r--   0        0        0      250 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/dataclasses/quality.py
--rw-r--r--   0        0        0      785 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/dataclasses/settings.py
--rw-r--r--   0        0        0      343 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/enums.py
--rw-r--r--   0        0        0      164 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/responses/__init__.py
--rw-r--r--   0        0        0     1199 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/responses/biomarkers_response.py
--rw-r--r--   0        0        0      652 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/models/responses/quality_response.py
--rw-r--r--   0        0        0       91 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/utils/__init__.py
--rw-r--r--   0        0        0      169 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/utils/identifiers.py
--rw-r--r--   0        0        0     2459 2023-03-30 15:25:50.658529 intelliprove-1.0.0/intelliprove/api/utils/media.py
--rw-r--r--   0        0        0      414 2023-03-30 15:25:50.658529 intelliprove-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 intelliprove-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1686 2023-04-11 08:40:11.152223 intelliprove-1.0.1/README.md
+-rw-r--r--   0        0        0      185 2023-04-11 08:40:11.152223 intelliprove-1.0.1/intelliprove/api/__init__.py
+-rw-r--r--   0        0        0     5147 2023-04-11 08:40:11.152223 intelliprove-1.0.1/intelliprove/api/api_service.py
+-rw-r--r--   0        0        0      141 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/__init__.py
+-rw-r--r--   0        0        0      891 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/api.py
+-rw-r--r--   0        0        0      790 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/media.py
+-rw-r--r--   0        0        0      261 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/uuid.py
+-rw-r--r--   0        0        0     3125 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/intelliprove_api.py
+-rw-r--r--   0        0        0      214 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/__init__.py
+-rw-r--r--   0        0        0      214 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/biomarkers.py
+-rw-r--r--   0        0        0      250 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/quality.py
+-rw-r--r--   0        0        0      785 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/settings.py
+-rw-r--r--   0        0        0      343 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/enums.py
+-rw-r--r--   0        0        0      164 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/responses/__init__.py
+-rw-r--r--   0        0        0     1199 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/responses/biomarkers_response.py
+-rw-r--r--   0        0        0      754 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/responses/quality_response.py
+-rw-r--r--   0        0        0       91 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/utils/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/utils/identifiers.py
+-rw-r--r--   0        0        0     2459 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/utils/media.py
+-rw-r--r--   0        0        0      414 2023-04-11 08:40:11.156224 intelliprove-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 intelliprove-1.0.1/PKG-INFO
```

### Comparing `intelliprove-1.0.0/README.md` & `intelliprove-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/api_service.py` & `intelliprove-1.0.1/intelliprove/api/api_service.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/exceptions/api.py` & `intelliprove-1.0.1/intelliprove/api/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/exceptions/media.py` & `intelliprove-1.0.1/intelliprove/api/exceptions/media.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/intelliprove_api.py` & `intelliprove-1.0.1/intelliprove/api/intelliprove_api.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/models/dataclasses/biomarkers.py` & `intelliprove-1.0.1/intelliprove/api/models/dataclasses/biomarkers.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/models/dataclasses/settings.py` & `intelliprove-1.0.1/intelliprove/api/models/dataclasses/settings.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/models/responses/biomarkers_response.py` & `intelliprove-1.0.1/intelliprove/api/models/responses/biomarkers_response.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/intelliprove/api/models/responses/quality_response.py` & `intelliprove-1.0.1/intelliprove/api/models/responses/quality_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     error_type: QualityErrorType
     message: str
     signature: Optional[str] = None
 
     @classmethod
     def from_json(cls, data: dict):
         return cls(
-            score=data['quality_score'],
-            error_type=QualityErrorType(data['quality_error_code']),
+            score=data['quality_score'] if 'quality_score' in data else data['score'],
+            error_type=QualityErrorType(data['quality_error_code'] if 'quality_error_code' in data else data['error_code']),
             message=data['prompt'],
             signature=data['signature']
         )
 
     def to_dataclass(self):
         return Quality(**self.__dict__)
```

### Comparing `intelliprove-1.0.0/intelliprove/api/utils/media.py` & `intelliprove-1.0.1/intelliprove/api/utils/media.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.0/PKG-INFO` & `intelliprove-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelliprove
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Python SDK for using IntelliProve.
 Author: Seppe De Langhe
 Author-email: seppe.delanghe@intelliprove.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

