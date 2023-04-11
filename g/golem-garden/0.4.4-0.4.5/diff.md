# Comparing `tmp/golem_garden-0.4.4.tar.gz` & `tmp/golem_garden-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_garden-0.4.4.tar", last modified: Sat Mar 25 19:22:49 2023, max compression
+gzip compressed data, was "golem_garden-0.4.5.tar", last modified: Tue Apr 11 13:51:44 2023, max compression
```

## Comparing `golem_garden-0.4.4.tar` & `golem_garden-0.4.5.tar`

### file list

```diff
@@ -1,24 +1,39 @@
--rw-r--r--   0        0        0      519 2023-03-25 19:22:41.720356 golem_garden-0.4.4/.github/workflows/deploy_docs.yml
--rw-r--r--   0        0        0     1142 2023-03-25 19:22:41.720356 golem_garden-0.4.4/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1832 2023-03-25 19:22:41.720356 golem_garden-0.4.4/.gitignore
--rw-r--r--   0        0        0    34523 2023-03-25 19:22:41.720356 golem_garden-0.4.4/LICENSE
--rw-r--r--   0        0        0       60 2023-03-25 19:22:41.720356 golem_garden-0.4.4/README.md
--rw-r--r--   0        0        0      129 2023-03-25 19:22:41.720356 golem_garden-0.4.4/RUN_ME.py
--rw-r--r--   0        0        0       14 2023-03-25 19:22:41.720356 golem_garden-0.4.4/docs/development/contributing.md
--rw-r--r--   0        0        0     2359 2023-03-25 19:22:41.720356 golem_garden-0.4.4/docs/development/style_guide.md
--rw-r--r--   0        0        0     1306 2023-03-25 19:22:41.720356 golem_garden-0.4.4/docs/index.md
--rw-r--r--   0        0        0      328 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/__init__.py
--rw-r--r--   0        0        0      187 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/__main__.py
--rw-r--r--   0        0        0     2907 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/database/context_database.py
--rw-r--r--   0        0        0     3423 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/golems/golem.py
--rw-r--r--   0        0        0     1993 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/golems/golem_configs/_default_golem.toml
--rw-r--r--   0        0        0     1067 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/golems/golem_configs/golem_config.py
--rw-r--r--   0        0        0     1570 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/openai/openai_api.py
--rw-r--r--   0        0        0      217 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/openai/openai_chat_configs/_default_openai_chat_config.toml
--rw-r--r--   0        0        0     1790 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/openai/openai_chat_configs/openai_chat_config.py
--rw-r--r--   0        0        0     1117 2023-03-25 19:22:41.720356 golem_garden-0.4.4/golem_garden/user_interface/command_line_interface.py
--rw-r--r--   0        0        0      398 2023-03-25 19:22:41.720356 golem_garden-0.4.4/mkdocs.yml
--rw-r--r--   0        0        0     1041 2023-03-25 19:22:41.720356 golem_garden-0.4.4/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-25 19:22:41.720356 golem_garden-0.4.4/requirements.txt
--rw-r--r--   0        0        0     4835 2023-03-25 19:22:41.720356 golem_garden-0.4.4/utilities/grab_all_py_in_one_text_block.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 golem_garden-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      519 2023-04-11 13:51:39.723108 golem_garden-0.4.5/.github/workflows/deploy_docs.yml
+-rw-r--r--   0        0        0     1142 2023-04-11 13:51:39.723108 golem_garden-0.4.5/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1844 2023-04-11 13:51:39.723108 golem_garden-0.4.5/.gitignore
+-rw-r--r--   0        0        0    34523 2023-04-11 13:51:39.723108 golem_garden-0.4.5/LICENSE
+-rw-r--r--   0        0        0      178 2023-04-11 13:51:39.723108 golem_garden-0.4.5/README.md
+-rw-r--r--   0        0        0      114 2023-04-11 13:51:39.723108 golem_garden-0.4.5/RUN_ME.py
+-rw-r--r--   0        0        0       14 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/development/contributing.md
+-rw-r--r--   0        0        0     2359 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/development/style_guide.md
+-rw-r--r--   0        0        0     2396 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/development/style_guide_for_gpt.md
+-rw-r--r--   0        0        0     1306 2023-04-11 13:51:39.723108 golem_garden-0.4.5/docs/index.md
+-rw-r--r--   0        0        0    78233 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/Notebook_Companion_Embedding_as_a_Service.ipynb
+-rw-r--r--   0        0        0     3739 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/knowledge_corpus_embeddings/string_chopper.py
+-rw-r--r--   0        0        0     2341 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/pinecone_open_ai_ada_embedding.py
+-rw-r--r--   0        0        0     1305 2023-04-11 13:51:39.723108 golem_garden-0.4.5/experimental/sentence_transformer.py
+-rw-r--r--   0        0        0      313 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/__main__.py
+-rw-r--r--   0        0        0     2125 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/api/main.py
+-rw-r--r--   0        0        0      712 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/command_line_interface.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/__init__.py
+-rw-r--r--   0        0        0      350 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/base_database.py
+-rw-r--r--   0        0        0     3770 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/json_database.py
+-rw-r--r--   0        0        0     3276 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/_strategies/mongo_database.py
+-rw-r--r--   0        0        0      502 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/database.json
+-rw-r--r--   0        0        0     1293 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/database/database_factory.py
+-rw-r--r--   0        0        0     3274 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/golems/golem.py
+-rw-r--r--   0        0        0     1993 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/golems/golem_configs/_default_golem.toml
+-rw-r--r--   0        0        0     1067 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/golems/golem_configs/golem_config.py
+-rw-r--r--   0        0        0     1603 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/openai/openai_api.py
+-rw-r--r--   0        0        0      217 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/openai/openai_chat_configs/_default_openai_chat_config.toml
+-rw-r--r--   0        0        0     1790 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/openai/openai_chat_configs/openai_chat_config.py
+-rw-r--r--   0        0        0     1717 2023-04-11 13:51:39.723108 golem_garden-0.4.5/golem_garden/tests/test_string_chopper.py
+-rw-r--r--   0        0        0      398 2023-04-11 13:51:39.723108 golem_garden-0.4.5/mkdocs.yml
+-rw-r--r--   0        0        0     1152 2023-04-11 13:51:39.723108 golem_garden-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2988 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/directory_printer.py
+-rw-r--r--   0        0        0     5029 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/grab_all_py_in_one_text_block.py
+-rw-r--r--   0        0        0     2306 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/pinecone.py
+-rw-r--r--   0        0        0      507 2023-04-11 13:51:39.723108 golem_garden-0.4.5/utilities/try_mongo_connection.py
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 golem_garden-0.4.5/PKG-INFO
```

### Comparing `golem_garden-0.4.4/.github/workflows/deploy_docs.yml` & `golem_garden-0.4.5/.github/workflows/deploy_docs.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `golem_garden-0.4.5/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/.gitignore` & `golem_garden-0.4.5/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -125,8 +125,10 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .idea
 .vscode
-utilities/output/*
+utilities/output/*
+
+.DS_Store
```

