# Comparing `tmp/trcli-1.4.4.tar.gz` & `tmp/trcli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trcli-1.4.4.tar", last modified: Thu Apr  6 17:15:42 2023, max compression
+gzip compressed data, was "trcli-1.5.0.tar", last modified: Tue Apr 11 19:33:44 2023, max compression
```

## Comparing `trcli-1.4.4.tar` & `trcli-1.5.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.229703 trcli-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-06 17:15:32.000000 trcli-1.4.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-06 17:15:42.229703 trcli-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-04-06 17:15:32.000000 trcli-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 17:15:42.229703 trcli-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-06 17:15:32.000000 trcli-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.225703 trcli-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_api_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    31484 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_api_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_dataclass_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_junit_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_load_data_from_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_response_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    31398 2023-04-06 17:15:32.000000 trcli-1.4.4/tests/test_results_uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.225703 trcli-1.4.4/trcli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.229703 trcli-1.4.4/trcli/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27476 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/api/api_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/api/api_response_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/api/results_uploader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10831 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.229703 trcli-1.4.4/trcli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/commands/cmd_parse_junit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.229703 trcli-1.4.4/trcli/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/data_classes/data_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/data_classes/dataclass_testrail.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/data_classes/validation_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.229703 trcli-1.4.4/trcli/data_providers/
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/data_providers/api_data_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.229703 trcli-1.4.4/trcli/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/readers/file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/readers/junit_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-06 17:15:32.000000 trcli-1.4.4/trcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:15:42.225703 trcli-1.4.4/trcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-06 17:15:42.000000 trcli-1.4.4/trcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-06 17:15:42.000000 trcli-1.4.4/trcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 17:15:42.000000 trcli-1.4.4/trcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 17:15:42.000000 trcli-1.4.4/trcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-06 17:15:42.000000 trcli-1.4.4/trcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 17:15:42.000000 trcli-1.4.4/trcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.824831 trcli-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-11 19:33:33.000000 trcli-1.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-11 19:33:44.824831 trcli-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-11 19:33:33.000000 trcli-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:33:44.824831 trcli-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-11 19:33:33.000000 trcli-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.812831 trcli-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_api_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31484 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_api_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_dataclass_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_junit_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_load_data_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_response_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31398 2023-04-11 19:33:33.000000 trcli-1.5.0/tests/test_results_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.816831 trcli-1.5.0/trcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.816831 trcli-1.5.0/trcli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27509 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/api/api_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/api/api_response_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/api/results_uploader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11093 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.820831 trcli-1.5.0/trcli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/commands/cmd_parse_junit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/commands/cmd_parse_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.820831 trcli-1.5.0/trcli/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/data_classes/data_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/data_classes/dataclass_testrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/data_classes/validation_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.820831 trcli-1.5.0/trcli/data_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/data_providers/api_data_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.824831 trcli-1.5.0/trcli/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/readers/file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/readers/junit_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/readers/openapi_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 19:33:33.000000 trcli-1.5.0/trcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:44.816831 trcli-1.5.0/trcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-11 19:33:44.000000 trcli-1.5.0/trcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 19:33:44.000000 trcli-1.5.0/trcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:33:44.000000 trcli-1.5.0/trcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 19:33:44.000000 trcli-1.5.0/trcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 19:33:44.000000 trcli-1.5.0/trcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 19:33:44.000000 trcli-1.5.0/trcli.egg-info/top_level.txt
```

### Comparing `trcli-1.4.4/LICENSE.md` & `trcli-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/README.md` & `trcli-1.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 ![Tests](https://github.com/gurock/trcli/actions/workflows/python-app.yml/badge.svg)
 
 trcli - The TestRail CLI
 ================================
-The TestRail CLI (trcli) is a command line tool for interacting with TestRail and uploading test automation results.
+The TestRail CLI (trcli) is a command line tool for interacting with TestRail. 
+It integrates directly with the TestRail API and provides abstractions to easily 
+create test cases and upload automated test results.
+
+The TestRail CLI currently supports:
+- **Uploading automated test results from JUnit reports**
+- **Auto-generating test cases from OpenAPI specifications**
 
-- Install the CLI tool on your system and run it as part of your build pipeline
-- Automatically generate new test runs and upload results from automated tests
-- Optionally create new test cases in TestRail for test cases scripted in your test automation suite
-
-To see more documentation about the TestRail CLI, please refer to the 
+To see further documentation about the TestRail CLI, please refer to the 
 [TestRail CLI documentation pages](https://support.gurock.com/hc/en-us/articles/7146548750868-TestRail-CLI)
 on the TestRail help center.
 
 Installation
 ------------
 
 If you already have [Python](https://www.python.org/) and [pip](https://pip.pypa.io) installed,
@@ -20,24 +22,26 @@
 ```
 $ pip install trcli
 ```
 
 To verify the installation was successful, you can run the `trcli` command.
 ```
 $ trcli
-TestRail CLI v1.4.0 
+TestRail CLI v1.5.0                                 
 Copyright 2021 Gurock Software GmbH - www.gurock.com
-Supported and loaded modules: 
-- junit: JUnit XML Files (& Similar) 
+Supported and loaded modules:                 
+    - parse_junit: JUnit XML Files (& Similar)
 ```
 
 CLI general reference
 --------
-```
+```shell
 $ trcli --help
+TestRail CLI v1.5.0
+Copyright 2021 Gurock Software GmbH - www.gurock.com
 Usage: trcli [OPTIONS] COMMAND [ARGS]...
 
   TestRail CLI
 
 Options:
   -c, --config       Optional path definition for testrail-credentials file or
                      CF file.
@@ -55,20 +59,29 @@
   -t, --timeout      Batch timeout duration.  [default: (30); x>=0]
   -y, --yes          answer 'yes' to all prompts around auto-creation
   -n, --no           answer 'no' to all prompts around auto-creation
   -s, --silent       Silence stdout
   --help             Show this message and exit.
 
 Commands:
-  parse_junit  Parse report files and upload results to TestRail
+  parse_junit    Parse JUnit report and upload results to TestRail
+  parse_openapi  Parse OpenAPI spec and create cases in TestRail
 ```
 
-Parse JUnit Reference (Upload Results)
+Uploading automated test results
 --------
-```
+
+The `parse_junit` command allows you to upload automated test results, provided that you are using
+a framework that supports generating JUnit XML report files.
+
+In the next sections you will find information on how to use the TestRail CLI for **code-first** and
+**specification-first** approaches to test automation.
+
+### Reference
+```shell
 $ trcli parse_junit --help
 Usage: trcli parse_junit [OPTIONS]
 
   Parse report files and upload results to TestRail
 
 Options:
   -f, --file          Filename and path.
@@ -90,16 +103,15 @@
                       --result-fields custom_field_b:3
   --special-parser    Optional special parser option for specialized JUnit
                       reports.
   --allow-ms          Allows using milliseconds for elapsed times.
   --help              Show this message and exit.
 ```
 
-JUnit XML report example
---------
+### JUnit XML report example
 ```xml
 <testsuites name="test suites root">
   <testsuite failures="0" errors="0" skipped="1" tests="1" time="3049" name="tests.LoginTests">
     <properties>
       <property name="setting1" value="True"/>
       <property name="setting2" value="value2"/>
     </properties>
@@ -125,17 +137,15 @@
 | `<testsuites>`     | suite           |
 | `<testsuite>`      | section         |
 | `<testcase>`       | case            |
 
 For further detail, please refer to the 
 [JUnit to TestRail mapping](https://support.gurock.com/hc/en-us/articles/12989737200276) documentation.
 
-Uploading test results
---------
-
+### Uploading test results
 To submit test case results, the TestRail CLI will attempt to match the test cases in your automation suite to test cases in TestRail.
 There are 2 mechanisms to match test cases:
 1. Using Automation ID
 2. Using Case ID (in test case `name` or `property`)
 
 The first mechanism allows to automatically match test cases, meaning you can take a code-first approach,
 while the second one is suited for a specification-first approach, where you write your test cases in TestRail and add the case ID to your automated tests.
@@ -144,15 +154,15 @@
 > 1. The TestRail CLI has a prompt mechanism that allows you to choose whether you want test cases to be automatically created: 
 >   - If you enter `yes` (or use the `-y` option), the TestRail CLI will automatically create any test case it can't match in TestRail
 >   - If you enter `no` (or use the `-n` option), the TestRail CLI will not create any new test cases
 > 2. If you are using a **multi-suite project** in TestRail, you should provide the ID of the test suite 
 >   you want the cases to be created in using the `--suite-id` command line option, 
 >   otherwise the CLI tool will attempt to find the suite on TestRail or create it.
 
-### 1. Using Automation ID
+#### 1. Using Automation ID (code-first approach)
 To use this mechanism, you must first add a new [custom field](https://www.gurock.com/testrail/docs/user-guide/howto/fields/) 
 of type `String` with system name `automation_id`.
 
 The TestRail CLI will use the unique combination of your automation test case’s `classname` and `name` 
 (expressed as `classname.name`) to compare against values of the `automation_id` field in your TestRail test case repository.
 If a match is found, this test case will be included in the auto-generated test run for this upload. 
 
@@ -167,15 +177,15 @@
 > 1. If you would like to upload automation results for test cases that already exist in TestRail, be sure to update the `automation_id` for those test cases before uploading your automation results
 > 2. If you change the test name in your automation suite later, that will create a new test case in TestRail, unless you also update the `automation_id` field for the test case in TestRail
 > 3. If you are using the CLI tool in a CI context, we recommend using the `-y` option to automatically accept test case creation prompts
 
 For more detail, please refer to the [Automation workflows - Code-first](https://support.gurock.com/hc/en-us/articles/12609674354068)
 documentation.
 
-### 2. Using Case ID
+#### 2. Using Case ID (specification-first approach)
 
 You can use the Case ID mechanism if you want to manually match your automated test cases to case IDs in TestRail.
 From an implementation perspective, you can do this in one of two ways:
 
 1. Map by setting the case ID in the test name, using the case-matcher `name`:
 ```xml
 <testsuites name="test suites root">
@@ -199,29 +209,128 @@
 ```
 > **Important usage notes:**
 > - We recommend using the `-n` option to skip creating new test cases due to the potential risk of duplication 
 
 For more details, please refer to the [Automation workflows - Specification-first](https://support.gurock.com/hc/en-us/articles/12609869124116)
 documentation.
 
-Exploring other features
-------------------------
+### Exploring other features
 
-### General features
+#### General features
 Please refer to the [Usage examples](https://support.gurock.com/hc/en-us/articles/12908548726804) documentation page to see how you
 can leverage all the functionalities provided by the TestRail CLI.
 
-### SauceLabs saucectl reports
+#### SauceLabs saucectl reports
 If you are using `saucectl` from SauceLabs to execute your automation projects, the TestRail CLI has an enhanced parser 
 that fetches session information and adds it to your test runs. You can enable this functionality by using 
 the `--special-parser saucectl` command line option.
 
 Please refer to the [SauceLabs and saucectl reports](https://support.gurock.com/hc/en-us/articles/12719558686484)
 documentation for further information.
 
+Generating test cases from OpenAPI specs
+-----------------
+
+The `parse_openapi` command allows you to automatically generate and upload test cases to TestRail based on an
+OpenAPI specification. This feature is intended to be used once to quickly bootstrap your test case design,
+providing you with a solid base of test cases, which you can further expand on TestRail.
+
+### Reference
+```shell
+$ trcli parse_openapi --help
+TestRail CLI v1.5.0
+Copyright 2021 Gurock Software GmbH - www.gurock.com
+Usage: trcli parse_openapi [OPTIONS]
+
+  Parse OpenAPI spec and create cases in TestRail
+
+Options:
+  -f, --file      Filename and path.
+  --suite-id      Suite ID to create the tests in (if project is multi-suite).
+                  [x>=1]
+  --case-fields   List of case fields and values for new test cases creation.
+                  Usage: --case-fields type_id:1 --case-fields priority_id:3
+  --help          Show this message and exit.
+```
+
+### OpenAPI specification example
+```yaml
+openapi: 3.0.0
+info:
+  description: This is a sample API.
+  version: 1.0.0
+  title: My API
+paths:
+  /pet:
+    post:
+      summary: Add a new pet to the store
+      description: Add new pet to the store inventory.
+      operationId: addPet
+      responses:
+        '200':
+          description: Pet created
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/Pet'
+        '400':
+          description: Invalid request
+      requestBody:
+        $ref: '#/components/schemas/Pet'
+  '/pet/{petId}':
+    get:
+      summary: Find pet by ID
+      description: Returns a single pet
+      operationId: getPetById
+      parameters:
+        - name: petId
+          in: path
+          description: ID of pet to return
+          required: true
+          schema:
+            type: integer
+            format: int64
+      responses:
+        '200':
+          description: Successful operation
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/Pet'
+        '400':
+          description: Invalid request
+        '404':
+          description: Pet not found
+components:
+  schemas:
+    Pet:
+      type: object
+      required:
+        - name
+      properties:
+        id:
+          type: integer
+          format: int64
+          readOnly: true
+        name:
+          description: The name given to a pet
+          type: string
+          example: Guru
+```
+
+### Generating test cases
+
+The test cases are generated based on the OpenAPI specification paths, operation verbs and possible response
+status codes, which provides a good basic test coverage for an API, although we recommend you further
+expand your test cases to cover specific business logic and workflows.
+
+| Pattern                               | Test case title example                           |
+|---------------------------------------|---------------------------------------------------|
+| `VERB /path -> status_code (summary)` | `GET /pet/{petId} -> 200 (Successful operation) ` |
+
 Parameter sources
 -----------------
 You can choose to set parameters from different sources, like a default config file,
 environment variables, custom config file, cli parameters or in some cases use
 default values.
 The priority of setting parameters from different sources is as per the table below, where 1 is the highest priority.
```

### Comparing `trcli-1.4.4/tests/test_api_client.py` & `trcli-1.5.0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/tests/test_api_data_provider.py` & `trcli-1.5.0/tests/test_api_data_provider.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/tests/test_api_request_handler.py` & `trcli-1.5.0/tests/test_api_request_handler.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/tests/test_cli.py` & `trcli-1.5.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,14 @@
             result.exit_code == 2
         ), f"Exit code 2 expected. Got: {result.exit_code} instead."
         assert (
             "Missing command." in result.output
         ), "'Missing command.' is not present in output when calling trcli without command parameter."
 
     @pytest.mark.cli
-    # @pytest.mark.parametrize()
-    def test_run_with_case_id_project_title_not_required(self, mocker, cli_resources):
-        cli_args_helper, cli_runner = cli_resources
-
-        args = cli_args_helper.get_all_required_parameters_without_specified(
-            ["project", "title"]
-        )
-        args = ["--run-id 20", "--case-id", "10", *args]
-        mocker.patch("sys.argv", ["trcli", *args])
-        result = cli_runner.invoke(cli, args)
-        assert FAULT_MAPPING["missing_project"] not in result.output, ""
-        assert FAULT_MAPPING["missing_title"] not in result.output, ""
-
-    @pytest.mark.cli
     @pytest.mark.parametrize(
         "missing_args, expected_output, expected_exit_code",
         CHECK_ERROR_MESSAGE_FOR_REQUIRED_PARAMETERS_TEST_DATA,
         ids=CHECK_ERROR_MESSAGE_FOR_REQUIRED_PARAMETERS_TEST_IDS,
     )
     def test_check_error_message_for_required_parameters(
         self, missing_args, expected_output, expected_exit_code, mocker, cli_resources
```

### Comparing `trcli-1.4.4/tests/test_dataclass_creation.py` & `trcli-1.5.0/tests/test_dataclass_creation.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/tests/test_junit_parser.py` & `trcli-1.5.0/tests/test_junit_parser.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/tests/test_load_data_from_config.py` & `trcli-1.5.0/tests/test_load_data_from_config.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/tests/test_response_verify.py` & `trcli-1.5.0/tests/test_response_verify.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/tests/test_results_uploader.py` & `trcli-1.5.0/tests/test_results_uploader.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/trcli/api/api_client.py` & `trcli-1.5.0/trcli/api/api_client.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/trcli/api/api_request_handler.py` & `trcli-1.5.0/trcli/api/api_request_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 import html
-import json
-from pprint import pprint
+from concurrent.futures import ThreadPoolExecutor, as_completed
+from typing import List, Union, Tuple
 
 from trcli.api.api_client import APIClient, APIClientResult
-from trcli.cli import Environment
 from trcli.api.api_response_verify import ApiResponseVerify
-from trcli.data_classes.dataclass_testrail import TestRailSuite, TestRailCase
-from trcli.data_classes.data_parsers import MatchersParser
-from trcli.data_providers.api_data_provider import ApiDataProvider
+from trcli.cli import Environment
 from trcli.constants import (
     ProjectErrors,
     FAULT_MAPPING,
 )
+from trcli.data_classes.data_parsers import MatchersParser
+from trcli.data_classes.dataclass_testrail import TestRailSuite, TestRailCase, ProjectData
+from trcli.data_providers.api_data_provider import ApiDataProvider
 from trcli.settings import MAX_WORKERS_ADD_RESULTS, MAX_WORKERS_ADD_CASE
-from typing import List, Union
-from dataclasses import dataclass
-from concurrent.futures import ThreadPoolExecutor, as_completed
-
-
-@dataclass
-class ProjectData:
-    project_id: int
-    suite_mode: int
-    error_message: str
 
 
 class ApiRequestHandler:
     """Sends requests based on DataProvider bodies"""
 
     def __init__(
         self,
@@ -135,15 +125,15 @@
                 (True, "")
                 if suite_id in available_suites
                 else (False, FAULT_MAPPING["missing_suite"].format(suite_id=suite_id))
             )
         else:
             return None, response.error_message
 
-    def resolve_suite_id_using_name(self, project_id: int) -> (int, str):
+    def resolve_suite_id_using_name(self, project_id: int) -> Tuple[int, str]:
         """Get suite ID matching suite name on data provider or returns -1 if unable to match any suite.
         :arg project_id: project id
         :returns: tuple with id of the suite and error message"""
         suite_id = -1
         error_message = ""
         response = self.client.send_get(f"get_suites/{project_id}")
         if not response.error_message:
@@ -156,40 +146,40 @@
                 suite_id = suite["id"]
                 self.data_provider.update_data([{"suite_id": suite["id"], "name": suite["name"]}])
         else:
             error_message = response.error_message
 
         return suite_id, error_message
 
-    def get_suite_ids(self, project_id: int) -> (List[int], str):
+    def get_suite_ids(self, project_id: int) -> Tuple[List[int], str]:
         """Get suite IDs for requested project_id.
         : project_id: project id
         : returns: tuple with list of suite ids and error string"""
         available_suites = []
         returned_resources = []
         error_message = ""
         response = self.client.send_get(f"get_suites/{project_id}")
         if not response.error_message:
             for suite in response.response_text:
-                available_suites.append(suite["id"])
+                available_suites.append(int(suite["id"]))
                 returned_resources.append(
                     {
                         "suite_id": suite["id"],
                         "name": suite["name"],
                     }
                 )
         else:
             error_message = response.error_message
 
         self.data_provider.update_data(suite_data=returned_resources) if len(
             returned_resources
         ) > 0 else "Update skipped"
         return available_suites, error_message
 
-    def add_suites(self, project_id: int) -> (List[dict], str):
+    def add_suites(self, project_id: int) -> Tuple[List[dict], str]:
         """
         Adds suites that doesn't have ID's in DataProvider.
         Runs update_data in data_provider for successfully created resources.
         :project_id: project_id
         :returns: Tuple with list of dict created resources and error string.
         """
         add_suite_data = self.data_provider.add_suites_data()
@@ -217,15 +207,15 @@
             for response in responses
         ]
         self.data_provider.update_data(suite_data=returned_resources) if len(
             returned_resources
         ) > 0 else "Update skipped"
         return returned_resources, error_message
 
-    def check_missing_section_ids(self, project_id: int) -> (List[int], str):
+    def check_missing_section_ids(self, project_id: int) -> Tuple[bool, str]:
         """
         Check what section id's are missing in DataProvider.
         :project_id: project_id
         :returns: Tuple with list missing section ID and error string.
         """
         suite_id = self.suites_data_from_provider.suite_id
         returned_sections, error_message = self.__get_all_sections(project_id, suite_id)
@@ -244,15 +234,15 @@
                 else:
                     missing_test_sections = True
             self.data_provider.update_data(section_data=section_data)
             return missing_test_sections, error_message
         else:
             return False, error_message
 
-    def add_sections(self, project_id: int) -> (List[dict], str):
+    def add_sections(self, project_id: int) -> Tuple[List[dict], str]:
         """
         Add sections that doesn't have ID in DataProvider.
         Runs update_data in data_provider for successfully created resources.
         :project_id: project_id
         :returns: Tuple with list of dict created resources and error string.
         """
         add_sections_data = self.data_provider.add_sections_data()
@@ -280,15 +270,15 @@
             for response in responses
         ]
         self.data_provider.update_data(section_data=returned_resources) if len(
             returned_resources
         ) > 0 else "Update skipped"
         return returned_resources, error_message
 
-    def check_missing_test_cases_ids(self, project_id: int) -> (bool, str):
+    def check_missing_test_cases_ids(self, project_id: int) -> Tuple[bool, str]:
         """
         Check what test cases id's are missing in DataProvider.
         :project_id: project_id
         :returns: Tuple with list test case ID missing and error string.
         """
         missing_cases_number = 0
         suite_id = self.suites_data_from_provider.suite_id
@@ -330,15 +320,15 @@
                 self.environment.log(f"Found {missing_cases_number} test cases without case ID in the report file.")
             if nonexistent_ids:
                 self.environment.elog(f"Nonexistent case IDs found in the report file: {nonexistent_ids}")
                 return False, "Case IDs not in TestRail project or suite were detected in the report file."
 
         return missing_cases_number > 0, ""
 
-    def add_cases(self) -> (List[dict], str):
+    def add_cases(self) -> Tuple[List[dict], str]:
         """
         Add cases that doesn't have ID in DataProvider.
         Runs update_data in data_provider for successfully created resources.
         :returns: Tuple with list of dict created resources and error string.
         """
         add_case_data = self.data_provider.add_cases()
         responses = []
@@ -367,15 +357,15 @@
                 "section_id": response.response_text["section_id"],
                 "title": response.response_text["title"]
             }
             for response in responses
         ]
         return returned_resources, error_message
 
