# Comparing `tmp/frigidaire-0.7.tar.gz` & `tmp/frigidaire-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frigidaire-0.7.tar", last modified: Wed May 26 20:13:52 2021, max compression
+gzip compressed data, was "frigidaire-0.8.tar", last modified: Wed May 26 22:43:39 2021, max compression
```

## Comparing `frigidaire-0.7.tar` & `frigidaire-0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-26 20:13:52.649825 frigidaire-0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-05-26 20:13:43.000000 frigidaire-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-05-26 20:13:52.649825 frigidaire-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-05-26 20:13:43.000000 frigidaire-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-26 20:13:52.649825 frigidaire-0.7/frigidaire/
--rw-r--r--   0 runner    (1001) docker     (121)    11896 2021-05-26 20:13:43.000000 frigidaire-0.7/frigidaire/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-26 20:13:52.649825 frigidaire-0.7/frigidaire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-05-26 20:13:52.000000 frigidaire-0.7/frigidaire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-05-26 20:13:52.000000 frigidaire-0.7/frigidaire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-26 20:13:52.000000 frigidaire-0.7/frigidaire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-05-26 20:13:52.000000 frigidaire-0.7/frigidaire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-26 20:13:52.649825 frigidaire-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-05-26 20:13:43.000000 frigidaire-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-26 22:43:39.409874 frigidaire-0.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-05-26 22:43:27.000000 frigidaire-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2021-05-26 22:43:39.409874 frigidaire-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-05-26 22:43:27.000000 frigidaire-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-26 22:43:39.409874 frigidaire-0.8/frigidaire/
+-rw-r--r--   0 runner    (1001) docker     (121)    12954 2021-05-26 22:43:27.000000 frigidaire-0.8/frigidaire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-26 22:43:39.409874 frigidaire-0.8/frigidaire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2021-05-26 22:43:39.000000 frigidaire-0.8/frigidaire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-05-26 22:43:39.000000 frigidaire-0.8/frigidaire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-26 22:43:39.000000 frigidaire-0.8/frigidaire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-05-26 22:43:39.000000 frigidaire-0.8/frigidaire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-26 22:43:39.409874 frigidaire-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2021-05-26 22:43:27.000000 frigidaire-0.8/setup.py
```

### Comparing `frigidaire-0.7/LICENSE` & `frigidaire-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `frigidaire-0.7/PKG-INFO` & `frigidaire-0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frigidaire
-Version: 0.7
+Version: 0.8
 Summary: Python API for the Frigidaire 2.0 App
 Home-page: https://github.com/bm1549/frigidaire
 Author: Brian Marks
 License: UNKNOWN
 Description: # Frigidaire Python API
         
         This is an API wrapper written in Python around the Frigidaire 2.0 App.
```

### Comparing `frigidaire-0.7/frigidaire/__init__.py` & `frigidaire-0.8/frigidaire/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -142,14 +142,15 @@
     OFF = 0
     COOL = 1
     FAN = 3
     ECO = 4
 
 
 class FanSpeed(Enum):
+    OFF = 0
     LOW = 1
     MEDIUM = 2
     HIGH = 4
     AUTO = 7
 
 
 class Action:
@@ -240,60 +241,82 @@
         if not auth_response.get('sessionKey'):
             raise FrigidaireException(f'Failed to authenticate, sessionKey was not in response: {auth_response}')
 
         logging.debug('Authentication successful, storing new session key')
 
         self.session_key: Optional[str] = auth_response['sessionKey']
 
-    def get_appliances(self) -> List[Appliance]:
+    def re_authenticate(self) -> None:
         """
-        Uses the Frigidaire API to fetch the list of appliances.
-        Will authenticate if not already authenticated.
-        :return: The appliances that are associated with the Frigidaire account
+        Removes the session_key and tries to authenticate again
+        :return:
         """
+        self.session_key = None
         self.authenticate()
 
+    def get_appliances(self) -> List[Appliance]:
+        """
+        Uses the Frigidaire API to fetch the list of appliances
+        Will authenticate if the request fails
+        :return: The appliances that are associated with the Frigidaire account
+        """
         logging.debug('Listing appliances')
-        appliances = self.get_request(
-            f'/user-appliance-reg/users/{self.username}/appliances?country=US&includeFields=false'
-        )
-        return list(map(Appliance, appliances))
+
+        try:
+            appliances = self.get_request(
+                f'/user-appliance-reg/users/{self.username}/appliances?country=US&includeFields=false'
+            )
+            return list(map(Appliance, appliances))
+        except FrigidaireException:
+            logging.debug('Listing appliances failed - attempting to re-authenticate')
+            self.re_authenticate()
+            appliances = self.get_request(
+                f'/user-appliance-reg/users/{self.username}/appliances?country=US&includeFields=false'
+            )
+            return list(map(Appliance, appliances))
 
     def get_appliance_details(self, appliance: Appliance) -> ApplianceDetails:
         """
         Uses the Frigidaire API to fetch details for a given appliance
-        Will authenticate if not already authenticated
+        Will authenticate if the request fails
         :param appliance: The appliance to request from the API
         :return: The details for the passed in appliance
         """
-        self.authenticate()
+        logging.debug(f'Getting appliance details for appliance {appliance.nickname}')
 
-        details = self.get_request(f'/elux-ms/appliances/latest?{appliance.query_string}&includeSubcomponents=true')
-        return ApplianceDetails(list(map(ApplianceDetail, details)))
+        try:
+            details = self.get_request(f'/elux-ms/appliances/latest?{appliance.query_string}&includeSubcomponents=true')
+            return ApplianceDetails(list(map(ApplianceDetail, details)))
+        except FrigidaireException:
+            self.re_authenticate()
+            details = self.get_request(f'/elux-ms/appliances/latest?{appliance.query_string}&includeSubcomponents=true')
+            return ApplianceDetails(list(map(ApplianceDetail, details)))
 
     def execute_action(self, appliance: Appliance, action: List[Component]) -> None:
         """
         Executes any defined action on a given appliance
-        Will authenticate if not already authenticated
+        Will authenticate if the request fails
         :param appliance: The appliance to perform the action on
         :param action: The action to be performed
         :return:
         """
-        self.authenticate()
-
         data = {
             'components': action,
             'timestamp': str(int(time.time())),
             'operationMode': 'EXE',
             'version': 'ad',
             'source': 'RP1',
             'destination': 'AC1',
         }
 
-        self.post_request(f'/commander/remote/sendjson?{appliance.query_string}', data)
+        try:
+            self.post_request(f'/commander/remote/sendjson?{appliance.query_string}', data)
+        except FrigidaireException:
+            self.re_authenticate()
+            self.post_request(f'/commander/remote/sendjson?{appliance.query_string}', data)
 
     @property
     def headers(self):
         """
         Generates the headers that should be sent on every request to the Frigidaire API
         :return:
         """
```

### Comparing `frigidaire-0.7/frigidaire.egg-info/PKG-INFO` & `frigidaire-0.8/frigidaire.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frigidaire
-Version: 0.7
+Version: 0.8
 Summary: Python API for the Frigidaire 2.0 App
 Home-page: https://github.com/bm1549/frigidaire
 Author: Brian Marks
 License: UNKNOWN
 Description: # Frigidaire Python API
         
         This is an API wrapper written in Python around the Frigidaire 2.0 App.
```

### Comparing `frigidaire-0.7/setup.py` & `frigidaire-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='frigidaire',
-    version='0.7',
+    version='0.8',
     author="Brian Marks",
     description="Python API for the Frigidaire 2.0 App",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bm1549/frigidaire",
     packages=setuptools.find_packages(),
     classifiers=[
```

