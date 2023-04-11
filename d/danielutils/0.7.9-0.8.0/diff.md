# Comparing `tmp/danielutils-0.7.9.tar.gz` & `tmp/danielutils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.7.9.tar", last modified: Mon Apr  3 14:15:10 2023, max compression
+gzip compressed data, was "danielutils-0.8.0.tar", last modified: Tue Apr 11 11:33:08 2023, max compression
```

## Comparing `danielutils-0.7.9.tar` & `danielutils-0.8.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.508825 danielutils-0.7.9/
--rw-rw-rw-   0        0        0      834 2023-04-03 14:15:10.507819 danielutils-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-03 14:15:10.000000 danielutils-0.7.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.477982 danielutils-0.7.9/danielutils/
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.496779 danielutils-0.7.9/danielutils/Classes/
--rw-rw-rw-   0        0        0      103 2023-04-02 21:16:20.000000 danielutils-0.7.9/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     1694 2023-04-02 21:17:25.000000 danielutils-0.7.9/danielutils/Classes/DataStructures.py
--rw-rw-rw-   0        0        0     3569 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Classes/TypedBuiltins.py
--rw-rw-rw-   0        0        0      117 2023-03-30 21:30:39.000000 danielutils-0.7.9/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0      904 2023-03-30 21:22:39.000000 danielutils-0.7.9/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     2159 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.499424 danielutils-0.7.9/danielutils/Conversions/
--rw-rw-rw-   0        0        0     2032 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.501429 danielutils-0.7.9/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.7.9/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      454 2022-10-14 16:32:03.000000 danielutils-0.7.9/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      389 2022-10-28 08:08:26.000000 danielutils-0.7.9/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.7.9/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      308 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.502982 danielutils-0.7.9/danielutils/DataStructures/
--rw-rw-rw-   0        0        0     2587 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/DataStructures/Graph.py
--rw-rw-rw-   0        0        0     2653 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/DataStructures/MarkovChain.py
--rw-rw-rw-   0        0        0       50 2022-10-28 07:57:32.000000 danielutils-0.7.9/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0    19685 2023-04-03 14:10:10.000000 danielutils-0.7.9/danielutils/Decorators.py
--rw-rw-rw-   0        0        0     1122 2023-04-03 14:02:27.000000 danielutils-0.7.9/danielutils/Exceptions.py
--rw-rw-rw-   0        0        0     8193 2023-04-03 11:53:26.000000 danielutils-0.7.9/danielutils/Functions.py
--rw-rw-rw-   0        0        0     6929 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/IO.py
--rw-rw-rw-   0        0        0     1324 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Internet.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.506314 danielutils-0.7.9/danielutils/Math/
--rw-rw-rw-   0        0        0     6036 2022-10-28 20:26:06.000000 danielutils-0.7.9/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      237 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0     1123 2023-03-30 21:00:45.000000 danielutils-0.7.9/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     6485 2023-04-02 21:11:12.000000 danielutils-0.7.9/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0      234 2023-04-02 21:14:13.000000 danielutils-0.7.9/danielutils/Math/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.7.9/danielutils/Path.py
--rw-rw-rw-   0        0        0     1357 2023-01-05 22:01:09.000000 danielutils-0.7.9/danielutils/Serialization.py
--rw-rw-rw-   0        0        0     4907 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/System.py
--rw-rw-rw-   0        0        0     6785 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Testing.py
--rw-rw-rw-   0        0        0     3183 2023-04-03 13:58:33.000000 danielutils-0.7.9/danielutils/Text.py
--rw-rw-rw-   0        0        0      330 2022-10-28 08:07:45.000000 danielutils-0.7.9/danielutils/Threading.py
--rw-rw-rw-   0        0        0      251 2022-10-07 22:49:20.000000 danielutils-0.7.9/danielutils/Time.py
--rw-rw-rw-   0        0        0      649 2023-01-18 20:34:53.000000 danielutils-0.7.9/danielutils/Typing.py
--rw-rw-rw-   0        0        0     1248 2023-04-02 14:10:39.000000 danielutils-0.7.9/danielutils/Windows.py
--rw-rw-rw-   0        0        0      456 2023-03-22 23:38:57.000000 danielutils-0.7.9/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:15:10.494085 danielutils-0.7.9/danielutils.egg-info/
--rw-rw-rw-   0        0        0      834 2023-04-03 14:15:10.000000 danielutils-0.7.9/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1288 2023-04-03 14:15:10.000000 danielutils-0.7.9/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 14:15:10.000000 danielutils-0.7.9/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-03 14:15:10.000000 danielutils-0.7.9/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-03 14:15:10.000000 danielutils-0.7.9/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      728 2023-04-03 14:15:10.000000 danielutils-0.7.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-03 14:15:10.508825 danielutils-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-04-03 14:15:10.000000 danielutils-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.969068 danielutils-0.8.0/
+-rw-rw-rw-   0        0        0      834 2023-04-11 11:33:08.968062 danielutils-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-11 11:33:08.000000 danielutils-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.938437 danielutils-0.8.0/danielutils/
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.959109 danielutils-0.8.0/danielutils/Classes/
+-rw-rw-rw-   0        0        0      103 2023-04-02 21:16:20.000000 danielutils-0.8.0/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     1694 2023-04-02 21:17:25.000000 danielutils-0.8.0/danielutils/Classes/DataStructures.py
+-rw-rw-rw-   0        0        0     3569 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Classes/TypedBuiltins.py
+-rw-rw-rw-   0        0        0      117 2023-03-30 21:30:39.000000 danielutils-0.8.0/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-03-30 21:22:39.000000 danielutils-0.8.0/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     2159 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.960561 danielutils-0.8.0/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     2032 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.963162 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      454 2022-10-14 16:32:03.000000 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      389 2022-10-28 08:08:26.000000 danielutils-0.8.0/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.0/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.964565 danielutils-0.8.0/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0     2587 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/DataStructures/Graph.py
+-rw-rw-rw-   0        0        0     2653 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/DataStructures/MarkovChain.py
+-rw-rw-rw-   0        0        0       50 2022-10-28 07:57:32.000000 danielutils-0.8.0/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0    19685 2023-04-03 14:10:10.000000 danielutils-0.8.0/danielutils/Decorators.py
+-rw-rw-rw-   0        0        0     1122 2023-04-03 14:02:27.000000 danielutils-0.8.0/danielutils/Exceptions.py
+-rw-rw-rw-   0        0        0     8193 2023-04-03 11:53:26.000000 danielutils-0.8.0/danielutils/Functions.py
+-rw-rw-rw-   0        0        0     7484 2023-04-03 20:39:45.000000 danielutils-0.8.0/danielutils/IO.py
+-rw-rw-rw-   0        0        0     1324 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Internet.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.967059 danielutils-0.8.0/danielutils/Math/
+-rw-rw-rw-   0        0        0     6036 2022-10-28 20:26:06.000000 danielutils-0.8.0/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      237 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0      860 2023-04-03 18:56:27.000000 danielutils-0.8.0/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     6485 2023-04-02 21:11:12.000000 danielutils-0.8.0/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.0/danielutils/Math/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.0/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2681 2023-04-11 11:31:36.000000 danielutils-0.8.0/danielutils/Print.py
+-rw-rw-rw-   0        0        0     1357 2023-01-05 22:01:09.000000 danielutils-0.8.0/danielutils/Serialization.py
+-rw-rw-rw-   0        0        0     4907 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/System.py
+-rw-rw-rw-   0        0        0     6785 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Testing.py
+-rw-rw-rw-   0        0        0     3183 2023-04-03 13:58:33.000000 danielutils-0.8.0/danielutils/Text.py
+-rw-rw-rw-   0        0        0      330 2022-10-28 08:07:45.000000 danielutils-0.8.0/danielutils/Threading.py
+-rw-rw-rw-   0        0        0      251 2022-10-07 22:49:20.000000 danielutils-0.8.0/danielutils/Time.py
+-rw-rw-rw-   0        0        0      649 2023-01-18 20:34:53.000000 danielutils-0.8.0/danielutils/Typing.py
+-rw-rw-rw-   0        0        0     1248 2023-04-02 14:10:39.000000 danielutils-0.8.0/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      480 2023-04-03 18:57:22.000000 danielutils-0.8.0/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:33:08.956109 danielutils-0.8.0/danielutils.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 11:33:08.000000 danielutils-0.8.0/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      728 2023-04-11 11:33:08.000000 danielutils-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 11:33:08.969068 danielutils-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-04-11 11:33:08.000000 danielutils-0.8.0/setup.py
```

### Comparing `danielutils-0.7.9/PKG-INFO` & `danielutils-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.7.9
+Version: 0.8.0
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: <danielnachumdev@gmail.com>
 License: MIT License
 Keywords: functions,decorators,methods
 Platform: All
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
-# danielutils v=0.7.9
+# danielutils v=0.8.0
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
```

### Comparing `danielutils-0.7.9/danielutils/Classes/DataStructures.py` & `danielutils-0.8.0/danielutils/Classes/DataStructures.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Classes/TypedBuiltins.py` & `danielutils-0.8.0/danielutils/Classes/TypedBuiltins.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Classes/frange.py` & `danielutils-0.8.0/danielutils/Classes/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Colors.py` & `danielutils-0.8.0/danielutils/Colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Conversions/MainConversions.py` & `danielutils-0.8.0/danielutils/Conversions/MainConversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/DataStructures/Graph.py` & `danielutils-0.8.0/danielutils/DataStructures/Graph.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/DataStructures/MarkovChain.py` & `danielutils-0.8.0/danielutils/DataStructures/MarkovChain.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Decorators.py` & `danielutils-0.8.0/danielutils/Decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Exceptions.py` & `danielutils-0.8.0/danielutils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Functions.py` & `danielutils-0.8.0/danielutils/Functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/IO.py` & `danielutils-0.8.0/danielutils/IO.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+from typing import IO
 import shutil
 import os
 from .Decorators import validate_explicit
 from typing import Union
 from pathlib import Path
 
 
