# Comparing `tmp/tvault-0.2.9-py3-none-any.whl.zip` & `tmp/tvault-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 9173 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1455 b- defN 23-Apr-10 04:16 tvault/__init__.py
+Zip file size: 9855 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     2842 b- defN 23-Apr-11 06:23 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
--rw-r--r--  2.0 unx     6290 b- defN 23-Apr-10 04:24 tvault/parse_utils.py
--rw-r--r--  2.0 unx    12514 b- defN 23-Apr-10 04:26 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/RECORD
-10 files, 27354 bytes uncompressed, 7887 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     6606 b- defN 23-Apr-11 06:17 tvault/parse_utils.py
+-rw-r--r--  2.0 unx    13032 b- defN 23-Apr-11 05:35 tvault/torchvault.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-11 06:23 tvault-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-11 06:23 tvault-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 06:23 tvault-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-11 06:23 tvault-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 06:23 tvault-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-11 06:23 tvault-0.3.0.dist-info/RECORD
+11 files, 29722 bytes uncompressed, 8415 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.2.9.dist-info/LICENSE
+Filename: tvault-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.2.9.dist-info/METADATA
+Filename: tvault-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.2.9.dist-info/WHEEL
+Filename: tvault-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.2.9.dist-info/top_level.txt
+Filename: tvault-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: tvault-0.2.9.dist-info/RECORD
+Filename: tvault-0.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: tvault-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/__init__.py

```diff
@@ -1,9 +1,9 @@
 from .torchvault import TorchVault
-
+import click
 
 """
 Logging Functions
 """
 
 
 def log(model, log_dir="./model_log", model_dir="./"):
@@ -33,23 +33,71 @@
 
 
 def add_result(result=0, sha="", log_dir="./model_log"):
     vault = TorchVault(log_dir)
     vault.add_result(sha, result)
 
 
-def log_all(model, tag="", result=0, log_dir="./model_log", model_dir="./"):
+def log_all(model, tag="", result=-1, optimizer=None, log_dir="./model_log", model_dir="./"):
     vault = TorchVault(log_dir, model_dir)
     vault.log_model(model)
-    vault.add_tag("", tag)
-    vault.add_result("", result)
+    if optimizer is not None:
+        vault.log_optimizer(optimizer)
+    if tag is not "":
+        vault.add_tag("", tag)
+    if result is not -1:
+        vault.add_result("", result)
 
 
 """
 Other utils
 """
 
 
 def find(log_dir="./model_log", model_dir="./", condition="hash", hash="", tag="", min=0, max=100):
     vault = TorchVault(log_dir, model_dir)
-    vault.find(condition, hash, tag, min, max)
-    vault.show_result(hash)
+    target_models = vault.find(condition, hash, tag, min, max)
+    vault.show_result(target_models)
+
+
+"""
+cli utils
+"""
+
+
+@click.command()
+@click.option("--find_flag", is_flag=True, default=False, help="tvault cli for tvault.find")
+@click.option("--diff_flag", is_flag=True, default=False, help="tvault cli for tvault.diff")
+# options for find
+@click.option("--log_dir", type=str, default="./model_log")
+@click.option("--model_dir", type=str, default="./")
+@click.option("--condition", type=str, default="hash")
+@click.option("--hash", type=str, default="")
+@click.option("--tag", type=str, default="")
+@click.option("--min", type=int, default=0)
+@click.option("--max", type=int, default=100)
+# options for diff
+@click.option("--sha1", type=str, default="")
+@click.option("--index1", type=int, default="")
+@click.option("--sha2", type=str, default="")
+@click.option("--index2", type=int, default="")
+def cli_main(
+    find_flag,
+    diff_flag,
+    log_dir,
+    model_dir,
+    condition,
+    hash,
+    tag,
+    min,
+    max,
+    sha1,
+    index1,
+    sha2,
+    index2,
+):
+    if find_flag:
+        find(log_dir, model_dir, condition, hash, tag, min, max)
+    elif diff_flag:
+        diff(sha1, index1, sha2, index2, out=False, ask_gpt=False, log_dir=log_dir)
+    else:
+        print("tvault: not implemented")
```

## tvault/parse_utils.py

