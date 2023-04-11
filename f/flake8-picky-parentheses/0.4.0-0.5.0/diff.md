# Comparing `tmp/flake8-picky-parentheses-0.4.0.tar.gz` & `tmp/flake8-picky-parentheses-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-picky-parentheses-0.4.0.tar", last modified: Wed Nov  2 13:28:57 2022, max compression
+gzip compressed data, was "flake8-picky-parentheses-0.5.0.tar", last modified: Tue Apr 11 09:43:25 2023, max compression
```

## Comparing `flake8-picky-parentheses-0.4.0.tar` & `flake8-picky-parentheses-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 rouven    (1000) rouven    (1000)        0 2022-11-02 13:28:57.166614 flake8-picky-parentheses-0.4.0/
--rw-rw-r--   0 rouven    (1000) rouven    (1000)    11357 2022-08-09 10:40:53.000000 flake8-picky-parentheses-0.4.0/LICENSE
--rw-rw-r--   0 rouven    (1000) rouven    (1000)     7941 2022-11-02 13:28:57.166614 flake8-picky-parentheses-0.4.0/PKG-INFO
--rw-rw-r--   0 rouven    (1000) rouven    (1000)     6416 2022-11-02 13:26:54.000000 flake8-picky-parentheses-0.4.0/README.md
-drwxrwxr-x   0 rouven    (1000) rouven    (1000)        0 2022-11-02 13:28:57.166614 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/
--rw-rw-r--   0 rouven    (1000) rouven    (1000)      258 2022-09-21 11:27:24.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/__init__.py
--rw-rw-r--   0 rouven    (1000) rouven    (1000)     6540 2022-09-22 13:25:55.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/_brackets_position.py
--rw-rw-r--   0 rouven    (1000) rouven    (1000)       18 2022-11-02 13:28:56.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/_meta.py
--rw-rw-r--   0 rouven    (1000) rouven    (1000)    18009 2022-10-25 12:00:57.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/_redundant_parentheses.py
--rw-rw-r--   0 rouven    (1000) rouven    (1000)     1999 2022-09-21 11:27:24.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/_util.py
-drwxrwxr-x   0 rouven    (1000) rouven    (1000)        0 2022-11-02 13:28:57.166614 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/
--rw-rw-r--   0 rouven    (1000) rouven    (1000)     7941 2022-11-02 13:28:57.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/PKG-INFO
--rw-rw-r--   0 rouven    (1000) rouven    (1000)      529 2022-11-02 13:28:57.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/SOURCES.txt
--rw-rw-r--   0 rouven    (1000) rouven    (1000)        1 2022-11-02 13:28:57.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/dependency_links.txt
--rw-rw-r--   0 rouven    (1000) rouven    (1000)      134 2022-11-02 13:28:57.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/entry_points.txt
--rw-rw-r--   0 rouven    (1000) rouven    (1000)       12 2022-11-02 13:28:57.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/requires.txt
--rw-rw-r--   0 rouven    (1000) rouven    (1000)       25 2022-11-02 13:28:57.000000 flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/top_level.txt
--rw-rw-r--   0 rouven    (1000) rouven    (1000)      375 2022-11-02 13:28:57.166614 flake8-picky-parentheses-0.4.0/setup.cfg
--rw-rw-r--   0 rouven    (1000) rouven    (1000)     2129 2022-11-02 13:26:54.000000 flake8-picky-parentheses-0.4.0/setup.py
+drwxrwxr-x   0 rouven    (1000) rouven    (1000)        0 2023-04-11 09:43:25.258134 flake8-picky-parentheses-0.5.0/
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)    11357 2022-08-09 10:40:53.000000 flake8-picky-parentheses-0.5.0/LICENSE
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)     8591 2023-04-11 09:43:25.258134 flake8-picky-parentheses-0.5.0/PKG-INFO
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)     7086 2023-04-11 09:38:09.000000 flake8-picky-parentheses-0.5.0/README.md
+drwxrwxr-x   0 rouven    (1000) rouven    (1000)        0 2023-04-11 09:43:25.258134 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)      258 2022-09-21 11:27:24.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/__init__.py
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)     6540 2023-04-11 09:38:09.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/_brackets_position.py
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)       18 2023-04-11 09:43:24.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/_meta.py
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)    18021 2023-04-11 08:14:24.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/_redundant_parentheses.py
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)     1999 2022-09-21 11:27:24.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/_util.py
+drwxrwxr-x   0 rouven    (1000) rouven    (1000)        0 2023-04-11 09:43:25.258134 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)     8591 2023-04-11 09:43:25.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/PKG-INFO
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)      597 2023-04-11 09:43:25.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/SOURCES.txt
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)        1 2023-04-11 09:43:25.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/dependency_links.txt
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)      133 2023-04-11 09:43:25.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/entry_points.txt
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)       12 2023-04-11 09:43:25.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/requires.txt
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)       25 2023-04-11 09:43:25.000000 flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/top_level.txt
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)      375 2023-04-11 09:43:25.258134 flake8-picky-parentheses-0.5.0/setup.cfg
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)     2129 2022-11-02 13:26:54.000000 flake8-picky-parentheses-0.5.0/setup.py
+drwxrwxr-x   0 rouven    (1000) rouven    (1000)        0 2023-04-11 09:43:25.258134 flake8-picky-parentheses-0.5.0/tests/
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)    17892 2023-04-11 09:38:09.000000 flake8-picky-parentheses-0.5.0/tests/test_brackets_position.py
+-rw-rw-r--   0 rouven    (1000) rouven    (1000)    38346 2023-04-11 09:38:09.000000 flake8-picky-parentheses-0.5.0/tests/test_redundant_parentheses.py
```

### Comparing `flake8-picky-parentheses-0.4.0/LICENSE` & `flake8-picky-parentheses-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-picky-parentheses-0.4.0/PKG-INFO` & `flake8-picky-parentheses-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: flake8-picky-parentheses
-Version: 0.4.0
+Version: 0.5.0
 Summary: flake8 plugin to nitpick about parenthesis, brackets, and braces
 Home-page: https://github.com/robsdedude/flake8-picky-parentheses
