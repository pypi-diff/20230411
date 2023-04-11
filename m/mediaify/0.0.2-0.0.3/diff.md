# Comparing `tmp/mediaify-0.0.2.tar.gz` & `tmp/mediaify-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-0.0.2.tar", last modified: Tue Apr 11 02:05:22 2023, max compression
+gzip compressed data, was "mediaify-0.0.3.tar", last modified: Tue Apr 11 02:15:08 2023, max compression
```

## Comparing `mediaify-0.0.2.tar` & `mediaify-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3078 2023-04-11 00:07:16.807074 mediaify-0.0.2/.gitignore
--rw-r--r--   0        0        0       74 2023-04-11 00:34:55.393480 mediaify-0.0.2/README.md
--rw-r--r--   0        0        0      384 2023-04-11 01:50:24.775819 mediaify-0.0.2/mediaify/__init__.py
--rw-r--r--   0        0        0      479 2023-04-11 01:52:01.941889 mediaify-0.0.2/mediaify/configs.py
--rw-r--r--   0        0        0       93 2023-04-11 01:50:47.536304 mediaify-0.0.2/mediaify/encoders/__init__.py
--rw-r--r--   0        0        0      462 2023-04-11 00:43:21.728006 mediaify-0.0.2/mediaify/encoders/_dimensions.py
--rw-r--r--   0        0        0     3066 2023-04-11 01:50:26.375854 mediaify-0.0.2/mediaify/encoders/animation.py
--rw-r--r--   0        0        0     1427 2023-04-11 01:51:35.797332 mediaify-0.0.2/mediaify/encoders/image.py
--rw-r--r--   0        0        0     2222 2023-04-11 00:31:12.504848 mediaify-0.0.2/mediaify/encoders/probe.py
--rw-r--r--   0        0        0     1494 2023-04-11 01:52:17.498220 mediaify-0.0.2/mediaify/presets.py
--rw-r--r--   0        0        0      505 2023-04-11 01:52:23.082339 mediaify-0.0.2/mediaify/types.py
--rw-r--r--   0        0        0     1322 2023-04-11 01:50:26.375854 mediaify-0.0.2/mediaify/utils.py
--rw-r--r--   0        0        0      722 2023-04-11 02:05:21.454885 mediaify-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 01:00:14.570967 mediaify-0.0.2/test/__init__.py
--rw-r--r--   0        0        0     1761 2023-04-11 01:00:14.690970 mediaify-0.0.2/test/_test_video.py
--rw-r--r--   0        0        0    84144 2023-04-11 01:04:42.829067 mediaify-0.0.2/test/data/animation/SingleFrame.gif
--rw-r--r--   0        0        0  1056303 2023-04-11 01:04:42.833067 mediaify-0.0.2/test/data/animation/fractal.gif
--rw-r--r--   0        0        0   400305 2023-04-11 01:04:42.837067 mediaify-0.0.2/test/data/animation/ricardo.gif
--rw-r--r--   0        0        0   106970 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Complex.webp
--rw-r--r--   0        0        0   284256 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Landscape.webp
--rw-r--r--   0        0        0     4574 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Massive.webp
--rw-r--r--   0        0        0      732 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Small.webp
--rw-r--r--   0        0        0   988699 2023-04-11 01:04:42.845068 mediaify-0.0.2/test/data/video/Fire.webm
--rw-r--r--   0        0        0  3357969 2023-04-11 01:04:42.857068 mediaify-0.0.2/test/data/video/Heavy.mp4
--rw-r--r--   0        0        0     3940 2023-04-11 01:00:41.047578 mediaify-0.0.2/test/test_animation.py
--rw-r--r--   0        0        0     1817 2023-04-11 01:00:14.630969 mediaify-0.0.2/test/test_generate_media.py
--rw-r--r--   0        0        0     4395 2023-04-11 02:03:56.449081 mediaify-0.0.2/test/test_image.py
--rw-r--r--   0        0        0     1824 2023-04-11 02:03:06.628025 mediaify-0.0.2/test/testdata.py
--rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 mediaify-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-11 00:07:16.807074 mediaify-0.0.3/.gitignore
+-rw-r--r--   0        0        0      705 2023-04-11 02:14:22.462385 mediaify-0.0.3/README.md
+-rw-r--r--   0        0        0      384 2023-04-11 01:50:24.775819 mediaify-0.0.3/mediaify/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-11 01:52:01.941889 mediaify-0.0.3/mediaify/configs.py
+-rw-r--r--   0        0        0       93 2023-04-11 01:50:47.536304 mediaify-0.0.3/mediaify/encoders/__init__.py
+-rw-r--r--   0        0        0      462 2023-04-11 00:43:21.728006 mediaify-0.0.3/mediaify/encoders/_dimensions.py
+-rw-r--r--   0        0        0     3066 2023-04-11 01:50:26.375854 mediaify-0.0.3/mediaify/encoders/animation.py
+-rw-r--r--   0        0        0     1427 2023-04-11 01:51:35.797332 mediaify-0.0.3/mediaify/encoders/image.py
+-rw-r--r--   0        0        0     2222 2023-04-11 00:31:12.504848 mediaify-0.0.3/mediaify/encoders/probe.py
+-rw-r--r--   0        0        0     1494 2023-04-11 01:52:17.498220 mediaify-0.0.3/mediaify/presets.py
+-rw-r--r--   0        0        0      541 2023-04-11 02:11:42.174975 mediaify-0.0.3/mediaify/types.py
+-rw-r--r--   0        0        0     1322 2023-04-11 01:50:26.375854 mediaify-0.0.3/mediaify/utils.py
+-rw-r--r--   0        0        0      722 2023-04-11 02:14:32.746603 mediaify-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 01:00:14.570967 mediaify-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0     1761 2023-04-11 01:00:14.690970 mediaify-0.0.3/test/_test_video.py
+-rw-r--r--   0        0        0    84144 2023-04-11 01:04:42.829067 mediaify-0.0.3/test/data/animation/SingleFrame.gif
+-rw-r--r--   0        0        0  1056303 2023-04-11 01:04:42.833067 mediaify-0.0.3/test/data/animation/fractal.gif
+-rw-r--r--   0        0        0   400305 2023-04-11 01:04:42.837067 mediaify-0.0.3/test/data/animation/ricardo.gif
+-rw-r--r--   0        0        0   106970 2023-04-11 01:04:42.841068 mediaify-0.0.3/test/data/image/Complex.webp
+-rw-r--r--   0        0        0   284256 2023-04-11 01:04:42.841068 mediaify-0.0.3/test/data/image/Landscape.webp
+-rw-r--r--   0        0        0     4574 2023-04-11 01:04:42.841068 mediaify-0.0.3/test/data/image/Massive.webp
+-rw-r--r--   0        0        0      732 2023-04-11 01:04:42.841068 mediaify-0.0.3/test/data/image/Small.webp
+-rw-r--r--   0        0        0   988699 2023-04-11 01:04:42.845068 mediaify-0.0.3/test/data/video/Fire.webm
+-rw-r--r--   0        0        0  3357969 2023-04-11 01:04:42.857068 mediaify-0.0.3/test/data/video/Heavy.mp4
+-rw-r--r--   0        0        0     3940 2023-04-11 01:00:41.047578 mediaify-0.0.3/test/test_animation.py
+-rw-r--r--   0        0        0     1817 2023-04-11 01:00:14.630969 mediaify-0.0.3/test/test_generate_media.py
+-rw-r--r--   0        0        0     4395 2023-04-11 02:03:56.449081 mediaify-0.0.3/test/test_image.py
+-rw-r--r--   0        0        0     1824 2023-04-11 02:03:06.628025 mediaify-0.0.3/test/testdata.py
+-rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 mediaify-0.0.3/PKG-INFO
```

### Comparing `mediaify-0.0.2/.gitignore` & `mediaify-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/mediaify/encoders/animation.py` & `mediaify-0.0.3/mediaify/encoders/animation.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/mediaify/encoders/image.py` & `mediaify-0.0.3/mediaify/encoders/image.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/mediaify/encoders/probe.py` & `mediaify-0.0.3/mediaify/encoders/probe.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/mediaify/presets.py` & `mediaify-0.0.3/mediaify/presets.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/mediaify/utils.py` & `mediaify-0.0.3/mediaify/utils.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/pyproject.toml` & `mediaify-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "mediaify"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 description = "Encoding media into multiple qualities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mediaify-0.0.2/test/_test_video.py` & `mediaify-0.0.3/test/_test_video.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/animation/SingleFrame.gif` & `mediaify-0.0.3/test/data/animation/SingleFrame.gif`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/animation/fractal.gif` & `mediaify-0.0.3/test/data/animation/fractal.gif`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/animation/ricardo.gif` & `mediaify-0.0.3/test/data/animation/ricardo.gif`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/image/Complex.webp` & `mediaify-0.0.3/test/data/image/Complex.webp`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/image/Landscape.webp` & `mediaify-0.0.3/test/data/image/Landscape.webp`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/image/Massive.webp` & `mediaify-0.0.3/test/data/image/Massive.webp`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/image/Small.webp` & `mediaify-0.0.3/test/data/image/Small.webp`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/video/Fire.webm` & `mediaify-0.0.3/test/data/video/Fire.webm`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/data/video/Heavy.mp4` & `mediaify-0.0.3/test/data/video/Heavy.mp4`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/test_animation.py` & `mediaify-0.0.3/test/test_animation.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/test_generate_media.py` & `mediaify-0.0.3/test/test_generate_media.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/test_image.py` & `mediaify-0.0.3/test/test_image.py`

 * *Files identical despite different names*

### Comparing `mediaify-0.0.2/test/testdata.py` & `mediaify-0.0.3/test/testdata.py`

 * *Files identical despite different names*
