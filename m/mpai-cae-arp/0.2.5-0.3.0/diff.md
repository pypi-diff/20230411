# Comparing `tmp/mpai_cae_arp-0.2.5.tar.gz` & `tmp/mpai_cae_arp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpai_cae_arp-0.2.5.tar", max compression
+gzip compressed data, was "mpai_cae_arp-0.3.0.tar", max compression
```

## Comparing `mpai_cae_arp-0.2.5.tar` & `mpai_cae_arp-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-04-03 21:35:54.975907 mpai_cae_arp-0.2.5/LICENSE
--rw-r--r--   0        0        0      491 2023-04-03 21:22:02.773309 mpai_cae_arp-0.2.5/README.md
--rw-r--r--   0        0        0      276 2023-04-04 08:31:02.533352 mpai_cae_arp-0.2.5/mpai_cae_arp/__init__.py
--rw-r--r--   0        0        0      176 2023-04-04 07:37:21.160932 mpai_cae_arp-0.2.5/mpai_cae_arp/audio/__init__.py
--rw-r--r--   0        0        0    17904 2023-04-06 15:03:52.274016 mpai_cae_arp-0.2.5/mpai_cae_arp/audio/_audio.py
--rw-r--r--   0        0        0     2516 2023-04-04 07:38:52.008419 mpai_cae_arp-0.2.5/mpai_cae_arp/audio/_noise.py
--rw-r--r--   0        0        0      219 2023-04-03 21:48:20.943719 mpai_cae_arp-0.2.5/mpai_cae_arp/audio/standards.py
--rw-r--r--   0        0        0     4211 2023-04-04 07:22:07.372604 mpai_cae_arp-0.2.5/mpai_cae_arp/audio/utils.py
--rw-r--r--   0        0        0     2055 2023-04-10 18:12:57.428996 mpai_cae_arp-0.2.5/mpai_cae_arp/files.py
--rw-r--r--   0        0        0     1304 2023-04-06 14:57:19.804922 mpai_cae_arp-0.2.5/mpai_cae_arp/io.py
--rw-r--r--   0        0        0     3100 2023-04-03 21:32:30.045143 mpai_cae_arp-0.2.5/mpai_cae_arp/time.py
--rw-r--r--   0        0        0        0 2023-04-03 21:25:06.272009 mpai_cae_arp-0.2.5/mpai_cae_arp/types/__init__.py
--rw-r--r--   0        0        0     6902 2023-04-10 17:34:13.680239 mpai_cae_arp-0.2.5/mpai_cae_arp/types/irregularity.py
--rw-r--r--   0        0        0     1668 2023-04-03 21:48:21.015718 mpai_cae_arp-0.2.5/mpai_cae_arp/types/schema.py
--rw-r--r--   0        0        0     1215 2023-04-10 18:13:04.516962 mpai_cae_arp-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 mpai_cae_arp-0.2.5/setup.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 mpai_cae_arp-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-03 21:35:54.975907 mpai_cae_arp-0.3.0/LICENSE
+-rw-r--r--   0        0        0      491 2023-04-03 21:22:02.773309 mpai_cae_arp-0.3.0/README.md
+-rw-r--r--   0        0        0      276 2023-04-04 08:31:02.533352 mpai_cae_arp-0.3.0/mpai_cae_arp/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-04 07:37:21.160932 mpai_cae_arp-0.3.0/mpai_cae_arp/audio/__init__.py
+-rw-r--r--   0        0        0    17904 2023-04-06 15:03:52.274016 mpai_cae_arp-0.3.0/mpai_cae_arp/audio/_audio.py
+-rw-r--r--   0        0        0     2516 2023-04-04 07:38:52.008419 mpai_cae_arp-0.3.0/mpai_cae_arp/audio/_noise.py
+-rw-r--r--   0        0        0      219 2023-04-03 21:48:20.943719 mpai_cae_arp-0.3.0/mpai_cae_arp/audio/standards.py
+-rw-r--r--   0        0        0     4211 2023-04-04 07:22:07.372604 mpai_cae_arp-0.3.0/mpai_cae_arp/audio/utils.py
+-rw-r--r--   0        0        0     2055 2023-04-10 18:12:57.428996 mpai_cae_arp-0.3.0/mpai_cae_arp/files.py
+-rw-r--r--   0        0        0     1304 2023-04-06 14:57:19.804922 mpai_cae_arp-0.3.0/mpai_cae_arp/io.py
+-rw-r--r--   0        0        0     1470 2023-04-11 18:41:39.855128 mpai_cae_arp-0.3.0/mpai_cae_arp/network/arp.proto
+-rw-r--r--   0        0        0     3320 2023-04-11 18:46:42.741189 mpai_cae_arp-0.3.0/mpai_cae_arp/network/arp_pb2.py
+-rw-r--r--   0        0        0    18550 2023-04-11 18:46:53.137122 mpai_cae_arp-0.3.0/mpai_cae_arp/network/arp_pb2_grpc.py
+-rw-r--r--   0        0        0     3100 2023-04-03 21:32:30.045143 mpai_cae_arp-0.3.0/mpai_cae_arp/time.py
+-rw-r--r--   0        0        0        0 2023-04-03 21:25:06.272009 mpai_cae_arp-0.3.0/mpai_cae_arp/types/__init__.py
+-rw-r--r--   0        0        0     6902 2023-04-10 17:34:13.680239 mpai_cae_arp-0.3.0/mpai_cae_arp/types/irregularity.py
+-rw-r--r--   0        0        0     1668 2023-04-03 21:48:21.015718 mpai_cae_arp-0.3.0/mpai_cae_arp/types/schema.py
+-rw-r--r--   0        0        0     1240 2023-04-11 18:41:04.999351 mpai_cae_arp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.0/setup.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.0/PKG-INFO
```

### Comparing `mpai_cae_arp-0.2.5/LICENSE` & `mpai_cae_arp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/audio/_audio.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/audio/_audio.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/audio/_noise.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/audio/_noise.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/audio/utils.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/audio/utils.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/files.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/files.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/io.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/io.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/time.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/time.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/types/irregularity.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/types/irregularity.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/mpai_cae_arp/types/schema.py` & `mpai_cae_arp-0.3.0/mpai_cae_arp/types/schema.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.2.5/pyproject.toml` & `mpai_cae_arp-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "mpai-cae-arp"
-version = "0.2.5"
+version = "0.3.0"
 description = "The MPAI CAE-ARP software API"
 authors = ["Matteo Spanio <dev2@audioinnova.com>"]
 readme = "README.md"
 packages = [{include = "mpai_cae_arp"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "1.23.3"
 pydantic = "^1.10.7"
 pyyaml = "^6.0"
 llvmlite = "^0.39.1"
 librosa = "^0.10.0.post2"
+grpcio-tools = "^1.53.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.2"
 yapf = "^0.32.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.2.1"
```

### Comparing `mpai_cae_arp-0.2.5/setup.py` & `mpai_cae_arp-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['mpai_cae_arp', 'mpai_cae_arp.audio', 'mpai_cae_arp.types']
+['mpai_cae_arp',
+ 'mpai_cae_arp.audio',
+ 'mpai_cae_arp.network',
+ 'mpai_cae_arp.types']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['librosa>=0.10.0.post2,<0.11.0',
+['grpcio-tools>=1.53.0,<2.0.0',
+ 'librosa>=0.10.0.post2,<0.11.0',
  'llvmlite>=0.39.1,<0.40.0',
  'numpy==1.23.3',
  'pydantic>=1.10.7,<2.0.0',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'mpai-cae-arp',
-    'version': '0.2.5',
+    'version': '0.3.0',
     'description': 'The MPAI CAE-ARP software API',
     'long_description': '# MPAI CAE-ARP API\n\n[![LICENSE](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://img.shields.io/badge/license-GPLv3-blue.svg)\n\n## Description\n\nThis package provides a set of tools for common task in MPAI CAE-ARP standard. It is usend in the official implementation of the standard and can be used as well to develop your own.\n\n## License\n\nThis software is licensed under the GPLv3 license. See the [official site](http://www.gnu.org/licenses/gpl-3.0.html) for more information.\n',
     'author': 'Matteo Spanio',
     'author_email': 'dev2@audioinnova.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mpai_cae_arp-0.2.5/PKG-INFO` & `mpai_cae_arp-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mpai-cae-arp
-Version: 0.2.5
+Version: 0.3.0
 Summary: The MPAI CAE-ARP software API
 Author: Matteo Spanio
 Author-email: dev2@audioinnova.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: grpcio-tools (>=1.53.0,<2.0.0)
 Requires-Dist: librosa (>=0.10.0.post2,<0.11.0)
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: numpy (==1.23.3)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
```

