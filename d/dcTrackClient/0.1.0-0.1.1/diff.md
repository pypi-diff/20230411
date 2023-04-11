# Comparing `tmp/dctrackclient-0.1.0.tar.gz` & `tmp/dctrackclient-0.1.1.tar.gz`

## Comparing `dctrackclient-0.1.0.tar` & `dctrackclient-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/LICENSE
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dctrackclient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dctrackclient-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 dctrackclient-0.1.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.1.1/LICENSE
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dctrackclient-0.1.1/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dctrackclient-0.1.1/PKG-INFO
```

### Comparing `dctrackclient-0.1.0/.github/workflows/python-publish.yml` & `dctrackclient-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.1.0/src/dcTrackClient/__init__.py` & `dctrackclient-0.1.1/src/dcTrackClient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
         self.__BASE_URL = baseUrl
         self.__USERNAME = username
         self.__PASSWORD = password
         self.__APITOKEN = apiToken
 
     def __request(self, method: str, endpoint: str, body: dict = None):
         if self.__USERNAME and self.__PASSWORD:
-            return requests.request(method,  self.__BASE_URL + endpoint, json=body, auth=(self.__USERNAME, self.__PASSWORD)).json()
+            return requests.request(method,  self.__BASE_URL + '/' + endpoint, json=body, auth=(self.__USERNAME, self.__PASSWORD)).json()
         elif self.__APITOKEN:
-            return requests.request(method, self.__BASE_URL + endpoint, json=body, headers={'Authorization': 'Token ' + self.__APITOKEN}).json()
+            return requests.request(method, self.__BASE_URL + '/' + endpoint, json=body, headers={'Authorization': 'Token ' + self.__APITOKEN}).json()
         else:
             raise Exception('Undefined username/password or token.')
 
     # Manage Items
 
     def createItem(self, data: dict, returnDetails: bool = True):
         """Create a new item."""
```

### Comparing `dctrackclient-0.1.0/LICENSE` & `dctrackclient-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.1.0/pyproject.toml` & `dctrackclient-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.1.0/PKG-INFO` & `dctrackclient-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

