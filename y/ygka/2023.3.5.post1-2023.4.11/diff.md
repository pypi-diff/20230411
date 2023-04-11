# Comparing `tmp/ygka-2023.3.5.post1.tar.gz` & `tmp/ygka-2023.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygka-2023.3.5.post1.tar", max compression
+gzip compressed data, was "ygka-2023.4.11.tar", max compression
```

## Comparing `ygka-2023.3.5.post1.tar` & `ygka-2023.4.11.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1068 2023-03-05 14:50:15.609326 ygka-2023.3.5.post1/LICENSE
--rw-r--r--   0        0        0     2567 2023-03-05 14:50:15.609326 ygka-2023.3.5.post1/README.md
--rw-r--r--   0        0        0     1411 2023-03-05 14:50:40.121249 ygka-2023.3.5.post1/pyproject.toml
--rw-r--r--   0        0        0       53 2023-03-05 14:50:15.617326 ygka-2023.3.5.post1/ygka/__init__.py
--rw-r--r--   0        0        0      119 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/__main__.py
--rw-r--r--   0        0        0       78 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/adapters/__init__.py
--rw-r--r--   0        0        0     1151 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/adapters/openai_cookie_adapter.py
--rw-r--r--   0        0        0      704 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/adapters/test/test_openai_cookie_adapter.py
--rw-r--r--   0        0        0       84 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/cli/__init__.py
--rw-r--r--   0        0        0       43 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/cli/cli_app.py
--rw-r--r--   0        0        0     2824 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/cli/config_ygka.py
--rw-r--r--   0        0        0      112 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/cli/retrieve_stdin.py
--rw-r--r--   0        0        0     1751 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/cli/ygka.py
--rw-r--r--   0        0        0       90 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/exceptions/__init__.py
--rw-r--r--   0        0        0       51 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/exceptions/unauthorized_access_error.py
--rw-r--r--   0        0        0      234 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/models/__init__.py
--rw-r--r--   0        0        0      155 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/models/language_model.py
--rw-r--r--   0        0        0      705 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/models/revchatgpt_chatbot_config_model.py
--rw-r--r--   0        0        0      403 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/models/str_enum.py
--rw-r--r--   0        0        0     1038 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/models/ygka_config_model.py
--rw-r--r--   0        0        0      324 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/query_clients/__init__.py
--rw-r--r--   0        0        0      714 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/query_clients/official_chatgpt_client.py
--rw-r--r--   0        0        0      155 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/query_clients/query_client.py
--rw-r--r--   0        0        0      868 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/query_clients/query_client_factory.py
--rw-r--r--   0        0        0     1662 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/query_clients/reverse_engineered_chatgpt_client.py
--rw-r--r--   0        0        0        0 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/tests/__init__.py
--rw-r--r--   0        0        0       58 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/tests/test_sample.py
--rw-r--r--   0        0        0       73 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/utils/__init__.py
--rw-r--r--   0        0        0      334 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/utils/test/test_ygka_config_manager.py
--rw-r--r--   0        0        0     1669 2023-03-05 14:50:15.621326 ygka-2023.3.5.post1/ygka/utils/ygka_config_manager.py
--rw-r--r--   0        0        0     3146 1970-01-01 00:00:00.000000 ygka-2023.3.5.post1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-11 08:06:45.484779 ygka-2023.4.11/LICENSE
+-rw-r--r--   0        0        0     2810 2023-04-11 08:06:45.484779 ygka-2023.4.11/README.md
+-rw-r--r--   0        0        0     1409 2023-04-11 08:07:11.336987 ygka-2023.4.11/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/__main__.py
+-rw-r--r--   0        0        0       78 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/adapters/__init__.py
+-rw-r--r--   0        0        0     1151 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/adapters/openai_cookie_adapter.py
+-rw-r--r--   0        0        0      704 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/adapters/test/test_openai_cookie_adapter.py
+-rw-r--r--   0        0        0       84 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/__init__.py
+-rw-r--r--   0        0        0       43 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/cli_app.py
+-rw-r--r--   0        0        0     2824 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/config_ygka.py
+-rw-r--r--   0        0        0      112 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/retrieve_stdin.py
+-rw-r--r--   0        0        0     1751 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/ygka.py
+-rw-r--r--   0        0        0       90 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/exceptions/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/exceptions/unauthorized_access_error.py
+-rw-r--r--   0        0        0      234 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/language_model.py
+-rw-r--r--   0        0        0      705 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/revchatgpt_chatbot_config_model.py
+-rw-r--r--   0        0        0      403 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/str_enum.py
+-rw-r--r--   0        0        0     1038 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/ygka_config_model.py
+-rw-r--r--   0        0        0      324 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/__init__.py
+-rw-r--r--   0        0        0      714 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/official_chatgpt_client.py
+-rw-r--r--   0        0        0      155 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/query_client.py
+-rw-r--r--   0        0        0      868 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/query_client_factory.py
+-rw-r--r--   0        0        0     1661 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/reverse_engineered_chatgpt_client.py
+-rw-r--r--   0        0        0        0 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/tests/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/tests/test_sample.py
+-rw-r--r--   0        0        0       73 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/utils/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/utils/test/test_ygka_config_manager.py
+-rw-r--r--   0        0        0     1669 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/utils/ygka_config_manager.py
+-rw-r--r--   0        0        0     3384 1970-01-01 00:00:00.000000 ygka-2023.4.11/PKG-INFO
```

### Comparing `ygka-2023.3.5.post1/LICENSE` & `ygka-2023.4.11/LICENSE`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/README.md` & `ygka-2023.4.11/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -46,20 +46,24 @@
 
 ```sh
 cat textfile.txt | ygka "what is this file?"
 ```
 
 ## Advanced Settings 🛠
 
-By default, YGKA is configured to use either the official_chatgpt or reverse_engineered_chatgpt language model. To change the language model, modify the `~/.ygka_config.json` file as follows:
+By default, `YGKA` is configured to use the reverse-engineered ChatGPT client and retrieve login information from your browser, so you don't need to configure anything to use `YGKA`. However, for those who want to use different models with an OpenAI API Key, you can configure it as follows:
+
+1. Create an account on OpenAI.
+1. Go to <https://platform.openai.com/account/api-keys> and copy your API key.
+1. Modify or create the `~/.ygka_config.json` file as follows:
 
 ```json
 {
     ...
-    "language_model": <language model of your preference>, //"official_chatgpt" or "reverse_engineered_chatgpt"
+    "language_model": <language model of your preference>, //"official_chatgpt"
     "openai_api_key": <your OpenAI API key>
 }
 ```
 
 Here, you can specify the language model of your preference and add your OpenAI API key.
 
 ## Inspired By 🎨
```

