# Comparing `tmp/abml-cli-0.1.4.tar.gz` & `tmp/abml_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abml-cli-0.1.4.tar", max compression
+gzip compressed data, was "abml_cli-0.1.6.tar", max compression
```

## Comparing `abml-cli-0.1.4.tar` & `abml_cli-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      149 2023-03-19 13:04:36.090108 abml-cli-0.1.4/abml_cli/__init__.py
--rw-r--r--   0        0        0     5536 2023-03-08 14:18:33.000000 abml-cli-0.1.4/abml_cli/abml_cli_helpers.py
--rw-r--r--   0        0        0    11654 2023-04-05 09:20:25.000000 abml-cli-0.1.4/abml_cli/abml_exec-DESKTOP-N7IPE21.py
--rw-r--r--   0        0        0    12271 2023-04-07 14:59:30.566839 abml-cli-0.1.4/abml_cli/abml_exec.py
--rw-r--r--   0        0        0      306 2023-04-03 07:42:15.263976 abml-cli-0.1.4/abml_cli/abml_filters.py
--rw-r--r--   0        0        0     2346 2023-04-05 07:52:22.000000 abml-cli-0.1.4/abml_cli/abml_parser.py
--rw-r--r--   0        0        0     4731 2023-04-07 14:40:15.642023 abml-cli-0.1.4/abml_cli/abml_subroutines.py
--rw-r--r--   0        0        0    14049 2023-03-08 11:39:18.000000 abml-cli-0.1.4/abml_cli/dataclasses/abml_schema.json
--rw-r--r--   0        0        0     4448 2023-03-08 12:22:33.000000 abml-cli-0.1.4/abml_cli/dataclasses/model.py
--rw-r--r--   0        0        0     2667 2023-03-05 15:19:05.000000 abml-cli-0.1.4/abml_cli/dataclasses/template_schema.json
--rw-r--r--   0        0        0      215 2023-03-08 11:46:11.000000 abml-cli-0.1.4/abml_cli/examples/test.abml
--rw-r--r--   0        0        0      168 2023-03-21 09:13:53.000000 abml-cli-0.1.4/abml_cli/subroutines/dload/templates/block.j2.f
--rw-r--r--   0        0        0      116 2023-03-21 08:43:40.000000 abml-cli-0.1.4/abml_cli/subroutines/dload/templates/circle.j2.f
--rw-r--r--   0        0        0      298 2023-03-20 10:54:43.471639 abml-cli-0.1.4/abml_cli/subroutines/dload/templates/head.j2.f
--rw-r--r--   0        0        0      157 2023-03-21 10:23:24.000000 abml-cli-0.1.4/abml_cli/subroutines/dload/templates/rect.j2.f
--rw-r--r--   0        0        0       68 2023-03-19 14:20:12.928461 abml-cli-0.1.4/abml_cli/subroutines/dload/templates/tail.j2.f
--rw-r--r--   0        0        0      407 2023-03-18 20:33:18.495847 abml-cli-0.1.4/abml_cli/subroutines/dload/test.f
--rw-r--r--   0        0        0      502 2023-03-18 20:33:30.969561 abml-cli-0.1.4/abml_cli/subroutines/dload/test.py
--rw-r--r--   0        0        0      732 2023-04-07 15:21:01.867207 abml-cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-07 14:06:33.000000 abml-cli-0.1.4/README.md
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 abml-cli-0.1.4/setup.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 abml-cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      184 2023-04-09 12:29:28.000000 abml_cli-0.1.6/abml_cli/__init__.py
+-rw-r--r--   0        0        0     5536 2023-03-08 14:18:33.236588 abml_cli-0.1.6/abml_cli/abml_cli_helpers.py
+-rw-r--r--   0        0        0    11654 2023-04-05 09:20:25.287588 abml_cli-0.1.6/abml_cli/abml_exec-DESKTOP-N7IPE21.py
+-rw-r--r--   0        0        0    12509 2023-04-10 13:25:11.000000 abml_cli-0.1.6/abml_cli/abml_exec.py
+-rw-r--r--   0        0        0      306 2023-04-03 07:42:15.000000 abml_cli-0.1.6/abml_cli/abml_filters.py
+-rw-r--r--   0        0        0     2852 2023-04-10 13:27:42.000000 abml_cli-0.1.6/abml_cli/abml_parser.py
+-rw-r--r--   0        0        0     4731 2023-04-07 14:40:15.000000 abml_cli-0.1.6/abml_cli/abml_subroutines.py
+-rw-r--r--   0        0        0     1276 2023-04-11 06:53:40.721642 abml_cli-0.1.6/abml_cli/abml_tester.py
+-rw-r--r--   0        0        0    14049 2023-03-08 11:39:18.967142 abml_cli-0.1.6/abml_cli/dataclasses/abml_schema.json
+-rw-r--r--   0        0        0     4448 2023-03-08 12:22:33.145120 abml_cli-0.1.6/abml_cli/dataclasses/model.py
+-rw-r--r--   0        0        0     2667 2023-03-05 15:19:05.000000 abml_cli-0.1.6/abml_cli/dataclasses/template_schema.json
+-rw-r--r--   0        0        0      215 2023-03-08 11:46:11.768354 abml_cli-0.1.6/abml_cli/examples/test.abml
+-rw-r--r--   0        0        0      168 2023-03-21 09:13:53.978078 abml_cli-0.1.6/abml_cli/subroutines/dload/templates/block.j2.f
+-rw-r--r--   0        0        0      116 2023-03-21 08:43:40.648845 abml_cli-0.1.6/abml_cli/subroutines/dload/templates/circle.j2.f
+-rw-r--r--   0        0        0      298 2023-03-20 10:54:43.000000 abml_cli-0.1.6/abml_cli/subroutines/dload/templates/head.j2.f
+-rw-r--r--   0        0        0      157 2023-03-21 10:23:24.303646 abml_cli-0.1.6/abml_cli/subroutines/dload/templates/rect.j2.f
+-rw-r--r--   0        0        0       68 2023-03-19 14:20:12.000000 abml_cli-0.1.6/abml_cli/subroutines/dload/templates/tail.j2.f
+-rw-r--r--   0        0        0      407 2023-03-18 20:33:18.000000 abml_cli-0.1.6/abml_cli/subroutines/dload/test.f
+-rw-r--r--   0        0        0      502 2023-03-18 20:33:30.000000 abml_cli-0.1.6/abml_cli/subroutines/dload/test.py
+-rw-r--r--   0        0        0      732 2023-04-11 07:40:49.545712 abml_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-07 14:06:33.197635 abml_cli-0.1.6/README.md
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 abml_cli-0.1.6/setup.py
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 abml_cli-0.1.6/PKG-INFO
```

### Comparing `abml-cli-0.1.4/abml_cli/abml_cli_helpers.py` & `abml_cli-0.1.6/abml_cli/abml_cli_helpers.py`

 * *Files identical despite different names*

### Comparing `abml-cli-0.1.4/abml_cli/abml_exec-DESKTOP-N7IPE21.py` & `abml_cli-0.1.6/abml_cli/abml_exec-DESKTOP-N7IPE21.py`

 * *Files identical despite different names*

### Comparing `abml-cli-0.1.4/abml_cli/abml_exec.py` & `abml_cli-0.1.6/abml_cli/abml_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,23 @@
     # with open(filename_render, mode="r", encoding="utf-8") as f:
     subs_dict = data.get("subroutines")
 
     if subs_dict is not None:
         Abml_Subroutine(subs_dict, cwd=cwd, name=name)
 
 
