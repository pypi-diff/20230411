# Comparing `tmp/fabrictestbed-extensions-1.4.2rc2.tar.gz` & `tmp/fabrictestbed-extensions-1.4.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.4.2rc2.tar", last modified: Mon Mar 13 20:14:13 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.4.2rc3.tar", last modified: Mon Apr 10 22:01:45 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.4.2rc2.tar` & `fabrictestbed-extensions-1.4.2rc3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-02-17 15:17:48.718336 fabrictestbed-extensions-1.4.2rc2/.github/workflows/build.yml
--rw-r--r--   0        0        0      687 2023-03-13 16:30:41.657890 fabrictestbed-extensions-1.4.2rc2/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2309 2023-03-13 16:29:41.977358 fabrictestbed-extensions-1.4.2rc2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc2/.gitignore
--rw-r--r--   0        0        0      666 2023-02-17 15:17:48.718336 fabrictestbed-extensions-1.4.2rc2/.readthedocs.yaml
--rw-r--r--   0        0        0      529 2023-03-13 16:30:41.657890 fabrictestbed-extensions-1.4.2rc2/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc2/LICENSE
--rw-r--r--   0        0        0     3625 2023-03-13 16:30:41.657890 fabrictestbed-extensions-1.4.2rc2/README.md
--rw-r--r--   0        0        0      638 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc2/docs/Makefile
--rw-r--r--   0        0        0      799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc2/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc2/docs/source/conf.py
--rw-r--r--   0        0        0     8869 2023-02-17 15:17:40.022255 fabrictestbed-extensions-1.4.2rc2/docs/source/fablib.rst
--rw-r--r--   0        0        0      535 2023-03-13 16:30:41.657890 fabrictestbed-extensions-1.4.2rc2/docs/source/index.rst
--rw-r--r--   0        0        0      151 2023-03-13 20:13:09.832669 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    19993 2023-03-13 16:30:41.657890 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    71048 2023-03-13 16:30:41.661890 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    24778 2023-03-13 16:30:41.661890 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    37762 2023-03-13 16:30:41.665890 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    93938 2023-03-13 19:59:22.691974 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    28974 2023-03-13 16:30:41.665890 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    72777 2023-03-13 19:59:22.691974 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-02-17 15:17:48.718336 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     3372 2023-03-13 16:30:41.669890 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1304 2023-02-17 19:04:16.627066 fabrictestbed-extensions-1.4.2rc2/pyproject.toml
--rwxr-xr-x   0        0        0      122 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc2/sphinx.sh
--rw-r--r--   0        0        0     4815 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc2/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc3/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc3/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/.gitignore
+-rw-r--r--   0        0        0      666 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc3/.readthedocs.yaml
+-rw-r--r--   0        0        0     2130 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/LICENSE
+-rw-r--r--   0        0        0     4054 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc3/README.md
+-rw-r--r--   0        0        0      638 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/docs/Makefile
+-rw-r--r--   0        0        0      799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc3/docs/source/conf.py
+-rw-r--r--   0        0        0     8869 2023-02-17 15:17:40.022255 fabrictestbed-extensions-1.4.2rc3/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc3/docs/source/index.rst
+-rw-r--r--   0        0        0      151 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    20922 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    77033 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5807 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    25514 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    38001 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    94159 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    34672 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    72974 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34231 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-04-02 13:36:30.333332 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-04-10 21:57:28.682104 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1304 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/sphinx.sh
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc3/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/.github/workflows/build.yml` & `fabrictestbed-extensions-1.4.2rc3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/.github/workflows/test.yml` & `fabrictestbed-extensions-1.4.2rc3/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,27 @@
     branches:
       - "main"
   pull_request:
 
 jobs:
   test:
 
-    runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version:
           - "3.9"
           - "3.10"
           - "3.11"
+        os:
+          - "ubuntu-22.04"
+          - "windows-2022"
+          - "macos-11"
+
+    runs-on: ${{ matrix.os }}
 
     steps:
     - name: Check out sources
       uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/.gitignore` & `fabrictestbed-extensions-1.4.2rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/.readthedocs.yaml` & `fabrictestbed-extensions-1.4.2rc3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/LICENSE` & `fabrictestbed-extensions-1.4.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/README.md` & `fabrictestbed-extensions-1.4.2rc3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -51,17 +51,26 @@
 Since FABlib 1.4, API docs can be found [here][fablib-api-rtd]. Older
 API docs are [here][fablib-api-old].
 
 If you want to interact with FABRIC from Jupyter installed on your
 computer, see: [Install the FABRIC Python API][fablib-install].
 
 
-## Testing FABlib
+## Contributing to FABlib
 
-Run tests with [pytest]:
+Contributions to FABlib are made with GitHub Pull Requests. When you
+submit a pull request, some tests will run against it:
+
+- Code formatting will be checked using [black].  Be sure that your
+  code is formatted with black, using its defaults.
+- CHANGELOG.md will be checked for updates.
+- Packages will be built.
+- Unit tests will be run.
+
+You can run tests in your environment, like so, using [pytest]:
 
 ```console
 $ pip install -e .[test]
 $ pytest
 ```
 
 ## Packaging FABlib
@@ -125,8 +134,8 @@
 [fablib-api-old]: https://learn.fabric-testbed.net/docs/fablib/fablib.html
 
 [flit]: https://flit.pypa.io/en/stable/
 [package uploads]: https://flit.pypa.io/en/latest/upload.html
 
 [build]: https://pypi.org/project/build/
 [pytest]: https://pypi.org/project/pytest/
-
+[black]: https://pypi.org/project/black/
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/docs/Makefile` & `fabrictestbed-extensions-1.4.2rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/docs/make.bat` & `fabrictestbed-extensions-1.4.2rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/docs/source/conf.py` & `fabrictestbed-extensions-1.4.2rc3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/docs/source/fablib.rst` & `fabrictestbed-extensions-1.4.2rc3/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/component.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,15 @@
             "details": "Details",
             "disk": "Disk",
             "units": "Units",
             "pci_address": "PCI Address",
             "model": "Model",
             "type": "Type",
             "dev": "Device",
