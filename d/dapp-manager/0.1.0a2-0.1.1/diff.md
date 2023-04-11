# Comparing `tmp/dapp-manager-0.1.0a2.tar.gz` & `tmp/dapp-manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapp-manager-0.1.0a2.tar", max compression
+gzip compressed data, was "dapp-manager-0.1.1.tar", max compression
```

## Comparing `dapp-manager-0.1.0a2.tar` & `dapp-manager-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    26526 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     7420 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/README.md
--rw-r--r--   0        0        0      149 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/__init__.py
--rw-r--r--   0        0        0       97 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/__main__.py
--rw-r--r--   0        0        0     1261 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/autocomplete/__init__.py
--rw-r--r--   0        0        0      633 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/autocomplete/scripts/.dapp-manager.bash
--rw-r--r--   0        0        0      701 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/autocomplete/scripts/.dapp-manager.fish
--rw-r--r--   0        0        0     1010 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/autocomplete/scripts/.dapp-manager.zsh
--rw-r--r--   0        0        0     4863 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/cli.py
--rw-r--r--   0        0        0     9265 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/dapp_manager.py
--rw-r--r--   0        0        0     4056 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/dapp_starter.py
--rw-r--r--   0        0        0     2067 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/py.typed
--rw-r--r--   0        0        0     4887 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_manager/storage.py
--rw-r--r--   0        0        0       50 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_stats/README.md
--rw-r--r--   0        0        0       70 2023-02-23 12:01:23.588338 dapp-manager-0.1.0a2/dapp_stats/__init__.py
--rw-r--r--   0        0        0     1634 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/__main__.py
--rw-r--r--   0        0        0     4928 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/dapp_size_resolver.py
--rw-r--r--   0        0        0     1960 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/dapp_stats.py
--rw-r--r--   0        0        0      118 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/statistics/__init__.py
--rw-r--r--   0        0        0      360 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/statistics/enums.py
--rw-r--r--   0        0        0     1272 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/statistics/models.py
--rw-r--r--   0        0        0      257 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/dapp_stats/statistics/schemas.py
--rw-r--r--   0        0        0     4502 2023-02-23 12:01:23.592337 dapp-manager-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     8804 1970-01-01 00:00:00.000000 dapp-manager-0.1.0a2/setup.py
--rw-r--r--   0        0        0     8640 1970-01-01 00:00:00.000000 dapp-manager-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7276 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/README.md
+-rw-r--r--   0        0        0      149 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/__init__.py
+-rw-r--r--   0        0        0       97 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/__main__.py
+-rw-r--r--   0        0        0     1261 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/__init__.py
+-rw-r--r--   0        0        0      674 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.bash
+-rw-r--r--   0        0        0      171 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.fish
+-rw-r--r--   0        0        0      900 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.zsh
+-rw-r--r--   0        0        0     4825 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/cli.py
+-rw-r--r--   0        0        0     9265 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/dapp_manager.py
+-rw-r--r--   0        0        0     4056 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/dapp_starter.py
+-rw-r--r--   0        0        0     2067 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/py.typed
+-rw-r--r--   0        0        0     4887 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/storage.py
+-rw-r--r--   0        0        0       50 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/README.md
+-rw-r--r--   0        0        0       70 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/__init__.py
+-rw-r--r--   0        0        0     1634 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/__main__.py
+-rw-r--r--   0        0        0     4928 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/dapp_size_resolver.py
+-rw-r--r--   0        0        0     1960 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/dapp_stats.py
+-rw-r--r--   0        0        0      118 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/__init__.py
+-rw-r--r--   0        0        0      360 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/enums.py
+-rw-r--r--   0        0        0     1272 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/models.py
+-rw-r--r--   0        0        0      257 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/schemas.py
+-rw-r--r--   0        0        0     4499 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8658 1970-01-01 00:00:00.000000 dapp-manager-0.1.1/setup.py
+-rw-r--r--   0        0        0     8499 1970-01-01 00:00:00.000000 dapp-manager-0.1.1/PKG-INFO
```

### Comparing `dapp-manager-0.1.0a2/LICENSE` & `dapp-manager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/README.md` & `dapp-manager-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ```
 
 The app is started in a background `dapp-runner` process, and you're returned an application ID in
 the form of a hexadecimal string. You can use this ID to query the state and other output streams
 using `dapp-manager`'s `read` command, e.g.:
 
 ```bash