### Comparing `golem_garden-0.4.4/LICENSE` & `golem_garden-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/docs/development/style_guide.md` & `golem_garden-0.4.5/docs/development/style_guide.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/docs/index.md` & `golem_garden-0.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/golem_garden/database/context_database.py` & `golem_garden-0.4.5/golem_garden/database/_strategies/mongo_database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+import os
 import uuid
 from typing import Dict, List, Union
 
+from dotenv import load_dotenv
 from pymongo import MongoClient
 
 
-class ContextDatabase:
+
+class MongoDatabase:
     # TODO - integrate with new refactor of Golem class
     def __init__(self,
                  database_name: str = "golem_garden",
                  collection_name: str = "conversations",
                  session_id: str = str(uuid.uuid4())):
-        self._mongo_client = MongoClient()
+        # load_dotenv()
+        # self._mongo_client = MongoClient(os.getenv('MONGO_URI'))
+        self._mongo_client = MongoClient("mongodb://localhost:27017/")
+        db = self._mongo_client.test
+        print(f"\n\n\n_________\ndb: {db}\n__________\n\n\n")
+        print(f"\n\n\n_________\ndb.list_collection_names(): {db.list_collection_names()}\n__________\n\n\n")
+
         self._database = self._mongo_client[database_name]
         self._conversations_collection = self._database[collection_name]
         self._session_id = session_id
 
     def add_message(self,
                     golem_name: str,
                     user_id: str,
```

### Comparing `golem_garden-0.4.4/golem_garden/golems/golem.py` & `golem_garden-0.4.5/golem_garden/golems/golem.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import asyncio
 import os
 import uuid
 
-import openai
-from dotenv import load_dotenv
 
-from golem_garden.database.context_database import ContextDatabase
+from golem_garden.database.database_factory import get_database
 from golem_garden.golems.golem_configs.golem_config import GolemConfig, load_golem_config
 from golem_garden.openai.openai_api import OpenAIAPIClient
 from golem_garden.openai.openai_chat_configs.openai_chat_config import OpenaiChatParameters, load_openai_chat_parameters
 
-load_dotenv()
-openai.api_key = os.getenv("OPENAI_API_KEY")
-
 
 class Golem:
     def __init__(self,
                  user_id: str,
                  session_id: str = str(uuid.uuid4()),
                  golem_config: GolemConfig = load_golem_config(),
                  openai_chat_parameters: OpenaiChatParameters = load_openai_chat_parameters(),
                  ):
         self._user_id = user_id
         self._session_id = session_id
         self._golem_config = golem_config
         self._openai_chat_parameters = openai_chat_parameters
-        self._openai_client = OpenAIAPIClient(api_key=openai.api_key)
-        self._context_database = ContextDatabase(session_id=self._session_id)
+        self._openai_client = OpenAIAPIClient()
+        self._context_database = get_database()
 
     @property
     def name(self) -> str:
+        #TODO - create unique uuid for each golem when it is created
         return self._golem_config.name
 
     @property
     def type(self) -> str:
         return self._golem_config.type
 
     @property
@@ -47,30 +43,30 @@
     async def chat(self, user_input: str) -> str:
         system = {"role": "system",
                   "content": self._golem_config.golem_string,
                   }
         new_message = {"role": "user",
                        "content": user_input.strip()}
 
-        history = self._context_database.get_history({"golem_name": self._golem_config.name,
-                                                      "user_id": self._user_id,
-                                                      "session_id": self._session_id})
+        history = self._context_database.get_history(golem_id=self.name,
+                                                     user_id=self._user_id,
+                                                     )
 
         conversation = [system]
         if len(history) > 0:
             conversation.extend(history)
         conversation.append(new_message)
 
         response = await self._openai_client.query(conversation=conversation,
                                                    chat_parameters=self._openai_chat_parameters, )
 
-        self._context_database.add_message(golem_name=self.name,
+        self._context_database.add_message(golem_id=self.name,
                                            user_id=self._user_id,
                                            message=new_message)
-        self._context_database.add_response(golem_name=self.name,
+        self._context_database.add_response(golem_id = self.name,
                                             user_id=self._user_id,
                                             response=response)
 
         return response["choices"][0]["message"]["content"].strip()
 
     async def poke(self):
         user_input = f"A human just poked you, say the Golem equivalent of 'Hello World!'"
```

### Comparing `golem_garden-0.4.4/golem_garden/golems/golem_configs/_default_golem.toml` & `golem_garden-0.4.5/golem_garden/golems/golem_configs/_default_golem.toml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/golem_garden/golems/golem_configs/golem_config.py` & `golem_garden-0.4.5/golem_garden/golems/golem_configs/golem_config.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/golem_garden/openai/openai_api.py` & `golem_garden-0.4.5/golem_garden/openai/openai_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import asyncio
+import os
 from typing import Dict, List, Any
 
 import openai
+from dotenv import load_dotenv
 
 from golem_garden.openai.openai_chat_configs.openai_chat_config import OpenaiChatParameters, load_openai_chat_parameters
 
 
 class OpenAIAPIClient:
     # TODO - integrate with new impelementation fo Golem and use openai_chat_config
-    def __init__(self, api_key: str):
-        self.api_key = api_key
-        openai.api_key = self.api_key
+    def __init__(self):
+        load_dotenv()
+        openai.api_key = os.getenv("OPENAI_API_KEY")
 
     async def query(self,
                     conversation: List[Dict[str, str]],
                     chat_parameters: OpenaiChatParameters = load_openai_chat_parameters(),
                     only_return_message_content: bool = False) -> Dict[str, Any]:
         loop = asyncio.get_event_loop()
         response = await loop.run_in_executor(None, lambda: openai.ChatCompletion.create(
```

### Comparing `golem_garden-0.4.4/golem_garden/openai/openai_chat_configs/openai_chat_config.py` & `golem_garden-0.4.5/golem_garden/openai/openai_chat_configs/openai_chat_config.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.4.4/pyproject.toml` & `golem_garden-0.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,35 @@
 ]
 
 
 dependencies = [
     "python-dotenv",
     "openai",
     "pymongo",
+    "motor",
     "toml",
+    "openai",
+    "fastapi",
+    "uvicorn",
+    "torch",
+    "retry",
+    "sentence-transformers"
 ]
 requires-python = ">=3.8"
 
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/jonmatthis/golem_garden"
 
 [tool.bumpver]
-current_version = "v0.4.4"
+current_version = "v0.4.5"
 
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
```

### Comparing `golem_garden-0.4.4/utilities/grab_all_py_in_one_text_block.py` & `golem_garden-0.4.5/utilities/grab_all_py_in_one_text_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,15 +79,18 @@
 
     def _get_current_timestamp(self):
         now = datetime.now().strftime("%Y-%m-%d_%H_%M_%S")
         return now
 
 
 if __name__ == '__main__':
-    directory_paths = [r"C:\Users\jonma\github_repos\jonmatthis\golem_garden\golem_garden"]
+    # directory_paths = [r"C:\Users\jonma\github_repos\jonmatthis\golem_garden\golem_garden"]
+    # directory_paths = [r"C:\Users\jonma\github_repos\jonmatthis\golem_garden\golem_garden\database"]
+    directory_paths = [r"C:\Users\jonma\github_repos\freemocap_organization\freemocap"]
+
     included_files = []
 
     excluded_directories = ['__pycache__',
                             'venv',
                             '.venv',
                             'build',
                             'dist',
```

### Comparing `golem_garden-0.4.4/PKG-INFO` & `golem_garden-0.4.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 Metadata-Version: 2.1
 Name: golem_garden
-Version: 0.4.4
+Version: 0.4.5
 Summary: Welcome to the Garden - We're so glad you're here <3 
 Keywords: chat
 Author: Jonathan Samir Matthis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: python-dotenv
 Requires-Dist: openai
 Requires-Dist: pymongo
+Requires-Dist: motor
 Requires-Dist: toml
+Requires-Dist: openai
+Requires-Dist: fastapi
+Requires-Dist: uvicorn
+Requires-Dist: torch
+Requires-Dist: retry
+Requires-Dist: sentence-transformers
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Project-URL: Homepage, https://github.com/jonmatthis/golem_garden
 Provides-Extra: dev
 
 # Welcome to the Garden 
 
 We're so glad you're here 🌱✨
 
+In a terminal with a Python environment enabled, enter:
+```bash
+pip install -e .
+```
+Then:
+```bash
+golem_garden`
+```
+
```