+            "node": "Node",
         }
 
     def toDict(self, skip=[]):
         """
         Returns the component attributes as a dictionary
 
         :return: slice attributes as dictionary
@@ -115,21 +116,24 @@
             "details": str(self.get_details()),
             "disk": str(self.get_disk()),
             "units": str(self.get_unit()),
             "pci_address": str(self.get_pci_addr()),
             "model": str(self.get_model()),
             "type": str(self.get_type()),
             "dev": str(self.get_device_name()),
+            "node": str(self.get_node().get_name()),
         }
 
     def generate_template_context(self):
         context = self.toDict()
         context["interfaces"] = []
-        for interface in self.get_interfaces():
-            context["interfaces"].append(interface.generate_template_context())
+        # for interface in self.get_interfaces():
+        #    context["interfaces"].append(interface.get_name())
+
+        #    context["interfaces"].append(interface.generate_template_context())
         return context
 
     def get_template_context(self):
         return self.get_slice().get_template_context(self)
 
     def render_template(self, input_string):
         environment = jinja2.Environment()
@@ -511,55 +515,73 @@
         Gets the type of this component.
 
         :return: the type of component
         :rtype: str
         """
         return self.get_fim_component().type
 
-    def configure_nvme(self, mount_point="/mnt/nvme_mount"):
+    def configure_nvme(self, mount_point=""):
         """
         Configure the NVMe drive.
 
         Note this works but may be reorganized.
 
-        :param mount_point: The mount point in the filesystem. Default = /mnt/nvme_mount
+        :param mount_point: The mount point in the filesystem. Default = "" later reassigned to /mnt/{linux device name}
         :type mount_point: String
         """
         output = []
         try:
-            output.append(self.node.execute("sudo fdisk -l /dev/nvme*"), quiet=True)
-            output.append(
-                self.node.execute("sudo parted -s /dev/nvme0n1 mklabel gpt"), quiet=True
+            device_pci_id = self.get_pci_addr()[0]
+            stdout, stderr = self.node.execute(
+                f'basename `sudo ls -l /sys/block/nvme*|grep "'
+                f"{device_pci_id}\"|awk '{{print $9}}'`",
+                quiet=True,
             )
+            if stderr != "":
+                output.append(
+                    f"Cannot find NVME device name for PCI ID : {device_pci_id}"
+                )
+                raise Exception
+            device_name = stdout.strip()
+            block_device_name = f"/dev/{device_name}"
+            output.append(self.node.execute(f"sudo fdisk -l {block_device_name}"))
             output.append(
-                self.node.execute("sudo parted -s /dev/nvme0n1 print"), quiet=True
+                self.node.execute(f"sudo parted -s {block_device_name} mklabel gpt")
             )
             output.append(
-                self.node.execute(
-                    "sudo parted -s /dev/nvme0n1 print unit MB print free"
-                ),
-                quiet=True,
+                self.node.execute(f"sudo parted -s {block_device_name} print")
             )
             output.append(
                 self.node.execute(
-                    "sudo parted -s --align optimal /dev/nvme0n1 mkpart primary ext4 0% 960197MB"
-                ),
-                quiet=True,
+                    f"sudo parted -s {block_device_name} print unit MB print free"
+                )
             )
-            output.append(self.node.execute("lsblk /dev/nvme0n1"), quiet=True)
             output.append(
-                self.node.execute("sudo mkfs.ext4 /dev/nvme0n1p1"), quiet=True
+                self.node.execute(
+                    f"sudo parted -s --align optimal "
+                    f"{block_device_name} "
+                    f"mkpart primary ext4 0% 100%"
+                )
             )
+            output.append(self.node.execute(f"lsblk {block_device_name}"))
+            output.append(self.node.execute(f"sudo mkfs.ext4 {block_device_name}p1"))
+            # This is to use a unique mountpoint when it is not provided by the user
+            if mount_point == "":
+                mount_point = f"/mnt/{device_name}"
             output.append(
                 self.node.execute(
-                    f"sudo mkdir {mount_point} && sudo mount /dev/nvme0n1p1 {mount_point}"
-                ),
-                quiet=True,
+                    f"sudo mkdir -p "
+                    f"{mount_point}"
+                    f" && sudo mount "
+                    f"{block_device_name}"
+                    f"p1 "
+                    f"{mount_point}"
+                )
             )
-            output.append(self.node.execute(f"df -h {mount_point}"), quiet=True)
+            output.append(self.node.execute(f"df -h {mount_point}"))
         except Exception as e:
             print(f"config_nvme Fail: {self.get_name()}")
             # traceback.print_exc()
             raise Exception(str(output))
 
         return output
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/fablib.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 if TYPE_CHECKING:
     from fabric_cf.orchestrator.swagger_client import Slice as OrchestratorSlice
 
 from fabrictestbed.slice_manager import SliceManager, Status, SliceState
 from fim.user import Node as FimNode
 
-from fabrictestbed_extensions.fablib.resources import Resources
+from fabrictestbed_extensions.fablib.resources import Resources, Links, FacilityPorts
 from fabrictestbed_extensions.fablib.slice import Slice
 
 
 class fablib:
     default_fablib_manager = None
 
     @staticmethod