-dapp-manager read state <the-hex-string>
+dapp-manager read <the-hex-string> state
 ```
 
 will display the contents of the `state` stream of the running app:
 
 ```shell
 {"db": {"0": "pending"}}
 {"db": {"0": "starting"}}
@@ -110,15 +110,15 @@
 In case something goes amiss, `dapp-manager` will output:
 ```App <the-hex-string> is not running.```
 
 Whatever the reason, you can still query the various streams of a terminated dapp by adding the
 `--no-ensure-alive` option, e.g.:
 
 ```bash
-dapp-manager read stderr <the-hex-string> --no-ensure-alive
+dapp-manager read <the-hex-string> --no-ensure-alive stderr
 ```
 
 ## Full usage
 
 ```shell
 Usage: dapp-manager [OPTIONS] COMMAND [ARGS]...
 
@@ -184,27 +184,22 @@
 
 ### Read
 
 The `read` command outputs the full contents of the specified stream. There are five streams as
 specified by the usage below:
 
 ```shell
-Usage: dapp-manager read [OPTIONS] COMMAND [ARGS]...
+Usage: dapp-manager read [OPTIONS] APP_ID [state|data|log|stdout|stderr]
 
   Read output from the given app.
 
 Options:
-  --help  Show this message and exit.
-
-Commands:
-  data    Read the data stream of the given app.
-  log     Read the log stream of a given app.
-  state   Read the state stream of the given app.
-  stderr  Read the stderr of a given app.
-  stdout  Read the stdout of a given app.
+  --ensure-alive / --no-ensure-alive
+  -f, --follow
+  --help                          Show this message and exit.
 ```
 
 By default, the stream will only be output if the app is currently running. Otherwise, you'll get
 the ```App <the-hex-string> is not running.``` message and no stream.
 
 If you wish to query a stream of a terminated app, add the `--no-ensure-alive` parameter to the
 specific `read` command.
```

### Comparing `dapp-manager-0.1.0a2/dapp_manager/autocomplete/__init__.py` & `dapp-manager-0.1.1/dapp_manager/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_manager/autocomplete/scripts/.dapp-manager.zsh` & `dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.zsh`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-
 #compdef dapp-manager
 
 _dapp_manager_completion() {
     local -a completions
     local -a completions_with_descriptions
     local -a response
     (( ! $+commands[dapp-manager] )) && return 1
 
-    response=("${(@f)$(env COMP_WORDS="${words[*]}" COMP_CWORD=$((CURRENT-1)) _DAPP_MANAGER_COMPLETE=zsh_complete dapp-manager)}")
-
-    for type key descr in ${response}; do
-        if [[ "$type" == "plain" ]]; then
-            if [[ "$descr" == "_" ]]; then
-                completions+=("$key")
-            else
-                completions_with_descriptions+=("$key":"$descr")
-            fi
-        elif [[ "$type" == "dir" ]]; then
-            _path_files -/
-        elif [[ "$type" == "file" ]]; then
-            _path_files -f
-        fi
+    response=("${(@f)$( env COMP_WORDS="${words[*]}" \
+                        COMP_CWORD=$((CURRENT-1)) \
+                        _DAPP_MANAGER_COMPLETE="complete_zsh" \
+                        dapp-manager )}")
+
+    for key descr in ${(kv)response}; do
+      if [[ "$descr" == "_" ]]; then
+          completions+=("$key")
+      else
+          completions_with_descriptions+=("$key":"$descr")
+      fi
     done
 
     if [ -n "$completions_with_descriptions" ]; then
         _describe -V unsorted completions_with_descriptions -U
     fi
 
     if [ -n "$completions" ]; then
         compadd -U -V unsorted -a completions
     fi
+    compstate[insert]="automenu"
 }
 
 compdef _dapp_manager_completion dapp-manager;
