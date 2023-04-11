# Comparing `tmp/chatgpt_prompt_wrapper-0.0.7.tar.gz` & `tmp/chatgpt_prompt_wrapper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_prompt_wrapper-0.0.7.tar", max compression
+gzip compressed data, was "chatgpt_prompt_wrapper-0.0.8.tar", max compression
```

## Comparing `chatgpt_prompt_wrapper-0.0.7.tar` & `chatgpt_prompt_wrapper-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11337 2023-04-10 15:06:55.587443 chatgpt_prompt_wrapper-0.0.7/LICENSE
--rw-r--r--   0        0        0    11848 2023-04-10 15:38:31.427438 chatgpt_prompt_wrapper-0.0.7/README.md
--rw-r--r--   0        0        0     2668 2023-04-10 15:41:05.027434 chatgpt_prompt_wrapper-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      113 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/__init__.py
--rw-r--r--   0        0        0       81 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/__version__.py
--rw-r--r--   0        0        0     3638 2023-04-10 15:32:05.457427 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/arg_parser.py
--rw-r--r--   0        0        0      133 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
--rw-r--r--   0        0        0     2414 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/ask.py
--rw-r--r--   0        0        0     6661 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chat.py
--rw-r--r--   0        0        0     7504 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
--rw-r--r--   0        0        0     5836 2023-04-10 15:15:17.007437 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
--rw-r--r--   0        0        0      106 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
--rw-r--r--   0        0        0      117 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/__init__.py
--rw-r--r--   0        0        0      854 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/commands.py
--rw-r--r--   0        0        0      355 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/cost.py
--rw-r--r--   0        0        0      442 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/init.py
--rw-r--r--   0        0        0     1410 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/config.py
--rw-r--r--   0        0        0     1490 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/docstring.py
--rw-r--r--   0        0        0     1403 2023-04-10 15:06:55.597443 chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/log_formatter.py
--rw-r--r--   0        0        0    13202 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-07 05:06:29.732833 chatgpt_prompt_wrapper-0.0.8/LICENSE
+-rw-r--r--   0        0        0    11989 2023-04-11 03:18:50.790208 chatgpt_prompt_wrapper-0.0.8/README.md
+-rw-r--r--   0        0        0     2704 2023-04-11 03:19:56.727892 chatgpt_prompt_wrapper-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-04-08 00:44:49.195989 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/__init__.py
+-rw-r--r--   0        0        0       81 2023-04-08 00:46:06.486873 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/__version__.py
+-rw-r--r--   0        0        0     3654 2023-04-11 02:53:38.594014 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/arg_parser.py
+-rw-r--r--   0        0        0      133 2023-04-09 10:56:36.068379 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/__init__.py
+-rw-r--r--   0        0        0     2414 2023-04-10 09:24:23.945045 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/ask.py
+-rw-r--r--   0        0        0     6673 2023-04-11 03:12:12.225520 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chat.py
+-rw-r--r--   0        0        0     7760 2023-04-11 03:10:48.348304 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py
+-rw-r--r--   0        0        0     7127 2023-04-11 03:02:08.687752 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py
+-rw-r--r--   0        0        0      106 2023-04-08 00:44:54.738169 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper_exception.py
+-rw-r--r--   0        0        0      117 2023-04-08 13:10:04.940242 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-09 15:44:22.008830 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/commands.py
+-rw-r--r--   0        0        0      355 2023-04-08 13:10:04.935293 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/cost.py
+-rw-r--r--   0        0        0      442 2023-04-08 12:08:28.972053 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/init.py
+-rw-r--r--   0        0        0     1410 2023-04-09 15:52:54.238316 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/config.py
+-rw-r--r--   0        0        0     1490 2023-04-10 01:24:32.721402 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/docstring.py
+-rw-r--r--   0        0        0     1403 2023-04-08 00:45:28.794147 chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/log_formatter.py
+-rw-r--r--   0        0        0    13379 1970-01-01 00:00:00.000000 chatgpt_prompt_wrapper-0.0.8/PKG-INFO
```

### Comparing `chatgpt_prompt_wrapper-0.0.7/LICENSE` & `chatgpt_prompt_wrapper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.7/README.md` & `chatgpt_prompt_wrapper-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 - `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the maximum values for the model. (default: 0)
 - `min_max_tokens`: The minimum of `max_tokens` for the completion when `max_tokens = 0`. (default: 200)
 - `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the maximum values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p at the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