@@ -88,14 +88,54 @@
 
         :return: tabulated string of site state
         :rtype: str
         """
         return fablib.get_default_fablib_manager().list_sites()
 
     @staticmethod
+    def list_links() -> object:
+        """
+        Print the links in pretty format
+
+        :return: Formatted list of links
+        :rtype: object
+        """
+        return fablib.get_default_fablib_manager().list_links()
+
+    @staticmethod
+    def get_links() -> str:
+        """
+        Get a string used to print a tabular list of links
+
+        :return: tabulated string of links
+        :rtype: str
+        """
+        return fablib.get_default_fablib_manager().get_links()
+
+    @staticmethod
+    def list_facility_ports() -> object:
+        """
+        Print the facility ports in pretty format
+
+        :return: Formatted list of facility ports
+        :rtype: object
+        """
+        return fablib.get_default_fablib_manager().list_facility_ports()
+
+    @staticmethod
+    def get_facility_ports() -> str:
+        """
+        Get a string used to print a tabular list of facility ports
+
+        :return: tabulated string of facility ports
+        :rtype: str
+        """
+        return fablib.get_default_fablib_manager().get_facility_ports()
+
+    @staticmethod
     def show_site(site_name: str):
         """
         Get a string used to print tabular info about a site
 
         :param site_name: the name of a site
         :type site_name: String
         :return: tabulated string of site state
@@ -603,34 +643,25 @@
         self.ssh_command_line = "ssh ${Username}@${Management IP}"
         self.ssh_config_file = ""
 
         # Setup slice key dict
         # self.slice_keys = {}
         self.default_slice_key = {}
 
-        # Set config values from env vars
-        if Constants.FABRIC_CREDMGR_HOST in os.environ:
-            self.credmgr_host = os.environ[Constants.FABRIC_CREDMGR_HOST]
-
-        if Constants.FABRIC_ORCHESTRATOR_HOST in os.environ:
-            self.orchestrator_host = os.environ[Constants.FABRIC_ORCHESTRATOR_HOST]
-
-        if Constants.FABRIC_TOKEN_LOCATION in os.environ:
-            self.fabric_token = os.environ[Constants.FABRIC_TOKEN_LOCATION]
-
-        if Constants.FABRIC_PROJECT_ID in os.environ:
-            self.project_id = os.environ[Constants.FABRIC_PROJECT_ID]
+        # Set config values from env vars.
+        self.credmgr_host = os.environ.get(Constants.FABRIC_CREDMGR_HOST)
+        self.orchestrator_host = os.environ.get(Constants.FABRIC_ORCHESTRATOR_HOST)
+        self.fabric_token = os.environ.get(Constants.FABRIC_TOKEN_LOCATION)
+        self.project_id = os.environ.get(Constants.FABRIC_PROJECT_ID)
+
+        # Bastion host setup.
+        self.bastion_username = os.environ.get(self.FABRIC_BASTION_USERNAME)
+        self.bastion_key_filename = os.environ.get(self.FABRIC_BASTION_KEY_LOCATION)
+        self.bastion_public_addr = os.environ.get(self.FABRIC_BASTION_HOST)
 
-        # Basstion host setup
-        if self.FABRIC_BASTION_USERNAME in os.environ:
-            self.bastion_username = os.environ[self.FABRIC_BASTION_USERNAME]
-        if self.FABRIC_BASTION_KEY_LOCATION in os.environ:
-            self.bastion_key_filename = os.environ[self.FABRIC_BASTION_KEY_LOCATION]
-        if self.FABRIC_BASTION_HOST in os.environ:
-            self.bastion_public_addr = os.environ[self.FABRIC_BASTION_HOST]
         # if self.FABRIC_BASTION_HOST_PRIVATE_IPV4 in os.environ:
         #    self.bastion_private_ipv4_addr = os.environ[self.FABRIC_BASTION_HOST_PRIVATE_IPV4]
         # if self.FABRIC_BASTION_HOST_PRIVATE_IPV6 in os.environ:
         #    self.bastion_private_ipv6_addr = os.environ[self.FABRIC_BASTION_HOST_PRIVATE_IPV6]
 
         # Slice Keys
         if self.FABRIC_SLICE_PUBLIC_KEY_FILE in os.environ:
@@ -658,21 +689,21 @@
 
         if Constants.FABRIC_CREDMGR_HOST in fabric_rc_dict:
             self.credmgr_host = fabric_rc_dict[Constants.FABRIC_CREDMGR_HOST]
 
         if Constants.FABRIC_ORCHESTRATOR_HOST in fabric_rc_dict:
             self.orchestrator_host = fabric_rc_dict[Constants.FABRIC_ORCHESTRATOR_HOST]
 
-        if "FABRIC_TOKEN_LOCATION" in fabric_rc_dict:
-            self.fabric_token = fabric_rc_dict["FABRIC_TOKEN_LOCATION"]
+        if Constants.FABRIC_TOKEN_LOCATION in fabric_rc_dict:
+            self.fabric_token = fabric_rc_dict[Constants.FABRIC_TOKEN_LOCATION]
             os.environ[Constants.FABRIC_TOKEN_LOCATION] = self.fabric_token
 
-        if "FABRIC_PROJECT_ID" in fabric_rc_dict:
-            self.project_id = fabric_rc_dict["FABRIC_PROJECT_ID"]
-            os.environ["FABRIC_PROJECT_ID"] = self.project_id
+        if Constants.FABRIC_PROJECT_ID in fabric_rc_dict:
+            self.project_id = fabric_rc_dict[Constants.FABRIC_PROJECT_ID]
+            os.environ[Constants.FABRIC_PROJECT_ID] = self.project_id
 
         # Basstion host setup
         if self.FABRIC_BASTION_HOST in fabric_rc_dict:
             self.bastion_public_addr = (
                 fabric_rc_dict[self.FABRIC_BASTION_HOST].strip().strip('"')
             )
         if self.FABRIC_BASTION_USERNAME in fabric_rc_dict:
@@ -748,19 +779,51 @@
         #    logging.basicConfig(filename=self.log_file, level=self.LOG_LEVELS[self.log_level],
         #                        format='[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
         #                        datefmt='%H:%M:%S')
 
         self.bastion_private_ipv4_addr = "0.0.0.0"
         self.bastion_private_ipv6_addr = "0:0:0:0:0:0"
 
