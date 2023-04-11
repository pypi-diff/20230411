# Comparing `tmp/hcf-backend-0.4.7.tar.gz` & `tmp/hcf-backend-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcf-backend-0.4.7.tar", last modified: Mon Nov 28 15:21:46 2022, max compression
+gzip compressed data, was "hcf-backend-0.5.1.tar", last modified: Tue Apr 11 21:21:50 2023, max compression
```

## Comparing `hcf-backend-0.4.7.tar` & `hcf-backend-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-11-28 15:21:46.216308 hcf-backend-0.4.7/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.4.7/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2434 2022-11-28 15:21:46.216308 hcf-backend-0.4.7/PKG-INFO
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1815 2021-04-28 22:54:27.000000 hcf-backend-0.4.7/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-11-28 15:21:46.216308 hcf-backend-0.4.7/hcf_backend/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       47 2022-11-28 15:21:24.000000 hcf-backend-0.4.7/hcf_backend/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2022-11-16 15:07:50.000000 hcf-backend-0.4.7/hcf_backend/backend.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4286 2021-07-13 20:41:18.000000 hcf-backend-0.4.7/hcf_backend/manager.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-11-28 15:21:46.216308 hcf-backend-0.4.7/hcf_backend/utils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1631 2022-11-16 14:59:35.000000 hcf-backend-0.4.7/hcf_backend/utils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3931 2022-11-28 15:21:24.000000 hcf-backend-0.4.7/hcf_backend/utils/crawlmanager.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13575 2021-07-13 00:16:37.000000 hcf-backend-0.4.7/hcf_backend/utils/hcfpal.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-11-28 15:21:46.216308 hcf-backend-0.4.7/hcf_backend.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2434 2022-11-28 15:21:46.000000 hcf-backend-0.4.7/hcf_backend.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2022-11-28 15:21:46.000000 hcf-backend-0.4.7/hcf_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2022-11-28 15:21:46.000000 hcf-backend-0.4.7/hcf_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      105 2022-11-28 15:21:46.000000 hcf-backend-0.4.7/hcf_backend.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2022-11-28 15:21:46.000000 hcf-backend-0.4.7/hcf_backend.egg-info/top_level.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.4.7/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2022-11-28 15:21:46.216308 hcf-backend-0.4.7/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1010 2022-11-28 15:21:24.000000 hcf-backend-0.4.7/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/hcf_backend/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       46 2023-04-11 21:21:16.000000 hcf-backend-0.5.1/hcf_backend/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-11 20:57:08.000000 hcf-backend-0.5.1/hcf_backend/backend.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4286 2021-07-13 20:41:18.000000 hcf-backend-0.5.1/hcf_backend/manager.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/hcf_backend/utils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.1/hcf_backend/utils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3896 2023-04-11 21:07:29.000000 hcf-backend-0.5.1/hcf_backend/utils/crawlmanager.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13407 2023-04-11 21:12:01.000000 hcf-backend-0.5.1/hcf_backend/utils/hcfpal.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/hcf_backend.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-11 21:21:50.000000 hcf-backend-0.5.1/hcf_backend.egg-info/top_level.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-11 21:21:50.701049 hcf-backend-0.5.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1012 2023-04-11 21:21:23.000000 hcf-backend-0.5.1/setup.py
```

### Comparing `hcf-backend-0.4.7/LICENSE` & `hcf-backend-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.4.7/PKG-INFO` & `hcf-backend-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.4.7
+Version: 0.5.1
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -36,7 +36,23 @@
 Another provided tool is [crawlmanager.py](https://github.com/scrapinghub/hcf-backend/blob/master/hcf_backend/utils/crawlmanager.py). It facilitates the
 scheduling of consumer spider jobs. Examples of usage are also available in the already mentioned `shub-workflow` Tutorial.
 
 Installation
 ============
 
 `pip install hcf-backend`
+
+
+Development environment setup
+=============================
+
+For hcf-backend developers, Pipfile files are provided for a development environment.
+
+Run:
+
+```
+$ pipenv install --dev
+$ pipenv shell
+$ cp .envtemplate .env
+```
+
+and edit .env accordingly
```

### Comparing `hcf-backend-0.4.7/README.md` & `hcf-backend-0.5.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,7 +19,23 @@
 Another provided tool is [crawlmanager.py](https://github.com/scrapinghub/hcf-backend/blob/master/hcf_backend/utils/crawlmanager.py). It facilitates the
 scheduling of consumer spider jobs. Examples of usage are also available in the already mentioned `shub-workflow` Tutorial.
 
 Installation
 ============
 
 `pip install hcf-backend`
+
+
+Development environment setup
+=============================
+
+For hcf-backend developers, Pipfile files are provided for a development environment.
+
+Run:
+
+```
+$ pipenv install --dev
+$ pipenv shell
+$ cp .envtemplate .env
+```
+
+and edit .env accordingly
```

### Comparing `hcf-backend-0.4.7/hcf_backend/backend.py` & `hcf-backend-0.5.1/hcf_backend/backend.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.4.7/hcf_backend/manager.py` & `hcf-backend-0.5.1/hcf_backend/manager.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.4.7/hcf_backend/utils/__init__.py` & `hcf-backend-0.5.1/hcf_backend/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import hashlib
 import six
 
-try:
-    from collections import Mapping
-except ImportError:
-    from collections.abc import Mapping
+from collections.abc import Mapping
 
 from scrapinghub.client import parse_auth
 
 
 def convert_from_bytes(data):
     if data is not None:
         data_type = type(data)
```

### Comparing `hcf-backend-0.4.7/hcf_backend/utils/crawlmanager.py` & `hcf-backend-0.5.1/hcf_backend/utils/crawlmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class HCFCrawlManager(CrawlManager):
 
     default_max_jobs = 1
 
     def __init__(self):
         super().__init__()
-        self.hcfpal = HCFPal(self.client._hsclient.get_project(self.project_id))
+        self.hcfpal = HCFPal(self.project_id)
 
     def add_argparser_options(self):
         super().add_argparser_options()
         self.argparser.add_argument("frontier", help="Frontier name")
         self.argparser.add_argument("prefix", help="Slot prefix")
         self.argparser.add_argument("--frontera-settings-json")
```

### Comparing `hcf-backend-0.4.7/hcf_backend/utils/hcfpal.py` & `hcf-backend-0.5.1/hcf_backend/utils/hcfpal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 import re
 import pprint
 from itertools import cycle, groupby
 from operator import itemgetter
+from typing import Optional
 
 import humanize
 import requests
 from requests.auth import HTTPBasicAuth
-from requests.exceptions import HTTPError, ConnectionError
 from retrying import retry
-from shub_workflow.script import BaseScript
+from shub_workflow.script import BaseScript, SCProjectClass
+from shub_workflow.utils import dash_retry_decorator
 
 from hcf_backend.utils import assign_slotno
 
 
-def retry_if_http_error(e):
-    for exctype in HTTPError, ConnectionError:
-        if isinstance(e, exctype):
-            print(f"Error: {e}. Retrying...")
-            return True
-    return False
-
-
-class HCFPal:
+class HCFPal(SCProjectClass):
 
     HCF_API_URLS = {
         "count": "https://storage.scrapinghub.com/hcf/{pid}/{frontier}/s/{slot}/q/count",
         "list_frontiers": "https://storage.scrapinghub.com/hcf/{pid}/list",
         "list_slots": "https://storage.scrapinghub.com/hcf/{pid}/{frontier}/list",
     }
 
-    def __init__(self, project):
-        self.project = project
-
-    @property
-    def projectid(self):
-        return self.project.projectid
+    def __init__(self, project_id: Optional[int] = None):
+        super().__init__()
+        self.project_id = project_id or self.project_id
+        hsc = self.client._hsclient
+        self.project = hsc.get_project(self.project_id)
 
     @property
     def auth(self):
         return self.project.auth
 
-    @retry(
-        retry_on_exception=retry_if_http_error, wait_fixed=60000, stop_max_attempt_number=60 * 24,  # 1 min
-    )  # 1 day
+    @dash_retry_decorator
     def _get_json(self, url):
         response = requests.get(url, auth=HTTPBasicAuth(*self.auth))
         response.raise_for_status()
         return response.json()
 
     def get_frontiers(self):
-        url = self.HCF_API_URLS["list_frontiers"].format(pid=self.projectid)
+        url = self.HCF_API_URLS["list_frontiers"].format(pid=self.project_id)
         return self._get_json(url)
 
     def get_slots(self, frontier):
-        url = self.HCF_API_URLS["list_slots"].format(pid=self.projectid, frontier=frontier)
+        url = self.HCF_API_URLS["list_slots"].format(pid=self.project_id, frontier=frontier)
         return self._get_json(url)
 
     def delete_slots(self, frontier, slots):
         for slot in slots:
             self.project.frontier.delete_slot(frontier, slot)
 
     def list_all(self, prettyprint=False):
@@ -66,15 +56,15 @@
             yall[frontier] = self.get_slots(frontier)
         if prettyprint:
             return pprint.pformat(yall, indent=4)
         else:
             return yall
 
     def get_slot_count(self, frontier, slot):
-        URL = self.HCF_API_URLS["count"].format(pid=self.projectid, frontier=frontier, slot=slot)
+        URL = self.HCF_API_URLS["count"].format(pid=self.project_id, frontier=frontier, slot=slot)
         total = 0
         nextstart = ""
         while True:
             next_url = URL + "?start={}".format(nextstart) if nextstart else URL
             data = self._get_json(next_url)
             total += int(data.get("count"))
             nextstart = data.get("nextstart", "")
@@ -116,15 +106,15 @@
 
     flow_id_required = False
 
     def __init__(self):
         super().__init__()
         hsc = self.client._hsclient
         self.hsp = hsc.get_project(self.project_id)
-        self.hcf = HCFPal(self.hsp)
+        self.hcf = HCFPal()
 
     @property
     def description(self):
         return "Helper script for accessing HubCrawlFrontier."
 
     def add_argparser_options(self):
         super().add_argparser_options()
```

### Comparing `hcf-backend-0.4.7/hcf_backend.egg-info/PKG-INFO` & `hcf-backend-0.5.1/hcf_backend.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.4.7
+Version: 0.5.1
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -36,7 +36,23 @@
 Another provided tool is [crawlmanager.py](https://github.com/scrapinghub/hcf-backend/blob/master/hcf_backend/utils/crawlmanager.py). It facilitates the
 scheduling of consumer spider jobs. Examples of usage are also available in the already mentioned `shub-workflow` Tutorial.
 
 Installation
 ============
 
 `pip install hcf-backend`
+
+
+Development environment setup
+=============================
+
+For hcf-backend developers, Pipfile files are provided for a development environment.
+
+Run:
+
+```
+$ pipenv install --dev
+$ pipenv shell
+$ cp .envtemplate .env
+```
+
+and edit .env accordingly
```

### Comparing `hcf-backend-0.4.7/setup.py` & `hcf-backend-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name="hcf-backend",
-    version="0.4.7",
+    version="0.5.1",
     description="ScrapyCloud HubStorage frontier backend for Frontera",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/scrapinghub/hcf-backend",
     maintainer="Scrapinghub",
     packages=find_packages(),
     install_requires=(
         "frontera==0.7.1",
         "humanize==0.5.1",
         "requests>=2.18.4",
         "retrying>=1.3.3",
         "scrapinghub>=2.0.0",
-        "shub-workflow>=1.5.1",
+        "shub-workflow>=1.10.20",
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
```

