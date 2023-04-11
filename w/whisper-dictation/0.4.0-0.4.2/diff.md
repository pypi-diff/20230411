# Comparing `tmp/whisper_dictation-0.4.0.tar.gz` & `tmp/whisper_dictation-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_dictation-0.4.0.tar", max compression
+gzip compressed data, was "whisper_dictation-0.4.2.tar", max compression
```

## Comparing `whisper_dictation-0.4.0.tar` & `whisper_dictation-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1860 2023-04-11 12:58:04.603652 whisper_dictation-0.4.0/README.md
--rw-r--r--   0        0        0      458 2023-04-11 13:10:11.552150 whisper_dictation-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.4.0/whisper_dictation/Client.py
--rw-r--r--   0        0        0     3842 2023-04-11 13:08:13.643532 whisper_dictation-0.4.0/whisper_dictation/DictationDeamon.py
--rw-r--r--   0        0        0     3667 2023-04-11 13:09:29.862993 whisper_dictation-0.4.0/whisper_dictation/WhisperDictator.py
--rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.4.0/whisper_dictation/__init__.py
--rw-r--r--   0        0        0     1446 2023-04-11 12:22:54.375540 whisper_dictation-0.4.0/whisper_dictation/cli.py
--rw-r--r--   0        0        0   159788 2023-04-11 13:09:09.242410 whisper_dictation-0.4.0/whisper_dictation/output.wav
--rw-r--r--   0        0        0      176 2023-04-11 12:30:24.128343 whisper_dictation-0.4.0/whisper_dictation/whipsper_dictation.service
--rw-r--r--   0        0        0     2340 1970-01-01 00:00:00.000000 whisper_dictation-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 13:54:02.592960 whisper_dictation-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2178 2023-04-11 14:14:05.566619 whisper_dictation-0.4.2/README.md
+-rw-r--r--   0        0        0      458 2023-04-11 14:43:05.548588 whisper_dictation-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.4.2/whisper_dictation/Client.py
+-rw-r--r--   0        0        0     3842 2023-04-11 13:08:13.643532 whisper_dictation-0.4.2/whisper_dictation/DictationDeamon.py
+-rw-r--r--   0        0        0     3819 2023-04-11 14:38:41.641877 whisper_dictation-0.4.2/whisper_dictation/WhisperDictator.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.4.2/whisper_dictation/__init__.py
+-rw-r--r--   0        0        0     1398 2023-04-11 13:47:51.649171 whisper_dictation-0.4.2/whisper_dictation/cli.py
+-rw-r--r--   0        0        0  2076716 2023-04-11 14:40:14.691401 whisper_dictation-0.4.2/whisper_dictation/output.wav
+-rw-r--r--   0        0        0      191 2023-04-11 14:05:52.516538 whisper_dictation-0.4.2/whisper_dictation/whisper_dictation.service
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 whisper_dictation-0.4.2/PKG-INFO
```

### Comparing `whisper_dictation-0.4.0/README.md` & `whisper_dictation-0.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 ## Whisper-dictation
 
 This is an app using openai's whisper to dictate on KDE wayland.  
 
