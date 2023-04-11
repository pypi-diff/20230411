# Comparing `tmp/clera-0.0.4.tar.gz` & `tmp/clera-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clera-0.0.4.tar", last modified: Tue Apr 11 13:09:53 2023, max compression
+gzip compressed data, was "clera-0.0.5.tar", last modified: Tue Apr 11 13:14:31 2023, max compression
```

## Comparing `clera-0.0.4.tar` & `clera-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:53.159275 clera-0.0.4/
--rw-rw-rw-   0        0        0      306 2023-04-11 12:10:43.000000 clera-0.0.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1058 2023-04-01 11:32:04.000000 clera-0.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 11:31:56.000000 clera-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    17705 2023-04-11 13:09:53.157478 clera-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    16175 2023-04-11 12:09:09.000000 clera-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 13:09:53.159275 clera-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1289 2023-04-11 13:09:41.000000 clera-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:52.763521 clera-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:52.800236 clera-0.0.4/src/clera/
--rw-rw-rw-   0        0        0       44 2023-01-04 21:56:46.000000 clera-0.0.4/src/clera/__init__.py
--rw-rw-rw-   0        0        0    45872 2023-04-01 23:28:48.000000 clera-0.0.4/src/clera/core.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:52.765329 clera-0.0.4/src/clera/docs/
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:53.073505 clera-0.0.4/src/clera/docs/images/
--rw-rw-rw-   0        0        0     7524 2023-04-04 11:32:50.000000 clera-0.0.4/src/clera/docs/images/empty_window.png
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:53.081516 clera-0.0.4/src/clera/icons/
--rw-rw-rw-   0        0        0   290225 2023-02-13 13:07:36.000000 clera-0.0.4/src/clera/icons/hand-drawn-icon.png
--rw-rw-rw-   0        0        0    87456 2023-02-13 13:46:44.000000 clera-0.0.4/src/clera/icons/toon-icon.ico
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:53.150783 clera-0.0.4/src/clera/utils/
--rw-rw-rw-   0        0        0      121 2023-03-19 13:16:12.000000 clera-0.0.4/src/clera/utils/__init__.py
--rw-rw-rw-   0        0        0      129 2023-03-24 12:03:54.000000 clera-0.0.4/src/clera/utils/exceptions.py
--rw-rw-rw-   0        0        0    15007 2023-04-01 23:18:54.000000 clera-0.0.4/src/clera/utils/handlers.py
--rw-rw-rw-   0        0        0     1071 2023-03-19 13:17:06.000000 clera-0.0.4/src/clera/utils/keys.py
--rw-rw-rw-   0        0        0     6196 2023-03-24 12:02:34.000000 clera-0.0.4/src/clera/utils/procr.py
--rw-rw-rw-   0        0        0     3328 2023-03-24 12:03:42.000000 clera-0.0.4/src/clera/utils/style.py
--rw-rw-rw-   0        0        0    27094 2023-04-11 10:49:46.000000 clera-0.0.4/src/clera/widgets.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:09:53.071510 clera-0.0.4/src/clera.egg-info/
--rw-rw-rw-   0        0        0    17705 2023-04-11 13:09:52.000000 clera-0.0.4/src/clera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-04-11 13:09:52.000000 clera-0.0.4/src/clera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:09:52.000000 clera-0.0.4/src/clera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 13:09:52.000000 clera-0.0.4/src/clera.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:09:52.000000 clera-0.0.4/src/clera.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.830162 clera-0.0.5/
+-rw-rw-rw-   0        0        0      306 2023-04-11 12:10:43.000000 clera-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1058 2023-04-01 11:32:04.000000 clera-0.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       42 2023-04-01 11:31:56.000000 clera-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    17705 2023-04-11 13:14:31.828026 clera-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16175 2023-04-11 12:09:09.000000 clera-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:14:31.830162 clera-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1315 2023-04-11 13:14:28.000000 clera-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.701942 clera-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.741306 clera-0.0.5/src/clera/
+-rw-rw-rw-   0        0        0       44 2023-01-04 21:56:46.000000 clera-0.0.5/src/clera/__init__.py
+-rw-rw-rw-   0        0        0    45872 2023-04-01 23:28:48.000000 clera-0.0.5/src/clera/core.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.707044 clera-0.0.5/src/clera/docs/
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.794115 clera-0.0.5/src/clera/docs/images/
+-rw-rw-rw-   0        0        0     7524 2023-04-04 11:32:50.000000 clera-0.0.5/src/clera/docs/images/empty_window.png
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.801676 clera-0.0.5/src/clera/icons/
+-rw-rw-rw-   0        0        0   290225 2023-02-13 13:07:36.000000 clera-0.0.5/src/clera/icons/hand-drawn-icon.png
+-rw-rw-rw-   0        0        0    87456 2023-02-13 13:46:44.000000 clera-0.0.5/src/clera/icons/toon-icon.ico
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.824035 clera-0.0.5/src/clera/utils/
+-rw-rw-rw-   0        0        0      121 2023-03-19 13:16:12.000000 clera-0.0.5/src/clera/utils/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-03-24 12:03:54.000000 clera-0.0.5/src/clera/utils/exceptions.py
+-rw-rw-rw-   0        0        0    15007 2023-04-01 23:18:54.000000 clera-0.0.5/src/clera/utils/handlers.py
+-rw-rw-rw-   0        0        0     1071 2023-03-19 13:17:06.000000 clera-0.0.5/src/clera/utils/keys.py
+-rw-rw-rw-   0        0        0     6196 2023-03-24 12:02:34.000000 clera-0.0.5/src/clera/utils/procr.py
+-rw-rw-rw-   0        0        0     3328 2023-03-24 12:03:42.000000 clera-0.0.5/src/clera/utils/style.py
+-rw-rw-rw-   0        0        0    27094 2023-04-11 10:49:46.000000 clera-0.0.5/src/clera/widgets.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:14:31.791124 clera-0.0.5/src/clera.egg-info/
+-rw-rw-rw-   0        0        0    17705 2023-04-11 13:14:31.000000 clera-0.0.5/src/clera.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-04-11 13:14:31.000000 clera-0.0.5/src/clera.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:14:31.000000 clera-0.0.5/src/clera.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 13:14:31.000000 clera-0.0.5/src/clera.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 13:14:31.000000 clera-0.0.5/src/clera.egg-info/top_level.txt
```

### Comparing `clera-0.0.4/LICENCE.txt` & `clera-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/PKG-INFO` & `clera-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clera
-Version: 0.0.4
+Version: 0.0.5
 Summary: Write Simple and Quick Python GUI Application
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: gui,clera,simple,simplegui,pyside,pyside6
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `clera-0.0.4/README.md` & `clera-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/setup.py` & `clera-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Write Simple and Quick Python GUI Application'
 KEYWORDS = ['gui', 'clera', 'simple', 'simplegui', 'pyside', 'pyside6']
 
 # LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 CLASSIFIERS = [
     'Development Status :: 2 - Pre-Alpha',
@@ -34,10 +34,11 @@
     long_description_content_type="text/markdown",
     licence='MIT',
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['PySide6'],
     keywords=KEYWORDS,
     classifiers=CLASSIFIERS,
-    package_dir={'': 'src'}
+    package_dir={'': 'src'},
+    py_modules=['clera']
 )
```

### Comparing `clera-0.0.4/src/clera/core.py` & `clera-0.0.5/src/clera/core.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/docs/images/empty_window.png` & `clera-0.0.5/src/clera/docs/images/empty_window.png`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/icons/hand-drawn-icon.png` & `clera-0.0.5/src/clera/icons/hand-drawn-icon.png`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/icons/toon-icon.ico` & `clera-0.0.5/src/clera/icons/toon-icon.ico`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/utils/handlers.py` & `clera-0.0.5/src/clera/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/utils/keys.py` & `clera-0.0.5/src/clera/utils/keys.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/utils/procr.py` & `clera-0.0.5/src/clera/utils/procr.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/utils/style.py` & `clera-0.0.5/src/clera/utils/style.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera/widgets.py` & `clera-0.0.5/src/clera/widgets.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.4/src/clera.egg-info/PKG-INFO` & `clera-0.0.5/src/clera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clera
-Version: 0.0.4
+Version: 0.0.5
 Summary: Write Simple and Quick Python GUI Application
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: gui,clera,simple,simplegui,pyside,pyside6
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `clera-0.0.4/src/clera.egg-info/SOURCES.txt` & `clera-0.0.5/src/clera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