-    def add_run(self, project_id: int, run_name: str, milestone_id: int = None) -> (List[dict], str):
+    def add_run(self, project_id: int, run_name: str, milestone_id: int = None) -> Tuple[int, str]:
         """
         Creates a new test run.
         :project_id: project_id
         :run_name: run name
         :returns: Tuple with run id and error string.
         """
         add_run_data = self.data_provider.add_run(run_name, milestone_id=milestone_id)
@@ -395,15 +385,15 @@
                         with open(file_path, "rb") as file:
                             self.client.send_post(f"add_attachment_to_result/{result_id}", files={"attachment": file})
                     except Exception as ex:
                         self.environment.elog(f"Error uploading attachment for case {case_id}: {ex}")
         else:
             self.environment.elog(f"Unable to upload attachments due to API request error: {error}")
 
-    def add_results(self, run_id: int) -> (dict, str):
+    def add_results(self, run_id: int) -> Tuple[list, str, int]:
         """
         Adds one or more new test results.
         :run_id: run id
         :returns: Tuple with dict created resources and error string.
         """
         responses = []
         error_message = ""
@@ -451,15 +441,15 @@
             self.environment.log(f"Uploading {attachments_count} attachments "
                                  f"for {len(report_results_w_attachments)} test results.")
             self.upload_attachments(report_results_w_attachments, results, run_id)
         else:
             self.environment.log(f"No attachments found to upload.")
         return responses, error_message, progress_bar.n
 
