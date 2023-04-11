# Comparing `tmp/whisper_dictation-0.3.0.tar.gz` & `tmp/whisper_dictation-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_dictation-0.3.0.tar", max compression
+gzip compressed data, was "whisper_dictation-0.4.0.tar", max compression
```

## Comparing `whisper_dictation-0.3.0.tar` & `whisper_dictation-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1860 2023-04-11 12:58:04.603652 whisper_dictation-0.3.0/README.md
--rw-r--r--   0        0        0      458 2023-04-11 12:58:32.254112 whisper_dictation-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.3.0/whisper_dictation/Client.py
--rw-r--r--   0        0        0     3842 2023-04-11 12:17:27.984556 whisper_dictation-0.3.0/whisper_dictation/DictationDeamon.py
--rw-r--r--   0        0        0     3588 2023-04-11 12:49:25.489404 whisper_dictation-0.3.0/whisper_dictation/WhisperDictator.py
--rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.3.0/whisper_dictation/__init__.py
--rw-r--r--   0        0        0     1446 2023-04-11 12:22:54.375540 whisper_dictation-0.3.0/whisper_dictation/cli.py
--rw-r--r--   0        0        0      176 2023-04-11 12:30:24.128343 whisper_dictation-0.3.0/whisper_dictation/whipsper_dictation.service
--rw-r--r--   0        0        0     2340 1970-01-01 00:00:00.000000 whisper_dictation-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1860 2023-04-11 12:58:04.603652 whisper_dictation-0.4.0/README.md
+-rw-r--r--   0        0        0      458 2023-04-11 13:10:11.552150 whisper_dictation-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.4.0/whisper_dictation/Client.py
+-rw-r--r--   0        0        0     3842 2023-04-11 13:08:13.643532 whisper_dictation-0.4.0/whisper_dictation/DictationDeamon.py
+-rw-r--r--   0        0        0     3667 2023-04-11 13:09:29.862993 whisper_dictation-0.4.0/whisper_dictation/WhisperDictator.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.4.0/whisper_dictation/__init__.py
+-rw-r--r--   0        0        0     1446 2023-04-11 12:22:54.375540 whisper_dictation-0.4.0/whisper_dictation/cli.py
+-rw-r--r--   0        0        0   159788 2023-04-11 13:09:09.242410 whisper_dictation-0.4.0/whisper_dictation/output.wav
+-rw-r--r--   0        0        0      176 2023-04-11 12:30:24.128343 whisper_dictation-0.4.0/whisper_dictation/whipsper_dictation.service
+-rw-r--r--   0        0        0     2340 1970-01-01 00:00:00.000000 whisper_dictation-0.4.0/PKG-INFO
```

### Comparing `whisper_dictation-0.3.0/README.md` & `whisper_dictation-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.3.0/whisper_dictation/Client.py` & `whisper_dictation-0.4.0/whisper_dictation/Client.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.3.0/whisper_dictation/DictationDeamon.py` & `whisper_dictation-0.4.0/whisper_dictation/DictationDeamon.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.3.0/whisper_dictation/WhisperDictator.py` & `whisper_dictation-0.4.0/whisper_dictation/WhisperDictator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pyaudio
 import wave
 import numpy as np
 import threading
+import shlex
 import os
 from ctypes import *
 from contextlib import contextmanager
 
 ERROR_HANDLER_FUNC = CFUNCTYPE(None, c_char_p, c_int, c_char_p, c_int,
                                c_char_p)
 
@@ -34,17 +35,18 @@
 
     def transcribe(self, audio_data: np.ndarray, language: str = "en") -> str:
         """Transcribe the audio data.
         """
         result = self.model.transcribe(
             audio_data, language=language, fp16=False)
 
-        os.system(
-            "kdialog --title 'Dictation copied' --passivepopup " + "'" +result['text'], "'")
-        
+        result_text = result['text']
+        escaped_result_text = shlex.quote(result_text)
+        os.system(f'kdialog --title "Dictation copied" --passivepopup {escaped_result_text}')
+
         # os.system(f"wl-copy '{result['text']}")
 
         # copy to wl-copy, not using f-string
         os.system("wl-copy " + result['text'])
 
         return result["text"]
```

### Comparing `whisper_dictation-0.3.0/whisper_dictation/cli.py` & `whisper_dictation-0.4.0/whisper_dictation/cli.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.3.0/PKG-INFO` & `whisper_dictation-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-dictation
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Lumen Young
 Author-email: lumen.young@lumeny.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

