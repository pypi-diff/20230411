# Comparing `tmp/cwinput-0.1.3.tar.gz` & `tmp/cwinput-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwinput-0.1.3.tar", last modified: Sun Nov 27 11:05:28 2022, max compression
+gzip compressed data, was "cwinput-0.1.4.tar", last modified: Tue Apr 11 19:35:06 2023, max compression
```

## Comparing `cwinput-0.1.3.tar` & `cwinput-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-27 11:05:28.666881 cwinput-0.1.3/
--rw-rw-rw-   0        0        0     1094 2022-11-27 09:46:01.000000 cwinput-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2324 2022-11-27 11:05:28.664866 cwinput-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      527 2022-11-27 10:44:20.000000 cwinput-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2022-11-27 11:05:28.637741 cwinput-0.1.3/cwinput/
--rw-rw-rw-   0        0        0      139 2022-11-27 11:04:34.000000 cwinput-0.1.3/cwinput/__init__.py
--rw-rw-rw-   0        0        0     1846 2022-11-27 09:40:04.000000 cwinput-0.1.3/cwinput/binds.py
--rw-rw-rw-   0        0        0     1608 2022-11-27 10:30:40.000000 cwinput-0.1.3/cwinput/main.py
-drwxrwxrwx   0        0        0        0 2022-11-27 11:05:28.662846 cwinput-0.1.3/cwinput.egg-info/
--rw-rw-rw-   0        0        0     2324 2022-11-27 11:05:28.000000 cwinput-0.1.3/cwinput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2022-11-27 11:05:28.000000 cwinput-0.1.3/cwinput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-27 11:05:28.000000 cwinput-0.1.3/cwinput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-11-27 11:05:28.000000 cwinput-0.1.3/cwinput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      613 2022-11-27 11:04:37.000000 cwinput-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-27 11:05:28.666881 cwinput-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      286 2022-11-27 11:04:40.000000 cwinput-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:35:06.703684 cwinput-0.1.4/
+-rw-rw-rw-   0        0        0     1094 2022-11-27 09:46:02.000000 cwinput-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2324 2023-04-11 19:35:06.702119 cwinput-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2022-11-27 10:44:22.000000 cwinput-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 19:35:06.654940 cwinput-0.1.4/cwinput/
+-rw-rw-rw-   0        0        0      139 2023-04-11 19:27:24.000000 cwinput-0.1.4/cwinput/__init__.py
+-rw-rw-rw-   0        0        0     2383 2023-04-11 19:27:00.000000 cwinput-0.1.4/cwinput/binds.py
+-rw-rw-rw-   0        0        0     1607 2023-04-11 19:24:38.000000 cwinput-0.1.4/cwinput/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:35:06.699602 cwinput-0.1.4/cwinput.egg-info/
+-rw-rw-rw-   0        0        0     2324 2023-04-11 19:35:06.000000 cwinput-0.1.4/cwinput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-11 19:35:06.000000 cwinput-0.1.4/cwinput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:35:06.000000 cwinput-0.1.4/cwinput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 19:35:06.000000 cwinput-0.1.4/cwinput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-04-11 19:27:41.000000 cwinput-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 19:35:06.703684 cwinput-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      271 2023-04-11 19:27:30.000000 cwinput-0.1.4/setup.py
```

### Comparing `cwinput-0.1.3/LICENSE` & `cwinput-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cwinput-0.1.3/PKG-INFO` & `cwinput-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwinput
-Version: 0.1.3
+Version: 0.1.4
 Summary: Listen to raw console input
 Author: Zhilkaidarov Damir
 Author-email: Zhilkaidarov Damir <rustam030201@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Zhilkaidarov Damir
```

### Comparing `cwinput-0.1.3/README.md` & `cwinput-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cwinput-0.1.3/cwinput/main.py` & `cwinput-0.1.4/cwinput/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         super(CWInput, self).__init__()
         self.running = False
 
     def subscribe(self, func: Callable) -> None:
         """
         Add new listener
 
-        NOTE: Listener should accept only one parameter 
+        NOTE: Listener should accept only one parameter
         """
         self.listeners.append(func)
 
     def unsubscribe(self, func: Callable) -> None:
         """
         Remove listener from list
         """
```

### Comparing `cwinput-0.1.3/cwinput.egg-info/PKG-INFO` & `cwinput-0.1.4/cwinput.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwinput
-Version: 0.1.3
+Version: 0.1.4
 Summary: Listen to raw console input
 Author: Zhilkaidarov Damir
 Author-email: Zhilkaidarov Damir <rustam030201@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Zhilkaidarov Damir
```

### Comparing `cwinput-0.1.3/pyproject.toml` & `cwinput-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [project]
 name = "cwinput"
-version = "0.1.3"
+version = "0.1.4"
 description = "Listen to raw console input"
 readme = "README.md"
-authors = [
-  { name = "Zhilkaidarov Damir", email = "rustam030201@gmail.com" }
-]
+authors = [{ name = "Zhilkaidarov Damir", email = "rustam030201@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
-Homepage = "https://github.com/mitaraaa/cwinput"
+Homepage = "https://github.com/mitaraaa/cwinput"
```

