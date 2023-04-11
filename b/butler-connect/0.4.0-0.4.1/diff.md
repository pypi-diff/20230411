# Comparing `tmp/butler-connect-0.4.0.tar.gz` & `tmp/butler-connect-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.4.0.tar", last modified: Wed Mar 22 08:42:52 2023, max compression
+gzip compressed data, was "butler-connect-0.4.1.tar", last modified: Tue Apr 11 15:46:23 2023, max compression
```

## Comparing `butler-connect-0.4.0.tar` & `butler-connect-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 08:42:52.138795 butler-connect-0.4.0/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1886 2023-03-22 08:42:52.137799 butler-connect-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      135 2023-03-22 08:42:33.000000 butler-connect-0.4.0/README.md
--rw-rw-rw-   0        0        0      738 2023-03-22 08:42:01.000000 butler-connect-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-22 08:42:52.138795 butler-connect-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-22 08:42:52.108105 butler-connect-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 08:42:52.116624 butler-connect-0.4.0/src/butlerConnect/
--rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.0/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    16289 2023-03-22 08:41:04.000000 butler-connect-0.4.0/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-03-22 08:42:52.119617 butler-connect-0.4.0/src/butlerDescription/
--rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.0/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      109 2023-02-25 11:14:38.000000 butler-connect-0.4.0/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.0/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.0/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-03-22 08:42:52.137799 butler-connect-0.4.0/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-03-22 08:42:52.000000 butler-connect-0.4.0/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-03-22 08:42:52.000000 butler-connect-0.4.0/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 08:42:52.000000 butler-connect-0.4.0/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-03-22 08:42:52.000000 butler-connect-0.4.0/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-03-22 08:42:52.000000 butler-connect-0.4.0/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.276066 butler-connect-0.4.1/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1886 2023-04-11 15:46:23.275067 butler-connect-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      135 2023-03-22 08:42:33.000000 butler-connect-0.4.1/README.md
+-rw-rw-rw-   0        0        0      738 2023-04-11 15:45:57.000000 butler-connect-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:46:23.276066 butler-connect-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.252828 butler-connect-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.255827 butler-connect-0.4.1/src/butlerConnect/
+-rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.1/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    16289 2023-03-22 08:41:04.000000 butler-connect-0.4.1/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.258827 butler-connect-0.4.1/src/butlerDescription/
+-rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.1/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.4.1/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.1/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.1/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:46:23.274068 butler-connect-0.4.1/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     1886 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-11 15:46:23.000000 butler-connect-0.4.1/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.4.0/LICENSE` & `butler-connect-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.0/PKG-INFO` & `butler-connect-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.0
+Version: 0.4.1
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `butler-connect-0.4.0/pyproject.toml` & `butler-connect-0.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.4.0"
+version = "0.4.1"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.4.0/src/butlerConnect/pikaButler.py` & `butler-connect-0.4.1/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.0/src/butlerDescription/control.py` & `butler-connect-0.4.1/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.0/src/butlerDescription/signal.py` & `butler-connect-0.4.1/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.0/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.4.1/src/butler_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.0
+Version: 0.4.1
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