### Comparing `ygka-2023.3.5.post1/pyproject.toml` & `ygka-2023.4.11/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ygka"
-version = "2023.03.05-1"
+version = "2023.04.11"
 description = ""
 authors = []
 readme = "README.md"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 pythonPlatform = "All"
@@ -33,15 +33,15 @@
 line-length = 119
 select = [ "PLE", "PLR", "PLW", "E", "W", "F", "I", "Q",]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 poetry = "^1.4.0"
 rich = "<13.0.0"
-revchatgpt = "^3.1.1"
+revchatgpt = "^4.1.6"
 pydantic = "^1.10.5"
 yt-dlp = "^2023.3.4"
 
 [tool.poetry.scripts]
 ygka = "ygka:main"
 
 [tool.ruff.flake8-quotes]
```

### Comparing `ygka-2023.3.5.post1/ygka/adapters/openai_cookie_adapter.py` & `ygka-2023.4.11/ygka/adapters/openai_cookie_adapter.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/adapters/test/test_openai_cookie_adapter.py` & `ygka-2023.4.11/ygka/adapters/test/test_openai_cookie_adapter.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/cli/config_ygka.py` & `ygka-2023.4.11/ygka/cli/config_ygka.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/cli/ygka.py` & `ygka-2023.4.11/ygka/cli/ygka.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/models/revchatgpt_chatbot_config_model.py` & `ygka-2023.4.11/ygka/models/revchatgpt_chatbot_config_model.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/models/ygka_config_model.py` & `ygka-2023.4.11/ygka/models/ygka_config_model.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/query_clients/official_chatgpt_client.py` & `ygka-2023.4.11/ygka/query_clients/official_chatgpt_client.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/query_clients/query_client_factory.py` & `ygka-2023.4.11/ygka/query_clients/query_client_factory.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/ygka/query_clients/reverse_engineered_chatgpt_client.py` & `ygka-2023.4.11/ygka/query_clients/reverse_engineered_chatgpt_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional, Union, cast
+from typing import Optional, Union
 
 from revChatGPT.V1 import Chatbot
 
 from ygka.exceptions import UnauthorizedAccessError
 from ygka.models import RevChatGPTChatbotConfigModel
 
 from .query_client import QueryClient
@@ -36,11 +36,11 @@
 
     def query(self, prompt: str) -> str:
         chatbot = Chatbot(config=self.revchatgpt_config)  #  pyright: ignore [reportGeneralTypeIssues]
         # ignore for wrong type hint of revchatgpt
 
         response_text = ''
         for data in chatbot.ask(prompt):
-            response_text = data['message']
+            response_text = data['message']  # type: ignore
 
-        response_text = cast(str, response_text)
+        response_text = response_text
         return response_text
```

### Comparing `ygka-2023.3.5.post1/ygka/utils/ygka_config_manager.py` & `ygka-2023.4.11/ygka/utils/ygka_config_manager.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.3.5.post1/PKG-INFO` & `ygka-2023.4.11/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ygka
-Version: 2023.3.5.post1
+Version: 2023.4.11
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poetry (>=1.4.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: revchatgpt (>=3.1.1,<4.0.0)
+Requires-Dist: revchatgpt (>=4.1.6,<5.0.0)
 Requires-Dist: rich (<13.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # YGKA 🤖
 
@@ -63,20 +63,24 @@
 
 ```sh
 cat textfile.txt | ygka "what is this file?"
 ```
 
 ## Advanced Settings 🛠
 
-By default, YGKA is configured to use either the official_chatgpt or reverse_engineered_chatgpt language model. To change the language model, modify the `~/.ygka_config.json` file as follows:
+By default, `YGKA` is configured to use the reverse-engineered ChatGPT client and retrieve login information from your browser, so you don't need to configure anything to use `YGKA`. However, for those who want to use different models with an OpenAI API Key, you can configure it as follows:
+
+1. Create an account on OpenAI.
+1. Go to <https://platform.openai.com/account/api-keys> and copy your API key.
+1. Modify or create the `~/.ygka_config.json` file as follows:
 
 ```json
 {
     ...
-    "language_model": <language model of your preference>, //"official_chatgpt" or "reverse_engineered_chatgpt"
+    "language_model": <language model of your preference>, //"official_chatgpt"
     "openai_api_key": <your OpenAI API key>
 }
 ```
 
 Here, you can specify the language model of your preference and add your OpenAI API key.
 
 ## Inspired By 🎨
```