@@ -246,14 +247,31 @@
     shutil.copy(src, dest)
 
 
 def copy_directory(src: str, dest: str) -> None:
     shutil.copy(src, dest)
 
 
+class IndentedWriter:
+    def __init__(self, output_stream: IO, indent_char: str = "\t"):
+        self.indent_level = 0
+        self.output_stream: IO = output_stream
+        self.indent_char = indent_char
+
+    def write(self, *args, sep=" ", end="\n"):
+        self.output_stream.write(
+            self.indent_level*self.indent_char + sep.join(args)+end)
+
+    def indent(self):
+        self.indent_level += 1
+
+    def undent(self):
+        self.indent_level = max(0, self.indent_level-1)
+
+
 __all__ = [
     "write_to_file",
     "path_exists",
     "file_exists",
     "directory_exists",
     "delete_file",
     "read_file",
@@ -268,9 +286,10 @@
     "get_file_type_from_directory",
     "get_file_type_from_directory_recursively",
     "rename_file",
     "move_file",
     "open_file",
     "move_directory",
     "copy_file",
-    "copy_directory"
+    "copy_directory",
+    "IndentedWriter"
 ]
```

### Comparing `danielutils-0.7.9/danielutils/Internet.py` & `danielutils-0.8.0/danielutils/Internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Math/Constants.py` & `danielutils-0.8.0/danielutils/Math/Constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Math/MathSymbols.py` & `danielutils-0.8.0/danielutils/Math/MathSymbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Path.py` & `danielutils-0.8.0/danielutils/Path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Serialization.py` & `danielutils-0.8.0/danielutils/Serialization.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/System.py` & `danielutils-0.8.0/danielutils/System.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Testing.py` & `danielutils-0.8.0/danielutils/Testing.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Text.py` & `danielutils-0.8.0/danielutils/Text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Typing.py` & `danielutils-0.8.0/danielutils/Typing.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils/Windows.py` & `danielutils-0.8.0/danielutils/Windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.7.9/danielutils.egg-info/PKG-INFO` & `danielutils-0.8.0/danielutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.7.9
+Version: 0.8.0
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: <danielnachumdev@gmail.com>
 License: MIT License
 Keywords: functions,decorators,methods
 Platform: All
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
-# danielutils v=0.7.9
+# danielutils v=0.8.0
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
```

### Comparing `danielutils-0.7.9/danielutils.egg-info/SOURCES.txt` & `danielutils-0.8.0/danielutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 danielutils/Data.py
 danielutils/Decorators.py
 danielutils/Exceptions.py
 danielutils/Functions.py
 danielutils/IO.py
 danielutils/Internet.py
 danielutils/Path.py
+danielutils/Print.py
 danielutils/Serialization.py
 danielutils/System.py
 danielutils/Testing.py
 danielutils/Text.py
 danielutils/Threading.py
 danielutils/Time.py
 danielutils/Typing.py
```

### Comparing `danielutils-0.7.9/pyproject.toml` & `danielutils-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.7.9"
+version = "0.8.0"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
 requires-python = ">=3.10.5"
 classifiers = [
```

### Comparing `danielutils-0.7.9/setup.py` & `danielutils-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.7.9"
+VERSION = "0.8.0"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
```

