# Comparing `tmp/mediaify-0.0.1.tar.gz` & `tmp/mediaify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-0.0.1.tar", last modified: Mon Apr 10 23:43:44 2023, max compression
+gzip compressed data, was "mediaify-0.0.2.tar", last modified: Tue Apr 11 02:05:22 2023, max compression
```

## Comparing `mediaify-0.0.1.tar` & `mediaify-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,29 @@
--rw-r--r--   0        0        0        0 2023-04-10 23:36:36.026051 mediaify-0.0.1/README.md
--rw-r--r--   0        0        0      451 2023-04-10 23:37:38.235333 mediaify-0.0.1/mediaify/__init__.py
--rw-r--r--   0        0        0      515 2023-04-10 23:37:38.247334 mediaify-0.0.1/mediaify/_types.py
--rw-r--r--   0        0        0     3011 2023-04-10 23:37:38.247334 mediaify-0.0.1/mediaify/animation.py
--rw-r--r--   0        0        0      880 2023-04-10 23:37:38.251334 mediaify-0.0.1/mediaify/encoder.py
--rw-r--r--   0        0        0     3124 2023-04-10 23:38:51.608850 mediaify-0.0.1/mediaify/image.py
--rw-r--r--   0        0        0     2306 2023-04-10 23:37:38.251334 mediaify-0.0.1/mediaify/probe.py
--rw-r--r--   0        0        0     1322 2023-04-10 23:37:38.251334 mediaify-0.0.1/mediaify/utils.py
--rw-r--r--   0        0        0     2701 2023-04-10 23:37:38.251334 mediaify-0.0.1/mediaify/video.py
--rw-r--r--   0        0        0      617 2023-04-10 23:42:16.381106 mediaify-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 mediaify-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-11 00:07:16.807074 mediaify-0.0.2/.gitignore
+-rw-r--r--   0        0        0       74 2023-04-11 00:34:55.393480 mediaify-0.0.2/README.md
+-rw-r--r--   0        0        0      384 2023-04-11 01:50:24.775819 mediaify-0.0.2/mediaify/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-11 01:52:01.941889 mediaify-0.0.2/mediaify/configs.py
+-rw-r--r--   0        0        0       93 2023-04-11 01:50:47.536304 mediaify-0.0.2/mediaify/encoders/__init__.py
+-rw-r--r--   0        0        0      462 2023-04-11 00:43:21.728006 mediaify-0.0.2/mediaify/encoders/_dimensions.py
+-rw-r--r--   0        0        0     3066 2023-04-11 01:50:26.375854 mediaify-0.0.2/mediaify/encoders/animation.py
+-rw-r--r--   0        0        0     1427 2023-04-11 01:51:35.797332 mediaify-0.0.2/mediaify/encoders/image.py
+-rw-r--r--   0        0        0     2222 2023-04-11 00:31:12.504848 mediaify-0.0.2/mediaify/encoders/probe.py
+-rw-r--r--   0        0        0     1494 2023-04-11 01:52:17.498220 mediaify-0.0.2/mediaify/presets.py
+-rw-r--r--   0        0        0      505 2023-04-11 01:52:23.082339 mediaify-0.0.2/mediaify/types.py
+-rw-r--r--   0        0        0     1322 2023-04-11 01:50:26.375854 mediaify-0.0.2/mediaify/utils.py
+-rw-r--r--   0        0        0      722 2023-04-11 02:05:21.454885 mediaify-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 01:00:14.570967 mediaify-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0     1761 2023-04-11 01:00:14.690970 mediaify-0.0.2/test/_test_video.py
+-rw-r--r--   0        0        0    84144 2023-04-11 01:04:42.829067 mediaify-0.0.2/test/data/animation/SingleFrame.gif
+-rw-r--r--   0        0        0  1056303 2023-04-11 01:04:42.833067 mediaify-0.0.2/test/data/animation/fractal.gif
+-rw-r--r--   0        0        0   400305 2023-04-11 01:04:42.837067 mediaify-0.0.2/test/data/animation/ricardo.gif
+-rw-r--r--   0        0        0   106970 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Complex.webp
+-rw-r--r--   0        0        0   284256 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Landscape.webp
+-rw-r--r--   0        0        0     4574 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Massive.webp
+-rw-r--r--   0        0        0      732 2023-04-11 01:04:42.841068 mediaify-0.0.2/test/data/image/Small.webp
+-rw-r--r--   0        0        0   988699 2023-04-11 01:04:42.845068 mediaify-0.0.2/test/data/video/Fire.webm
+-rw-r--r--   0        0        0  3357969 2023-04-11 01:04:42.857068 mediaify-0.0.2/test/data/video/Heavy.mp4
+-rw-r--r--   0        0        0     3940 2023-04-11 01:00:41.047578 mediaify-0.0.2/test/test_animation.py
+-rw-r--r--   0        0        0     1817 2023-04-11 01:00:14.630969 mediaify-0.0.2/test/test_generate_media.py
+-rw-r--r--   0        0        0     4395 2023-04-11 02:03:56.449081 mediaify-0.0.2/test/test_image.py
+-rw-r--r--   0        0        0     1824 2023-04-11 02:03:06.628025 mediaify-0.0.2/test/testdata.py
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 mediaify-0.0.2/PKG-INFO
```

### Comparing `mediaify-0.0.1/mediaify/probe.py` & `mediaify-0.0.2/mediaify/encoders/probe.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from functools import cached_property
 import mimetypes
