# Comparing `tmp/alibabacloud-ros-iact3-0.1.0.tar.gz` & `tmp/alibabacloud-ros-iact3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-ros-iact3-0.1.0.tar", last modified: Wed Feb 22 08:23:38 2023, max compression
+gzip compressed data, was "dist/alibabacloud-ros-iact3-0.1.1.tar", last modified: Tue Apr 11 11:58:48 2023, max compression
```

## Comparing `alibabacloud-ros-iact3-0.1.0.tar` & `alibabacloud-ros-iact3-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      111 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10291 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7604 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10291 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      932 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1448 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)      450 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/bin/iact3
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10773 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/
--rw-r--r--   0 root         (0) root         (0)       96 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4177 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/base.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/delete.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/list.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/test.py
--rw-r--r--   0 root         (0) root         (0)    18392 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/config.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    16055 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/generate_params.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/logger.py
--rwxr-xr-x   0 root         (0) root         (0)     1590 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/base_plugin.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/ecs.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/error_code.py
--rw-r--r--   0 root         (0) root         (0)     3550 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/oss.py
--rw-r--r--   0 root         (0) root         (0)     6683 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/ros.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/plugin/vpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/report/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9475 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/report/generate_reports.py
--rw-r--r--   0 root         (0) root         (0)     3805 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/report/html.css
--rw-r--r--   0 root         (0) root         (0)    13220 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/stack.py
--rw-r--r--   0 root         (0) root         (0)     3309 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/termial_print.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/testing/base.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/testing/ros_stack.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/iact3/util.py
--rw-r--r--   0 root         (0) root         (0)       37 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)     1448 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1230 2023-02-22 08:23:38.000000 alibabacloud-ros-iact3-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10291 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7604 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10291 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      450 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/bin/iact3
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10773 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/base.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/delete.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/list.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/test.py
+-rw-r--r--   0 root         (0) root         (0)    18319 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/config.py
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    16055 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/generate_params.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/logger.py
+-rwxr-xr-x   0 root         (0) root         (0)     1590 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/base_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/error_code.py
+-rw-r--r--   0 root         (0) root         (0)     3550 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/oss.py
+-rw-r--r--   0 root         (0) root         (0)     6683 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/ros.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/plugin/vpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9475 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/generate_reports.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/report/html.css
+-rw-r--r--   0 root         (0) root         (0)    13220 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/stack.py
+-rw-r--r--   0 root         (0) root         (0)     3309 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/termial_print.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/base.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/testing/ros_stack.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/iact3/util.py
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 11:58:48.000000 alibabacloud-ros-iact3-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-04-11 11:58:47.000000 alibabacloud-ros-iact3-0.1.1/setup.py
```

### Comparing `alibabacloud-ros-iact3-0.1.0/PKG-INFO` & `alibabacloud-ros-iact3-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros-iact3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.
 Home-page: UNKNOWN
 Author: AlibabaCloud
 License: UNKNOWN
 Description: # What is iact3?
         
         Iact3(IaC Template Testing Tool) is a tool that tests [Terraform](https://developer.hashicorp.com/terraform) and [Alibaba Cloud ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) templates. It deploys your template in multiple Alibaba Cloud Regions and generates a report for each region via a simple configuration file.
```

### Comparing `alibabacloud-ros-iact3-0.1.0/README.md` & `alibabacloud-ros-iact3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/PKG-INFO` & `alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros-iact3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.
 Home-page: UNKNOWN
 Author: AlibabaCloud
 License: UNKNOWN
 Description: # What is iact3?
         
         Iact3(IaC Template Testing Tool) is a tool that tests [Terraform](https://developer.hashicorp.com/terraform) and [Alibaba Cloud ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) templates. It deploys your template in multiple Alibaba Cloud Regions and generates a report for each region via a simple configuration file.
```

### Comparing `alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/SOURCES.txt` & `alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/alibabacloud_ros_iact3.egg-info/requires.txt` & `alibabacloud-ros-iact3-0.1.1/alibabacloud_ros_iact3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/cli.py` & `alibabacloud-ros-iact3-0.1.1/iact3/cli.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/base.py` & `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/base.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/delete.py` & `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/delete.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/list.py` & `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/list.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/cli_modules/test.py` & `alibabacloud-ros-iact3-0.1.1/iact3/cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/config.py` & `alibabacloud-ros-iact3-0.1.1/iact3/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         'Description': 'Role name to use while running test.',
         'Examples': ['my-test-role']
     }
 }
 
 # types
 ParameterKey = NewType('ParameterKey', str)
