# Comparing `tmp/edwh_pipcompile_plugin-0.1.1.tar.gz` & `tmp/edwh_pipcompile_plugin-0.1.2.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.1.tar` & `edwh_pipcompile_plugin-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/README.md
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.2/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.1/requirements-dev.txt` & `edwh_pipcompile_plugin-0.1.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.1.2/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Dit script maakt het werken met pip-tools nog iets slimmer.
 De volgende commando's zijn beschikbaar:
 - pip.compile
 - pip.install
-- pip.install-pip-tools
 - pip.remove
 - pip.upgrade
 
 Het verschil met standaard pip-tools is dat operations zoals install, remove en upgrade ook aanpassingen in de .in file
 kunnen doen. Compile werkt hetzelfde, maar het is fijn om alle related commando's onder invoke pip.* te hebben.
 """
 
@@ -243,28 +242,15 @@
         PACKAGE_RE.format(package=package),
         re.MULTILINE | re.IGNORECASE,
     )
 
 
 ### ONLY @task's AFTER THIS!!!
 
-
-@task
-def install_pip_tools(ctx):
-    """
-    Task that's executed before other pip-tools tasks to make sure pip-tools is installed.
-    """
-    try:
-        import piptools
-    except ModuleNotFoundError:
-        warn("missing pip-tools, installing")
-        ctx.run("pip install pip-tools")
-
-
-@task(pre=[install_pip_tools])
+@task()
 def compile(ctx, path, pypi_server=DEFAULT_SERVER):
     """
     Task (invoke pip.compile) to run pip-compile on one or more files (-f requirements1.in -f requirements2.in)
 
     Arguments:
         ctx (invoke.Context): invoke context
         path (str): path to directory to compile infiles or specific infile
@@ -284,15 +270,15 @@
 
     for file in files:
         _pip_compile(file, **args)
 
         success(f"Ran pip-compile! Check {in_to_out(file)}")
 
 
-@task(pre=[install_pip_tools])
+@task()
 def install(ctx, path, package, pypi_server=DEFAULT_SERVER):
     """
     Install a package to the .in file of the specified directory and re-compile the requirements.txt
     The command also checks if the command is already added and if it exists on the specified pypi server
 
     Arguments:
         ctx (invoke.Context): invoke context
@@ -324,15 +310,15 @@
         success(f"Installing {package} in {file}")
 
         # post: pip-compile
         with rollback(contents, file), show_diff(in_to_out(file)):
             compile(ctx, path=path, pypi_server=pypi_server)
 
 
-@task(pre=[install_pip_tools], iterable=["files"])
+@task(iterable=["files"])
 def upgrade(ctx, path, package=None, force=False, pypi_server=DEFAULT_SERVER):
     """
     Upgrade package(s) in one or multiple infiles. Version pins will be respected,
     unless a specific package with --force or a specific package with a new pin is supplied.
 
     Arguments:
         ctx (invoke.Context): invoke context
@@ -392,15 +378,14 @@
             # ctx.run(f'pip-compile {arg} {file}')
             _pip_compile(file, **args)
 
         success("Upgrade complete.")
 
 
 @task(
-    pre=[install_pip_tools],
     iterable=["files"]
     # post=[pip_compile],
 )
 def remove(ctx, path, package, pypi_server=DEFAULT_SERVER):
     """
     Remove a package from one or multiple infiles
```

### Comparing `edwh_pipcompile_plugin-0.1.1/LICENSE.txt` & `edwh_pipcompile_plugin-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.1/README.md` & `edwh_pipcompile_plugin-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
+- [Changelog](#changelog)
 
 ## Installation
 
 ```console
 pip install edwh-pipcompile-plugin
 ```
 
@@ -23,7 +24,11 @@
 # or
 pipx install edwh[plugins,omgeving]
 ```
 
 ## License
 
 `edwh-pipcompile-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Changelog 
+
+[See CHANGELOG.md](CHANGELOG.md)
```

### Comparing `edwh_pipcompile_plugin-0.1.1/pyproject.toml` & `edwh_pipcompile_plugin-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 [project.entry-points."edwh.tasks"]
 pip = "edwh_pipcompile_plugin.pipcompile_plugin"
 
 [tool.hatch.version]
 path = "src/edwh_pipcompile_plugin/__about__.py"
 
 [tool.semantic_release]
-branch = "main"
+branch = "master"
 version_variable = "src/edwh_pipcompile_plugin/__about__.py:__version__"
 change_log = "CHANGELOG.md"
 upload_to_repository = false
 upload_to_release = false
 build_command = "hatch build"
```

### Comparing `edwh_pipcompile_plugin-0.1.1/PKG-INFO` & `edwh_pipcompile_plugin-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -29,14 +29,15 @@
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
+- [Changelog](#changelog)
 
 ## Installation
 
 ```console
 pip install edwh-pipcompile-plugin
 ```
 
@@ -47,7 +48,11 @@
 # or
 pipx install edwh[plugins,omgeving]
 ```
 
 ## License
 
 `edwh-pipcompile-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Changelog 
+
+[See CHANGELOG.md](CHANGELOG.md)
```

