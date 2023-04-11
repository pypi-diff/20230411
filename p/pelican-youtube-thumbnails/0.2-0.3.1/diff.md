# Comparing `tmp/pelican-youtube-thumbnails-0.2.tar.gz` & `tmp/pelican-youtube-thumbnails-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-youtube-thumbnails-0.2.tar", last modified: Tue Apr 11 16:40:49 2023, max compression
+gzip compressed data, was "pelican-youtube-thumbnails-0.3.1.tar", last modified: Tue Apr 11 17:26:21 2023, max compression
```

## Comparing `pelican-youtube-thumbnails-0.2.tar` & `pelican-youtube-thumbnails-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 16:40:49.164936 pelican-youtube-thumbnails-0.2/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    34523 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.2/COPYING
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1624 2023-04-11 16:40:49.164936 pelican-youtube-thumbnails-0.2/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      635 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.2/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 16:40:49.164936 pelican-youtube-thumbnails-0.2/pelican_youtube_thumbnails.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1624 2023-04-11 16:40:49.000000 pelican-youtube-thumbnails-0.2/pelican_youtube_thumbnails.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      308 2023-04-11 16:40:49.000000 pelican-youtube-thumbnails-0.2/pelican_youtube_thumbnails.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-04-11 16:40:49.000000 pelican-youtube-thumbnails-0.2/pelican_youtube_thumbnails.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      131 2023-04-11 16:40:49.000000 pelican-youtube-thumbnails-0.2/pelican_youtube_thumbnails.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-04-11 16:40:49.000000 pelican-youtube-thumbnails-0.2/pelican_youtube_thumbnails.egg-info/top_level.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2023-04-11 16:40:49.164936 pelican-youtube-thumbnails-0.2/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1681 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.2/setup.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 16:40:49.164936 pelican-youtube-thumbnails-0.2/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10089 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.2/tests/test_youtube_thumbnails.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 17:26:21.602357 pelican-youtube-thumbnails-0.3.1/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    34523 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.3.1/COPYING
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       68 2023-04-11 17:13:05.000000 pelican-youtube-thumbnails-0.3.1/MANIFEST.in
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1724 2023-04-11 17:26:21.602357 pelican-youtube-thumbnails-0.3.1/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      733 2023-04-11 17:13:05.000000 pelican-youtube-thumbnails-0.3.1/README.md
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 17:26:21.598357 pelican-youtube-thumbnails-0.3.1/pelican/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 17:26:21.598357 pelican-youtube-thumbnails-0.3.1/pelican/plugins/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 17:26:21.602357 pelican-youtube-thumbnails-0.3.1/pelican/plugins/youtube_thumbnails/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      193 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.3.1/pelican/plugins/youtube_thumbnails/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      641 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.3.1/pelican/plugins/youtube_thumbnails/logo.png
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     6239 2023-04-11 17:17:03.000000 pelican-youtube-thumbnails-0.3.1/pelican/plugins/youtube_thumbnails/youtube_thumbnails.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 17:26:21.602357 pelican-youtube-thumbnails-0.3.1/pelican_youtube_thumbnails.egg-info/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1724 2023-04-11 17:26:21.000000 pelican-youtube-thumbnails-0.3.1/pelican_youtube_thumbnails.egg-info/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      468 2023-04-11 17:26:21.000000 pelican-youtube-thumbnails-0.3.1/pelican_youtube_thumbnails.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-04-11 17:26:21.000000 pelican-youtube-thumbnails-0.3.1/pelican_youtube_thumbnails.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      131 2023-04-11 17:26:21.000000 pelican-youtube-thumbnails-0.3.1/pelican_youtube_thumbnails.egg-info/requires.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        8 2023-04-11 17:26:21.000000 pelican-youtube-thumbnails-0.3.1/pelican_youtube_thumbnails.egg-info/top_level.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2023-04-11 17:26:21.602357 pelican-youtube-thumbnails-0.3.1/setup.cfg
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1799 2023-04-11 17:26:12.000000 pelican-youtube-thumbnails-0.3.1/setup.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-04-11 17:26:21.602357 pelican-youtube-thumbnails-0.3.1/tests/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10089 2023-04-11 16:40:27.000000 pelican-youtube-thumbnails-0.3.1/tests/test_youtube_thumbnails.py
```

### Comparing `pelican-youtube-thumbnails-0.2/COPYING` & `pelican-youtube-thumbnails-0.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `pelican-youtube-thumbnails-0.2/PKG-INFO` & `pelican-youtube-thumbnails-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-youtube-thumbnails
-Version: 0.2
+Version: 0.3.1
 Summary: Pelican plugin to link to YouTube videos by their thumbnail
 Home-page: https://github.com/FriedrichFroebel/pelican-youtube-thumbnails/
 Author: FriedrichFröbel
 License: AGPL-3.0
 Keywords: pelican,plugin,youtube
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -27,15 +27,17 @@
 
 Pelican plugin for YouTube videos.
 
 This Pelican plugin saves the thumbnails of included YouTube videos inside a local file and includes this image with an hyperlink to the YouTube video itself. This may be used to avoid third-party JavaScript and cookies caused by IFrames for YouTube videos.
 
 ## Installation
 
-You can easily install this plugin using *pip* straight from a source checkout: `python -m pip install .`
+The package is available on PyPI and can be installed using `pip install pelican-youtube-thumbnails`.
+
+Alternatively, you may want to install it straight from a source checkout: `python -m pip install .`
 
 ## Usage
 
 Include the plugin by adding it to your `pelicanconf.py` and referencing it inside your source files using
 
 ```
 .. youtube:: myVideoId
