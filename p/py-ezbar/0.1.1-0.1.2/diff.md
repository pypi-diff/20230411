# Comparing `tmp/py_ezbar-0.1.1.tar.gz` & `tmp/py_ezbar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ezbar-0.1.1.tar", last modified: Tue Apr 11 20:06:44 2023, max compression
+gzip compressed data, was "py_ezbar-0.1.2.tar", last modified: Tue Apr 11 20:17:20 2023, max compression
```

## Comparing `py_ezbar-0.1.1.tar` & `py_ezbar-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.297255 py_ezbar-0.1.1/
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1080 2023-04-11 19:32:04.000000 py_ezbar-0.1.1/LICENSE
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2516 2023-04-11 20:06:44.297133 py_ezbar-0.1.1/PKG-INFO
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      821 2023-04-11 20:02:02.000000 py_ezbar-0.1.1/README.md
-drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.296019 py_ezbar-0.1.1/py_ezbar/
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)       81 2023-04-11 20:02:30.000000 py_ezbar-0.1.1/py_ezbar/__init__.py
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      543 2023-04-08 00:43:58.000000 py_ezbar-0.1.1/py_ezbar/bar_styles.py
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1993 2023-04-08 00:50:37.000000 py_ezbar-0.1.1/py_ezbar/progress_bar.py
-drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.296749 py_ezbar-0.1.1/py_ezbar.egg-info/
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2516 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/PKG-INFO
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      265 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/SOURCES.txt
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)        1 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/dependency_links.txt
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)        9 2023-04-11 20:06:44.000000 py_ezbar-0.1.1/py_ezbar.egg-info/top_level.txt
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      436 2023-04-11 19:42:51.000000 py_ezbar-0.1.1/pyproject.toml
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)       38 2023-04-11 20:06:44.297309 py_ezbar-0.1.1/setup.cfg
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)      648 2023-04-11 20:06:40.000000 py_ezbar-0.1.1/setup.py
-drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:06:44.296873 py_ezbar-0.1.1/tests/
--rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1087 2023-04-11 20:03:21.000000 py_ezbar-0.1.1/tests/test_progress_bar.py
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:17:20.468277 py_ezbar-0.1.2/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1080 2023-04-11 19:32:04.000000 py_ezbar-0.1.2/LICENSE
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2516 2023-04-11 20:17:20.468152 py_ezbar-0.1.2/PKG-INFO
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      821 2023-04-11 20:02:02.000000 py_ezbar-0.1.2/README.md
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:17:20.467161 py_ezbar-0.1.2/py_ezbar/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)       98 2023-04-11 20:15:28.000000 py_ezbar-0.1.2/py_ezbar/__init__.py
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      543 2023-04-08 00:43:58.000000 py_ezbar-0.1.2/py_ezbar/bar_styles.py
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2002 2023-04-11 20:15:48.000000 py_ezbar-0.1.2/py_ezbar/progress_bar.py
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:17:20.467792 py_ezbar-0.1.2/py_ezbar.egg-info/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     2516 2023-04-11 20:17:20.000000 py_ezbar-0.1.2/py_ezbar.egg-info/PKG-INFO
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      265 2023-04-11 20:17:20.000000 py_ezbar-0.1.2/py_ezbar.egg-info/SOURCES.txt
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)        1 2023-04-11 20:17:20.000000 py_ezbar-0.1.2/py_ezbar.egg-info/dependency_links.txt
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)        9 2023-04-11 20:17:20.000000 py_ezbar-0.1.2/py_ezbar.egg-info/top_level.txt
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      436 2023-04-11 19:42:51.000000 py_ezbar-0.1.2/pyproject.toml
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)       38 2023-04-11 20:17:20.468325 py_ezbar-0.1.2/setup.cfg
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)      648 2023-04-11 20:16:21.000000 py_ezbar-0.1.2/setup.py
+drwxr-xr-x   0 kadirkaragoz   (501) staff       (20)        0 2023-04-11 20:17:20.467912 py_ezbar-0.1.2/tests/
+-rw-r--r--   0 kadirkaragoz   (501) staff       (20)     1087 2023-04-11 20:03:21.000000 py_ezbar-0.1.2/tests/test_progress_bar.py
```

### Comparing `py_ezbar-0.1.1/LICENSE` & `py_ezbar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ezbar-0.1.1/PKG-INFO` & `py_ezbar-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ezbar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple progress bar for terminal
 Home-page: https://github.com/kdrkrgz/ez-bar
 Author: kadir-karagoz
 Author-email: Kadir Karagoz <kadir@kadirkaragoz.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kadir Karagoz
```

### Comparing `py_ezbar-0.1.1/README.md` & `py_ezbar-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py_ezbar-0.1.1/py_ezbar/bar_styles.py` & `py_ezbar-0.1.2/py_ezbar/bar_styles.py`

 * *Files identical despite different names*

### Comparing `py_ezbar-0.1.1/py_ezbar/progress_bar.py` & `py_ezbar-0.1.2/py_ezbar/progress_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from bar_styles import BAR_STYLES, BarColors, BarStyles
+from py_ezbar.bar_styles import BAR_STYLES, BarColors, BarStyles
 
 
 class ProgressBar:
     def __init__(self, color=BarColors.GREEN, style=BarStyles.DEFAULT, show_fractions=True, show_time=True):
         self.color = color.value
         self.style = BAR_STYLES.get(style.value)
         self.show_fractions = show_fractions
```

### Comparing `py_ezbar-0.1.1/py_ezbar.egg-info/PKG-INFO` & `py_ezbar-0.1.2/py_ezbar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ezbar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple progress bar for terminal
 Home-page: https://github.com/kdrkrgz/ez-bar
 Author: kadir-karagoz
 Author-email: Kadir Karagoz <kadir@kadirkaragoz.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kadir Karagoz
```

### Comparing `py_ezbar-0.1.1/setup.py` & `py_ezbar-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ez-bar",
-    version="0.1.1",
+    version="0.1.2",
     author="kadir-karagoz",
     author_email="kadir@kadirkaragoz.com",
     description="Simple progress bar for terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kdrkrgz/ez-bar",
     packages=find_packages(),
```

### Comparing `py_ezbar-0.1.1/tests/test_progress_bar.py` & `py_ezbar-0.1.2/tests/test_progress_bar.py`

 * *Files identical despite different names*