```diff
@@ -107,16 +107,20 @@
 def extract_diff(prev_model, cur_model):
     diff_dict = dict()
     # 1. get model diff using string
     model_diff = [
         e for e in difflib.ndiff(prev_model["model"].split("\n"), cur_model["model"].split("\n"))
     ]
     filter_model_diff = [l for l in model_diff if not l.startswith("? ")]
-    model_diff = "\n".join(filter_model_diff)
-    diff_dict["model"] = model_diff
+    changes = [l for l in model_diff if l.startswith("+ ") or l.startswith("- ")]
+    if len(changes) > 0:
+        model_diff = "\n".join(filter_model_diff)
+        diff_dict["model"] = model_diff
+    else:
+        diff_dict["model"] = ""
 
     # 2. Check module definition between modules
     class_diff_dict = dict()
     for p_module, p_source in prev_model["src"].items():
         # if module still exists in current model
         if p_module in cur_model["src"].keys():
             class_diff = [
@@ -159,13 +163,17 @@
     opt_diff = [
         e
         for e in difflib.ndiff(
             prev_model["optimizer"].split("\n"), cur_model["optimizer"].split("\n")
         )
     ]
     filter_opt_diff = [l for l in opt_diff if not l.startswith("? ")]
-    opt_diff = "\n".join(filter_opt_diff)
-    diff_dict["optimizer"] = opt_diff
+    changes = [l for l in opt_diff if l.startswith("+ ") or l.startswith("- ")]
+    if len(changes) > 0:
+        opt_diff = "\n".join(filter_opt_diff)
+        diff_dict["optimizer"] = opt_diff
+    else:
+        diff_dict["optimizer"] = ""
 
     ret_str = print_util(diff_dict)
 
     return ret_str, diff_dict
```

## tvault/torchvault.py

