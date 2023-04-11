# Comparing `tmp/beards_analytics-0.1.2-py3-none-any.whl.zip` & `tmp/beards_analytics-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 5361 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 14:24 beards_analytics/__init__.py
--rw-r--r--  2.0 unx      847 b- defN 23-Apr-11 13:23 beards_analytics/date.py
+Zip file size: 4883 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 15:25 beards_analytics/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:10 beards_analytics/cloud_functions/__init__.py
 -rw-r--r--  2.0 unx     3049 b- defN 23-Apr-11 14:20 beards_analytics/cloud_functions/http.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 11:18 beards_analytics/data/__init__.py
 -rw-r--r--  2.0 unx      514 b- defN 23-Apr-11 13:34 beards_analytics/data/models.py
--rw-r--r--  2.0 unx      757 b- defN 23-Apr-11 13:39 beards_analytics/data/operations.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      680 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/RECORD
-12 files, 8095 bytes uncompressed, 3541 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-11 14:50 beards_analytics/data/operations.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Apr-11 15:26 beards_analytics-0.1.3.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      680 b- defN 23-Apr-11 15:26 beards_analytics-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 15:26 beards_analytics-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-11 15:26 beards_analytics-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      977 b- defN 23-Apr-11 15:26 beards_analytics-0.1.3.dist-info/RECORD
+11 files, 7193 bytes uncompressed, 3187 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -1,13 +1,10 @@
 Filename: beards_analytics/__init__.py
 Comment: 
 
-Filename: beards_analytics/date.py
-Comment: 
-
 Filename: beards_analytics/cloud_functions/__init__.py
 Comment: 
 
 Filename: beards_analytics/cloud_functions/http.py
 Comment: 
 
 Filename: beards_analytics/data/__init__.py
@@ -15,23 +12,23 @@
 
 Filename: beards_analytics/data/models.py
 Comment: 
 
 Filename: beards_analytics/data/operations.py
 Comment: 
 
-Filename: beards_analytics-0.1.2.dist-info/LICENCE.txt
+Filename: beards_analytics-0.1.3.dist-info/LICENCE.txt
 Comment: 
 
-Filename: beards_analytics-0.1.2.dist-info/METADATA
+Filename: beards_analytics-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: beards_analytics-0.1.2.dist-info/WHEEL
+Filename: beards_analytics-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: beards_analytics-0.1.2.dist-info/top_level.txt
+Filename: beards_analytics-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: beards_analytics-0.1.2.dist-info/RECORD
+Filename: beards_analytics-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beards_analytics/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
```

## beards_analytics/data/operations.py

```diff
@@ -1,14 +1,13 @@
 from slugify import slugify
 import typing as t
+from beards_analytics.common import types
 
 
-_T = t.TypeVar('_T')
-
-def slugify_object_keys(obj, separator='-', lowercase=False):
+def slugify_object_keys(obj, separator='_', lowercase=False):
     def inner_func(data):        
         if isinstance(data, dict):
             new_data = {}
             for key, value in data.items():
                 new_key = slugify(key, separator=separator, lowercase=lowercase)
                 new_value = inner_func(value)
                 new_data[new_key] = new_value
@@ -16,9 +15,9 @@
         elif isinstance(data, list):
             return [inner_func(item) for item in data]
         else:
             return data
 
     return inner_func(obj)
 
-def chunk_list(lst: t.List[_T], chunk_size: int):
+def chunk_list(lst: t.List[types.T], chunk_size: int):
     return [lst[i:i + chunk_size] for i in range(0, len(lst), chunk_size)]
```

## Comparing `beards_analytics-0.1.2.dist-info/LICENCE.txt` & `beards_analytics-0.1.3.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `beards_analytics-0.1.2.dist-info/METADATA` & `beards_analytics-0.1.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beards-analytics
-Version: 0.1.2
+Version: 0.1.3
 Summary: Beards Analytics packages
 Home-page: https://beardsanalytics.com
 Author: Beards Analytics
 Author-email: tz@or.com.ua
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `beards_analytics-0.1.2.dist-info/RECORD` & `beards_analytics-0.1.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-beards_analytics/__init__.py,sha256=mdp2CftfqYbdKtP-eWv1z7rAUycYv6X1ntXSMUf8Kss,22
-beards_analytics/date.py,sha256=amLlla8Smayw8ZnEAS0lJebusnIaBBAdxA0u-h_tl7M,847
+beards_analytics/__init__.py,sha256=uZsygMXMKRw-7qhWojAjnpm8GFPXU92xW6XA8O5GwFY,22
 beards_analytics/cloud_functions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beards_analytics/cloud_functions/http.py,sha256=seAsFkG3PuXnLXe0xl_kCQQj2MNAnR0gwfSHey1Zn6Y,3049
 beards_analytics/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beards_analytics/data/models.py,sha256=79oHvRbMaWTz_o1GK2dIqL6Uh2cIIVbnel4JcxUkHxk,514
-beards_analytics/data/operations.py,sha256=XYzdSjon7XCkh2GaCPZURHO9MEhoPcpRu8Hm5hIoRbo,757
-beards_analytics-0.1.2.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
-beards_analytics-0.1.2.dist-info/METADATA,sha256=4EUq15hB2vOyo319q0wMgulOrk03VyaVovasFuJFZ1o,680
-beards_analytics-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-beards_analytics-0.1.2.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
-beards_analytics-0.1.2.dist-info/RECORD,,
+beards_analytics/data/operations.py,sha256=QwIoW6LXlhAVH7RGM8xkW7DgC7qAD1De_1sulm_zBLU,782
+beards_analytics-0.1.3.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
+beards_analytics-0.1.3.dist-info/METADATA,sha256=EYG9PVZV27NyTG0N5p2rRhkVngei6R2zGqDZ-OOCbKU,680
+beards_analytics-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+beards_analytics-0.1.3.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
+beards_analytics-0.1.3.dist-info/RECORD,,
```

