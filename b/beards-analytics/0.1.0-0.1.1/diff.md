# Comparing `tmp/beards_analytics-0.1.0-py3-none-any.whl.zip` & `tmp/beards_analytics-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 4868 bytes, number of entries: 11
--rw-r--r--  2.0 unx       22 b- defN 23-Mar-31 14:46 beards_analytics/__init__.py
+Zip file size: 5453 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 13:42 beards_analytics/__init__.py
+-rw-r--r--  2.0 unx      847 b- defN 23-Apr-11 13:23 beards_analytics/date.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:10 beards_analytics/cloud_functions/__init__.py
--rw-r--r--  2.0 unx     3363 b- defN 23-Mar-31 14:44 beards_analytics/cloud_functions/http.py
+-rw-r--r--  2.0 unx     3363 b- defN 23-Apr-11 13:37 beards_analytics/cloud_functions/http.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 11:18 beards_analytics/data/__init__.py
--rw-r--r--  2.0 unx      521 b- defN 23-Mar-30 11:20 beards_analytics/data/models.py
--rw-r--r--  2.0 unx      649 b- defN 23-Mar-30 11:17 beards_analytics/data/operations.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Mar-31 14:46 beards_analytics-0.1.0.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      612 b- defN 23-Mar-31 14:46 beards_analytics-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 14:46 beards_analytics-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-31 14:46 beards_analytics-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      977 b- defN 23-Mar-31 14:46 beards_analytics-0.1.0.dist-info/RECORD
-11 files, 7313 bytes uncompressed, 3172 bytes compressed:  56.6%
+-rw-r--r--  2.0 unx      514 b- defN 23-Apr-11 13:34 beards_analytics/data/models.py
+-rw-r--r--  2.0 unx      757 b- defN 23-Apr-11 13:39 beards_analytics/data/operations.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      680 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/RECORD
+12 files, 8409 bytes uncompressed, 3633 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: beards_analytics/__init__.py
 Comment: 
 
+Filename: beards_analytics/date.py
+Comment: 
+
 Filename: beards_analytics/cloud_functions/__init__.py
 Comment: 
 
 Filename: beards_analytics/cloud_functions/http.py
 Comment: 
 
 Filename: beards_analytics/data/__init__.py
@@ -12,23 +15,23 @@
 
 Filename: beards_analytics/data/models.py
 Comment: 
 
 Filename: beards_analytics/data/operations.py
 Comment: 
 
-Filename: beards_analytics-0.1.0.dist-info/LICENCE.txt
+Filename: beards_analytics-0.1.1.dist-info/LICENCE.txt
 Comment: 
 
-Filename: beards_analytics-0.1.0.dist-info/METADATA
+Filename: beards_analytics-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: beards_analytics-0.1.0.dist-info/WHEEL
+Filename: beards_analytics-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: beards_analytics-0.1.0.dist-info/top_level.txt
+Filename: beards_analytics-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: beards_analytics-0.1.0.dist-info/RECORD
+Filename: beards_analytics-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beards_analytics/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## beards_analytics/data/models.py

```diff
@@ -1,15 +1,15 @@
 from datetime import date, datetime
 import pydantic
 import pendulum
 
 
 class BaseModel(pydantic.BaseModel):
     @pydantic.validator('*', pre=True)
-    def validate(cls, value, values, config, field: pydantic.fields.ModelField):
+    def _(cls, value, values, config, field: pydantic.fields.ModelField):
         if field.type_ in (date, datetime) and type(value) is str:
             value = datetime.fromisoformat(pendulum.parser.parse(value).to_datetime_string())
         
         return value
     
     class Config:
         json_encoders = {
```

## beards_analytics/data/operations.py

```diff
@@ -1,21 +1,24 @@
 from slugify import slugify
+import typing as t
 
 
-def slugify_object_keys(obj, **kwargs):
-    kwargs['separator'] = kwargs.get('separator', '_')
-    kwargs['lowercase'] = kwargs.get('lowercase', False)
+_T = t.TypeVar('_T')
 
+def slugify_object_keys(obj, separator='-', lowercase=False):
     def inner_func(data):        
         if isinstance(data, dict):
             new_data = {}
             for key, value in data.items():
-                new_key = slugify(key, **kwargs)
+                new_key = slugify(key, separator=separator, lowercase=lowercase)
                 new_value = inner_func(value)
                 new_data[new_key] = new_value
             return new_data
         elif isinstance(data, list):
             return [inner_func(item) for item in data]
         else:
             return data
 
     return inner_func(obj)
+
+def chunk_list(lst: t.List[_T], chunk_size: int):
+    return [lst[i:i + chunk_size] for i in range(0, len(lst), chunk_size)]
```

## Comparing `beards_analytics-0.1.0.dist-info/LICENCE.txt` & `beards_analytics-0.1.1.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `beards_analytics-0.1.0.dist-info/METADATA` & `beards_analytics-0.1.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beards-analytics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Beards Analytics packages
 Home-page: https://beardsanalytics.com
 Author: Beards Analytics
 Author-email: tz@or.com.ua
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,9 @@
 Requires-Dist: flask
 Requires-Dist: pydantic
 Requires-Dist: functions-framework
 Requires-Dist: ujson
 Requires-Dist: pendulum
 
 # Beards Analytics Python Packages
+
+A useful set of functions to build Google Cloud Functions and more
```

