# Comparing `tmp/aadetools-0.0.2.tar.gz` & `tmp/aadetools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aadetools-0.0.2.tar", last modified: Tue Apr 11 21:29:03 2023, max compression
+gzip compressed data, was "aadetools-0.0.3.tar", last modified: Tue Apr 11 21:32:29 2023, max compression
```

## Comparing `aadetools-0.0.2.tar` & `aadetools-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:29:03.485142 aadetools-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       35 2023-03-19 10:52:53.000000 aadetools-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      521 2023-04-11 21:29:03.484075 aadetools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:29:03.481965 aadetools-0.0.2/aadetools.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-11 21:29:03.000000 aadetools-0.0.2/aadetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-11 21:29:03.000000 aadetools-0.0.2/aadetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:29:03.000000 aadetools-0.0.2/aadetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      244 2023-04-11 21:29:03.000000 aadetools-0.0.2/aadetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 21:29:03.000000 aadetools-0.0.2/aadetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:29:03.485142 aadetools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1802 2023-04-11 21:28:23.000000 aadetools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:32:29.878349 aadetools-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       35 2023-03-19 10:52:53.000000 aadetools-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      521 2023-04-11 21:32:29.877348 aadetools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:32:29.875305 aadetools-0.0.3/aadetools.egg-info/
+-rw-rw-rw-   0        0        0      521 2023-04-11 21:32:29.000000 aadetools-0.0.3/aadetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-11 21:32:29.000000 aadetools-0.0.3/aadetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:32:29.000000 aadetools-0.0.3/aadetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-04-11 21:32:29.000000 aadetools-0.0.3/aadetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 21:32:29.000000 aadetools-0.0.3/aadetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:32:29.878349 aadetools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2023-04-11 21:32:25.000000 aadetools-0.0.3/setup.py
```

### Comparing `aadetools-0.0.2/LICENSE.txt` & `aadetools-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.2/PKG-INFO` & `aadetools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.0.2/aadetools.egg-info/PKG-INFO` & `aadetools-0.0.3/aadetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aadetools-0.0.2/setup.py` & `aadetools-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,20 @@
     'coverage==4.5.4',
     'Sphinx==6.1.3',
     'twine==4.0.2',
     'six==1.16.0',
     'farasapy==0.0.14',
     'tqdm==4.62.2',
     'requests==2.25.1',
-    'regex==2021.4.4',
-    'pickle'
+    'regex==2021.4.4'
 ]
 
 setup(
     name="aadetools",                     # This is the name of the package
-    version="0.0.2",                        # The initial release version
+    version="0.0.3",                        # The initial release version
     url="",                                  #
     author_email="alaa.omer2009@gmail.com",   #
     author="Alaa' Omar",                     # Full name of the author
     description="Test Package Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=find_packages(include=['src.*']),    # List of all python modules to be installed
```

