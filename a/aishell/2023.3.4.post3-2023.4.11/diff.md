# Comparing `tmp/aishell-2023.3.4.post3.tar.gz` & `tmp/aishell-2023.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishell-2023.3.4.post3.tar", max compression
+gzip compressed data, was "aishell-2023.4.11.tar", max compression
```

## Comparing `aishell-2023.3.4.post3.tar` & `aishell-2023.4.11.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1064 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/LICENSE
--rw-r--r--   0        0        0     2529 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/README.md
--rw-r--r--   0        0        0       53 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/__init__.py
--rw-r--r--   0        0        0      128 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/__main__.py
--rw-r--r--   0        0        0       78 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/adapters/__init__.py
--rw-r--r--   0        0        0     1151 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/adapters/openai_cookie_adapter.py
--rw-r--r--   0        0        0        0 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/adapters/test/__init__.py
--rw-r--r--   0        0        0      707 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/adapters/test/test_openai_chatgpt_adapter.py
--rw-r--r--   0        0        0       90 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/cli/__init__.py
--rw-r--r--   0        0        0     2787 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/cli/aishell.py
--rw-r--r--   0        0        0       43 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/cli/cli_app.py
--rw-r--r--   0        0        0     2675 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/cli/config_aishell.py
--rw-r--r--   0        0        0        0 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/cli/test/__init__.py
--rw-r--r--   0        0        0     2614 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/cli/test/test_config_aishell.py
--rw-r--r--   0        0        0       90 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/exceptions/__init__.py
--rw-r--r--   0        0        0       51 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/exceptions/unauthorized_access_error.py
--rw-r--r--   0        0        0      323 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/models/__init__.py
--rw-r--r--   0        0        0     1058 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/models/aishell_config_model.py
--rw-r--r--   0        0        0      173 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/models/language_model.py
--rw-r--r--   0        0        0      505 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/models/open_ai_response_model.py
--rw-r--r--   0        0        0      705 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/models/revchatgpt_chatbot_config_model.py
--rw-r--r--   0        0        0      403 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/models/str_enum.py
--rw-r--r--   0        0        0        0 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/py.typed
--rw-r--r--   0        0        0      299 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/query_clients/__init__.py
--rw-r--r--   0        0        0     1330 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/query_clients/gpt3_client.py
--rw-r--r--   0        0        0     1150 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/query_clients/official_chatgpt_client.py
--rw-r--r--   0        0        0      155 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/query_clients/query_client.py
--rw-r--r--   0        0        0     2070 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/query_clients/reverse_engineered_chatgpt_client.py
--rw-r--r--   0        0        0        0 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/tests/__init__.py
--rw-r--r--   0        0        0       77 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/tests/sample_test.py
--rw-r--r--   0        0        0      171 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/utils/__init__.py
--rw-r--r--   0        0        0     1708 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/utils/aishell_config_manager.py
--rw-r--r--   0        0        0      389 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/utils/make_executable_command.py
--rw-r--r--   0        0        0        0 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/utils/test/__init__.py
--rw-r--r--   0        0        0      349 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/utils/test/test_aishell_config_manager.py
--rw-r--r--   0        0        0      884 2023-03-04 06:38:11.406439 aishell-2023.3.4.post3/aishell/utils/test/test_make_executable_command.py
--rw-r--r--   0        0        0     1456 2023-03-04 06:38:40.754659 aishell-2023.3.4.post3/pyproject.toml
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 aishell-2023.3.4.post3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-11 07:50:18.503513 aishell-2023.4.11/LICENSE
+-rw-r--r--   0        0        0     2959 2023-04-11 07:50:18.503513 aishell-2023.4.11/README.md
+-rw-r--r--   0        0        0       53 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/__init__.py
+-rw-r--r--   0        0        0      128 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/__main__.py
+-rw-r--r--   0        0        0       78 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/__init__.py
+-rw-r--r--   0        0        0     1151 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/openai_cookie_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/test/__init__.py
+-rw-r--r--   0        0        0      707 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/test/test_openai_chatgpt_adapter.py
+-rw-r--r--   0        0        0       90 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/aishell.py
+-rw-r--r--   0        0        0       43 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/cli_app.py
+-rw-r--r--   0        0        0     2675 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/config_aishell.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/test/__init__.py
+-rw-r--r--   0        0        0     2614 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/test/test_config_aishell.py
+-rw-r--r--   0        0        0       90 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/exceptions/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/exceptions/unauthorized_access_error.py
+-rw-r--r--   0        0        0      323 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/__init__.py
+-rw-r--r--   0        0        0     1058 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/aishell_config_model.py
+-rw-r--r--   0        0        0      173 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/language_model.py
+-rw-r--r--   0        0        0      505 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/open_ai_response_model.py
+-rw-r--r--   0        0        0      705 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/revchatgpt_chatbot_config_model.py
+-rw-r--r--   0        0        0      403 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/str_enum.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/py.typed
+-rw-r--r--   0        0        0      299 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/__init__.py
+-rw-r--r--   0        0        0     1330 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/gpt3_client.py
+-rw-r--r--   0        0        0     1150 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/official_chatgpt_client.py
+-rw-r--r--   0        0        0      155 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/query_client.py
+-rw-r--r--   0        0        0     2069 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/reverse_engineered_chatgpt_client.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/tests/__init__.py
+-rw-r--r--   0        0        0       77 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/tests/sample_test.py
+-rw-r--r--   0        0        0      171 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/__init__.py
+-rw-r--r--   0        0        0     1708 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/aishell_config_manager.py
+-rw-r--r--   0        0        0      389 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/make_executable_command.py
+-rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/test/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/test/test_aishell_config_manager.py
+-rw-r--r--   0        0        0      884 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/test/test_make_executable_command.py
+-rw-r--r--   0        0        0     1433 2023-04-11 07:50:44.415679 aishell-2023.4.11/pyproject.toml
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 aishell-2023.4.11/PKG-INFO
```

### Comparing `aishell-2023.3.4.post3/LICENSE` & `aishell-2023.4.11/LICENSE`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/README.md` & `aishell-2023.4.11/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # AiShell 🤖
 
 [![codecov](https://codecov.io/gh/code-yeongyu/AiShell/branch/master/graph/badge.svg?token=MR72XGUQWJ)](https://codecov.io/gh/code-yeongyu/AiShell)
 [![Release Package to PyPI](https://github.com/code-yeongyu/AiShell/actions/workflows/release.yml/badge.svg)](https://github.com/code-yeongyu/AiShell/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/aishell.svg)](https://badge.fury.io/py/aishell)
+[![Downloads](https://static.pepy.tech/personalized-badge/aishell?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/aishell)
 
 A simple Python code that connects to OpenAI's ChatGPT and executes the returned results.
 
+If you are interested in these projects, please checkout AiShell's brother project: [YGK-a](https://github.com/code-yeongyu/YGK-a). YGK-a is a client for the ChatGPT from your terminal, and also supports unix/linux pipelines.
+
 ## Demo
 
 ![Demo](https://raw.githubusercontent.com/code-yeongyu/AiShell/master/images/example.gif)
 
 ## Key Features 💡
 
 - Interact with your computer using natural language
@@ -42,15 +45,15 @@
 
 ## Advanced Settings 🛠
 
 By default, `AiShell` is configured to use the reverse-engineered ChatGPT client and retrieve login information from your browser, so you don't need to configure anything to use `AiShell`. However, for those who want to use different models with an OpenAI API Key, you can configure it as follows:
 
 1. Create an account on OpenAI.
 1. Go to <https://platform.openai.com/account/api-keys> and copy your API key.
-1. Modify or create the `~/.aishell/config.json` file as follows:
+1. Modify or create the `~/.aishell_config.json` file as follows:
 
   ```json
   {
       ...
       "language_model": <language model of your preference>, //"official_chatgpt" or "gpt3"
       "openai_api_key": <your OpenAI API key>
   }
