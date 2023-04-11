# Comparing `tmp/whisper_dictation-0.1.0.tar.gz` & `tmp/whisper_dictation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_dictation-0.1.0.tar", max compression
+gzip compressed data, was "whisper_dictation-0.2.0.tar", max compression
```

## Comparing `whisper_dictation-0.1.0.tar` & `whisper_dictation-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      364 2023-04-11 09:54:59.345575 whisper_dictation-0.1.0/README.md
--rw-r--r--   0        0        0      430 2023-04-11 10:55:02.171519 whisper_dictation-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.1.0/whisper_dictation/Client.py
--rw-r--r--   0        0        0     4078 2023-04-11 10:48:51.651961 whisper_dictation-0.1.0/whisper_dictation/DictationDeamon.py
--rw-r--r--   0        0        0     3414 2023-04-11 10:29:26.915934 whisper_dictation-0.1.0/whisper_dictation/WhisperDictator.py
--rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.1.0/whisper_dictation/__init__.py
--rw-r--r--   0        0        0     1200 2023-04-11 10:48:30.054425 whisper_dictation-0.1.0/whisper_dictation/cli.py
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 whisper_dictation-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      364 2023-04-11 09:54:59.345575 whisper_dictation-0.2.0/README.md
+-rw-r--r--   0        0        0      458 2023-04-11 12:22:01.288428 whisper_dictation-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1340 2023-04-11 10:35:40.610344 whisper_dictation-0.2.0/whisper_dictation/Client.py
+-rw-r--r--   0        0        0     3842 2023-04-11 12:17:27.984556 whisper_dictation-0.2.0/whisper_dictation/DictationDeamon.py
+-rw-r--r--   0        0        0     3414 2023-04-11 10:29:26.915934 whisper_dictation-0.2.0/whisper_dictation/WhisperDictator.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:49:30.915277 whisper_dictation-0.2.0/whisper_dictation/__init__.py
+-rw-r--r--   0        0        0     1446 2023-04-11 12:22:54.375540 whisper_dictation-0.2.0/whisper_dictation/cli.py
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 whisper_dictation-0.2.0/PKG-INFO
```

### Comparing `whisper_dictation-0.1.0/whisper_dictation/Client.py` & `whisper_dictation-0.2.0/whisper_dictation/Client.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.1.0/whisper_dictation/DictationDeamon.py` & `whisper_dictation-0.2.0/whisper_dictation/DictationDeamon.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import argparse
 from whisper import load_model
 from whisper_dictation.WhisperDictator import WhisperDictator, Transcriber
 
 recording: bool = False
 
 
-def initializing_deamon(args: argparse.Namespace) -> WhisperDictator:
+def initializing_daemon(model_name:str) -> WhisperDictator:
 
     print("Loading Model....")
-    model_name = args.model_name
     model = load_model(model_name)
 
     transcriber = Transcriber(model)
     dictator = WhisperDictator(transcriber=transcriber, save_audio=True)
 
+    print("Load Complete!")
     return dictator
 
 
 def run_daemon(host, port, selector, dictator):
     # Initialize daemon
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.bind((host, port))
@@ -112,16 +112,9 @@
             'If using a model ending in .en, you cannot specify a language other than English.'
         )
 
     return args
 
 
 if __name__ == "__main__":
+    pass
 
-    args = parse_args()
-
-    dictator = initializing_deamon(args)
-
-    selector: selectors.DefaultSelector = selectors.DefaultSelector()
-
-    # Pass the dictator instance here
-    run_daemon('localhost', 9000, selector, dictator)
```

### Comparing `whisper_dictation-0.1.0/whisper_dictation/WhisperDictator.py` & `whisper_dictation-0.2.0/whisper_dictation/WhisperDictator.py`

 * *Files identical despite different names*

### Comparing `whisper_dictation-0.1.0/whisper_dictation/cli.py` & `whisper_dictation-0.2.0/whisper_dictation/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import click
 import socket
-from whisper_dictation.DictationDeamon import run_daemon, parse_args, initializing_deamon # Assuming these are imported from your project
+# Assuming these are imported from your project
+from whisper_dictation.DictationDeamon import run_daemon, parse_args, initializing_daemon
 from whisper_dictation.WhisperDictator import WhisperDictator
 import selectors
 
+
 @click.group()
 def cli():
     pass
 
+
 @click.command()
 @click.option('--port', default=9000, help='The port for the dictation server.')
-def daemon(host, port):
+@click.option('--model_name', default="base", type=click.Choice(['tiny', 'tiny.en', 'base', 'base.en', 'small', 'small.en', 'medium', 'medium.en', 'large']), help='The the whisper model used on the dictation server.')
+def daemon(port, model_name):
     """Start the Whisper Dictation daemon."""
 
-    args = parse_args()
-    if args.port is not port:
-        args.port = port
-    dictator = initializing_deamon(args)
+    dictator = initializing_daemon(model_name=model_name)
     selector: selectors.DefaultSelector = selectors.DefaultSelector()
     run_daemon('localhost', port, selector, dictator)
 
 @click.command()
+def hello():
+    click.echo('Hello World!')
+
+
+@click.command()
 @click.option('--port', default=9000, help='The dictation server port to connect.')
 @click.option('--language', default='en', help='Specify the language you want to use.')
-def say(host, port, language):
+def say(port, language):
     """Send a voice sample to the dictation server."""
 
     server_address = ('localhost', port)
     sock = socket.create_connection(server_address)
     sock.sendall(language.encode())
     sock.close()
 
+
 cli.add_command(daemon)
+cli.add_command(hello)
 cli.add_command(say)
 
 if __name__ == "__main__":
-    cli()
+    cli()
```

### Comparing `whisper_dictation-0.1.0/PKG-INFO` & `whisper_dictation-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: whisper-dictation
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Lumen Young
 Author-email: lumen.young@lumeny.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: openai-whisper (>=20230314,<20230315)
 Requires-Dist: pyaudio (>=0.2.13,<0.3.0)
 Description-Content-Type: text/markdown
 
 ## Whisper-dictation
 
 This is an app using openai's whisper to dictate on KDE.
```

