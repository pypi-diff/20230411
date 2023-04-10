# Comparing `tmp/turbo_docs-0.4.1.tar.gz` & `tmp/turbo_docs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.4.1.tar", last modified: Sun Apr  9 23:42:11 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.5.0.tar", last modified: Mon Apr 10 22:55:37 2023, max compression
```

## Comparing `turbo_docs-0.4.1.tar` & `turbo_docs-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 23:42:11.891680 turbo_docs-0.4.1/
--rw-rw-rw-   0        0        0      452 2023-04-09 23:42:11.890682 turbo_docs-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-04-09 16:47:21.000000 turbo_docs-0.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 23:42:11.893701 turbo_docs-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-04-09 23:41:42.000000 turbo_docs-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 23:42:11.867178 turbo_docs-0.4.1/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-09 17:13:17.000000 turbo_docs-0.4.1/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-04-09 23:41:24.000000 turbo_docs-0.4.1/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-09 23:42:11.887681 turbo_docs-0.4.1/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-09 17:33:26.000000 turbo_docs-0.4.1/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      487 2023-04-09 16:37:59.000000 turbo_docs-0.4.1/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2155 2023-04-09 16:35:50.000000 turbo_docs-0.4.1/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      686 2023-04-09 16:35:50.000000 turbo_docs-0.4.1/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-09 23:42:11.879429 turbo_docs-0.4.1/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0      452 2023-04-09 23:42:11.000000 turbo_docs-0.4.1/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-09 23:42:11.000000 turbo_docs-0.4.1/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 23:42:11.000000 turbo_docs-0.4.1/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-09 23:42:11.000000 turbo_docs-0.4.1/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-09 23:42:11.000000 turbo_docs-0.4.1/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 23:42:11.000000 turbo_docs-0.4.1/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.484126 turbo_docs-0.5.0/
+-rw-rw-rw-   0        0        0      452 2023-04-10 22:55:37.482612 turbo_docs-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1611 2023-04-10 22:45:42.000000 turbo_docs-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:55:37.484126 turbo_docs-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-04-10 22:55:32.000000 turbo_docs-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.466251 turbo_docs-0.5.0/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.5.0/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     2021 2023-04-10 22:41:35.000000 turbo_docs-0.5.0/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.481607 turbo_docs-0.5.0/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.5.0/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-10 22:20:57.000000 turbo_docs-0.5.0/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1796 2023-04-10 22:44:30.000000 turbo_docs-0.5.0/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      566 2023-04-10 22:51:04.000000 turbo_docs-0.5.0/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.475614 turbo_docs-0.5.0/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.4.1/setup.py` & `turbo_docs-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="turbo_docs",
-    version="0.4.1",
+    version="0.5.0",
     packages=find_packages(),
     install_requires=[
         "requests",
         "openai",
         "click",
         "pyperclip",
     ],
```

### Comparing `turbo_docs-0.4.1/turbo_docs/utils/directory.py` & `turbo_docs-0.5.0/turbo_docs/utils/directory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,51 @@
 import json
 import os
 from pathlib import Path
-from typing import List
+from typing import List, Dict
 
 def ignored_files_init() -> List[str]:
+    """ Initialize a list of ignored files and including README.md, docs.md, etc.
     """
-    Initialize a list of ignored files and including README.md, dir_text.txt, etc.
-    :return: list, The list of ignored files.
-    """
-    ignored_files = ["README.md", "dir_text.txt"]
+    ignored_files = ["README.md", "docs.md"]
     for file in os.listdir():
         if file[0] == ".":
             ignored_files.append(file)
     return ignored_files
 
 def read_gitignore() -> List[str]:
-    """
-    Read .gitignore file and return the list of ignored files.
-    :return: list, The list of ignored files.
+    """ Read .gitignore file and return the list of ignored files.
     """
     ignore_files = ignored_files_init()
     try:
         with open(".gitignore", "r") as gitignore:
             for line in gitignore:
                 ignore_files.append(line.strip())
     except FileNotFoundError:
         raise ValueError(".gitignore file required for excluding files from documentation generation")
     return ignore_files
 
 def ignore_filepath(filepath: str, ignore_files: List[str]) -> bool:
-    """
-    Check if a filepath should be ignored based on the ignore_files list.
-    :param filepath: str, The filepath to check.
-    :param ignore_files: list, The list of ignored files.
-    :return: bool, True if the filepath should be ignored, False otherwise.
+    """ Check if a filepath should be ignored based on the ignore_files list.
     """
     for part in Path(filepath).parts:
         if part in ignore_files:
             return True
     return False
 
-def get_directory_text() -> str:
+def get_files() -> Dict:
+    """ Retrieve the content of all files in the current directory, excluding those listed in the ignore_files.
     """
-    Get the text representation of the current directory, excluding ignored files.
-    :return: str, The text representation of the directory.
-    """
-    dir_text = ""
+    files_dict = {}
     ignore_files = read_gitignore()
 
     # Iterate over files
     for root, _, files in os.walk("."):
         for file in files:
-            filepath = os.path.join(root.replace(".\\", ""), file)
+            filepath = os.path.join(root, file).replace(".\\", "")
 
             # If not in ignore, collect file text
             if not ignore_filepath(filepath, ignore_files):
                 with open(filepath, "r") as f:
                     content = f.read().replace(" " * 4, "\t")
-                dir_text += f"{filepath}:\n\n{content}\n\n"
-
-    return dir_text
+                files_dict[filepath] = content
+    return files_dict
```

### Comparing `turbo_docs-0.4.1/turbo_docs/utils/openai_api.py` & `turbo_docs-0.5.0/turbo_docs/utils/openai_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 
 openai.api_key = os.environ.get('OPENAI_API_KEY')
 if not openai.api_key:
     raise ValueError("Cannot find API key. Run the following command: export OPENAI_API_KEY=<your_api_key>")
 
 
 def gpt_completion_wrapper(prompt):
-    """
-    Send a prompt to the OpenAI GPT-3 API and receive a completion.
-    :param prompt: str, The prompt to send to the API.
-    :return: dict, The choice object containing the generated text.
+    """ Send a prompt to the OpenAI GPT-3 API and receive a completion.
     """
     completions = openai.Completion.create(
         engine="text-davinci-003",
         prompt=prompt,
         max_tokens=2048,
         n=1,
         stop=None,
     )
-    return completions.choices[0]
+    return completions.choices[0]['text']
+
```

