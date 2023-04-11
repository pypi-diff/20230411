# Comparing `tmp/aws-credentialer-0.1.0.tar.gz` & `tmp/aws-credentialer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/aws-credentialer/aws-credentialer/dist/.tmp-xj_9wlem/aws-credentialer-0.1.0.tar", last modified: Mon Feb 13 01:25:50 2023, max compression
+gzip compressed data, was "/home/runner/work/aws-credentialer/aws-credentialer/dist/.tmp-7mc2eiy3/aws-credentialer-0.1.2.tar", last modified: Tue Apr 11 15:55:17 2023, max compression
```

## Comparing `aws-credentialer-0.1.0.tar` & `aws-credentialer-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-13 01:25:39.000000 aws-credentialer-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-13 01:25:39.000000 aws-credentialer-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-13 01:25:39.000000 aws-credentialer-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/aws_credentialer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 01:25:39.000000 aws-credentialer-0.1.0/src/aws_credentialer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-02-13 01:25:39.000000 aws-credentialer-0.1.0/src/aws_credentialer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/aws_credentialer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/aws_credentialer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/aws_credentialer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/aws_credentialer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/aws_credentialer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-13 01:25:50.000000 aws-credentialer-0.1.0/src/aws_credentialer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 15:55:03.000000 aws-credentialer-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 15:55:03.000000 aws-credentialer-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 15:55:03.000000 aws-credentialer-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/aws_credentialer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:55:03.000000 aws-credentialer-0.1.2/src/aws_credentialer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-11 15:55:03.000000 aws-credentialer-0.1.2/src/aws_credentialer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/aws_credentialer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/aws_credentialer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/aws_credentialer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/aws_credentialer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/aws_credentialer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 15:55:17.000000 aws-credentialer-0.1.2/src/aws_credentialer.egg-info/top_level.txt
```

### Comparing `aws-credentialer-0.1.0/LICENSE` & `aws-credentialer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-credentialer-0.1.0/PKG-INFO` & `aws-credentialer-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-credentialer
-Version: 0.1.0
+Version: 0.1.2
 Summary: An AWS MFA Credentials Updater
 Author-email: Hidayatullah Ahsan <hahsan@techicon.net>
 Project-URL: Homepage, https://github.com/hahsan-ti/aws-credentialer
 Project-URL: Bug Tracker, https://github.com/hahsan-ti/aws-credentialer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,24 +17,26 @@
 > A convinient way to update AWS credentials for an AWS profile with MFA enforced.
 
 ## Installation
 
 Using `pip`
 
 ```sh
-pip install aws_credentialer
+pip install aws-credentialer
 ```
 
 ## Usage Example
 
 Run the following command in your favorite terminal:
 
 ```sh
 python -m aws_credentialer nnnnnn
 ```
 
 Help is available with the `-h` parameter.
 
 ## Release History
 
+* 0.1.2
+  * Updated packages.
 * 0.1.0
   * The first proper release.
```

### Comparing `aws-credentialer-0.1.0/pyproject.toml` & `aws-credentialer-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "aws-credentialer"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="Hidayatullah Ahsan", email="hahsan@techicon.net" }
 ]
 description = "An AWS MFA Credentials Updater"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
-    "boto3==1.26.69",
-    "botocore==1.29.69",
+    "boto3==1.26.110",
+    "botocore==1.29.110",
     "jmespath==1.0.1",
     "python-dateutil==2.8.2",
     "s3transfer==0.6.0",
     "six==1.16.0",
-    "urllib3==1.26.14",
+    "urllib3==1.26.15",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `aws-credentialer-0.1.0/src/aws_credentialer/__main__.py` & `aws-credentialer-0.1.2/src/aws_credentialer/__main__.py`

 * *Files identical despite different names*

### Comparing `aws-credentialer-0.1.0/src/aws_credentialer.egg-info/PKG-INFO` & `aws-credentialer-0.1.2/src/aws_credentialer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-credentialer
-Version: 0.1.0
+Version: 0.1.2
 Summary: An AWS MFA Credentials Updater
 Author-email: Hidayatullah Ahsan <hahsan@techicon.net>
 Project-URL: Homepage, https://github.com/hahsan-ti/aws-credentialer
 Project-URL: Bug Tracker, https://github.com/hahsan-ti/aws-credentialer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,24 +17,26 @@
 > A convinient way to update AWS credentials for an AWS profile with MFA enforced.
 
 ## Installation
 
 Using `pip`
 
 ```sh
-pip install aws_credentialer
+pip install aws-credentialer
 ```
 
 ## Usage Example
 
 Run the following command in your favorite terminal:
 
 ```sh
 python -m aws_credentialer nnnnnn
 ```
 
 Help is available with the `-h` parameter.
 
 ## Release History
 
+* 0.1.2
+  * Updated packages.
 * 0.1.0
   * The first proper release.
```