-    def handle_futures(self, futures, action_string, progress_bar):
+    def handle_futures(self, futures, action_string, progress_bar) -> Tuple[list, str]:
         responses = []
         error_message = ""
         try:
             for future in as_completed(futures):
                 arguments = futures[future]
                 response = future.result()
                 if not response.error_message:
@@ -488,34 +478,34 @@
             else:
                 progress_bar.set_postfix_str(s="Done.")
         except KeyboardInterrupt:
             self.__cancel_running_futures(futures, action_string)
             raise KeyboardInterrupt
         return responses, error_message
 
-    def close_run(self, run_id: int) -> (dict, str):
+    def close_run(self, run_id: int) -> Tuple[dict, str]:
         """
         Closes an existing test run and archives its tests & results.
         :run_id: run id
         :returns: Tuple with dict created resources and error string.
         """
         body = {"run_id": run_id}
         response = self.client.send_post(f"close_run/{run_id}", body)
         return response.response_text, response.error_message
 
-    def delete_suite(self, suite_id: int) -> (dict, str):
+    def delete_suite(self, suite_id: int) -> Tuple[dict, str]:
         """
         Delete suite given suite id
         :suite_id: suite id
         :returns: Tuple with dict created resources and error string.
         """
         response = self.client.send_post(f"delete_suite/{suite_id}", payload={})
         return response.response_text, response.error_message
 
