# Comparing `tmp/shopback_sdk-0.1.2b0.tar.gz` & `tmp/shopback_sdk-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopback_sdk-0.1.2b0.tar", max compression
+gzip compressed data, was "shopback_sdk-0.1.3b0.tar", max compression
```

## Comparing `shopback_sdk-0.1.2b0.tar` & `shopback_sdk-0.1.3b0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-04-04 14:29:34.546458 shopback_sdk-0.1.2b0/LICENSE
--rw-r--r--   0        0        0    12730 2023-04-04 14:29:34.546458 shopback_sdk-0.1.2b0/README.md
--rw-r--r--   0        0        0     3050 2023-04-04 14:29:34.546458 shopback_sdk-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0      350 2023-04-04 14:29:34.546458 shopback_sdk-0.1.2b0/shopback_sdk/__init__.py
--rw-r--r--   0        0        0     8324 2023-04-04 14:29:34.546458 shopback_sdk-0.1.2b0/shopback_sdk/old_client_sdk.py
--rw-r--r--   0        0        0     5455 2023-04-04 14:29:34.546458 shopback_sdk-0.1.2b0/shopback_sdk/products.py
--rw-r--r--   0        0        0    13716 1970-01-01 00:00:00.000000 shopback_sdk-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-11 17:23:30.908842 shopback_sdk-0.1.3b0/LICENSE
+-rw-r--r--   0        0        0    12741 2023-04-11 17:23:30.908842 shopback_sdk-0.1.3b0/README.md
+-rw-r--r--   0        0        0     3050 2023-04-11 17:23:30.908842 shopback_sdk-0.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0      350 2023-04-11 17:23:30.908842 shopback_sdk-0.1.3b0/shopback_sdk/__init__.py
+-rw-r--r--   0        0        0     8324 2023-04-11 17:23:30.908842 shopback_sdk-0.1.3b0/shopback_sdk/old_client_sdk.py
+-rw-r--r--   0        0        0     5605 2023-04-11 17:23:30.908842 shopback_sdk-0.1.3b0/shopback_sdk/products.py
+-rw-r--r--   0        0        0    13727 1970-01-01 00:00:00.000000 shopback_sdk-0.1.3b0/PKG-INFO
```

### Comparing `shopback_sdk-0.1.2b0/LICENSE` & `shopback_sdk-0.1.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `shopback_sdk-0.1.2b0/README.md` & `shopback_sdk-0.1.3b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # shopback-sdk
 
 <div align="center">
 
-[![Build status](https://github.com/ktsstudio/shopback-sdk/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ktsstudio/shopback-sdk/actions?query=workflow%3Abuild)
+[![Build status](https://github.com/ktsstudio/shopback-sdk/actions/workflows/build-publish.yml/badge.svg?event=push)](https://github.com/ktsstudio/shopback-sdk/actions/workflows/build-publish.yml)
 [![Python Version](https://img.shields.io/pypi/pyversions/shopback-sdk.svg)](https://pypi.org/project/shopback-sdk/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ktsstudio/shopback-sdk/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ktsstudio/shopback-sdk/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ktsstudio/shopback-sdk/releases)
```

### Comparing `shopback_sdk-0.1.2b0/pyproject.toml` & `shopback_sdk-0.1.3b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "shopback-sdk"
-version = "0.1.2b"
+version = "0.1.3b"
 description = "shopback.ru - no code shop constructor and cafe for telegram"
 readme = "README.md"
 authors = ["ktsstudio <hello@ktsstudio.com>"]
 license = "MIT"
 repository = "https://github.com/ktsstudio/shopback-sdk"
 homepage = "https://github.com/ktsstudio/shopback-sdk"
```

### Comparing `shopback_sdk-0.1.2b0/shopback_sdk/old_client_sdk.py` & `shopback_sdk-0.1.3b0/shopback_sdk/old_client_sdk.py`

 * *Files identical despite different names*

### Comparing `shopback_sdk-0.1.2b0/shopback_sdk/products.py` & `shopback_sdk-0.1.3b0/shopback_sdk/products.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 @dataclass
 class CategoryData:
     project_id: int
     name: str
     external_id: str
+    is_visible: bool = True
     attachment: Optional[int] = None
     parent_external_id: Optional[int] = None
 
 
 class ClientSDK:
     DEFAULT_URL = "https://shopback-prod.ru-prod2.kts.studio"
 
@@ -133,21 +134,23 @@
     def upload_category(self, category: CategoryData) -> dict:
         query = gql(
             """
             mutation category(
                 $project: String!,
                 $name: String,
                 $externalId: String!,
+                $isVisible: Boolean,
                 $attachment: String,
                 $parentExternalId: String
             ) {
               category(input: {
                 project: $project,
                 name: $name,
                 externalId: $externalId,
+                isVisible: $isVisible,
                 attachment: $attachment,
                 parentExternalId: $parentExternalId
               }) {
                 data {
                   id
                 },
                 errors {status, message, fieldProblems {fieldName, errDescription}}
@@ -155,12 +158,13 @@
             }
         """
         )
         params = {
             "project": str(category.project_id),
             "name": category.name,
             "externalId": category.external_id,
+            "isVisible": category.is_visible,
             "attachment": str(category.attachment) if category.attachment else "",
             "parentExternalId": category.parent_external_id or "",
         }
         result = self.client.execute(query, variable_values=params)
         return result
```

### Comparing `shopback_sdk-0.1.2b0/PKG-INFO` & `shopback_sdk-0.1.3b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopback-sdk
-Version: 0.1.2b0
+Version: 0.1.3b0
 Summary: shopback.ru - no code shop constructor and cafe for telegram
 Home-page: https://github.com/ktsstudio/shopback-sdk
 License: MIT
 Author: ktsstudio
 Author-email: hello@ktsstudio.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -22,15 +22,15 @@
 Project-URL: Repository, https://github.com/ktsstudio/shopback-sdk
 Description-Content-Type: text/markdown
 
 # shopback-sdk
 
 <div align="center">
 
-[![Build status](https://github.com/ktsstudio/shopback-sdk/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ktsstudio/shopback-sdk/actions?query=workflow%3Abuild)
+[![Build status](https://github.com/ktsstudio/shopback-sdk/actions/workflows/build-publish.yml/badge.svg?event=push)](https://github.com/ktsstudio/shopback-sdk/actions/workflows/build-publish.yml)
 [![Python Version](https://img.shields.io/pypi/pyversions/shopback-sdk.svg)](https://pypi.org/project/shopback-sdk/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ktsstudio/shopback-sdk/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ktsstudio/shopback-sdk/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ktsstudio/shopback-sdk/releases)
```

