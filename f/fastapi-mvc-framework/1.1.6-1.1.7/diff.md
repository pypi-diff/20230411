# Comparing `tmp/fastapi_mvc_framework-1.1.6.tar.gz` & `tmp/fastapi_mvc_framework-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.1.6.tar", last modified: Tue Apr 11 05:37:30 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.1.7.tar", last modified: Tue Apr 11 14:16:20 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.1.6.tar` & `fastapi_mvc_framework-1.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:37:30.873590 fastapi_mvc_framework-1.1.6/
--rw-rw-rw-   0        0        0     7266 2023-04-11 05:37:30.873590 fastapi_mvc_framework-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 05:37:30.864614 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0    10267 2023-04-11 05:28:54.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     3716 2023-04-11 05:08:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    12964 2023-04-11 05:36:01.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    11379 2023-04-11 05:34:55.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     1905 2023-04-10 14:13:08.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/database.py
--rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:37:30.872594 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     7266 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 05:37:30.874600 fastapi_mvc_framework-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-04-11 05:37:17.000000 fastapi_mvc_framework-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:16:20.448663 fastapi_mvc_framework-1.1.7/
+-rw-rw-rw-   0        0        0     7266 2023-04-11 14:16:20.447666 fastapi_mvc_framework-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 14:16:20.441682 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0      994 2023-04-11 14:13:14.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0    10309 2023-04-11 12:22:29.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     3716 2023-04-11 05:08:30.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    13007 2023-04-11 14:01:29.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    11379 2023-04-11 05:34:55.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     1905 2023-04-10 14:13:08.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/database.py
+-rw-rw-rw-   0        0        0     5413 2023-04-11 11:47:05.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:16:20.446669 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     7266 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-11 14:16:20.000000 fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 14:16:20.448663 fastapi_mvc_framework-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2023-04-11 14:16:13.000000 fastapi_mvc_framework-1.1.7/setup.py
```

### Comparing `fastapi_mvc_framework-1.1.6/PKG-INFO` & `fastapi_mvc_framework-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_mvc_framework
-Version: 1.1.6
+Version: 1.1.7
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.6 Summary:
+Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.7 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: Apache License 2.0 Description: # fastapi_framework A mvc framework
 used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
 ```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
```

### Comparing `fastapi_mvc_framework-1.1.6/README.md` & `fastapi_mvc_framework-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/_utils.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from datetime import datetime, date
 from json import JSONEncoder
 import re
 
 def is_datetime_format(s):
-
+    if not isinstance(s,str) or not str:
+        return False 
     _datetime_regex = re.compile(
         r'^\d{4}-\d{2}-\d{2}(T\d{2}:\d{2}:\d{2}(\.\d+)?(Z|[+-]\d{2}:\d{2})?)?$'
     )
 
     _date_regex = re.compile(r'^\d{4}-\d{2}-\d{2}$')
 
     _time_regex = re.compile(r'^\d{2}:\d{2}:\d{2}$')
```

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,16 @@
                 scheme, credentials = auth.split() 
                 token = self.__get_token_from_header(authorization=auth, prefix=prefix)
                 
                 del kwargs['username_field']
                 try:
                     payload = jwt.decode(token,**kwargs)
                 except jwt.InvalidTokenError as e:
-                    raise AuthenticationError(str(e)) from e
+                    request.session[self.__session_name] = None
+                    return "","",None
                 if is_datetime_format(payload['exp']):
                     payload['exp'] = datetime.fromisoformat(payload['exp'])
 
 
                 return  payload[username_field],token,payload
             elif userobj:
                 if 'token' in userobj:
```

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/base_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/controller_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,18 +337,18 @@
                 result = await func(*args, **kwargs)
             else:
                 result =  func(*args,**kwargs)
             if isinstance(result,tuple):result = result[0]
             if response and isinstance(result,Response):
                 
                 result.raw_headers.extend(response.raw_headers)
-            
-            ret = await cls._deconstructor(cls,result)
-            if isinstance(ret,Response):
-                result = ret
+            if isinstance(result,Response):
+                ret = await cls._deconstructor(cls,result)
+                if isinstance(ret,Response):
+                    result = ret
             # __clear_flash(request=rqst)
             return result
         setattr(decorator, PATH_KEY, path)
         setattr(decorator, METHOD_KEY, method)
         setattr(decorator, ARGS_KEY, args)
         if '__auth_url__' in mwargs: 
             setattr(func,'__auth_url__',mwargs['__auth_url__'])
```

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/core.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/database.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/database.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,17 +64,15 @@
             return ret
         else:
             content = "<h1>404 Not Found(URL Exception)</h1>"
             content += '<h3>please check url</h3>'
             if debug:
                 content += '<p>' + str(e.detail) + '</p>'
             return HTMLResponse(content=content, status_code=404)
-        _log.error(f"OMG! An HTTP error!: {repr(exc)}")
-        return await http_exception_handler(request, exc)#by default handler
-
+   
     @app.exception_handler(Exception)
     async def validation_exception_handler(request, e:Exception):
         ret = error_page(500,request=request,e=e)
         if ret:
             return ret
         else:
             content = "<h1>500 Internal Server Error</h1>"
@@ -93,18 +91,19 @@
     @app.exception_handler(RequestValidationError)
     async def validation_exception_handler(request, exc):
         _log.error(f"OMG! The client sent invalid data!: {exc}")
         return await request_validation_exception_handler(request, exc)
 
     @app.route('/public/error_404.html',['GET','POST','HEAD','OPTION','PUT','DELETE'])
     def _error1(request):
-        return Response(content = None,status_code= 404)
+        raise HTTPException(404,"Not Found.")
+        # return Response(content = None,status_code= 404)
     @app.route('/public/error_500.html',['GET','POST','HEAD','OPTION','PUT','DELETE'])
     def _error2(request):
-        return Response(content = None,status_code= 404)
+        raise HTTPException(404,"Not Found.")
     
     #mount public resources
     public_dir =  os.path.abspath(config.get("public_dir" ) )
     if not os.path.exists(public_dir):
         os.mkdir(public_dir) 
     app.mount('/public',  StaticFiles(directory=public_dir), name='public')
```

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/midware_session.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mvc-framework
-Version: 1.1.6
+Version: 1.1.7
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.6 Summary:
+Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.7 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: Apache License 2.0 Description: # fastapi_framework A mvc framework
 used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
 ```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
```

### Comparing `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.1.7/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.6/setup.py` & `fastapi_mvc_framework-1.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     long_description = fh.read()
 with open('requirements.txt', encoding="utf-8-sig") as f:
     requirements = f.readlines()
 
 
 setup(
     name='fastapi_mvc_framework',
-    version='1.1.6',
+    version='1.1.7',
     license='Apache License 2.0',
     author='Bruce chou',
     author_email='smjkzsl@gmail.com',
     description='Simple and elegant use of FastApi in MVC mode',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
```