+        self._validate_configuration()
+
         # Create slice manager
         self.slice_manager = None
         self.resources = None
+        self.links = None
+        self.facility_ports = None
         self.build_slice_manager()
 
+    def _validate_configuration(self):
+        """
+        Raise an error if we don't have the required configuration.
+        """
+        errors = []
+
+        required_attrs = {
+            "orchestrator_host": "orchestrator host",
+            "credmgr_host": "credmanager host",
+            "fabric_token": "FABRIC token",
+            "project_id": "project ID",
+            "bastion_username": "bastion username",
+            "bastion_key_filename": "bastion key file",
+            "bastion_public_addr": "bastion host address",
+        }
+
+        for attr, value in required_attrs.items():
+            if not hasattr(self, attr) or getattr(self, attr) is None:
+                errors.append(f"{value} is not set")
+
+        if errors:
+            # TODO: define custom exception class to report errors,
+            # and emit a more helpful error message with hints about
+            # setting up environment variables or configuration file.
+            raise AttributeError(
+                f"Error initializing {self.__class__.__name__}: {errors}"
+            )
+
     def get_ssh_thread_pool_executor(self) -> ThreadPoolExecutor:
         return self.ssh_thread_pool_executor
 
     # def set_data_dir(self, data_dir: str):
     #    """
     #    Sets the directory for fablib to store temporary data
     #
@@ -997,14 +1060,106 @@
             output=output,
             fields=fields,
             quiet=quiet,
             filter_function=filter_function,
             pretty_names=pretty_names,
         )
 
+    def list_links(
+        self,
+        output: str = None,
+        fields: str = None,
+        quiet: bool = False,
+        filter_function=None,
+        update: bool = True,
+        pretty_names=True,
+    ) -> object:
+        """
+        Lists all the links and their attributes.
+
+        There are several output options: "text", "pandas", and "json" that determine the format of the
+        output that is returned and (optionally) displayed/printed.
+
+        output:  'text': string formatted with tabular
+                  'pandas': pandas dataframe
+                  'json': string in json format
+
+        fields: json output will include all available fields/columns.
+
+        Example: TODO
+
+        filter_function:  A lambda function to filter data by field values.
+
+        Example: filter_function=lambda s: s['ConnectX-5 Available'] > 3 and s['NVMe Available'] <= 10
+
+        :param output: output format
+        :type output: str
+        :param fields: list of fields (table columns) to show
+        :type fields: List[str]
+        :param quiet: True to specify printing/display
+        :type quiet: bool
+        :param filter_function: lambda function
+        :type filter_function: lambda
+        :return: table in format specified by output parameter
+        :rtype: Object
+        """
+        return self.get_links(update=update).list_links(
+            output=output,
+            fields=fields,
+            quiet=quiet,
+            filter_function=filter_function,
+            pretty_names=pretty_names,
+        )
+
+    def list_facility_ports(
+        self,
+        output: str = None,
+        fields: str = None,
+        quiet: bool = False,
+        filter_function=None,
+        update: bool = True,
+        pretty_names=True,
+    ) -> object:
+        """
+        Lists all the facility ports and their attributes.
+
+        There are several output options: "text", "pandas", and "json" that determine the format of the
+        output that is returned and (optionally) displayed/printed.
+
+        output:  'text': string formatted with tabular
+                  'pandas': pandas dataframe
+                  'json': string in json format
+
+        fields: json output will include all available fields/columns.
+
+        Example: TODO
+
+        filter_function:  A lambda function to filter data by field values.
+
+        Example: filter_function=lambda s: s['ConnectX-5 Available'] > 3 and s['NVMe Available'] <= 10
+
+        :param output: output format
+        :type output: str
+        :param fields: list of fields (table columns) to show
+        :type fields: List[str]
+        :param quiet: True to specify printing/display
+        :type quiet: bool
+        :param filter_function: lambda function
+        :type filter_function: lambda
+        :return: table in format specified by output parameter
+        :rtype: Object
+        """
+        return self.get_facility_ports(update=update).list_facility_ports(
+            output=output,
+            fields=fields,
+            quiet=quiet,
+            filter_function=filter_function,
+            pretty_names=pretty_names,
+        )
+
     def show_config(
         self,
         output: str = None,
         fields: list[str] = None,
         quiet: bool = False,
         pretty_names=True,
     ):
@@ -1085,14 +1240,49 @@
                 fields=fields,
                 output=output,
                 quiet=quiet,
                 pretty_names=pretty_names,
             )
         )
 
