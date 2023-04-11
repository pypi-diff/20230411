# Comparing `tmp/jira-assistant-0.1.6.tar.gz` & `tmp/jira-assistant-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-assistant-0.1.6.tar", last modified: Mon Apr  3 08:02:20 2023, max compression
+gzip compressed data, was "jira-assistant-0.1.7.tar", last modified: Tue Apr 11 06:21:25 2023, max compression
```

## Comparing `jira-assistant-0.1.6.tar` & `jira-assistant-0.1.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:02:20.688803 jira-assistant-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-03 08:02:20.688803 jira-assistant-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 08:02:20.688803 jira-assistant-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:02:20.676803 jira-assistant-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:02:20.680803 jira-assistant-0.1.6/src/jira_assistant/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:02:20.684803 jira-assistant-0.1.6/src/jira_assistant/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/assets/excel_definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/assets/sprint_schedule.json
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/src/jira_assistant/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:02:20.684803 jira-assistant-0.1.6/src/jira_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-03 08:02:20.000000 jira-assistant-0.1.6/src/jira_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-03 08:02:20.000000 jira-assistant-0.1.6/src/jira_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 08:02:20.000000 jira-assistant-0.1.6/src/jira_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-03 08:02:20.000000 jira-assistant-0.1.6/src/jira_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-03 08:02:20.000000 jira-assistant-0.1.6/src/jira_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-03 08:02:20.000000 jira-assistant-0.1.6/src/jira_assistant.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:02:20.688803 jira-assistant-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-03 08:02:10.000000 jira-assistant-0.1.6/tests/test_story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.588825 jira-assistant-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.588825 jira-assistant-0.1.7/src/jira_assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/src/jira_assistant/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/assets/excel_definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/assets/sprint_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/src/jira_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_story.py
```

### Comparing `jira-assistant-0.1.6/LICENSE` & `jira-assistant-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/PKG-INFO` & `jira-assistant-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-assistant
-Version: 0.1.6
+Version: 0.1.7
 Summary: Useful Jira tools
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,24 +34,28 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 Jira Assistant - userful jira tools
 =============================================
 
-|pypi| |Download| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate|
+|pypi| |Download| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/jira-assistant.svg?style=flat-square
     :target https://pypi.org/project/jira-assistant/
     :alt: pypi version
 
 .. |Download| image:: https://static.pepy.tech/personalized-badge/jira-assistant?period=month&units=international_system&left_color=black&right_color=blue&left_text=downloads/month
     :target: https://pepy.tech/project/jira-assistant
     :alt: download
 
+.. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
+   :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
+   :alt: GitHub issues
+
 .. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
     :alt: python 3.11 (Linux)
 
 .. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml
     :alt: python 3.11 (Mac OS)
@@ -76,14 +80,22 @@
     :target: https://codecov.io/gh/SharryXu/jira-assistant
     :alt: Codecov
 
 .. |CodeClimate| image:: https://api.codeclimate.com/v1/badges/aeae36dcbb250784672b/maintainability
    :target: https://codeclimate.com/github/SharryXu/jira-assistant/maintainability
    :alt: Maintainability
 
+.. |License| image:: https://img.shields.io/github/license/sharryxu/jira-assistant
+   :target: https://img.shields.io/github/license/sharryxu/jira-assistant
+   :alt: License
+
+Collecting Ideas!!!
+===================
+If you have any ideas or good requirements related to this package, please let us know and we will do our best to fulfill! Please send emails to <sharry.xu@outlook.com>.
+
 Installation
 ============
 `jira-assistant` can be installed from PyPI using `pip` (note that the package name is different from the importable name)::
 
     pip install -U jira-assistant
 
 Download
@@ -102,15 +114,14 @@
 * Parsing the excel file which usually been downloaded from the Jira platform.
 * Sorting the excel records using some specific logic.
 * Generating the target excel file which contains the result.
 * The excel file structure can be customized by JSON file.
 
 A Simple Example
 ================
