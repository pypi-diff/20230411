# Comparing `tmp/cloudlab_client-0.1.73.tar.gz` & `tmp/cloudlab_client-0.1.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlab_client-0.1.73.tar", max compression
+gzip compressed data, was "cloudlab_client-0.1.79.tar", max compression
```

## Comparing `cloudlab_client-0.1.73.tar` & `cloudlab_client-0.1.79.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1022 2022-12-30 13:50:39.782029 cloudlab_client-0.1.73/README.md
--rw-r--r--   0        0        0        0 2022-12-30 13:50:39.782029 cloudlab_client-0.1.73/cloudlab_client/__init__.py
--rw-r--r--   0        0        0     8305 2022-12-30 13:50:39.782029 cloudlab_client-0.1.73/cloudlab_client/client.py
--rw-r--r--   0        0        0     1635 2022-12-30 13:50:39.782029 cloudlab_client-0.1.73/cloudlab_client/test_client.py
--rw-r--r--   0        0        0      451 2022-12-30 13:50:58.870219 cloudlab_client-0.1.73/pyproject.toml
--rw-r--r--   0        0        0     1716 1970-01-01 00:00:00.000000 cloudlab_client-0.1.73/setup.py
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cloudlab_client-0.1.73/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/cloudlab_client/__init__.py
+-rw-r--r--   0        0        0     8305 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/cloudlab_client/client.py
+-rw-r--r--   0        0        0     1635 2023-04-10 22:35:15.071517 cloudlab_client-0.1.79/cloudlab_client/test_client.py
+-rw-r--r--   0        0        0      451 2023-04-10 22:35:34.075517 cloudlab_client-0.1.79/pyproject.toml
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cloudlab_client-0.1.79/PKG-INFO
```

### Comparing `cloudlab_client-0.1.73/README.md` & `cloudlab_client-0.1.79/README.md`

 * *Files identical despite different names*

### Comparing `cloudlab_client-0.1.73/cloudlab_client/client.py` & `cloudlab_client-0.1.79/cloudlab_client/client.py`

 * *Files identical despite different names*

### Comparing `cloudlab_client-0.1.73/cloudlab_client/test_client.py` & `cloudlab_client-0.1.79/cloudlab_client/test_client.py`

 * *Files identical despite different names*

### Comparing `cloudlab_client-0.1.73/setup.py` & `cloudlab_client-0.1.79/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,48 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cloudlab-client
+Version: 0.1.79
+Summary: Client for the cloudlab academic cloud environment.
+Author: Yannis Zarkadas
+Author-email: yanniszark@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: selenium (>=4.1.3,<5.0.0)
+Description-Content-Type: text/markdown
+
+# Cloudlab Client
+
+This package is a client for the Cloudlab service. Cloudlab is a cloud for
+academic institutions. Because I could not (yet) find any working API for
+Cloudlab, the current client relies on username / password authentication and
+web scraping.
+
+
+## Usage
+
+
+```python
+# Create new client and login
+username = os.environ.get("CLOUDLAB_USERNAME")
+password = os.environ.get("CLOUDLAB_PASSWORD")
+cloudlab_client = CloudlabClient()
+cloudlab_client.login(username, password)
+
+# List experiments
+experiments = cloudlab_client.experiment_list()
+print(experiments)
+
+# List an experiment's nodes
+nodes = cloudlab_client.experiment_list_nodes("my-experiment")
+print(nodes)
+
+# Request an extension (e.g., for 6 days). Reason must be at least 120 characters.
+reason = ("Important experiment needed for research, conducted under advisor"
+          " <fill_your_advisor>. Particular machines are needed because"
+          " <fill_your_reasons>.")
+cloudlab_client.experiment_extend("my-experiment", reason, hours=6*24)
+```
 
-packages = \
-['cloudlab_client']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['selenium>=4.1.3,<5.0.0']
-
-setup_kwargs = {
-    'name': 'cloudlab-client',
-    'version': '0.1.73',
-    'description': 'Client for the cloudlab academic cloud environment.',
-    'long_description': '# Cloudlab Client\n\nThis package is a client for the Cloudlab service. Cloudlab is a cloud for\nacademic institutions. Because I could not (yet) find any working API for\nCloudlab, the current client relies on username / password authentication and\nweb scraping.\n\n\n## Usage\n\n\n```python\n# Create new client and login\nusername = os.environ.get("CLOUDLAB_USERNAME")\npassword = os.environ.get("CLOUDLAB_PASSWORD")\ncloudlab_client = CloudlabClient()\ncloudlab_client.login(username, password)\n\n# List experiments\nexperiments = cloudlab_client.experiment_list()\nprint(experiments)\n\n# List an experiment\'s nodes\nnodes = cloudlab_client.experiment_list_nodes("my-experiment")\nprint(nodes)\n\n# Request an extension (e.g., for 6 days). Reason must be at least 120 characters.\nreason = ("Important experiment needed for research, conducted under advisor"\n          " <fill_your_advisor>. Particular machines are needed because"\n          " <fill_your_reasons>.")\ncloudlab_client.experiment_extend("my-experiment", reason, hours=6*24)\n```\n',
-    'author': 'Yannis Zarkadas',
-    'author_email': 'yanniszark@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

