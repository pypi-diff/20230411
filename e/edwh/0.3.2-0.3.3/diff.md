# Comparing `tmp/edwh-0.3.2.tar.gz` & `tmp/edwh-0.3.3.tar.gz`

## Comparing `edwh-0.3.2.tar` & `edwh-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,12 @@
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/.gitignore
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/edwh.iml
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/vcs.xml
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 edwh-0.3.2/c/edwh-0.3.0-py3-none-any.whl
--rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 edwh-0.3.2/c/edwh-0.3.0.tar.gz
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/cli.py
--rw-r--r--   0        0        0    16936 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.2/README.md
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 edwh-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 edwh-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 edwh-0.3.3/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/cli.py
+-rw-r--r--   0        0        0    16936 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.3/README.md
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 edwh-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 edwh-0.3.3/PKG-INFO
```

### Comparing `edwh-0.3.2/CHANGELOG.md` & `edwh-0.3.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `edwh-0.3.2/src/edwh/cli.py` & `edwh-0.3.3/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.3.2/src/edwh/tasks.py` & `edwh-0.3.3/src/edwh/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh-0.3.2/LICENSE.txt` & `edwh-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.3.2/README.md` & `edwh-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.3.2/pyproject.toml` & `edwh-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 plugins = [
   'edwh-multipass-plugin',
   'edwh-demo-tasks-plugin',
   'edwh-restic-plugin',
   #'edwh-pipcompile-plugin'
 ]
 
+restic = [
+  'edwh-restic-plugin',
+]
+
+multipass = [
+  'edwh-multipass-plugin',
+]
+
 [project.scripts]
 edwh = "edwh.cli:program.run"
 ew = "edwh.cli:program.run"
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh#readme"
 Issues = "https://github.com/educationwarehouse/edwh/issues"
```

### Comparing `edwh-0.3.2/PKG-INFO` & `edwh-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.3.2
+Version: 0.3.3
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -20,23 +20,27 @@
 Requires-Python: >=3.7
 Requires-Dist: diceware
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: invoke
 Requires-Dist: pyyaml
 Requires-Dist: tabulate
 Requires-Dist: tomlkit
+Provides-Extra: multipass
+Requires-Dist: edwh-multipass-plugin; extra == 'multipass'
 Provides-Extra: omgeving
 Requires-Dist: humanize; extra == 'omgeving'
 Requires-Dist: pyyaml; extra == 'omgeving'
 Requires-Dist: tabulate; extra == 'omgeving'
 Requires-Dist: tomlkit; extra == 'omgeving'
 Provides-Extra: plugins
 Requires-Dist: edwh-demo-tasks-plugin; extra == 'plugins'
 Requires-Dist: edwh-multipass-plugin; extra == 'plugins'
 Requires-Dist: edwh-restic-plugin; extra == 'plugins'
+Provides-Extra: restic
+Requires-Dist: edwh-restic-plugin; extra == 'restic'
 Description-Content-Type: text/markdown
 
 # edwh
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh.svg)](https://pypi.org/project/edwh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh.svg)](https://pypi.org/project/edwh)
```

