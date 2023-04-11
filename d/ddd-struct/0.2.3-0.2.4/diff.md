# Comparing `tmp/ddd-struct-0.2.3.tar.gz` & `tmp/ddd-struct-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddd-struct-0.2.3.tar", last modified: Tue Apr 11 10:11:02 2023, max compression
+gzip compressed data, was "ddd-struct-0.2.4.tar", last modified: Tue Apr 11 11:51:21 2023, max compression
```

## Comparing `ddd-struct-0.2.3.tar` & `ddd-struct-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 10:11:02.552492 ddd-struct-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.544491 ddd-struct-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.544491 ddd-struct-0.2.3/src/ddd_struct/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/application/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8716 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/application/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/domain/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/infrastructure/repository_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/lib/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1873 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/common.py
--rw-rw-rw-   0 root         (0) root         (0)     5051 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/thread.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/warning.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.258086 ddd-struct-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/application/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8716 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/application/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/domain/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/infrastructure/repository_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/src/ddd_struct/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     5078 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/thread.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/warning.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/top_level.txt
```

### Comparing `ddd-struct-0.2.3/LICENSE` & `ddd-struct-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.3/setup.py` & `ddd-struct-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.3/src/ddd_struct/application/action.py` & `ddd-struct-0.2.4/src/ddd_struct/application/action.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.3/src/ddd_struct/domain/repository.py` & `ddd-struct-0.2.4/src/ddd_struct/domain/repository.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.3/src/ddd_struct/infrastructure/repository_impl.py` & `ddd-struct-0.2.4/src/ddd_struct/infrastructure/repository_impl.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.3/src/ddd_struct/lib/common.py` & `ddd-struct-0.2.4/src/ddd_struct/lib/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, string, random, hashlib, psutil, time
 from multiprocessing import Process, Event, Queue
 
 
 
 
-__all__=['get_random_string', 'get_md5']
+__all__=['get_random_string', 'get_md5', 'monitor_usage']
 def get_random_string(l=10):
     letters = string.digits + string.ascii_letters
     return ''.join(random.choice(letters) for i in range(l))
 
 
 def get_md5(txt):
     md5hash = hashlib.md5(str(txt).encode('utf-8'))
```

### Comparing `ddd-struct-0.2.3/src/ddd_struct/lib/thread.py` & `ddd-struct-0.2.4/src/ddd_struct/lib/thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio, traceback, time
 from typing import Tuple
 from functools import wraps, partial
 from copy import copy
 from .warning import deprecated
 
 
+__all__=['CoroutinePool']
 class TaskItem:
     def __init__(self, index, func, args, kwargs, retry=None) -> None:
         self.index = index
         self.func = func
         self.args = args
         self.kwargs = kwargs
         self.retry = retry
```

### Comparing `ddd-struct-0.2.3/src/ddd_struct/lib/warning.py` & `ddd-struct-0.2.4/src/ddd_struct/lib/warning.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.3/src/ddd_struct.egg-info/SOURCES.txt` & `ddd-struct-0.2.4/src/ddd_struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

