# Comparing `tmp/fastapi_mvc_framework-1.1.5.tar.gz` & `tmp/fastapi_mvc_framework-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.1.5.tar", last modified: Mon Apr 10 14:23:17 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.1.6.tar", last modified: Tue Apr 11 05:37:30 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.1.5.tar` & `fastapi_mvc_framework-1.1.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:23:17.472672 fastapi_mvc_framework-1.1.5/
--rw-rw-rw-   0        0        0     6979 2023-04-10 14:23:17.471674 fastapi_mvc_framework-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:23:17.464692 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0     9943 2023-04-09 05:56:58.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     3733 2023-04-09 05:46:23.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    12971 2023-04-09 05:48:57.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    11234 2023-04-10 14:14:04.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     1905 2023-04-10 14:13:08.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/database.py
--rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:23:17.469679 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     6979 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      682 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-10 14:23:17.000000 fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 14:23:17.473669 fastapi_mvc_framework-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-04-10 14:23:07.000000 fastapi_mvc_framework-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:37:30.873590 fastapi_mvc_framework-1.1.6/
+-rw-rw-rw-   0        0        0     7266 2023-04-11 05:37:30.873590 fastapi_mvc_framework-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 05:37:30.864614 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0    10267 2023-04-11 05:28:54.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     3716 2023-04-11 05:08:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    12964 2023-04-11 05:36:01.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    11379 2023-04-11 05:34:55.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     1905 2023-04-10 14:13:08.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/database.py
+-rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:37:30.872594 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     7266 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-11 05:37:30.000000 fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:37:30.874600 fastapi_mvc_framework-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2023-04-11 05:37:17.000000 fastapi_mvc_framework-1.1.6/setup.py
```

### Comparing `fastapi_mvc_framework-1.1.5/PKG-INFO` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: fastapi_mvc_framework
-Version: 1.1.5
+Name: fastapi-mvc-framework
+Version: 1.1.6
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
-License: UNKNOWN
+License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
         Simple and elegant use of FastApi in MVC mode
         
         ## usage:
         install:
         ```bash
@@ -193,13 +193,18 @@
         |   |   |   |   ac7ce07126b3_autogenerate.py
         |   |   |   |   e51711eb3d84_autogenerate.py
         |   |   |   |
         |   \---db
         |           test.db
         
         ```
+Keywords: web framework,mvc framework,fastapi framework
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.5 Summary:
+Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.6 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
-License: UNKNOWN Description: # fastapi_framework A mvc framework used FastApi
-Simple and elegant use of FastApi in MVC mode ## usage: install: ```bash pip
-install fastapi-mvc-framework ``` controller: ```python from
+License: Apache License 2.0 Description: # fastapi_framework A mvc framework
+used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
+```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
 from typing import Dict from app.services import UserService
 application._public_auth_url = '/user/login' application._user_auth_url = '/
 user/login' @api_router(auth='public') class TestController(BaseController):
 @api.get("/user/login") def login(self): """:title Login""" redirect =
 self.params['redirect'] if 'redirect' in self.params else '/' return self.view
@@ -51,11 +51,14 @@
 +---test1 | | | \---v1.0 | | | home.css | | | home.html | | | home1.css | | | |
 | \---test2 | +---configs | alembic.ini | cache.yaml | casbin-adapter.csv |
 casbin-model.conf | database.yaml | general.yaml | session.yaml | +---data | +-
 --alembic | | | env.py | | | README | | | script.py.mako | | | | | +---versions
 | | | | 0d0205db5b39_create_tables.py | | | | 0e4e15e67367_autogenerate.py | |
 | | 108dad121227__new_upgrade_operations_detected__add_.py | | | |
 ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | \--
--db | test.db ``` Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown
+-db | test.db ``` Keywords: web framework,mvc framework,fastapi framework
+Platform: UNKNOWN Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `fastapi_mvc_framework-1.1.5/README.md` & `fastapi_mvc_framework-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/_utils.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,25 +62,26 @@
                 
                 del kwargs['username_field']
                 try:
                     payload = jwt.decode(token,**kwargs)
                 except jwt.InvalidTokenError as e:
                     raise AuthenticationError(str(e)) from e
                 if is_datetime_format(payload['exp']):