+    def get_links(self, update: bool = True) -> Links:
+        """
+        Get the links.
+
+        Optionally update the available resources by querying the FABRIC
+        services. Otherwise, this method returns the existing information.
+
+        :param update:
+        :return: Links
+        """
+
+        if self.links is None:
+            self.links = Links(self)
+        elif update:
+            self.links.update()
+
+        return self.links
+
+    def get_facility_ports(self, update: bool = True) -> FacilityPorts:
+        """
+        Get the facility ports.
+
+        Optionally update the available resources by querying the FABRIC
+        services. Otherwise, this method returns the existing information.
+
+        :param update:
+        :return: Links
+        """
+        if self.facility_ports is None:
+            self.facility_ports = FacilityPorts(self)
+        elif update:
+            self.facility_ports.update()
+
+        return self.facility_ports
+
     def get_resources(self, update: bool = True) -> Resources:
         """
         Get a reference to the resources object. The resources object
         is used to query for available resources and capacities.
 
         :return: the resources object
         :rtype: Resources
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,28 +142,39 @@
             logging.info(
                 f"Getting results from get node name thread for iface {self.get_name()} "
             )
             node_name = self.get_node().get_name()
         else:
             node_name = None
 
+        if self.get_node() and str(self.get_node().get_reservation_state()) == "Active":
+            mac = str(self.get_mac())
+            physical_dev = str(self.get_physical_os_interface_name())
+            dev = str(self.get_os_interface())
+            ip_addr = str(self.get_ip_addr())
+        else:
+            mac = ""
+            physical_dev = ""
+            dev = ""
+            ip_addr = ""
+
         return {
             "name": str(self.get_name()),
             "short_name": str(self.get_short_name()),
             "node": str(node_name),
             "network": str(network_name),
             "bandwidth": str(self.get_bandwidth()),
             "mode": str(self.get_mode()),
             "vlan": str(self.get_vlan())
             if self.get_vlan()
             else "",  # str(self.get_vlan()),
-            "mac": str(self.get_mac()),
-            "physical_dev": str(self.get_physical_os_interface_name()),
-            "dev": str(self.get_os_interface()),
-            "ip_addr": str(self.get_ip_addr()),
+            "mac": mac,
+            "physical_dev": physical_dev,
+            "dev": dev,
+            "ip_addr": ip_addr,
         }
 
     def generate_template_context(self):
         context = self.toDict()
         return context
 
     def get_template_context(self):
@@ -606,25 +617,33 @@
     def get_network(self) -> NetworkService:
         """
         Gets the network this interface is on.
 
         :return: the network service this interface is on
         :rtype: NetworkService
         """
+
         if self.network is not None:
-            # print(f"hasattr(self, 'network'): {hasattr(self, 'network')}, {self.network.get_name()}")
+            logging.debug(
+                f"Interface known network. Returning known network for interface {self.get_name()}"
+            )
             return self.network
         else:
+            logging.debug(
+                f"Interface does not known network. Finding network for interface {self.get_name()}"
+            )
+
             for net in self.get_slice().get_networks():
                 if net.has_interface(self):
                     self.network = net
-                    # print(f"return found network, {self.network.get_name()}")
+                    logging.debug(
+                        f"Interface network found. interface {self.get_name()}, network {self.network.get_name()}"
+                    )
                     return self.network
 
-        # print(f"hasattr(self, 'network'): {hasattr(self, 'network')}, None")
         return None
 
     # fablib.Interface.get_ip_link()
     def get_ip_link(self):
         """
         Gets the ip link info for this interface.
 
@@ -773,35 +792,41 @@
                 addr = ipaddress.ip_address(fablib_data["addr"])
             except:
                 addr = fablib_data["addr"]
             return addr
         else:
             return None
 
-    def set_mode(self, mode: str = "user"):
+    def set_mode(self, mode: str = "config"):
         fablib_data = self.get_fablib_data()
         fablib_data["mode"] = mode
         self.set_fablib_data(fablib_data)
 
         return self
 
     def get_mode(self):
         fablib_data = self.get_fablib_data()
         if "mode" not in fablib_data:
-            self.set_mode("user")
+            self.set_mode("config")
             fablib_data = self.get_fablib_data()
 
         return fablib_data["mode"]
 
     def config(self):
         fablib_data = self.get_fablib_data()
 
         fablib_data = self.get_fablib_data()
-        if "configured" in fablib_data and not bool(fablib_data["configured"]):
+        if "configured" in fablib_data and bool(fablib_data["configured"]):
+            logging.debug(
+                f"interface {self.get_name()} already configured, skipping config."
+            )
             return
+        else:
+            logging.debug(f"interface {self.get_name()} not configured, configuring.")
+
         fablib_data["configured"] = str(True)
         self.set_fablib_data(fablib_data)
 
         if "mode" in fablib_data:
             mode = fablib_data["mode"]
         else:
             mode = "manual"
@@ -810,15 +835,15 @@
             fablib_data["addr"] = str(self.get_network().allocate_ip())
             addr = fablib_data["addr"]
 
             # print(f"auto allocated addr: {addr}")
 
             self.set_fablib_data(fablib_data)
 
-        if mode == "fablib" or mode == "auto":
+        if mode == "config" or mode == "auto":
             subnet = self.get_network().get_subnet()
             if "addr" in fablib_data:
                 addr = fablib_data["addr"]
                 if addr and subnet:
                     self.ip_addr_add(addr=addr, subnet=ipaddress.ip_network(subnet))
         else:
             # manual mode... do nothing
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             except Exception as e:
                 logging.info(
                     f"validate_nstype: skipping interface {interface.get_name()}, likely its a facility port"
                 )
 
         # models: 'NIC_Basic', 'NIC_ConnectX_6', 'NIC_ConnectX_5'
         if type == NetworkService.network_service_map["L2Bridge"]:
-            if not len(sites) <= 0 or len(sites) >= 1:
+            if len(sites) <= 0 or len(sites) > 1:
                 raise Exception(
                     f"Network type {type} must be empty or include interfaces from exactly one site. {len(sites)} sites requested: {sites}"
                 )
 
         elif type == NetworkService.network_service_map["L2PTP"]:
             if not len(sites) == 2:
                 raise Exception(
@@ -558,14 +558,22 @@
             "site": str(self.get_site()),
             "subnet": str(self.get_subnet()),
             "gateway": str(self.get_gateway()),
             "state": str(self.get_reservation_state()),
             "error": str(self.get_error_message()),
         }
 
+    def generate_template_context(self):
+        context = self.toDict()
+        context["interfaces"] = []
+        # for interface in self.get_interfaces():
+        #    context["interfaces"].append(interface.get_name())
+
+        return context
+
     def get_template_context(self):
         return self.get_slice().get_template_context(self)
 
     def render_template(self, input_string):
         environment = jinja2.Environment()
         environment.json_encoder = json.JSONEncoder(ensure_ascii=False)
 
@@ -804,15 +812,15 @@
         try:
             return (
                 self.get_fim_network_service()
                 .get_property(pname="reservation_info")
                 .reservation_id
             )
         except Exception as e:
