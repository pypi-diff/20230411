# Comparing `tmp/se_lib-0.22.tar.gz` & `tmp/se_lib-0.23.tar.gz`

## Comparing `se_lib-0.22.tar` & `se_lib-0.23.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.22/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.22/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.22/selib/.DS_Store
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 se_lib-0.22/selib/__init__.py
--rw-r--r--   0        0        0    62356 2020-02-02 00:00:00.000000 se_lib-0.22/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.22/LICENSE
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 se_lib-0.22/README.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 se_lib-0.22/pyproject.toml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 se_lib-0.22/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.23/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.23/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.23/selib/.DS_Store
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 se_lib-0.23/selib/__init__.py
+-rw-r--r--   0        0        0    62382 2020-02-02 00:00:00.000000 se_lib-0.23/selib/selib.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.23/LICENSE
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 se_lib-0.23/README.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 se_lib-0.23/pyproject.toml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 se_lib-0.23/PKG-INFO
```

### Comparing `se_lib-0.22/selib/.DS_Store` & `se_lib-0.23/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.22/selib/selib.py` & `se_lib-0.23/selib/selib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-se-lib Version .22
+se-lib Version .23
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
@@ -12,14 +12,15 @@
 
 import graphviz
 import textwrap
 import os
 import sys
 from os.path import exists
 import pandas as pd
+import matplotlib.pyplot as plt
 from copy import deepcopy
 
 # text for SVG included files
 
 actor_svg = """<?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <svg
    xmlns:dc="http://purl.org/dc/elements/1.1/"
@@ -1501,37 +1502,37 @@
 
     Returns
     ----------
     matplotlib graph
     """
     #print (outputs, len(outputs))
     for var in outputs:
-        fig, axis = plot.subplots(figsize=(4, 3))
+        fig, axis = plt.subplots(figsize=(4, 3))
         axis.set(xlabel='Time', ylabel=var)
-        axis.plot(output.index, output[var].values, label=var)
+        axis.plt(output.index, output[var].values, label=var)
         if len(outputs) > 1: axis.legend(loc="best", )
-        plot.show()
+        plt.show()
   
 def save_graph(*outputs, filename="graph.png"):
   """
   save graph to file
 
   Parameters
   ----------
   variables: variable name or list of variable names to plot on graph
   filename: file name with format extension
   """
   for var in outputs:
     #print(var)
-    fig, axis = plot.subplots()
+    fig, axis = plt.subplots()
     axis.set(xlabel='Time', ylabel=var)
-    axis.plot(output.index, output[var].values, label=var)
+    axis.plt(output.index, output[var].values, label=var)
     axis.legend(loc="best", )
     #plot.show()
-    plot.savefig(filename)
+    plt.savefig(filename)
             
 def run_model():
     """
     Executes the model
     
     Returns
     ----------
```

### Comparing `se_lib-0.22/LICENSE` & `se_lib-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `se_lib-0.22/README.md` & `se_lib-0.23/README.md`

 * *Files identical despite different names*

### Comparing `se_lib-0.22/PKG-INFO` & `se_lib-0.23/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.22
+Version: 0.23
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

