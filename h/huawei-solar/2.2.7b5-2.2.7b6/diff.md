# Comparing `tmp/huawei-solar-2.2.7b5.tar.gz` & `tmp/huawei-solar-2.2.7b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei-solar-2.2.7b5.tar", last modified: Thu Apr  6 05:36:20 2023, max compression
+gzip compressed data, was "huawei-solar-2.2.7b6.tar", last modified: Tue Apr 11 06:47:43 2023, max compression
```

## Comparing `huawei-solar-2.2.7b5.tar` & `huawei-solar-2.2.7b6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:36:20.509934 huawei-solar-2.2.7b5/
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/.codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/.yamllint
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     7725 2023-04-06 05:36:20.509934 huawei-solar-2.2.7b5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7170 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/bridge_tst.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/requirements_test.txt
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-06 05:36:20.510851 huawei-solar-2.2.7b5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:36:20.496183 huawei-solar-2.2.7b5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:36:20.506267 huawei-solar-2.2.7b5/src/huawei_solar/
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18668 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/files.py
--rw-rw-rw-   0 root         (0) root         (0)    23824 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     6382 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/modbus.py
--rw-rw-rw-   0 root         (0) root         (0)    18080 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/register_names.py
--rw-rw-rw-   0 root         (0) root         (0)    22439 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/register_values.py
--rw-rw-rw-   0 root         (0) root         (0)    42679 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/registers.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/src/huawei_solar/utils.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-06 05:36:20.000000 huawei-solar-2.2.7b5/src/huawei_solar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:36:20.508100 huawei-solar-2.2.7b5/src/huawei_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7725 2023-04-06 05:36:20.000000 huawei-solar-2.2.7b5/src/huawei_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-06 05:36:20.000000 huawei-solar-2.2.7b5/src/huawei_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 05:36:20.000000 huawei-solar-2.2.7b5/src/huawei_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-06 05:36:20.000000 huawei-solar-2.2.7b5/src/huawei_solar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-06 05:36:20.000000 huawei-solar-2.2.7b5/src/huawei_solar.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3577 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:36:20.509934 huawei-solar-2.2.7b5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/tests/mock_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     3531 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/tests/test__registers__peak_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/tests/test__registers__time_of_use.py
--rw-rw-rw-   0 root         (0) root         (0)    16324 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/tests/test_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/tests/test_registers.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-04-06 05:35:58.000000 huawei-solar-2.2.7b5/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.770935 huawei-solar-2.2.7b6/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.yamllint
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     7718 2023-04-11 06:47:43.770935 huawei-solar-2.2.7b6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/bridge_tst.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/requirements_test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-11 06:47:43.771935 huawei-solar-2.2.7b6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.755933 huawei-solar-2.2.7b6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.766934 huawei-solar-2.2.7b6/src/huawei_solar/
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/files.py
+-rw-rw-rw-   0 root         (0) root         (0)    24953 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     6590 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/modbus.py
+-rw-rw-rw-   0 root         (0) root         (0)    18080 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/register_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    22487 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/register_values.py
+-rw-rw-rw-   0 root         (0) root         (0)    42679 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/utils.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.768935 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7718 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.770935 huawei-solar-2.2.7b6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/mock_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3531 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test__registers__peak_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test__registers__time_of_use.py
+-rw-rw-rw-   0 root         (0) root         (0)    16324 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test_registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tox.ini
```

### Comparing `huawei-solar-2.2.7b5/.gitignore` & `huawei-solar-2.2.7b6/.gitignore`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/.gitlab-ci.yml` & `huawei-solar-2.2.7b6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/.pre-commit-config.yaml` & `huawei-solar-2.2.7b6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/LICENSE.md` & `huawei-solar-2.2.7b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/PKG-INFO` & `huawei-solar-2.2.7b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b5
+Version: 2.2.7b6
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,26 +20,26 @@
 [![PyPI version](https://badge.fury.io/py/huawei-solar.svg)](https://badge.fury.io/py/huawei-solar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/huawei-solar.svg)](https://pypi.org/project/huawei-solar/)
 [![PyPI - License](https://img.shields.io/pypi/l/huawei-solar.svg)](https://choosealicense.com/licenses/mit/)
 [![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 # Python library for connecting to Huawei SUN2000 Inverters over Modbus
 
-This library implements an easy to use interface to locally connect to Huawei SUN2000 inverters over 
+This library implements an easy to use interface to locally connect to Huawei SUN2000 inverters over
 Modbus-TCP or Modbus-RTU following the 'Solar Inverter Modbus Interface Definitions' provided by Huawei.
 
 It was primarily developed to add support for Huawei Solar inverters to Home Assistant, resulting
-in the following integration: [wlcrs/huawei_solar](https://github.com/wlcrs/huawei_solar). 
+in the following integration: [wlcrs/huawei_solar](https://github.com/wlcrs/huawei_solar).
 
 **Features:**
-- Modbus-TCP support: connecting to the inverter via the SDongle, or over the WiFi-AP (`SUN2000-<serial_no>`) 
+- Modbus-TCP support: connecting to the inverter via the SDongle, or over the WiFi-AP (`SUN2000-<serial_no>`)
   broadcasted by the inverter
 - Modbus-RTU support: connecting to the inverter via the RS485A1 and RS485B1 pins on the COM port
 - Batched reading of Modbus registers and converting them into the correct units
-- Reading Optimizer data via the specialized 'file' Modbus extension  
+- Reading Optimizer data via the specialized 'file' Modbus extension
 - Writing to Modbus registers (mostly useful for setting battery parameters)
 - Performing the login sequence to gain 'installer'-level access rights
 
 Note t
 
 ## Installation
 
@@ -47,15 +47,15 @@
 
 ```bash
 pip3 install huawei-solar
 ```
 
 ## Basic usage
 
-The library consists out of a low level interface implemented in [huwei_solar.py](src/huawei_solar/huawei_solar.py) which implements all the Modbus-operations, and a high level interface in [bridge.py](src/huawei_solar/bridge.py) which facilitates easy usage (primarily meant for the HA integration). 
+The library consists out of a low level interface implemented in [huwei_solar.py](src/huawei_solar/huawei_solar.py) which implements all the Modbus-operations, and a high level interface in [bridge.py](src/huawei_solar/bridge.py) which facilitates easy usage (primarily meant for the HA integration).
 
 ### Using the high level interface
 
 An example on how to read the most interesting registers from the inverter:
 
 ```py
 bridge = await HuaweiSolarBridge.create(host="192.168.200.1", port=6607)