-def abml_file_mode(file: str, parameters: dict, env: Environment, cwd=None, name=None, config={}):
+def abml_file_mode(
+    file: str,
+    parameters: dict,
+    env: Environment,
+    cwd=None,
+    name=None,
+    config={},
+    test=False,
+):
     if name is None:
         filename_render = f"_{file}"
         name = file.split(".")[0]
     else:
         filename_render = f"_{name}.abml"
 
     parameters["abml_name"] = name
@@ -174,15 +182,16 @@
         "file": render_path,
         "name": name,
         "input_type": config.get("build", {}).get("inputs", {}).get("type", "copy"),
         "input_folder": input_folder,
     }
 
     params_string = " ".join([f'--{key} "{val}"' for key, val in params.items()])
-    cmd = f'abaqus cae noGui="{parser}" -- {params_string}'
+    cmd = f'abaqus cae noGui="{parser}" -- {params_string} --test {test}'
+    console.print(cmd)
     subprocess.call(cmd, shell=True, cwd=cwd)
 
     return True
 
 
 def generate_param_grid(param_grid):
     if not isinstance(param_grid, dict):
@@ -232,16 +241,16 @@
         else:
             items.append((new_key, value))
     return dict(items)
 
 
 @click.command()
 @click.option("--files", "-f", help="abml-files", required=False, multiple=True)
