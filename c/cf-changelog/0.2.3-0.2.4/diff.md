# Comparing `tmp/cf_changelog-0.2.3.tar.gz` & `tmp/cf_changelog-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-nwlavd_o\cf_changelog-0.2.3.tar", last modified: Tue Apr 11 21:13:35 2023, max compression
+gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-feq7xq7w\cf_changelog-0.2.4.tar", last modified: Tue Apr 11 21:16:32 2023, max compression
```

## Comparing `cf_changelog-0.2.3.tar` & `cf_changelog-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:13:35.000000 cf_changelog-0.2.3/
--rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      196 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1175 2023-04-11 19:59:42.000000 cf_changelog-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog/
--rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-0.2.3/cf_changelog/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-04-11 20:43:01.000000 cf_changelog-0.2.3/cf_changelog/cf_changelog.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog.egg-info/
--rw-rw-rw-   0        0        0      196 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 21:13:34.000000 cf_changelog-0.2.3/cf_changelog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:13:35.000000 cf_changelog-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      537 2023-04-11 21:12:44.000000 cf_changelog-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/
+-rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      196 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1175 2023-04-11 19:59:42.000000 cf_changelog-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog/
+-rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-0.2.4/cf_changelog/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-04-11 20:43:01.000000 cf_changelog-0.2.4/cf_changelog/cf_changelog.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/cf_changelog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:16:32.000000 cf_changelog-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      539 2023-04-11 21:15:43.000000 cf_changelog-0.2.4/setup.py
```

### Comparing `cf_changelog-0.2.3/LICENSE` & `cf_changelog-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_changelog-0.2.3/README.md` & `cf_changelog-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cf_changelog-0.2.3/cf_changelog/cf_changelog.py` & `cf_changelog-0.2.4/cf_changelog/cf_changelog.py`

 * *Files identical despite different names*

### Comparing `cf_changelog-0.2.3/setup.py` & `cf_changelog-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(name='cf_changelog',
-      version='0.2.3',
+      version='0.2.4',
       description='Conflict-Free Changelog manager',
       author='Paweł Sałek',
       author_email='salekpawel@gmail.com',
       url='',
       packages=['cf_changelog', ],
       install_requires=[
-        'GitPython >= 3.1',
+        'GitPython >= 3.1.0',
         'pyyaml >= 6.0',
         'schema >= 0.7.0',
       ],
       entry_points={
         'console_scripts': [
             'cf_changelog = cf_changelog:main',
         ]
```