@@ -88,15 +88,15 @@
 
 results = await self.client.get_multiple([rn.LINE_VOLTAGE_A_B, rn.LINE_VOLTAGE_B_C, rn.LINE_VOLTAGE_C_A], self.slave_id)
 print("A-B voltage: ", results[0].value)
 print("B-C voltage: ", results[1].value)
 print("C-A voltage: ", results[2].value)
 ```
 
-A good starting point to learn how to use the low level interface is to look at how the high level interface in 
+A good starting point to learn how to use the low level interface is to look at how the high level interface in
 [bridge.py](src/huawei_solar/bridge.py) uses it.
 
 # Acknowledgements
 
 The initial implementation of v1 was done by [@Emilv2](https://gitlab.com/Emilv2/huawei-solar/-/tree/1.1.0).
 
 Subsequent developement on v2 was done by [@wlcrs](https://github.com/wlcrs/huawei_solar).
```

### Comparing `huawei-solar-2.2.7b5/README.md` & `huawei-solar-2.2.7b6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 [![PyPI version](https://badge.fury.io/py/huawei-solar.svg)](https://badge.fury.io/py/huawei-solar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/huawei-solar.svg)](https://pypi.org/project/huawei-solar/)
 [![PyPI - License](https://img.shields.io/pypi/l/huawei-solar.svg)](https://choosealicense.com/licenses/mit/)
 [![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 # Python library for connecting to Huawei SUN2000 Inverters over Modbus
 
-This library implements an easy to use interface to locally connect to Huawei SUN2000 inverters over 
+This library implements an easy to use interface to locally connect to Huawei SUN2000 inverters over
 Modbus-TCP or Modbus-RTU following the 'Solar Inverter Modbus Interface Definitions' provided by Huawei.
 
 It was primarily developed to add support for Huawei Solar inverters to Home Assistant, resulting
-in the following integration: [wlcrs/huawei_solar](https://github.com/wlcrs/huawei_solar). 
+in the following integration: [wlcrs/huawei_solar](https://github.com/wlcrs/huawei_solar).
 
 **Features:**
-- Modbus-TCP support: connecting to the inverter via the SDongle, or over the WiFi-AP (`SUN2000-<serial_no>`) 
+- Modbus-TCP support: connecting to the inverter via the SDongle, or over the WiFi-AP (`SUN2000-<serial_no>`)
   broadcasted by the inverter
 - Modbus-RTU support: connecting to the inverter via the RS485A1 and RS485B1 pins on the COM port
 - Batched reading of Modbus registers and converting them into the correct units
-- Reading Optimizer data via the specialized 'file' Modbus extension  
+- Reading Optimizer data via the specialized 'file' Modbus extension
 - Writing to Modbus registers (mostly useful for setting battery parameters)
 - Performing the login sequence to gain 'installer'-level access rights
 
 Note t
 
 ## Installation
 
@@ -30,15 +30,15 @@
 
 ```bash
 pip3 install huawei-solar
 ```
 
 ## Basic usage
 
-The library consists out of a low level interface implemented in [huwei_solar.py](src/huawei_solar/huawei_solar.py) which implements all the Modbus-operations, and a high level interface in [bridge.py](src/huawei_solar/bridge.py) which facilitates easy usage (primarily meant for the HA integration). 
+The library consists out of a low level interface implemented in [huwei_solar.py](src/huawei_solar/huawei_solar.py) which implements all the Modbus-operations, and a high level interface in [bridge.py](src/huawei_solar/bridge.py) which facilitates easy usage (primarily meant for the HA integration).
 
 ### Using the high level interface
 
 An example on how to read the most interesting registers from the inverter:
 
 ```py
 bridge = await HuaweiSolarBridge.create(host="192.168.200.1", port=6607)
@@ -71,15 +71,15 @@
 
 results = await self.client.get_multiple([rn.LINE_VOLTAGE_A_B, rn.LINE_VOLTAGE_B_C, rn.LINE_VOLTAGE_C_A], self.slave_id)
 print("A-B voltage: ", results[0].value)
 print("B-C voltage: ", results[1].value)
 print("C-A voltage: ", results[2].value)
 ```
 
-A good starting point to learn how to use the low level interface is to look at how the high level interface in 
+A good starting point to learn how to use the low level interface is to look at how the high level interface in
 [bridge.py](src/huawei_solar/bridge.py) uses it.
 
 # Acknowledgements
 
 The initial implementation of v1 was done by [@Emilv2](https://gitlab.com/Emilv2/huawei-solar/-/tree/1.1.0).
 
 Subsequent developement on v2 was done by [@wlcrs](https://github.com/wlcrs/huawei_solar).
```

### Comparing `huawei-solar-2.2.7b5/bridge_tst.py` & `huawei-solar-2.2.7b6/bridge_tst.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/pyproject.toml` & `huawei-solar-2.2.7b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/setup.cfg` & `huawei-solar-2.2.7b6/setup.cfg`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/__init__.py` & `huawei-solar-2.2.7b6/src/huawei_solar/__init__.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/bridge.py` & `huawei-solar-2.2.7b6/src/huawei_solar/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         return bridge
 
     @classmethod
     async def create_extra_slave(cls, primary_bridge: "HuaweiSolarBridge", slave_id: int):
         """Creates a HuaweiSolarBridge instance for extra slaves accessible via the given AsyncHuaweiSolar instance."""
         assert primary_bridge.slave_id != slave_id
 
-        await primary_bridge.client._determine_battery_type(slave_id)
+        await primary_bridge.client.determine_battery_type(slave_id)
 
         bridge = cls(
             primary_bridge.client,
             primary_bridge.update_lock,
             primary=False,
             slave_id=slave_id,
         )
@@ -371,18 +371,18 @@
                 return await self.client.set(name, value, slave=self.slave_id)
 
             # we have no login-credentials available, pass on permission error
             raise err
 
     @property
     def battery_type(self) -> rv.StorageProductModel:
+        """The battery type present on this inverter"""
         if self.battery_1_type != rv.StorageProductModel.NONE:
             return self.battery_1_type
-        else:
-            return self.battery_2_type
+        return self.battery_2_type
 
 
 # Registers which should always be read
 INVERTER_REGISTERS = [
     rn.INPUT_POWER,
     rn.LINE_VOLTAGE_A_B,
     rn.LINE_VOLTAGE_B_C,
```

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/exceptions.py` & `huawei-solar-2.2.7b6/src/huawei_solar/exceptions.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/files.py` & `huawei-solar-2.2.7b6/src/huawei_solar/files.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/huawei_solar.py` & `huawei-solar-2.2.7b6/src/huawei_solar/huawei_solar.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,17 +98,18 @@
         self.time_zone = None
         self.battery_type = None
 
     async def _initialize(self):
         # get some registers which are needed to correctly decode all values
 
         self.time_zone = (await self.get(rn.TIME_ZONE)).value
-        await self._determine_battery_type()
+        await self.determine_battery_type()
 
-    async def _determine_battery_type(self, slave_id: t.Optional[int] = None):
+    async def determine_battery_type(self, slave_id: t.Optional[int] = None):
+        """Determine the battery type connected to this inverter"""
         # Skip if the battery type was already determined via another slave
         if self.battery_type is not None and self.battery_type != rv.StorageProductModel.NONE:
             return
 
         try:
             self.battery_type = (await self.get(rn.STORAGE_UNIT_1_PRODUCT_MODEL, slave_id or self.slave)).value
 
@@ -206,14 +207,19 @@
             LOGGER.exception("Aborting client creation due to error.")
             raise ConnectionException from err
 
     async def stop(self):
         """Stop the modbus client."""
         await self._client.close()
 
+    async def _reconnect(self):
+        """Reconnect to the inverter"""
+        await self._client.close()
+        await self._client.connect()
+
     async def _decode_response(self, reg: RegisterDefinition, decoder: BinaryPayloadDecoder):
         """Decodes a modbus register and puts it into a Result object."""
         result = reg.decode(decoder, self)
 
         if not hasattr(reg, "unit") or callable(reg.unit) or isinstance(reg.unit, dict):
             return Result(result, None)
         return Result(result, reg.unit)
@@ -276,28 +282,56 @@
 
         This is solved by sleeping between the first connection and a request,
         and up to 5 retries between following requests.
 
         It seems to only support connections from one device at the same time.
         """
 
+        def on_backoff(details):
+            LOGGER.debug(
+                "Received %s: backing off reading for %0.1f seconds after %d tries",
+                sys.exc_info()[0],
+                details["wait"],
+                details["tries"],
+            )
+
+        def on_backoff_with_reconnect(details):
+            if details.tries % 2 == 0:
+                asyncio.create_task(self._reconnect())
+                LOGGER.debug(
+                    "Received %s: reconnecting and backing off reading for %0.1f seconds after %d tries",
+                    sys.exc_info()[0],
+                    details["wait"],
+                    details["tries"],
+                )
+            else:
+                LOGGER.debug(
+                    "Received %s: backing off reading for %0.1f seconds after %d tries",
+                    sys.exc_info()[0],
+                    details["wait"],
+                    details["tries"],
+                )
+
         def backoff_giveup(details):
             raise ReadException(f"Failed to read register {register} after {details['tries']} tries")
 
         @backoff.on_exception(
             backoff.expo,
-            (asyncio.TimeoutError, SlaveBusyException, SlaveFailureException, ConnectionInterruptedException),
+            (asyncio.TimeoutError),
             max_tries=6,
             jitter=None,
-            on_backoff=lambda details: LOGGER.debug(
-                "Received %s: backing off reading for %0.1f seconds after %d tries",
-                sys.exc_info()[0],
-                details["wait"],
-                details["tries"],
-            ),
+            on_backoff=on_backoff_with_reconnect,
+            on_giveup=backoff_giveup,
+        )
+        @backoff.on_exception(
+            backoff.expo,
+            (SlaveBusyException, SlaveFailureException, ConnectionInterruptedException),
+            max_tries=6,
+            jitter=None,
+            on_backoff=on_backoff,
             on_giveup=backoff_giveup,
         )
         async def _do_read():
             if not self._client.connected:
                 message = "Modbus client is not connected to the inverter."
                 LOGGER.exception(message)
                 raise ConnectionInterruptedException(message)
@@ -506,16 +540,15 @@
                     f"Failed to write value {value} to register {register}: "
                     f"{ModbusExceptions.decode(response.exception_code)}",
                     modbus_exception_code=response.exception_code,
                 )
 
             if single_register:
                 return response.address == register and response.value == value[0]
-            else:
-                return response.address == register and response.count == len(value)
+            return response.address == register and response.count == len(value)
         except ModbusConnectionException as err:
             LOGGER.exception("Failed to connect to device, is the host correct?")
             raise ConnectionInterruptedException(err) from err
 
     async def login(self, username: str, password: str, slave: t.Optional[int] = None):
         """Login into the inverter."""
```

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/modbus.py` & `huawei-solar-2.2.7b6/src/huawei_solar/modbus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Custom classes for pyModbus"""
+
 import asyncio
 import logging
 import struct
 import typing as t
 
 from pymodbus.client import AsyncModbusSerialClient, AsyncModbusTcpClient
 from pymodbus.pdu import ModbusRequest, ModbusResponse
@@ -9,20 +11,24 @@
 RECONNECT_DELAY = 1000  # in milliseconds
 WAIT_ON_CONNECT = 1500  # in milliseconds
 
 LOGGER = logging.getLogger(__name__)
 
 
 class AsyncHuaweiSolarModbusSerialClient(AsyncModbusSerialClient):
+    """Custom SerialClient with support for custom Huawei modbus messages"""
+
     def __init__(self, port, baudrate, timeout: int, **serial_kwargs):
         super().__init__(port, **serial_kwargs, baudrate=baudrate, reconnect_delay=RECONNECT_DELAY, timeout=timeout)
         self.register(PrivateHuaweiModbusResponse)
 
 
 class AsyncHuaweiSolarModbusTcpClient(AsyncModbusTcpClient):
+    """Custom TcpClient that supports wait after connect and custom Huawei modbus messages"""
+
     connected_event = asyncio.Event()
 
     def __init__(self, host, port, timeout) -> AsyncModbusTcpClient:
         super().__init__(host, port, timeout=timeout, reconnect_delay=RECONNECT_DELAY)
         self.register(PrivateHuaweiModbusResponse)
 
     def client_made_connection(self, protocol):
```

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/register_names.py` & `huawei-solar-2.2.7b6/src/huawei_solar/register_names.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/register_values.py` & `huawei-solar-2.2.7b6/src/huawei_solar/register_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,12 +537,14 @@
     """WLAN Wakeup"""
 
     WAKEN_UP = 0
     DISABLED = 1
 
 
 class RemoteChargeDischargeControlMode(IntEnum):
+    """Remote Charge/Discharge Control Mode"""
+
     LOCAL_CONTROL = 0
     REMOTE_CONTROL_MAXIMUM_SELF_CONSUMPTION = 1
     REMOTE_CONTROL_FULLY_FED_TO_GRID = 2
     REMOTE_CONTROL_TOU = 3
     REMOTE_CONTROL_AI_CONTROL = 4
```

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar/registers.py` & `huawei-solar-2.2.7b6/src/huawei_solar/registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar.egg-info/PKG-INFO` & `huawei-solar-2.2.7b6/src/huawei_solar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b5
+Version: 2.2.7b6
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,26 +20,26 @@
 [![PyPI version](https://badge.fury.io/py/huawei-solar.svg)](https://badge.fury.io/py/huawei-solar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/huawei-solar.svg)](https://pypi.org/project/huawei-solar/)
 [![PyPI - License](https://img.shields.io/pypi/l/huawei-solar.svg)](https://choosealicense.com/licenses/mit/)
 [![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 # Python library for connecting to Huawei SUN2000 Inverters over Modbus
 
-This library implements an easy to use interface to locally connect to Huawei SUN2000 inverters over 
+This library implements an easy to use interface to locally connect to Huawei SUN2000 inverters over
 Modbus-TCP or Modbus-RTU following the 'Solar Inverter Modbus Interface Definitions' provided by Huawei.
 
 It was primarily developed to add support for Huawei Solar inverters to Home Assistant, resulting
-in the following integration: [wlcrs/huawei_solar](https://github.com/wlcrs/huawei_solar). 
+in the following integration: [wlcrs/huawei_solar](https://github.com/wlcrs/huawei_solar).
 
 **Features:**
-- Modbus-TCP support: connecting to the inverter via the SDongle, or over the WiFi-AP (`SUN2000-<serial_no>`) 
+- Modbus-TCP support: connecting to the inverter via the SDongle, or over the WiFi-AP (`SUN2000-<serial_no>`)
   broadcasted by the inverter
 - Modbus-RTU support: connecting to the inverter via the RS485A1 and RS485B1 pins on the COM port
 - Batched reading of Modbus registers and converting them into the correct units
-- Reading Optimizer data via the specialized 'file' Modbus extension  
+- Reading Optimizer data via the specialized 'file' Modbus extension
 - Writing to Modbus registers (mostly useful for setting battery parameters)
 - Performing the login sequence to gain 'installer'-level access rights
 
 Note t
 
 ## Installation
 
@@ -47,15 +47,15 @@
 
 ```bash
 pip3 install huawei-solar
 ```
 
 ## Basic usage
 
-The library consists out of a low level interface implemented in [huwei_solar.py](src/huawei_solar/huawei_solar.py) which implements all the Modbus-operations, and a high level interface in [bridge.py](src/huawei_solar/bridge.py) which facilitates easy usage (primarily meant for the HA integration). 
+The library consists out of a low level interface implemented in [huwei_solar.py](src/huawei_solar/huawei_solar.py) which implements all the Modbus-operations, and a high level interface in [bridge.py](src/huawei_solar/bridge.py) which facilitates easy usage (primarily meant for the HA integration).
 
 ### Using the high level interface
 
 An example on how to read the most interesting registers from the inverter:
 
 ```py
 bridge = await HuaweiSolarBridge.create(host="192.168.200.1", port=6607)
@@ -88,15 +88,15 @@
 
 results = await self.client.get_multiple([rn.LINE_VOLTAGE_A_B, rn.LINE_VOLTAGE_B_C, rn.LINE_VOLTAGE_C_A], self.slave_id)
 print("A-B voltage: ", results[0].value)
 print("B-C voltage: ", results[1].value)
 print("C-A voltage: ", results[2].value)
 ```
 
-A good starting point to learn how to use the low level interface is to look at how the high level interface in 
+A good starting point to learn how to use the low level interface is to look at how the high level interface in
 [bridge.py](src/huawei_solar/bridge.py) uses it.
 
 # Acknowledgements
 
 The initial implementation of v1 was done by [@Emilv2](https://gitlab.com/Emilv2/huawei-solar/-/tree/1.1.0).
 
 Subsequent developement on v2 was done by [@wlcrs](https://github.com/wlcrs/huawei_solar).
```

### Comparing `huawei-solar-2.2.7b5/src/huawei_solar.egg-info/SOURCES.txt` & `huawei-solar-2.2.7b6/src/huawei_solar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/test.py` & `huawei-solar-2.2.7b6/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from huawei_solar import AsyncHuaweiSolar
 import asyncio
 
+from huawei_solar import AsyncHuaweiSolar
+
 loop = asyncio.new_event_loop()
 
 
 async def test(names):
 
     hs = await AsyncHuaweiSolar.create("192.168.10.2")
     responses = await hs.get_multiple(names)
```

### Comparing `huawei-solar-2.2.7b5/tests/conftest.py` & `huawei-solar-2.2.7b6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/tests/mock_huawei_solar.py` & `huawei-solar-2.2.7b6/tests/mock_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/tests/test__registers__peak_periods.py` & `huawei-solar-2.2.7b6/tests/test__registers__peak_periods.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/tests/test__registers__time_of_use.py` & `huawei-solar-2.2.7b6/tests/test__registers__time_of_use.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/tests/test_huawei_solar.py` & `huawei-solar-2.2.7b6/tests/test_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/tests/test_registers.py` & `huawei-solar-2.2.7b6/tests/test_registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b5/tox.ini` & `huawei-solar-2.2.7b6/tox.ini`

 * *Files identical despite different names*

