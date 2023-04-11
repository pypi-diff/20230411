# Comparing `tmp/python-lsp-ruff-1.3.0.tar.gz` & `tmp/python-lsp-ruff-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lsp-ruff-1.3.0.tar", last modified: Sun Apr  2 21:55:02 2023, max compression
+gzip compressed data, was "python-lsp-ruff-1.4.0.tar", last modified: Tue Apr 11 13:35:16 2023, max compression
```

## Comparing `python-lsp-ruff-1.3.0.tar` & `python-lsp-ruff-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-02 21:55:02.833327 python-lsp-ruff-1.3.0/
--rw-r--r--   0 juli      (1000) juli      (1000)     1138 2022-12-05 16:14:35.000000 python-lsp-ruff-1.3.0/LICENSE
--rw-r--r--   0 juli      (1000) juli      (1000)     2799 2023-04-02 21:55:02.833327 python-lsp-ruff-1.3.0/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)     2379 2023-04-02 21:46:29.000000 python-lsp-ruff-1.3.0/README.md
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-02 21:55:02.833327 python-lsp-ruff-1.3.0/pylsp_ruff/
--rw-r--r--   0 juli      (1000) juli      (1000)        0 2022-12-01 22:28:29.000000 python-lsp-ruff-1.3.0/pylsp_ruff/__init__.py
--rw-r--r--   0 juli      (1000) juli      (1000)    14089 2023-04-02 21:39:03.000000 python-lsp-ruff-1.3.0/pylsp_ruff/plugin.py
--rw-r--r--   0 juli      (1000) juli      (1000)      436 2023-04-02 21:39:03.000000 python-lsp-ruff-1.3.0/pylsp_ruff/ruff.py
--rw-r--r--   0 juli      (1000) juli      (1000)      833 2023-04-02 21:51:19.000000 python-lsp-ruff-1.3.0/pyproject.toml
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-02 21:55:02.833327 python-lsp-ruff-1.3.0/python_lsp_ruff.egg-info/
--rw-r--r--   0 juli      (1000) juli      (1000)     2799 2023-04-02 21:55:02.000000 python-lsp-ruff-1.3.0/python_lsp_ruff.egg-info/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)      391 2023-04-02 21:55:02.000000 python-lsp-ruff-1.3.0/python_lsp_ruff.egg-info/SOURCES.txt
--rw-r--r--   0 juli      (1000) juli      (1000)        1 2023-04-02 21:55:02.000000 python-lsp-ruff-1.3.0/python_lsp_ruff.egg-info/dependency_links.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       33 2023-04-02 21:55:02.000000 python-lsp-ruff-1.3.0/python_lsp_ruff.egg-info/entry_points.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       80 2023-04-02 21:55:02.000000 python-lsp-ruff-1.3.0/python_lsp_ruff.egg-info/requires.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       11 2023-04-02 21:55:02.000000 python-lsp-ruff-1.3.0/python_lsp_ruff.egg-info/top_level.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       38 2023-04-02 21:55:02.833327 python-lsp-ruff-1.3.0/setup.cfg
--rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-01-14 19:42:55.000000 python-lsp-ruff-1.3.0/setup.py
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-02 21:55:02.833327 python-lsp-ruff-1.3.0/tests/
--rw-r--r--   0 juli      (1000) juli      (1000)     2907 2023-04-02 21:39:03.000000 python-lsp-ruff-1.3.0/tests/test_code_actions.py
--rw-r--r--   0 juli      (1000) juli      (1000)     6734 2023-04-02 21:39:03.000000 python-lsp-ruff-1.3.0/tests/test_ruff_lint.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/
+-rw-r--r--   0 juli      (1000) juli      (1000)     1138 2022-12-05 16:14:35.000000 python-lsp-ruff-1.4.0/LICENSE
+-rw-r--r--   0 juli      (1000) juli      (1000)     3732 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)     3312 2023-04-11 13:29:01.000000 python-lsp-ruff-1.4.0/README.md
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.681051 python-lsp-ruff-1.4.0/pylsp_ruff/
+-rw-r--r--   0 juli      (1000) juli      (1000)        0 2022-12-01 22:28:29.000000 python-lsp-ruff-1.4.0/pylsp_ruff/__init__.py
+-rw-r--r--   0 juli      (1000) juli      (1000)    16250 2023-04-11 13:29:01.000000 python-lsp-ruff-1.4.0/pylsp_ruff/plugin.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      436 2023-04-02 21:39:03.000000 python-lsp-ruff-1.4.0/pylsp_ruff/ruff.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     1628 2023-04-10 17:55:44.000000 python-lsp-ruff-1.4.0/pylsp_ruff/settings.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      876 2023-04-11 13:31:40.000000 python-lsp-ruff-1.4.0/pyproject.toml
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/
+-rw-r--r--   0 juli      (1000) juli      (1000)     3732 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)      414 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/SOURCES.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)        1 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/dependency_links.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       33 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/entry_points.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)      121 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/requires.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       11 2023-04-11 13:35:16.000000 python-lsp-ruff-1.4.0/python_lsp_ruff.egg-info/top_level.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       38 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/setup.cfg
+-rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-01-14 19:42:55.000000 python-lsp-ruff-1.4.0/setup.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-04-11 13:35:16.684385 python-lsp-ruff-1.4.0/tests/
+-rw-r--r--   0 juli      (1000) juli      (1000)     3960 2023-04-11 11:39:49.000000 python-lsp-ruff-1.4.0/tests/test_code_actions.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     6832 2023-04-10 17:38:09.000000 python-lsp-ruff-1.4.0/tests/test_ruff_lint.py
```

### Comparing `python-lsp-ruff-1.3.0/LICENSE` & `python-lsp-ruff-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-1.3.0/pyproject.toml` & `python-lsp-ruff-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-lsp-ruff"
 authors = [
   {name = "Julian Hossbach", email = "julian.hossbach@gmx.de"}
 ]
