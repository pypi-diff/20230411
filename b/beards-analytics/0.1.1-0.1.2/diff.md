# Comparing `tmp/beards_analytics-0.1.1-py3-none-any.whl.zip` & `tmp/beards_analytics-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5453 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 13:42 beards_analytics/__init__.py
+Zip file size: 5361 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-11 14:24 beards_analytics/__init__.py
 -rw-r--r--  2.0 unx      847 b- defN 23-Apr-11 13:23 beards_analytics/date.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 13:10 beards_analytics/cloud_functions/__init__.py
--rw-r--r--  2.0 unx     3363 b- defN 23-Apr-11 13:37 beards_analytics/cloud_functions/http.py
+-rw-r--r--  2.0 unx     3049 b- defN 23-Apr-11 14:20 beards_analytics/cloud_functions/http.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 11:18 beards_analytics/data/__init__.py
 -rw-r--r--  2.0 unx      514 b- defN 23-Apr-11 13:34 beards_analytics/data/models.py
 -rw-r--r--  2.0 unx      757 b- defN 23-Apr-11 13:39 beards_analytics/data/operations.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      680 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-11 13:43 beards_analytics-0.1.1.dist-info/RECORD
-12 files, 8409 bytes uncompressed, 3633 bytes compressed:  56.8%
+-rw-r--r--  2.0 unx     1060 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      680 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-11 14:24 beards_analytics-0.1.2.dist-info/RECORD
+12 files, 8095 bytes uncompressed, 3541 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: beards_analytics/data/models.py
 Comment: 
 
 Filename: beards_analytics/data/operations.py
 Comment: 
 
-Filename: beards_analytics-0.1.1.dist-info/LICENCE.txt
+Filename: beards_analytics-0.1.2.dist-info/LICENCE.txt
 Comment: 
 
-Filename: beards_analytics-0.1.1.dist-info/METADATA
+Filename: beards_analytics-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: beards_analytics-0.1.1.dist-info/WHEEL
+Filename: beards_analytics-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: beards_analytics-0.1.1.dist-info/top_level.txt
+Filename: beards_analytics-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: beards_analytics-0.1.1.dist-info/RECORD
+Filename: beards_analytics-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beards_analytics/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
```

## beards_analytics/cloud_functions/http.py

```diff
@@ -29,19 +29,17 @@
     
     @property
     def args(self) -> _ConvertableDict:
         d = _ConvertableDict(super().args)
         d._input_source_label = 'query params'
         return d
 
-def _get_request_from_cf_func(*args, func: _ENTRY_FUNC) -> flask.Request:
-    request: flask.Request = (args or (None,))[0]
-    if not isinstance(request, flask.Request):
-        raise RuntimeError(f'{func.__name__} is not valid CF entrypoint')
-    return request
+def _update_flask_request():
+    if flask.request.__class__ != Request:
+        flask.request.__class__ = Request
 
 def _to_flask_response(obj: t.Any):
     if obj is None:
         return ''
 
     if isinstance(obj, (dict, list, tuple)):
         return flask.jsonify(obj)
@@ -55,17 +53,16 @@
     return flask.jsonify(dict(
         message = message, 
         errors = errors if type(errors) is list else [errors]
     )), status_code
 
 def safe_return(func: _ENTRY_FUNC):
     @functools.wraps(func)
-    def wrapper(*args):
-        request: flask.Request = _get_request_from_cf_func(*args, func=func)
-        return_val = func(request)
+    def wrapper(*args, **kwargs):
+        return_val = func(*args, **kwargs)
         status_code = None
         
         if type(return_val) is tuple and type(return_val[1]) is int:
             return_val, status_code = return_val
 
         response = _to_flask_response(return_val)
 
@@ -75,35 +72,33 @@
     return wrapper
 
 def entry_point(func: _ENTRY_FUNC):
     func = functions_framework.http(func)
     func = safe_return(func)
 
     @functools.wraps(func)
-    def wrapper(*args):
-        request = _get_request_from_cf_func(*args, func=func)
-        request.__class__ = Request
+    def wrapper(*args, **kwargs):
+        _update_flask_request()
         
         try:
-            return func(request)
+            return func(*args, **kwargs)
         except pydantic.ValidationError as e:
             if hasattr(e, _INPUT_SOURCE):
                 input_source: str = getattr(e, _INPUT_SOURCE)
                 return error_response(message=f'Invalid {input_source}', errors=e.errors(), status_code=400)
             raise
 
     return wrapper
 
 def api_key_auth(allowed_api_key: str, api_key_query_param_name: str = 'api_key'):
     def decorator(func: _ENTRY_FUNC):
         @functools.wraps(func)
-        def wrapper(*args):
-            request: flask.Request = _get_request_from_cf_func(*args, func=func)
-            api_key = request.args.get(api_key_query_param_name)
+        def wrapper(*args, **kwargs):
+            api_key = flask.request.args.get(api_key_query_param_name)
             
             if api_key != allowed_api_key:
                 return error_response(message='Forbidden', errors='Invalid API key', status_code=403)
             
-            return func(request)
+            return func(*args, **kwargs)
 
         return wrapper
     return decorator
```

## Comparing `beards_analytics-0.1.1.dist-info/LICENCE.txt` & `beards_analytics-0.1.2.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `beards_analytics-0.1.1.dist-info/METADATA` & `beards_analytics-0.1.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beards-analytics
-Version: 0.1.1
+Version: 0.1.2
 Summary: Beards Analytics packages
 Home-page: https://beardsanalytics.com
 Author: Beards Analytics
 Author-email: tz@or.com.ua
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `beards_analytics-0.1.1.dist-info/RECORD` & `beards_analytics-0.1.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-beards_analytics/__init__.py,sha256=ls1camlIoMxEZz9gSkZ1OJo-MXqHWwKPtdPbZJmwp7E,22
+beards_analytics/__init__.py,sha256=mdp2CftfqYbdKtP-eWv1z7rAUycYv6X1ntXSMUf8Kss,22
 beards_analytics/date.py,sha256=amLlla8Smayw8ZnEAS0lJebusnIaBBAdxA0u-h_tl7M,847
 beards_analytics/cloud_functions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-beards_analytics/cloud_functions/http.py,sha256=LUQY5aRlDOCNaYHC42CEYyAKGspith3tMl3xdpsdKpo,3363
+beards_analytics/cloud_functions/http.py,sha256=seAsFkG3PuXnLXe0xl_kCQQj2MNAnR0gwfSHey1Zn6Y,3049
 beards_analytics/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beards_analytics/data/models.py,sha256=79oHvRbMaWTz_o1GK2dIqL6Uh2cIIVbnel4JcxUkHxk,514
 beards_analytics/data/operations.py,sha256=XYzdSjon7XCkh2GaCPZURHO9MEhoPcpRu8Hm5hIoRbo,757
-beards_analytics-0.1.1.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
-beards_analytics-0.1.1.dist-info/METADATA,sha256=wjm4VE3gCUgh9cm6PtiuZFveipUpbNWg1DpVvPc5Njo,680
-beards_analytics-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-beards_analytics-0.1.1.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
-beards_analytics-0.1.1.dist-info/RECORD,,
+beards_analytics-0.1.2.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
+beards_analytics-0.1.2.dist-info/METADATA,sha256=4EUq15hB2vOyo319q0wMgulOrk03VyaVovasFuJFZ1o,680
+beards_analytics-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+beards_analytics-0.1.2.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
+beards_analytics-0.1.2.dist-info/RECORD,,
```

