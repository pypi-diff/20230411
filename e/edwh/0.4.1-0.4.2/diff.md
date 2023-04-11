# Comparing `tmp/edwh-0.4.1.tar.gz` & `tmp/edwh-0.4.2.tar.gz`

## Comparing `edwh-0.4.1.tar` & `edwh-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.4.1/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/__init__.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/cli.py
--rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.4.1/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.4.1/README.md
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 edwh-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 edwh-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.4.2/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.4.2/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.2/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 edwh-0.4.2/src/edwh/cli.py
+-rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 edwh-0.4.2/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.4.2/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.4.2/README.md
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 edwh-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 edwh-0.4.2/PKG-INFO
```

### Comparing `edwh-0.4.1/CHANGELOG.md` & `edwh-0.4.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `edwh-0.4.1/src/edwh/cli.py` & `edwh-0.4.2/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.4.1/src/edwh/tasks.py` & `edwh-0.4.2/src/edwh/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh-0.4.1/LICENSE.txt` & `edwh-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.4.1/README.md` & `edwh-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.4.1/pyproject.toml` & `edwh-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,29 @@
   'pyyaml',
   'tomlkit'
 ]
 plugins = [
   'edwh-multipass-plugin',
   'edwh-demo-tasks-plugin',
   'edwh-restic-plugin',
-  #'edwh-pipcompile-plugin'
+  'edwh-pipcompile-plugin'
 ]
 
 restic = [
   'edwh-restic-plugin',
 ]
 
 multipass = [
   'edwh-multipass-plugin',
 ]
 
+pip = [
+  'edwh-pipcompile-plugin',
+]
+
 [project.scripts]
 edwh = "edwh.cli:program.run"
 ew = "edwh.cli:program.run"
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh#readme"
 Issues = "https://github.com/educationwarehouse/edwh/issues"
```

### Comparing `edwh-0.4.1/PKG-INFO` & `edwh-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.4.1
+Version: 0.4.2
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -27,17 +27,20 @@
 Provides-Extra: multipass
 Requires-Dist: edwh-multipass-plugin; extra == 'multipass'
 Provides-Extra: omgeving
 Requires-Dist: humanize; extra == 'omgeving'
 Requires-Dist: pyyaml; extra == 'omgeving'
 Requires-Dist: tabulate; extra == 'omgeving'
 Requires-Dist: tomlkit; extra == 'omgeving'
+Provides-Extra: pip
+Requires-Dist: edwh-pipcompile-plugin; extra == 'pip'
 Provides-Extra: plugins
 Requires-Dist: edwh-demo-tasks-plugin; extra == 'plugins'
 Requires-Dist: edwh-multipass-plugin; extra == 'plugins'
+Requires-Dist: edwh-pipcompile-plugin; extra == 'plugins'
 Requires-Dist: edwh-restic-plugin; extra == 'plugins'
 Provides-Extra: restic
 Requires-Dist: edwh-restic-plugin; extra == 'restic'
 Description-Content-Type: text/markdown
 
 # edwh
```

