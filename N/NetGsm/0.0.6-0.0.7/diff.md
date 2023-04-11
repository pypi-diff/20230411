# Comparing `tmp/NetGsm-0.0.6.tar.gz` & `tmp/NetGsm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetGsm-0.0.6.tar", last modified: Tue Apr 11 18:34:52 2023, max compression
+gzip compressed data, was "NetGsm-0.0.7.tar", last modified: Tue Apr 11 19:49:33 2023, max compression
```

## Comparing `NetGsm-0.0.6.tar` & `NetGsm-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 18:34:52.285769 NetGsm-0.0.6/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 NetGsm-0.0.6/LICENSE
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 18:34:52.284305 NetGsm-0.0.6/NetGsm.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1934 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      253 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        7 2023-04-11 18:34:52.000000 NetGsm-0.0.6/NetGsm.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1934 2023-04-11 18:34:52.285638 NetGsm-0.0.6/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1430 2023-04-10 19:34:03.000000 NetGsm-0.0.6/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 18:34:52.285344 NetGsm-0.0.6/netgsm/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       99 2022-11-20 13:13:27.000000 NetGsm-0.0.6/netgsm/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1096 2023-04-10 19:15:27.000000 NetGsm-0.0.6/netgsm/error_code.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      298 2022-11-20 10:40:53.000000 NetGsm-0.0.6/netgsm/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2628 2023-04-11 18:33:32.000000 NetGsm-0.0.6/netgsm/service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-11 18:34:52.285813 NetGsm-0.0.6/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      823 2023-04-11 18:34:45.000000 NetGsm-0.0.6/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 19:49:33.712614 NetGsm-0.0.7/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 NetGsm-0.0.7/LICENSE
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 19:49:33.711079 NetGsm-0.0.7/NetGsm.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1934 2023-04-11 19:49:33.000000 NetGsm-0.0.7/NetGsm.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      253 2023-04-11 19:49:33.000000 NetGsm-0.0.7/NetGsm.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-11 19:49:33.000000 NetGsm-0.0.7/NetGsm.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-11 19:49:33.000000 NetGsm-0.0.7/NetGsm.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        7 2023-04-11 19:49:33.000000 NetGsm-0.0.7/NetGsm.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1934 2023-04-11 19:49:33.712491 NetGsm-0.0.7/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1430 2023-04-10 19:34:03.000000 NetGsm-0.0.7/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-11 19:49:33.712303 NetGsm-0.0.7/netgsm/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       99 2022-11-20 13:13:27.000000 NetGsm-0.0.7/netgsm/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1096 2023-04-10 19:15:27.000000 NetGsm-0.0.7/netgsm/error_code.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      298 2022-11-20 10:40:53.000000 NetGsm-0.0.7/netgsm/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3107 2023-04-11 19:49:25.000000 NetGsm-0.0.7/netgsm/service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-11 19:49:33.712655 NetGsm-0.0.7/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      823 2023-04-11 19:49:25.000000 NetGsm-0.0.7/setup.py
```

### Comparing `NetGsm-0.0.6/LICENSE` & `NetGsm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NetGsm-0.0.6/NetGsm.egg-info/PKG-INFO` & `NetGsm-0.0.7/NetGsm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetGsm
-Version: 0.0.6
+Version: 0.0.7
 Summary: NetGsm Sms Client Python package
 Home-page: https://github.com/blueromans/NetGsm.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/NetGsm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NetGsm-0.0.6/PKG-INFO` & `NetGsm-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetGsm
-Version: 0.0.6
+Version: 0.0.7
 Summary: NetGsm Sms Client Python package
 Home-page: https://github.com/blueromans/NetGsm.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/NetGsm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NetGsm-0.0.6/README.md` & `NetGsm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `NetGsm-0.0.6/netgsm/error_code.py` & `NetGsm-0.0.7/netgsm/error_code.py`

 * *Files identical despite different names*

### Comparing `NetGsm-0.0.6/netgsm/service.py` & `NetGsm-0.0.7/netgsm/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,7 +59,20 @@
     def check_sms_status(self, response):
         response = response.text
         response_code = re.search('[0-9]+', response).group()
         self.is_sms_send = int(response_code) not in ErrorCode.sms_error_codes
         if self.is_sms_send:
             return
         raise NetGsmException(ErrorCode.sms_error_codes[response_code])
+
+    def get_sms_by_bulk_id(self, bulk_id, url='/sms/report', type=0):
+        try:
+            self.params.update({'bulkid': bulk_id,
+                                'type': type})
+            response = requests.get(
+                f'{self.API_URL}{url}',
+                params=self.params,
+            )
+            response = response.text.split(" ")
+            return response[0], response[1]
+        except Exception as e:
+            raise NetGsmException(e.__str__())
```

### Comparing `NetGsm-0.0.6/setup.py` & `NetGsm-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='NetGsm',
-    version="0.0.6",
+    version="0.0.7",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='NetGsm Sms Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/NetGsm.git',
     project_urls={
```

