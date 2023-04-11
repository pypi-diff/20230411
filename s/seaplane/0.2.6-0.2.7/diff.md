# Comparing `tmp/seaplane-0.2.6.tar.gz` & `tmp/seaplane-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.2.6.tar", max compression
+gzip compressed data, was "seaplane-0.2.7.tar", max compression
```

## Comparing `seaplane-0.2.6.tar` & `seaplane-0.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1538 2023-04-06 23:53:57.317488 seaplane-0.2.6/README.md
--rw-r--r--   0        0        0     2452 2023-04-06 23:53:57.317488 seaplane-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      899 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/__init__.py
--rw-r--r--   0        0        0       84 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/__init__.py
--rw-r--r--   0        0        0      527 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/api_http.py
--rw-r--r--   0        0        0     2018 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/api_request.py
--rw-r--r--   0        0        0     2987 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/compute_api.py
--rw-r--r--   0        0        0     3158 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/formation_configuration_api.py
--rw-r--r--   0        0        0     7410 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/lock_api.py
--rw-r--r--   0        0        0     5806 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/metadata_api.py
--rw-r--r--   0        0        0     7724 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/restrict_api.py
--rw-r--r--   0        0        0     1520 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/sql_api.py
--rw-r--r--   0        0        0     3141 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/api/token_api.py
--rw-r--r--   0        0        0     5458 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/configuration.py
--rw-r--r--   0        0        0     1830 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/logging/__init__.py
--rw-r--r--   0        0        0      213 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/__init__.py
--rw-r--r--   0        0        0     1310 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/compute/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/compute/formation_configuration.py
--rw-r--r--   0        0        0      129 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/compute/formation_metadata.py
--rw-r--r--   0        0        0      436 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/errors.py
--rw-r--r--   0        0        0     3077 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/locks/__init__.py
--rw-r--r--   0        0        0     3560 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/metadata/__init__.py
--rw-r--r--   0        0        0      422 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/provider.py
--rw-r--r--   0        0        0      478 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/region.py
--rw-r--r--   0        0        0     4221 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/restrict/__init__.py
--rw-r--r--   0        0        0      386 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/model/sql/__init__.py
--rw-r--r--   0        0        0      424 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/util/__init__.py
--rw-r--r--   0        0        0      318 2023-04-06 23:53:57.317488 seaplane-0.2.6/src/seaplane/util/base64url.py
--rw-r--r--   0        0        0     2882 2023-04-06 23:54:08.858218 seaplane-0.2.6/setup.py
--rw-r--r--   0        0        0     2897 2023-04-06 23:54:08.858574 seaplane-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-04-11 18:08:47.163341 seaplane-0.2.7/README.md
+-rw-r--r--   0        0        0     2452 2023-04-11 18:08:47.163341 seaplane-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      899 2023-04-11 18:08:47.163341 seaplane-0.2.7/src/seaplane/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-11 18:08:47.163341 seaplane-0.2.7/src/seaplane/api/__init__.py
+-rw-r--r--   0        0        0      527 2023-04-11 18:08:47.163341 seaplane-0.2.7/src/seaplane/api/api_http.py
+-rw-r--r--   0        0        0     2018 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/api_request.py
+-rw-r--r--   0        0        0     2987 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/compute_api.py
+-rw-r--r--   0        0        0     3158 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/formation_configuration_api.py
+-rw-r--r--   0        0        0     7410 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/lock_api.py
+-rw-r--r--   0        0        0     5806 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/metadata_api.py
+-rw-r--r--   0        0        0     7724 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/restrict_api.py
+-rw-r--r--   0        0        0     1552 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/sql_api.py
+-rw-r--r--   0        0        0     3141 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/api/token_api.py
+-rw-r--r--   0        0        0     5458 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/configuration.py
+-rw-r--r--   0        0        0     1830 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/logging/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/__init__.py
+-rw-r--r--   0        0        0     1310 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/compute/__init__.py
+-rw-r--r--   0        0        0     1539 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/compute/formation_configuration.py
+-rw-r--r--   0        0        0      129 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/compute/formation_metadata.py
+-rw-r--r--   0        0        0      436 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/errors.py
+-rw-r--r--   0        0        0     3077 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/locks/__init__.py
+-rw-r--r--   0        0        0     3560 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/metadata/__init__.py
+-rw-r--r--   0        0        0      422 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/provider.py
+-rw-r--r--   0        0        0      478 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/region.py
+-rw-r--r--   0        0        0     4221 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/restrict/__init__.py
+-rw-r--r--   0        0        0      530 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/model/sql/__init__.py
+-rw-r--r--   0        0        0      424 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/util/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-11 18:08:47.167341 seaplane-0.2.7/src/seaplane/util/base64url.py
+-rw-r--r--   0        0        0     2882 2023-04-11 18:09:00.394400 seaplane-0.2.7/setup.py
+-rw-r--r--   0        0        0     2897 2023-04-11 18:09:00.394752 seaplane-0.2.7/PKG-INFO
```

### Comparing `seaplane-0.2.6/README.md` & `seaplane-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/pyproject.toml` & `seaplane-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.2.6"
+version = "0.2.7"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
```

### Comparing `seaplane-0.2.6/src/seaplane/__init__.py` & `seaplane-0.2.7/src/seaplane/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/api_http.py` & `seaplane-0.2.7/src/seaplane/api/api_http.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/api_request.py` & `seaplane-0.2.7/src/seaplane/api/api_request.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/compute_api.py` & `seaplane-0.2.7/src/seaplane/api/compute_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/formation_configuration_api.py` & `seaplane-0.2.7/src/seaplane/api/formation_configuration_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/lock_api.py` & `seaplane-0.2.7/src/seaplane/api/lock_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/metadata_api.py` & `seaplane-0.2.7/src/seaplane/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/restrict_api.py` & `seaplane-0.2.7/src/seaplane/api/restrict_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/api/sql_api.py` & `seaplane-0.2.7/src/seaplane/api/sql_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 import requests
 
 from ..configuration import Configuration, config
