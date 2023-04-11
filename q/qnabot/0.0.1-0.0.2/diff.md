# Comparing `tmp/qnabot-0.0.1.tar.gz` & `tmp/qnabot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnabot-0.0.1.tar", last modified: Tue Apr 11 19:52:01 2023, max compression
+gzip compressed data, was "qnabot-0.0.2.tar", last modified: Tue Apr 11 20:04:50 2023, max compression
```

## Comparing `qnabot-0.0.1.tar` & `qnabot-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-11 19:52:01.353076 qnabot-0.0.1/
--rw-r--r--   0 momegas    (501) staff       (20)     1524 2023-04-11 19:52:01.352939 qnabot-0.0.1/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)     1164 2023-04-11 19:46:24.000000 qnabot-0.0.1/README.md
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-11 19:52:01.352328 qnabot-0.0.1/qnabot/
--rw-r--r--   0 momegas    (501) staff       (20)     3228 2023-04-11 19:00:03.000000 qnabot-0.0.1/qnabot/QnABot.py
--rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-11 19:01:30.000000 qnabot-0.0.1/qnabot/__init__.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-11 19:52:01.352763 qnabot-0.0.1/qnabot.egg-info/
--rw-r--r--   0 momegas    (501) staff       (20)     1524 2023-04-11 19:52:01.000000 qnabot-0.0.1/qnabot.egg-info/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)      174 2023-04-11 19:52:01.000000 qnabot-0.0.1/qnabot.egg-info/SOURCES.txt
--rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-11 19:52:01.000000 qnabot-0.0.1/qnabot.egg-info/dependency_links.txt
--rw-r--r--   0 momegas    (501) staff       (20)        7 2023-04-11 19:52:01.000000 qnabot-0.0.1/qnabot.egg-info/top_level.txt
--rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-11 19:52:01.353117 qnabot-0.0.1/setup.cfg
--rw-r--r--   0 momegas    (501) staff       (20)      695 2023-04-11 19:51:59.000000 qnabot-0.0.1/setup.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-11 20:04:50.034061 qnabot-0.0.2/
+-rw-r--r--   0 momegas    (501) staff       (20)     1524 2023-04-11 20:04:50.033930 qnabot-0.0.2/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)     1164 2023-04-11 19:46:24.000000 qnabot-0.0.2/README.md
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-11 20:04:50.033239 qnabot-0.0.2/qnabot/
+-rw-r--r--   0 momegas    (501) staff       (20)     3228 2023-04-11 19:00:03.000000 qnabot-0.0.2/qnabot/QnABot.py
+-rw-r--r--   0 momegas    (501) staff       (20)       26 2023-04-11 20:04:01.000000 qnabot-0.0.2/qnabot/__init__.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-11 20:04:50.033773 qnabot-0.0.2/qnabot.egg-info/
+-rw-r--r--   0 momegas    (501) staff       (20)     1524 2023-04-11 20:04:50.000000 qnabot-0.0.2/qnabot.egg-info/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)      174 2023-04-11 20:04:50.000000 qnabot-0.0.2/qnabot.egg-info/SOURCES.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-11 20:04:50.000000 qnabot-0.0.2/qnabot.egg-info/dependency_links.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        7 2023-04-11 20:04:50.000000 qnabot-0.0.2/qnabot.egg-info/top_level.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-11 20:04:50.034185 qnabot-0.0.2/setup.cfg
+-rw-r--r--   0 momegas    (501) staff       (20)      714 2023-04-11 20:04:31.000000 qnabot-0.0.2/setup.py
```

### Comparing `qnabot-0.0.1/PKG-INFO` & `qnabot-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnabot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create a question answering over docs bot with one line of code.
 Home-page: https://github.com/momegas/qnabot
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qnabot-0.0.1/README.md` & `qnabot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qnabot-0.0.1/qnabot/QnABot.py` & `qnabot-0.0.2/qnabot/QnABot.py`

 * *Files identical despite different names*

### Comparing `qnabot-0.0.1/qnabot.egg-info/PKG-INFO` & `qnabot-0.0.2/qnabot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnabot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create a question answering over docs bot with one line of code.
 Home-page: https://github.com/momegas/qnabot
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qnabot-0.0.1/setup.py` & `qnabot-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
 
+VERSION = "0.0.2"
+
 setup(
     name="qnabot",
-    version="0.0.1",
+    version=VERSION,
     packages=find_packages(),
     install_requires=[
         # List your package's dependencies here, e.g.,
         # "numpy>=1.18",
     ],
     author="Megaklis Vasilakis",
     author_email="megaklis.vasilakis@gmail.com",
```