-from typing import Union
+from typing import Any, Union
 from magic import Magic
 from PIL import Image as PILImage
 import ffmpeg
 import io
 
 
 class VideoProbe:
@@ -13,64 +12,64 @@
 
     def __init__(self, filepath):
         with open(filepath, 'rb') as f:
             self.data = f.read()
         self.filepath = filepath
         self.probe_data = ffmpeg.probe(self.filepath)
 
-    @cached_property
-    def video_stream(self) -> dict:
+    @property
+    def video_stream(self) -> "dict[str, Any]":
         streams = self.probe_data['streams']
         video_streams = [x for x in streams if x['codec_type'] == 'video']
         if len(video_streams) == 1:
             return video_streams[0]
         else:
             raise Exception('No or Multiple Video Streams Found')
 
-    @cached_property
+    @property
     def height(self) -> int:
         return int(self.video_stream['height'])
 
-    @cached_property
+    @property
     def width(self) -> int:
         return int(self.video_stream['width'])
 
-    @cached_property
+    @property
     def framerate(self) -> str:
         framerate = eval(self.video_stream['r_frame_rate'])
         if framerate % 1 == 0:
             framerate = int(framerate)
 
         return str(framerate)
 
-    @cached_property
+    @property
     def mimetype(self) -> str:
         magic = Magic(mime=True)
         return magic.from_buffer(self.data)
 
-    @cached_property
+    @property
     def extention(self) -> str:
         ext = mimetypes.guess_extension(self.mimetype)
         if isinstance(ext, str):
             return ext
         else:
             raise Exception("Couldn't Guess File Extention")
 
-    @cached_property
+    @property
     def audio(self) -> bool:
         for stream in self.probe_data['streams']:
             if stream['codec_type'] == 'audio':
                 return True
         return False
 
-    @cached_property
+    @property
     def duration(self) -> float:
         return float(self.probe_data['format']['duration'])
 
-    @cached_property
+    @property
     def frame_count(self) -> Union[float, None]:
         if 'nb_frames' in self.video_stream:
             return float(self.video_stream['nb_frames'])
         else:
             return None
```

### Comparing `mediaify-0.0.1/pyproject.toml` & `mediaify-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "mediaify"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 description = "Encoding media into multiple qualities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,9 +16,12 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "ffmpeg~=1.2.0",
+    "ffmpeg-python~=0.2.0",
+    "pillow~=9.5.0",
+    "python_magic~=0.4.27",
+    "python-magic-bin; sys_platform == 'win32'",
 ]
```

### Comparing `mediaify-0.0.1/PKG-INFO` & `mediaify-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 Metadata-Version: 2.1
 Name: mediaify
-Version: 0.0.1
+Version: 0.0.2
 Summary: Encoding media into multiple qualities
 Author-email: Ben Brady <benbradybusiness@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: ffmpeg~=1.2.0
+Requires-Dist: ffmpeg-python~=0.2.0
+Requires-Dist: pillow~=9.5.0
+Requires-Dist: python_magic~=0.4.27
+Requires-Dist: python-magic-bin; sys_platform == 'win32'
 
+# Dependencies
+- ffmpeg
+- libmagic
+    - `sudo apt-get install libmagic1`
```