-            logging.warning(f"Failed to get reservation_id: {e}")
+            logging.debug(f"Failed to get reservation_id: {e}")
             return None
 
     def get_reservation_state(self) -> str or None:
         """
         Gets the reservation state of the network
 
         :return: reservation state
@@ -840,15 +848,14 @@
     def get_interfaces(self) -> List[Interface]:
         """
         Gets the interfaces on this network service.
 
         :return: the interfaces on this network service
         :rtype: List[Interfaces]
         """
-
         interfaces = []
         for interface in self.get_fim_network_service().interface_list:
             logging.debug(f"interface: {interface}")
             interfaces.append(self.get_slice().get_interface(name=interface.name))
 
         return interfaces
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,52 +233,41 @@
         if "site" not in skip:
             rtn_dict["site"] = str(self.get_site())
         if "username" not in skip:
             rtn_dict["username"] = str(self.get_username())
         if "management_ip" not in skip:
             rtn_dict["management_ip"] = (
                 str(self.get_management_ip()).strip()
-                if self.get_management_ip()
+                if str(self.get_reservation_state()) == "Active"
+                and self.get_management_ip()
                 else ""
             )  # str(self.get_management_ip())
         if "state" not in skip:
             rtn_dict["state"] = str(self.get_reservation_state())
         if "error" not in skip:
             rtn_dict["error"] = str(self.get_error_message())
         if "ssh_command" not in skip:
-            rtn_dict["ssh_command"] = str(self.get_ssh_command())
+            if str(self.get_reservation_state()) == "Active":
+                rtn_dict["ssh_command"] = str(self.get_ssh_command())
+            else:
+                rtn_dict["ssh_command"] = ""
         if "public_ssh_key_file" not in skip:
             rtn_dict["public_ssh_key_file"] = str(self.get_public_key_file())
         if "private_ssh_key_file" not in skip:
             rtn_dict["private_ssh_key_file"] = str(self.get_private_key_file())
 
         return rtn_dict
-        # return { "ID":  str(self.get_reservation_id()),
-        #        "Name": str(self.get_name()),
-        #        "Cores": str(self.get_cores()),
-        #        "RAM": str(self.get_ram()),
-        #        "Disk": str(self.get_disk()),
-        #        "Image": str(self.get_image()),
-        #        "Image Type": str(self.get_image_type()),
-        #        "Host": str(self.get_host()),
-        #        "Site": str(self.get_site()),
-        #        "Username" : str(self.get_username()),
-        #        "Management IP": str(self.get_management_ip()),
-        #        "State": str(self.get_reservation_state()),
-        #        "Error": str(self.get_error_message()),
-        #        "SSH Command": str(self.get_ssh_command()),
-        #        "Public SSH Key File": str(self.get_public_key_file()),
-        #        "Private SSH Key File": str(self.get_private_key_file()),
-        #         }
 
     def generate_template_context(self):
         context = self.toDict(skip=["ssh_command"])
         context["components"] = []
-        for component in self.get_components():
-            context["components"].append(component.generate_template_context())
+        # for component in self.get_components():
+        #    context["components"].append(component.get_name())
+
+        #    context["components"].append(component.generate_template_context())
 
         return context
 
     def get_template_context(self):
         return self.get_slice().get_template_context(self, skip=["ssh_command"])
 
     def render_template(self, input_string):
@@ -470,14 +459,20 @@
         :type quiet: bool
         :param filter_function: lambda function
         :type filter_function: lambda
         :return: table in format specified by output parameter
         :rtype: Object
         """
 
+        if str(self.get_reservation_state()) != "Active":
+            logging.debug(
+                f"Node {self.get_name()} is {self.get_reservation_state()}, Skipping get interfaces."
+            )
+            return
+
         ifaces = []
         for iface in self.get_interfaces():
             ifaces.append(iface.get_name())
 
         def combined_filter_function(x):
             if filter_function == None:
                 if x["name"]["value"] in set(ifaces):
