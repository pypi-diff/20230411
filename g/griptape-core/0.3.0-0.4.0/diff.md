# Comparing `tmp/griptape_core-0.3.0.tar.gz` & `tmp/griptape_core-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.3.0.tar", max compression
+gzip compressed data, was "griptape_core-0.4.0.tar", max compression
```

## Comparing `griptape_core-0.3.0.tar` & `griptape_core-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.3.0/LICENSE
--rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.3.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.3.0/griptape/__init__.py
--rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.3.0/griptape/core/__init__.py
--rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.3.0/griptape/core/adapters/__init__.py
--rw-r--r--   0        0        0     2399 2023-04-08 22:46:20.173376 griptape_core-0.3.0/griptape/core/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1010 2023-04-08 22:52:20.104416 griptape_core-0.3.0/griptape/core/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.3.0/griptape/core/base_adapter.py
--rw-r--r--   0        0        0      467 2023-04-07 15:43:24.032498 griptape_core-0.3.0/griptape/core/base_executor.py
--rw-r--r--   0        0        0     3287 2023-04-08 22:48:21.389760 griptape_core-0.3.0/griptape/core/base_tool.py
--rw-r--r--   0        0        0      533 2023-04-08 22:54:40.019493 griptape_core-0.3.0/griptape/core/decorators.py
--rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.3.0/griptape/core/executors/__init__.py
--rw-r--r--   0        0        0     3048 2023-04-07 15:57:20.791900 griptape_core-0.3.0/griptape/core/executors/docker_executor.py
--rw-r--r--   0        0        0     1887 2023-04-07 15:42:00.394059 griptape_core-0.3.0/griptape/core/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.3.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.3.0/griptape/core/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.3.0/griptape/core/utils/__init__.py
--rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.3.0/griptape/core/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.3.0/griptape/core/utils/manifest_validator.py
--rw-r--r--   0        0        0      708 2023-04-09 16:41:52.228246 griptape_core-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.4.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.4.0/griptape/__init__.py
+-rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.4.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.4.0/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2385 2023-04-11 16:28:17.823406 griptape_core-0.4.0/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0     1010 2023-04-08 22:52:20.104416 griptape_core-0.4.0/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.4.0/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.4.0/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     3688 2023-04-11 17:33:25.304240 griptape_core-0.4.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      533 2023-04-11 16:17:03.307430 griptape_core-0.4.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.4.0/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.4.0/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.4.0/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.4.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.4.0/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.4.0/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.4.0/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.4.0/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      708 2023-04-11 20:38:38.831174 griptape_core-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.4.0/PKG-INFO
```

### Comparing `griptape_core-0.3.0/LICENSE` & `griptape_core-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.3.0/README.md` & `griptape_core-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape_core-0.3.0/griptape/core/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.4.0/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,11 +61,11 @@
                 functools.partial(self.__execute_action, action),
                 methods=["GET"],
                 description=tool.get_action_description(action)
             )
 
         return app
 
-    def __execute_action(self, action: callable, action_input: str) -> dict:
+    def __execute_action(self, action: callable, value: str) -> dict:
         return ast.literal_eval(
-            self.executor.execute(action, action_input.encode()).decode()
+            self.executor.execute(action, value.encode()).decode()
         )
```

### Comparing `griptape_core-0.3.0/griptape/core/adapters/langchain_tool_adapter.py` & `griptape_core-0.4.0/griptape/core/adapters/langchain_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.3.0/griptape/core/base_tool.py` & `griptape_core-0.4.0/griptape/core/base_tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 @define
 class BaseTool(ABC):
     MANIFEST_FILE = "manifest.yml"
     DOCKERFILE_FILE = "Dockerfile"
     REQUIREMENTS_FILE = "requirements.txt"
 
     @property
+    def name(self) -> str:
+        return self.__class__.__name__
+
+    @property
     def env_fields(self) -> list[Attribute]:
         return [f for f in fields(self.__class__) if f.metadata.get("env")]
 
     @property
     def env(self) -> dict[str, str]:
         return {f.metadata["env"]: str(getattr(self, f.name)) for f in self.env_fields}
 
@@ -50,49 +54,57 @@
     def abs_file_path(self):
         return os.path.abspath(inspect.getfile(self.__class__))
 
     @property
     def abs_dir_path(self):
         return os.path.dirname(self.abs_file_path)
 
+    def actions(self) -> list[callable]:
+        methods = []
+
+        for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
+            if getattr(method, "is_action", False):
+                methods.append(method)
+
+        return methods
+
     def env_value(self, name: str) -> Optional[str]:
         env_var_value = os.environ.get(name, None)
         if env_var_value:
             return env_var_value
         else:
             return next(
                 (str(getattr(self, f.name)) for f in self.env_fields if f.metadata.get("env") == name),
                 None
             )
 
