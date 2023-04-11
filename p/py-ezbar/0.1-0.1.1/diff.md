# Comparing `tmp/py_ezbar-0.1.tar.gz` & `tmp/py_ezbar-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ezbar-0.1.tar", last modified: Tue Apr 11 19:43:03 2023, max compression
+gzip compressed data, was "py_ezbar-0.1.1.tar", last modified: Tue Apr 11 20:06:44 2023, max compression
```

## Comparing `py_ezbar-0.1.tar` & `py_ezbar-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 19:43:03.593075 py_ezbar-0.1/
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1080 2023-04-11 19:32:04.000000 py_ezbar-0.1/LICENSE
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 17:50:41.000000 py_ezbar-0.1/MANIFEST.in
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2510 2023-04-11 19:43:03.592885 py_ezbar-0.1/PKG-INFO
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      817 2023-04-11 19:30:29.000000 py_ezbar-0.1/README.md
-drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 19:43:03.592314 py_ezbar-0.1/py_ezbar.egg-info/
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2510 2023-04-11 19:43:03.000000 py_ezbar-0.1/py_ezbar.egg-info/PKG-INFO
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      208 2023-04-11 19:43:03.000000 py_ezbar-0.1/py_ezbar.egg-info/SOURCES.txt
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)        1 2023-04-11 19:43:03.000000 py_ezbar-0.1/py_ezbar.egg-info/dependency_links.txt
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)        1 2023-04-11 19:43:03.000000 py_ezbar-0.1/py_ezbar.egg-info/top_level.txt
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      436 2023-04-11 19:42:51.000000 py_ezbar-0.1/pyproject.toml
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)       38 2023-04-11 19:43:03.593130 py_ezbar-0.1/setup.cfg
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      646 2023-04-11 19:40:03.000000 py_ezbar-0.1/setup.py
-drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 19:43:03.592453 py_ezbar-0.1/tests/
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1114 2023-04-11 18:21:28.000000 py_ezbar-0.1/tests/test_progress_bar.py
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.297255 py_ezbar-0.1.1/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1080 2023-04-11 19:32:04.000000 py_ezbar-0.1.1/LICENSE
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2516 2023-04-11 20:06:44.297133 py_ezbar-0.1.1/PKG-INFO
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      821 2023-04-11 20:02:02.000000 py_ezbar-0.1.1/README.md
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.296019 py_ezbar-0.1.1/py_ezbar/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)       81 2023-04-11 20:02:30.000000 py_ezbar-0.1.1/py_ezbar/__init__.py
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      543 2023-04-08 00:43:58.000000 py_ezbar-0.1.1/py_ezbar/bar_styles.py
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1993 2023-04-08 00:50:37.000000 py_ezbar-0.1.1/py_ezbar/progress_bar.py
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.296749 py_ezbar-0.1.1/py_ezbar.egg-info/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2516 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/PKG-INFO
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      265 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/SOURCES.txt
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)        1 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/dependency_links.txt
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)        9 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/top_level.txt
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      436 2023-04-11 19:42:51.000000 py_ezbar-0.1.1/pyproject.toml
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)       38 2023-04-11 20:06:44.297309 py_ezbar-0.1.1/setup.cfg
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      648 2023-04-11 20:06:40.000000 py_ezbar-0.1.1/setup.py
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.296873 py_ezbar-0.1.1/tests/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1087 2023-04-11 20:03:21.000000 py_ezbar-0.1.1/tests/test_progress_bar.py
```

### Comparing `py_ezbar-0.1/LICENSE` & `py_ezbar-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ezbar-0.1/PKG-INFO` & `py_ezbar-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ezbar
-Version: 0.1
+Version: 0.1.1
 Summary: Simple progress bar for terminal
 Home-page: https://github.com/kdrkrgz/ez-bar
 Author: kadir-karagoz
 Author-email: Kadir Karagoz <kadir@kadirkaragoz.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kadir Karagoz
@@ -37,22 +37,22 @@
 
 # Ez-Bar
 
 Very simple customizable progress bar.
 
 ## Installation
 ```bash
-pip install ez-bar
+pip install py-ezbar
 ```
 
 ## Usage and Examples
 
 import, configure and use it's easy
 ```bash
-from ez-bar import ProgressBar, BarStyles, BarColors
+from py_ezbar import ProgressBar, BarStyles, BarColors
     
 progress_bar = ProgressBar(color=BarColors.YELLOW, style=BarStyles.DEFAULT, show_fractions=True)
 t = range(327)
 x = [fake.bs() for _ in range(5)]
 y = {
     "1": "a",
     "2": "b",
```

### Comparing `py_ezbar-0.1/README.md` & `py_ezbar-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 # Ez-Bar
 
 Very simple customizable progress bar.
 
 ## Installation
 ```bash
-pip install ez-bar
+pip install py-ezbar
 ```
 
 ## Usage and Examples
 
 import, configure and use it's easy
 ```bash
-from ez-bar import ProgressBar, BarStyles, BarColors
+from py_ezbar import ProgressBar, BarStyles, BarColors
     
 progress_bar = ProgressBar(color=BarColors.YELLOW, style=BarStyles.DEFAULT, show_fractions=True)
 t = range(327)
 x = [fake.bs() for _ in range(5)]
 y = {
     "1": "a",
     "2": "b",
```

### Comparing `py_ezbar-0.1/py_ezbar.egg-info/PKG-INFO` & `py_ezbar-0.1.1/py_ezbar.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ezbar
-Version: 0.1
+Version: 0.1.1
 Summary: Simple progress bar for terminal
 Home-page: https://github.com/kdrkrgz/ez-bar
 Author: kadir-karagoz
 Author-email: Kadir Karagoz <kadir@kadirkaragoz.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kadir Karagoz
@@ -37,22 +37,22 @@
 
 # Ez-Bar
 
 Very simple customizable progress bar.
 
 ## Installation
 ```bash
-pip install ez-bar
+pip install py-ezbar
 ```
 
 ## Usage and Examples
 
 import, configure and use it's easy
 ```bash
-from ez-bar import ProgressBar, BarStyles, BarColors
+from py_ezbar import ProgressBar, BarStyles, BarColors
     
 progress_bar = ProgressBar(color=BarColors.YELLOW, style=BarStyles.DEFAULT, show_fractions=True)
 t = range(327)
 x = [fake.bs() for _ in range(5)]
 y = {
     "1": "a",
     "2": "b",
```

### Comparing `py_ezbar-0.1/setup.py` & `py_ezbar-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ez-bar",
-    version="0.1",
+    version="0.1.1",
     author="kadir-karagoz",
     author_email="kadir@kadirkaragoz.com",
     description="Simple progress bar for terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kdrkrgz/ez-bar",
     packages=find_packages(),
```

### Comparing `py_ezbar-0.1/tests/test_progress_bar.py` & `py_ezbar-0.1.1/tests/test_progress_bar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-from ez_bar import ProgressBar
-from ez_bar.bar_styles import BarColors, BarStyles
+from py_ezbar import ProgressBar, BarStyles, BarColors
 
 
 class ProgressBarTestCase(unittest.TestCase):
     def setUp(self):
         self.range = range(5000)
         self.test_list = ["a", "b", "c", "d", "e", "f"]
         self.test_dict = {
```