-                    payload['exp'] =   datetime.fromisoformat(payload['exp'])
+                    payload['exp'] = datetime.fromisoformat(payload['exp'])
 
 
                 return  payload[username_field],token,payload
             elif userobj:
                 if 'token' in userobj:
                     try:
                         payload = jwt.decode(userobj['token'],**kwargs)
                     except jwt.InvalidTokenError as e:#Signature has expired
+                        request.session[self.__session_name] = None
                         return "","",None
-                        raise AuthenticationError(str(e)) from e
+                        # raise AuthenticationError(str(e)) from e
                      
                     return  payload[username_field],userobj['token'],payload
         else:
             if userobj: 
                 return userobj,"",None
             else:
                 decoded = base64.b64decode(credentials).decode("ascii")
@@ -194,15 +195,20 @@
             if authCfg:
                 expires_delta = int(authCfg.get('expires_delta',60))
             else:
                 expires_delta = 60
             expire = datetime.utcnow() + timedelta(
                 minutes=expires_delta
             )
-        userObj = {"exp": expire, "username": user }
+        if isinstance(user,str):
+            userObj = {"exp": expire, "username": user }
+        elif isinstance(user,JWTUser):
+            userObj = {"exp": expire, "username": user.username}
+        elif isinstance(user,BaseUser):
+            userObj = {"exp": expire, "username": user.display_name}
         request:Request = kwargs['request']
         
         access_token = jwt.encode(userObj, self.secret_key ,self.algorithm )
         userObj.update({"token":access_token})
         request.session[_session_name] = userObj
         return access_token
```

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/base_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,15 @@
 
     setattr(GeneratedController, TEMPLATE_PATH_KEY, template_path_prefix)
     setattr(GeneratedController, VER_KEY, version)
 
     return GeneratedController
 
 
-class controller:
-     
-        
+class MvcRouter: 
     """ """
     @staticmethod
     def http(path,methods=['GET'],*args,**kwargs):
         return _route_method(path,method=methods,*args,**kwargs)
     @staticmethod
     def get(path: str, *args, **kwargs): 
         return _route_method(path, "get", *args, **kwargs)
```

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/controller_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,17 +313,15 @@
             #instance = cls.__dict__.get('__wrapped__', None).__self__ #or cls.__dict__.get('__objclass__', None)(obj)
             response:Response = None
             result:Response = None
             
             if 'request' in kwargs and 'response' in kwargs:
                 response  = kwargs["response"]
                 rqst = kwargs['request']  
-
-                # __init_flash(rqst)
-                
+                #auth first then call constructor
                 if auth_type and auth_type !="none"  :
                     auth_result,user = await cls._auth__(request=rqst,response=kwargs['response'],auth_type=auth_type)
                     if isinstance(auth_result,Response):
                         # __clear_flash(request=rqst)
                         return auth_result
                     if not auth_result:
                         auth_error()
