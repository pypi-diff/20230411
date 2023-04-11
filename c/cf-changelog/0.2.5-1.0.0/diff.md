# Comparing `tmp/cf_changelog-0.2.5.tar.gz` & `tmp/cf_changelog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-pcvvgjwk\cf_changelog-0.2.5.tar", last modified: Tue Apr 11 21:32:39 2023, max compression
+gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-zsmv9_rk\cf_changelog-1.0.0.tar", last modified: Tue Apr 11 21:41:09 2023, max compression
```

## Comparing `cf_changelog-0.2.5.tar` & `cf_changelog-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/
--rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     1509 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1175 2023-04-11 19:59:42.000000 cf_changelog-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog/
--rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-0.2.5/cf_changelog/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-04-11 20:43:01.000000 cf_changelog-0.2.5/cf_changelog/cf_changelog.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog.egg-info/
--rw-rw-rw-   0        0        0     1509 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/cf_changelog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:32:39.000000 cf_changelog-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-04-11 21:31:55.000000 cf_changelog-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/
+-rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1503 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-04-11 21:35:22.000000 cf_changelog-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog/
+-rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.0/cf_changelog/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-04-11 20:43:01.000000 cf_changelog-1.0.0/cf_changelog/cf_changelog.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/
+-rw-rw-rw-   0        0        0     1503 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-04-11 21:37:28.000000 cf_changelog-1.0.0/setup.py
```

### Comparing `cf_changelog-0.2.5/LICENSE` & `cf_changelog-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_changelog-0.2.5/PKG-INFO` & `cf_changelog-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_changelog
-Version: 0.2.5
+Version: 1.0.0
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,15 +17,15 @@
 ## Usage
 1. Install it from pip:
 ```bash
 pip install cf_changelog
 ```
 2. Create some changelog on different branches entries using:
 ```bash
-cf_changelog.py add
+cf_changelog add
 ```
 It is recommended to run this from root of your repository.
 This will invoke standard text editor (or notepad if standard editor is not configured), where you can fill a template with new features, bug fixes etc. Example:
 ```yaml
 New:
     - One new cool feature
     - Another cool feature
@@ -35,15 +35,15 @@
 ```
 
 3. Commit newly created files.
 4. Repeat 2 and 3 on different branches as many times as you need.
 5. Merge all branches.
 6. On merged branch run:
 ```bash
-cf_changelog.py release X.Y.Z
+cf_changelog release X.Y.Z
 ```
 where X.Y.Z is description of version you wan't to see in final changelog.
 7. Commit registered changes in git repository
 8. Enjoy your updated changelog.
 
 ## Project status
 It is very initial version. Manual tests passed. Waiting for some feedback before moving on.
```

### Comparing `cf_changelog-0.2.5/README.md` & `cf_changelog-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ## Usage
 1. Install it from pip:
 ```bash
 pip install cf_changelog
 ```
 2. Create some changelog on different branches entries using:
 ```bash
-cf_changelog.py add
+cf_changelog add
 ```
 It is recommended to run this from root of your repository.
 This will invoke standard text editor (or notepad if standard editor is not configured), where you can fill a template with new features, bug fixes etc. Example:
 ```yaml
 New:
     - One new cool feature
     - Another cool feature
@@ -24,15 +24,15 @@
 ```
 
 3. Commit newly created files.
 4. Repeat 2 and 3 on different branches as many times as you need.
 5. Merge all branches.
 6. On merged branch run:
 ```bash
-cf_changelog.py release X.Y.Z
+cf_changelog release X.Y.Z
 ```
 where X.Y.Z is description of version you wan't to see in final changelog.
 7. Commit registered changes in git repository
 8. Enjoy your updated changelog.
 
 ## Project status
 It is very initial version. Manual tests passed. Waiting for some feedback before moving on.
```

### Comparing `cf_changelog-0.2.5/cf_changelog/cf_changelog.py` & `cf_changelog-1.0.0/cf_changelog/cf_changelog.py`

 * *Files identical despite different names*

### Comparing `cf_changelog-0.2.5/cf_changelog.egg-info/PKG-INFO` & `cf_changelog-1.0.0/cf_changelog.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-changelog
-Version: 0.2.5
+Version: 1.0.0
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,15 +17,15 @@
 ## Usage
 1. Install it from pip:
 ```bash
 pip install cf_changelog
 ```
 2. Create some changelog on different branches entries using:
 ```bash
-cf_changelog.py add
+cf_changelog add
 ```
 It is recommended to run this from root of your repository.
 This will invoke standard text editor (or notepad if standard editor is not configured), where you can fill a template with new features, bug fixes etc. Example:
 ```yaml
 New:
     - One new cool feature
     - Another cool feature
@@ -35,15 +35,15 @@
 ```
 
 3. Commit newly created files.
 4. Repeat 2 and 3 on different branches as many times as you need.
 5. Merge all branches.
 6. On merged branch run:
 ```bash
-cf_changelog.py release X.Y.Z
+cf_changelog release X.Y.Z
 ```
 where X.Y.Z is description of version you wan't to see in final changelog.
 7. Commit registered changes in git repository
 8. Enjoy your updated changelog.
 
 ## Project status
 It is very initial version. Manual tests passed. Waiting for some feedback before moving on.
```

### Comparing `cf_changelog-0.2.5/setup.py` & `cf_changelog-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='cf_changelog',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version='0.2.5',
+      version='1.0.0',
       description='Conflict-Free Changelog manager',
       author='Paweł Sałek',
       author_email='salekpawel@gmail.com',
       url='https://gitlab.com/salekpawel/cf_changelog',
       packages=['cf_changelog', ],
       license="MIT",
       install_requires=[
```

