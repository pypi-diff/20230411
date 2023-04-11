# Comparing `tmp/taichu-serve-1.0.10.tar.gz` & `tmp/taichu-serve-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-1.0.10.tar", last modified: Mon Apr 10 07:50:08 2023, max compression
+gzip compressed data, was "taichu-serve-1.0.11.tar", last modified: Tue Apr 11 08:59:04 2023, max compression
```

## Comparing `taichu-serve-1.0.10.tar` & `taichu-serve-1.0.11.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:50:08.374060 taichu-serve-1.0.10/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-10 07:50:08.373890 taichu-serve-1.0.10/PKG-INFO
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:50:08.372077 taichu-serve-1.0.10/model_service/
--rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-serve-1.0.10/model_service/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     8308 2023-04-10 07:48:58.000000 taichu-serve-1.0.10/model_service/app.py
--rw-r--r--   0 chen       (501) staff       (20)     1302 2023-04-10 07:48:58.000000 taichu-serve-1.0.10/model_service/command.py
--rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-serve-1.0.10/model_service/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-1.0.10/model_service/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-serve-1.0.10/model_service/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-serve-1.0.10/model_service/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     3568 2023-04-03 11:36:45.000000 taichu-serve-1.0.10/model_service/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-serve-1.0.10/model_service/log.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:50:08.372440 taichu-serve-1.0.10/model_service/model_def/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-1.0.10/model_service/model_def/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-serve-1.0.10/model_service/model_def/model_def.py
--rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-serve-1.0.10/model_service/model_service.py
--rw-r--r--   0 chen       (501) staff       (20)     1061 2023-04-10 07:48:58.000000 taichu-serve-1.0.10/model_service/settings.py
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-10 07:50:08.374111 taichu-serve-1.0.10/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      952 2023-04-10 07:48:58.000000 taichu-serve-1.0.10/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:50:08.373585 taichu-serve-1.0.10/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-10 07:50:08.000000 taichu-serve-1.0.10/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      609 2023-04-10 07:50:08.000000 taichu-serve-1.0.10/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-10 07:50:08.000000 taichu-serve-1.0.10/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-10 07:50:08.000000 taichu-serve-1.0.10/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-10 07:50:08.000000 taichu-serve-1.0.10/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-10 07:50:08.000000 taichu-serve-1.0.10/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.811370 taichu-serve-1.0.11/
+-rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-11 08:59:04.811127 taichu-serve-1.0.11/PKG-INFO
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.809610 taichu-serve-1.0.11/model_service/
+-rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     8308 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     1302 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-serve-1.0.11/model_service/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-1.0.11/model_service/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     3572 2023-04-11 04:36:47.000000 taichu-serve-1.0.11/model_service/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-serve-1.0.11/model_service/log.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.809947 taichu-serve-1.0.11/model_service/model_def/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/model_def/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-serve-1.0.11/model_service/model_def/model_def.py
+-rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-serve-1.0.11/model_service/model_service.py
+-rw-r--r--   0 chen       (501) staff       (20)     1061 2023-04-10 07:48:58.000000 taichu-serve-1.0.11/model_service/settings.py
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-11 08:59:04.811428 taichu-serve-1.0.11/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      952 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 08:59:04.810922 taichu-serve-1.0.11/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      236 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      609 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-11 08:59:04.000000 taichu-serve-1.0.11/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-1.0.10/model_service/app.py` & `taichu-serve-1.0.11/model_service/app.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/command.py` & `taichu-serve-1.0.11/model_service/command.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/common.py` & `taichu-serve-1.0.11/model_service/common.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/error_code.py` & `taichu-serve-1.0.11/model_service/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/grpc_predict_v2_pb2.py` & `taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-1.0.11/model_service/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/grpc_server.py` & `taichu-serve-1.0.11/model_service/grpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,30 +75,30 @@
 
     @grpc_interceptor
     def ModelStreamInfer(self, request, context):
         # 检测是否有客户端断开连接
         ctx = {}
         while context.is_active():
             for req in request:
-                logger.info('recv: %s', req)
+                # logger.info('recv: %s', req)
                 ctx['model_name'] = req.model_name
                 ctx['model_version'] = req.model_version
 
                 instance = get_model_service(req.model_name, req.model_version)
 
                 rec_dict = parameters_to_dict(req.parameters)
 
                 try:
                     res = instance.inference(rec_dict, context=ctx)
                 except Exception as e:
                     logger.error('Algorithm crashed!, %s', str(e))
                     logger.error(traceback.format_exc())
                     raise ModelPredictError(message=str(e))
 
-                logger.info('ret: %s', res)
+                # logger.info('ret: %s', res)
                 resp = self.make_response(res)
                 resp.model_name = req.model_name
                 resp.model_version = req.model_version
 
                 yield resp
 
     def ServerLive(self, request, context):
```

### Comparing `taichu-serve-1.0.10/model_service/log.py` & `taichu-serve-1.0.11/model_service/log.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/model_def/model_def.py` & `taichu-serve-1.0.11/model_service/model_def/model_def.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/model_service.py` & `taichu-serve-1.0.11/model_service/model_service.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/model_service/settings.py` & `taichu-serve-1.0.11/model_service/settings.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.10/setup.py` & `taichu-serve-1.0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if __name__ == '__main__':
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf', 'Flask', 'gunicorn', 'Jinja2', 'Pillow']
 
     setup(
         name=name,
-        version='1.0.10',
+        version='1.0.11',
         description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
```

### Comparing `taichu-serve-1.0.10/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-1.0.11/taichu_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