-    def delete_sections(self, added_sections: List[dict]) -> (dict, str):
+    def delete_sections(self, added_sections: List[dict]) -> Tuple[list, str]:
         """
         Delete section given add_sections response
         :suite_id: section id
         :returns: Tuple with dict created resources and error string.
         """
         responses = []
         error_message = ""
@@ -526,46 +516,46 @@
             if not response.error_message:
                 responses.append(response.response_text)
             else:
                 error_message = response.error_message
                 break
         return responses, error_message
 
-    def delete_cases(self, suite_id: int, added_cases: List[dict]) -> (dict, str):
+    def delete_cases(self, suite_id: int, added_cases: List[dict]) -> Tuple[dict, str]:
         """
         Delete cases given add_cases response
         :suite_id: section id
         :returns: Tuple with dict created resources and error string.
         """
         body = {"case_ids": [case["case_id"] for case in added_cases]}
         response = self.client.send_post(f"delete_cases/{suite_id}", payload=body)
         return response.response_text, response.error_message
 
-    def delete_run(self, run_id) -> (dict, str):
+    def delete_run(self, run_id) -> Tuple[dict, str]:
         """
         Delete run given add_run response
         :suite_id: section id
         :returns: Tuple with dict created resources and error string.
         """
         response = self.client.send_post(f"delete_run/{run_id}", payload={})
         return response.response_text, response.error_message
 
     @staticmethod
