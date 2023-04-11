# Comparing `tmp/chatcli_gpt-0.3.2.tar.gz` & `tmp/chatcli_gpt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcli_gpt-0.3.2.tar", max compression
+gzip compressed data, was "chatcli_gpt-0.4.0.tar", max compression
```

## Comparing `chatcli_gpt-0.3.2.tar` & `chatcli_gpt-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.3.2/LICENSE
--rw-r--r--   0        0        0     3388 2023-04-02 09:27:22.992169 chatcli_gpt-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.3.2/chatcli_gpt/__init__.py
--rw-r--r--   0        0        0       34 2023-03-26 16:42:54.474450 chatcli_gpt-0.3.2/chatcli_gpt/__main__.py
--rw-r--r--   0        0        0    14029 2023-04-02 08:51:29.376930 chatcli_gpt-0.3.2/chatcli_gpt/chatcli.py
--rw-r--r--   0        0        0     6453 2023-03-30 21:34:59.294322 chatcli_gpt-0.3.2/chatcli_gpt/log.py
--rw-r--r--   0        0        0     1940 2023-03-31 09:14:14.767161 chatcli_gpt-0.3.2/chatcli_gpt/plugins.py
--rw-r--r--   0        0        0      915 2023-04-02 09:28:59.444863 chatcli_gpt-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 chatcli_gpt-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3498 2023-04-10 16:46:32.407744 chatcli_gpt-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.4.0/chatcli_gpt/__init__.py
+-rw-r--r--   0        0        0       34 2023-03-26 16:42:54.474450 chatcli_gpt-0.4.0/chatcli_gpt/__main__.py
+-rw-r--r--   0        0        0    14346 2023-04-11 14:13:07.411332 chatcli_gpt-0.4.0/chatcli_gpt/chatcli.py
+-rw-r--r--   0        0        0     7808 2023-04-11 13:59:19.090439 chatcli_gpt-0.4.0/chatcli_gpt/log.py
+-rw-r--r--   0        0        0     2847 2023-04-11 13:20:15.453209 chatcli_gpt-0.4.0/chatcli_gpt/plugins.py
+-rw-r--r--   0        0        0      915 2023-04-11 13:13:54.910005 chatcli_gpt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4651 1970-01-01 00:00:00.000000 chatcli_gpt-0.4.0/PKG-INFO
```

### Comparing `chatcli_gpt-0.3.2/LICENSE` & `chatcli_gpt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.3.2/README.md` & `chatcli_gpt-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 pip install chatcli-gpt
 ```
 
 ### Running chatcli
 
 2. Initialise the log:
 
+By default it would save logs in ".chatcli.log", could override by setting environment variable `CHATCLI_LOGFILE`.
+
+
 ```
 chatcli init
 ```
 
-3. Set your OpenAI API key in the environment variable `OPENAI_API_SECRET_KEY`.
+3. Set your OpenAI API key in the environment variable `OPENAI_API_KEY`.
 
 4. Run chatcli
 
 ```
 chatcli
 ```
```

### Comparing `chatcli_gpt-0.3.2/chatcli_gpt/chatcli.py` & `chatcli_gpt-0.4.0/chatcli_gpt/chatcli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import openai
 import prompt_toolkit
 import tiktoken
 
 from .log import (
     write_log,
     search_conversations,
-    get_logged_conversation,
     conversation_log,
-    convert_log,
     create_initial_log,
 )
 from .plugins import evaluate_plugins
 
 MODELS = [
     "gpt-4",
     "gpt-3.5-turbo",
@@ -33,26 +31,27 @@
 }
 
 USAGE_COSTS = {
     "gpt-3.5-turbo": {"prompt_tokens": 0.002, "completion_tokens": 0.002},
     "gpt-4": {"prompt_tokens": 0.03, "completion_tokens": 0.06},
 }
 
+
 @click.group(cls=DefaultGroup, default="chat", default_if_no_args=True)
 @click.version_option()
 def cli():
     pass
 
 
 def cli_search_options(command):
