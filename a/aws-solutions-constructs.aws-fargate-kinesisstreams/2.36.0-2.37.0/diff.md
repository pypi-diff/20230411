# Comparing `tmp/aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0.tar.gz` & `tmp/aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src168626414/src/source/patterns/@aws-solutions-constructs/aws-fargate-kinesisstreams/dist/python/aws-solutio", last modified: Wed Mar 29 17:48:10 2023, max compression
+gzip compressed data, was "/codebuild/output/src062777248/src/source/patterns/@aws-solutions-constructs/aws-fargate-kinesisstreams/dist/python/aws-solutio", last modified: Tue Apr 11 17:42:41 2023, max compression
```

## Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0.tar` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9951 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8993 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2012 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/
--rw-r--r--   0 root         (0) root         (0)    37036 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/
--rw-r--r--   0 root         (0) root         (0)      503 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78824 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/aws-fargate-kinesisstreams@2.36.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 17:47:57.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9951 2023-03-29 17:48:09.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      759 2023-03-29 17:48:10.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 17:48:09.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-03-29 17:48:09.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-29 17:48:09.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9951 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8993 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/
+-rw-r--r--   0 root         (0) root         (0)    37036 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77801 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/aws-fargate-kinesisstreams@2.37.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:42:28.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:42:41.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9951 2023-04-11 17:42:40.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-11 17:42:40.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:42:40.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-11 17:42:40.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-11 17:42:40.000000 aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/top_level.txt
```

### Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/LICENSE` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/PKG-INFO` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-fargate-kinesisstreams
-Version: 2.36.0
+Version: 2.37.0
 Summary: CDK Constructs for AWS Fargate to an Amazon Kinesis Data Stream 
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/README.md` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/setup.py` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-solutions-constructs.aws-fargate-kinesisstreams",
-    "version": "2.36.0",
+    "version": "2.37.0",
     "description": "CDK Constructs for AWS Fargate to an Amazon Kinesis Data Stream ",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-solutions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "aws_solutions_constructs.aws_fargate_kinesisstreams",
         "aws_solutions_constructs.aws_fargate_kinesisstreams._jsii"
     ],
     "package_data": {
         "aws_solutions_constructs.aws_fargate_kinesisstreams._jsii": [
-            "aws-fargate-kinesisstreams@2.36.0.jsii.tgz"
+            "aws-fargate-kinesisstreams@2.37.0.jsii.tgz"
         ],
         "aws_solutions_constructs.aws_fargate_kinesisstreams": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.71.0, <3.0.0",
-        "aws-solutions-constructs.core==2.36.0",
+        "aws-cdk-lib>=2.73.0, <3.0.0",
+        "aws-solutions-constructs.core==2.37.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/__init__.py` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs/aws_fargate_kinesisstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/PKG-INFO` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-solutions-constructs.aws-fargate-kinesisstreams
-Version: 2.36.0
+Version: 2.37.0
 Summary: CDK Constructs for AWS Fargate to an Amazon Kinesis Data Stream 
 Home-page: https://github.com/awslabs/aws-solutions-constructs.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-solutions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-solutions-constructs.aws-fargate-kinesisstreams-2.36.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/SOURCES.txt` & `aws-solutions-constructs.aws-fargate-kinesisstreams-2.37.0/src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/SOURCES.txt
 src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/dependency_links.txt
 src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/requires.txt
 src/aws_solutions_constructs.aws_fargate_kinesisstreams.egg-info/top_level.txt
 src/aws_solutions_constructs/aws_fargate_kinesisstreams/__init__.py
 src/aws_solutions_constructs/aws_fargate_kinesisstreams/py.typed
 src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/__init__.py
-src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/aws-fargate-kinesisstreams@2.36.0.jsii.tgz
+src/aws_solutions_constructs/aws_fargate_kinesisstreams/_jsii/aws-fargate-kinesisstreams@2.37.0.jsii.tgz
```