@@ -1179,14 +1174,24 @@
         """
         import logging
 
         logging.debug(
             f"execute node: {self.get_name()}, management_ip: {self.get_management_ip()}, command: {command}"
         )
 
+        if not self.get_reservation_state() == "Active":
+            logging.debug(
+                f"Execute failed. Node {self.get_name()} in state {self.get_reservation_state()}"
+            )
+
+        if not self.get_management_ip():
+            logging.debug(
+                f"Execute failed. Node {self.get_name()} in management IP  {self.get_management_ip()}"
+            )
+
         # if not quiet:
         chunking = True
 
         if self.get_fablib_manager().get_log_level() == logging.DEBUG:
             start = time.time()
 
         # Get and test src and management_ips
@@ -1981,15 +1986,15 @@
                     stdout, stderr = self.execute(f"sudo  ip -j addr list", quiet=True)
                     self.ip_addr_list_json = json.loads(stdout)
                     return self.ip_addr_list_json
                 else:
                     stdout, stderr = self.execute(f"sudo ip list", quiet=True)
                     return stdout
         except Exception as e:
-            logging.warning(f"Failed to get ip addr list: {e}")
+            logging.debug(f"Failed to get ip addr list: {e}")
             raise e
 
     def ip_route_add(
         self,
         subnet: Union[IPv4Network, IPv6Network],
         gateway: Union[IPv4Address, IPv6Address],
     ):
@@ -2566,16 +2571,14 @@
                 net_name = route["subnet"].split(".")[0]
                 subnet = self.get_slice().get_network(name=str(net_name)).get_subnet()
 
             # print(f"subnet: {subnet} ({type(subnet)}, next_hop: {next_hop} ({type(next_hop)}")
 
             self.ip_route_add(subnet=ipaddress.ip_network(subnet), gateway=next_hop)
 
-
-
     def run_post_boot_tasks(self, log_dir: str = "."):
         fablib_data = self.get_fablib_data()
         if "post_boot_tasks" in fablib_data:
             commands = fablib_data["post_boot_tasks"]
         else:
             commands = []
 
@@ -2603,19 +2606,29 @@
         for command in commands:
             self.execute(
                 command, quiet=True, output_file=f"{log_dir}/{self.get_name()}.log"
             )
 
     def is_instantiated(self):
         fablib_data = self.get_fablib_data()
+        if "instantiated" not in fablib_data:
+            logging.debug(
+                f"is_instantiated False, {self.get_name()}, fablib_data['instantiated']: does not exist"
+            )
+            return False
+
         if fablib_data["instantiated"] == "True":
-            logging.debug(f"is_instantiated True, {self.get_name()}, fablib_data['instantiated']: {fablib_data['instantiated']}")
+            logging.debug(
+                f"is_instantiated True, {self.get_name()}, fablib_data['instantiated']: {fablib_data['instantiated']}"
+            )
             return True
         else:
-            logging.debug(f"is_instantiated False, {self.get_name()}, fablib_data['instantiated']: {fablib_data['instantiated']}")
+            logging.debug(
+                f"is_instantiated False, {self.get_name()}, fablib_data['instantiated']: {fablib_data['instantiated']}"
+            )
             return False
 
     def set_instantiated(self, instantiated: bool = True):
         fablib_data = self.get_fablib_data()
         fablib_data["instantiated"] = str(instantiated)
         self.set_fablib_data(fablib_data)
 
@@ -2627,15 +2640,14 @@
             return False
 
     def set_run_update_commands(self, run_update_commands: bool = True):
         fablib_data = self.get_fablib_data()
         fablib_data["run_update_commands"] = str(run_update_commands)
         self.set_fablib_data(fablib_data)
 
-
     def config(self, log_dir="."):
         self.execute(f"sudo hostnamectl set-hostname {self.get_name()}", quiet=True)
 
         for iface in self.get_interfaces():
             iface.config()
         self.config_routes()
 
@@ -2643,10 +2655,7 @@
             self.set_instantiated(True)
             self.run_post_boot_tasks()
 
         if self.run_update_commands():
             self.run_post_update_commands()
 
         return "Done"
-
-
-
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
 import logging
 from tabulate import tabulate
-import json
 
 from typing import List, Tuple
+import json
 
 from fabrictestbed.slice_editor import AdvertisedTopology
 from fabrictestbed.slice_editor import Capacities
 from fabrictestbed.slice_manager import Status
+from fim.user import link, interface
 
 
 class Resources:
     site_pretty_names = {
         "name": "Name",
         "state": "State",
         "address": "Address",
@@ -769,7 +770,208 @@
             fields=fields,
             title="Sites",
             output=output,
             quiet=quiet,
             filter_function=filter_function,
             pretty_names_dict=pretty_names_dict,
         )
+
+
+class Links(Resources):
+    link_pretty_names = {
+        "site_names": "Sites",
+        "node_id": "Link Name",
+        "link_capacity_Gbps": "Capacity (Gbps)",
+        "link_layer": "Link Layer",
+    }
+
+    def __init__(self, fablib_manager):
+        """
+        Constructor
+        :return:
+        """
+        super().__init__(fablib_manager)
+
+    def __str__(self) -> str:
+        """
+        Creates a tabulated string of all the links.
+
+        Intended for printing available resources.
+
+        :return: Tabulated string of available resources
+        :rtype: String
+        """
+        table = []
+        for _, link in self.topology.links.items():
+            iface = link.interface_list[0]
+            site_names = iface.name.split("_")
+            if iface.type.name == "TrunkPort" and "HundredGig" not in site_names[0]:
+                table.append(
+                    [
+                        tuple(site_names),
+                        link.node_id,
+                        iface.capacities.bw if iface.capacities else "N/A",
+                        link.layer,
+                    ]
+                )
+
+        return tabulate(
+            table,
+            headers=[
+                "site_names",
+                "node_id",
+                "link_capacity_Gbps",
+                "link_layer",
+            ],
+        )
+
+    def link_to_dict(self, link: link.Link, iface: interface.Interface) -> dict:
+        """
+        Converts the link resources to a dictionary.
+
+        Intended for printing links in table format.
+
+        :return: collection of link properties
+        :rtype: dict
+        """
+        return {
+            "site_names": tuple(iface.name.split("_")),
+            "node_id": link.node_id,
+            "link_capacity_Gbps": iface.capacities.bw if iface.capacities else "N/A",
+            "link_layer": link.layer,
+        }
+
+    def list_links(
+        self,
+        output=None,
+        fields=None,
+        quiet=False,
+        filter_function=None,
+        pretty_names=True,
+    ) -> object:
+        """
+        Print a table of link resources in pretty format.
+
+        :return: formatted table of resources
+        :rtype: object
+        """
+        table = []
+        for _, link in self.topology.links.items():
+            iface = link.interface_list[0]
+            site_names = iface.name.split("_")
+            if iface.type.name == "TrunkPort" and "HundredGig" not in site_names[0]:
+                table.append(self.link_to_dict(link, iface))
+
+        if pretty_names:
+            pretty_names_dict = self.link_pretty_names
+        else:
+            pretty_names_dict = {}
+
+        return self.get_fablib_manager().list_table(
+            table,
+            fields=fields,
+            title="Links",
+            output=output,
+            quiet=quiet,
+            filter_function=filter_function,
+            pretty_names_dict=pretty_names_dict,
+        )
+
+
+class FacilityPorts(Resources):
+    link_pretty_names = {
+        "site_name": "Site",
+        "node_id": "Link Name",
+        "vlan_range": "VLAN Range",
+        "link_layer": "Link Layer",
+    }
+
+    def __init__(self, fablib_manager):
+        """
+        Constructor
+        :return:
+        """
+        super().__init__(fablib_manager)
+
+    def __str__(self) -> str:
+        """
+        Creates a tabulated string of all the links.
+
+        Intended for printing available resources.
+
+        :return: Tabulated string of available resources
+        :rtype: String
+        """
+        table = []
+        for _, link in self.topology.links.items():
+            iface = link.interface_list[0]
+            site_names = iface.name.split("_")
+            if iface.type.name == "FacilityPort":
+                table.append(
+                    [
+                        tuple(site_names),
+                        link.node_id,
+                        iface.labels.vlan_range,
+                        link.layer,
+                    ]
+                )
+
+        return tabulate(
+            table,
+            headers=[
+                "site_name",
+                "node_id",
+                "vlan_range",
+                "link_layer",
+            ],
+        )
+
+    def fp_to_dict(self, link: link.Link, iface: interface.Interface) -> dict:
+        """
+        Converts the link resources to a dictionary.
+
+        Intended for printing links in table format.
+
+        :return: collection of link properties
+        :rtype: dict
+        """
+        return {
+            "site_name": tuple(iface.name.split("_")),
+            "node_id": link.node_id,
+            "vlan_range": iface.labels.vlan_range if iface.labels else "N/A",
+            "link_layer": link.layer,
+        }
+
+    def list_facility_ports(
+        self,
+        output=None,
+        fields=None,
+        quiet=False,
+        filter_function=None,
+        pretty_names=True,
+    ) -> object:
+        """
+        Print a table of link resources in pretty format.
+
+        :return: formatted table of resources
+        :rtype: object
+        """
+        table = []
+        for _, link in self.topology.links.items():
+            iface = link.interface_list[0]
+            if iface.type.name == "FacilityPort":
+                table.append(self.fp_to_dict(link, iface))
+
+        if pretty_names:
+            pretty_names_dict = self.link_pretty_names
+        else:
+            pretty_names_dict = {}
+
+        return self.get_fablib_manager().list_table(
+            table,
+            fields=fields,
+            title="Facility Ports",
+            output=output,
+            quiet=quiet,
+            filter_function=filter_function,
+            pretty_names_dict=pretty_names_dict,
+        )
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,30 +489,34 @@
             context["_self_"] = base_object.generate_template_context()
         else:
             context["_self_"] = {}
 
         context["config"] = self.get_fablib_manager().get_config()
         context["slice"] = self.toDict()
 
-        context["nodes"] = []
+        context["nodes"] = {}
         for node in self.get_nodes():
             node_context = node.generate_template_context()
-            context["nodes"].append(node_context)
+            context["nodes"][node.get_name()] = node_context
 
-        # context["components"] = []
-        # for component in self.get_components():
-        #    context["components"].append(component.toDict())
+        context["components"] = {}
+        for component in self.get_components():
+            context["components"][
+                component.get_name()
+            ] = component.generate_template_context()
 
-        # context["interfaces"] = []
-        # for interface in self.get_interfaces():
-        #    context["interfaces"].append(interface.toDict())
+        context["interfaces"] = {}
+        for interface in self.get_interfaces():
+            context["interfaces"][interface.get_name()] = interface.toDict()
 
-        context["networks"] = []
+        context["networks"] = {}
         for network in self.get_networks():
-            context["networks"].append(network.toDict())
+            context["networks"][
+                network.get_name()
+            ] = network.generate_template_context()
 
         return context
 
     def get_fim_topology(self) -> ExperimentTopology:
         """
         Not recommended for most users.
 