-def run(files=None):
-    console.print("#################### run test")
+@click.option("--test", "-t", is_flag=True, help="Enable verbose output.")
+def run(files=None, test=False):
     env = Env(loader=FileSystemLoader(os.getcwd()), autoescape=select_autoescape())
     env.load_filters(abml_filters)
 
     try:
         sys.path.append(os.getcwd())
         import _filters
 
@@ -258,22 +267,29 @@
             parameters.update(yaml.load(f, Loader=Loader))
 
     cae_reg = {
         "abml": abml_file_mode,
     }
 
     processed = False
-
+    console.print(test)
     if files is None or files == ():
         pattern = re.compile("^(?!_).*.abml$")
         files = list(filter(pattern.match, os.listdir(".")))
     for file in files:
         file = os.path.basename(file)
         extension = file.split(".")[-1]
-        processed = cae_reg.get(extension, abml_file_mode)(file, parameters, env, config=config)
+
+        processed = cae_reg.get(extension, abml_file_mode)(
+            file,
+            parameters,
+            env,
+            config=config,
+            test=test,
+        )
 
     if processed is False:
         console.print("no abml File found!", style="bold red")
 
 
 def load_grid(env, parameters, filename="_grids.abml"):
     grids = {}
```

### Comparing `abml-cli-0.1.4/abml_cli/abml_parser.py` & `abml_cli-0.1.6/abml_cli/abml_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,84 @@
 from json import loads, dumps
 import ast
 import argparse
 from io import open
 
 from abml.abml_dataclass import Abml_Cae
 from abml.abml_helpers import exit_handler, cprint
-
 from yaml import load as yload
 from yaml import Loader
 import os
 
 import logging
 
+
+def str_to_bool(value):
+    if isinstance(value, bool):
+        return value
+    if value.lower() in ("yes", "true", "t", "y", "1"):
+        return True
+    elif value.lower() in ("no", "false", "f", "n", "0"):
+        return False
+    else:
+        raise argparse.ArgumentTypeError("Boolean value expected.")
+
+
 parser = argparse.ArgumentParser()
 
 group = parser.add_mutually_exclusive_group(required=True)
 group.add_argument("--cae", type=str, default=None)
 group.add_argument("--file", type=str, default=None)
 parser.add_argument("--name", type=str, default=None)
-parser.add_argument("--input_type", type=str, default="copy")
+parser.add_argument("--input_type", type=str, default=None)
 parser.add_argument("--input_folder", type=str, default="inputs")
+parser.add_argument("--test", type=str_to_bool, default=False)
 
 args, _ = parser.parse_known_args()
 
 if args.cae is not None:
     args_string = args.cae.replace("'", '"')
     cae = ast.literal_eval(dumps(loads(args.cae.replace("'", '"'), encoding="utf-8")))
 elif args.file is not None:
     with open(args.file, mode="r", encoding="utf-8") as f:
         cae = yload(f, Loader=Loader)
 
 
 if __name__ == "__main__":
-    logger = logging.getLogger("abml_logger")
-    logger.setLevel(logging.DEBUG)
+    logger = logging.getLogger()
+
+    if args.test:
+        logger.setLevel(logging.INFO)
+
     fh = logging.FileHandler(
         filename="{}.abml.log".format(args.name),
         mode="w",
         encoding="utf-8",
     )
     formatter = logging.Formatter("%(levelname)s - %(module)s - %(message)s")
     fh.setFormatter(formatter)
     logger.addHandler(fh)
 
