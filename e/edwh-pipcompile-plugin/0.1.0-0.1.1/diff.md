# Comparing `tmp/edwh_pipcompile_plugin-0.1.0.tar.gz` & `tmp/edwh_pipcompile_plugin-0.1.1.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.0.tar` & `edwh_pipcompile_plugin-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/README.md
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.0/requirements-dev.txt` & `edwh_pipcompile_plugin-0.1.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.0/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.0/LICENSE.txt` & `edwh_pipcompile_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.0/pyproject.toml` & `edwh_pipcompile_plugin-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.0/PKG-INFO` & `edwh_pipcompile_plugin-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -18,28 +18,36 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: invoke
 Requires-Dist: pip-tools
 Description-Content-Type: text/markdown
 
-# edwh-demo-plugin
+# edwh-pipcompile-plugin
 
-[![PyPI - Version](https://img.shields.io/pypi/v/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
+[![PyPI - Version](https://img.shields.io/pypi/v/edwh-pipcompile-plugin.svg)](https://pypi.org/project/edwh-pipcompile-plugin)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-pipcompile-plugin.svg)](https://pypi.org/project/edwh-pipcompile-plugin)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
-pip install edwh-demo-plugin
+pip install edwh-pipcompile-plugin
+```
+
+But probably you want to install the whole edwh package:
+
+```console
+pipx install edwh[pip]
+# or
+pipx install edwh[plugins,omgeving]
 ```
 
 ## License
 
-`edwh-demo-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`edwh-pipcompile-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