-The project is designed as a dictation server that runs at background (To avoid the time to load model each time starts the dictation) and a client to toggle if the server should be recording. You can assign a shortcut to toggle the server to start/stop the recording (`whisper_dicatation -l [language_code]`).
+The project is designed as a dictation server that runs at background (To avoid the time to load model each time starts the dictation) and a client to toggle if the server should be recording. You can assign a shortcut to toggle the server to start/stop the recording (`whisper_dicatation --language [language_code]`).
 
 Whenever the dictation is stopped, the content will be sent to your clipboard and a notification will be displayed.
 
 The project depends on the `kdialog` [package](https://archlinux.org/packages/extra/x86_64/kdialog/) and `wl-copy` (from `wl-clipboard` [package](https://github.com/bugaevc/wl-clipboard)).
 
 This project is designed to work on KDE wayland. Other wayland platforms might work as well, but without the ability to send a notification.
 
 ## Installation
 
+Install using pip:
+
 ```
 pip install whisper_dictation
 ```
 
+Note that it is recommended to install at user directory (not globally). Since the systemd service provided is written only for executable at `~/.local/bin`
+
 ## Usage
 
-To start the project manually, you should use two terminals:
+To start the project manually, you should use two terminals, for the server:
 
 ```
 whisper_dictation daemon [--port 9000] [--model_name base]
 ```
 
-See `whisper_dictation daemon --help for all the available models`
+See `whisper_dictation daemon --help` for all the available models
 
 You can use a command to trigger the daemon, or assign a shortcut to this command in order to use it. Press once for start, and press the second time to stop the recording.
 
 ```
 whisper_dictation say [--language en]
 ```
 
 You should assign a language code, it can help with the performance especially using a small model.
 
-Alternatively, you can use the systemd service unit provided inside this repo to make the daemon running in the background. Place it in your `~/.config/systemd/user/`, enable and start it.
+Alternatively, you can use the systemd service unit provided inside this repo to make the daemon running in the background. Place it in your `~/.config/systemd/user/`, enable and start it:
+
+```
+systemctl --user enable whisper_dictation
+systemctl --user start whisper_dictation
+```
 
 ## TODO
 
 - [x] add system integration for a shortcut to start/stop dictation
 - [ ] output the dictation to where the cursor is (planned as fcitx addon).
 - [ ] optional(A system tray)
+- [ ] package it on aur
 
 
 ## Requirements
 
 1. `wl-clipboard`
 2. `kdialog`
```

### Comparing `whisper_dictation-0.4.0/whisper_dictation/Client.py` & `whisper_dictation-0.4.2/whisper_dictation/Client.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.4.0/whisper_dictation/DictationDeamon.py` & `whisper_dictation-0.4.2/whisper_dictation/DictationDeamon.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.4.0/whisper_dictation/WhisperDictator.py` & `whisper_dictation-0.4.2/whisper_dictation/WhisperDictator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pyaudio
 import wave
 import numpy as np
 import threading
 import shlex
 import os
+import subprocess
 from ctypes import *
 from contextlib import contextmanager
 
 ERROR_HANDLER_FUNC = CFUNCTYPE(None, c_char_p, c_int, c_char_p, c_int,
                                c_char_p)
 
 
@@ -37,20 +38,22 @@
         """Transcribe the audio data.
         """
         result = self.model.transcribe(
             audio_data, language=language, fp16=False)
 
         result_text = result['text']
         escaped_result_text = shlex.quote(result_text)
-        os.system(f'kdialog --title "Dictation copied" --passivepopup {escaped_result_text}')
+
+        popup_duration = 5  # specify duration in seconds, adjust this value as needed
+        subprocess.run(["kdialog", "--title", "Dictation copied", "--passivepopup", escaped_result_text, str(popup_duration)])
 
         # os.system(f"wl-copy '{result['text']}")
 
         # copy to wl-copy, not using f-string
-        os.system("wl-copy " + result['text'])
+        subprocess.run(["wl-copy", result_text], text=True)
 
         return result["text"]
 
 
 class WhisperDictator(object):
     """An audio object to record the microphone.
     """
```

### Comparing `whisper_dictation-0.4.0/whisper_dictation/cli.py` & `whisper_dictation-0.4.2/whisper_dictation/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import click
 import socket
-# Assuming these are imported from your project
 from whisper_dictation.DictationDeamon import run_daemon, parse_args, initializing_daemon
 from whisper_dictation.WhisperDictator import WhisperDictator
 import selectors
 
 
 @click.group()
 def cli():
```

### Comparing `whisper_dictation-0.4.0/PKG-INFO` & `whisper_dictation-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-dictation
-Version: 0.4.0
+Version: 0.4.2
 Summary: 
 Author: Lumen Young
 Author-email: lumen.young@lumeny.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,53 +13,63 @@
 Requires-Dist: pyaudio (>=0.2.13,<0.3.0)
 Description-Content-Type: text/markdown
 
 ## Whisper-dictation
 
 This is an app using openai's whisper to dictate on KDE wayland.  
 
-The project is designed as a dictation server that runs at background (To avoid the time to load model each time starts the dictation) and a client to toggle if the server should be recording. You can assign a shortcut to toggle the server to start/stop the recording (`whisper_dicatation -l [language_code]`).
+The project is designed as a dictation server that runs at background (To avoid the time to load model each time starts the dictation) and a client to toggle if the server should be recording. You can assign a shortcut to toggle the server to start/stop the recording (`whisper_dicatation --language [language_code]`).
 
 Whenever the dictation is stopped, the content will be sent to your clipboard and a notification will be displayed.
 
 The project depends on the `kdialog` [package](https://archlinux.org/packages/extra/x86_64/kdialog/) and `wl-copy` (from `wl-clipboard` [package](https://github.com/bugaevc/wl-clipboard)).
 
 This project is designed to work on KDE wayland. Other wayland platforms might work as well, but without the ability to send a notification.
 
 ## Installation
 
+Install using pip:
+
 ```
 pip install whisper_dictation
 ```
 
+Note that it is recommended to install at user directory (not globally). Since the systemd service provided is written only for executable at `~/.local/bin`
+
 ## Usage
 
-To start the project manually, you should use two terminals:
+To start the project manually, you should use two terminals, for the server:
 
 ```
 whisper_dictation daemon [--port 9000] [--model_name base]
 ```
 
-See `whisper_dictation daemon --help for all the available models`
+See `whisper_dictation daemon --help` for all the available models
 
 You can use a command to trigger the daemon, or assign a shortcut to this command in order to use it. Press once for start, and press the second time to stop the recording.
 
 ```
 whisper_dictation say [--language en]
 ```
 
 You should assign a language code, it can help with the performance especially using a small model.
 
-Alternatively, you can use the systemd service unit provided inside this repo to make the daemon running in the background. Place it in your `~/.config/systemd/user/`, enable and start it.
+Alternatively, you can use the systemd service unit provided inside this repo to make the daemon running in the background. Place it in your `~/.config/systemd/user/`, enable and start it:
+
+```
+systemctl --user enable whisper_dictation
+systemctl --user start whisper_dictation
+```
 
 ## TODO
 
 - [x] add system integration for a shortcut to start/stop dictation
 - [ ] output the dictation to where the cursor is (planned as fcitx addon).
 - [ ] optional(A system tray)
+- [ ] package it on aur
 
 
 ## Requirements
 
 1. `wl-clipboard`
 2. `kdialog`
```