-    def retrieve_results_after_cancelling(futures):
+    def retrieve_results_after_cancelling(futures) -> list:
         responses = []
         for future in as_completed(futures):
             if not future.cancelled():
                 response = future.result()
                 if not response.error_message:
                     responses.append(response)
         return responses
 
-    def _add_case_and_update_data(self, case: TestRailCase):
+    def _add_case_and_update_data(self, case: TestRailCase) -> APIClientResult:
         case_body = case.to_dict()
-        if self.environment.case_matcher != MatchersParser.AUTO:
+        if self.environment.case_matcher != MatchersParser.AUTO and "custom_automation_id" in case_body:
             case_body.pop("custom_automation_id")
         response = self.client.send_post(f"add_case/{case_body.pop('section_id')}", case_body)
         if response.status_code == 200:
             case.case_id = response.response_text["id"]
             case.result.case_id = response.response_text["id"]
             case.section_id = response.response_text["section_id"]
         return response
@@ -573,39 +563,39 @@
     def __cancel_running_futures(self, futures, action_string):
         self.environment.log(
             f"\nAborting: {action_string}. Trying to cancel scheduled tasks."
         )
         for future in futures:
             future.cancel()
 
-    def __get_all_cases(self, project_id=None, suite_id=None) -> (List[dict], str):
+    def __get_all_cases(self, project_id=None, suite_id=None) -> Tuple[List[dict], str]:
         """
         Get all cases from all pages
         """
         return self.__get_all_entities('cases', f"get_cases/{project_id}&suite_id={suite_id}")
 