+    def get_action_name(self, action: callable) -> str:
+        if action is None or not getattr(action, "is_action", False):
+            raise Exception("This method is not a tool action.")
+        else:
+            schema = action.config["value_schema"].json_schema("ToolActionSchema")
+
+            return action.config["name"]
+
     def get_action_description(self, action: callable) -> str:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
-            schema = action.config['input_schema'].json_schema('ToolActionSchema')
+            schema = action.config["value_schema"].json_schema("ToolActionSchema")
 
             return str.join("\n", [
                 action.config["description"],
                 f"Input schema: {json.dumps(schema)}"
             ])
 
-    def get_action_input_schema(self, action: callable) -> str:
+    def get_action_value_schema(self, action: callable) -> dict:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
-            return json.dumps(action.config["input_schema"].json_schema("ToolInputSchema"))
-
-    def actions(self) -> list[callable]:
-        methods = []
-
-        for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
-            if getattr(method, "is_action", False):
-                methods.append(method)
-
-        return methods
+            return action.config["value_schema"].json_schema("ToolInputSchema")
 
     def validate(self) -> bool:
         from griptape.core.utils import ManifestValidator
 
         if not os.path.exists(self.manifest_path):
             raise Exception(f"{self.MANIFEST_FILE} not found")
```

### Comparing `griptape_core-0.3.0/griptape/core/decorators.py` & `griptape_core-0.4.0/griptape/core/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     return decorator
 
 
 def __config_schema() -> Schema:
     return Schema({
         "name": str,
         "description": str,
-        "input_schema": Schema
+        "value_schema": Schema
     }, ignore_extra_keys=True)
```

### Comparing `griptape_core-0.3.0/griptape/core/executors/docker_executor.py` & `griptape_core-0.4.0/griptape/core/executors/docker_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.remove_existing_container(self.container_name(tool))
 
         return self.run_container(tool_action, value).encode()
 
     def run_container(self, tool_action: callable, value: bytes) -> str:
         tool = tool_action.__self__
         workdir = "/tool"
-        tool_name = self.tool_name(tool)
+        tool_name = tool.name
         command = [
             "python",
             "-c",
             f'from tool import {tool_name}; print({tool_name}().{tool_action.__name__}({value}))'
         ]
         binds = {
             self.tool_dir(tool): {
@@ -90,11 +90,11 @@
             )
 
             response = [line for line in image]
 
             logging.info(f"Built image: {response[0].short_id}")
 
     def image_name(self, tool: BaseTool) -> str:
-        return f"{stringcase.snakecase(self.tool_name(tool))}_image"
+        return f"{stringcase.snakecase(tool.name)}_image"
 
     def container_name(self, tool: BaseTool) -> str:
-        return f"{stringcase.snakecase(self.tool_name(tool))}_container"
+        return f"{stringcase.snakecase(tool.name)}_container"
```

### Comparing `griptape_core-0.3.0/griptape/core/executors/local_executor.py` & `griptape_core-0.4.0/griptape/core/executors/local_executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @define
 class LocalExecutor(BaseExecutor):
     verbose: int = field(default=False, kw_only=True)
 
     def execute(self, tool_action: callable, value: bytes) -> bytes:
         tool = tool_action.__self__
 
-        logging.warning(f"You are executing the {self.tool_name(tool)} tool in the local environment. Make sure to "
+        logging.warning(f"You are executing the {tool.name} tool in the local environment. Make sure to "
                         f"switch to a more secure ToolExecutor in production.")
 
         env = os.environ.copy()
 
         env.update(tool.env)
 
         self.install_dependencies(env, tool)
@@ -44,15 +44,15 @@
             cwd=self.tool_dir(tool),
             stdout=None if self.verbose else subprocess.DEVNULL,
             stderr=None if self.verbose else subprocess.DEVNULL
         )
 
     def run_subprocess(self, env: dict[str, str], tool_action: callable, value: bytes) -> subprocess.CompletedProcess:
         tool = tool_action.__self__
-        tool_name = self.tool_name(tool)
+        tool_name = tool.name
         command = [
             "python",
             "-c",
             f'from tool import {tool_name}; print({tool_name}().{tool_action.__name__}({value}))'
         ]
 
         return subprocess.run(
```

### Comparing `griptape_core-0.3.0/griptape/core/utils/j2.py` & `griptape_core-0.4.0/griptape/core/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.3.0/pyproject.toml` & `griptape_core-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.3.0"
+version = "0.4.0"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
```

### Comparing `griptape_core-0.3.0/PKG-INFO` & `griptape_core-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

