# Comparing `tmp/asconnect-2.2.8.tar.gz` & `tmp/asconnect-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asconnect-2.2.8.tar", max compression
+gzip compressed data, was "asconnect-2.2.9.tar", max compression
```

## Comparing `asconnect-2.2.8.tar` & `asconnect-2.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1141 2020-09-30 13:33:16.848652 asconnect-2.2.8/LICENSE
--rw-r--r--   0        0        0     4502 2021-07-08 12:23:19.634821 asconnect-2.2.8/README.md
--rwxr-xr-x   0        0        0      297 2020-10-16 13:31:57.508255 asconnect-2.2.8/asconnect/__init__.py
--rw-r--r--   0        0        0     3165 2022-01-25 09:30:52.395345 asconnect-2.2.8/asconnect/altool.py
--rwxr-xr-x   0        0        0     3406 2021-07-08 12:24:00.974744 asconnect-2.2.8/asconnect/app_client.py
--rwxr-xr-x   0        0        0     5930 2021-07-08 12:23:27.324782 asconnect-2.2.8/asconnect/app_info_client.py
--rwxr-xr-x   0        0        0    10487 2021-07-08 12:23:27.323700 asconnect-2.2.8/asconnect/beta_review_client.py
--rwxr-xr-x   0        0        0     6296 2022-01-25 09:30:52.436718 asconnect-2.2.8/asconnect/build_client.py
--rwxr-xr-x   0        0        0     2301 2021-11-23 15:48:57.548392 asconnect-2.2.8/asconnect/client.py
--rw-r--r--   0        0        0     1301 2021-09-15 10:35:15.311279 asconnect-2.2.8/asconnect/exceptions.py
--rwxr-xr-x   0        0        0    12681 2021-11-25 15:58:40.305681 asconnect-2.2.8/asconnect/httpclient.py
--rw-r--r--   0        0        0      537 2021-10-05 12:17:03.862444 asconnect-2.2.8/asconnect/models/__init__.py
--rw-r--r--   0        0        0     2166 2021-07-08 12:38:54.734204 asconnect-2.2.8/asconnect/models/app_info.py
--rw-r--r--   0        0        0     4313 2021-07-08 12:39:08.683657 asconnect-2.2.8/asconnect/models/app_store.py
--rw-r--r--   0        0        0      903 2021-07-08 12:39:02.519876 asconnect-2.2.8/asconnect/models/app_store_version_localizations.py
--rw-r--r--   0        0        0     2721 2021-07-08 12:39:33.172840 asconnect-2.2.8/asconnect/models/apps.py
--rw-r--r--   0        0        0     1178 2021-07-08 12:39:40.941398 asconnect-2.2.8/asconnect/models/beta_app_review.py
--rw-r--r--   0        0        0     1866 2021-07-08 12:39:48.437450 asconnect-2.2.8/asconnect/models/beta_detail.py
--rw-r--r--   0        0        0     1277 2021-07-08 12:39:56.175568 asconnect-2.2.8/asconnect/models/beta_groups.py
--rw-r--r--   0        0        0     1225 2021-07-08 12:40:04.219871 asconnect-2.2.8/asconnect/models/builds.py
--rw-r--r--   0        0        0     1221 2021-07-08 12:38:40.406073 asconnect-2.2.8/asconnect/models/common.py
--rw-r--r--   0        0        0      978 2021-07-08 12:40:20.452423 asconnect-2.2.8/asconnect/models/idfa.py
--rw-r--r--   0        0        0     1373 2021-07-08 12:40:27.075321 asconnect-2.2.8/asconnect/models/localization.py
--rw-r--r--   0        0        0     4280 2021-07-08 12:40:45.165084 asconnect-2.2.8/asconnect/models/screenshots.py
--rw-r--r--   0        0        0     1364 2021-10-19 11:02:07.515543 asconnect-2.2.8/asconnect/models/users.py
--rwxr-xr-x   0        0        0     9963 2021-09-15 10:35:37.326234 asconnect-2.2.8/asconnect/screenshot_client.py
--rw-r--r--   0        0        0      352 2021-07-08 12:20:48.317779 asconnect-2.2.8/asconnect/sorting.py
--rwxr-xr-x   0        0        0     1216 2021-10-19 11:02:40.906719 asconnect-2.2.8/asconnect/users_client.py
--rw-r--r--   0        0        0     2170 2020-10-16 13:25:57.722356 asconnect-2.2.8/asconnect/utilities.py
--rwxr-xr-x   0        0        0    15343 2021-09-15 09:47:55.803065 asconnect-2.2.8/asconnect/version_client.py
--rw-r--r--   0        0        0     1125 2022-01-25 09:31:35.471858 asconnect-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     5427 2022-01-25 09:31:48.287580 asconnect-2.2.8/setup.py
--rw-r--r--   0        0        0     5663 2022-01-25 09:31:48.287982 asconnect-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1141 2020-09-30 13:33:16.848652 asconnect-2.2.9/LICENSE
+-rw-r--r--   0        0        0     4502 2021-07-08 12:23:19.634821 asconnect-2.2.9/README.md
+-rwxr-xr-x   0        0        0      297 2020-10-16 13:31:57.508255 asconnect-2.2.9/asconnect/__init__.py
+-rw-r--r--   0        0        0     3165 2022-01-25 09:30:52.395345 asconnect-2.2.9/asconnect/altool.py
+-rwxr-xr-x   0        0        0     3406 2021-07-08 12:24:00.974744 asconnect-2.2.9/asconnect/app_client.py
+-rwxr-xr-x   0        0        0     5930 2021-07-08 12:23:27.324782 asconnect-2.2.9/asconnect/app_info_client.py
+-rwxr-xr-x   0        0        0    10487 2021-07-08 12:23:27.323700 asconnect-2.2.9/asconnect/beta_review_client.py
+-rwxr-xr-x   0        0        0     6296 2022-01-25 09:30:52.436718 asconnect-2.2.9/asconnect/build_client.py
+-rwxr-xr-x   0        0        0     2301 2021-11-23 15:48:57.548392 asconnect-2.2.9/asconnect/client.py
+-rw-r--r--   0        0        0     1301 2021-09-15 10:35:15.311279 asconnect-2.2.9/asconnect/exceptions.py
+-rwxr-xr-x   0        0        0    12681 2021-11-25 15:58:40.305681 asconnect-2.2.9/asconnect/httpclient.py
+-rw-r--r--   0        0        0      537 2021-10-05 12:17:03.862444 asconnect-2.2.9/asconnect/models/__init__.py
+-rw-r--r--   0        0        0     2166 2021-07-08 12:38:54.734204 asconnect-2.2.9/asconnect/models/app_info.py
+-rw-r--r--   0        0        0     4313 2021-07-08 12:39:08.683657 asconnect-2.2.9/asconnect/models/app_store.py
+-rw-r--r--   0        0        0      903 2021-07-08 12:39:02.519876 asconnect-2.2.9/asconnect/models/app_store_version_localizations.py
+-rw-r--r--   0        0        0     2721 2021-07-08 12:39:33.172840 asconnect-2.2.9/asconnect/models/apps.py
+-rw-r--r--   0        0        0     1178 2021-07-08 12:39:40.941398 asconnect-2.2.9/asconnect/models/beta_app_review.py
+-rw-r--r--   0        0        0     1866 2021-07-08 12:39:48.437450 asconnect-2.2.9/asconnect/models/beta_detail.py
+-rw-r--r--   0        0        0     1277 2021-07-08 12:39:56.175568 asconnect-2.2.9/asconnect/models/beta_groups.py
+-rw-r--r--   0        0        0     1225 2021-07-08 12:40:04.219871 asconnect-2.2.9/asconnect/models/builds.py
+-rw-r--r--   0        0        0     1221 2021-07-08 12:38:40.406073 asconnect-2.2.9/asconnect/models/common.py
+-rw-r--r--   0        0        0      978 2021-07-08 12:40:20.452423 asconnect-2.2.9/asconnect/models/idfa.py
+-rw-r--r--   0        0        0     1373 2021-07-08 12:40:27.075321 asconnect-2.2.9/asconnect/models/localization.py
+-rw-r--r--   0        0        0     4280 2021-07-08 12:40:45.165084 asconnect-2.2.9/asconnect/models/screenshots.py
+-rw-r--r--   0        0        0     1364 2021-10-19 11:02:07.515543 asconnect-2.2.9/asconnect/models/users.py
+-rwxr-xr-x   0        0        0     9963 2021-09-15 10:35:37.326234 asconnect-2.2.9/asconnect/screenshot_client.py
+-rw-r--r--   0        0        0      352 2021-07-08 12:20:48.317779 asconnect-2.2.9/asconnect/sorting.py
+-rwxr-xr-x   0        0        0     1216 2021-10-19 11:02:40.906719 asconnect-2.2.9/asconnect/users_client.py
+-rw-r--r--   0        0        0     2170 2020-10-16 13:25:57.722356 asconnect-2.2.9/asconnect/utilities.py
+-rwxr-xr-x   0        0        0    15965 2022-02-28 09:26:20.342765 asconnect-2.2.9/asconnect/version_client.py
+-rw-r--r--   0        0        0     1125 2022-02-28 09:26:31.683491 asconnect-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5427 2022-02-28 09:26:55.356837 asconnect-2.2.9/setup.py
+-rw-r--r--   0        0        0     5663 2022-02-28 09:26:55.357365 asconnect-2.2.9/PKG-INFO
```

### Comparing `asconnect-2.2.8/LICENSE` & `asconnect-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/README.md` & `asconnect-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/altool.py` & `asconnect-2.2.9/asconnect/altool.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/app_client.py` & `asconnect-2.2.9/asconnect/app_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/app_info_client.py` & `asconnect-2.2.9/asconnect/app_info_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/beta_review_client.py` & `asconnect-2.2.9/asconnect/beta_review_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/build_client.py` & `asconnect-2.2.9/asconnect/build_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/client.py` & `asconnect-2.2.9/asconnect/client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/exceptions.py` & `asconnect-2.2.9/asconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/httpclient.py` & `asconnect-2.2.9/asconnect/httpclient.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/__init__.py` & `asconnect-2.2.9/asconnect/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/app_info.py` & `asconnect-2.2.9/asconnect/models/app_info.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/app_store.py` & `asconnect-2.2.9/asconnect/models/app_store.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/app_store_version_localizations.py` & `asconnect-2.2.9/asconnect/models/app_store_version_localizations.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/apps.py` & `asconnect-2.2.9/asconnect/models/apps.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/beta_app_review.py` & `asconnect-2.2.9/asconnect/models/beta_app_review.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/beta_detail.py` & `asconnect-2.2.9/asconnect/models/beta_detail.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/beta_groups.py` & `asconnect-2.2.9/asconnect/models/beta_groups.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/builds.py` & `asconnect-2.2.9/asconnect/models/builds.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/common.py` & `asconnect-2.2.9/asconnect/models/common.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/idfa.py` & `asconnect-2.2.9/asconnect/models/idfa.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/localization.py` & `asconnect-2.2.9/asconnect/models/localization.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/screenshots.py` & `asconnect-2.2.9/asconnect/models/screenshots.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/models/users.py` & `asconnect-2.2.9/asconnect/models/users.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/screenshot_client.py` & `asconnect-2.2.9/asconnect/screenshot_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/users_client.py` & `asconnect-2.2.9/asconnect/users_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/utilities.py` & `asconnect-2.2.9/asconnect/utilities.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.8/asconnect/version_client.py` & `asconnect-2.2.9/asconnect/version_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 import logging
 from typing import Iterator, List, Optional
 
