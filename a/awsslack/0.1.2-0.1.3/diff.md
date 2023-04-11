# Comparing `tmp/awsslack-0.1.2.tar.gz` & `tmp/awsslack-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsslack-0.1.2.tar", max compression
+gzip compressed data, was "awsslack-0.1.3.tar", max compression
```

## Comparing `awsslack-0.1.2.tar` & `awsslack-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1691 2023-04-10 19:48:19.044052 awsslack-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-09 18:51:06.063459 awsslack-0.1.2/awsslack/__init__.py
--rw-r--r--   0        0        0      124 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/__main__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:51:06.083459 awsslack-0.1.2/awsslack/commands/__init__.py
--rw-r--r--   0        0        0      778 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/commands/codebuild.py
--rw-r--r--   0        0        0     1208 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/commands/codedeploy.py
--rw-r--r--   0        0        0     8812 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/commands/config.py
--rw-r--r--   0        0        0     2819 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/main.py
--rw-r--r--   0        0        0        0 2023-04-09 18:51:06.067458 awsslack-0.1.2/awsslack/utils/__init__.py
--rw-r--r--   0        0        0     5496 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/utils/code_build.py
--rw-r--r--   0        0        0    10841 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/utils/code_deploy.py
--rw-r--r--   0        0        0      884 2023-04-10 19:48:19.044052 awsslack-0.1.2/awsslack/utils/yaml.py
--rw-r--r--   0        0        0      709 2023-04-10 19:56:40.872798 awsslack-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 awsslack-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1691 2023-04-10 19:48:19.044052 awsslack-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 18:51:06.063459 awsslack-0.1.3/awsslack/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-10 19:48:19.044052 awsslack-0.1.3/awsslack/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:51:06.083459 awsslack-0.1.3/awsslack/commands/__init__.py
+-rw-r--r--   0        0        0      778 2023-04-10 19:48:19.044052 awsslack-0.1.3/awsslack/commands/codebuild.py
+-rw-r--r--   0        0        0     1208 2023-04-10 19:48:19.044052 awsslack-0.1.3/awsslack/commands/codedeploy.py
+-rw-r--r--   0        0        0     8812 2023-04-10 19:48:19.044052 awsslack-0.1.3/awsslack/commands/config.py
+-rw-r--r--   0        0        0     2819 2023-04-10 19:48:19.044052 awsslack-0.1.3/awsslack/main.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:51:06.067458 awsslack-0.1.3/awsslack/utils/__init__.py
+-rw-r--r--   0        0        0     8413 2023-04-11 21:11:31.112996 awsslack-0.1.3/awsslack/utils/code_build.py
+-rw-r--r--   0        0        0    10841 2023-04-10 19:48:19.044052 awsslack-0.1.3/awsslack/utils/code_deploy.py
+-rw-r--r--   0        0        0      884 2023-04-10 19:48:19.044052 awsslack-0.1.3/awsslack/utils/yaml.py
+-rw-r--r--   0        0        0      709 2023-04-11 21:13:20.857042 awsslack-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 awsslack-0.1.3/PKG-INFO
```

### Comparing `awsslack-0.1.2/README.md` & `awsslack-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.2/awsslack/commands/codebuild.py` & `awsslack-0.1.3/awsslack/commands/codebuild.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.2/awsslack/commands/codedeploy.py` & `awsslack-0.1.3/awsslack/commands/codedeploy.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.2/awsslack/commands/config.py` & `awsslack-0.1.3/awsslack/commands/config.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.2/awsslack/main.py` & `awsslack-0.1.3/awsslack/main.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.2/awsslack/utils/code_deploy.py` & `awsslack-0.1.3/awsslack/utils/code_deploy.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.2/awsslack/utils/yaml.py` & `awsslack-0.1.3/awsslack/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `awsslack-0.1.2/pyproject.toml` & `awsslack-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsslack"
-version = "0.1.2"
+version = "0.1.3"
 description = "AWS CodeBuild/CodeDeploy triggers & updates to Slack with a cool Progress Bar!"
 authors = ["Saurabh Chopra <Saurabh.Chopra.2021@live.rhul.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["./scripts", "./tests"]
 
 [tool.poetry.scripts]
```

### Comparing `awsslack-0.1.2/PKG-INFO` & `awsslack-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsslack
-Version: 0.1.2
+Version: 0.1.3
 Summary: AWS CodeBuild/CodeDeploy triggers & updates to Slack with a cool Progress Bar!
 License: MIT
 Author: Saurabh Chopra
 Author-email: Saurabh.Chopra.2021@live.rhul.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

