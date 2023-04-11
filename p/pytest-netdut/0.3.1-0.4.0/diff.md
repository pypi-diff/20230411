# Comparing `tmp/pytest_netdut-0.3.1.tar.gz` & `tmp/pytest_netdut-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_netdut-0.3.1.tar", last modified: Wed Jan 11 22:53:47 2023, max compression
+gzip compressed data, was "pytest_netdut-0.4.0.tar", last modified: Tue Apr 11 03:59:03 2023, max compression
```

## Comparing `pytest_netdut-0.3.1.tar` & `pytest_netdut-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.988247 pytest_netdut-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.984247 pytest_netdut-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.984247 pytest_netdut-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-01-11 22:53:47.988247 pytest_netdut-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.984247 pytest_netdut-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.984247 pytest_netdut-0.3.1/docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.984247 pytest_netdut-0.3.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/docs/images/failed_assertion.png
--rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/docs/images/test_showver_results.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.988247 pytest_netdut-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/examples/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/examples/test_eapi_ssh_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/examples/test_showver.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/examples/test_skip_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/examples/test_using_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-11 22:53:47.988247 pytest_netdut-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.984247 pytest_netdut-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.988247 pytest_netdut-0.3.1/src/pytest_netdut/
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/src/pytest_netdut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/src/pytest_netdut/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/src/pytest_netdut/px.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/src/pytest_netdut/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/src/pytest_netdut/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.988247 pytest_netdut-0.3.1/src/pytest_netdut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-01-11 22:53:47.000000 pytest_netdut-0.3.1/src/pytest_netdut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-01-11 22:53:47.000000 pytest_netdut-0.3.1/src/pytest_netdut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 22:53:47.000000 pytest_netdut-0.3.1/src/pytest_netdut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-11 22:53:47.000000 pytest_netdut-0.3.1/src/pytest_netdut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-11 22:53:47.000000 pytest_netdut-0.3.1/src/pytest_netdut.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 22:53:47.988247 pytest_netdut-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/tests/test_netdut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/tests/test_wait_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-11 22:53:31.000000 pytest_netdut-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.596732 pytest_netdut-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.600732 pytest_netdut-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.604733 pytest_netdut-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.596732 pytest_netdut-0.4.0/docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.604733 pytest_netdut-0.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/images/failed_assertion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/images/test_showver_results.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.604733 pytest_netdut-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_eapi_ssh_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_showver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_skip_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_using_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.596732 pytest_netdut-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.608733 pytest_netdut-0.4.0/src/pytest_netdut/
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18701 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.608733 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_netdut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_wait_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tox.ini
```

### Comparing `pytest_netdut-0.3.1/.github/workflows/build.yaml` & `pytest_netdut-0.4.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/.github/workflows/release.yaml` & `pytest_netdut-0.4.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/.gitignore` & `pytest_netdut-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/Dockerfile` & `pytest_netdut-0.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/LICENSE` & `pytest_netdut-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/Makefile` & `pytest_netdut-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/PKG-INFO` & `pytest_netdut-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_netdut
-Version: 0.3.1
+Version: 0.4.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
```

### Comparing `pytest_netdut-0.3.1/README.md` & `pytest_netdut-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/docs/images/failed_assertion.png` & `pytest_netdut-0.4.0/docs/images/failed_assertion.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/docs/images/test_showver_results.png` & `pytest_netdut-0.4.0/docs/images/test_showver_results.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/examples/test_daemon.py` & `pytest_netdut-0.4.0/examples/test_daemon.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/examples/test_eapi_ssh_x.py` & `pytest_netdut-0.4.0/examples/test_eapi_ssh_x.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/examples/test_skip_demo.py` & `pytest_netdut-0.4.0/examples/test_skip_demo.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/mkdocs.yml` & `pytest_netdut-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/setup.cfg` & `pytest_netdut-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/src/pytest_netdut/__init__.py` & `pytest_netdut-0.4.0/src/pytest_netdut/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/src/pytest_netdut/factories.py` & `pytest_netdut-0.4.0/src/pytest_netdut/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import logging
 import re
 import pytest
 from .wrappers import CLI, xapi
 
 
 def create_dut_fixture(name):
-    @pytest.fixture(name=f"{name}")
+    @pytest.fixture(scope="session", name=f"{name}")
     def _dut(request):
         skipper = request.getfixturevalue(f"{name}_skipper")
         skipper(request.node)
 
         class Dut:
             def __getattr__(self, attr):
                 return request.getfixturevalue(f"{name}_{attr}")
