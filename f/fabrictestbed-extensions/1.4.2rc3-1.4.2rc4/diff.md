# Comparing `tmp/fabrictestbed-extensions-1.4.2rc3.tar.gz` & `tmp/fabrictestbed-extensions-1.4.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.4.2rc3.tar", last modified: Mon Apr 10 22:01:45 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.4.2rc4.tar", last modified: Tue Apr 11 21:37:27 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.4.2rc3.tar` & `fabrictestbed-extensions-1.4.2rc4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc3/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc3/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/.gitignore
--rw-r--r--   0        0        0      666 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc3/.readthedocs.yaml
--rw-r--r--   0        0        0     2130 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/LICENSE
--rw-r--r--   0        0        0     4054 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc3/README.md
--rw-r--r--   0        0        0      638 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/docs/Makefile
--rw-r--r--   0        0        0      799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc3/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc3/docs/source/conf.py
--rw-r--r--   0        0        0     8869 2023-02-17 15:17:40.022255 fabrictestbed-extensions-1.4.2rc3/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc3/docs/source/index.rst
--rw-r--r--   0        0        0      151 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    20922 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    77033 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    25514 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    38001 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    94159 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    34672 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    72974 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-04-02 13:36:30.333332 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-04-10 21:57:28.682104 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1304 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc3/pyproject.toml
--rwxr-xr-x   0        0        0      122 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc3/sphinx.sh
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc3/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-02-17 18:08:19.627880 fabrictestbed-extensions-1.4.2rc4/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-04-07 02:35:56.572672 fabrictestbed-extensions-1.4.2rc4/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-04-07 02:36:06.076705 fabrictestbed-extensions-1.4.2rc4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2022-11-25 02:08:11.401934 fabrictestbed-extensions-1.4.2rc4/.gitignore
+-rw-r--r--   0        0        0      666 2023-02-17 18:08:19.628880 fabrictestbed-extensions-1.4.2rc4/.readthedocs.yaml
+-rw-r--r--   0        0        0     2130 2023-04-11 21:36:26.791911 fabrictestbed-extensions-1.4.2rc4/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2022-11-25 02:08:11.402934 fabrictestbed-extensions-1.4.2rc4/LICENSE
+-rw-r--r--   0        0        0     4054 2023-04-03 14:05:06.148272 fabrictestbed-extensions-1.4.2rc4/README.md
+-rw-r--r--   0        0        0      638 2022-11-25 02:08:11.402934 fabrictestbed-extensions-1.4.2rc4/docs/Makefile
+-rw-r--r--   0        0        0      799 2022-11-25 02:08:11.402934 fabrictestbed-extensions-1.4.2rc4/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-01-17 14:22:08.133013 fabrictestbed-extensions-1.4.2rc4/docs/source/conf.py
+-rw-r--r--   0        0        0     8869 2023-01-30 21:29:15.591148 fabrictestbed-extensions-1.4.2rc4/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-04-03 14:05:06.149272 fabrictestbed-extensions-1.4.2rc4/docs/source/index.rst
+-rw-r--r--   0        0        0      151 2023-04-11 21:36:26.832911 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-01-17 14:22:08.134013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-02-17 18:08:11.386871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-02-17 18:08:11.386871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-02-17 18:08:11.386871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2022-11-25 02:08:11.404934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-01-30 23:39:04.228930 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    20922 2023-04-11 21:29:21.986065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    77033 2023-04-11 21:36:26.756911 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5807 2023-02-17 18:08:11.387871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    25514 2023-04-11 21:29:21.986065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    37982 2023-04-11 21:29:21.987065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    94159 2023-04-11 21:29:21.987065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    34672 2023-04-11 21:36:26.757911 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    72795 2023-04-11 21:29:21.988065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-01-17 14:22:08.137013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2022-11-25 02:08:11.407934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2022-11-25 02:08:11.407934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2022-11-25 02:08:11.408934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-02-17 18:05:26.140992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-02-17 18:08:11.388871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34231 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-02-17 18:05:26.142992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-02-17 18:05:26.143992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-02-17 18:05:26.144992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-02-17 18:05:26.145992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-04-03 14:05:06.152272 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-01-17 14:22:08.139013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-01-30 23:39:04.236930 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-01-17 14:22:08.139013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1304 2023-02-17 18:08:19.628880 fabrictestbed-extensions-1.4.2rc4/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2022-11-25 02:08:11.409934 fabrictestbed-extensions-1.4.2rc4/sphinx.sh
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc4/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.4.2rc3/.github/workflows/build.yml` & `fabrictestbed-extensions-1.4.2rc4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.4.2rc4/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/.github/workflows/test.yml` & `fabrictestbed-extensions-1.4.2rc4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/.gitignore` & `fabrictestbed-extensions-1.4.2rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/.readthedocs.yaml` & `fabrictestbed-extensions-1.4.2rc4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/CHANGELOG.md` & `fabrictestbed-extensions-1.4.2rc4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/LICENSE` & `fabrictestbed-extensions-1.4.2rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/README.md` & `fabrictestbed-extensions-1.4.2rc4/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/docs/Makefile` & `fabrictestbed-extensions-1.4.2rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/docs/make.bat` & `fabrictestbed-extensions-1.4.2rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/docs/source/conf.py` & `fabrictestbed-extensions-1.4.2rc4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/docs/source/fablib.rst` & `fabrictestbed-extensions-1.4.2rc4/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/docs/source/index.rst` & `fabrictestbed-extensions-1.4.2rc4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/interface.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             except Exception as e:
                 logging.info(
                     f"validate_nstype: skipping interface {interface.get_name()}, likely its a facility port"
                 )
 
         # models: 'NIC_Basic', 'NIC_ConnectX_6', 'NIC_ConnectX_5'
         if type == NetworkService.network_service_map["L2Bridge"]:
-            if len(sites) <= 0 or len(sites) > 1:
+            if len(sites) > 1:
                 raise Exception(
                     f"Network type {type} must be empty or include interfaces from exactly one site. {len(sites)} sites requested: {sites}"
                 )
 
         elif type == NetworkService.network_service_map["L2PTP"]:
             if not len(sites) == 2:
                 raise Exception(
```

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1922,18 +1922,14 @@
             # return 'color: %s' % color
             return "background-color: %s" % color
 
         table = []
         for network in self.get_networks():
             table.append(network.toDict())
 
-        # if fields == None:
-        #    fields = ["ID", "Name", "Layer", "Type",
-        #              "Site", "Gateway", "L3 Subnet", "State",
-        #              "Error"]
         if pretty_names:
             pretty_names_dict = NetworkService.get_pretty_name_dict()
         else:
             pretty_names_dict = {}
 
         logging.debug(f"network service: pretty_names_dict = {pretty_names_dict}")
```

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/pyproject.toml` & `fabrictestbed-extensions-1.4.2rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc3/PKG-INFO` & `fabrictestbed-extensions-1.4.2rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.4.2rc3
+Version: 1.4.2rc4
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