+- Table of `alias`: Dictionary of role aliases. The default alias is: '`user' = 'User'`, `'system' = 'System'`, `'assistant' = 'Assistant'`.
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
 The options for ask mode:
 
 - `show`: Set `true` to show prompt for non chat command.
 - `hide`: Set `true` to hide prompt for non chat command (default).
```

### Comparing `chatgpt_prompt_wrapper-0.0.7/pyproject.toml` & `chatgpt_prompt_wrapper-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "chatgpt-prompt-wrapper"
-version = "0.0.7"
-description = ""
+version = "0.0.8"
+description = "CLI tool to wrap ChatGPT Python API."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 homepage = "https://github.com/rcmdnk/chatgpt-prompt-wrapper"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["chat", "gpt", "openai", "cli"]
 classifiers = ["Development Status :: 3 - Alpha", "Environment :: Console", "Intended Audience :: Developers", "Intended Audience :: End Users/Desktop", "License :: OSI Approved :: Apache Software License", "Natural Language :: English", "Operating System :: OS Independent", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic :: Communications :: Chat", "Topic :: Utilities"]
```

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/arg_parser.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/arg_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
-import sys
 from argparse import ArgumentParser, Namespace
 
-direct_chatgpt_params = [
-    "key",
-    "model",
-    "max_tokens",
-    "min_max_tokens",
-    "tokens_limit",
+true_false_params = [
+    ("show", "hide"),
+    ("multiline", "no_multiline"),
+    ("vi", "emacs"),
 ]
 
+true_params = ["show_cost"]
+
 
 def get_arg_parser() -> ArgumentParser:
     arg_parser = ArgumentParser()
     arg_parser.add_argument(
         "subcommand",
         help="Subcommand to run. Use 'commands' subcommand to list up available subcommands.",
         type=str,
@@ -87,29 +86,29 @@
         "--show_cost",
         help="Show cost used.",
         action="store_true",
     )
     return arg_parser
 
 
-def parse_arg() -> Namespace:
+def parse_args(argv: list[str]) -> Namespace:
     arg_parser = get_arg_parser()
     optional_strings: dict[str, int] = {}
     for action in arg_parser._actions:
         for s in action.option_strings:
             if isinstance(action.nargs, int):
                 optional_strings[s] = action.nargs
             elif action.nargs is None:
                 optional_strings[s] = 1
 
     positional = []
     option = []
     is_option = 0
     is_positional = False
-    for arg in sys.argv[1:]:
+    for arg in argv:
         if is_positional:
             positional.append(arg)
         elif is_option:
             option.append(arg)
             is_option -= 1
         elif arg == "--":
             is_positional = True
```

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/ask.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/ask.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chat.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         for message in messages:
             self.log.info(self.get_output(message, max_size))
 
         self.set_no_line_break_log()
         cost = 0.0
         self.finish_chat = False
         while True:
-            user = [("class:user", f"{'user':>{max_size}}> ")]
+            user = [("class:user", f"{self.alias['user']:>{max_size}}> ")]
             text = prompt(user, **self.prompt_params)  # type: ignore
             if self.finish_chat:
                 break
             message = {"role": "user", "content": text}
             if message["content"].lower() in self.chat_exit_cmd:
                 break
             message_tokens = self.num_tokens_from_message(message)
```

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt/chatgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p in the same time.
     presence_penalty: float
         The penalty for the model to return the same token (-2 ~ 2).
     frequency_penalty: float
         The penalty for the model to return the same token multiple times (-2 ~ 2).
     colors: dict[str, str]
         The colors to use for the different roles.
+    alias: dict[str, str]
+        The aliases of role names.
     """
 
     key: str
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 0
     min_max_tokens: int = 200
     tokens_limit: int = 0
@@ -54,14 +56,21 @@
     colors: dict[str, str] = field(
         default_factory=lambda: {
             "system": "blue",
             "user": "green",
             "assistant": "cyan",
         }
     )
+    alias: dict[str, str] = field(
+        default_factory=lambda: {
+            "system": "System",
+            "user": "User",
+            "assistant": "Assistant",
+        }
+    )
 
     def __post_init__(self) -> None:
         self.log = logging.getLogger(__name__)
         openai.api_key = self.key
         if self.max_tokens:
             self.min_max_tokens = self.max_tokens
 
@@ -178,15 +187,15 @@
         if "gpt-3.5" in self.model:
             for message in messages:
                 if message["role"] == "system":
                     message["role"] = "user"
         return messages
 
     def get_name(self, message: dict[str, str]) -> str:
-        name = message["role"]
+        name = self.alias[message["role"]]
         if "name" in message:
             if "gpt-3.5" in self.model:
                 name = message["name"]
             else:
                 name = f"{message['name']} ({message['role']})"
         return name
```

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/chatgpt_prompt_wrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,200 +1,219 @@
 from __future__ import annotations
 
 import inspect
 import json
-from argparse import Namespace
+import sys
+from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 from .__version__ import __version__
-from .arg_parser import cli_help, direct_chatgpt_params, parse_arg
-from .chatgpt import Ask, Chat, Messages
+from .arg_parser import cli_help, parse_args, true_false_params, true_params
+from .chatgpt import Ask, Chat
 from .chatgpt_prompt_wrapper_exception import ChatGPTPromptWrapperError
 from .cmd import commands, cost, init
 from .config import get_config
 from .log_formatter import get_logger
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib  # type: ignore
 
 
-log = get_logger(__name__.split(".")[0])
-
-
-def set_config_messages(config: dict[str, Any], args: Namespace) -> None:
-    if "messages" not in config:
-        config["messages"] = []
-    if args.message:
-        config["messages"].append(
-            {"role": "user", "content": " ".join(args.message)}
+@dataclass
+class ChatGPTPromptWrapper:
+    """ChatGPTPromptWrapper main class.
+
+    Parameters
+    ----------
+    argv : list[str] | None
+        Arguments to parse. If None, use sys.argv[1:]. It must have at least one positional argument as subcommand.
+    cmd_name : str
+        Command name.
+    config_file_name : str
+        Configuration TOML file name.
+    cost_file_name : str
+        Cost JSON file name.
+    """
+
+    argv: list[str] | None = None
+    cmd_name: str = "cg"
+    config_file_name: str = "config.toml"
+    cost_file_name: str = "cost.json"
+
+    def __post_init__(self) -> None:
+        self.log = get_logger(__name__.split(".")[0])
+
+        if self.argv is None:
+            self.argv = sys.argv[1:]
+        self.args = parse_args(self.argv)
+        self.cmd = self.args.subcommand[0]
+
+    def cmd_wo_config(self) -> bool:
+        if self.cmd == "help":
+            self.log.info(cli_help())
+            return True
+
+        if self.cmd == "version":
+            self.log.info(f"{__package__} {__version__}")
+            return True
+
+        return False
+
+    def cmd_wo_key(self) -> bool:
+        if self.cmd == "init":
+            init(self.config_file)
+            self.log.info(f"Created config file at {self.config_file}.")
+            return True
+
+        if self.cmd == "cost":
+            cost(self.cost_file, self.log)
+            return True
+        return False
+
+    def set_files(self) -> None:
+        self.config_file = (
+            Path(self.args.conf)
+            if self.args.conf
+            else get_config(self.cmd_name, self.config_file_name)
         )
+        self.cost_file = get_config(self.cmd_name, self.cost_file_name)
 
-
-def set_config_show(config: dict[str, Any], args: Namespace) -> None:
-    if "show" in config:
-        pass
-    elif "hide" in config:
-        config["show"] = not config["hide"]
-    if args.show:
-        config["show"] = True
-    elif args.hide:
-        config["show"] = False
-
-
-def set_config_multiline(config: dict[str, Any], args: Namespace) -> None:
-    if "multiline" in config:
-        pass
-    elif "no_multiline" in config:
-        config["multiline"] = not config["no_multiline"]
-    if args.multiline:
-        config["multiline"] = True
-    elif args.no_multiline:
-        config["multiline"] = False
-
-
-def set_config_vi(config: dict[str, Any], args: Namespace) -> None:
-    if "vi" in config:
-        pass
-    elif "emacs" in config:
-        config["vi"] = not config["emacs"]
-    if args.vi:
-        config["vi"] = True
-    elif args.emacs:
-        config["vi"] = False
-
-
-def get_show_cost(config: dict[str, Any], args: Namespace) -> bool:
-    show_cost = False
-    show_cost = config["show_cost"] if "show_cost" in config else False
-    if args.show_cost:
-        show_cost = True
-    return show_cost
-
-
-def check_args(
-    config: dict[str, Any], args: Namespace
-) -> tuple[dict[str, Any], Messages, bool, bool]:
-    set_config_messages(config, args)
-    set_config_show(config, args)
-    set_config_multiline(config, args)
-    set_config_vi(config, args)
-    show_cost = get_show_cost(config, args)
-    chat = config["chat"] if "chat" in config else False
-
-    for arg in vars(args):
-        if arg not in direct_chatgpt_params:
-            continue
-        if (param := getattr(args, arg)) is not None:
-            config[arg] = param
-
-    chatgpt_params = {
-        k: v
-        for k, v in config.items()
-        if k in direct_chatgpt_params + ["show", "multiline", "vi"]
-    }
-    if not chat and not config["messages"]:
-        raise ChatGPTPromptWrapperError(
-            "This subcommand (ask mode) does not predefined prompt and need input message."
+    def set_config_messages(self, config: dict[str, Any]) -> None:
+        if "messages" not in config:
+            config["messages"] = []
+        if self.args.message:
+            config["messages"].append(
+                {"role": "user", "content": " ".join(self.args.message)}
+            )
+
+    def set_ture_false_config(
+        self,
+        config: dict[str, Any],
+        true_value: str,
+        false_value: str | None = None,
+        default_value: bool | None = None,
+    ) -> None:
+        if default_value is not None:
+            config[true_value] = default_value
+
+        if true_value in config:
+            pass
+        elif false_value is not None and false_value in config:
+            config[true_value] = not config[false_value]
+
+        if getattr(self.args, true_value):
+            config[true_value] = True
+        elif false_value is not None and getattr(self.args, false_value):
+            config[true_value] = False
+
+    def update_cmd_config(self, config: dict[str, Any]) -> None:
+        self.set_config_messages(config)
+        for true_value, false_value in true_false_params:
+            self.set_ture_false_config(config, true_value, false_value)
+        for true_value in true_params:
+            self.set_ture_false_config(config, true_value, default_value=False)
+
+        config.update(
+            {
+                k: v
+                for k, v in vars(self.args).items()
+                if k
+                not in [x for y in true_false_params for x in y] + true_params
+                and v is not None
+            }
         )
-    return chatgpt_params, config["messages"], chat, show_cost
-
 
-def update_cost(
-    cost_file: Path, new_cost: float, show_cost: bool = False
-) -> None:
-    if show_cost:
-        log.info(f"\nEstimated cost: ${new_cost:.6f}")
-    cost_data = {}
-    if cost_file.exists():
-        with open(cost_file, "r") as f:
-            cost_data = {k: v for k, v in sorted(json.load(f).items())}
-    month = datetime.now().strftime("%Y%m")
-    cost_data[month] = cost_data.get(month, 0) + new_cost
-    cost_file.parent.mkdir(parents=True, exist_ok=True)
-    with open(cost_file, "w") as f:
-        json.dump(cost_data, f)
-
-
-def run_chatgpt(
-    messages: Messages, params: dict[str, Any], chat: bool
-) -> float:
-    cls: Ask | Chat = Chat if chat else Ask
-    accepted_args = inspect.signature(cls.__init__).parameters  # type: ignore
-    params = {k: v for k, v in params.items() if k in accepted_args}
-    cost_data_this = cls(**params).run(messages)  # type: ignore
-    return cost_data_this
-
-
-def chatgpt_prompt_wrapper() -> None:
-    args = parse_arg()
-    cmd = args.subcommand[0]
-
-    if cmd == "help":
-        log.info(cli_help())
-        return
-
-    if cmd == "version":
-        log.info(f"{__package__} {__version__}")
-        return
-
-    config_file = (
-        Path(args.conf) if args.conf else get_config("cg", "config.toml")
-    )
-    cost_file = get_config("cg", "cost.json")
-
-    if cmd == "init":
-        init(config_file)
-        log.info(f"Created config file at {config_file}.")
-        return
-    if cmd == "cost":
-        cost(cost_file, log)
-        return
-
-    if not args.key:
-        raise ChatGPTPromptWrapperError(
-            "Set OPEN_AI_API_KEY environment variable or give it by -k (--key) argument."
+    def get_cmd_config(self, config: dict[str, Any]) -> dict[str, Any]:
+        cmd_config = config.get("global", {})
+        cmd_config.update(config.get(self.cmd, {}))
+        cmd_config["chat"] = (
+            True if self.cmd == "chat" else cmd_config.get("chat", False)
         )
+        self.update_cmd_config(cmd_config)
 
-    if cmd not in ['ask', 'chat'] and not config_file.is_file():
-        raise ChatGPTPromptWrapperError(
-            f"Configuration file {config_file} does not exist"
-            f"`ask` or `cht` subcommand can be used w/o configuration file."
-            f"You prepare the configuration file by `cg init` command."
+        if not cmd_config["chat"] and not cmd_config["messages"]:
+            raise ChatGPTPromptWrapperError(
+                "This subcommand (ask mode) does not predefined prompt and need input message."
+            )
+
+        return cmd_config
+
+    def run_chatgpt(self, config: dict[str, Any]) -> float:
+        cls: Ask | Chat = Chat if config["chat"] else Ask
+        accepted_args = inspect.signature(cls.__init__).parameters  # type: ignore
+        params = {k: v for k, v in config.items() if k in accepted_args}
+        cost_data_this = cls(**params).run(config["messages"])  # type: ignore
+        return cost_data_this
+
+    def update_cost(
+        self, cost_file: Path, new_cost: float, show_cost: bool = False
+    ) -> None:
+        if show_cost:
+            self.log.info(f"\nEstimated cost: ${new_cost:.6f}")
+        cost_data = {}
+        if cost_file.exists():
+            with open(cost_file, "r") as f:
+                cost_data = {k: v for k, v in sorted(json.load(f).items())}
+        month = datetime.now().strftime("%Y%m")
+        cost_data[month] = cost_data.get(month, 0) + new_cost
+        cost_file.parent.mkdir(parents=True, exist_ok=True)
+        with open(cost_file, "w") as f:
+            json.dump(cost_data, f)
+
+    def main(self) -> None:
+        if self.cmd_wo_config():
+            return
+
+        self.set_files()
+
+        if self.cmd_wo_key():
+            return
+
+        if not self.args.key:
+            raise ChatGPTPromptWrapperError(
+                "Set OPEN_AI_API_KEY environment variable or give it by -k (--key) argument."
+            )
+
+        if self.cmd not in ["ask", "chat"] and not self.config_file.is_file():
+            raise ChatGPTPromptWrapperError(
+                f"Configuration file {self.config_file} does not exist"
+                f"`ask` or `cht` subcommand can be used w/o configuration file."
+                f"You prepare the configuration file by `cg init` command."
+            )
+
+        if self.config_file.is_file():
+            with open(self.config_file, "rb") as f:
+                config = tomllib.load(f)
+        else:
+            config = {}
+
+        if self.cmd == "commands":
+            commands(config, self.log)
+            return
+
+        cmds = ["ask", "chat"] + [x for x in config if x != "global"]
+        if self.cmd == "global":
+            raise ChatGPTPromptWrapperError("`global` is not a subcommand.")
+        if self.cmd not in cmds:
+            raise ChatGPTPromptWrapperError(
+                f"Subcommand: `{self.cmd}` is not defined."
+            )
+
+        cmd_config = self.get_cmd_config(config)
+        cost_data_this = self.run_chatgpt(cmd_config)
+        self.update_cost(
+            self.cost_file, cost_data_this, cmd_config["show_cost"]
         )
 
-    if config_file.is_file():
-        with open(config_file, "rb") as f:
-            config = tomllib.load(f)
-    else:
-        config = {}
-
-    if cmd == "commands":
-        commands(config, log)
-        return
-
-    cmds = ["ask", "chat"] + list(config)
-    if cmd not in cmds or cmd == "global":
-        raise ChatGPTPromptWrapperError(f"Subcommand: {cmd} is not defined.")
-
-    cmd_config = config.get("global", {})
-    cmd_config.update(config.get(cmd, {}))
-    if cmd == "chat":
-        cmd_config["chat"] = True
-
-    chatgpt_params, messages, chat, show_cost = check_args(cmd_config, args)
-
-    cost_data_this = run_chatgpt(messages, chatgpt_params, chat)
-
-    update_cost(cost_file, cost_data_this, show_cost)
-
 
 def main() -> int:
+    cg = ChatGPTPromptWrapper()
     try:
-        chatgpt_prompt_wrapper()
+        cg.main()
         return 0
     except ChatGPTPromptWrapperError as e:
-        log.error(e)
+        cg.log.error(e)
         return 1
```

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/cmd/commands.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/config.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/docstring.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/docstring.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.7/src/chatgpt_prompt_wrapper/log_formatter.py` & `chatgpt_prompt_wrapper-0.0.8/src/chatgpt_prompt_wrapper/log_formatter.py`

 * *Files identical despite different names*

### Comparing `chatgpt_prompt_wrapper-0.0.7/PKG-INFO` & `chatgpt_prompt_wrapper-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chatgpt-prompt-wrapper
-Version: 0.0.7
-Summary: 
+Version: 0.0.8
+Summary: CLI tool to wrap ChatGPT Python API.
 Home-page: https://github.com/rcmdnk/chatgpt-prompt-wrapper
 License: Apache-2.0
 Keywords: chat,gpt,openai,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -171,14 +171,15 @@
 - `max_tokens`: The maximum number of tokens to generate in the chat completion. Set 0 to use the maximum values for the model. (default: 0)
 - `min_max_tokens`: The minimum of `max_tokens` for the completion when `max_tokens = 0`. (default: 200)
 - `tokens_limit`: The limit of the total tokens of the prompt and the completion. Set 0 to use the maximum values for the model. (default: 0)
 - `temperature`: Sampling temperature (0 ~ 2). (default: 1)
 - `top_p`: Probability (0 ~ 1) that the model will consider the top_p tokens. Do not set both temperature and top_p at the same time. (default: 1)
 - `presence_penalty`: The penalty for the model to return the same token (-2 ~ 2). (default: 0)
 - `frequency_penalty`: The penalty for the model to return the same token multiple times (-2 ~ 2). (default: 0)
+- Table of `alias`: Dictionary of role aliases. The default alias is: '`user' = 'User'`, `'system' = 'System'`, `'assistant' = 'Assistant'`.
 - List of `messages`: Dictionary of message, which must have `role` ('system', 'user' or 'assistant') and `content` (message text).
 
 The options for ask mode:
 
 - `show`: Set `true` to show prompt for non chat command.
 - `hide`: Set `true` to hide prompt for non chat command (default).
```

