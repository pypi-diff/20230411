# Comparing `tmp/py3d-0.0.8.tar.gz` & `tmp/py3d-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3d-0.0.8.tar", last modified: Tue Nov  2 16:42:52 2021, max compression
+gzip compressed data, was "dist/py3d-0.0.9.tar", last modified: Wed Nov  3 12:56:47 2021, max compression
```

## Comparing `py3d-0.0.8.tar` & `py3d-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-02 16:42:52.050843 py3d-0.0.8/
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    28086 2021-11-02 16:42:52.041761 py3d-0.0.8/PKG-INFO
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    18365 2021-06-06 10:33:39.000000 py3d-0.0.8/README.md
-drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-02 16:42:51.621898 py3d-0.0.8/py3d.egg-info/
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    28086 2021-11-02 16:42:50.000000 py3d-0.0.8/py3d.egg-info/PKG-INFO
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      210 2021-11-02 16:42:50.000000 py3d-0.0.8/py3d.egg-info/SOURCES.txt
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        1 2021-11-02 16:42:50.000000 py3d-0.0.8/py3d.egg-info/dependency_links.txt
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       14 2021-11-02 16:42:50.000000 py3d-0.0.8/py3d.egg-info/requires.txt
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        5 2021-11-02 16:42:50.000000 py3d-0.0.8/py3d.egg-info/top_level.txt
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    21734 2021-11-01 16:28:28.000000 py3d-0.0.8/py3d.py
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       38 2021-11-02 16:42:52.052834 py3d-0.0.8/setup.cfg
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      710 2021-11-02 16:42:43.000000 py3d-0.0.8/setup.py
-drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-02 16:42:51.958704 py3d-0.0.8/static/
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)  1800083 2021-10-23 14:06:00.000000 py3d-0.0.8/static/bundle.js
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)     4550 2021-06-18 15:29:48.000000 py3d-0.0.8/static/logo.png
--rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      527 2021-09-12 10:41:59.000000 py3d-0.0.8/viewer.html
+drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-03 12:56:47.682647 py3d-0.0.9/
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    28086 2021-11-03 12:56:47.679647 py3d-0.0.9/PKG-INFO
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    18365 2021-06-06 10:33:39.000000 py3d-0.0.9/README.md
+drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-03 12:56:46.439569 py3d-0.0.9/py3d.egg-info/
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    28086 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/PKG-INFO
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      220 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        1 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       14 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/requires.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       12 2021-11-03 12:56:45.000000 py3d-0.0.9/py3d.egg-info/top_level.txt
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)    21734 2021-11-01 16:28:28.000000 py3d-0.0.9/py3d.py
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)     5123 2021-10-23 06:22:53.000000 py3d-0.0.9/server.py
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)       38 2021-11-03 12:56:47.684649 py3d-0.0.9/setup.cfg
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      719 2021-11-03 12:56:00.000000 py3d-0.0.9/setup.py
+drwxrwxrwx   0 tumiz     (1000) tumiz     (1000)        0 2021-11-03 12:56:47.653184 py3d-0.0.9/static/
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)  1800083 2021-10-23 14:06:00.000000 py3d-0.0.9/static/bundle.js
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)     4550 2021-06-18 15:29:48.000000 py3d-0.0.9/static/logo.png
+-rwxrwxrwx   0 tumiz     (1000) tumiz     (1000)      527 2021-09-12 10:41:59.000000 py3d-0.0.9/viewer.html
```

### Comparing `py3d-0.0.8/PKG-INFO` & `py3d-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.8
+Version: 0.0.9
 Summary: a 3d library
 Home-page: https://github.com/Tumiz/scenario
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Description: *Copyright (c) Tumiz. Distributed under the terms of the GPL-3.0 License.*
```

### Comparing `py3d-0.0.8/README.md` & `py3d-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.8/py3d.egg-info/PKG-INFO` & `py3d-0.0.9/py3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.8
+Version: 0.0.9
 Summary: a 3d library
 Home-page: https://github.com/Tumiz/scenario
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Description: *Copyright (c) Tumiz. Distributed under the terms of the GPL-3.0 License.*
```

### Comparing `py3d-0.0.8/py3d.py` & `py3d-0.0.9/py3d.py`

 * *Files identical despite different names*

### Comparing `py3d-0.0.8/setup.py` & `py3d-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="py3d",
-    version="0.0.8",
+    version="0.0.9",
     description="a 3d library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Tumiz",
     author_email="hh11698@163.com",
     python_requires=">=3.5.0",
     url="https://github.com/Tumiz/scenario",
     install_requires=["numpy","tornado"],
     packages=find_packages(),
-    py_modules=["py3d"],
+    py_modules=["py3d","server"],
     data_files=[
         ("/py3d/static",["static/logo.png","static/bundle.js"]),
         ("/py3d",["viewer.html"])
         ],
     license="GPL-3.0 License"
 )
```

### Comparing `py3d-0.0.8/static/bundle.js` & `py3d-0.0.9/static/bundle.js`

 * *Files identical despite different names*

### Comparing `py3d-0.0.8/static/logo.png` & `py3d-0.0.9/static/logo.png`

 * *Files identical despite different names*

### Comparing `py3d-0.0.8/viewer.html` & `py3d-0.0.9/viewer.html`

 * *Files identical despite different names*

