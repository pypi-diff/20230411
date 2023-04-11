# Comparing `tmp/sharry-jira-tool-0.2.4.tar.gz` & `tmp/sharry-jira-tool-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharry-jira-tool-0.2.4.tar", last modified: Fri Mar 24 07:38:22 2023, max compression
+gzip compressed data, was "sharry-jira-tool-0.2.5.tar", last modified: Tue Apr 11 06:33:53 2023, max compression
```

## Comparing `sharry-jira-tool-0.2.4.tar` & `sharry-jira-tool-0.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 07:38:22.768889 sharry-jira-tool-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-03-24 07:38:22.768889 sharry-jira-tool-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 07:38:22.768889 sharry-jira-tool-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 07:38:22.764889 sharry-jira-tool-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 07:38:22.764889 sharry-jira-tool-0.2.4/src/jira_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 07:38:22.764889 sharry-jira-tool-0.2.4/src/jira_tool/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/assets/excel_definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/assets/sprint_schedule.json
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/src/jira_tool/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 07:38:22.764889 sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-03-24 07:38:22.000000 sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-24 07:38:22.000000 sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 07:38:22.000000 sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-24 07:38:22.000000 sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-24 07:38:22.000000 sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-24 07:38:22.000000 sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 07:38:22.768889 sharry-jira-tool-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-03-24 07:38:11.000000 sharry-jira-tool-0.2.4/tests/test_story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.814945 sharry-jira-tool-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.814945 sharry-jira-tool-0.2.5/src/jira_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.814945 sharry-jira-tool-0.2.5/src/jira_tool/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/assets/excel_definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/assets/sprint_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_story.py
```

### Comparing `sharry-jira-tool-0.2.4/LICENSE` & `sharry-jira-tool-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/PKG-INFO` & `sharry-jira-tool-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharry-jira-tool
-Version: 0.2.4
+Version: 0.2.5
 Summary: Sort Jira stories in Excel
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
+Important!!!
+============
+We will no longer add new features or fix bugs for this project. 
+All new features/requirements/bug fixes will be move to package: jira-assistant <https://pypi.org/project/jira-assistant>.
+Welcome to provide your good advices as always!
+
 Jira Tool - userful tool to sort jira stories
 =============================================
 
 |pypi| |python 3.11| |python 3.11 (Mac OS)| |CodeQL| |Documentation|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/sharry-jira-tool.svg?style=flat-square
     :target https://pypi.org/project/sharry-jira-tool/
```

### Comparing `sharry-jira-tool-0.2.4/README.rst` & `sharry-jira-tool-0.2.5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Important!!!
+============
+We will no longer add new features or fix bugs for this project. 
+All new features/requirements/bug fixes will be move to package: jira-assistant <https://pypi.org/project/jira-assistant>.
+Welcome to provide your good advices as always!
+
 Jira Tool - userful tool to sort jira stories
 =============================================
 
 |pypi| |python 3.11| |python 3.11 (Mac OS)| |CodeQL| |Documentation|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/sharry-jira-tool.svg?style=flat-square
     :target https://pypi.org/project/sharry-jira-tool/
```

### Comparing `sharry-jira-tool-0.2.4/pyproject.toml` & `sharry-jira-tool-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sharry-jira-tool"
-version = "0.2.4"
+version = "0.2.5"
 description = "Sort Jira stories in Excel"
 readme = "README.rst"
 authors = [{ name = "Sharry Xu", email = "sharry.xu@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -35,8 +35,8 @@
 
 [tool.setuptools.package-data]
 "jira_tool.assets" = ["*.json", "*.conf"]
 
 [project.scripts]
 sort-excel-file = "jira_tool:sort_excel_file"
 generate-template = "jira_tool:generate_template"
-update-jira-info = "jira_tool:update_jira_info"
+update-jira-info = "jira_tool:update_jira_info"
```

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/__init__.py` & `sharry-jira-tool-0.2.5/src/jira_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/assets/excel_definition.json` & `sharry-jira-tool-0.2.5/src/jira_tool/assets/excel_definition.json`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/assets/sprint_schedule.json` & `sharry-jira-tool-0.2.5/src/jira_tool/assets/sprint_schedule.json`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/console_script.py` & `sharry-jira-tool-0.2.5/src/jira_tool/console_script.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/excel_definition.py` & `sharry-jira-tool-0.2.5/src/jira_tool/excel_definition.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/excel_operation.py` & `sharry-jira-tool-0.2.5/src/jira_tool/excel_operation.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/jira_client.py` & `sharry-jira-tool-0.2.5/src/jira_tool/jira_client.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/milestone.py` & `sharry-jira-tool-0.2.5/src/jira_tool/milestone.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/priority.py` & `sharry-jira-tool-0.2.5/src/jira_tool/priority.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/sprint_schedule.py` & `sharry-jira-tool-0.2.5/src/jira_tool/sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/jira_tool/story.py` & `sharry-jira-tool-0.2.5/src/jira_tool/story.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/PKG-INFO` & `sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharry-jira-tool
-Version: 0.2.4
+Version: 0.2.5
 Summary: Sort Jira stories in Excel
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
+Important!!!
+============
+We will no longer add new features or fix bugs for this project. 
+All new features/requirements/bug fixes will be move to package: jira-assistant <https://pypi.org/project/jira-assistant>.
+Welcome to provide your good advices as always!
+
 Jira Tool - userful tool to sort jira stories
 =============================================
 
 |pypi| |python 3.11| |python 3.11 (Mac OS)| |CodeQL| |Documentation|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/sharry-jira-tool.svg?style=flat-square
     :target https://pypi.org/project/sharry-jira-tool/
```

### Comparing `sharry-jira-tool-0.2.4/src/sharry_jira_tool.egg-info/SOURCES.txt` & `sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_console_script.py` & `sharry-jira-tool-0.2.5/tests/test_console_script.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_excel_definition.py` & `sharry-jira-tool-0.2.5/tests/test_excel_definition.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_excel_operation.py` & `sharry-jira-tool-0.2.5/tests/test_excel_operation.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_jira_client.py` & `sharry-jira-tool-0.2.5/tests/test_jira_client.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_milestone.py` & `sharry-jira-tool-0.2.5/tests/test_milestone.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_priority.py` & `sharry-jira-tool-0.2.5/tests/test_priority.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_sprint_schedule.py` & `sharry-jira-tool-0.2.5/tests/test_sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.4/tests/test_story.py` & `sharry-jira-tool-0.2.5/tests/test_story.py`

 * *Files identical despite different names*