-ParameterValue = Union[str, int, bool, List[Union[int, str]]]
 TagKey = NewType('TagKey', str)
 TagValue = NewType('TagValue', str)
 Region = NewType('Region', str)
 OssConfigKey = NewType('OssConfigKey', str)
 OssConfigValue = NewType('OssConfigValue', str)
 
 
@@ -305,15 +304,15 @@
 class GeneralConfig(JsonSchemaMixin):
     '''General configuration settings.'''
 
     auth: Auth = field(
         default_factory=Auth, metadata=METADATA[AUTH])
     regions: Optional[List[Region]] = field(
         default_factory=list, metadata=METADATA[REGIONS])
-    parameters: Optional[Dict[ParameterKey, ParameterValue]] = field(
+    parameters: Optional[Dict[ParameterKey, Any]] = field(
         default_factory=dict, metadata=METADATA[PARAMETERS])
     parameters_order: Optional[List[str]] = field(default_factory=list)
     tags: Optional[Dict[TagKey, TagValue]] = field(
         default_factory=dict, metadata=METADATA[TAGS])
     oss_config: Optional[OssConfig] = field(
         default_factory=OssConfig, metadata=METADATA[OSS_CONFIG])
```

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/exceptions.py` & `alibabacloud-ros-iact3-0.1.1/iact3/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/generate_params.py` & `alibabacloud-ros-iact3-0.1.1/iact3/generate_params.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/logger.py` & `alibabacloud-ros-iact3-0.1.1/iact3/logger.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/main.py` & `alibabacloud-ros-iact3-0.1.1/iact3/main.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/plugin/base_plugin.py` & `alibabacloud-ros-iact3-0.1.1/iact3/plugin/base_plugin.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/plugin/ecs.py` & `alibabacloud-ros-iact3-0.1.1/iact3/plugin/ecs.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/plugin/error_code.py` & `alibabacloud-ros-iact3-0.1.1/iact3/plugin/error_code.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/plugin/oss.py` & `alibabacloud-ros-iact3-0.1.1/iact3/plugin/oss.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/plugin/ros.py` & `alibabacloud-ros-iact3-0.1.1/iact3/plugin/ros.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/plugin/vpc.py` & `alibabacloud-ros-iact3-0.1.1/iact3/plugin/vpc.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/report/generate_reports.py` & `alibabacloud-ros-iact3-0.1.1/iact3/report/generate_reports.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/report/html.css` & `alibabacloud-ros-iact3-0.1.1/iact3/report/html.css`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/stack.py` & `alibabacloud-ros-iact3-0.1.1/iact3/stack.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/termial_print.py` & `alibabacloud-ros-iact3-0.1.1/iact3/termial_print.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/testing/base.py` & `alibabacloud-ros-iact3-0.1.1/iact3/testing/base.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/testing/ros_stack.py` & `alibabacloud-ros-iact3-0.1.1/iact3/testing/ros_stack.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/iact3/util.py` & `alibabacloud-ros-iact3-0.1.1/iact3/util.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/requirements.txt` & `alibabacloud-ros-iact3-0.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-iact3-0.1.0/setup.py` & `alibabacloud-ros-iact3-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md") as fp:
     long_description = fp.read()
 
 
 setuptools.setup(
     name="alibabacloud-ros-iact3",
-    version="0.1.0",
+    version="0.1.1",
 
     description="Iact3 is a tool that tests Terraform and ROS(Resource Orchestration Service) templates.",
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     author="AlibabaCloud",
     packages=[
```