-    def __get_all_sections(self, project_id=None, suite_id=None) -> (List[dict], str):
+    def __get_all_sections(self, project_id=None, suite_id=None) -> Tuple[List[dict], str]:
         """
         Get all sections from all pages
         """
         return self.__get_all_entities('sections', f"get_sections/{project_id}&suite_id={suite_id}")
 
-    def __get_all_tests_in_run(self, run_id=None) -> (List[dict], str):
+    def __get_all_tests_in_run(self, run_id=None) -> Tuple[List[dict], str]:
         """
         Get all tests from all pages
         """
         return self.__get_all_entities('tests', f"get_tests/{run_id}")
 
-    def __get_all_projects(self) -> (List[dict], str):
+    def __get_all_projects(self) -> Tuple[List[dict], str]:
         """
         Get all cases from all pages
         """
         return self.__get_all_entities('projects', f"get_projects")
 
-    def __get_all_entities(self, entity: str, link=None, entities=[]) -> (List[dict], str):
+    def __get_all_entities(self, entity: str, link=None, entities=[]) -> Tuple[List[dict], str]:
         """
         Get all entities from all pages if number of entities is too big to return in single response.
         Function using next page field in API response.
         Entity examples: cases, sections
         """
         if link.startswith(self.suffix):
             link = link.replace(self.suffix, "")
```

### Comparing `trcli-1.4.4/trcli/api/api_response_verify.py` & `trcli-1.5.0/trcli/api/api_response_verify.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/trcli/api/results_uploader.py` & `trcli-1.5.0/trcli/api/results_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,33 +12,29 @@
 
 class ResultsUploader:
     """
     Class to be used to upload the results to TestRail.
     Initialized with environment object and result file parser object (any parser derived from FileParser).
     """
 
-    def __init__(self, environment: Environment, suite: TestRailSuite):
+    def __init__(self, environment: Environment, suite: TestRailSuite, skip_run: bool = False):
         self.project = None
         self.environment = environment
-        self.parsed_data = suite
+        self.skip_run = skip_run
         self.run_name = self.environment.title
         if self.environment.special_parser == "saucectl":
-            self.run_name += f" ({self.parsed_data.name})"
+            self.run_name += f" ({suite.name})"
         if self.environment.suite_id:
-            self.parsed_data.suite_id = self.environment.suite_id
+            suite.suite_id = self.environment.suite_id
         self.api_request_handler = ApiRequestHandler(
             api_client=self.instantiate_api_client(),
             environment=self.environment,
-            suites_data=self.parsed_data,
+            suites_data=suite,
             verify=self.environment.verify,
         )
