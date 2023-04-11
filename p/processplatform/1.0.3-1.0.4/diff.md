# Comparing `tmp/processplatform-1.0.3.tar.gz` & `tmp/processplatform-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processplatform-1.0.3.tar", last modified: Tue Apr 11 01:38:13 2023, max compression
+gzip compressed data, was "processplatform-1.0.4.tar", last modified: Tue Apr 11 02:24:49 2023, max compression
```

## Comparing `processplatform-1.0.3.tar` & `processplatform-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 01:38:13.369964 processplatform-1.0.3/
--rw-rw-rw-   0        0        0      595 2023-04-11 01:38:13.369964 processplatform-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 01:38:13.351398 processplatform-1.0.3/processplatform/
--rw-rw-rw-   0        0        0     1096 2023-04-11 00:04:57.000000 processplatform-1.0.3/processplatform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 01:38:13.356284 processplatform-1.0.3/processplatform/bin/
--rwxrwxrwx   0        0        0  8157160 2023-04-10 23:57:08.000000 processplatform-1.0.3/processplatform/bin/get_process.exe
-drwxrwxrwx   0        0        0        0 2023-04-11 01:38:13.355306 processplatform-1.0.3/processplatform.egg-info/
--rw-rw-rw-   0        0        0      595 2023-04-11 01:38:12.000000 processplatform-1.0.3/processplatform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-11 01:38:12.000000 processplatform-1.0.3/processplatform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 01:38:12.000000 processplatform-1.0.3/processplatform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 01:38:12.000000 processplatform-1.0.3/processplatform.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 01:38:13.370940 processplatform-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-11 01:38:05.000000 processplatform-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:24:49.463279 processplatform-1.0.4/
+-rw-rw-rw-   0        0        0      601 2023-04-11 02:24:49.463279 processplatform-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 02:24:49.456439 processplatform-1.0.4/processplatform/
+-rw-rw-rw-   0        0        0   388620 2023-04-11 02:24:09.000000 processplatform-1.0.4/processplatform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:24:49.461324 processplatform-1.0.4/processplatform.egg-info/
+-rw-rw-rw-   0        0        0      601 2023-04-11 02:24:49.000000 processplatform-1.0.4/processplatform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-11 02:24:49.000000 processplatform-1.0.4/processplatform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:24:49.000000 processplatform-1.0.4/processplatform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 02:24:49.000000 processplatform-1.0.4/processplatform.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:24:49.463279 processplatform-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-04-11 02:24:36.000000 processplatform-1.0.4/setup.py
```

### Comparing `processplatform-1.0.3/PKG-INFO` & `processplatform-1.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: processplatform
-Version: 1.0.3
-Summary: Computer process information
+Version: 1.0.4
+Summary: Gain computer process information
 Home-page: https://google.com
 Author: vesper
 Author-email: google@gmail.com
 License: MIT
-Description: Get any computer information or python plugins path with a simple get command.
+Description: Gain any computer information or python plugins path with a simple get command.
 Keywords: process
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `processplatform-1.0.3/processplatform.egg-info/PKG-INFO` & `processplatform-1.0.4/processplatform.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: processplatform
-Version: 1.0.3
-Summary: Computer process information
+Version: 1.0.4
+Summary: Gain computer process information
 Home-page: https://google.com
 Author: vesper
 Author-email: google@gmail.com
 License: MIT
-Description: Get any computer information or python plugins path with a simple get command.
+Description: Gain any computer information or python plugins path with a simple get command.
 Keywords: process
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

