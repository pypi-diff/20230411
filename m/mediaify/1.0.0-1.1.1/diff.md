# Comparing `tmp/mediaify-1.0.0.tar.gz` & `tmp/mediaify-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-1.0.0.tar", last modified: Tue Apr 11 02:34:26 2023, max compression
+gzip compressed data, was "mediaify-1.1.1.tar", last modified: Tue Apr 11 13:06:53 2023, max compression
```

## Comparing `mediaify-1.0.0.tar` & `mediaify-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      755 2023-04-11 02:34:14.975582 mediaify-1.0.0/README.md
--rw-r--r--   0        0        0      384 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/__init__.py
--rw-r--r--   0        0        0      479 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/configs.py
--rw-r--r--   0        0        0       93 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/encoders/__init__.py
--rw-r--r--   0        0        0      462 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/encoders/_dimensions.py
--rw-r--r--   0        0        0     3066 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/encoders/animation.py
--rw-r--r--   0        0        0     1427 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/encoders/image.py
--rw-r--r--   0        0        0     2222 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/encoders/probe.py
--rw-r--r--   0        0        0     1494 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/presets.py
--rw-r--r--   0        0        0      971 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/types.py
--rw-r--r--   0        0        0     1322 2023-04-11 02:34:14.975582 mediaify-1.0.0/mediaify/utils.py
--rw-r--r--   0        0        0      722 2023-04-11 02:34:14.975582 mediaify-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1405 1970-01-01 00:00:00.000000 mediaify-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-04-11 13:06:43.340757 mediaify-1.1.1/LICENSE
+-rw-r--r--   0        0        0      935 2023-04-11 13:06:43.340757 mediaify-1.1.1/README.md
+-rw-r--r--   0        0        0      359 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/__init__.py
+-rw-r--r--   0        0        0      753 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/configs.py
+-rw-r--r--   0        0        0      335 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/__init__.py
+-rw-r--r--   0        0        0     4252 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/animation.py
+-rw-r--r--   0        0        0     2615 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/image.py
+-rw-r--r--   0        0        0     1954 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/probe.py
+-rw-r--r--   0        0        0      727 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/utils.py
+-rw-r--r--   0        0        0     2496 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/encoders/video.py
+-rw-r--r--   0        0        0     2342 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/presets.py
+-rw-r--r--   0        0        0     1014 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/types.py
+-rw-r--r--   0        0        0     1903 2023-04-11 13:06:43.340757 mediaify-1.1.1/mediaify/utils.py
+-rw-r--r--   0        0        0     1657 2023-04-11 13:06:43.340757 mediaify-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 mediaify-1.1.1/PKG-INFO
```

### Comparing `mediaify-1.0.0/mediaify/encoders/probe.py` & `mediaify-1.1.1/mediaify/encoders/probe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import mimetypes
 from typing import Any, Union
 from magic import Magic
-from PIL import Image as PILImage
-import ffmpeg
-import io
+import ffmpeg # type: ignore
 
 
 class VideoProbe:
     filepath: str
     data: bytes
 
-    def __init__(self, filepath):
+    def __init__(self, filepath: str):
         with open(filepath, 'rb') as f:
             self.data = f.read()
         self.filepath = filepath
         self.probe_data = ffmpeg.probe(self.filepath)
 
     @property
     def video_stream(self) -> "dict[str, Any]":
         streams = self.probe_data['streams']
         video_streams = [x for x in streams if x['codec_type'] == 'video']
         if len(video_streams) == 1:
-            return video_streams[0]
+            return video_streams[0] # type: ignore
         else:
             raise Exception('No or Multiple Video Streams Found')
 
     @property
     def height(self) -> int:
         return int(self.video_stream['height'])
 
@@ -68,17 +66,7 @@
     @property
     def frame_count(self) -> Union[float, None]:
         if 'nb_frames' in self.video_stream:
             return float(self.video_stream['nb_frames'])
         else:
             return None
 
-
-def is_animated_sequence(data: bytes) -> bool:
-    buf = io.BytesIO(data)
-    pil_img = PILImage.open(buf, formats=None)
-    return pil_img.is_animated
-
-
-def guess_mimetype(data: bytes) -> str:
-    magic = Magic(mime=True)
-    return magic.from_buffer(data)
```

### Comparing `mediaify-1.0.0/mediaify/types.py` & `mediaify-1.1.1/mediaify/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from dataclasses import dataclass
-from typing import Union
+from typing_extensions import TypeAlias
+
 
 @dataclass(repr=False)
 class ImageFile:
     data: bytes
     mimetype: str
     height: int
     width: int
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'ImageFile({self.width}x{self.height}, {self.mimetype})'
 
 
 @dataclass(repr=False)
 class AnimationFile:
     data: bytes
     mimetype: str
     height: int
     width: int
     frame_count: int
     duration: float
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'AnimationFile({self.width}x{self.height} {self.duration}ms, {self.mimetype})'
 
 
 @dataclass(repr=False)
 class VideoFile:
     data: bytes
     mimetype: str
     height: int
     width: int
     duration: float
     framerate: str
     hasAudio: bool
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'VideoFile(' \
             f"{self.width}x{self.height} {self.duration}s " \
             f"{'audio' if self.hasAudio else 'no audio'}, " \
             f"{self.mimetype})"
 
 
-GenericFile = Union[ImageFile, AnimationFile, VideoFile]
+MediaFile: TypeAlias = "ImageFile | AnimationFile | VideoFile"
```