-    @click.option("-n", "--offset", type=int, help="Message offset")
+    @click.argument("offset", type=int, required=False)
     @click.option("-s", "--search", help="Select by search term")
     @click.option("-t", "--tag", help="Select by tag")
     @functools.wraps(command)
-    def wrapper(*args, offset=None, search=None, tag=None, **kwargs):
+    def wrapper(offset, *args, search=None, tag=None, **kwargs):
         return command(
             *args,
             search_options={"offset": offset, "search": search, "tag": tag},
             **kwargs,
         )
 
     return wrapper
@@ -73,15 +72,15 @@
     "--file",
     type=click.Path(exists=True),
     multiple=True,
     help="Add a file to the conversation for context.",
 )
 @click.option("-r", "--retry", is_flag=True, help="Retry previous question")
 @click.option("--stream/--sync", default=True, help="Stream or sync mode.")
-@click.option("--model", type=click.Choice(MODELS), default="gpt-3.5-turbo")
+@click.option("--model", type=click.Choice(MODELS))
 @click.option("--plugin", "additional_plugins", multiple=True, help="Load a plugin.")
 @cli_search_options
 def chat(quick, continue_conversation, personality, file, retry, stream, model, additional_plugins, search_options):
     if (continue_conversation or retry) and not search_options["offset"]:
         search_options["offset"] = 1
     elif personality and not search_options["tag"] and not search_options["search"] and not search_options["offset"]:
         search_options["tag"] = "^" + personality
@@ -104,14 +103,16 @@
         tags_to_apply = [tags[-1]]
     else:
         tags_to_apply = []
 
     plugins = conversation["plugins"]
     plugins.extend(additional_plugins)
 