-from ..model.sql import CreatedDatabase, to_created_database
+from ..model.sql import CreatedDatabase, to_created_database, to_list_databases
 from ..util import unwrap
 from .api_http import headers
 from .api_request import provision_req
 
 
 class GlobalSQL:
     """
@@ -43,9 +43,9 @@
         list[database_name: str]
             Returns a list of database names if successful or it will raise an HTTPError otherwise.
         """
 
         return unwrap(
             self.req(
                 lambda access_token: requests.get(self.url, headers=headers(access_token))
-            ).map(lambda databases: list(databases))
+            ).map(lambda databases: to_list_databases(databases))
         )
```

### Comparing `seaplane-0.2.6/src/seaplane/api/token_api.py` & `seaplane-0.2.7/src/seaplane/api/token_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/configuration.py` & `seaplane-0.2.7/src/seaplane/configuration.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/logging/__init__.py` & `seaplane-0.2.7/src/seaplane/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/model/compute/__init__.py` & `seaplane-0.2.7/src/seaplane/model/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/model/compute/formation_configuration.py` & `seaplane-0.2.7/src/seaplane/model/compute/formation_configuration.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/model/locks/__init__.py` & `seaplane-0.2.7/src/seaplane/model/locks/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/model/metadata/__init__.py` & `seaplane-0.2.7/src/seaplane/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/src/seaplane/model/restrict/__init__.py` & `seaplane-0.2.7/src/seaplane/model/restrict/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.6/setup.py` & `seaplane-0.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'tomli==2.0.1',
  'types-requests>=2.28.0,<3.0.0',
  'types-simplejson>=3.17.7,<4.0.0',
  'urllib3==1.26.9']
 
 setup_kwargs = {
     'name': 'seaplane',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'Seaplane Python SDK',
     'long_description': '# Seaplane Python SDK\n[![PyPI](https://badge.fury.io/py/seaplane.svg)](https://badge.fury.io/py/seaplane)\n[![Python](https://img.shields.io/pypi/pyversions/seaplane.svg?style=plastic)](https://badge.fury.io/py/seaplane)\n\nSimple Python library to manage your resources at seaplane.\n\n## What is Seaplane?\n\nSeaplane is the global platform for building and scaling your application stack\nwithout the complexity of managing cloud infrastructure.\n\nIt serves as a reference application for how our APIs can be utilized.\n\nNot sure where to go to quickly run a workload on Seaplane? See our [Getting\nStarted] guide.\n\nTo build and test this software yourself, see the CONTRIBUTING document that is a peer to this one.\n\n## Installation\n\n```shell\npip install seaplane\n```\n\n## Configure your API KEY\n\n* Set `SEAPLANE_API_KEY` environment variable.\n* Use `config` object in order to set the api key.\n\n```python\nfrom seaplane import sea\n\nsea.config.set_api_key("your_api_key")\n```\n\n## License\n\nLicensed under the Apache License, Version 2.0, [LICENSE]. Copyright 2022 Seaplane IO, Inc.\n\n[//]: # (Links)\n\n[Seaplane]: https://seaplane.io/\n[CLI]: https://github.com/seaplane-io/seaplane/tree/main/seaplane-cli\n[SDK]: https://github.com/seaplane-io/seaplane/tree/main/seaplane\n[Getting Started]: https://github.com/seaplane-io/seaplane/blob/main/seaplane-sdk/python/docs/quickstart.md\n[CONTRIBUTING]: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python/CONTRIBUTIONS.md\n[LICENSE]: https://github.com/seaplane-io/seaplane/blob/main/LICENSE\n',
     'author': 'Seaplane IO, Inc.',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python',
```

### Comparing `seaplane-0.2.6/PKG-INFO` & `seaplane-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.2.6
+Version: 0.2.7
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

