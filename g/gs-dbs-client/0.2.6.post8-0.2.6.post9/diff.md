# Comparing `tmp/gs-dbs-client-0.2.6.post8.tar.gz` & `tmp/gs-dbs-client-0.2.6.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs-dbs-client-0.2.6.post8.tar", last modified: Thu Sep 15 20:09:26 2022, max compression
+gzip compressed data, was "gs-dbs-client-0.2.6.post9.tar", last modified: Fri Sep 16 08:43:06 2022, max compression
```

## Comparing `gs-dbs-client-0.2.6.post8.tar` & `gs-dbs-client-0.2.6.post9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-15 20:09:26.203408 gs-dbs-client-0.2.6.post8/
--rw-rw-rw-   0        0        0       19 2021-05-10 08:44:21.000000 gs-dbs-client-0.2.6.post8/MANIFEST.in
--rw-rw-rw-   0        0        0     1306 2022-09-15 20:09:26.202409 gs-dbs-client-0.2.6.post8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-09-15 20:09:26.194279 gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/
--rw-rw-rw-   0        0        0     1306 2022-09-15 20:09:25.000000 gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2022-09-15 20:09:26.000000 gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-15 20:09:26.000000 gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-09-15 20:09:26.000000 gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2022-09-15 20:09:26.000000 gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-15 20:09:26.000000 gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-15 20:09:26.201409 gs-dbs-client-0.2.6.post8/gsdbs/
--rw-rw-rw-   0        0        0    23124 2022-09-15 20:09:24.000000 gs-dbs-client-0.2.6.post8/gsdbs/dbclient.py
--rw-rw-rw-   0        0        0     2357 2022-08-12 15:35:43.000000 gs-dbs-client-0.2.6.post8/gsdbs/gsfilter.py
--rw-rw-rw-   0        0        0    17860 2022-08-12 11:04:46.000000 gs-dbs-client-0.2.6.post8/gsdbs/missioncontrol.py
--rw-rw-rw-   0        0        0     1203 2022-09-15 09:15:12.000000 gs-dbs-client-0.2.6.post8/gsdbs/utils.py
--rw-rw-rw-   0        0        0       42 2022-09-15 20:09:26.203408 gs-dbs-client-0.2.6.post8/setup.cfg
--rw-rw-rw-   0        0        0     1429 2022-09-15 20:09:24.000000 gs-dbs-client-0.2.6.post8/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-16 08:43:06.478876 gs-dbs-client-0.2.6.post9/
+-rw-rw-rw-   0        0        0       19 2021-05-10 08:44:21.000000 gs-dbs-client-0.2.6.post9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1306 2022-09-16 08:43:06.477876 gs-dbs-client-0.2.6.post9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-09-16 08:43:06.464876 gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/
+-rw-rw-rw-   0        0        0     1306 2022-09-16 08:43:06.000000 gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2022-09-16 08:43:06.000000 gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-16 08:43:06.000000 gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2022-09-16 08:43:06.000000 gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2022-09-16 08:43:06.000000 gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-09-16 08:43:06.000000 gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-16 08:43:06.476877 gs-dbs-client-0.2.6.post9/gsdbs/
+-rw-rw-rw-   0        0        0    23124 2022-09-16 08:43:04.000000 gs-dbs-client-0.2.6.post9/gsdbs/dbclient.py
+-rw-rw-rw-   0        0        0     2357 2022-08-12 15:35:43.000000 gs-dbs-client-0.2.6.post9/gsdbs/gsfilter.py
+-rw-rw-rw-   0        0        0    17860 2022-08-12 11:04:46.000000 gs-dbs-client-0.2.6.post9/gsdbs/missioncontrol.py
+-rw-rw-rw-   0        0        0     1388 2022-09-16 08:42:48.000000 gs-dbs-client-0.2.6.post9/gsdbs/utils.py
+-rw-rw-rw-   0        0        0       42 2022-09-16 08:43:06.478876 gs-dbs-client-0.2.6.post9/setup.cfg
+-rw-rw-rw-   0        0        0     1429 2022-09-16 08:43:04.000000 gs-dbs-client-0.2.6.post9/setup.py
```

### Comparing `gs-dbs-client-0.2.6.post8/PKG-INFO` & `gs-dbs-client-0.2.6.post9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-dbs-client
-Version: 0.2.6.post8
+Version: 0.2.6.post9
 Summary: python wrapper for the Glass Sphere DBS
 Home-page: https://glass-sphere-ai.de
 Author: Glass Sphere Software
 Author-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gs-dbs-client-0.2.6.post8/gs_dbs_client.egg-info/PKG-INFO` & `gs-dbs-client-0.2.6.post9/gs_dbs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-dbs-client
-Version: 0.2.6.post8
+Version: 0.2.6.post9
 Summary: python wrapper for the Glass Sphere DBS
 Home-page: https://glass-sphere-ai.de
 Author: Glass Sphere Software
 Author-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gs-dbs-client-0.2.6.post8/gsdbs/dbclient.py` & `gs-dbs-client-0.2.6.post9/gsdbs/dbclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from gql import gql, Client
 from gql.transport.aiohttp import AIOHTTPTransport
 import pandas as pd
 
 
 class GSDBS:
     def __init__(self, creadPath, configstr=""):
-        self.version = "0.2.6-8"
+        self.version = "0.2.6-9"
         self._logger = logging.getLogger(__name__)
         self.credentials = None
         self.accessToken = None
         self.dtablename = None
         self.superdtablename = None
         self.sriBuildInfo = list()
         self.data = pd.DataFrame()
```

### Comparing `gs-dbs-client-0.2.6.post8/gsdbs/gsfilter.py` & `gs-dbs-client-0.2.6.post9/gsdbs/gsfilter.py`

 * *Files identical despite different names*

### Comparing `gs-dbs-client-0.2.6.post8/gsdbs/missioncontrol.py` & `gs-dbs-client-0.2.6.post9/gsdbs/missioncontrol.py`

 * *Files identical despite different names*

### Comparing `gs-dbs-client-0.2.6.post8/gsdbs/utils.py` & `gs-dbs-client-0.2.6.post9/gsdbs/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,7 +33,13 @@
     return frame.tobytes(), frame.shape[0], frame.shape[1], frame.shape[2]
 
 
 def gsBytesToNPArray(frame):
     nparray = np.frombuffer(frame[0], dtype=np.uint8)
     nparray.shape = (int(frame[1]), int(frame[2]), int(frame[3]))
     return nparray
+
+
+def handleparametermissing(request, *args):
+    for parameter in args:
+        if request.get(parameter) is None:
+            raise ValueError('Missing paramter: ' + parameter)
```

### Comparing `gs-dbs-client-0.2.6.post8/setup.py` & `gs-dbs-client-0.2.6.post9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="gs-dbs-client",
-    version="0.2.6-8",
+    version="0.2.6-9",
     description="python wrapper for the Glass Sphere DBS",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://glass-sphere-ai.de",
     author="Glass Sphere Software",
     author_email="",
     license="MIT",
```