```

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                      Request,
                      Response,
                      WebSocket,
                      WebSocketDisconnect, 
                      Cookie,
                      status as StateCodes)
  
-from .controller import create_controller,controller as api,   register_controllers_to_app 
+from .controller import create_controller,MvcRouter as api,   register_controllers_to_app 
 from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
 from .config import config,ROOT_PATH,_log
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
@@ -152,23 +152,24 @@
             
             @classmethod
             async def _auth__(cls,request:Request,response:Response,**kwargs):
                 '''called by .controller_util.py->route_method'''
                 if not hasattr(application,'authObj'):
                     return True,None
                 auth_type = kwargs['auth_type'] 
-                kwargs['session'] = request.session # cls._session
+                kwargs['session'] = request.session  
                 ret,user = await application.authObj.authenticate(request,**kwargs)
                 def add_redirect_param(url: str, redirect_url: str) -> str:
                     if "?" in url:
                         return url + "&redirect=" + redirect_url
                     else:
                         return url + "?redirect=" + redirect_url
                 accept_header = request.headers.get("Accept")
-                
+                if user: #continue singture 
+                    application.authObj.create_access_token(user=user, expires_delta=None,request=request)
                 #
                 if not ret and not user: 
                     if accept_header == "application/json":
                         return  ORJSONResponse(content={"message": "401 UNAUTHORIZED!"},
                                                    status_code=StateCodes.HTTP_401_UNAUTHORIZED),None
                     _auth_url = getattr(application,f"_{auth_type}_auth_url") if hasattr(application,f"_{auth_type}_auth_url") else None
 
@@ -210,15 +211,16 @@
 
 def get_wrapped_endpoint(func):
     ret = func
     while hasattr(ret,'__wrapped__'):
         ret = getattr(ret,'__wrapped__')
     return ret
 
-def generate_mvc_app(isDebug):
+def generate_mvc_app( ):
+    global __is_debug
     if not len(__all_controller__)>0:
         raise "must use @api_route to define a controller class"
     all_routers = []
     all_routers_map = {}
     for ctrl in __all_controller__:
         all_routers.append(register_controllers_to_app(application, ctrl))
     for router in all_routers:
@@ -227,19 +229,19 @@
             end_point_abs = get_wrapped_endpoint(r.endpoint)
             auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
             doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
             if hasattr(r,'methods'):
                 methods = r.methods
             else:
                 methods = r.name
-            if isDebug:  
+            if __is_debug:  
                 _log.debug('{:20}-->{:50}-->{}'.format(str(methods),r.path,funcname) )
             all_routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type}
     application.routers_map = all_routers_map  
-    midware.init(app=application,debug=isDebug)
+    midware.init(app=application,debug=__is_debug)
     
     auth_type = config.get("auth",None)
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
             application.authObj = __init_auth(application,auth_type)
     __init_database()
```

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/database.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/database.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/midware_session.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: fastapi-mvc-framework
-Version: 1.1.5
+Name: fastapi_mvc_framework
+Version: 1.1.6
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
-License: UNKNOWN
+License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
         Simple and elegant use of FastApi in MVC mode
         
         ## usage:
         install:
         ```bash
@@ -193,13 +193,18 @@
         |   |   |   |   ac7ce07126b3_autogenerate.py
         |   |   |   |   e51711eb3d84_autogenerate.py
         |   |   |   |
         |   \---db
         |           test.db
         
         ```
+Keywords: web framework,mvc framework,fastapi framework
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.5 Summary:
+Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.6 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
-License: UNKNOWN Description: # fastapi_framework A mvc framework used FastApi
-Simple and elegant use of FastApi in MVC mode ## usage: install: ```bash pip
-install fastapi-mvc-framework ``` controller: ```python from
+License: Apache License 2.0 Description: # fastapi_framework A mvc framework
+used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
+```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
 from typing import Dict from app.services import UserService
 application._public_auth_url = '/user/login' application._user_auth_url = '/
 user/login' @api_router(auth='public') class TestController(BaseController):
 @api.get("/user/login") def login(self): """:title Login""" redirect =
 self.params['redirect'] if 'redirect' in self.params else '/' return self.view
@@ -51,11 +51,14 @@
 +---test1 | | | \---v1.0 | | | home.css | | | home.html | | | home1.css | | | |
 | \---test2 | +---configs | alembic.ini | cache.yaml | casbin-adapter.csv |
 casbin-model.conf | database.yaml | general.yaml | session.yaml | +---data | +-
 --alembic | | | env.py | | | README | | | script.py.mako | | | | | +---versions
 | | | | 0d0205db5b39_create_tables.py | | | | 0e4e15e67367_autogenerate.py | |
 | | 108dad121227__new_upgrade_operations_detected__add_.py | | | |
 ac7ce07126b3_autogenerate.py | | | | e51711eb3d84_autogenerate.py | | | | | \--
--db | test.db ``` Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown
+-db | test.db ``` Keywords: web framework,mvc framework,fastapi framework
+Platform: UNKNOWN Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `fastapi_mvc_framework-1.1.5/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.1.6/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 fastapi_mvc_framework/midware.py
 fastapi_mvc_framework/midware_casbin.py
 fastapi_mvc_framework/midware_session.py
 fastapi_mvc_framework/view.py
 fastapi_mvc_framework.egg-info/PKG-INFO
 fastapi_mvc_framework.egg-info/SOURCES.txt
 fastapi_mvc_framework.egg-info/dependency_links.txt
+fastapi_mvc_framework.egg-info/requires.txt
 fastapi_mvc_framework.egg-info/top_level.txt
```

