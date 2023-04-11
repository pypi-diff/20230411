# Comparing `tmp/echoai-dev-0.1.2.tar.gz` & `tmp/echoai-dev-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoai-dev-0.1.2.tar", last modified: Wed Mar 29 05:44:41 2023, max compression
+gzip compressed data, was "echoai-dev-0.2.0rc1.tar", last modified: Tue Apr 11 06:43:52 2023, max compression
```

## Comparing `echoai-dev-0.1.2.tar` & `echoai-dev-0.2.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:41.633410 echoai-dev-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-29 05:44:41.633410 echoai-dev-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:41.629409 echoai-dev-0.1.2/echoai/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/echoai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:41.629409 echoai-dev-0.1.2/echoai/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/echoai/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/echoai/clients/langchain_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/echoai/clients/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/echoai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:44:41.633410 echoai-dev-0.1.2/echoai_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-29 05:44:41.000000 echoai-dev-0.1.2/echoai_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-29 05:44:41.000000 echoai-dev-0.1.2/echoai_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 05:44:41.000000 echoai-dev-0.1.2/echoai_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-29 05:44:41.000000 echoai-dev-0.1.2/echoai_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-29 05:44:41.000000 echoai-dev-0.1.2/echoai_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-29 05:44:41.000000 echoai-dev-0.1.2/echoai_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 05:44:41.633410 echoai-dev-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-29 05:44:29.000000 echoai-dev-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:43:52.035560 echoai-dev-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 06:43:52.035560 echoai-dev-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:43:52.031560 echoai-dev-0.2.0rc1/echoai/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/echoai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:43:52.035560 echoai-dev-0.2.0rc1/echoai/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/echoai/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/echoai/clients/langchain_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/echoai/clients/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/echoai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:43:52.035560 echoai-dev-0.2.0rc1/echoai_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 06:43:51.000000 echoai-dev-0.2.0rc1/echoai_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 06:43:51.000000 echoai-dev-0.2.0rc1/echoai_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:43:51.000000 echoai-dev-0.2.0rc1/echoai_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:43:51.000000 echoai-dev-0.2.0rc1/echoai_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 06:43:51.000000 echoai-dev-0.2.0rc1/echoai_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 06:43:51.000000 echoai-dev-0.2.0rc1/echoai_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:43:52.035560 echoai-dev-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-11 06:43:42.000000 echoai-dev-0.2.0rc1/setup.py
```

### Comparing `echoai-dev-0.1.2/LICENSE.txt` & `echoai-dev-0.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `echoai-dev-0.1.2/PKG-INFO` & `echoai-dev-0.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoai-dev
-Version: 0.1.2
+Version: 0.2.0rc1
 Summary: The command line tool to interface with Generative AI.
 Author: Fabio Dr.No Nonato
 Author-email: echoaidev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `echoai-dev-0.1.2/README.md` & `echoai-dev-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `echoai-dev-0.1.2/echoai/clients/openai_client.py` & `echoai-dev-0.2.0rc1/echoai/clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `echoai-dev-0.1.2/echoai/main.py` & `echoai-dev-0.2.0rc1/echoai/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #!/usr/bin/env python
 import argparse
 import logging
 import os
 from pygments import highlight
-from pygments.lexers import PythonLexer, MarkdownLexer, BashLexer
-from pygments.formatters import TerminalFormatter
+from pygments.lexers import PythonLexer, MarkdownLexer, BashLexer, guess_lexer
+from pygments.formatters.terminal256 import Terminal256Formatter
 from echoai.clients.openai_client import OpenAIClient
-from echoai.clients.langchain_client import LangChainOpenAIClient
+from echoai.clients.langchain_client import OpenAILangChain
 
 def format_text(text):
     """
     Formats text with syntax highlighting and colors using the Markdown syntax and Pygments library.
 
     :param text: The text to format
     :return: The formatted text
     """
 
     # Format the text with syntax highlighting and colors
