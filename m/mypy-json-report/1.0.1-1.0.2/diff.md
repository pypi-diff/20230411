# Comparing `tmp/mypy_json_report-1.0.1.tar.gz` & `tmp/mypy_json_report-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_json_report-1.0.1.tar", max compression
+gzip compressed data, was "mypy_json_report-1.0.2.tar", max compression
```

## Comparing `mypy_json_report-1.0.1.tar` & `mypy_json_report-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10702 2023-02-28 14:39:12.945649 mypy_json_report-1.0.1/LICENSE
--rw-r--r--   0        0        0     2331 2023-02-28 14:39:12.945649 mypy_json_report-1.0.1/README.md
--rw-r--r--   0        0        0     9618 2023-02-28 14:39:12.945649 mypy_json_report-1.0.1/mypy_json_report.py
--rw-r--r--   0        0        0     1300 2023-02-28 14:39:12.945649 mypy_json_report-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 mypy_json_report-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10702 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2331 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/README.md
+-rw-r--r--   0        0        0     9626 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/mypy_json_report.py
+-rw-r--r--   0        0        0     1300 2023-04-10 22:00:28.927009 mypy_json_report-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 mypy_json_report-1.0.2/PKG-INFO
```

### Comparing `mypy_json_report-1.0.1/LICENSE` & `mypy_json_report-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_json_report-1.0.1/README.md` & `mypy_json_report-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mypy_json_report-1.0.1/mypy_json_report.py` & `mypy_json_report-1.0.2/mypy_json_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             self.old_report.pop(filename, None)
         )
         new_errors_in_file = error_frequencies - old_report_counter
 
         self.num_new_errors += sum(new_errors_in_file.values())
         for new_error in new_errors_in_file:
             for line_number in line_numbers_by_error[new_error]:
-                self.error_lines.extend(messages_by_line_number[line_number])
+                self.error_lines.extend(messages_by_line_number.pop(line_number, []))
 
         # Find counts for errors resolved.
         resolved_errors = old_report_counter - error_frequencies
         self.num_fixed_errors += sum(resolved_errors.values())
 
     def diff_report(self) -> DiffReport:
         unseen_errors = sum(sum(errors.values()) for errors in self.old_report.values())
```

### Comparing `mypy_json_report-1.0.1/pyproject.toml` & `mypy_json_report-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mypy-json-report"
-version = "1.0.1"
+version = "1.0.2"
 description = "Generate a JSON report from your mypy output"
 authors = ["Charlie Denton <charlie@meshy.co.uk>"]
 license = "Apache-2.0"
 repository = "https://github.com/memrise/mypy-json-report"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `mypy_json_report-1.0.1/PKG-INFO` & `mypy_json_report-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-json-report
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate a JSON report from your mypy output
 Home-page: https://github.com/memrise/mypy-json-report
 License: Apache-2.0
 Author: Charlie Denton
 Author-email: charlie@meshy.co.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

