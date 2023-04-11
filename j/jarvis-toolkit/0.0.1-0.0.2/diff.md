# Comparing `tmp/jarvis-toolkit-0.0.1.tar.gz` & `tmp/jarvis-toolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis-toolkit-0.0.1.tar", last modified: Tue Apr 11 00:05:53 2023, max compression
+gzip compressed data, was "jarvis-toolkit-0.0.2.tar", last modified: Tue Apr 11 00:14:41 2023, max compression
```

## Comparing `jarvis-toolkit-0.0.1.tar` & `jarvis-toolkit-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.511957 jarvis-toolkit-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-10 23:17:32.000000 jarvis-toolkit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      606 2023-04-11 00:05:53.510957 jarvis-toolkit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-04-10 23:23:41.000000 jarvis-toolkit-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.491699 jarvis-toolkit-0.0.1/jarvis/
--rw-rw-rw-   0        0        0        0 2023-03-18 15:29:16.000000 jarvis-toolkit-0.0.1/jarvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.495891 jarvis-toolkit-0.0.1/jarvis/config/
--rw-rw-rw-   0        0        0       56 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.1/jarvis/config/__init__.py
--rw-rw-rw-   0        0        0      813 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.1/jarvis/config/openai.py
--rw-rw-rw-   0        0        0      519 2023-03-26 09:13:29.000000 jarvis-toolkit-0.0.1/jarvis/config/silero.py
--rw-rw-rw-   0        0        0      322 2023-03-18 23:09:28.000000 jarvis-toolkit-0.0.1/jarvis/config/sound.py
--rw-rw-rw-   0        0        0      528 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.1/jarvis/config/vosk.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.498446 jarvis-toolkit-0.0.1/jarvis/gpt/
--rw-rw-rw-   0        0        0     7540 2023-03-19 13:42:09.000000 jarvis-toolkit-0.0.1/jarvis/gpt/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-03-19 13:18:28.000000 jarvis-toolkit-0.0.1/jarvis/gpt/context.py
--rw-rw-rw-   0        0        0     1660 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.1/jarvis/gpt/primitives.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.499454 jarvis-toolkit-0.0.1/jarvis/silero/
--rw-rw-rw-   0        0        0      891 2023-03-26 21:15:36.000000 jarvis-toolkit-0.0.1/jarvis/silero/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.500453 jarvis-toolkit-0.0.1/jarvis/vosk_/
--rw-rw-rw-   0        0        0     2518 2023-03-26 21:14:09.000000 jarvis-toolkit-0.0.1/jarvis/vosk_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.503032 jarvis-toolkit-0.0.1/jarvis/whisper/
--rw-rw-rw-   0        0        0      901 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.1/jarvis/whisper/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-04-10 22:59:37.000000 jarvis-toolkit-0.0.1/jarvis/whisper/inputs.py
--rw-rw-rw-   0        0        0      609 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.1/jarvis/whisper/outputs.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:05:53.509957 jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-11 00:05:53.000000 jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-04-11 00:05:53.000000 jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 00:05:53.000000 jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-04-11 00:05:53.000000 jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 00:05:53.000000 jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      915 2023-04-11 00:03:51.000000 jarvis-toolkit-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 00:05:53.511957 jarvis-toolkit-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.613481 jarvis-toolkit-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-10 23:17:32.000000 jarvis-toolkit-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-04-11 00:14:41.612481 jarvis-toolkit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-04-10 23:23:41.000000 jarvis-toolkit-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.596307 jarvis-toolkit-0.0.2/jarvis/
+-rw-rw-rw-   0        0        0        0 2023-03-18 15:29:16.000000 jarvis-toolkit-0.0.2/jarvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.599935 jarvis-toolkit-0.0.2/jarvis/config/
+-rw-rw-rw-   0        0        0       56 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.2/jarvis/config/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.2/jarvis/config/openai.py
+-rw-rw-rw-   0        0        0      519 2023-03-26 09:13:29.000000 jarvis-toolkit-0.0.2/jarvis/config/silero.py
+-rw-rw-rw-   0        0        0      322 2023-03-18 23:09:28.000000 jarvis-toolkit-0.0.2/jarvis/config/sound.py
+-rw-rw-rw-   0        0        0      528 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.2/jarvis/config/vosk.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.602083 jarvis-toolkit-0.0.2/jarvis/gpt/
+-rw-rw-rw-   0        0        0     7540 2023-03-19 13:42:09.000000 jarvis-toolkit-0.0.2/jarvis/gpt/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-03-19 13:18:28.000000 jarvis-toolkit-0.0.2/jarvis/gpt/context.py
+-rw-rw-rw-   0        0        0     1660 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.2/jarvis/gpt/primitives.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.602083 jarvis-toolkit-0.0.2/jarvis/silero/
+-rw-rw-rw-   0        0        0      891 2023-03-26 21:15:36.000000 jarvis-toolkit-0.0.2/jarvis/silero/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.603802 jarvis-toolkit-0.0.2/jarvis/vosk_/
+-rw-rw-rw-   0        0        0     2518 2023-03-26 21:14:09.000000 jarvis-toolkit-0.0.2/jarvis/vosk_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.605808 jarvis-toolkit-0.0.2/jarvis/whisper/
+-rw-rw-rw-   0        0        0      901 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.2/jarvis/whisper/__init__.py
+-rw-rw-rw-   0        0        0     2269 2023-04-10 22:59:37.000000 jarvis-toolkit-0.0.2/jarvis/whisper/inputs.py
+-rw-rw-rw-   0        0        0      609 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.2/jarvis/whisper/outputs.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:14:41.612481 jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-04-11 00:14:41.000000 jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-04-11 00:14:41.000000 jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 00:14:41.000000 jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-04-11 00:14:41.000000 jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 00:14:41.000000 jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2023-04-11 00:10:21.000000 jarvis-toolkit-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 00:14:41.613481 jarvis-toolkit-0.0.2/setup.cfg
```

### Comparing `jarvis-toolkit-0.0.1/LICENSE` & `jarvis-toolkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/PKG-INFO` & `jarvis-toolkit-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: jarvis-toolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jarvis Toolkit
 Author-email: Artur Aliiev <pastordev@jarvis-toolkit.com>
 Project-URL: Homepage, https://bitbucket.org/jarvis-toolkit/jarvis-core/src/master/t
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jarvis-toolkit-0.0.1/jarvis/config/openai.py` & `jarvis-toolkit-0.0.2/jarvis/config/openai.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/config/silero.py` & `jarvis-toolkit-0.0.2/jarvis/config/silero.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/config/vosk.py` & `jarvis-toolkit-0.0.2/jarvis/config/vosk.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/gpt/__init__.py` & `jarvis-toolkit-0.0.2/jarvis/gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/gpt/context.py` & `jarvis-toolkit-0.0.2/jarvis/gpt/context.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/gpt/primitives.py` & `jarvis-toolkit-0.0.2/jarvis/gpt/primitives.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/silero/__init__.py` & `jarvis-toolkit-0.0.2/jarvis/silero/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/vosk_/__init__.py` & `jarvis-toolkit-0.0.2/jarvis/vosk_/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/whisper/__init__.py` & `jarvis-toolkit-0.0.2/jarvis/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/whisper/inputs.py` & `jarvis-toolkit-0.0.2/jarvis/whisper/inputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis/whisper/outputs.py` & `jarvis-toolkit-0.0.2/jarvis/whisper/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/PKG-INFO` & `jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: jarvis-toolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jarvis Toolkit
 Author-email: Artur Aliiev <pastordev@jarvis-toolkit.com>
 Project-URL: Homepage, https://bitbucket.org/jarvis-toolkit/jarvis-core/src/master/t
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jarvis-toolkit-0.0.1/jarvis_toolkit.egg-info/SOURCES.txt` & `jarvis-toolkit-0.0.2/jarvis_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.1/pyproject.toml` & `jarvis-toolkit-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools==65.5.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jarvis-toolkit"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Artur Aliiev", email = "pastordev@jarvis-toolkit.com" },
 ]
 description = "Jarvis Toolkit"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
@@ -30,9 +30,8 @@
     "vosk==0.3.45",
     "nltk",
     "numpy",
     "silero"
 ]
 [project.urls]
 "Homepage" = "https://bitbucket.org/jarvis-toolkit/jarvis-core/src/master/t"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

