# Comparing `tmp/edwh_pipcompile_plugin-0.1.2.tar.gz` & `tmp/edwh_pipcompile_plugin-0.1.3.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.2.tar` & `edwh_pipcompile_plugin-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/README.md
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.3/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.2/requirements-dev.txt` & `edwh_pipcompile_plugin-0.1.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.1.3/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,30 +167,14 @@
 
         else:
             options.append(f"{pref} {value}")
 
     return " " + " ".join(options)
 
 
-class Test:
-    _excluded = ["a", "c"]
-
-    @property
-    def excluded(self):
-        # wat moet er uitgesloten worden?
-        return kwargs_to_options(excluded=self._excluded)
-
-
-@task
-def test(c):
-    a = Test()
-
-    print(a.excluded)
-
-
 def _pip_compile(*args, **kwargs):
     """
     Execute pip-compile with positional and keyword args
     """
     if "resolver" not in kwargs:
         kwargs["resolver"] = "backtracking"
 
@@ -421,8 +405,8 @@
             f.write(new_deps)
 
         with show_diff(
             in_to_out(file)
         ):  # no rollback required since pip compile can't fail on remove
             compile(ctx, path=path, pypi_server=pypi_server)
 
-        success(f"Package {_package} removed from {file}")
+        success(f"Package {_package} removed from {file}")
```

### Comparing `edwh_pipcompile_plugin-0.1.2/LICENSE.txt` & `edwh_pipcompile_plugin-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.2/README.md` & `edwh_pipcompile_plugin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.2/pyproject.toml` & `edwh_pipcompile_plugin-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.2/PKG-INFO` & `edwh_pipcompile_plugin-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

