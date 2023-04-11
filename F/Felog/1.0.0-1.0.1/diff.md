# Comparing `tmp/Felog-1.0.0.tar.gz` & `tmp/Felog-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Felog-1.0.0.tar", last modified: Mon Apr 10 17:29:54 2023, max compression
+gzip compressed data, was "Felog-1.0.1.tar", last modified: Tue Apr 11 15:49:10 2023, max compression
```

## Comparing `Felog-1.0.0.tar` & `Felog-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 17:29:54.975562 Felog-1.0.0/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 17:29:54.975562 Felog-1.0.0/Felog.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)     2670 2023-04-10 17:29:54.000000 Felog-1.0.0/Felog.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      202 2023-04-10 17:29:54.000000 Felog-1.0.0/Felog.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-10 17:29:54.000000 Felog-1.0.0/Felog.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        8 2023-04-10 17:29:54.000000 Felog-1.0.0/Felog.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        6 2023-04-10 17:29:54.000000 Felog-1.0.0/Felog.egg-info/top_level.txt
--rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-04-10 16:27:09.000000 Felog-1.0.0/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)     2670 2023-04-10 17:29:54.975562 Felog-1.0.0/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)     2366 2023-04-10 17:25:21.000000 Felog-1.0.0/README.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-10 17:29:54.975562 Felog-1.0.0/felog/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-04-10 16:33:40.000000 Felog-1.0.0/felog/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2504 2023-04-10 17:20:08.000000 Felog-1.0.0/felog/core.py
--rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-10 17:29:54.975562 Felog-1.0.0/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)      630 2023-04-10 16:38:02.000000 Felog-1.0.0/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-11 15:49:10.125319 Felog-1.0.1/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-11 15:49:10.125319 Felog-1.0.1/Felog.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2670 2023-04-11 15:49:10.000000 Felog-1.0.1/Felog.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      174 2023-04-11 15:49:10.000000 Felog-1.0.1/Felog.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-11 15:49:10.000000 Felog-1.0.1/Felog.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        6 2023-04-11 15:49:10.000000 Felog-1.0.1/Felog.egg-info/top_level.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-04-10 16:27:09.000000 Felog-1.0.1/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)     2670 2023-04-11 15:49:10.125319 Felog-1.0.1/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     2366 2023-04-10 17:25:21.000000 Felog-1.0.1/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-11 15:49:10.125319 Felog-1.0.1/felog/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-04-10 16:33:40.000000 Felog-1.0.1/felog/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2504 2023-04-10 17:20:08.000000 Felog-1.0.1/felog/core.py
+-rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-11 15:49:10.125319 Felog-1.0.1/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)      632 2023-04-11 15:49:04.000000 Felog-1.0.1/setup.py
```

### Comparing `Felog-1.0.0/Felog.egg-info/PKG-INFO` & `Felog-1.0.1/Felog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Felog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Felog is yet another simple logging library to quickly and simply deploy logging with projects.
 Home-page: https://github.com/basegodfelix/felog
 Author: Felix Hernandez
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Felog-1.0.0/LICENSE` & `Felog-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Felog-1.0.0/PKG-INFO` & `Felog-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Felog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Felog is yet another simple logging library to quickly and simply deploy logging with projects.
 Home-page: https://github.com/basegodfelix/felog
 Author: Felix Hernandez
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Felog-1.0.0/README.md` & `Felog-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Felog-1.0.0/felog/core.py` & `Felog-1.0.1/felog/core.py`

 * *Files identical despite different names*

### Comparing `Felog-1.0.0/setup.py` & `Felog-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     path = os.path.dirname(os.path.abspath(__file__))
     with open(os.path.join(path, 'README.md'), encoding='utf-8') as f:
         tmp = f.read()
     return tmp
 
 setuptools.setup(
     name="Felog",
-    version="1.0.0",
+    version="1.0.1",
     author="Felix Hernandez",
     description="Felog is yet another simple logging library to quickly and simply deploy logging with projects.",
     packages=["felog"],
-    install_requires=["logging"],
+    # install_requires=["logging"],
     url="https://github.com/basegodfelix/felog",
     long_description = read(),
     long_description_content_type = 'text/markdown',
     license="MIT"
 )
```

