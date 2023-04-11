# Comparing `tmp/mobio-monitor-system-sdk-1.0.1.tar.gz` & `tmp/mobio-monitor-system-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-monitor-system-sdk-1.0.1.tar", last modified: Tue Apr 11 07:29:58 2023, max compression
+gzip compressed data, was "mobio-monitor-system-sdk-1.0.2.tar", last modified: Tue Apr 11 09:03:35 2023, max compression
```

## Comparing `mobio-monitor-system-sdk-1.0.1.tar` & `mobio-monitor-system-sdk-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 07:29:58.259977 mobio-monitor-system-sdk-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      890 2023-04-11 07:29:58.258977 mobio-monitor-system-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 07:09:44.000000 mobio-monitor-system-sdk-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 07:29:58.249976 mobio-monitor-system-sdk-1.0.1/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 07:29:58.249976 mobio-monitor-system-sdk-1.0.1/mobio/sdks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 07:29:58.252977 mobio-monitor-system-sdk-1.0.1/mobio/sdks/monitor_system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 07:09:44.000000 mobio-monitor-system-sdk-1.0.1/mobio/sdks/monitor_system/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4645 2023-04-11 07:09:44.000000 mobio-monitor-system-sdk-1.0.1/mobio/sdks/monitor_system/initialize_monitor_kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 07:29:58.257977 mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      890 2023-04-11 07:29:58.000000 mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      421 2023-04-11 07:29:58.000000 mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 07:29:58.000000 mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 07:29:58.000000 mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-11 07:29:58.000000 mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 07:29:58.000000 mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-11 07:09:44.000000 mobio-monitor-system-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 07:29:58.259977 mobio-monitor-system-sdk-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9247 2023-04-11 07:29:57.000000 mobio-monitor-system-sdk-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:03:35.502898 mobio-monitor-system-sdk-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-11 09:03:35.502898 mobio-monitor-system-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:58:10.000000 mobio-monitor-system-sdk-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:03:35.493898 mobio-monitor-system-sdk-1.0.2/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:03:35.493898 mobio-monitor-system-sdk-1.0.2/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:03:35.497898 mobio-monitor-system-sdk-1.0.2/mobio/sdks/monitor_system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:58:10.000000 mobio-monitor-system-sdk-1.0.2/mobio/sdks/monitor_system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4685 2023-04-11 08:59:04.000000 mobio-monitor-system-sdk-1.0.2/mobio/sdks/monitor_system/initialize_monitor_kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:03:35.501898 mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-11 09:03:35.000000 mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      421 2023-04-11 09:03:35.000000 mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 09:03:35.000000 mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 09:03:35.000000 mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-11 09:03:35.000000 mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 09:03:35.000000 mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-11 08:58:10.000000 mobio-monitor-system-sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 09:03:35.503898 mobio-monitor-system-sdk-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9247 2023-04-11 09:03:34.000000 mobio-monitor-system-sdk-1.0.2/setup.py
```

### Comparing `mobio-monitor-system-sdk-1.0.1/PKG-INFO` & `mobio-monitor-system-sdk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-monitor-system-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mobio Monitor System SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-monitor-system-sdk-1.0.1/mobio/sdks/monitor_system/initialize_monitor_kafka.py` & `mobio-monitor-system-sdk-1.0.2/mobio/sdks/monitor_system/initialize_monitor_kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import sys
 
 APPLICATION_DATA_DIR = os.environ.get("APPLICATION_DATA_DIR")
 FOLDER_INFORMATION_CONSUMER_DATA_SHARE = 'MonitorSystem/'
 FOLDER_INFORMATION_CONSUMER = 'info-consumer/'
 FOLDER_INFORMATION_CONSUMER_NOT_MONITOR = 'info-consumer-not-monitor/'
 
 STORE_DATA_INFO_CONSUMER = '/info_consumer.json'
@@ -132,9 +133,11 @@
     def start_process(self):
         self.write_info_consumer()
         self.write_info_consumer_not_monitor()
         print('successfully')
 
 
 if __name__ == '__main__':
-    InitializeMonitorKafka('MOBIO_TEMPLATE_HOME').write_info_consumer()
-    InitializeMonitorKafka('MOBIO_TEMPLATE_HOME').write_info_consumer_not_monitor()
+    name_space = sys.argv[1]
+    print(name_space)
+    InitializeMonitorKafka(name_space).write_info_consumer()
+    InitializeMonitorKafka(name_space).write_info_consumer_not_monitor()
```

### Comparing `mobio-monitor-system-sdk-1.0.1/mobio_monitor_system_sdk.egg-info/PKG-INFO` & `mobio-monitor-system-sdk-1.0.2/mobio_monitor_system_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-monitor-system-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mobio Monitor System SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-monitor-system-sdk-1.0.1/setup.py` & `mobio-monitor-system-sdk-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from setuptools import find_namespace_packages, setup
 
+from setuptools import find_namespace_packages, setup
 
 class Readme(object):
     __readme_path = "README.md"
 
     @staticmethod
     def get():
         """get content README.md
@@ -24,15 +24,15 @@
         :param filename:
         :return:
         """
         requirements = ["m-singleton"]
         return requirements
 
 
-version_dev='1.0.1'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_dev='1.0.2'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 version_prod='1.0.0'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode = ''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -48,15 +48,15 @@
     name="mobio-monitor-system-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',  # Required, Phần này cũng không được format file.
+    version='1.0.2',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Monitor System SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

