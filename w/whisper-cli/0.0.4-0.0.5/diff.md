# Comparing `tmp/whisper_cli-0.0.4.tar.gz` & `tmp/whisper_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_cli-0.0.4.tar", max compression
+gzip compressed data, was "whisper_cli-0.0.5.tar", max compression
```

## Comparing `whisper_cli-0.0.4.tar` & `whisper_cli-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-03-04 03:02:03.779572 whisper_cli-0.0.4/LICENSE
--rw-r--r--   0        0        0     1234 2023-03-07 03:22:50.880332 whisper_cli-0.0.4/README.md
--rw-r--r--   0        0        0      553 2023-03-07 03:35:49.234753 whisper_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 03:07:26.773869 whisper_cli-0.0.4/whisper_cli/__init__.py
--rw-r--r--   0        0        0     1852 2023-03-07 03:31:42.449631 whisper_cli-0.0.4/whisper_cli/env.py
--rw-r--r--   0        0        0     2798 2023-03-07 03:35:12.299059 whisper_cli-0.0.4/whisper_cli/main.py
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 whisper_cli-0.0.4/setup.py
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 whisper_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-04 03:02:03.779572 whisper_cli-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1234 2023-03-07 03:22:50.880332 whisper_cli-0.0.5/README.md
+-rw-r--r--   0        0        0      553 2023-04-11 06:17:48.032674 whisper_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 03:07:26.773869 whisper_cli-0.0.5/whisper_cli/__init__.py
+-rw-r--r--   0        0        0     1852 2023-03-07 03:31:42.449631 whisper_cli-0.0.5/whisper_cli/env.py
+-rw-r--r--   0        0        0     2847 2023-04-11 06:17:24.204414 whisper_cli-0.0.5/whisper_cli/main.py
+-rw-r--r--   0        0        0     1441 2023-04-11 06:17:22.142473 whisper_cli-0.0.5/whisper_cli/utils.py
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 whisper_cli-0.0.5/setup.py
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 whisper_cli-0.0.5/PKG-INFO
```

### Comparing `whisper_cli-0.0.4/LICENSE` & `whisper_cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cli-0.0.4/README.md` & `whisper_cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cli-0.0.4/pyproject.toml` & `whisper_cli-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whisper-cli"
-version = "0.0.4"
+version = "0.0.5"
 description = "A command-line interface for transcribing and translating audio using OpenAI's Whisper API"
 authors = ["Vatsal <vatsalaggarwal@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "whisper_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `whisper_cli-0.0.4/whisper_cli/env.py` & `whisper_cli-0.0.5/whisper_cli/env.py`

 * *Files identical despite different names*

### Comparing `whisper_cli-0.0.4/whisper_cli/main.py` & `whisper_cli-0.0.5/whisper_cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import openai
+from typing import Optional
 import typer
 from rich import print
 
 import whisper_cli.env as env
 from whisper_cli.env import _read_user_config
 
 app = typer.Typer(no_args_is_help=True)
@@ -11,15 +12,15 @@
 
 
 def get_file_type(file_name: str) -> str:
     """Returns the file type of the file_name."""
     return file_name.split(".")[-1]
 
 
-def _check_response_format(response_format: str | None):
+def _check_response_format(response_format: Optional[str]):
     if response_format is None:
         return None
     elif response_format in ["json", "srt", "verbose_json", "vtt"]:
         return response_format
     else:
         raise ValueError("Response format not supported by OpenAI.")
 
@@ -49,33 +50,33 @@
             return value["api_key"]
 
     raise ValueError(
         "No active environment found. Activate one using `whisper activate-env`."
     )
 
 
-def show_result(result, response_format: str | None):
+def show_result(result, response_format: Optional[str]):
     """Show result."""
     if response_format is None:
         response_format = "json"
 
     if response_format == "json":
         print(result["text"])
     else:
         print(result)
 
 
 @app.command()
 def transcribe(
     file_name: str,
     model: str = "whisper-1",
-    prompt: str | None = None,
-    response_format: str | None = None,
+    prompt: Optional[str] = None,
+    response_format: Optional[str] = None,
     temperature: float = 0,
-    language: str | None = None,
+    language: Optional[str] = None,
 ):
     """Transcribe audio file using whisper."""
     openai.api_key = get_api_key()
 
     transcript = openai.Audio.transcribe(
         model,
         get_file_content(file_name),
@@ -89,16 +90,16 @@
     show_result(transcript, response_format)
 
 
 @app.command()
 def translate(
     file_name: str,
     model: str = "whisper-1",
-    prompt: str | None = None,
-    response_format: str | None = None,
+    prompt: Optional[str] = None,
+    response_format: Optional[str] = None,
     temperature: float = 0,
 ):
     """Translate audio file using whisper."""
     openai.api_key = get_api_key()
 
     translation = openai.Audio.translate(
         model,
```

### Comparing `whisper_cli-0.0.4/setup.py` & `whisper_cli-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['openai>=0.27.0,<0.28.0', 'toml>=0.10.2,<0.11.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['whisper = whisper_cli.main:app']}
 
 setup_kwargs = {
     'name': 'whisper-cli',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': "A command-line interface for transcribing and translating audio using OpenAI's Whisper API",
     'long_description': "# Whisper CLI\nWhisper CLI is a command-line interface for transcribing and translating audio using OpenAI's Whisper API. It also allows you to manage multiple OpenAI API keys as separate environments.\n\nTo install Whisper CLI, simply run:\n\n```sh\npip install whisper-cli\n```\n\n## Setup\nTo get started with Whisper CLI, you'll need to set your OpenAI API key. You can do this using the following command:\n\n```sh\nwhisper key set <openai_api_key>\n```\n\nThis will set the API key for the default environment. If you want to use a different API key, you can set up an alternative environment by running:\n\n```sh\nwhisper key set <openai_api_key> --env <env_name>\n```\n\nTo activate an alternative environment, run:\n\n```sh\nwhisper env activate <env_name>\n```\n\n## Usage\n\nWhisper CLI supports two main functionalities: translation and transcription.\n\n### Translation\nTo translate an audio file, simply run:\n\n```sh\nwhisper translate <file_name>\n```\n\n### Transcription\nTo transcribe an audio file, run:\n\n```sh\nwhisper transcribe <file_name>\n```\n\n## Development\nIf you'd like to contribute to Whisper CLI, you'll need to set up a development environment with Python 3.10.9.\n\n```sh\npython=3.10.9\n```\n\nHappy transcribing and translating with Whisper CLI.\n",
     'author': 'Vatsal',
     'author_email': 'vatsalaggarwal@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `whisper_cli-0.0.4/PKG-INFO` & `whisper_cli-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command-line interface for transcribing and translating audio using OpenAI's Whisper API
 License: MIT
 Author: Vatsal
 Author-email: vatsalaggarwal@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

