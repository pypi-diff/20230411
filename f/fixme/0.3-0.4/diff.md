# Comparing `tmp/fixme-0.3.tar.gz` & `tmp/fixme-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixme-0.3.tar", last modified: Mon Apr 10 06:45:09 2023, max compression
+gzip compressed data, was "fixme-0.4.tar", last modified: Mon Apr 10 22:05:28 2023, max compression
```

## Comparing `fixme-0.3.tar` & `fixme-0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.802559 fixme-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 06:44:55.000000 fixme-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 06:45:09.798559 fixme-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-10 06:44:55.000000 fixme-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.794559 fixme-0.3/fixme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 06:44:55.000000 fixme-0.3/fixme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 06:44:55.000000 fixme-0.3/fixme/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-04-10 06:44:55.000000 fixme-0.3/fixme/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-10 06:44:55.000000 fixme-0.3/fixme/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 06:44:55.000000 fixme-0.3/fixme/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.798559 fixme-0.3/fixme/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/diagnose_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/fix_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/gather_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/generate_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-10 06:44:55.000000 fixme-0.3/fixme/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-10 06:44:55.000000 fixme-0.3/fixme/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.798559 fixme-0.3/fixme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-10 06:44:55.000000 fixme-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 06:45:09.802559 fixme-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-10 06:44:55.000000 fixme-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.798559 fixme-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 06:44:55.000000 fixme-0.3/tests/test_fixme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:05:28.041633 fixme-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 22:05:04.000000 fixme-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-10 22:05:28.041633 fixme-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-10 22:05:04.000000 fixme-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:05:28.037633 fixme-0.4/fixme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:05:04.000000 fixme-0.4/fixme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 22:05:04.000000 fixme-0.4/fixme/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-10 22:05:04.000000 fixme-0.4/fixme/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-10 22:05:04.000000 fixme-0.4/fixme/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 22:05:04.000000 fixme-0.4/fixme/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:05:28.041633 fixme-0.4/fixme/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:05:04.000000 fixme-0.4/fixme/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-10 22:05:04.000000 fixme-0.4/fixme/prompts/diagnose_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-10 22:05:04.000000 fixme-0.4/fixme/prompts/fix_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-10 22:05:04.000000 fixme-0.4/fixme/prompts/gather_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 22:05:04.000000 fixme-0.4/fixme/prompts/generate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 22:05:04.000000 fixme-0.4/fixme/prompts/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-04-10 22:05:04.000000 fixme-0.4/fixme/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-10 22:05:04.000000 fixme-0.4/fixme/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:05:28.041633 fixme-0.4/fixme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-10 22:05:28.000000 fixme-0.4/fixme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 22:05:28.000000 fixme-0.4/fixme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:05:28.000000 fixme-0.4/fixme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 22:05:28.000000 fixme-0.4/fixme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 22:05:28.000000 fixme-0.4/fixme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 22:05:28.000000 fixme-0.4/fixme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-10 22:05:04.000000 fixme-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 22:05:28.041633 fixme-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-10 22:05:04.000000 fixme-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:05:28.041633 fixme-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 22:05:04.000000 fixme-0.4/tests/test_fixme.py
```

### Comparing `fixme-0.3/LICENSE` & `fixme-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fixme-0.3/PKG-INFO` & `fixme-0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixme
-Version: 0.3
+Version: 0.4
 Summary: Use AI to automatically fix bugs
 Home-page: https://github.com/helloworld/fixme
 Author: helloworld
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/helloworld/fixme/issues
 Project-URL: CI, https://github.com/helloworld/fixme/actions
 Project-URL: Changelog, https://github.com/helloworld/fixme/releases
