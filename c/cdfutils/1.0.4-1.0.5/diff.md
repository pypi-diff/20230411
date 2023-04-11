# Comparing `tmp/cdfutils-1.0.4-py3-none-any.whl.zip` & `tmp/cdfutils-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,11 @@
-Zip file size: 10649 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    25589 b- defN 22-Dec-12 11:14 cdfutils-1.0.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1395 b- defN 22-Dec-12 11:14 cdfutils-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Dec-12 11:14 cdfutils-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 22-Dec-12 11:14 cdfutils-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      395 b- defN 22-Dec-12 11:14 cdfutils-1.0.4.dist-info/RECORD
-5 files, 27472 bytes uncompressed, 9911 bytes compressed:  63.9%
+Zip file size: 14183 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     3085 b- defN 22-Dec-13 04:38 cdfutils/Config.py
+-rw-rw-rw-  2.0 fat     3957 b- defN 23-Mar-31 10:03 cdfutils/DotNet.py
+-rw-rw-rw-  2.0 fat     1061 b- defN 22-Jun-27 06:25 cdfutils/Textfile.py
+-rw-rw-rw-  2.0 fat      341 b- defN 22-Dec-13 03:59 cdfutils/__init__.py
+-rw-rw-rw-  2.0 fat    25589 b- defN 23-Apr-11 00:15 cdfutils-1.0.5.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1404 b- defN 23-Apr-11 00:15 cdfutils-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 00:15 cdfutils-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-11 00:15 cdfutils-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      698 b- defN 23-Apr-11 00:15 cdfutils-1.0.5.dist-info/RECORD
+9 files, 36236 bytes uncompressed, 12989 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,16 +1,28 @@
-Filename: cdfutils-1.0.4.dist-info/LICENSE.txt
+Filename: cdfutils/Config.py
 Comment: 
 
-Filename: cdfutils-1.0.4.dist-info/METADATA
+Filename: cdfutils/DotNet.py
 Comment: 
 
-Filename: cdfutils-1.0.4.dist-info/WHEEL
+Filename: cdfutils/Textfile.py
 Comment: 
 
-Filename: cdfutils-1.0.4.dist-info/top_level.txt
+Filename: cdfutils/__init__.py
 Comment: 
 
-Filename: cdfutils-1.0.4.dist-info/RECORD
+Filename: cdfutils-1.0.5.dist-info/LICENSE.txt
+Comment: 
+
+Filename: cdfutils-1.0.5.dist-info/METADATA
+Comment: 
+
+Filename: cdfutils-1.0.5.dist-info/WHEEL
+Comment: 
+
+Filename: cdfutils-1.0.5.dist-info/top_level.txt
+Comment: 
+
+Filename: cdfutils-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cdfutils-1.0.4.dist-info/LICENSE.txt` & `cdfutils-1.0.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cdfutils-1.0.4.dist-info/METADATA` & `cdfutils-1.0.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 Metadata-Version: 2.1
 Name: cdfutils
-Version: 1.0.4
+Version: 1.0.5
 Summary: A general utility library of miscellaneous functions and classes
 Home-page: https://github.com/cdfarrow/cdfutils
 Author: Craig Farrow
-License: UNKNOWN
 Platform: Windows
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # cdfutils
 
 A library of miscellaneous utility functions and classes
 that I've created for various projects. 
 
 ## Config
 
 + ConfigStore: A generic configuration class that persists values in a text file.
-
+    
 ## DotNet
 
 Some general helper classes for use with .NET Windows.Forms:
 
 + CustomMainMenu: Builds a full MainMenu from a supplied configuration.
 + CustomToolBar: Build a ToolBar from a supplied configuration.
 
 ## Textfile
 
 Utility functions for reading from text files:
 
 + randomLine(): return a random line from a file.
 + randomSection(): return a random section (delimited by lines starting 
     with #) from a file.
-
-
```