-    formatted_text = highlight(text, MarkdownLexer(), TerminalFormatter())
+    # guess = guess_lexer(text)
+    formatted_text = highlight(text, MarkdownLexer(), Terminal256Formatter())
+    # formatted_text = highlight(text, guess, Terminal256Formatter())
     return formatted_text
 
 def print_output(output):
     """
     Prints output to the console.
 
     :param output: The output to print
@@ -42,50 +44,35 @@
     # Set up logging
     log_level = os.getenv("LOG_LEVEL", "INFO")
     logging.basicConfig(level=log_level)
 
     # Define command line arguments
     parser = argparse.ArgumentParser(description="Generate code completions using OpenAI Codex.")
     parser.add_argument("prompt", help="The prompt for code completion.")
-    parser.add_argument("--nochat", help="DO NOT Use the GPT-3.5 turbo chat model instead of the Codex model.", action="store_true")
-    parser.add_argument("--chain", help="Use LangChain implementation of Clients", action="store_true")
+    parser.add_argument("--chat", help="Use chat interface", action="store_true")
+    parser.add_argument("--format", help="Use Pygments to format the terminal output", action="store_true")
 
     # Parse command line arguments
     args = parser.parse_args()
 
-    
-
-    if args.chain:
-        client = LangChainOpenAIClient(
-            key = os.getenv('OPENAI_API_KEY'),
-            engine = os.getenv('OPENAI_API_ENGINE','gpt-3.5-turbo-0301'),
-            version = os.getenv('OPENAI_API_VERSION')
-
-        )
-    else:
-        client = OpenAIClient(
-            key = os.getenv('OPENAI_API_KEY'),
-            engine = os.getenv('OPENAI_API_ENGINE','gpt-3.5-turbo-0301'),
-            version = os.getenv('OPENAI_API_VERSION')
-
-        )
-
+    client = OpenAILangChain(is_chat=args.chat)
     
     # Get response from OpenAI
-    if args.nochat:
-        logging.debug("Getting completion from OpenAI Codex for prompt: %s", args.prompt)
-        response = client.get_completion(args.prompt)
-    else:
+    if args.chat:
+        
         logging.debug("Getting chat response from OpenAI for prompt: %s", args.prompt)
         response = client.get_chat_completion(args.prompt)
-    
-
+    else:
+        logging.debug("Getting completion from OpenAI Codex for prompt: %s", args.prompt)
+        response = client.get_completion(args.prompt)
 
-    # Format response with syntax highlighting and colors
-    logging.debug("Formatting response")
-    formatted_response = format_text(response)
+    logging.debug(f"\nGot response: {response}")
+    if args.format:
+        # Format response with syntax highlighting and colors
+        logging.debug("Formatting response")
+        formatted_response = format_text(response)
 
-    # Print the output in a pretty format
-    print_output(formatted_response)
+        # Print the output in a pretty format
+        print_output(formatted_response)
 
 if __name__ == "__main__":
     main()
```

### Comparing `echoai-dev-0.1.2/echoai_dev.egg-info/PKG-INFO` & `echoai-dev-0.2.0rc1/echoai_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoai-dev
-Version: 0.1.2
+Version: 0.2.0rc1
 Summary: The command line tool to interface with Generative AI.
 Author: Fabio Dr.No Nonato
 Author-email: echoaidev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `echoai-dev-0.1.2/setup.py` & `echoai-dev-0.2.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     shutil.rmtree("echoai.egg-info")
 
 if os.path.exists("echoai.egg-info"):
     print("Removing old builds")
     cleanechoai()
 
 # get current git commit sha
-# commit_sha = subprocess.check_output(['git', 'rev-parse', 'HEAD']).strip().decode()
+commit_sha = subprocess.check_output(['git', 'rev-parse', 'HEAD']).strip().decode()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="echoai-dev",
-    version=f"0.1.2",
+    version=f"0.2.0rc1",
     author="Fabio Dr.No Nonato",
     author_email="echoaidev@gmail.com",
     description="The command line tool to interface with Generative AI.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