-        if self.environment.suite_id:
-            self.api_request_handler.data_provider.update_data(
-                [{"suite_id": self.environment.suite_id}]
-            )
 
     def upload_results(self):
         """
         Does all the job needed to upload the results parsed from result files to TestRail.
         If needed missing items like suite/section/test case would be added to TestRail.
         Exits with result code 1 printing proper message to the user in case of a failure
         or with result code 0 if succeeds.
@@ -99,14 +95,20 @@
                     added_suite_id=added_suite_id,
                     added_sections=added_sections,
                     added_test_cases=added_test_cases,
                 )
                 self.environment.log("\n".join(revert_logs))
                 exit(1)
 
+        if self.skip_run:
+            stop = time.time()
+            if added_test_cases:
+                self.environment.log(f"Submitted {len(added_test_cases)} test cases in {stop - start:.1f} secs.")
+            return
+
         # Create/update test run
         if not self.environment.run_id:
             self.environment.log(f"Creating test run. ", new_line=False)
             added_run, error_message = self.api_request_handler.add_run(
                 self.project.project_id, self.run_name, self.environment.milestone_id
             )
             if error_message:
```

### Comparing `trcli-1.4.4/trcli/cli.py` & `trcli-1.5.0/trcli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 import sys
 from typing import List, Union
 
 import click
 import yaml
 from pathlib import Path
@@ -11,27 +10,28 @@
 from click.core import ParameterSource
 from tqdm import tqdm
 
 from trcli.constants import (
     FAULT_MAPPING,
     MISSING_COMMAND_SLOGAN,
     TOOL_USAGE,
-    TOOL_VERSION,
+    TOOL_VERSION, PARSE_JUNIT_FAULT_MAPPING,
 )
 from trcli.data_classes.data_parsers import FieldsParser
 from trcli.settings import DEFAULT_API_CALL_TIMEOUT, DEFAULT_BATCH_SIZE
 
 CONTEXT_SETTINGS = dict(auto_envvar_prefix="TR_CLI")
 
 trcli_folder = Path(__file__).parent
 cmd_folder = trcli_folder / "commands/"
 
 
 class Environment:
-    def __init__(self):
+    def __init__(self, cmd="parse_junit"):
+        self.cmd = cmd
         self.home = os.getcwd()
         self.default_config_file = True
         self.params_from_config = dict()
         self.file = None
         self.host = None
         self.project = None
         self.project_id = None
@@ -137,14 +137,17 @@
     def check_for_required_parameters(self):
         """Checks that all required parameters were set. If not error message would be printed and
         program will exit with exit code 1"""
         for param, value in vars(self).items():
             if "missing_" + param in FAULT_MAPPING and not value:
                 self.elog(FAULT_MAPPING["missing_" + param])
                 exit(1)
+            if self.cmd == "parse_junit" and "missing_" + param in PARSE_JUNIT_FAULT_MAPPING and not value:
+                self.elog(PARSE_JUNIT_FAULT_MAPPING["missing_" + param])
+                exit(1)
         # special case for password and key (both needs to be missing for the error message to show up)
         if not self.password and not self.key:
             self.elog(FAULT_MAPPING["missing_password_and_key"])
             exit(1)
         # validate host syntax
         try:
             request = PreparedRequest()
```

### Comparing `trcli-1.4.4/trcli/commands/cmd_parse_junit.py` & `trcli-1.5.0/trcli/commands/cmd_parse_junit.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     type=click.Choice(["junit", "saucectl"], case_sensitive=False),
     help="Optional special parser option for specialized JUnit reports."
 )
 @click.option("--allow-ms", is_flag=True, help="Allows using milliseconds for elapsed times.")
 @click.pass_context
 @pass_environment
 def cli(environment: Environment, context: click.Context, *args, **kwargs):
-    """Parse report files and upload results to TestRail"""
+    """Parse JUnit report and upload results to TestRail"""
     environment.set_parameters(context)
     environment.check_for_required_parameters()
     settings.ALLOW_ELAPSED_MS = environment.allow_ms
     print_config(environment)
     try:
         parsed_suites = JunitParser(environment).parse_file()
         for suite in parsed_suites:
```

### Comparing `trcli-1.4.4/trcli/constants.py` & `trcli-1.5.0/trcli/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import trcli
 import enum
 
+PARSE_JUNIT_FAULT_MAPPING = dict(
+    missing_title="Please give your Test Run a title using the --title argument."
+)
 
 FAULT_MAPPING = dict(
     missing_file="Please provide a valid path to your results file with the -f argument.",
-    invalid_file="Provided file is not a valid XML file.",
+    invalid_file="Provided file is not a valid file.",
     missing_host="Please provide a TestRail server address with the -h argument.",
     missing_project="Please specify the project name using the --project argument.",
-    missing_title="Please give your Test Run a title using the --title argument.",
     missing_username="Please provide a valid TestRail username using the -u argument.",
     more_than_one_project="Given project name matches more than one result."
     "Please specify which should be used using the --project-id argument",
     project_doesnt_exists="Please specify a valid project name using the --project argument",
     missing_password_and_key="Please provide either a password using the -p "
     "argument or an API key using the -k argument.",
     no_response_from_host="Your upload to TestRail did not receive a successful response from your TestRail Instance. "
@@ -61,15 +63,16 @@
     "in TestRail or the IDs are not specified.\n"
     "Would you like to create missing test cases under project: '{project_name}'?",
 )
 
 TOOL_VERSION = f"""TestRail CLI v{trcli.__version__}
 Copyright 2021 Gurock Software GmbH - www.gurock.com"""
 TOOL_USAGE = f"""Supported and loaded modules:
-    - parse_junit: JUnit XML Files (& Similar)"""
+    - parse_junit: JUnit XML Files (& Similar)
+    - parse_openapi: OpenAPI YML Files"""
 
 MISSING_COMMAND_SLOGAN = """Usage: trcli [OPTIONS] COMMAND [ARGS]...\nTry 'trcli --help' for help.
 \nError: Missing command."""
 
 
 class ProjectErrors(enum.IntEnum):
     multiple_project_same_name = -1
```

### Comparing `trcli-1.4.4/trcli/data_classes/data_parsers.py` & `trcli-1.5.0/trcli/data_classes/data_parsers.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/trcli/data_classes/dataclass_testrail.py` & `trcli-1.5.0/trcli/data_classes/dataclass_testrail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dataclasses import dataclass
+from time import gmtime, strftime
 from typing import List, Optional
+
 from serde import field, serialize, deserialize, to_dict
-from time import gmtime, strftime
 
 from trcli import settings
