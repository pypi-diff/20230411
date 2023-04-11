# Comparing `tmp/aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0.tar.gz` & `tmp/aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src341352681/src/source/patterns/@aws-solutions-constructs/aws-iot-kinesisstreams/dist/python/aws-solutions-c", last modified: Fri May 20 15:25:40 2022, max compression
+gzip compressed data, was "/codebuild/output/src419658719/src/source/patterns/@aws-solutions-constructs/aws-iot-kinesisstreams/dist/python/aws-solutions-c", last modified: Mon Jun 13 20:50:05 2022, max compression
```

## Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0.tar` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6907 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5995 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1896 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/
--rw-r--r--   0 root         (0) root         (0)    13109 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/
--rw-r--r--   0 root         (0) root         (0)      459 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49347 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/aws-iot-kinesisstreams@2.8.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:29.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6907 2022-05-20 15:25:39.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      718 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 15:25:39.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-05-20 15:25:40.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6920 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6008 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1896 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/
+-rw-r--r--   0 root         (0) root         (0)    13122 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      459 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48958 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/aws-iot-kinesisstreams@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:49:53.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6920 2022-06-13 20:50:04.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-13 20:50:05.000000 aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/LICENSE` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/PKG-INFO` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-iot-kinesisstreams
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS IoT to AWS Kinesis Data Stream.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_iot_kinesisstreams`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-iot-kinesisstreams`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.iotkinesisstreams`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS IoT MQTT topic rule to send data to an Amazon Kinesis Data Stream.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/README.md` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_iot_kinesisstreams`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-iot-kinesisstreams`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.iotkinesisstreams`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS IoT MQTT topic rule to send data to an Amazon Kinesis Data Stream.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/setup.py` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-iot-kinesisstreams",
-    "version": "2.8.0",
+    "version": "2.9.0",
     "description": "CDK Constructs for AWS IoT to AWS Kinesis Data Stream.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_iot_kinesisstreams",
         "aws_solutions_constructs.aws_iot_kinesisstreams._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_iot_kinesisstreams._jsii": [
-            "aws-iot-kinesisstreams@2.8.0.jsii.tgz"
+            "aws-iot-kinesisstreams@2.9.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_iot_kinesisstreams": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.23.0, <3.0.0",
-        "aws-solutions-constructs.core==2.8.0",
+        "aws-solutions-constructs.core==2.9.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.59.0, <2.0.0",
+        "jsii>=1.60.1, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/__init__.py` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs/aws_iot_kinesisstreams/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_iot_kinesisstreams`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-iot-kinesisstreams`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.iotkinesisstreams`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS IoT MQTT topic rule to send data to an Amazon Kinesis Data Stream.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-iot-kinesisstreams
-Version: 2.8.0
+Version: 2.9.0
 Summary: CDK Constructs for AWS IoT to AWS Kinesis Data Stream.
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,16 @@
 
 | **Language**     | **Package**        |
 |:-------------|-----------------|
 |![Python Logo](https://docs.aws.amazon.com/cdk/api/latest/img/python32.png) Python|`aws_solutions_constructs.aws_iot_kinesisstreams`|
 |![Typescript Logo](https://docs.aws.amazon.com/cdk/api/latest/img/typescript32.png) Typescript|`@aws-solutions-constructs/aws-iot-kinesisstreams`|
 |![Java Logo](https://docs.aws.amazon.com/cdk/api/latest/img/java32.png) Java|`software.amazon.awsconstructs.services.iotkinesisstreams`|
 
+## Overview
+
 This AWS Solutions Construct implements an AWS IoT MQTT topic rule to send data to an Amazon Kinesis Data Stream.
 
 Here is a minimal deployable pattern definition:
 
 Typescript
 
 ```python
```

### Comparing `aws-solutions-constructs.aws-iot-kinesisstreams-2.8.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-iot-kinesisstreams-2.9.0/src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/requires.txt
 src/aws_solutions_constructs.aws_iot_kinesisstreams.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_iot_kinesisstreams/__init__.py
 src/aws_solutions_constructs/aws_iot_kinesisstreams/py.typed
 src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/__init__.py
-src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/aws-iot-kinesisstreams@2.8.0.jsii.tgz
+src/aws_solutions_constructs/aws_iot_kinesisstreams/_jsii/aws-iot-kinesisstreams@2.9.0.jsii.tgz
```
