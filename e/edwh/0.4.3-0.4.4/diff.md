# Comparing `tmp/edwh-0.4.3.tar.gz` & `tmp/edwh-0.4.4.tar.gz`

## Comparing `edwh-0.4.3.tar` & `edwh-0.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.4.3/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.4.3/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.4.3/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.3/src/edwh/__init__.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 edwh-0.4.3/src/edwh/cli.py
--rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 edwh-0.4.3/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.4.3/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.4.3/LICENSE.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.4.3/README.md
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 edwh-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 edwh-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 edwh-0.4.4/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.4.4/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.4.4/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.4/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 edwh-0.4.4/src/edwh/cli.py
+-rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 edwh-0.4.4/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.4.4/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.4.4/README.md
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 edwh-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 edwh-0.4.4/PKG-INFO
```

### Comparing `edwh-0.4.3/CHANGELOG.md` & `edwh-0.4.4/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.4 (2023-04-11)
+### Fix
+* **edwh:** Include bundler-plugin in edwh[plugins] as well ([`df4424d`](https://github.com/educationwarehouse/edwh/commit/df4424d37c225c3e6c89010a3186fc225d13e354))
+
 ## v0.3.2 (2023-04-10)
 ### Fix
 * Diceware was included as a dependency, but used as a pipx installed application. ([`2f6bc9f`](https://github.com/educationwarehouse/edwh/commit/2f6bc9f7c7aabafbab0b857d84905be13d3973f0))
 
 ## v0.3.1 (2023-04-10)
 ### Fix
 * Missing changelog entry ([`4fe91e4`](https://github.com/educationwarehouse/edwh/commit/4fe91e400a8b64197b7a1c7df55777c13787b2d7))
```

### Comparing `edwh-0.4.3/src/edwh/cli.py` & `edwh-0.4.4/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.4.3/src/edwh/tasks.py` & `edwh-0.4.4/src/edwh/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh-0.4.3/LICENSE.txt` & `edwh-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.4.3/README.md` & `edwh-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.4.3/pyproject.toml` & `edwh-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
   'pyyaml',
   'tomlkit'
 ]
 plugins = [
   'edwh-multipass-plugin',
   'edwh-demo-tasks-plugin',
   'edwh-restic-plugin',
-  'edwh-pipcompile-plugin'
+  'edwh-pipcompile-plugin',
+  'edwh-bundler-plugin'
 ]
 
 restic = [
   'edwh-restic-plugin',
 ]
 
 multipass = [
```

### Comparing `edwh-0.4.3/PKG-INFO` & `edwh-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.4.3
+Version: 0.4.4
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -36,14 +36,15 @@
 Requires-Dist: tabulate; extra == 'omgeving'
 Requires-Dist: tomlkit; extra == 'omgeving'
 Provides-Extra: pip
 Requires-Dist: edwh-pipcompile-plugin; extra == 'pip'
 Provides-Extra: pip-compile
 Requires-Dist: edwh-pipcompile-plugin; extra == 'pip-compile'
 Provides-Extra: plugins
+Requires-Dist: edwh-bundler-plugin; extra == 'plugins'
 Requires-Dist: edwh-demo-tasks-plugin; extra == 'plugins'
 Requires-Dist: edwh-multipass-plugin; extra == 'plugins'
 Requires-Dist: edwh-pipcompile-plugin; extra == 'plugins'
 Requires-Dist: edwh-restic-plugin; extra == 'plugins'
 Provides-Extra: restic
 Requires-Dist: edwh-restic-plugin; extra == 'restic'
 Description-Content-Type: text/markdown
```