-version = "1.3.0"
+version = "1.4.0"
 description = "Ruff linting plugin for pylsp"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 dependencies = [
   "ruff>=0.0.260",
   "python-lsp-server",
   "lsprotocol>=2022.0.0a1",
+  "tomli>=1.1.0; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "pre-commit"]
 
 [project.entry-points.pylsp]
 ruff = "pylsp_ruff.plugin"
```

### Comparing `python-lsp-ruff-1.3.0/tests/test_ruff_lint.py` & `python-lsp-ruff-1.4.0/tests/test_ruff_lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,30 +108,30 @@
         _name, doc = temp_document(DOC, workspace)
         ruff_lint.pylsp_lint(workspace, doc)
 
         (call_args,) = popen_mock.call_args[0]
         assert ruff_executable in call_args
 
 
-def get_ruff_cfg_settings(workspace, doc, config_str):
+def get_ruff_settings(workspace, doc, config_str):
     """Write a ``pyproject.toml``, load it in the workspace, and return the ruff
     settings.
 
     This function creates a ``pyproject.toml``; you'll have to delete it yourself.
     """
 
     with open(
         os.path.join(workspace.root_path, "pyproject.toml"), "w+", encoding="utf-8"
     ) as f:
         f.write(config_str)
 
-    return ruff_lint.load_config(workspace, doc)
+    return ruff_lint.load_settings(workspace, doc.path)
 
 
-def test_ruff_config(workspace):
+def test_ruff_settings(workspace):
     config_str = r"""[tool.ruff]
 ignore = ["F841"]
 exclude = [
     "blah/__init__.py",
     "file_2.py"
 ]
 extend-select = ["D"]
@@ -145,24 +145,30 @@
 def f():
     a = 2
 """
 
     doc_uri = uris.from_fs_path(os.path.join(workspace.root_path, "__init__.py"))
     workspace.put_document(doc_uri, doc_str)
 
-    ruff_settings = get_ruff_cfg_settings(
+    ruff_settings = get_ruff_settings(
         workspace, workspace.get_document(doc_uri), config_str
     )
 
     # Check that user config is ignored
-    for key, value in ruff_settings.items():
-        if key == "executable":
-            assert value == "ruff"
-            continue
-        assert value is None
+    assert ruff_settings.executable == "ruff"
+    empty_keys = [
+        "config",
+        "line_length",
+        "exclude",
+        "select",
+        "ignore",
+        "per_file_ignores",
+    ]
+    for k in empty_keys:
+        assert getattr(ruff_settings, k) is None
 
     with patch("pylsp_ruff.plugin.Popen") as popen_mock:
         mock_instance = popen_mock.return_value
         mock_instance.communicate.return_value = [bytes(), bytes()]
 
         doc = workspace.get_document(doc_uri)
         diags = ruff_lint.pylsp_lint(workspace, doc)
@@ -170,16 +176,15 @@
     call_args = popen_mock.call_args[0][0]
     assert call_args == [
         "ruff",
         "--quiet",
         "--format=json",
         "--no-fix",
         "--force-exclude",
-        "--stdin-filename",
-        os.path.join(workspace.root_path, "__init__.py"),
+        f"--stdin-filename={os.path.join(workspace.root_path, '__init__.py')}",
         "--",
         "-",
     ]
 
     workspace._config.update(
         {
             "plugins": {
@@ -201,15 +206,15 @@
     assert "D104" not in _list
     assert "F841" not in _list
 
     # Excludes
     doc_uri = uris.from_fs_path(os.path.join(workspace.root_path, "blah/__init__.py"))
     workspace.put_document(doc_uri, doc_str)
 
-    ruff_settings = get_ruff_cfg_settings(
+    ruff_settings = get_ruff_settings(
         workspace, workspace.get_document(doc_uri), config_str
     )
 
     doc = workspace.get_document(doc_uri)
     diags = ruff_lint.pylsp_lint(workspace, doc)
     assert diags == []
```