+Download-URL: https://pypi.python.org/pypi/flake8-picky-parentheses
 Author: Ivan Prychantovskyi, Rouven Bauer
 License: Apache License 2.0
-Download-URL: https://pypi.python.org/pypi/flake8-picky-parentheses
 Project-URL: Issue Tracker, https://github.com/robsdedude/flake8-picky-parentheses/issues
 Project-URL: Source Code, https://github.com/robsdedude/flake8-picky-parentheses
 Project-URL: Changelog, https://github.com/robsdedude/flake8-picky-parentheses/blob/master/CHANGELOG.md
 Keywords: flake8,plugin,redundant,superfluous,extraneous,unnecessary,parentheses,parenthesis,parens,brackets,linter,linting,codestyle,code style
-Platform: UNKNOWN
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -87,16 +86,18 @@
 | Code                | Brief Descritption                                                     |
 |---------------------|------------------------------------------------------------------------|
 | [`PAR0xx`](#par0xx) | [Group] Redundant parentheses                                          |
 | [`PAR001`](#par001) | Redundant parentheses (general)                                        |
 | [`PAR002`](#par002) | Parenteheses used for tuple unpacking                                  |
 |                     |                                                                        |
 | [`PAR1xx`](#par1xx) | [Group] (Opinioinated) parentheses, brackets, braces not well-alinged  |
-| [`PAR101`](#par101) | Opening bracket at the end the line, closing bracket not on a new line |
-| [`PAR102`](#par102) | Closing bracket on a new line, but indentation missmatch               |
+| [`PAR101`](#par101) | Opening bracket is last, but closing is not on new line                |
+| [`PAR102`](#par102) | Closing bracket has different indentation than the line with the opening bracket |
+| [`PAR103`](#par103) | Consecutive opening brackets at the end of the line must have consecutive closing brackets. |
+| [`PAR104`](#par104) | Only operators and comments are allowed after a closing bracket on a new line |
 
 ### `PAR0xx`
 These are the error codes for the redundant parentheses checker.
 #### `PAR001`
 It means that you use redundant parentheses, and they do not help readability.
 For example:
 ```python
@@ -167,14 +168,47 @@
 # GOOD
 a = [
     1, 2,
     3, 4
 ]
 ```
 
+#### `PAR103`
+It means that consecutive opening brackets at the end of a line must have
+consecutive closing brackets.
+```python
+# BAD
+answer = func((
+    1, 2, 3, 4, 5,
+    )
+)
+
+# GOOD
+answer = func((
+    1, 2, 3, 4, 5,
+))
+```
+
+#### `PAR104`
+Only operators and comments are allowed after a closing bracket on a new line.
+```python
+# BAD
+a = func(
+    1, 2, 3, 4, 5
+) + 6
+
+# GOOD
+a = (
+    func(
+        1, 2, 3, 4, 5
+    )
+    + 6
+)
+```
+
 
 ## Details and Exceptions
 
 The redundant parentheses checker uses Python's `tokenize` and `ast` module to
 try to remove each pair of parentheses and see if the code still compiles and
 yields the same AST (i.e., is semantically equivalent).
 If it does, a flake (lint error) is reported. However, there are two notable
@@ -309,9 +343,7 @@
    (a + b
    )
    ```
 
 ## Additional Notes
 
 This plugin was developed to improve the code quality of Neo4j Python projects.
-
-
```

### Comparing `flake8-picky-parentheses-0.4.0/README.md` & `flake8-picky-parentheses-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,18 @@
 | Code                | Brief Descritption                                                     |
 |---------------------|------------------------------------------------------------------------|
 | [`PAR0xx`](#par0xx) | [Group] Redundant parentheses                                          |
 | [`PAR001`](#par001) | Redundant parentheses (general)                                        |
 | [`PAR002`](#par002) | Parenteheses used for tuple unpacking                                  |
 |                     |                                                                        |
 | [`PAR1xx`](#par1xx) | [Group] (Opinioinated) parentheses, brackets, braces not well-alinged  |
-| [`PAR101`](#par101) | Opening bracket at the end the line, closing bracket not on a new line |
-| [`PAR102`](#par102) | Closing bracket on a new line, but indentation missmatch               |
+| [`PAR101`](#par101) | Opening bracket is last, but closing is not on new line                |
+| [`PAR102`](#par102) | Closing bracket has different indentation than the line with the opening bracket |
+| [`PAR103`](#par103) | Consecutive opening brackets at the end of the line must have consecutive closing brackets. |
+| [`PAR104`](#par104) | Only operators and comments are allowed after a closing bracket on a new line |
 
 ### `PAR0xx`
 These are the error codes for the redundant parentheses checker.
 #### `PAR001`
 It means that you use redundant parentheses, and they do not help readability.
 For example:
 ```python
@@ -137,14 +139,47 @@
 # GOOD
 a = [
     1, 2,
     3, 4
 ]
 ```
 
+#### `PAR103`
+It means that consecutive opening brackets at the end of a line must have
+consecutive closing brackets.
+```python
+# BAD
+answer = func((
+    1, 2, 3, 4, 5,
+    )
+)
+
+# GOOD
+answer = func((
+    1, 2, 3, 4, 5,
+))
+```
+
+#### `PAR104`
+Only operators and comments are allowed after a closing bracket on a new line.
+```python
+# BAD
+a = func(
+    1, 2, 3, 4, 5
+) + 6
+
+# GOOD
+a = (
+    func(
+        1, 2, 3, 4, 5
+    )
+    + 6
+)
+```
+
 
 ## Details and Exceptions
 
 The redundant parentheses checker uses Python's `tokenize` and `ast` module to
 try to remove each pair of parentheses and see if the code still compiles and
 yields the same AST (i.e., is semantically equivalent).
 If it does, a flake (lint error) is reported. However, there are two notable
```

### Comparing `flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/_brackets_position.py` & `flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/_brackets_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                         == self.file_tokens[coords.token_indexes[0]].start[0]):
                     count += 1
                 if (self.file_tokens[coords.token_indexes[0] - count].type
                         == tokenize.STRING):
                     break
                 self.problems.append((
                     coords_close[0], coords_close[1],
-                    "PAR101: Closing bracket has different indentation than "
+                    "PAR102: Closing bracket has different indentation than "
                     "the line with the opening bracket"
                 ))
 
             # if lines ends with `[({`, there should be a line that starts
             # with `]})` (matching closing brackets)
             for offset, prev_coords in enumerate(
                 reversed(parens_coords_sorted[:cords_idx])
@@ -94,15 +94,15 @@
                     prev_coord_open_token_idx == coord_open_token_idx - offset
                 is_closing_sequence = \
                     prev_coord_close_token_idx == coord_close_token_idx \
                     + offset
                 if is_opening_sequence and not is_closing_sequence:
                     self.problems.append((
                         coords[0][0], coords[0][1],
-                        "PAR101: Consecutive opening brackets at the end of "
+                        "PAR103: Consecutive opening brackets at the end of "
                         "the line must have consecutive closing brackets."
                     ))
 
         # if there is a closing bracket on after a new line, this line should
         # only contain: operators and comments
         for coords in self.all_parens_coords:
             if coords[0] in self.problems:
@@ -138,11 +138,11 @@
                 if token.type in (tokenize.NL, tokenize.NEWLINE):
                     # reached the next line, all cool
                     break
                 if (token.type not in (tokenize.OP, tokenize.COMMENT)
                         and breaker != 1):
                     self.problems.append((
                         close_coords[0], close_coords[1],
-                        "PAR101: Only operators and comments are allowed "
+                        "PAR104: Only operators and comments are allowed "
                         "after a closing bracket on a new line"
                     ))
                     break
```

### Comparing `flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/_redundant_parentheses.py` & `flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/_redundant_parentheses.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 class LogicalLine:
     def __init__(
         self,
         line: str,
         line_offset: int,
-        tokens: t.Tuple[tokenize.TokenInfo] = None,
+        tokens: t.Optional[t.Tuple[tokenize.TokenInfo]] = None,
         column_offset: int = 0
     ):
         self.line = line
         self.line_offset = line_offset
         self.column_offset = column_offset
         self._tokens = tokens
```

### Comparing `flake8-picky-parentheses-0.4.0/flake8_picky_parentheses/_util.py` & `flake8-picky-parentheses-0.5.0/flake8_picky_parentheses/_util.py`

 * *Files identical despite different names*

### Comparing `flake8-picky-parentheses-0.4.0/flake8_picky_parentheses.egg-info/PKG-INFO` & `flake8-picky-parentheses-0.5.0/flake8_picky_parentheses.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: flake8-picky-parentheses
-Version: 0.4.0
+Version: 0.5.0
 Summary: flake8 plugin to nitpick about parenthesis, brackets, and braces
 Home-page: https://github.com/robsdedude/flake8-picky-parentheses
+Download-URL: https://pypi.python.org/pypi/flake8-picky-parentheses
 Author: Ivan Prychantovskyi, Rouven Bauer
 License: Apache License 2.0
-Download-URL: https://pypi.python.org/pypi/flake8-picky-parentheses
 Project-URL: Issue Tracker, https://github.com/robsdedude/flake8-picky-parentheses/issues
 Project-URL: Source Code, https://github.com/robsdedude/flake8-picky-parentheses
 Project-URL: Changelog, https://github.com/robsdedude/flake8-picky-parentheses/blob/master/CHANGELOG.md
 Keywords: flake8,plugin,redundant,superfluous,extraneous,unnecessary,parentheses,parenthesis,parens,brackets,linter,linting,codestyle,code style
-Platform: UNKNOWN
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -87,16 +86,18 @@
 | Code                | Brief Descritption                                                     |
 |---------------------|------------------------------------------------------------------------|
 | [`PAR0xx`](#par0xx) | [Group] Redundant parentheses                                          |
 | [`PAR001`](#par001) | Redundant parentheses (general)                                        |
 | [`PAR002`](#par002) | Parenteheses used for tuple unpacking                                  |
 |                     |                                                                        |
 | [`PAR1xx`](#par1xx) | [Group] (Opinioinated) parentheses, brackets, braces not well-alinged  |
-| [`PAR101`](#par101) | Opening bracket at the end the line, closing bracket not on a new line |
-| [`PAR102`](#par102) | Closing bracket on a new line, but indentation missmatch               |
+| [`PAR101`](#par101) | Opening bracket is last, but closing is not on new line                |
+| [`PAR102`](#par102) | Closing bracket has different indentation than the line with the opening bracket |
+| [`PAR103`](#par103) | Consecutive opening brackets at the end of the line must have consecutive closing brackets. |
+| [`PAR104`](#par104) | Only operators and comments are allowed after a closing bracket on a new line |
 
 ### `PAR0xx`
 These are the error codes for the redundant parentheses checker.
 #### `PAR001`
 It means that you use redundant parentheses, and they do not help readability.
 For example:
 ```python
@@ -167,14 +168,47 @@
 # GOOD
 a = [
     1, 2,
     3, 4
 ]
 ```
 
+#### `PAR103`
+It means that consecutive opening brackets at the end of a line must have
+consecutive closing brackets.
+```python
+# BAD
+answer = func((
+    1, 2, 3, 4, 5,
+    )
+)
+
+# GOOD
+answer = func((
+    1, 2, 3, 4, 5,
+))
+```
+
+#### `PAR104`
+Only operators and comments are allowed after a closing bracket on a new line.
+```python
+# BAD
+a = func(
+    1, 2, 3, 4, 5
+) + 6
+
+# GOOD
+a = (
+    func(
+        1, 2, 3, 4, 5
+    )
+    + 6
+)
+```
+
 
 ## Details and Exceptions
 
 The redundant parentheses checker uses Python's `tokenize` and `ast` module to
 try to remove each pair of parentheses and see if the code still compiles and
 yields the same AST (i.e., is semantically equivalent).
 If it does, a flake (lint error) is reported. However, there are two notable
@@ -309,9 +343,7 @@
    (a + b
    )
    ```
 
 ## Additional Notes
 
 This plugin was developed to improve the code quality of Neo4j Python projects.
-
-
```

### Comparing `flake8-picky-parentheses-0.4.0/setup.py` & `flake8-picky-parentheses-0.5.0/setup.py`

 * *Files identical despite different names*

