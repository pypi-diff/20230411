# Comparing `tmp/whisper_dictation-0.4.2.tar.gz` & `tmp/whisper_dictation-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_dictation-0.4.2.tar", max compression
+gzip compressed data, was "whisper_dictation-0.4.3.tar", max compression
```

## Comparing `whisper_dictation-0.4.2.tar` & `whisper_dictation-0.4.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-11 13:54:02.592960 whisper_dictation-0.4.2/LICENSE
--rw-r--r--   0        0        0     2178 2023-04-11 14:14:05.566619 whisper_dictation-0.4.2/README.md
--rw-r--r--   0        0        0      458 2023-04-11 14:43:05.548588 whisper_dictation-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.4.2/whisper_dictation/Client.py
--rw-r--r--   0        0        0     3842 2023-04-11 13:08:13.643532 whisper_dictation-0.4.2/whisper_dictation/DictationDeamon.py
--rw-r--r--   0        0        0     3819 2023-04-11 14:38:41.641877 whisper_dictation-0.4.2/whisper_dictation/WhisperDictator.py
--rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.4.2/whisper_dictation/__init__.py
--rw-r--r--   0        0        0     1398 2023-04-11 13:47:51.649171 whisper_dictation-0.4.2/whisper_dictation/cli.py
--rw-r--r--   0        0        0  2076716 2023-04-11 14:40:14.691401 whisper_dictation-0.4.2/whisper_dictation/output.wav
--rw-r--r--   0        0        0      191 2023-04-11 14:05:52.516538 whisper_dictation-0.4.2/whisper_dictation/whisper_dictation.service
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 whisper_dictation-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 13:54:02.592960 whisper_dictation-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2178 2023-04-11 14:14:05.566619 whisper_dictation-0.4.3/README.md
+-rw-r--r--   0        0        0      458 2023-04-11 22:00:59.421220 whisper_dictation-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.4.3/whisper_dictation/Client.py
+-rw-r--r--   0        0        0     3842 2023-04-11 13:08:13.643532 whisper_dictation-0.4.3/whisper_dictation/DictationDeamon.py
+-rw-r--r--   0        0        0     4127 2023-04-11 21:59:57.727377 whisper_dictation-0.4.3/whisper_dictation/WhisperDictator.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.4.3/whisper_dictation/__init__.py
+-rw-r--r--   0        0        0     1398 2023-04-11 13:47:51.649171 whisper_dictation-0.4.3/whisper_dictation/cli.py
+-rw-r--r--   0        0        0      191 2023-04-11 14:05:52.516538 whisper_dictation-0.4.3/whisper_dictation/whisper_dictation.service
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 whisper_dictation-0.4.3/PKG-INFO
```

### Comparing `whisper_dictation-0.4.2/LICENSE` & `whisper_dictation-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.4.2/README.md` & `whisper_dictation-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.4.2/whisper_dictation/Client.py` & `whisper_dictation-0.4.3/whisper_dictation/Client.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.4.2/whisper_dictation/DictationDeamon.py` & `whisper_dictation-0.4.3/whisper_dictation/DictationDeamon.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.4.2/whisper_dictation/WhisperDictator.py` & `whisper_dictation-0.4.3/whisper_dictation/WhisperDictator.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,33 +60,40 @@
 
     def __init__(
         self,
         transcriber,
         save_audio: bool = False,
     ) -> None:
         self.recording = False
-
+        self.stop_event = threading.Event()
         self.transcriber = transcriber
-
         self.save_audio = save_audio
 
     # the start function implement the function to start recording
     def start(self, language: str = None) -> None:
-        # start a new thread to record the audio
-
-        # setup a timer, if the recording is not stopped after 300 seconds, stop it
-        timer = threading.Timer(300, self.stop)
-        timer.start()
+        # Clear the stop event
+        self.stop_event.clear()
 
+        # start a new thread to record the audio
         thread = threading.Thread(target=self._record, args=(language, ))
         thread.start()
 
+        # Set a time limit for the recording
+        stop_thread = threading.Thread(target=self._stop_timer, args=(300,))
+        stop_thread.start()
+
     # the stop function implement the function to stop recording
     def stop(self) -> None:
         self.recording = False
+        self.stop_event.set()
+
+    # The _stop_timer function will stop recording after the specified duration
+    def _stop_timer(self, duration):
+        self.stop_event.wait(duration)
+        self.stop()
 
     # the record function implement the function to record
     def _record(self, language: str) -> None:
 
         self.recording = True
         # audio parameters
         chunk = 1024
```

### Comparing `whisper_dictation-0.4.2/whisper_dictation/cli.py` & `whisper_dictation-0.4.3/whisper_dictation/cli.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.4.2/PKG-INFO` & `whisper_dictation-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-dictation
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Author: Lumen Young
 Author-email: lumen.young@lumeny.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

