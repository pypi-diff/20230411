# Comparing `tmp/jarvis-toolkit-0.0.3.tar.gz` & `tmp/jarvis-toolkit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis-toolkit-0.0.3.tar", last modified: Tue Apr 11 00:40:51 2023, max compression
+gzip compressed data, was "jarvis-toolkit-0.0.4.tar", last modified: Tue Apr 11 01:23:52 2023, max compression
```

## Comparing `jarvis-toolkit-0.0.3.tar` & `jarvis-toolkit-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.339412 jarvis-toolkit-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-10 23:17:32.000000 jarvis-toolkit-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      534 2023-04-11 00:40:51.338412 jarvis-toolkit-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-04-10 23:23:41.000000 jarvis-toolkit-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.311097 jarvis-toolkit-0.0.3/jarvis/
--rw-rw-rw-   0        0        0        0 2023-03-18 15:29:16.000000 jarvis-toolkit-0.0.3/jarvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.314641 jarvis-toolkit-0.0.3/jarvis/config/
--rw-rw-rw-   0        0        0       56 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.3/jarvis/config/__init__.py
--rw-rw-rw-   0        0        0      813 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.3/jarvis/config/openai.py
--rw-rw-rw-   0        0        0      519 2023-03-26 09:13:29.000000 jarvis-toolkit-0.0.3/jarvis/config/silero.py
--rw-rw-rw-   0        0        0      322 2023-03-18 23:09:28.000000 jarvis-toolkit-0.0.3/jarvis/config/sound.py
--rw-rw-rw-   0        0        0      528 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.3/jarvis/config/vosk.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.317665 jarvis-toolkit-0.0.3/jarvis/gpt/
--rw-rw-rw-   0        0        0     7540 2023-03-19 13:42:09.000000 jarvis-toolkit-0.0.3/jarvis/gpt/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-03-19 13:18:28.000000 jarvis-toolkit-0.0.3/jarvis/gpt/context.py
--rw-rw-rw-   0        0        0     1660 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.3/jarvis/gpt/primitives.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.318721 jarvis-toolkit-0.0.3/jarvis/silero/
--rw-rw-rw-   0        0        0      891 2023-03-26 21:15:36.000000 jarvis-toolkit-0.0.3/jarvis/silero/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.318721 jarvis-toolkit-0.0.3/jarvis/vosk_/
--rw-rw-rw-   0        0        0     2518 2023-03-26 21:14:09.000000 jarvis-toolkit-0.0.3/jarvis/vosk_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.320661 jarvis-toolkit-0.0.3/jarvis/whisper/
--rw-rw-rw-   0        0        0      901 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.3/jarvis/whisper/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-04-10 22:59:37.000000 jarvis-toolkit-0.0.3/jarvis/whisper/inputs.py
--rw-rw-rw-   0        0        0      609 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.3/jarvis/whisper/outputs.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:40:51.337411 jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/
--rw-rw-rw-   0        0        0      534 2023-04-11 00:40:51.000000 jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-04-11 00:40:51.000000 jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 00:40:51.000000 jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-04-11 00:40:51.000000 jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 00:40:51.000000 jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2023-04-11 00:40:07.000000 jarvis-toolkit-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 00:40:51.339412 jarvis-toolkit-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.072670 jarvis-toolkit-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-10 23:17:32.000000 jarvis-toolkit-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-04-11 01:23:52.071488 jarvis-toolkit-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-04-10 23:23:41.000000 jarvis-toolkit-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.044741 jarvis-toolkit-0.0.4/jarvis/
+-rw-rw-rw-   0        0        0        0 2023-03-18 15:29:16.000000 jarvis-toolkit-0.0.4/jarvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.049792 jarvis-toolkit-0.0.4/jarvis/config/
+-rw-rw-rw-   0        0        0       56 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.4/jarvis/config/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.4/jarvis/config/openai.py
+-rw-rw-rw-   0        0        0      519 2023-03-26 09:13:29.000000 jarvis-toolkit-0.0.4/jarvis/config/silero.py
+-rw-rw-rw-   0        0        0      322 2023-03-18 23:09:28.000000 jarvis-toolkit-0.0.4/jarvis/config/sound.py
+-rw-rw-rw-   0        0        0      528 2023-04-10 23:55:45.000000 jarvis-toolkit-0.0.4/jarvis/config/vosk.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.052062 jarvis-toolkit-0.0.4/jarvis/gpt/
+-rw-rw-rw-   0        0        0     7540 2023-03-19 13:42:09.000000 jarvis-toolkit-0.0.4/jarvis/gpt/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-03-19 13:18:28.000000 jarvis-toolkit-0.0.4/jarvis/gpt/context.py
+-rw-rw-rw-   0        0        0     1660 2023-03-12 12:42:11.000000 jarvis-toolkit-0.0.4/jarvis/gpt/primitives.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.052062 jarvis-toolkit-0.0.4/jarvis/silero/
+-rw-rw-rw-   0        0        0      891 2023-03-26 21:15:36.000000 jarvis-toolkit-0.0.4/jarvis/silero/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.053423 jarvis-toolkit-0.0.4/jarvis/vosk_/
+-rw-rw-rw-   0        0        0     2518 2023-03-26 21:14:09.000000 jarvis-toolkit-0.0.4/jarvis/vosk_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.055175 jarvis-toolkit-0.0.4/jarvis/whisper/
+-rw-rw-rw-   0        0        0      901 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.4/jarvis/whisper/__init__.py
+-rw-rw-rw-   0        0        0     2532 2023-04-11 01:23:05.000000 jarvis-toolkit-0.0.4/jarvis/whisper/inputs.py
+-rw-rw-rw-   0        0        0      609 2023-03-19 13:20:04.000000 jarvis-toolkit-0.0.4/jarvis/whisper/outputs.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:23:52.070525 jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-04-11 01:23:52.000000 jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-04-11 01:23:52.000000 jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 01:23:52.000000 jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-04-11 01:23:52.000000 jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 01:23:52.000000 jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2023-04-11 01:23:28.000000 jarvis-toolkit-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 01:23:52.072670 jarvis-toolkit-0.0.4/setup.cfg
```

### Comparing `jarvis-toolkit-0.0.3/LICENSE` & `jarvis-toolkit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/PKG-INFO` & `jarvis-toolkit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-toolkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Jarvis Toolkit
 Author-email: Artur Aliiev <pastordev@jarvis-toolkit.com>
 Project-URL: Homepage, https://bitbucket.org/jarvis-toolkit/jarvis-core/src/master/t
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `jarvis-toolkit-0.0.3/jarvis/config/openai.py` & `jarvis-toolkit-0.0.4/jarvis/config/openai.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/config/silero.py` & `jarvis-toolkit-0.0.4/jarvis/config/silero.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/config/vosk.py` & `jarvis-toolkit-0.0.4/jarvis/config/vosk.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/gpt/__init__.py` & `jarvis-toolkit-0.0.4/jarvis/gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/gpt/context.py` & `jarvis-toolkit-0.0.4/jarvis/gpt/context.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/gpt/primitives.py` & `jarvis-toolkit-0.0.4/jarvis/gpt/primitives.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/silero/__init__.py` & `jarvis-toolkit-0.0.4/jarvis/silero/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/vosk_/__init__.py` & `jarvis-toolkit-0.0.4/jarvis/vosk_/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/whisper/__init__.py` & `jarvis-toolkit-0.0.4/jarvis/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis/whisper/inputs.py` & `jarvis-toolkit-0.0.4/jarvis/whisper/inputs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import speech_recognition as sr
 
-
 from dataclasses import dataclass
 from io import BytesIO
 from pathlib import Path
 from typing import Literal, BinaryIO, Generator
 from pydub import AudioSegment
 
 from jarvis.config.sound import SOUND
@@ -32,36 +31,43 @@
     tmp_file_path: Path = Path('./temp_file.wav')
     tmp_file_format: Literal['mp3', 'wav', 'm4a'] = 'wav'
     stop_listen: bool = False
     recognizer = sr.Recognizer()
     recognizer.energy_threshold = SOUND.energy_threshold
     recognizer.pause_threshold = 1
 
-    def read(self, audio_data: sr.AudioData | BytesIO) -> FileInput:
+    @staticmethod
+    def raw_read(audio_data: sr.AudioData | BytesIO) -> BytesIO:
         if isinstance(audio_data, sr.AudioData):
-            audio_clip = AudioSegment.from_file(BytesIO(audio_data.get_wav_data()), format=self.tmp_file_format)
-        elif isinstance(audio_data, BytesIO):
-            audio_clip = AudioSegment.from_file(audio_data, format=self.tmp_file_format)
-        else:
-            raise ValueError
+            return audio_data.get_raw_data()
+        return audio_data
+
+    def read(self, audio_data: sr.AudioData | BytesIO) -> FileInput:
+        audio_clip = AudioSegment.from_file(BytesIO(audio_data.get_wav_data()), format=self.tmp_file_format)
         audio_clip.export(self.tmp_file_path, format=self.tmp_file_format)
         return FileInput(path=self.tmp_file_path, format=self.tmp_file_format)
 
-    def read_from_stream(self) -> Generator[FileInput, None, None]:
+    def read_from_stream(self, raw: bool = False) -> Generator[FileInput | BytesIO, None, None]:
         with sr.Microphone(
                 device_index=SOUND.device_index,
                 sample_rate=SOUND.sample_rate
         ) as source:
             self.recognizer.adjust_for_ambient_noise(source, 1)
             while 1:
-                yield self.read(self.recognizer.listen(source))
+                if raw:
+                    yield self.raw_read(self.recognizer.listen(source))
+                else:
+                    yield self.read(self.recognizer.listen(source))
                 if self.stop_listen:
                     break
 
-    def record_from_stream(self, duration: int) -> FileInput:
+    def record_from_stream(self, duration: int, raw: bool = False) -> FileInput | BytesIO:
 
         with sr.Microphone(
                 device_index=SOUND.device_index,
                 sample_rate=SOUND.sample_rate
         ) as source:
             self.recognizer.adjust_for_ambient_noise(source, 1)
-            return self.read(self.recognizer.record(source=source, duration=duration))
+            if raw:
+                return self.raw_read(self.recognizer.record(source=source, duration=duration))
+            else:
+                return self.read(self.recognizer.listen(source))
```

### Comparing `jarvis-toolkit-0.0.3/jarvis/whisper/outputs.py` & `jarvis-toolkit-0.0.4/jarvis/whisper/outputs.py`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/PKG-INFO` & `jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-toolkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Jarvis Toolkit
 Author-email: Artur Aliiev <pastordev@jarvis-toolkit.com>
 Project-URL: Homepage, https://bitbucket.org/jarvis-toolkit/jarvis-core/src/master/t
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `jarvis-toolkit-0.0.3/jarvis_toolkit.egg-info/SOURCES.txt` & `jarvis-toolkit-0.0.4/jarvis_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jarvis-toolkit-0.0.3/pyproject.toml` & `jarvis-toolkit-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools==65.5.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jarvis-toolkit"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Artur Aliiev", email = "pastordev@jarvis-toolkit.com" },
 ]
 description = "Jarvis Toolkit"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

