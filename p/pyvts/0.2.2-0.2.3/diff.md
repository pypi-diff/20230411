# Comparing `tmp/pyvts-0.2.2.macosx-13-arm64.tar.gz` & `tmp/pyvts-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.2.2.macosx-13-arm64.tar", last modified: Mon Apr 10 22:16:39 2023, max compression
+gzip compressed data, was "pyvts-0.2.3.tar", last modified: Mon Apr 10 22:20:25 2023, max compression
```

## Comparing `pyvts-0.2.2.macosx-13-arm64.tar` & `pyvts-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198736 ./
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198759 ./Users/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198783 ./Users/genteki/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198805 ./Users/genteki/.virtualenvs/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198829 ./Users/genteki/.virtualenvs/live2d/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198856 ./Users/genteki/.virtualenvs/live2d/lib/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198882 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198950 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.199900 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     2986 2023-04-10 22:16:39.195509 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:16:39.198613 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:16:39.195626 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:16:39.195767 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:16:39.195844 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/top_level.txt
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:20:25.272074 pyvts-0.2.3/
+-rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.3/LICENSE
+-rw-r--r--   0 genteki    (501) staff       (20)     2986 2023-04-10 22:20:25.271963 pyvts-0.2.3/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)     2191 2023-04-10 13:57:48.000000 pyvts-0.2.3/README.md
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:20:25.271072 pyvts-0.2.3/pyvts/
+-rw-r--r--   0 genteki    (501) staff       (20)      216 2023-04-10 22:20:08.000000 pyvts-0.2.3/pyvts/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.3/pyvts/config.py
+-rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.3/pyvts/error.py
+-rw-r--r--   0 genteki    (501) staff       (20)     6103 2023-04-10 07:13:50.000000 pyvts-0.2.3/pyvts/vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)    10273 2023-04-10 07:13:50.000000 pyvts-0.2.3/pyvts/vts_request.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:20:25.271785 pyvts-0.2.3/pyvts.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     2986 2023-04-10 22:20:25.000000 pyvts-0.2.3/pyvts.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:20:25.000000 pyvts-0.2.3/pyvts.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:20:25.000000 pyvts-0.2.3/pyvts.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:20:25.000000 pyvts-0.2.3/pyvts.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:20:25.000000 pyvts-0.2.3/pyvts.egg-info/top_level.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-10 22:20:25.272110 pyvts-0.2.3/setup.cfg
+-rw-r--r--   0 genteki    (501) staff       (20)     1173 2023-04-10 22:20:05.000000 pyvts-0.2.3/setup.py
```

### Comparing `./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/PKG-INFO` & `pyvts-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 4 - Beta
```