+    model = model or conversation["model"] or "gpt-3.5-turbo"
+
     if retry:
         response = answer(request_messages[:-1], model, plugins, stream=stream, tags=tags_to_apply)
         if not quick:
             request_messages.append(response)
             run_conversation(request_messages, model, plugins, stream=stream, tags=tags_to_apply)
     elif quick or not os.isatty(0):
         run_conversation(
@@ -129,69 +130,70 @@
 
 @cli.command(help="Create initial conversation log.")
 @click.option("-r", "--reinit", is_flag=True, help="re-initialize the personalities to default values")
 def init(reinit):
     try:
         create_initial_log(reinit)
     except FileExistsError as error:
-        click.echo(f"{error}: Conversation log already exists.")
+        click.echo(f"{error}: Conversation log already exists.", file=sys.stderr)
         sys.exit(1)
 
 
 @cli.command(help="Add a message to a new or existing conversation.")
 @click.option("--multiline/--singleline", default=True)
 @click.option("-p", "--personality")
 @click.option("--role", type=click.Choice(["system", "user", "assistant"]), default="system")
 @click.option("--plugin", multiple="True", help="Activate plugins.")
+@click.option("--model", type=click.Choice(MODELS), default="gpt-3.5-turbo")
 @cli_search_options
-def add(personality, role, plugin, multiline, search_options):
+def add(personality, role, plugin, multiline, search_options, model):
     if any(search_options.values()):
         conversation = get_logged_conversation(**search_options)
         messages = conversation["messages"]
     else:
         messages = []
 
     tags = []
     if personality:
         tags.append("^" + personality)
 
     if multiline and os.isatty(0):
         click.echo("(Finish input with <Alt-Enter> or <Esc><Enter>)")
     description = prompt(multiline=True)
     messages.append({"role": role, "content": description})
-    write_log(messages=messages, tags=tags, plugins=plugin)
+    write_log(messages=messages, tags=tags, plugins=plugin, model=model)
 
 
 @cli.command(help="List tags.", name="tags")
 def list_tags():
     tags = set()
     for conversation in conversation_log():
         for tag in conversation.get("tags", []):
             tags.add(tag)
     for tag in sorted(tags):
         click.echo(tag)
 
 
 @cli.command(help="Add tags to an conversation.", name="tag")
+@click.argument("tag")
 @cli_search_options
-@click.argument("tags", nargs=-1)
-def add_tag(tags, search_options):
+def add_tag(tag, search_options):
     conversation = get_logged_conversation(**search_options)
-    new_tags = [tag for tag in conversation.get("tags", []) if tag not in tags]
-    new_tags.extend(tags)
+    new_tags = [t for t in conversation.get("tags", []) if t != tag]
+    new_tags.append(tag)
 
     write_log(messages=conversation["messages"], tags=new_tags)
 
 
 @cli.command(help="Remove tags from an conversation.")
+@click.argument("tag")
 @cli_search_options
-@click.argument("tags", nargs=-1)
-def untag(tags, search_options):
+def untag(tag, search_options):
     conversation = get_logged_conversation(**search_options)
-    new_tags = [t for t in conversation.get("tags", []) if t not in tags]
+    new_tags = [t for t in conversation.get("tags", []) if t != tag]
     write_log(messages=conversation["messages"], tags=new_tags)
 
 
 @cli.command(help="Current tag")
 @cli_search_options
 def show_tag(search_options):
     conversation = get_logged_conversation(**search_options)
@@ -224,21 +226,22 @@
 
 @cli.command(help="List all the questions we've asked")
 @cli_search_options
 @click.option("-l", "--limit", type=int, help="Limit number of results")
 @click.option("-u", "--usage", is_flag=True, help="Show token usage")
 @click.option("--cost", is_flag=True, help="Show token cost")
 @click.option("--plugins", is_flag=True, help="Show enabled plugins")
-def log(limit, usage, cost, plugins, search_options):
+@click.option("--model", is_flag=True, help="Show model")
+def log(limit, usage, cost, plugins, search_options, model):
     for offset, conversation in reversed(list(itertools.islice(search_conversations(**search_options), limit))):
         try:
             question = find_recent_message(lambda message: message["role"] != "assistant", conversation)["content"]
         except ValueError:
             question = conversation["messages"][-1]["content"]
-        trimmed_message = question.split("\n", 1)[0][:80]
+        trimmed_message = question.strip().split("\n", 1)[0][:80]
 
         fields = []
         offset = click.style(f"{offset: 4d}:", fg="blue")
         fields.append(offset)
 
         if usage:
             if conversation["usage"]:
@@ -253,30 +256,18 @@
         fields.append(trimmed_message)
         if conversation.get("tags"):
             fields.append(click.style(f"{','.join(conversation['tags'])}", fg="green"))
 
         if plugins:
             fields.append(f"{','.join(conversation['plugins'])}")
 
-        click.echo(" ".join(fields))
-
+        if model:
+            fields.append(click.style(f"{conversation['model']}", fg="yellow"))
 
-@cli.command(
-    help="""Convert old chatlog format to new format.
-    Recommended usage:
-
-    \b
-    cp -i .chatcli.log .chatcli.log.bak
-    chatlog convert .chatcli.log.bak > .chatcli.log
-    """
-)
-@click.argument("filename", type=click.Path(exists=True))
-def convert(filename):
-    for line in convert_log(filename):
-        print(line)
+        click.echo(" ".join(fields))
 
 
 def run_conversation(request_messages, model, plugins, tags=None, stream=True, multiline=True, quick=False):
     if multiline and os.isatty(0):
         click.echo("(Finish input with <Alt-Enter> or <Esc><Enter>)")
 
     while True:
@@ -349,24 +340,29 @@
 
 def answer(request_messages, model, plugins, stream=True, tags=None):
     if stream:
         completion = stream_request(request_messages, model)
     else:
         completion = synchroneous_request(request_messages, model)
 
+    # TODO: handle multiple choices
     response_message = completion["choices"][0]["message"]
 
     write_log(
         messages=request_messages + [response_message],
         completion=completion,
         usage=completion_usage(request_messages, model, completion),
         tags=tags,
         plugins=plugins,
+        model=model,
     )
 
+    # TODO:
+    # - [ ] wrote more plugins and see what's good interface for plugins
+    # - [ ] middleware pattern for plugins
     if plugins:
         plugin_response = evaluate_plugins(response_message["content"], plugins)
 
         if plugin_response:
             request_messages.append(response_message)
             request_messages.append({"role": "user", "content": plugin_response})
             click.echo(click.style(plugin_response, fg=(200, 180, 90)))
@@ -416,17 +412,26 @@
     tokens = sum(conversation["usage"]["total_tokens"] for conversation in conversations if conversation["usage"])
 
     total_cost = sum(conversation_cost(conversation) for conversation in conversations)
     click.echo(f"Tokens: {tokens}")
     click.echo(f"Cost: ${total_cost:.2f}")
 
 
+def get_logged_conversation(offset, search=None, tag=None):
+    try:
+        return next(search_conversations(offset, search, tag))[1]
+    except StopIteration:
+        click.echo("Matching conversation not found", file=sys.stderr)
+        sys.exit(1)
+
+
+
 def main():
     try:
         cli()
     except FileNotFoundError as error:
-        click.echo(f"{error}: Chatlog not initialized. Run `chatlog init` first.")
+        click.echo(f"{error}: Chatcli not initialized. Run `chatcli init` first.")
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatcli_gpt-0.3.2/chatcli_gpt/log.py` & `chatcli_gpt-0.4.0/chatcli_gpt/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
-import os.path
+import sys
+import shutil
+from pathlib import Path
 import datetime
 import json
 from textwrap import dedent
 
 INITIAL_PERSONALITIES = {
     "concise": {
         "content": "You are a helpful, expert linux user and programmer. You give concise answers, providing code where possible.",
@@ -13,14 +15,15 @@
         "content": """
                 You generate commit messages from diffs. Every line of commit message should be less than eighty characters.
                 You never output anything that does not belong in the commit message.
                 """,
     },
     "pyeval": {
         "plugins": ["pyeval"],
+        "model": "gpt-4",
         "content": """
                 You can evaluate code by returning any python code in a code block with the line "EVALUATE:" before it.
                 Do you not attempt to compute expressions, or the results of python code yourself, instead use an EVALUATE block.
                 You will get the result of running the code you provide in a result block.
 
                 For example:
 
@@ -38,85 +41,125 @@
                 as the next message.
 
                 Use the result to help you answer the question.
             """,
     },
     "search": {
         "plugins": ["search"],
+        "model": "gpt-4",
         "content": """
             You can search the internet by returning query in the form SEARCH("query")
             Whenever you are asked a question, you should first search the internet for an answer.
             Search the internet by using the search command:
 
             For example:
 
             SEARCH("president of the united states")
 
             Use the result to help you answer the question.
 
             Run additional queries as necessary to answer further questions.
         """,
     },
+    "bash": {
+        "plugins": ["bash"],
+        "model": "gpt-4",
+        "content": """
+            You can evaluate bash code by returning any bash code in a code block with the line "EVALUATE:" before it.
+
+            Here is an example:
+
+            You reply:
+
+            EVALUATE:
+            ```bash
+            echo "hello world!"
+            ```
+
+            You would receive:
+
+            RESULT:
+            ```
+            hello world!
+            ```
+            Answer questions about by running commands and using the results you receive.
+        """,
+    },
 }
 
 CHAT_LOG = os.environ.get("CHATCLI_LOGFILE", ".chatcli.log")
 
 
-def write_log(messages, completion=None, usage=None, tags=None, plugins=None, path=None):
+def write_log(messages, completion=None, usage=None, tags=None, plugins=None, path=None, model=None):
     assert isinstance(messages, list)
     assert isinstance(tags, list) or tags is None
     assert isinstance(completion, dict) or completion is None
     assert isinstance(usage, dict) or usage is None
     assert isinstance(plugins, (list, tuple)) or plugins is None
+    assert isinstance(model, str) or model is None
     timestamp = datetime.datetime.now().isoformat()
 
     path = path or find_log()
 
     with open(path, "a", buffering=1, encoding="utf-8") as fh:
         fh.write(
             json.dumps(
                 {
                     "messages": messages,
                     "completion": completion,
                     "usage": usage,
                     "tags": tags or [],
                     "timestamp": timestamp,
                     "plugins": plugins or [],
+                    "model": model,
                 }
             )
             + "\n"
         )
 
 
 def create_initial_log(reinit):
-    if not reinit and os.path.exists(CHAT_LOG):
+    if not reinit and Path(CHAT_LOG).exists():
         raise FileExistsError(CHAT_LOG)
 
     for key, value in INITIAL_PERSONALITIES.items():
         write_log(
             messages=[{"role": "system", "content": dedent(value["content"].strip())}],
             tags=["^" + key],
             plugins=value.get("plugins"),
+            model=value.get("model"),
             path=CHAT_LOG,
         )
 
 
 def conversation_log():
     log_path = find_log()
-    with open(log_path, encoding="utf-8") as fh:
+    with log_path.open(encoding="utf-8") as fh:
+        line = json.loads(fh.readline())
+        version = line.get("version")
+        if version is None:
+            fh.close()
+            lines = list(convert_log_pre_0_4(log_path))
+            backup_file = log_path.with_suffix(".log.bak.0_3")
+            sys.stderr.write(f"Upgrading log file. Making backup in: {backup_file}\n")
+            shutil.copyfile(log_path, backup_file)
+            with log_path.open("w", encoding="utf-8") as fh:
+                fh.write(json.dumps({"version": "0.4"}) + "\n")
+                for line in lines:
+                    fh.write(line + "\n")
+            return [json.loads(line) for line in lines]
         return [json.loads(line) for line in fh]
 
 
 def find_log():
     path = CHAT_LOG
-    while not os.path.exists(path):
-        if os.path.dirname(os.path.abspath(path)) == "/":
-            raise FileNotFoundError(CHAT_LOG)
-        path = "../" + path
-    return path
+    for directory in Path(path).resolve().parents:
+        if (directory / path).exists():
+            return directory / path
+    raise FileNotFoundError(CHAT_LOG)
 
 
 def search_conversations(offset, search, tag):
     for idx, conversation in enumerate(reversed(conversation_log()), start=1):
         if offset and idx != offset:
             continue
 
@@ -128,19 +171,15 @@
         if search and search not in question:
             continue
         if tag and tag not in conversation.get("tags", []):
             continue
         yield idx, conversation
 
 
-def get_logged_conversation(offset, search=None, tag=None):
-    return next(search_conversations(offset, search, tag))[1]
-
-
-def convert_log(filename):
+def convert_log_pre_0_4(filename):
     with open(filename, "r", encoding="utf-8") as fh:
         for line in fh:
             data = json.loads(line)
 
             if "request" in data:
                 if data["response"]:
                     assistant_message = data["response"]["choices"][0]["message"]
@@ -182,9 +221,10 @@
             converted_data = {
                 "messages": messages,
                 "completion": completion,
                 "tags": tags,
                 "usage": usage,
                 "timestamp": timestamp,
                 "plugins": data.get("plugins", []),
+                "model": data.get("model"),
             }
             yield json.dumps(converted_data)
```

### Comparing `chatcli_gpt-0.3.2/chatcli_gpt/plugins.py` & `chatcli_gpt-0.4.0/chatcli_gpt/plugins.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,98 @@
 import re
 import io
 import sys
 import contextlib
 import ast
 import traceback
 import json
+import subprocess
 import duckduckgo_search
 
 
-BLOCK_PATTERNS = {"pyeval": r"EVALUATE:\n+```(?:python)?\n(.*?)```", "search": r"SEARCH\((.*)\)"}
+BLOCK_PATTERNS = {
+    "bash": r"EVALUATE:\n+```(?:bash)?\n(.*?)```",
+    "pyeval": r"EVALUATE:\n+```(?:python)?\n(.*?)```",
+    "search": r"SEARCH\((.*)\)",
+}
+
 
 def evaluate_plugins(response_text, plugins):
     active_plugin = plugins[0]
     blocks = extract_blocks(response_text, active_plugin)
     if not blocks:
         return None
     if active_plugin == "pyeval":
         output = exec_python(blocks[0])
+    elif active_plugin == "bash":
+        output = exec_bash(blocks[0])
     elif active_plugin == "search":
         search_term = blocks[0].strip()
         if search_term[0] in "\"'":
             search_term = ast.literal_eval(search_term)
         output = exec_duckduckgo(search_term)
     return format_block(output)
 
 
 def extract_blocks(response_text, plugin):
     block_pattern = BLOCK_PATTERNS[plugin]
     matches = re.findall(block_pattern, response_text, re.DOTALL)
     return matches
 
 
+def exec_bash(code):
+    try:
+        result = subprocess.run(["/bin/bash", "-c", code], capture_output=True, text=True)
+    except Exception:  # pylint: disable=broad-except
+        print(traceback.format_exc())
+
+    return {
+        "result": result.stdout.strip(),
+        "error": result.stderr.strip(),
+    }
+
+
 def exec_python(code):
-    buffer = io.StringIO()
+    stdout = io.StringIO()
+    stderr = io.StringIO()
 
-    with contextlib.redirect_stdout(buffer):
+    with contextlib.redirect_stdout(stdout), contextlib.redirect_stderr(stderr):
         global_scope = globals()
         try:
             mod = ast.parse(code, mode="exec")
             if isinstance(mod.body[-1], ast.Expr):
                 last_expr = mod.body.pop()
                 exec(compile(mod, "<ast>", "exec"), global_scope)
-                result = eval(compile(ast.Expression(last_expr.value), "<ast>", "eval"), global_scope)
+                result = eval(
+                    compile(ast.Expression(last_expr.value), "<ast>", "eval"),
+                    global_scope,
+                )
                 if result is not None:
                     print(result)
             else:
                 exec(code, global_scope)
         except Exception:  # pylint: disable=broad-except
             print(traceback.format_exc())
 
-    return buffer.getvalue().strip()
+    return {
+        "result": stdout.getvalue().strip(),
+        "error": stderr.getvalue().strip(),
+    }
 
 
 def exec_duckduckgo(search_term):
-    return json.dumps(duckduckgo_search.ddg(search_term, max_results=5))
+    return {"result": json.dumps(duckduckgo_search.ddg(search_term, max_results=5))}
 
 
+# TODO: Truncate the output to meet token requirement and save $$.
 def format_block(output):
-    formatted_output = f"RESULT:\n```\n{output}\n```"
-    return formatted_output
+    output_blocks = []
+    if output["result"]:
+        output_blocks.append(f"RESULT:\n```\n{output['result']}\n```")
+    if output["error"]:
+        output_blocks.append(f"ERROR:\n```\n{output['error']}\n```")
+    return "\n".join(output_blocks)
 
 
 if __name__ == "__main__":
     input_text = sys.stdin.read()
     print(evaluate_plugins(input_text, ["search"]))
```

### Comparing `chatcli_gpt-0.3.2/pyproject.toml` & `chatcli_gpt-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatcli-gpt"
-version = "0.3.2"
+version = "0.4.0"
 description = "A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations."
 readme = "README.md"
 license = "MIT"
 authors = ["Adam Kelly <adam@cthulahoops.org>"]
 repository = "https://github.com/cthulahoops/chatcli"
 
 [tool.poetry.dependencies]
```

### Comparing `chatcli_gpt-0.3.2/PKG-INFO` & `chatcli_gpt-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcli-gpt
-Version: 0.3.2
+Version: 0.4.0
 Summary: A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations.
 Home-page: https://github.com/cthulahoops/chatcli
 License: MIT
 Author: Adam Kelly
 Author-email: adam@cthulahoops.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -51,19 +51,22 @@
 pip install chatcli-gpt
 ```
 
 ### Running chatcli
 
 2. Initialise the log:
 
+By default it would save logs in ".chatcli.log", could override by setting environment variable `CHATCLI_LOGFILE`.
+
+
 ```
 chatcli init
 ```
 
-3. Set your OpenAI API key in the environment variable `OPENAI_API_SECRET_KEY`.
+3. Set your OpenAI API key in the environment variable `OPENAI_API_KEY`.
 
 4. Run chatcli
 
 ```
 chatcli
 ```
```