```diff
@@ -1,21 +1,20 @@
 import os
 import sys
 import ast
 import git
-import json
 import openai
 import pickle
 import astunparse
 from prettytable import PrettyTable
 from collections import defaultdict
 
 from .parse_utils import match_external_funcs, extract_info_from_model, extract_diff
 
-OPENAI_API_KEY = "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"
+OPENAI_API_KEY = "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"
 openai.api_key = OPENAI_API_KEY
 
 
 class TorchVaultError(Exception):
     pass
 
 
@@ -60,26 +59,24 @@
     """
     log torch scheduler 
     """
 
     def log_scheduler(self, scheduler):
         model_log = self.read_model_log()
         model_idx = len(model_log.keys()) - 1
-        print(f"model idx - add scheduler: {model_idx}")
         model_log[model_idx]["scheduler"] = scheduler.__str__()
         self.write_model_log("", model_log)
 
     """
     log torch optimizer
     """
 
     def log_optimizer(self, optimizer):
         model_log = self.read_model_log()
         model_idx = len(model_log.keys()) - 1
-        print(f"model idx - add optimizer: {model_idx}")
         model_log[model_idx]["optimizer"] = optimizer.__str__()
         self.write_model_log("", model_log)
 
     """
     add tag to model log, commit sha may be from previous results.
     if idx is set to -1, all models in the commit hash are tagged.
     if idx is set to None, tag of most recent model is changed.
@@ -105,15 +102,14 @@
             if "tag" in model_log[model_idx].keys():
                 print(
                     f"tvault: changing tag from {model_log[model_idx]['tag']} to {tag} for model {sha}"
                 )
             else:
                 print(f"tvault: setting tag {tag} for model {sha}")
             model_log[model_idx]["tag"] = tag
-        print(f"write log: {model_log}")
         self.write_model_log(sha, model_log)
 
     """
     add result to model log, commit sha may be from previous results.
     if idx is set to -1, all models in the commit hash are tagged.
     if idx is set to None, tag of most recent model is changed.
     """
@@ -138,15 +134,14 @@
             if "result" in model_log[model_idx].keys():
                 print(
                     f"tvault: changing result from {model_log[model_idx]['result']} to {result} for model {sha}"
                 )
             else:
                 print(f"tvault: setting result {result} for model {sha}")
             model_log[model_idx]["result"] = result
-        print(f"write log: {model_log}")
         self.write_model_log(sha, model_log)
 
     """
     Basic logging for pytorch model.
     1. Retrives target modules from pytorch model representation.
     2. Get class definition of target modules.
     3. Get external function definition of those used in target model.
@@ -181,19 +176,17 @@
                 if self.use_astunparse:
                     filter_target_funcs[k] = astunparse.unparse(v)
                 else:
                     filter_target_funcs[k] = ast.unparse(v)
 
         model_log = self.read_model_log()
         model_idx = len(model_log.keys())
-        print(f"model idx: {model_idx}")
         model_log[model_idx]["model"] = model.__str__()
         model_log[model_idx]["src"] = dict(filter_target_class)
         model_log[model_idx]["external_func"] = dict(filter_target_funcs)
-        print(f"write model in model log {model_log}")
         self.write_model_log("", model_log)
 
     """
     Basic diff calculator between two pytorch models.
     sha1: commit hash of previous model, must be set. (for now)
     index1: model index of model in commit hash sha1. If not set, use latest.
     sha2: commit hash of current model, must be set. (for now)
@@ -210,16 +203,16 @@
         if len(cur_model.keys()) == 0:
             print(f"tvault error: sha2 argument must be provided.")
         if index1 == -1:
             index1 = len(prev_model.keys()) - 1
         if index2 == -1:
             index2 = len(cur_model.keys()) - 1
 
-        prev_model = prev_model[str(index1)]
-        cur_model = cur_model[str(index2)]
+        prev_model = prev_model[index1]
+        cur_model = cur_model[index2]
 
         ret_str, diff_dict = extract_diff(prev_model, cur_model)
 
         if out:
             with open(f"{self.log_dir}/diff_{sha1}_{sha2}", "w") as f:
                 f.write(ret_str)
         print(ret_str)
@@ -248,81 +241,99 @@
         if len(diff_dict["func"].keys()) > 0:
             for k, v in diff_dict["func"].items():
                 feed_gpt += v + "\n"
 
         if len(diff_dict["optimizer"]) > 0:
             feed_gpt += diff_dict["optimizer"] + "\n"
 
-        print("=" * 20 + "GPT FED INPUT" + "=" * 20)
+        print("=" * 40 + "GPT FED INPUT" + "=" * 40)
         print(feed_gpt)
         model = "gpt-3.5-turbo"
         query = f"This is a string diff of two pytorch models. Please explain the difference of the two models. You do not need to explain model itself. Only elaborate on model differences. Only refer to diff sentences that starts with + or - signs. Do not refer to any other code parts. Use bulletpoints.\n{feed_gpt}"
         messages = [
             {
                 "role": "system",
                 "content": "You are a very talented machine learning engineer. Your job is to explain difference of two pytorch models in easy words. You are expected to answer in smallest number of senteces as possible.",
             },
             {"role": "user", "content": query},
         ]
         response = openai.ChatCompletion.create(model=model, messages=messages)
         answer = response["choices"][0]["message"]["content"]
         print("\n\n")
-        print("=" * 20 + "ChatGPT Answer" + "=" * 20)
+        print("=" * 40 + "ChatGPT Answer" + "=" * 40)
         print(answer)
         return
 
     """
     find models using either commit hash, tag, or result
+    should find suitable models and return list of [hash, model index, tag, result].
     """
 
     def find(self, condition="hash", hash="", tag="", min=0, max=100):
+        target_models = []
         if os.path.exists(self.log_dir):
             if len(os.listdir(self.log_dir)) == 0:
                 print(f"tvault error: log dir is empty")
                 raise TorchVaultError
             if condition == "hash":
                 if hash == "":
                     print(f"tvault error: hash is not set for hash finding")
                     raise TorchVaultError
                 if os.path.exists(f"{self.log_dir}/model_{hash}"):
                     model_log = self.read_model_log(hash)
                     print(
                         f"tvault: model {hash} exists! - contains {len(model_log.keys())} experiments"
                     )
+                    for model_idx, model in model_log.items():
+                        model_info = [hash, model_idx]
+                        if "tag" in model.keys():
+                            model_info.append(model["tag"])
+                        else:
+                            model_info.append("")
+                        if "result" in model.keys():
+                            model_info.append(model["result"])
+                        else:
+                            model_info.append(-1)
+                        target_models.append(model_info)
+
                 else:
                     print(f"tvault: model {hash} does not exist.")
             elif condition == "tag":
-                target_models = []
                 for model in os.listdir(self.log_dir):
                     with open(f"{self.log_dir}/{model}", "rb") as f:
                         model_log = pickle.load(f)
                     for model_idx, v in model_log.items():
+                        model_info = []
                         if "tag" in v.keys() and v["tag"] == tag:
-                            target_models.append([model, model_idx])
-                print(f"tvault: models {target_models} match tag {tag}.")
+                            model_info = [model, model_idx, v["tag"]]
+                            if "result" in v.keys():
+                                model_info.append(v["result"])
+                            else:
+                                model_info.append(-1)
+                            target_models.append(model_info)
             elif condition == "result":
-                target_models = []
                 for model in os.listdir(self.log_dir):
                     with open(f"{self.log_dir}/{model}", "rb") as f:
                         model_log = pickle.load(f)
                     for model_idx, v in model_log.items():
+                        model_info = []
                         if "result" in v.keys() and min <= v["result"] <= max:
-                            target_models.append([model, model_idx])
-                print(f"tvault: models {target_models} have result between {min} ~ {max}.")
+                            if "tag" in v.keys():
+                                model_info = [model, model_idx, v["tag"], v["result"]]
+                            else:
+                                model_info = [model, model_idx, "", v["result"]]
+                            target_models.append(model_info)
             else:
                 print(f"tvault error:condition other than [hash, tag, result] is not supported.")
                 raise TorchVaultError
+        return target_models
 
-    def show_result(self, sha=""):
-        model_log = self.read_model_log(sha)
-        if len(model_log.keys()) == 0:
-            print(f"tvault error: model log with commit hash {sha} is empty.")
-            raise TorchVaultError
+    def show_result(self, target_models):
+        if len(target_models) == 0:
+            print(f"tvault: no model satisfying the conditions")
+            return
 
-        target_idxs = [*range(len(model_log.keys()))]
-        table = ["MODEL-IDX", "RESULT"]
+        table = ["HASH", "MODEL-IDX", "TAG", "RESULT"]
         tab = PrettyTable(table)
-        for i in target_idxs:
-            target_model = model_log[i]
-            if "result" in target_model.keys():
-                tab.add_row([i, target_model["result"]])
+        for e in target_models:
+            tab.add_row(e)
         print(tab)
```

## Comparing `tvault-0.2.9.dist-info/LICENSE` & `tvault-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

