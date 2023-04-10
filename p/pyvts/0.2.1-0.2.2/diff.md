# Comparing `tmp/pyvts-0.2.1.macosx-13-arm64.tar.gz` & `tmp/pyvts-0.2.2.macosx-13-arm64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.2.1.macosx-13-arm64.tar", last modified: Mon Apr 10 22:13:04 2023, max compression
+gzip compressed data, was "pyvts-0.2.2.macosx-13-arm64.tar", last modified: Mon Apr 10 22:16:39 2023, max compression
```

## Comparing `pyvts-0.2.1.macosx-13-arm64.tar` & `pyvts-0.2.2.macosx-13-arm64.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674318 ./
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674342 ./Users/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674366 ./Users/genteki/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674394 ./Users/genteki/.virtualenvs/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674416 ./Users/genteki/.virtualenvs/live2d/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674448 ./Users/genteki/.virtualenvs/live2d/lib/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674473 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674543 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.675238 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     2986 2023-04-10 22:13:04.670907 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:13:04.674109 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:13:04.671039 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:13:04.671185 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:13:04.671270 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/top_level.txt
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198736 ./
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198759 ./Users/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198783 ./Users/genteki/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198805 ./Users/genteki/.virtualenvs/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198829 ./Users/genteki/.virtualenvs/live2d/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198856 ./Users/genteki/.virtualenvs/live2d/lib/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198882 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.198950 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:16:39.199900 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     2986 2023-04-10 22:16:39.195509 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:16:39.198613 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:16:39.195626 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:16:39.195767 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:16:39.195844 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/top_level.txt
```

### Comparing `./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/PKG-INFO` & `./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.2-py3.9.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 4 - Beta
```