-
```

### Comparing `dapp-manager-0.1.0a2/dapp_manager/cli.py` & `dapp-manager-0.1.1/dapp_manager/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from pathlib import Path
 from typing import Optional, Tuple
 
 import click
 from dapp_runner.log import LOG_CHOICES
 
 from dapp_manager import DappManager
+from dapp_manager.autocomplete import install_autocomplete
 from dapp_manager.exceptions import DappManagerException
 from dapp_manager.storage import RunnerReadFileType
 
-# from dapp_manager.autocomplete import install_autocomplete
 
-
-def _app_id_autocomplete(_ctx, _param, incomplete):
+def _app_id_autocomplete(ctx, args, incomplete):  # noqa
     return [app_id for app_id in DappManager.list() if app_id.startswith(incomplete)]
 
 
 def _with_app_id(wrapped_func):
-    wrapped_func = click.argument("app-id", type=str)(  # shell_complete=_app_id_autocomplete)(
+    wrapped_func = click.argument("app-id", type=click.STRING, autocompletion=_app_id_autocomplete)(
         wrapped_func
     )
     return wrapped_func
 
 
 def _capture_api_exceptions(f):
     @wraps(f)
@@ -167,31 +166,31 @@
     if follow:
         for chunk in dapp.read_file_follow(file_type, ensure_alive=ensure_alive):
             print(chunk, end="")
     else:
         print(dapp.read_file(file_type, ensure_alive=ensure_alive))
 
 
-# @cli.command()
-# @click.argument("shell", type=click.Choice(["bash", "fish", "zsh"]))
-# @click.option(
-#     "--path",
-#     "-p",
-#     type=Path,
-#     default=None,
-#     help="Path to the file to which the shell completion function should be added.",
-# )
-# def autocomplete(shell: str, path: Path):
-#     """Enable CLI shell completion for the given shell.
-#
-#     This command works by appending a pre-defined piece of shell code to the user's shell
-#     configuration file.
-#
-#     The default target file will depend on the selected shell type (bash, fish or zsh):
-#         - bash: `~/.bashrc`
-#         - fish: `~/.config/fish/completions/{script_name}.fish`
-#         - zsh: `~/.zshrc`
-#     Use the `--path` flag to override the default target file.
-#
-#     The command does nothing if the target file already contains the completion code.
-#     """
-#     install_autocomplete(shell, path)
+@cli.command()
+@click.argument("shell", type=click.Choice(["bash", "fish", "zsh"]))
+@click.option(
+    "--path",
+    "-p",
+    type=Path,
+    default=None,
+    help="Path to the file to which the shell completion function should be added.",
+)
+def autocomplete(shell: str, path: Path):
+    """Enable CLI shell completion for the given shell.
+
+    This command works by appending a pre-defined piece of shell code to the user's shell
+    configuration file.
+
+    The default target file will depend on the selected shell type (bash, fish or zsh):
+        - bash: `~/.bashrc`
+        - fish: `~/.config/fish/completions/{script_name}.fish`
+        - zsh: `~/.zshrc`
+    Use the `--path` flag to override the default target file.
+
+    The command does nothing if the target file already contains the completion code.
+    """
+    install_autocomplete(shell, path)
```

### Comparing `dapp-manager-0.1.0a2/dapp_manager/dapp_manager.py` & `dapp-manager-0.1.1/dapp_manager/dapp_manager.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_manager/dapp_starter.py` & `dapp-manager-0.1.1/dapp_manager/dapp_starter.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_manager/exceptions.py` & `dapp-manager-0.1.1/dapp_manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_manager/storage.py` & `dapp-manager-0.1.1/dapp_manager/storage.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_stats/__main__.py` & `dapp-manager-0.1.1/dapp_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_stats/dapp_size_resolver.py` & `dapp-manager-0.1.1/dapp_stats/dapp_size_resolver.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_stats/dapp_stats.py` & `dapp-manager-0.1.1/dapp_stats/dapp_stats.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/dapp_stats/statistics/models.py` & `dapp-manager-0.1.1/dapp_stats/statistics/models.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.0a2/pyproject.toml` & `dapp-manager-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapp-manager"
-version = "0.1.0a2"
+version = "0.1.1"
 description = "Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
@@ -31,15 +31,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 
 psutil = "^5.9"
 appdirs = "^1.4"
 click = "^7.0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
 pydantic = "^1.9"
-dapp-runner = "0.1.0a1"
+dapp-runner = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "*"  # implicitly required by liccehck
 pip = "*"  # implicitly required by liccehck
 
 autoflake = "^1"
 black = "^21.0b0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
```

### Comparing `dapp-manager-0.1.0a2/setup.py` & `dapp-manager-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 package_data = \
 {'': ['*'], 'dapp_manager.autocomplete': ['scripts/*']}
 
 install_requires = \
 ['appdirs>=1.4,<2.0',
  'click>=7.0,<8.0',
- 'dapp-runner==0.1.0a1',
+ 'dapp-runner>=0.1.1,<0.2.0',
  'psutil>=5.9,<6.0',
  'pydantic>=1.9,<2.0']
 
 entry_points = \
 {'console_scripts': ['dapp-manager = dapp_manager.__main__:main',
                      'dapp-stats = dapp_stats.__main__:main']}
 
 setup_kwargs = {
     'name': 'dapp-manager',
-    'version': '0.1.0a2',
+    'version': '0.1.1',
     'description': "Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface",
-    'long_description': '# Golem dApp Manager\n\n`dapp-manager` is a purposefully minimalistic manager for decentralized applications running on\nGolem. It works together with the [dapp-runner](https://github.com/golemfactory/dapp-runner/).\nWhile the responsibility of the latter is to run a single Golem application, `dapp-manager` takes\ncare of spawning, interacting with, and stopping the running instances of the `dapp-runner`.\n\n## Quick start\n\n### Yagna daemon\n\nAs the `dapp-manager` uses the `dapp-runner`, which in turn requires a properly configured\n[yagna](https://github.com/golemfactory/yagna) daemon, you\'ll need to have it set up.\n\nFor now, please follow the ["Requestor development: a quick primer"](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development)\ntutorial and ensure that your `yagna` is up and running. Only the first part of this\ntutorial is required - you don\'t need to run the blender example.\n\nMost importantly, make sure you have set the `YAGNA_APPKEY` in your environment, e.g. with:\n\n```bash\nexport YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nor, on Windows:\n\n```bash\nset YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nand if you don\'t know what your app-key is, you can always query `yagna` with:\n\n```bash\nyagna app-key list\n```\n\n### Python environment\n\nFirst, ensure you have Python 3.8 or later:\n\n```bash\npython3 --version\n```\n\n[ depending on the platform, it may be just `python` instead of `python3` ]\n\nIf your Python version is older, consider using [pyenv](https://github.com/pyenv/pyenv-installer).\n\nOnce your python interpreter reports a version 3.8 or later, you can set up your virtual\nenvironment:\n\n```bash\npython3 -m venv ~/.envs/dapp-manager\nsource ~/.envs/dapp-manager/bin/activate\n```\n\nor, if you\'re on Windows:\n\n```shell\npython -m venv --clear %HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-manager\n%HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-manager\\Scripts\\activate.bat\n```\n\n### DApp manager\n\n#### Clone the repository\n\n```bash\ngit clone --recurse-submodules https://github.com/golemfactory/dapp-manager.git\n```\n\n#### Install the dependencies\n\n```bash\ncd dapp-manager\npip install -U pip poetry\npoetry install\n```\n\n#### Run an example application\n\nMake sure your `yagna` daemon is running,\nyou have initialized the payment driver with `yagna payment init --sender`,\nand that you have set the `YAGNA_APPKEY` environment variable.\n\nThen run:\n\n```bash\ndapp-manager start --config sample_config.yml dapp-store/apps/webapp.yaml\n```\n\nThe app is started in a background `dapp-runner` process, and you\'re returned an application ID in\nthe form of a hexadecimal string. You can use this ID to query the state and other output streams\nusing `dapp-manager`\'s `read` command, e.g.:\n\n```bash\ndapp-manager read state <the-hex-string>\n```\n\nwill display the contents of the `state` stream of the running app:\n\n```shell\n{"db": {"0": "pending"}}\n{"db": {"0": "starting"}}\n{"db": {"0": "running"}}\n{"db": {"0": "running"}, "http": {"0": "pending"}}\n{"db": {"0": "running"}, "http": {"0": "starting"}}\n```\n\nIn case something goes amiss, `dapp-manager` will output:\n```App <the-hex-string> is not running.```\n\nWhatever the reason, you can still query the various streams of a terminated dapp by adding the\n`--no-ensure-alive` option, e.g.:\n\n```bash\ndapp-manager read stderr <the-hex-string> --no-ensure-alive\n```\n\n## Full usage\n\n```shell\nUsage: dapp-manager [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  autocomplete  Enable CLI shell completion for the given shell.\n  kill          Stop the given app forcibly.\n  list          List known app IDs (both active and dead).\n  prune         Remove data for non-running apps.\n  read          Read output from the given app.\n  start         Start a new app using the provided descriptor and config...\n  stop          Stop the given app gracefully.\n```\n\n### Start\n\nThe `start` command launches a new instance of the `dapp-runner` in a background process and\nreturns the hexadecimal string that is the identifier of the running `dapp-runner` instance.\n\n```shell\nUsage: dapp-manager start [OPTIONS] DESCRIPTORS...\n\n  Start a new app using the provided descriptor and config files.\n\nOptions:\n  -c, --config PATH  Path to the file containing yagna-specific config.\n                     [required]\n  --help             Show this message and exit.\n```\n\nImportantly, it requires a config file which contains the parameters used to connect to the `yagna`\ndaemon and initialize the requestor engine. We\'re providing a default, sample configuration as\n`sample_config.yml` in the root of the `dapp-manager` repository.\n\nOf course, it also requires one or more descriptor files that are used by the `dapp-runner` to\ndeploy the specified applications on Golem.\n\n### Stop / Kill\n\nThe `stop` and `kill` commands terminate the given `dapp-runner` instance, the main difference\nbeing the signal that\'s sent to do that. Essentially, `stop` should be enough and should give the\n`dapp-runner` a chance to shut the app down gracefully, correctly terminating the services,\nclosing the agreements and paying for them.\n\nIn case `stop` is stuck for whatever reason, you might want to resort to `kill` which terminates\nthe `dapp-runner` immediately without allowing for any graceful shutdown.\n\n### List\n\nThe `list` command shows the identifiers of all the previously-started apps, whether they\'re still\nrunning or not.\n\n### Prune\n\n`prune` causes `dapp-manager` to remove the data for those apps that it had previously identified as\ndefunct. Consequently, those apps will no longer appear on the list.\n\nUnless an app has been explicitly stopped with a `stop` or `kill` command, the `dapp-manager`\nwill not purge it until it has had a chance to notice the termination, e.g. by issuing a `read`\ncommand to the defunct app.\n\n### Read\n\nThe `read` command outputs the full contents of the specified stream. There are five streams as\nspecified by the usage below:\n\n```shell\nUsage: dapp-manager read [OPTIONS] COMMAND [ARGS]...\n\n  Read output from the given app.\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  data    Read the data stream of the given app.\n  log     Read the log stream of a given app.\n  state   Read the state stream of the given app.\n  stderr  Read the stderr of a given app.\n  stdout  Read the stdout of a given app.\n```\n\nBy default, the stream will only be output if the app is currently running. Otherwise, you\'ll get\nthe ```App <the-hex-string> is not running.``` message and no stream.\n\nIf you wish to query a stream of a terminated app, add the `--no-ensure-alive` parameter to the\nspecific `read` command.\n\n### Shell completion\n\nThis program supports shell completion for all of its commands, as well as existing dApp IDs (where applicable).\n\nTo enable completion, use the `autocomplete` command with your shell of choice:\n\n* **bash**:\n\n    ```bash\n    dapp-manager autocomplete bash\n    ```\n\n* **zsh**:\n\n    ```bash\n    dapp-manager autocomplete zsh\n    ```\n\n* **fish**:\n\n    ```bash\n    dapp-manager autocomplete fish\n    ```\n\nThe completion functions are defined in `dapp_manager/autocomplete/scripts`.\n\nShould the entrypoint name ever change, those files will need to be updated as well.\n\n**WARNING** Completion will **NOT WORK** when `autocomplete` is invoked with `python -m dapp_manager`.\nOnly the installed entrypoint (i.e. `dapp-manager`) is supported. To have it available, run `poetry install`.\n',
+    'long_description': '# Golem dApp Manager\n\n`dapp-manager` is a purposefully minimalistic manager for decentralized applications running on\nGolem. It works together with the [dapp-runner](https://github.com/golemfactory/dapp-runner/).\nWhile the responsibility of the latter is to run a single Golem application, `dapp-manager` takes\ncare of spawning, interacting with, and stopping the running instances of the `dapp-runner`.\n\n## Quick start\n\n### Yagna daemon\n\nAs the `dapp-manager` uses the `dapp-runner`, which in turn requires a properly configured\n[yagna](https://github.com/golemfactory/yagna) daemon, you\'ll need to have it set up.\n\nFor now, please follow the ["Requestor development: a quick primer"](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development)\ntutorial and ensure that your `yagna` is up and running. Only the first part of this\ntutorial is required - you don\'t need to run the blender example.\n\nMost importantly, make sure you have set the `YAGNA_APPKEY` in your environment, e.g. with:\n\n```bash\nexport YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nor, on Windows:\n\n```bash\nset YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nand if you don\'t know what your app-key is, you can always query `yagna` with:\n\n```bash\nyagna app-key list\n```\n\n### Python environment\n\nFirst, ensure you have Python 3.8 or later:\n\n```bash\npython3 --version\n```\n\n[ depending on the platform, it may be just `python` instead of `python3` ]\n\nIf your Python version is older, consider using [pyenv](https://github.com/pyenv/pyenv-installer).\n\nOnce your python interpreter reports a version 3.8 or later, you can set up your virtual\nenvironment:\n\n```bash\npython3 -m venv ~/.envs/dapp-manager\nsource ~/.envs/dapp-manager/bin/activate\n```\n\nor, if you\'re on Windows:\n\n```shell\npython -m venv --clear %HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-manager\n%HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-manager\\Scripts\\activate.bat\n```\n\n### DApp manager\n\n#### Clone the repository\n\n```bash\ngit clone --recurse-submodules https://github.com/golemfactory/dapp-manager.git\n```\n\n#### Install the dependencies\n\n```bash\ncd dapp-manager\npip install -U pip poetry\npoetry install\n```\n\n#### Run an example application\n\nMake sure your `yagna` daemon is running,\nyou have initialized the payment driver with `yagna payment init --sender`,\nand that you have set the `YAGNA_APPKEY` environment variable.\n\nThen run:\n\n```bash\ndapp-manager start --config sample_config.yml dapp-store/apps/webapp.yaml\n```\n\nThe app is started in a background `dapp-runner` process, and you\'re returned an application ID in\nthe form of a hexadecimal string. You can use this ID to query the state and other output streams\nusing `dapp-manager`\'s `read` command, e.g.:\n\n```bash\ndapp-manager read <the-hex-string> state\n```\n\nwill display the contents of the `state` stream of the running app:\n\n```shell\n{"db": {"0": "pending"}}\n{"db": {"0": "starting"}}\n{"db": {"0": "running"}}\n{"db": {"0": "running"}, "http": {"0": "pending"}}\n{"db": {"0": "running"}, "http": {"0": "starting"}}\n```\n\nIn case something goes amiss, `dapp-manager` will output:\n```App <the-hex-string> is not running.```\n\nWhatever the reason, you can still query the various streams of a terminated dapp by adding the\n`--no-ensure-alive` option, e.g.:\n\n```bash\ndapp-manager read <the-hex-string> --no-ensure-alive stderr\n```\n\n## Full usage\n\n```shell\nUsage: dapp-manager [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  autocomplete  Enable CLI shell completion for the given shell.\n  kill          Stop the given app forcibly.\n  list          List known app IDs (both active and dead).\n  prune         Remove data for non-running apps.\n  read          Read output from the given app.\n  start         Start a new app using the provided descriptor and config...\n  stop          Stop the given app gracefully.\n```\n\n### Start\n\nThe `start` command launches a new instance of the `dapp-runner` in a background process and\nreturns the hexadecimal string that is the identifier of the running `dapp-runner` instance.\n\n```shell\nUsage: dapp-manager start [OPTIONS] DESCRIPTORS...\n\n  Start a new app using the provided descriptor and config files.\n\nOptions:\n  -c, --config PATH  Path to the file containing yagna-specific config.\n                     [required]\n  --help             Show this message and exit.\n```\n\nImportantly, it requires a config file which contains the parameters used to connect to the `yagna`\ndaemon and initialize the requestor engine. We\'re providing a default, sample configuration as\n`sample_config.yml` in the root of the `dapp-manager` repository.\n\nOf course, it also requires one or more descriptor files that are used by the `dapp-runner` to\ndeploy the specified applications on Golem.\n\n### Stop / Kill\n\nThe `stop` and `kill` commands terminate the given `dapp-runner` instance, the main difference\nbeing the signal that\'s sent to do that. Essentially, `stop` should be enough and should give the\n`dapp-runner` a chance to shut the app down gracefully, correctly terminating the services,\nclosing the agreements and paying for them.\n\nIn case `stop` is stuck for whatever reason, you might want to resort to `kill` which terminates\nthe `dapp-runner` immediately without allowing for any graceful shutdown.\n\n### List\n\nThe `list` command shows the identifiers of all the previously-started apps, whether they\'re still\nrunning or not.\n\n### Prune\n\n`prune` causes `dapp-manager` to remove the data for those apps that it had previously identified as\ndefunct. Consequently, those apps will no longer appear on the list.\n\nUnless an app has been explicitly stopped with a `stop` or `kill` command, the `dapp-manager`\nwill not purge it until it has had a chance to notice the termination, e.g. by issuing a `read`\ncommand to the defunct app.\n\n### Read\n\nThe `read` command outputs the full contents of the specified stream. There are five streams as\nspecified by the usage below:\n\n```shell\nUsage: dapp-manager read [OPTIONS] APP_ID [state|data|log|stdout|stderr]\n\n  Read output from the given app.\n\nOptions:\n  --ensure-alive / --no-ensure-alive\n  -f, --follow\n  --help                          Show this message and exit.\n```\n\nBy default, the stream will only be output if the app is currently running. Otherwise, you\'ll get\nthe ```App <the-hex-string> is not running.``` message and no stream.\n\nIf you wish to query a stream of a terminated app, add the `--no-ensure-alive` parameter to the\nspecific `read` command.\n\n### Shell completion\n\nThis program supports shell completion for all of its commands, as well as existing dApp IDs (where applicable).\n\nTo enable completion, use the `autocomplete` command with your shell of choice:\n\n* **bash**:\n\n    ```bash\n    dapp-manager autocomplete bash\n    ```\n\n* **zsh**:\n\n    ```bash\n    dapp-manager autocomplete zsh\n    ```\n\n* **fish**:\n\n    ```bash\n    dapp-manager autocomplete fish\n    ```\n\nThe completion functions are defined in `dapp_manager/autocomplete/scripts`.\n\nShould the entrypoint name ever change, those files will need to be updated as well.\n\n**WARNING** Completion will **NOT WORK** when `autocomplete` is invoked with `python -m dapp_manager`.\nOnly the installed entrypoint (i.e. `dapp-manager`) is supported. To have it available, run `poetry install`.\n',
     'author': 'Golem Factory',
     'author_email': 'contact@golem.network',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/golemfactory/dapp-manager',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dapp-manager-0.1.0a2/PKG-INFO` & `dapp-manager-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapp-manager
-Version: 0.1.0a2
+Version: 0.1.1
 Summary: Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface
 Home-page: https://github.com/golemfactory/dapp-manager
 License: LGPL-3.0
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: appdirs (>=1.4,<2.0)
 Requires-Dist: click (>=7.0,<8.0)
-Requires-Dist: dapp-runner (==0.1.0a1)
+Requires-Dist: dapp-runner (>=0.1.1,<0.2.0)
 Requires-Dist: psutil (>=5.9,<6.0)
 Requires-Dist: pydantic (>=1.9,<2.0)
 Project-URL: Repository, https://github.com/golemfactory/dapp-manager
 Description-Content-Type: text/markdown
 
 # Golem dApp Manager
 
@@ -119,15 +119,15 @@
 ```
 
 The app is started in a background `dapp-runner` process, and you're returned an application ID in
 the form of a hexadecimal string. You can use this ID to query the state and other output streams
 using `dapp-manager`'s `read` command, e.g.:
 
 ```bash
-dapp-manager read state <the-hex-string>
+dapp-manager read <the-hex-string> state
 ```
 
 will display the contents of the `state` stream of the running app:
 
 ```shell
 {"db": {"0": "pending"}}
 {"db": {"0": "starting"}}
@@ -139,15 +139,15 @@
 In case something goes amiss, `dapp-manager` will output:
 ```App <the-hex-string> is not running.```
 
 Whatever the reason, you can still query the various streams of a terminated dapp by adding the
 `--no-ensure-alive` option, e.g.:
 
 ```bash
-dapp-manager read stderr <the-hex-string> --no-ensure-alive
+dapp-manager read <the-hex-string> --no-ensure-alive stderr
 ```
 
 ## Full usage
 
 ```shell
 Usage: dapp-manager [OPTIONS] COMMAND [ARGS]...
 
@@ -213,27 +213,22 @@
 
 ### Read
 
 The `read` command outputs the full contents of the specified stream. There are five streams as
 specified by the usage below:
 
 ```shell
-Usage: dapp-manager read [OPTIONS] COMMAND [ARGS]...
+Usage: dapp-manager read [OPTIONS] APP_ID [state|data|log|stdout|stderr]
 
   Read output from the given app.
 
 Options:
-  --help  Show this message and exit.
-
-Commands:
-  data    Read the data stream of the given app.
-  log     Read the log stream of a given app.
-  state   Read the state stream of the given app.
-  stderr  Read the stderr of a given app.
-  stdout  Read the stdout of a given app.
+  --ensure-alive / --no-ensure-alive
+  -f, --follow
+  --help                          Show this message and exit.
 ```
 
 By default, the stream will only be output if the app is currently running. Otherwise, you'll get
 the ```App <the-hex-string> is not running.``` message and no stream.
 
 If you wish to query a stream of a terminated app, add the `--no-ensure-alive` parameter to the
 specific `read` command.
```