-
 You can run below command in the PowerShell (Windows OS) or Shell (UNIX OS) to process the excel files.
 
 .. code-block:: console
 
     process-excel-file source.xlsx
 
 After that, you can find the output file in the same folder along with the source file. 
@@ -139,27 +150,26 @@
 .. code-block:: console
 
     generate-template -h
 
 
 Code Example For Developer
 ==========================
-
 Here's a simple program, just to give you an idea about how to use this package.
 
 .. code-block:: python
 
   import pathlib
   from jira_assistant import run_steps_and_sort_excel_file
   HERE = pathlib.Path().resolve()
   run_steps_and_sort_excel_file(HERE / "source.xlsx", HERE / "target.xlsx")
 
 If you want to customize the definition file to adapt the new Excel, you can do below steps.
 
-1. Creating the definition file like below. Inside the :code:`PreProcessSteps` list, you can determine the procedure which will be triggered before sorting and also inside the :code:`SortStrategyPriority` list, you can decide the sort algorithms' order.
+1. Creating the definition file like below. Inside the :code:`PreProcessSteps` list, you can determine the procedure which will be triggered before sorting and also inside the :code:`SortStrategyPriority` list, you can decide the sort algorithms' order. Note: We need to make sure there is one column named ``StoryId`` and only one.
 
 .. code-block:: json
 
   [
       {
           "PreProcessSteps": [
               {
@@ -267,16 +277,12 @@
       sprint_schedule_file=HERE / "milestone_priority.json"
   )
 
 Author
 ======
 The jira-assistant was written by Sharry Xu <sharry.xu@outlook.com> in 2022.
 
-Starting with version 0.1.13, the main function of this project has been totally finished.
-
-Contact
-=======
-Our mailing list is available at `sharry.xu@outlook.com`.
+Starting with version 0.1.5, the main function of this project has been totally finished.
 
 License
 =======
 All contributions after December 1, 2022 released under MIT license.
```

### Comparing `jira-assistant-0.1.6/README.rst` & `jira-assistant-0.1.7/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Jira Assistant - userful jira tools
 =============================================
 
-|pypi| |Download| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate|
+|pypi| |Download| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/jira-assistant.svg?style=flat-square
     :target https://pypi.org/project/jira-assistant/
     :alt: pypi version
 
 .. |Download| image:: https://static.pepy.tech/personalized-badge/jira-assistant?period=month&units=international_system&left_color=black&right_color=blue&left_text=downloads/month
     :target: https://pepy.tech/project/jira-assistant
     :alt: download
 
+.. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
+   :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
+   :alt: GitHub issues
+
 .. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
     :alt: python 3.11 (Linux)
 
 .. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml
     :alt: python 3.11 (Mac OS)
@@ -39,14 +43,22 @@
     :target: https://codecov.io/gh/SharryXu/jira-assistant
     :alt: Codecov
 
 .. |CodeClimate| image:: https://api.codeclimate.com/v1/badges/aeae36dcbb250784672b/maintainability
    :target: https://codeclimate.com/github/SharryXu/jira-assistant/maintainability
    :alt: Maintainability
 
+.. |License| image:: https://img.shields.io/github/license/sharryxu/jira-assistant
+   :target: https://img.shields.io/github/license/sharryxu/jira-assistant
+   :alt: License
+
+Collecting Ideas!!!
+===================
+If you have any ideas or good requirements related to this package, please let us know and we will do our best to fulfill! Please send emails to <sharry.xu@outlook.com>.
+
 Installation
 ============
 `jira-assistant` can be installed from PyPI using `pip` (note that the package name is different from the importable name)::
 
     pip install -U jira-assistant
 
 Download
@@ -65,15 +77,14 @@
 * Parsing the excel file which usually been downloaded from the Jira platform.
 * Sorting the excel records using some specific logic.
 * Generating the target excel file which contains the result.
 * The excel file structure can be customized by JSON file.
 
 A Simple Example
 ================
-
 You can run below command in the PowerShell (Windows OS) or Shell (UNIX OS) to process the excel files.
 
 .. code-block:: console
 
     process-excel-file source.xlsx
 
 After that, you can find the output file in the same folder along with the source file. 
@@ -102,27 +113,26 @@
 .. code-block:: console
 
     generate-template -h
 
 
 Code Example For Developer
 ==========================
-
 Here's a simple program, just to give you an idea about how to use this package.
 
 .. code-block:: python
 
   import pathlib
   from jira_assistant import run_steps_and_sort_excel_file
   HERE = pathlib.Path().resolve()
   run_steps_and_sort_excel_file(HERE / "source.xlsx", HERE / "target.xlsx")
 
 If you want to customize the definition file to adapt the new Excel, you can do below steps.
 
-1. Creating the definition file like below. Inside the :code:`PreProcessSteps` list, you can determine the procedure which will be triggered before sorting and also inside the :code:`SortStrategyPriority` list, you can decide the sort algorithms' order.
+1. Creating the definition file like below. Inside the :code:`PreProcessSteps` list, you can determine the procedure which will be triggered before sorting and also inside the :code:`SortStrategyPriority` list, you can decide the sort algorithms' order. Note: We need to make sure there is one column named ``StoryId`` and only one.
 
 .. code-block:: json
 
   [
       {
           "PreProcessSteps": [
               {
@@ -230,16 +240,12 @@
       sprint_schedule_file=HERE / "milestone_priority.json"
   )
 
 Author
 ======
 The jira-assistant was written by Sharry Xu <sharry.xu@outlook.com> in 2022.
 
-Starting with version 0.1.13, the main function of this project has been totally finished.
-
-Contact
-=======
-Our mailing list is available at `sharry.xu@outlook.com`.
+Starting with version 0.1.5, the main function of this project has been totally finished.
 
 License
 =======
 All contributions after December 1, 2022 released under MIT license.
```

### Comparing `jira-assistant-0.1.6/pyproject.toml` & `jira-assistant-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jira-assistant"
-version = "0.1.6"
+version = "0.1.7"
 description = "Useful Jira tools"
 readme = "README.rst"
 authors = [{ name = "Sharry Xu", email = "sharry.xu@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `jira-assistant-0.1.6/src/jira_assistant/__init__.py` & `jira-assistant-0.1.7/src/jira_assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/assets/excel_definition.json` & `jira-assistant-0.1.7/src/jira_assistant/assets/excel_definition.json`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/assets/sprint_schedule.json` & `jira-assistant-0.1.7/src/jira_assistant/assets/sprint_schedule.json`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/console_script.py` & `jira-assistant-0.1.7/src/jira_assistant/console_script.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/excel_definition.py` & `jira-assistant-0.1.7/src/jira_assistant/excel_definition.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/excel_operation.py` & `jira-assistant-0.1.7/src/jira_assistant/excel_operation.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/jira_client.py` & `jira-assistant-0.1.7/src/jira_assistant/jira_client.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/milestone.py` & `jira-assistant-0.1.7/src/jira_assistant/milestone.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/priority.py` & `jira-assistant-0.1.7/src/jira_assistant/priority.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/sprint_schedule.py` & `jira-assistant-0.1.7/src/jira_assistant/sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant/story.py` & `jira-assistant-0.1.7/src/jira_assistant/story.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/src/jira_assistant.egg-info/PKG-INFO` & `jira-assistant-0.1.7/src/jira_assistant.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-assistant
-Version: 0.1.6
+Version: 0.1.7
 Summary: Useful Jira tools
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,24 +34,28 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 Jira Assistant - userful jira tools
 =============================================
 
-|pypi| |Download| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate|
+|pypi| |Download| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/jira-assistant.svg?style=flat-square
     :target https://pypi.org/project/jira-assistant/
     :alt: pypi version
 
 .. |Download| image:: https://static.pepy.tech/personalized-badge/jira-assistant?period=month&units=international_system&left_color=black&right_color=blue&left_text=downloads/month
     :target: https://pepy.tech/project/jira-assistant
     :alt: download
 
+.. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
+   :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
+   :alt: GitHub issues
+
 .. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
     :alt: python 3.11 (Linux)
 
 .. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml
     :alt: python 3.11 (Mac OS)
@@ -76,14 +80,22 @@
     :target: https://codecov.io/gh/SharryXu/jira-assistant
     :alt: Codecov
 
 .. |CodeClimate| image:: https://api.codeclimate.com/v1/badges/aeae36dcbb250784672b/maintainability
    :target: https://codeclimate.com/github/SharryXu/jira-assistant/maintainability
    :alt: Maintainability
 
+.. |License| image:: https://img.shields.io/github/license/sharryxu/jira-assistant
+   :target: https://img.shields.io/github/license/sharryxu/jira-assistant
+   :alt: License
+
+Collecting Ideas!!!
+===================
+If you have any ideas or good requirements related to this package, please let us know and we will do our best to fulfill! Please send emails to <sharry.xu@outlook.com>.
+
 Installation
 ============
 `jira-assistant` can be installed from PyPI using `pip` (note that the package name is different from the importable name)::
 
     pip install -U jira-assistant
 
 Download
@@ -102,15 +114,14 @@
 * Parsing the excel file which usually been downloaded from the Jira platform.
 * Sorting the excel records using some specific logic.
 * Generating the target excel file which contains the result.
 * The excel file structure can be customized by JSON file.
 
 A Simple Example
 ================
-
 You can run below command in the PowerShell (Windows OS) or Shell (UNIX OS) to process the excel files.
 
 .. code-block:: console
 
     process-excel-file source.xlsx
 
 After that, you can find the output file in the same folder along with the source file. 
@@ -139,27 +150,26 @@
 .. code-block:: console
 
     generate-template -h
 
 
 Code Example For Developer
 ==========================
-
 Here's a simple program, just to give you an idea about how to use this package.
 
 .. code-block:: python
 
   import pathlib
   from jira_assistant import run_steps_and_sort_excel_file
   HERE = pathlib.Path().resolve()
   run_steps_and_sort_excel_file(HERE / "source.xlsx", HERE / "target.xlsx")
 
 If you want to customize the definition file to adapt the new Excel, you can do below steps.
 
-1. Creating the definition file like below. Inside the :code:`PreProcessSteps` list, you can determine the procedure which will be triggered before sorting and also inside the :code:`SortStrategyPriority` list, you can decide the sort algorithms' order.
+1. Creating the definition file like below. Inside the :code:`PreProcessSteps` list, you can determine the procedure which will be triggered before sorting and also inside the :code:`SortStrategyPriority` list, you can decide the sort algorithms' order. Note: We need to make sure there is one column named ``StoryId`` and only one.
 
 .. code-block:: json
 
   [
       {
           "PreProcessSteps": [
               {
@@ -267,16 +277,12 @@
       sprint_schedule_file=HERE / "milestone_priority.json"
   )
 
 Author
 ======
 The jira-assistant was written by Sharry Xu <sharry.xu@outlook.com> in 2022.
 
-Starting with version 0.1.13, the main function of this project has been totally finished.
-
-Contact
-=======
-Our mailing list is available at `sharry.xu@outlook.com`.
+Starting with version 0.1.5, the main function of this project has been totally finished.
 
 License
 =======
 All contributions after December 1, 2022 released under MIT license.
```

### Comparing `jira-assistant-0.1.6/src/jira_assistant.egg-info/SOURCES.txt` & `jira-assistant-0.1.7/src/jira_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_console_script.py` & `jira-assistant-0.1.7/tests/test_console_script.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_excel_definition.py` & `jira-assistant-0.1.7/tests/test_excel_definition.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_excel_operation.py` & `jira-assistant-0.1.7/tests/test_excel_operation.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_jira_client.py` & `jira-assistant-0.1.7/tests/test_jira_client.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_milestone.py` & `jira-assistant-0.1.7/tests/test_milestone.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_priority.py` & `jira-assistant-0.1.7/tests/test_priority.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_sprint_schedule.py` & `jira-assistant-0.1.7/tests/test_sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.6/tests/test_story.py` & `jira-assistant-0.1.7/tests/test_story.py`

 * *Files identical despite different names*