-
 from trcli.data_classes.validation_exception import ValidationException
 
 
 @serialize
 @deserialize
 @dataclass
 class TestRailResult:
     """Class for creating Test Rail result for cases"""
 
-    case_id: int
+    case_id: int = field(default=None, skip_if_default=True)
     status_id: int = field(default=None, skip_if_default=True)
     comment: str = field(default=None, skip_if_default=True)
     version: str = field(default=None, skip_if_default=True)
     elapsed: str = field(default=None, skip_if_default=True)
     defects: str = field(default=None, skip_if_default=True)
     assignedto_id: int = field(default=None, skip_if_default=True)
     attachments: Optional[List[str]] = field(default_factory=list, skip_if_default=True)
@@ -32,15 +32,14 @@
             )
             self.comment = self.get_comment_from_junit_element(
                 self.junit_result_unparsed
             )
         if self.elapsed is not None:
             self.elapsed = self.proper_format_for_elapsed(self.elapsed)
 
-
     @staticmethod
     def calculate_status_id_from_junit_element(junit_result: list) -> int:
         """
          Calculate id for first result. In junit no result mean pass
         1 - Passed
         3 - Untested
         4 - Retest
@@ -100,14 +99,15 @@
         self.result_fields = new_results_fields
 
     def to_dict(self) -> dict:
         result_dict = to_dict(self)
         result_dict.update(self.result_fields)
         return result_dict
 
+
 @serialize
 @deserialize
 @dataclass
 class TestRailCase:
     """Class for creating Test Rail test case"""
 
     title: str
@@ -151,14 +151,15 @@
         self.case_fields = new_case_fields
 
     def to_dict(self) -> dict:
         case_dict = to_dict(self)
         case_dict.update(self.case_fields)
         return case_dict
 
+
 @serialize
 @deserialize
 @dataclass
 class TestRailProperty:
     """Class for creating Test Rail property - run description"""
 
     name: str = field(default=None, skip_if_default=True)
@@ -215,7 +216,14 @@
         default_factory=list, metadata={"serde_skip": True}
     )
     source: str = field(default=None, metadata={"serde_skip": True})
 
     def __post_init__(self):
         current_time = strftime("%d-%m-%y %H:%M:%S", gmtime())
         self.name = f"{self.source} {current_time}" if self.name is None else self.name
+
+
+@dataclass
+class ProjectData:
+    project_id: int
+    suite_mode: int
+    error_message: str
```

### Comparing `trcli-1.4.4/trcli/data_classes/validation_exception.py` & `trcli-1.5.0/trcli/data_classes/validation_exception.py`

 * *Files identical despite different names*

### Comparing `trcli-1.4.4/trcli/data_providers/api_data_provider.py` & `trcli-1.5.0/trcli/data_providers/api_data_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
 
     def __init__(self, suites_input: TestRailSuite, case_fields: dict = None, run_description: str = None, result_fields: dict = None):
         self.suites_input = suites_input
         self.case_fields = case_fields
         self.run_description = run_description
         self.result_fields = result_fields
+        self.update_data([{"suite_id": self.suites_input.suite_id}])
 
     def add_suites_data(self) -> list:
         """Return list of bodies for adding suites"""
         return [to_dict(self.suites_input)]
 
     def add_sections_data(self, return_all_items=False) -> list:
         """Return list of bodies for adding sections.
```

### Comparing `trcli-1.4.4/trcli/readers/junit_xml.py` & `trcli-1.5.0/trcli/readers/junit_xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from typing import Union
 from unittest import TestCase, TestSuite
 from xml.etree import ElementTree as etree
 
 from junitparser import JUnitXml, JUnitXmlError, Element, Attr
 
+from trcli.cli import Environment
 from trcli.data_classes.data_parsers import MatchersParser, FieldsParser
 from trcli.data_classes.dataclass_testrail import (
     TestRailCase,
     TestRailSuite,
     TestRailSection,
     TestRailProperty,
     TestRailResult,
@@ -27,14 +28,20 @@
 class Property(Element):
     _tag = "property"
     name = Attr()
     value = Attr()
 
 
 class JunitParser(FileParser):
+
+    def __init__(self, environment: Environment):
+        super().__init__(environment)
+        self.case_matcher = environment.case_matcher
+        self.special = environment.special_parser
+
     @classmethod
     def _add_root_element_to_tree(cls, filepath: Union[str, Path]) -> etree:
         """
         Because some of junits have XML root as testsuites and some not.
         This way make sure that we always have testsuites root.
         """
         tree = etree.parse(filepath)
```

### Comparing `trcli-1.4.4/trcli.egg-info/SOURCES.txt` & `trcli-1.5.0/trcli.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 trcli/api/__init__.py
 trcli/api/api_client.py
 trcli/api/api_request_handler.py
 trcli/api/api_response_verify.py
 trcli/api/results_uploader.py
 trcli/commands/__init__.py
 trcli/commands/cmd_parse_junit.py
+trcli/commands/cmd_parse_openapi.py
 trcli/data_classes/__init__.py
 trcli/data_classes/data_parsers.py
 trcli/data_classes/dataclass_testrail.py
 trcli/data_classes/validation_exception.py
 trcli/data_providers/api_data_provider.py
 trcli/readers/__init__.py
 trcli/readers/file_parser.py
-trcli/readers/junit_xml.py
+trcli/readers/junit_xml.py
+trcli/readers/openapi_yml.py
```

