# Comparing `tmp/mdast_cli-2023.4.2.tar.gz` & `tmp/mdast_cli-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli-2023.4.2.tar", last modified: Fri Apr  7 19:29:33 2023, max compression
+gzip compressed data, was "mdast_cli-2023.4.3.tar", last modified: Tue Apr 11 07:30:15 2023, max compression
```

## Comparing `mdast_cli-2023.4.2.tar` & `mdast_cli-2023.4.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.656478 mdast_cli-2023.4.2/mdast_cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3714 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/app_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appgallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
--rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
--rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/store.py
--rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/firebase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/google_play.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/config.py
--rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/device.properties
--rw-r--r--   0 runner    (1001) docker     (122)    15468 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay.py
--rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/rustore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/mdast_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/helpers/const.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/mdast_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.656478 mdast_cli-2023.4.2/mdast_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/token.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.486710 mdast_cli-2023.4.3/mdast_cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3589 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/app_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appgallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/google_play.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/device.properties
+-rw-r--r--   0 runner    (1001) docker     (122)    15468 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/rustore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/mdast_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/helpers/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/mdast_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/setup.py
```

### Comparing `mdast_cli-2023.4.2/PKG-INFO` & `mdast_cli-2023.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast_cli
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.4.2/README.md` & `mdast_cli-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/app_center.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/app_center.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 f' Request return status code: {response.status_code}')
 
         result = response.json()
         return result
 
     def get_version_info(self, owner_name, app_identifier, app_version=None, app_id=None):
         if not app_version and not app_id:
-            raise 'One of properties AppVersion or AppID should be set'
+            raise ValueError('One of properties AppVersion or AppID should be set')
 
         if app_id:
             return self.get_version_info_by_id(owner_name, app_identifier, app_id)
 
         return self.get_version_info_by_version(owner_name, app_identifier, app_version)
 
     def get_version_info_by_id(self, owner_name, app_identifier, app_id):
@@ -59,22 +59,18 @@
         for version in versions_info:
             if version['version'] != app_version:
                 continue
 
             version_info = self.get_version_info_by_id(owner_name, app_identifier, version['id'])
             return version_info
 
-        return None
+        raise RuntimeError(f'AppCenter - Cannot find version {app_version}')
 
     def download_app(self, download_path, owner_name, app_identifier, app_version=None, app_id=None):
         version_info = self.get_version_info(owner_name, app_identifier, app_version, app_id)
-        if not version_info:
-            logger.error('AppCenter - Failed to get app version information.'
-                         ' Verify that you set up arguments correctly and try again')
-
         logger.info('AppCenter - Start download application')
         download_url = version_info.get('download_url')
 
         response = requests.get(download_url, headers=self.auth_header, allow_redirects=True)
         if response.status_code != 200:
             raise RuntimeError(f'AppCenter - Failed to download application. '
                                f'Request return status code: {response.status_code}')
```

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appgallery.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appgallery.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
             logger.info(f"Appgallery - Successfully found app with id: {app_id}, "
                         f"package name: {app_info['package_name']},"
                         f" version:{app_info['version_name']},"
                         f" name: {app_info['name']}")
             return app_info
 
+    raise RuntimeError(f'Appgallery - Cannot find application {app_id}')
+
 
 def appgallery_download_app(app_id, download_path, file_name=None):
     logger.info(f'Appgallery - Try to download application with id {app_id}')
     app_info = get_app_info(app_id)
     r = requests.get(f'https://appgallery.cloud.huawei.com/appdl/{app_id}')
     if r.status_code != 200:
         raise RuntimeError(f'Appgallery - Failed to download application. '
```

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/store.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/store.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/firebase.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/firebase.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/google_play.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/google_play.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/config.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/config.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/device.properties` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/device.properties`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus2.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/distribution_systems/rustore.py` & `mdast_cli-2023.4.3/mdast_cli/distribution_systems/rustore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/helpers/const.py` & `mdast_cli-2023.4.3/mdast_cli/helpers/const.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli/mdast_scan.py` & `mdast_cli-2023.4.3/mdast_cli/mdast_scan.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli.egg-info/PKG-INFO` & `mdast_cli-2023.4.3/mdast_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast-cli
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.4.2/mdast_cli.egg-info/SOURCES.txt` & `mdast_cli-2023.4.3/mdast_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli.egg-info/requires.txt` & `mdast_cli-2023.4.3/mdast_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli_core/api.py` & `mdast_cli-2023.4.3/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli_core/base.py` & `mdast_cli-2023.4.3/mdast_cli_core/base.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/mdast_cli_core/token.py` & `mdast_cli-2023.4.3/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.2/setup.py` & `mdast_cli-2023.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli",
 
 
-    version='2023.04.02',
+    version='2023.04.03',
 
 
 
     author="Dynamic-Mobile-Security",
     description="Dynamic-Mobile-Security",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

