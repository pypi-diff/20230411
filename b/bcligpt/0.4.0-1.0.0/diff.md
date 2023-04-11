# Comparing `tmp/bcligpt-0.4.0.tar.gz` & `tmp/bcligpt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcligpt-0.4.0.tar", last modified: Fri Apr  7 15:40:26 2023, max compression
+gzip compressed data, was "bcligpt-1.0.0.tar", last modified: Tue Apr 11 12:31:42 2023, max compression
```

## Comparing `bcligpt-0.4.0.tar` & `bcligpt-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-07 15:40:26.504482 bcligpt-0.4.0/
--rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-07 15:40:26.504482 bcligpt-0.4.0/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)      133 2023-04-03 14:53:27.000000 bcligpt-0.4.0/README.md
--rw-r--r--   0 marco     (1000) marco     (1000)      374 2023-04-07 15:40:22.000000 bcligpt-0.4.0/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-04-07 15:40:26.504482 bcligpt-0.4.0/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-07 15:40:26.492482 bcligpt-0.4.0/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-07 15:40:26.504482 bcligpt-0.4.0/src/bcligpt/
--rw-r--r--   0 marco     (1000) marco     (1000)       48 2023-04-03 15:22:45.000000 bcligpt-0.4.0/src/bcligpt/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2624 2023-04-07 15:38:54.000000 bcligpt-0.4.0/src/bcligpt/app.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-07 15:40:26.504482 bcligpt-0.4.0/src/bcligpt.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-07 15:40:26.000000 bcligpt-0.4.0/src/bcligpt.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)      279 2023-04-07 15:40:26.000000 bcligpt-0.4.0/src/bcligpt.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-04-07 15:40:26.000000 bcligpt-0.4.0/src/bcligpt.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       42 2023-04-07 15:40:26.000000 bcligpt-0.4.0/src/bcligpt.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       21 2023-04-07 15:40:26.000000 bcligpt-0.4.0/src/bcligpt.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        8 2023-04-07 15:40:26.000000 bcligpt-0.4.0/src/bcligpt.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.114300 bcligpt-1.0.0/
+-rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-11 12:31:42.114300 bcligpt-1.0.0/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      133 2023-04-03 14:53:27.000000 bcligpt-1.0.0/README.md
+-rw-r--r--   0 marco     (1000) marco     (1000)      374 2023-04-11 12:31:38.000000 bcligpt-1.0.0/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-04-11 12:31:42.114300 bcligpt-1.0.0/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.106300 bcligpt-1.0.0/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.110300 bcligpt-1.0.0/src/bcligpt/
+-rw-r--r--   0 marco     (1000) marco     (1000)       48 2023-04-03 15:22:45.000000 bcligpt-1.0.0/src/bcligpt/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2953 2023-04-11 12:28:20.000000 bcligpt-1.0.0/src/bcligpt/app.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.114300 bcligpt-1.0.0/src/bcligpt.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      279 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       42 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       21 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        8 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/top_level.txt
```

### Comparing `bcligpt-0.4.0/src/bcligpt/app.py` & `bcligpt-1.0.0/src/bcligpt/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 import subprocess
 import tiktoken
 from openai.error import InvalidRequestError
 from rich.console import Console
 from rich.markdown import Markdown
 import json
 from rich.live import Live
+import readline
 
 def start():
+    # Enable arrow key editing in input()
+    readline.parse_and_bind("bind ^[[A ed-prev-line")  # Up arrow
+    readline.parse_and_bind("bind ^[[B ed-next-line")  # Down arrow
+    readline.parse_and_bind("bind ^[[C ed-next-char")  # Right arrow
+    readline.parse_and_bind("bind ^[[D ed-prev-char")  # Left arrow
     print("Loading...")
     openai.api_key = os.getenv("OPENAI_API_KEY")
     code_theme = os.getenv("BCLIGPT_CODE_THEME", "monokai")
     model = os.getenv("BCLIGPT_MODEL", "gpt-3.5-turbo")
     messages = [
             {"role": "system", "content": "Your are an helpful coding assistant. You write responses in markdown. In code blocks, always add the language of the code to enable syntax highlighting. For code blocks containing commands, always add bash as a language near the ``` mark, like this: ```bash"},
         ]
```