```

### Comparing `pelican-youtube-thumbnails-0.2/pelican_youtube_thumbnails.egg-info/PKG-INFO` & `pelican-youtube-thumbnails-0.3.1/pelican_youtube_thumbnails.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-youtube-thumbnails
-Version: 0.2
+Version: 0.3.1
 Summary: Pelican plugin to link to YouTube videos by their thumbnail
 Home-page: https://github.com/FriedrichFroebel/pelican-youtube-thumbnails/
 Author: FriedrichFröbel
 License: AGPL-3.0
 Keywords: pelican,plugin,youtube
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -27,15 +27,17 @@
 
 Pelican plugin for YouTube videos.
 
 This Pelican plugin saves the thumbnails of included YouTube videos inside a local file and includes this image with an hyperlink to the YouTube video itself. This may be used to avoid third-party JavaScript and cookies caused by IFrames for YouTube videos.
 
 ## Installation
 
-You can easily install this plugin using *pip* straight from a source checkout: `python -m pip install .`
+The package is available on PyPI and can be installed using `pip install pelican-youtube-thumbnails`.
+
+Alternatively, you may want to install it straight from a source checkout: `python -m pip install .`
 
 ## Usage
 
 Include the plugin by adding it to your `pelicanconf.py` and referencing it inside your source files using
 
 ```
 .. youtube:: myVideoId
```

### Comparing `pelican-youtube-thumbnails-0.2/setup.py` & `pelican-youtube-thumbnails-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 
 setup(
     name="pelican-youtube-thumbnails",
     description="Pelican plugin to link to YouTube videos by their thumbnail",
-    version="0.2",
+    version="0.3.1",
     license="AGPL-3.0",
     long_description=(ROOT_DIRECTORY / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     author="FriedrichFröbel",
     url="https://github.com/FriedrichFroebel/pelican-youtube-thumbnails/",
-    packages=find_packages(where=".", exclude=["tests", "tests.*"]),
+    packages=find_packages(
+        where=".",
+        include=[
+            "pelican.plugins.youtube_thumbnails",
+            "pelican.plugins.youtube_thumbnails.*",
+        ],
+    ),
     include_package_data=True,
     python_requires=">=3.7, <4",
     install_requires=[
         "beautifulsoup4",
         "lxml",
         "Pillow",
         "requests",
```

### Comparing `pelican-youtube-thumbnails-0.2/tests/test_youtube_thumbnails.py` & `pelican-youtube-thumbnails-0.3.1/tests/test_youtube_thumbnails.py`

 * *Files identical despite different names*