@@ -591,15 +595,15 @@
         """
         Not recommended for most users.  See Slice.update() method.
 
         Updates the slivers with the current slice manager.
 
         :raises Exception: if topology could not be gotten from slice manager
         """
-        logging.info(f"update_slivers: {self.get_name()}")
+        logging.debug(f"update_slivers: {self.get_name()}")
 
         if self.sm_slice is None:
             return
         status, slivers = self.fablib_manager.get_slice_manager().slivers(
             slice_object=self.sm_slice
         )
         if status == Status.OK:
@@ -1557,16 +1561,17 @@
 
         # from concurrent.futures import ThreadPoolExecutor
         my_thread_pool_executor = ThreadPoolExecutor(32)
         threads = {}
 
         for node in self.get_nodes():
             # print(f"Configuring {node.get_name()}")
-            thread = my_thread_pool_executor.submit(node.config)
-            threads[thread] = node
+            if not node.is_instantiated():
+                thread = my_thread_pool_executor.submit(node.config)
+                threads[thread] = node
 
         print(
             f"Running post boot config threads ..."
         )  # ({time.time() - start:.0f} sec)")
 
         for thread in concurrent.futures.as_completed(threads.keys()):
             try:
```

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/pyproject.toml` & `fabrictestbed-extensions-1.4.2rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc2/PKG-INFO` & `fabrictestbed-extensions-1.4.2rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.4.2rc2
+Version: 1.4.2rc3
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -82,17 +82,26 @@
 Since FABlib 1.4, API docs can be found [here][fablib-api-rtd]. Older
 API docs are [here][fablib-api-old].
 
 If you want to interact with FABRIC from Jupyter installed on your
 computer, see: [Install the FABRIC Python API][fablib-install].
 
 
-## Testing FABlib
+## Contributing to FABlib
 
-Run tests with [pytest]:
+Contributions to FABlib are made with GitHub Pull Requests. When you
+submit a pull request, some tests will run against it:
+
+- Code formatting will be checked using [black].  Be sure that your
+  code is formatted with black, using its defaults.
+- CHANGELOG.md will be checked for updates.
+- Packages will be built.
+- Unit tests will be run.
+
+You can run tests in your environment, like so, using [pytest]:
 
 ```console
 $ pip install -e .[test]
 $ pytest
 ```
 
 ## Packaging FABlib
@@ -156,9 +165,9 @@
 [fablib-api-old]: https://learn.fabric-testbed.net/docs/fablib/fablib.html
 
 [flit]: https://flit.pypa.io/en/stable/
 [package uploads]: https://flit.pypa.io/en/latest/upload.html
 
 [build]: https://pypi.org/project/build/
 [pytest]: https://pypi.org/project/pytest/
-
+[black]: https://pypi.org/project/black/
```