+from asconnect.exceptions import AppStoreConnectError
 from asconnect.httpclient import HttpClient
 from asconnect.models import (
     AppStoreVersion,
     AppStoreVersionPhasedRelease,
     PhasedReleaseState,
     Platform,
     AppStoreVersionLocalization,
@@ -417,27 +418,38 @@
             data_type=AppStoreVersion,
         )
 
     def submit_for_review(
         self,
         *,
         version_id: str,
+        attempt: int = 1,
+        max_attempts: int = 3,
     ) -> None:
         """Submit the version for review
 
         :param version_id: The ID of the version to submit for review
+        :param attempt: The attempt this is
+        :param max_attempts: The number of attempts allowed
         """
 
         self.log.info(f"Submitting version for review {version_id}")
 
-        self.http_client.post(
-            endpoint="appStoreVersionSubmissions",
-            data={
-                "data": {
+        try:
+            self.http_client.post(
+                endpoint="appStoreVersionSubmissions",
+                data={
+                    "data": {
                     "type": "appStoreVersionSubmissions",
                     "relationships": {
                         "appStoreVersion": {"data": {"type": "appStoreVersions", "id": version_id}}
                     },
                 }
             },
-            data_type=None,
-        )
+                data_type=None,
+            )
+        except AppStoreConnectError as ex:
+            if attempt < max_attempts and ex.response.status_code >= 500 and ex.response.status_code < 600:
+                self.log.info("Submit failed due to server-side intermittent issue. Will sleep for 1 minute and try again.")
+                time.sleep(60)
+                self.submit_for_review(version_id=version_id)
+
```

### Comparing `asconnect-2.2.8/pyproject.toml` & `asconnect-2.2.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asconnect"
-version = "2.2.8"
+version = "2.2.9"
 description = "A wrapper around the Apple App Store Connect APIs"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
```

### Comparing `asconnect-2.2.8/setup.py` & `asconnect-2.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'deserialize>=1.2.0,<2.0.0',
  'pyjwt>=1.7.0,<2.0.0',
  'requests>=2.20.0,<3.0.0',
  'tenacity>=6.2.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'asconnect',
-    'version': '2.2.8',
+    'version': '2.2.9',
     'description': 'A wrapper around the Apple App Store Connect APIs',
     'long_description': '# asconnect\n\nasconnect is a Python wrapper around the [Apple App Store Connect REST APIs](https://developer.apple.com/documentation/appstoreconnectapi).\n\nThis wrapper does not cover every API, but does cover the basics, including:\n\n* Uploading a build\n* Creating a new TestFlight version\n* Setting TestFlight review information\n* Creating a new app store version\n* Setting the app review information\n* Submitting for app review\n\n## Getting Started\n\n### Installation\n\nThe package is available on PyPI, so you can run `pip install asconnect` to get the latest version.\n\n### Creating a client\n\nTo begin, you need to [generate a key](https://developer.apple.com/documentation/appstoreconnectapi/creating_api_keys_for_app_store_connect_api), then get it\'s ID, the contents of the key itself, and the issuer ID.\n\nOnce you have those, you can create a new client by running:\n\n```python\nclient = asconnect.Client(key_id="...", key_contents="...", issuer_id="...")\n```\n\n### Getting your App\n\nMost operations require an app identifier. This is not the same as the bundle ID you choose, but is an ID generated by Apple. The easiest way to get this is to run this code:\n\n```python\napp = client.app.get_from_bundle_id("com.example.my_bundle_id")\n```\n\n### Uploading a Build\n\nUploading a build isn\'t technically part of the App Store Connect APIs, but a wrapper around altool is included to make things as easy as possible. Let\'s upload a build for your app:\n\n```python\nclient.build.upload(\n  ipa_path="/path/to/the/app.ipa",\n  platform=asconnect.Platform.ios,\n)\n```\n\nAnd if you want to wait for your build to finish processing:\n\n```python\nbuild = client.build.wait_for_build_to_process("com.example.my_bundle_id", build_number)\n```\n\n`build_number` is the build number you gave your build when you created it. It\'s used by the app store to identify the build.\n\n### App Store Submission\n\nLet\'s take that build, create a new app store version and submit it,\n\n```python\n# Create a new version\nversion = client.app.create_new_version(version="1.2.3", app_id=app.identifier)\n\n# Set the build for that version\nclient.version.set_build(version_id=version.identifier, build_id=build.identifier)\n\n# Submit for review\nclient.version.submit_for_review(version_id=version.identifier)\n```\n\nIt\'s that easy. Most of the time at least. If you don\'t have previous version to inherit information from you\'ll need to do things like set screenshots, reviewer info, etc. All of which is possible through this library.\n### Phased Distribution\n```python\n# Create a new version\nversion = client.app.create_new_version(version="1.2.3", app_id=app.identifier)\n\n# Start a versions\' phased release, the initial state of which is INACTIVE\nphased_release = client.version.create_phased_release(version_id=version.identifier)\n\n# Check on a phased release\nphased_release = client.version.get_phased_release(version_id=version.identifier)\n\n# Advance or modify a phased release\nphased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.active)\nphased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.pause)\nphased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.complete)\n\n# Delete\nclient.version.delete_phased_release(phased_release_id=phased_release.identifier)\n```\n# Getting Started\n\nFor development `asconnect` uses [`poetry`](https://github.com/python-poetry/poetry)\n\n# Contributing\n\nThis project welcomes contributions and suggestions.  Most contributions require you to agree to a\nContributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us\nthe rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.\n\nWhen you submit a pull request, a CLA bot will automatically determine whether you need to provide\na CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions\nprovided by the bot. You will only need to do this once across all repos using our CLA.\n\nThis project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).\nFor more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or\ncontact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.\n',
     'author': 'Dale Myers',
     'author_email': 'dalemy@microsoft.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/microsoft/asconnect',
```

### Comparing `asconnect-2.2.8/PKG-INFO` & `asconnect-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asconnect
-Version: 2.2.8
+Version: 2.2.9
 Summary: A wrapper around the Apple App Store Connect APIs
 Home-page: https://github.com/microsoft/asconnect
 License: MIT
 Keywords: apple,app store,itunes,connect
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
 Requires-Python: >=3.6.2,<4.0.0
```