```

### Comparing `pytest_netdut-0.3.1/src/pytest_netdut/px.py` & `pytest_netdut-0.4.0/src/pytest_netdut/px.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             self.expect(self._prompt, timeout)
         return self.before.replace("\r\n", "\n")
 
     def sendcmd(self, cmd="", timeout=-1, reset=0, wait=True):
         if not isinstance(self.after, six.string_types) or not self._prompt.match(
             self.after
         ):
-            raise Exception(
+            raise RuntimeError(
                 "Cannot find prompt. Refusing to send command.",
                 self.after,
                 self._prompt.pattern,
             )
 
         self.sendcmd_unchecked(cmd)
 
@@ -333,29 +333,29 @@
         except TIMEOUT:
             # Check if the CLI is busted or if previous tests left a password set
             try:
                 index = self.expect(
                     ["Traceback", "Login incorrect", "Password:"], timeout=10
                 )
                 if index == 0:
-                    raise Exception(  # pylint: disable=raise-missing-from
+                    raise RuntimeError(  # pylint: disable=raise-missing-from
                         "CLI is busted, try logging in as root!"
                     )
                 if index == 1:
                     self.expect("login:", timeout=2)
                     self.sendline(self.username)
                     self.expect(self.username + "(\r)?\r\n", timeout=10)
                     self.expect("Password:", timeout=10)
                     self.sendline("opensesame")  # This is used in some tests.
                     self.expect("Last login:.*\r\n", timeout=10)
                 elif index == 2:
                     self.sendline("opensesame")  # This is used in some tests.
                     self.expect("Last login:.*\r\n", timeout=10)
                 self.expect("Traceback", timeout=10)
-                raise Exception(  # pylint: disable=raise-missing-from
+                raise RuntimeError(  # pylint: disable=raise-missing-from
                     "CLI is busted, try logging in as root!"
                 )
             except TIMEOUT:
                 self.prompt(reset=1)
 
         # Sometime there are weird control characters printed as "^[[0n"
         # on the first line that escape the control code filtering.
@@ -404,15 +404,15 @@
 
                 # Failsafe in case the provided timeout is funky
                 if cli_timeout > 0:
                     self.sendcmd_simple("set timeout {}".format(cli_timeout))
                 else:
                     self.sendcmd_simple("no timeout")
             else:
-                raise Exception("Not at CLI prompt")
+                raise RuntimeError("Not at CLI prompt")
 
     def sendcmd_simple(self, cmd="", timeout=-1, reset=0, wait=True):
         if wait:
             output = Shell.sendcmd(self, cmd, timeout, reset, wait)
             return self.process_output(output)
 
         Shell.sendcmd(self, cmd, timeout, reset, wait)
```

### Comparing `pytest_netdut-0.3.1/src/pytest_netdut/utils.py` & `pytest_netdut-0.4.0/src/pytest_netdut/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/src/pytest_netdut/wrappers.py` & `pytest_netdut-0.4.0/src/pytest_netdut/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         """CLI translator.
 
         Args:
             cmds (str | Iterable[str]): Either an iterable of commands to be run or a newline separated string containing one or more commands.
         """
         commands = []
         for command in _splitcmds(cmds):
-            for (before, after) in self.config_patterns:
+            for before, after in self.config_patterns:
                 matcher = re.match(before, command)
                 if matcher:
                     commands.append(matcher.expand(after))
                     break
             else:
                 # If we don't get a match, just append the original.
                 commands.append(command)
```

### Comparing `pytest_netdut-0.3.1/src/pytest_netdut.egg-info/PKG-INFO` & `pytest_netdut-0.4.0/src/pytest_netdut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-netdut
-Version: 0.3.1
+Version: 0.4.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
```

### Comparing `pytest_netdut-0.3.1/src/pytest_netdut.egg-info/SOURCES.txt` & `pytest_netdut-0.4.0/src/pytest_netdut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/tests/conftest.py` & `pytest_netdut-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/tests/test_netdut.py` & `pytest_netdut-0.4.0/tests/test_netdut.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/tests/test_translator.py` & `pytest_netdut-0.4.0/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/tests/test_wait_for.py` & `pytest_netdut-0.4.0/tests/test_wait_for.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/tests/test_xapi.py` & `pytest_netdut-0.4.0/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.3.1/tox.ini` & `pytest_netdut-0.4.0/tox.ini`

 * *Files identical despite different names*

