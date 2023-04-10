# Comparing `tmp/pyvts-0.2.0.tar.gz` & `tmp/pyvts-0.2.1.macosx-13-arm64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.2.0.tar", last modified: Mon Apr 10 22:05:52 2023, max compression
+gzip compressed data, was "pyvts-0.2.1.macosx-13-arm64.tar", last modified: Mon Apr 10 22:13:04 2023, max compression
```

## Comparing `pyvts-0.2.0.tar` & `pyvts-0.2.1.macosx-13-arm64.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:05:52.715329 pyvts-0.2.0/
--rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.0/LICENSE
--rw-r--r--   0 genteki    (501) staff       (20)     2987 2023-04-10 22:05:52.715210 pyvts-0.2.0/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)     2191 2023-04-10 13:57:48.000000 pyvts-0.2.0/README.md
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:05:52.714304 pyvts-0.2.0/pyvts/
--rw-r--r--   0 genteki    (501) staff       (20)      216 2023-04-10 22:02:46.000000 pyvts-0.2.0/pyvts/__init__.py
--rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.0/pyvts/config.py
--rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.0/pyvts/error.py
--rw-r--r--   0 genteki    (501) staff       (20)     6103 2023-04-10 07:13:50.000000 pyvts-0.2.0/pyvts/vts.py
--rw-r--r--   0 genteki    (501) staff       (20)    10273 2023-04-10 07:13:50.000000 pyvts-0.2.0/pyvts/vts_request.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:05:52.715005 pyvts-0.2.0/pyvts.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     2987 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:05:52.000000 pyvts-0.2.0/pyvts.egg-info/top_level.txt
--rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-10 22:05:52.715372 pyvts-0.2.0/setup.cfg
--rw-r--r--   0 genteki    (501) staff       (20)     1196 2023-04-10 22:02:46.000000 pyvts-0.2.0/setup.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674318 ./
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674342 ./Users/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674366 ./Users/genteki/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674394 ./Users/genteki/.virtualenvs/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674416 ./Users/genteki/.virtualenvs/live2d/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674448 ./Users/genteki/.virtualenvs/live2d/lib/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674473 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.674543 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-10 22:13:04.675238 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     2986 2023-04-10 22:13:04.670907 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-10 22:13:04.674109 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:13:04.671039 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-10 22:13:04.671185 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-10 22:13:04.671270 ./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/top_level.txt
```

### Comparing `pyvts-0.2.0/PKG-INFO` & `./Users/genteki/.virtualenvs/live2d/lib/python3.9/site-packages/pyvts-0.2.1-py3.9.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