-    logger.info("test")
-    logger.debug("test")
-
     if "cae" in globals():
-        cae = Abml_Cae(cae)
+        cae = Abml_Cae(cae, test=args.test)
         exit_handler()
 
-        cae.save_cae("{}.cae".format(args.name))
-
-        if args.input_type == "copy":
-            if not os.path.isdir(args.input_folder):
-                os.mkdir(args.input_folder)
-            for model in cae.models:
-                if hasattr(cae.models[model], "jobs"):
-                    for job in cae.models[model].jobs:
-                        cae.models[model].jobs[job].write_and_copy_input_to_path(args.input_folder)
-
-        elif args.input_type == "move":
-            if not os.path.isdir(args.input_folder):
-                os.mkdir(args.input_folder)
-            for model in cae.models:
-                if hasattr(cae.models[model], "jobs"):
-                    for job in cae.models[model].jobs:
-                        cae.models[model].jobs[job].write_and_move_input_to_path(args.input_folder)
+        cprint(args.test)
+        if not args.test:
+            cprint(args.test)
+            cae.save_cae("{}.cae".format(args.name))
+
+            if args.input_type == "copy":
+                if not os.path.isdir(args.input_folder):
+                    os.mkdir(args.input_folder)
+                for model in cae.models:
+                    if hasattr(cae.models[model], "jobs"):
+                        for job in cae.models[model].jobs:
+                            cae.models[model].jobs[job].write_and_copy_input_to_path(args.input_folder)
+
+            elif args.input_type == "move":
+                if not os.path.isdir(args.input_folder):
+                    os.mkdir(args.input_folder)
+                for model in cae.models:
+                    if hasattr(cae.models[model], "jobs"):
+                        for job in cae.models[model].jobs:
+                            cae.models[model].jobs[job].write_and_move_input_to_path(args.input_folder)
```

### Comparing `abml-cli-0.1.4/abml_cli/abml_subroutines.py` & `abml_cli-0.1.6/abml_cli/abml_subroutines.py`

 * *Files identical despite different names*

### Comparing `abml-cli-0.1.4/abml_cli/dataclasses/abml_schema.json` & `abml_cli-0.1.6/abml_cli/dataclasses/abml_schema.json`

 * *Files identical despite different names*

### Comparing `abml-cli-0.1.4/abml_cli/dataclasses/model.py` & `abml_cli-0.1.6/abml_cli/dataclasses/model.py`

 * *Files identical despite different names*

### Comparing `abml-cli-0.1.4/abml_cli/dataclasses/template_schema.json` & `abml_cli-0.1.6/abml_cli/dataclasses/template_schema.json`

 * *Files identical despite different names*

### Comparing `abml-cli-0.1.4/pyproject.toml` & `abml_cli-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abml-cli"
-version = "0.1.4"
+version = "0.1.6"
 description = ""
 authors = ["DavidNaizheZhou <70525024+DavidNaizheZhou@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "abml_cli"} ]
 
 [tool.poetry.dependencies]
 python = ">3.8"
```

### Comparing `abml-cli-0.1.4/setup.py` & `abml_cli-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 entry_points = \
 {'console_scripts': ['abml = abml_cli.abml_exec:run',
                      'abml-grid = abml_cli.abml_exec:run_grid',
                      'jnl = abml_cli.helpers:extract_data_from_jnl']}
 
 setup_kwargs = {
     'name': 'abml-cli',
-    'version': '0.1.4',
+    'version': '0.1.6',
     'description': '',
     'long_description': '',
     'author': 'DavidNaizheZhou',
     'author_email': '70525024+DavidNaizheZhou@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `abml-cli-0.1.4/PKG-INFO` & `abml_cli-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: abml-cli
-Version: 0.1.4
+Version: 0.1.6
 Summary: 
 Author: DavidNaizheZhou
 Author-email: 70525024+DavidNaizheZhou@users.noreply.github.com
 Requires-Python: >3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: abqpy (>=2023.4.3,<2024.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: invoke (>=2.0.0,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
```

