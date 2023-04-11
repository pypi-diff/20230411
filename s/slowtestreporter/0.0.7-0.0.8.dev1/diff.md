# Comparing `tmp/slowtestreporter-0.0.7.tar.gz` & `tmp/slowtestreporter-0.0.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slowtestreporter-0.0.7.tar", last modified: Mon Apr 10 04:17:29 2023, max compression
+gzip compressed data, was "slowtestreporter-0.0.8.dev1.tar", last modified: Tue Apr 11 10:12:46 2023, max compression
```

## Comparing `slowtestreporter-0.0.7.tar` & `slowtestreporter-0.0.8.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:29.901074 slowtestreporter-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:29.897074 slowtestreporter-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:29.901074 slowtestreporter-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-10 04:17:29.901074 slowtestreporter-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 04:17:29.901074 slowtestreporter-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:29.901074 slowtestreporter-0.0.7/slowtestreporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/slowtestreporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/slowtestreporter/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/slowtestreporter/slowtestreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:29.901074 slowtestreporter-0.0.7/slowtestreporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-10 04:17:29.000000 slowtestreporter-0.0.7/slowtestreporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-10 04:17:29.000000 slowtestreporter-0.0.7/slowtestreporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 04:17:29.000000 slowtestreporter-0.0.7/slowtestreporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-10 04:17:29.000000 slowtestreporter-0.0.7/slowtestreporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 04:17:29.000000 slowtestreporter-0.0.7/slowtestreporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 04:17:29.000000 slowtestreporter-0.0.7/slowtestreporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:29.901074 slowtestreporter-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-10 04:17:17.000000 slowtestreporter-0.0.7/tests/test_slow_test_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:46.445571 slowtestreporter-0.0.8.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:46.441571 slowtestreporter-0.0.8.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:46.445571 slowtestreporter-0.0.8.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-11 10:12:46.445571 slowtestreporter-0.0.8.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:12:46.445571 slowtestreporter-0.0.8.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:46.445571 slowtestreporter-0.0.8.dev1/slowtestreporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/slowtestreporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/slowtestreporter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/slowtestreporter/slowtestreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:46.445571 slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-11 10:12:46.000000 slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-11 10:12:46.000000 slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:12:46.000000 slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 10:12:46.000000 slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 10:12:46.000000 slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 10:12:46.000000 slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:46.445571 slowtestreporter-0.0.8.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-11 10:12:38.000000 slowtestreporter-0.0.8.dev1/tests/test_slow_test_reporter.py
```

### Comparing `slowtestreporter-0.0.7/.github/workflows/python-app.yml` & `slowtestreporter-0.0.8.dev1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `slowtestreporter-0.0.7/.gitignore` & `slowtestreporter-0.0.8.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `slowtestreporter-0.0.7/LICENSE` & `slowtestreporter-0.0.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `slowtestreporter-0.0.7/PKG-INFO` & `slowtestreporter-0.0.8.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slowtestreporter
-Version: 0.0.7
+Version: 0.0.8.dev1
 Summary: A small python package for reporting slow tests.
 Project-URL: Homepage, https://github.com/jerrylu8888/slowtestreporter
 Project-URL: Bug Tracker, https://github.com/jerrylu8888/slowtestreporter/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `slowtestreporter-0.0.7/README.md` & `slowtestreporter-0.0.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `slowtestreporter-0.0.7/pyproject.toml` & `slowtestreporter-0.0.8.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slowtestreporter-0.0.7/slowtestreporter/slowtestreporter.py` & `slowtestreporter-0.0.8.dev1/slowtestreporter/slowtestreporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,46 +16,29 @@
         junit_file_path (str) : The file path of the junit file results
         xml_output_file_name (str) : Output file name, if a junit file is to be produced. Do not include the file
                                     extension
         display_results (str) : Displays test results if set to true
     """
     junit_xml = JUnitXml.fromfile(junit_file_path)
 
-    test_results, xml_output, passed = parse_test_results(junit_xml)
+    test_results, xml_output = parse_test_results(junit_xml)
     average_test_duration = calculate_average_test_duration(junit_xml)
 
     if display_results:
         print(tabulate(test_results, headers=["Test", "Time (s)", "Result", "Message"]))
         logging.info('Average test duration: %s s', average_test_duration)
 
     if xml_output_file_name:
         xml_output.write(xml_output_file_name + '.xml')
         logging.info('junit file created: %s.xml', xml_output_file_name)
-    return passed
-
-
-def report_average_test_result(average_threshold: float, junit_xml: JUnitXml, display_result: bool) -> (bool, float):
-    average_time = calculate_average_test_duration(junit_xml)
-    if average_threshold < average_time:
-        result = False
-    else:
-        result = True
-    if display_result:
-        if result:
-            logging.info('Tests passed average test duration threshold. Threshold for pass: %s, actual: %s',
-                         str(average_threshold), str(average_time))
-        else:
-            logging.info('Tests failed average test duration threshold. Threshold for pass: %s, actual: %s',
-                         str(average_threshold), str(average_time))
-    return result, average_time
 
 
 def parse_test_results(junit_xml: JUnitXml):
     test_results = []
-    passed = True
+
     """
     IF TEST FAILED => FAILED
     IF TEST TOO SLOW => FAILED
     IF TEST TOO SLOW + FAILED => FAILED
     OTHERWISE => PASS
     """
 
@@ -64,24 +47,22 @@
             if testcase.time > THRESHOLD:
                 result = FAIL_TEXT
                 if testcase.result and testcase.result[0]:
                     testcase.result[0].message += ' ' + SLOW_ERROR_MSG
                 else:
                     testcase.result = [Failure(SLOW_ERROR_MSG)]
                 test_results.append([testcase.name, testcase.time, result, testcase.result[0].message])
-                passed = False
             elif testcase.result and testcase.result[0]:
                 result = FAIL_TEXT
                 test_results.append([testcase.name, testcase.time, result, testcase.result[0].message])
-                passed = False
             else:
                 result = 'PASS'
                 test_results.append([testcase.name, testcase.time, result])
 
-    return test_results, junit_xml, passed
+    return test_results, junit_xml
 
 
 def calculate_average_test_duration(junit_xml: JUnitXml) -> float:
     test_count: float = 0
     total_duration: float = 0
     for suite in junit_xml:
         for testcase in suite:
```

### Comparing `slowtestreporter-0.0.7/slowtestreporter.egg-info/PKG-INFO` & `slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slowtestreporter
-Version: 0.0.7
+Version: 0.0.8.dev1
 Summary: A small python package for reporting slow tests.
 Project-URL: Homepage, https://github.com/jerrylu8888/slowtestreporter
 Project-URL: Bug Tracker, https://github.com/jerrylu8888/slowtestreporter/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `slowtestreporter-0.0.7/slowtestreporter.egg-info/SOURCES.txt` & `slowtestreporter-0.0.8.dev1/slowtestreporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slowtestreporter-0.0.7/tests/test_cli.py` & `slowtestreporter-0.0.8.dev1/tests/test_cli.py`

 * *Files identical despite different names*