@@ -16,15 +16,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # fixme
 
 [![PyPI](https://img.shields.io/pypi/v/fixme.svg)](https://pypi.org/project/fixme/)
 [![Changelog](https://img.shields.io/github/v/release/helloworld/fixme?include_prereleases&label=changelog)](https://github.com/helloworld/fixme/releases)
-[![Tests](https://github.com/helloworld/fixme/workflows/Test/badge.svg)](https://github.com/helloworld/fixme/actions?query=workflow%3ATest)
+[![Tests](https://github.com/helloworld/fixme/actions/workflows/test.yml/badge.svg)](https://github.com/helloworld/fixme/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/helloworld/fixme/blob/master/LICENSE)
 
 Use AI to automatically fix bugs
 
 ## Installation
 
 Install this tool using `pip`:
```

### Comparing `fixme-0.3/README.md` & `fixme-0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # fixme
 
 [![PyPI](https://img.shields.io/pypi/v/fixme.svg)](https://pypi.org/project/fixme/)
 [![Changelog](https://img.shields.io/github/v/release/helloworld/fixme?include_prereleases&label=changelog)](https://github.com/helloworld/fixme/releases)
-[![Tests](https://github.com/helloworld/fixme/workflows/Test/badge.svg)](https://github.com/helloworld/fixme/actions?query=workflow%3ATest)
+[![Tests](https://github.com/helloworld/fixme/actions/workflows/test.yml/badge.svg)](https://github.com/helloworld/fixme/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/helloworld/fixme/blob/master/LICENSE)
 
 Use AI to automatically fix bugs
 
 ## Installation
 
 Install this tool using `pip`:
```

### Comparing `fixme-0.3/fixme/api.py` & `fixme-0.4/fixme/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from abc import ABC, abstractmethod
-from enum import Enum
-from typing import Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import openai
 from pydantic import BaseModel
 
 from fixme.prompts.diagnose_issue import diagnose_issue_prompt
 from fixme.prompts.gather_information import gather_information_prompt
 from fixme.prompts.generate_patch import generate_patch_prompt
@@ -26,30 +25,22 @@
 class GatherContextResponse(BaseModel):
     debug: Optional[DebugInformation]
     gather_context_commands: List[Tuple[str, str]]
 
 
 class DiagnoseIssueResponse(BaseModel):
     debug: Optional[DebugInformation]
-    issue_diagnosis: str
+    issue_diagnosis_stream: Any
 
 
 class GeneratePatchResponse(BaseModel):
     debug: Optional[DebugInformation]
     patch: str
 
 
-class Mode(Enum):
-    CHAT = "chat"
-    COMPLETION = "completion"
-
-
-MODE: Mode = Mode.CHAT
-
-
 class API(ABC):
     @abstractmethod
     def request_completion(self, prompt: str, max_tokens: int = 1024) -> str:
         pass
 
     @abstractmethod
     def gather_context(
@@ -71,50 +62,37 @@
         gathered_context: List[Tuple[str, str]],
         issue_diagnosis: str,
     ) -> GeneratePatchResponse:
         pass
 
 
 class OpenAIAPI(API):
-    def __init__(self, api_key):
+    def __init__(self, api_key, model):
         self._api_key = api_key
+        self._model = model
 
-    def request_completion(self, prompt, max_tokens=1024, print_prompt=False):
+    def request_completion(self, prompt, stream=False):
         def _request_chatgpt(prompt):
             response = openai.ChatCompletion.create(
-                model="gpt-4",
+                model=self._model,
                 messages=[
                     {
                         "role": "system",
                         "content": prompt["system_prompt"],
                     },
                     {"role": "user", "content": prompt["user_prompt"]},
                 ],
+                stream=stream,
             )
+            if stream:
+                return response
+            else:
+                return response.choices[0]["message"]["content"].strip()
 
-            return response.choices[0]["message"]["content"].strip()
-
-        def _request_davinci(prompt):
-            response = openai.Completion.create(
-                engine="text-davinci-003",
-                prompt=prompt,
-                max_tokens=max_tokens,
-                n=1,
-                stop=None,
-                temperature=0.7,
-            )
-
-            return response.choices[0].text.strip()
-
-        if MODE == Mode.CHAT:
-            return _request_chatgpt(prompt)
-        elif MODE == Mode.COMPLETION:
-            return _request_davinci(prompt)
-        else:
-            raise ValueError(f"Unknown mode for request_completion: {MODE}")
+        return _request_chatgpt(prompt)
 
     def gather_context(
         self,
         command_context: CommandContext,
     ) -> GatherContextResponse:
         debug = True
 
@@ -156,23 +134,19 @@
         prompt = diagnose_issue_prompt(
             command=command_context.command,
             stdout=command_context.stdout,
             stderr=command_context.stderr,
             cwd=command_context.cwd,
             gathered_context=gathered_context,
         )
-        issue_diagnosis = self.request_completion(prompt)
+        issue_diagnosis_stream = self.request_completion(prompt, stream=True)
 
         return DiagnoseIssueResponse(
-            issue_diagnosis=issue_diagnosis,
-            debug=(
-                DebugInformation(prompt=prompt, response=issue_diagnosis)
-                if debug
-                else None
-            ),
+            issue_diagnosis_stream=issue_diagnosis_stream,
+            debug=(DebugInformation(prompt=prompt, response=None) if debug else None),
         )
 
     def generate_patch(
         self,
         command_context: CommandContext,
         gathered_context: List[Tuple[str, str]],
         issue_diagnosis: str,
```

### Comparing `fixme-0.3/fixme/cli.py` & `fixme-0.4/fixme/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,24 @@
 @click.version_option()
 @click.argument(
     "full_command",
     nargs=-1,  # Accepts any number of arguments
     type=click.UNPROCESSED,  # Keeps the raw input format
     required=False,
 )
+@click.option(
+    "--model",
+    "-m",
+    "model",
+    default="gpt-4",
+    help="The chat model to use for the AI. Defaults to gpt-4. See https://beta.openai.com/docs/api-reference/models for more information.",
+)
 @click.pass_context
 @require_api_key
-def cli(ctx: click.Context, full_command: str, openai_api_key: str):
+def cli(ctx: click.Context, full_command: str, model: str, openai_api_key: str):
     if ctx.invoked_subcommand is not None:
         return
 
     if not full_command:
         click.echo(ctx.command.get_help(ctx))
         ctx.exit()
 
@@ -68,15 +75,18 @@
             console.print("\n")
             return stdout.read().decode()
 
     with tempfile.NamedTemporaryFile(
         delete=False
     ) as stdout, tempfile.NamedTemporaryFile(delete=False) as stderr:
         process = subprocess.Popen(
-            full_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
+            full_command_joined,
+            shell=True,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
         )
 
         print_labels = False
         if process.stdout and process.stderr:
             print_labels = True
 
         if process.stdout:
@@ -93,15 +103,15 @@
                 label="stderr" if print_labels else None,
             )
 
         process.wait()
 
     cwd = subprocess.check_output("pwd", shell=True).decode().strip()
 
-    client = OpenAIAPI(api_key=openai_api_key)
+    client = OpenAIAPI(api_key=openai_api_key, model=model)
     session = Session(
         fixme_client=client,
         command=full_command_joined,
         stdout=stdout_contents,
         stderr=stderr_contents,
         cwd=cwd,
     )
```

### Comparing `fixme-0.3/fixme/prompts/diagnose_issue.py` & `fixme-0.4/fixme/prompts/diagnose_issue.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def diagnose_issue_prompt(command, stdout, stderr, cwd, gathered_context):
     user_prompt = f"""{command_prompt(command, stdout, stderr, cwd)}
 
 Here is some extra information I gathered:
 
 {gathered_context_message(gathered_context)}
 
-Diagnose the issue based on the information I have gathered and explain the issue step by step in detail.
+Diagnose the issue based on the information I have gathered and explain the issue step by step in detail. Be as concise as possible.
 
 Here is the issue diagnosis:"""
 
     return {
         "system_prompt": system_prompt,
         "user_prompt": user_prompt,
     }
```

### Comparing `fixme-0.3/fixme/prompts/gather_information.py` & `fixme-0.4/fixme/prompts/gather_information.py`

 * *Files identical despite different names*

### Comparing `fixme-0.3/fixme/prompts/generate_patch.py` & `fixme-0.4/fixme/prompts/generate_patch.py`

 * *Files identical despite different names*

### Comparing `fixme-0.3/fixme/prompts/helpers.py` & `fixme-0.4/fixme/prompts/helpers.py`

 * *Files identical despite different names*

### Comparing `fixme-0.3/fixme/session.py` & `fixme-0.4/fixme/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import re
 import subprocess
 import tempfile
 
+from rich.live import Live
 from rich.panel import Panel
+from rich.text import Text
 
 from fixme.api import API, CommandContext
 from fixme.console import console, mark_step
-from fixme.utils import memoize_function_to_disk
 
 
 class Session:
     def __init__(self, fixme_client, command, stdout, stderr, cwd):
         self._api_client: API = fixme_client
         self._command_context = CommandContext(
             command=command, stdout=stdout, stderr=stderr, cwd=cwd
@@ -61,15 +62,14 @@
         if "debug" in response and response["debug"]:
             prompt = response["debug"]["prompt"]
             response = response["debug"]["response"]
 
             _print_prompt(prompt, header)
             _print_response(response, header)
 
-    @memoize_function_to_disk
     def _gather_context_request(self):
         return self._api_client.gather_context(
             command_context=self._command_context,
         )
 
     def gather_context(self):
         mark_step("Gathering context...")
@@ -83,51 +83,69 @@
                 gathered_context.append((message, output))
             else:
                 gathered_context.append((message, output))
 
         console.print("\n")
         return gathered_context
 
-    @memoize_function_to_disk
     def _diagnose_issue_request(self, gathered_context):
         return self._api_client.diagnose_issue(
             command_context=self._command_context,
             gathered_context=gathered_context,
         )
 
     def _parse_patch(self, patch):
-        code_block = re.search(r"```diff(.*)```", patch, re.DOTALL)
+        code_block = re.search(r"```diff(.*?)```", patch, re.DOTALL)
         if code_block:
-            patch = code_block.group(1).splitlines()[1:]
+            patch = code_block.group(1).strip().splitlines()[1:]
             patch = [line for line in patch if not re.match(r"index \w+\.\.\w+", line)]
             return "\n".join(patch)
         else:
             return None
 
+    def _clean_patch(self, patch):
+        return patch
+
     def _validate_patch(self, patch, retries=0, max_retries=5):
         with tempfile.NamedTemporaryFile(mode="w", delete=False) as f:
             f.write(patch)
             f.flush()
             patch_file = f.name
 
             mark_step("Validating patch...")
             try:
                 subprocess.run(
                     f"git apply --check {patch_file}", shell=True, check=True
                 )
-                return True, patch
+                return True
 
             except subprocess.CalledProcessError:
-                return False, patch
+                return False
 
     def diagnose_issue(self, gathered_context):
         mark_step("Diagnosing issue...")
         response = self._diagnose_issue_request(gathered_context=gathered_context)
-        issue_diagnosis = response.issue_diagnosis
-        self._print_output(issue_diagnosis, header="Issue Diagnosis")
+        issue_diagnosis_stream = response.issue_diagnosis_stream
+
+        issue_diagnosis = ""
+        with Live(auto_refresh=False) as live:
+            for chunk in issue_diagnosis_stream:
+                if "content" not in chunk["choices"][0]["delta"]:
+                    continue
+                message_content = chunk["choices"][0]["delta"]["content"]
+                issue_diagnosis += message_content
+                live.update(
+                    Panel.fit(
+                        Text(issue_diagnosis),
+                        title="Issue Diagnosis",
+                        border_style="green",
+                    )
+                )
+                live.refresh()
+
         return issue_diagnosis
 
     def _generate_patch_request(self, gathered_context, issue_diagnosis):
         return self._api_client.generate_patch(
             command_context=self._command_context,
             gathered_context=gathered_context,
             issue_diagnosis=issue_diagnosis,
@@ -148,17 +166,18 @@
 
         mark_step("Generating patch...")
         response = self._generate_patch_request(
             gathered_context=gathered_context, issue_diagnosis=issue_diagnosis
         )
         patch = response.patch
         parsed_patch = self._parse_patch(patch)
-        self._print_output(parsed_patch, header="Patch")
+        cleaned_patch = self._clean_patch(parsed_patch)
+        self._print_output(cleaned_patch, header="Patch")
 
-        is_patch_valid, patch = self._validate_patch(parsed_patch)
+        is_patch_valid = self._validate_patch(cleaned_patch)
         if not is_patch_valid:
             console.print(
                 Panel.fit(
                     (
                         "Patch is invalid. Trying again. Attempt"
                         f" {attempts + 1}/{max_attempts}."
                     ),
@@ -178,15 +197,15 @@
                 Panel.fit(
                     "Patch is valid!.",
                     title="Success",
                     border_style="green",
                 ),
             )
 
-        return patch
+        return cleaned_patch
 
     def apply_patch(self, patch):
         mark_step("Applying patch...")
         with tempfile.NamedTemporaryFile(mode="w", delete=False) as f:
             f.write(patch)
             f.flush()
             patch_file = f.name
```

### Comparing `fixme-0.3/fixme/utils.py` & `fixme-0.4/fixme/utils.py`

 * *Files identical despite different names*

### Comparing `fixme-0.3/fixme.egg-info/PKG-INFO` & `fixme-0.4/fixme.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixme
-Version: 0.3
+Version: 0.4
 Summary: Use AI to automatically fix bugs
 Home-page: https://github.com/helloworld/fixme
 Author: helloworld
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/helloworld/fixme/issues
 Project-URL: CI, https://github.com/helloworld/fixme/actions
 Project-URL: Changelog, https://github.com/helloworld/fixme/releases
@@ -16,15 +16,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # fixme
 
 [![PyPI](https://img.shields.io/pypi/v/fixme.svg)](https://pypi.org/project/fixme/)
 [![Changelog](https://img.shields.io/github/v/release/helloworld/fixme?include_prereleases&label=changelog)](https://github.com/helloworld/fixme/releases)
-[![Tests](https://github.com/helloworld/fixme/workflows/Test/badge.svg)](https://github.com/helloworld/fixme/actions?query=workflow%3ATest)
+[![Tests](https://github.com/helloworld/fixme/actions/workflows/test.yml/badge.svg)](https://github.com/helloworld/fixme/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/helloworld/fixme/blob/master/LICENSE)
 
 Use AI to automatically fix bugs
 
 ## Installation
 
 Install this tool using `pip`:
```

### Comparing `fixme-0.3/fixme.egg-info/SOURCES.txt` & `fixme-0.4/fixme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixme-0.3/pyproject.toml` & `fixme-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fixme-0.3/setup.py` & `fixme-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import find_packages, setup
 
-VERSION = "0.3"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