```

### Comparing `aishell-2023.3.4.post3/aishell/adapters/openai_cookie_adapter.py` & `aishell-2023.4.11/aishell/adapters/openai_cookie_adapter.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/adapters/test/test_openai_chatgpt_adapter.py` & `aishell-2023.4.11/aishell/adapters/test/test_openai_chatgpt_adapter.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/cli/aishell.py` & `aishell-2023.4.11/aishell/cli/aishell.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/cli/config_aishell.py` & `aishell-2023.4.11/aishell/cli/config_aishell.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/cli/test/test_config_aishell.py` & `aishell-2023.4.11/aishell/cli/test/test_config_aishell.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/models/aishell_config_model.py` & `aishell-2023.4.11/aishell/models/aishell_config_model.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/models/revchatgpt_chatbot_config_model.py` & `aishell-2023.4.11/aishell/models/revchatgpt_chatbot_config_model.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/query_clients/gpt3_client.py` & `aishell-2023.4.11/aishell/query_clients/gpt3_client.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/query_clients/official_chatgpt_client.py` & `aishell-2023.4.11/aishell/query_clients/official_chatgpt_client.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/query_clients/reverse_engineered_chatgpt_client.py` & `aishell-2023.4.11/aishell/query_clients/reverse_engineered_chatgpt_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional, Union, cast
+from typing import Optional, Union
 
 from revChatGPT.V1 import Chatbot
 
 from aishell.exceptions import UnauthorizedAccessError
 from aishell.models import RevChatGPTChatbotConfigModel
 from aishell.utils import make_executable_command
 
@@ -38,17 +38,17 @@
     def query(self, prompt: str) -> str:
         prompt = self._construct_prompt(prompt)
         chatbot = Chatbot(config=self.revchatgpt_config)  #  pyright: ignore [reportGeneralTypeIssues]
         # ignore for wrong type hint of revchatgpt
 
         response_text = ''
         for data in chatbot.ask(prompt):
-            response_text = data['message']
+            response_text = data['message']  # type: ignore
 
-        response_text = make_executable_command(cast(str, response_text))
+        response_text = make_executable_command(response_text)
 
         return response_text
 
     def _construct_prompt(self, text: str) -> str:
         return f'''
 You are now a translater from human language to {os.uname()[0]} shell command.
 No explanation required, respond with only the raw shell command.
```

### Comparing `aishell-2023.3.4.post3/aishell/utils/aishell_config_manager.py` & `aishell-2023.4.11/aishell/utils/aishell_config_manager.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/aishell/utils/test/test_make_executable_command.py` & `aishell-2023.4.11/aishell/utils/test/test_make_executable_command.py`

 * *Files identical despite different names*

### Comparing `aishell-2023.3.4.post3/pyproject.toml` & `aishell-2023.4.11/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aishell"
-version = "2023.03.04-3"
+version = "2023.04.11"
 description = ""
 authors = []
 readme = "README.md"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 pythonPlatform = "All"
@@ -32,19 +32,18 @@
 [tool.ruff]
 line-length = 119
 select = [ "PLE", "PLR", "PLW", "E", "W", "F", "I", "Q", "C", "B",]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 poetry = "^1.4.0"
-revchatgpt = "^3.0.9"
-openai = "^0.26.5"
+revchatgpt = "^4.1.6"
+openai = "^0.27.4"
 pydantic = "^1.10.5"
 yt-dlp = "^2023.3.3"
-pyperclip = "^1.8.2"
 
 [tool.poetry.scripts]
 aishell = "aishell:main"
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 docstring-quotes = "single"
```

### Comparing `aishell-2023.3.4.post3/PKG-INFO` & `aishell-2023.4.11/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: aishell
-Version: 2023.3.4.post3
+Version: 2023.4.11
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.26.5,<0.27.0)
+Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: poetry (>=1.4.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
-Requires-Dist: revchatgpt (>=3.0.9,<4.0.0)
+Requires-Dist: revchatgpt (>=4.1.6,<5.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: yt-dlp (>=2023.3.3,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # AiShell 🤖
 
 [![codecov](https://codecov.io/gh/code-yeongyu/AiShell/branch/master/graph/badge.svg?token=MR72XGUQWJ)](https://codecov.io/gh/code-yeongyu/AiShell)
 [![Release Package to PyPI](https://github.com/code-yeongyu/AiShell/actions/workflows/release.yml/badge.svg)](https://github.com/code-yeongyu/AiShell/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/aishell.svg)](https://badge.fury.io/py/aishell)
+[![Downloads](https://static.pepy.tech/personalized-badge/aishell?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/aishell)
 
 A simple Python code that connects to OpenAI's ChatGPT and executes the returned results.
 
+If you are interested in these projects, please checkout AiShell's brother project: [YGK-a](https://github.com/code-yeongyu/YGK-a). YGK-a is a client for the ChatGPT from your terminal, and also supports unix/linux pipelines.
+
 ## Demo
 
 ![Demo](https://raw.githubusercontent.com/code-yeongyu/AiShell/master/images/example.gif)
 
 ## Key Features 💡
 
 - Interact with your computer using natural language
@@ -60,15 +62,15 @@
 
 ## Advanced Settings 🛠
 
 By default, `AiShell` is configured to use the reverse-engineered ChatGPT client and retrieve login information from your browser, so you don't need to configure anything to use `AiShell`. However, for those who want to use different models with an OpenAI API Key, you can configure it as follows:
 
 1. Create an account on OpenAI.
 1. Go to <https://platform.openai.com/account/api-keys> and copy your API key.
-1. Modify or create the `~/.aishell/config.json` file as follows:
+1. Modify or create the `~/.aishell_config.json` file as follows:
 
   ```json
   {
       ...
       "language_model": <language model of your preference>, //"official_chatgpt" or "gpt3"
       "openai_api_key": <your OpenAI API key>
   }
```

