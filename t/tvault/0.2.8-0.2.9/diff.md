# Comparing `tmp/tvault-0.2.8-py3-none-any.whl.zip` & `tmp/tvault-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9077 bytes, number of entries: 10
+Zip file size: 9173 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     1455 b- defN 23-Apr-10 04:16 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
--rw-r--r--  2.0 unx     5737 b- defN 23-Apr-05 05:40 tvault/parse_utils.py
--rw-r--r--  2.0 unx    12413 b- defN 23-Apr-10 04:10 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:16 tvault-0.2.8.dist-info/RECORD
-10 files, 26700 bytes uncompressed, 7791 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx     6290 b- defN 23-Apr-10 04:24 tvault/parse_utils.py
+-rw-r--r--  2.0 unx    12514 b- defN 23-Apr-10 04:26 tvault/torchvault.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      760 b- defN 23-Apr-10 04:26 tvault-0.2.9.dist-info/RECORD
+10 files, 27354 bytes uncompressed, 7887 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.2.8.dist-info/LICENSE
+Filename: tvault-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.2.8.dist-info/METADATA
+Filename: tvault-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.2.8.dist-info/WHEEL
+Filename: tvault-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.2.8.dist-info/top_level.txt
+Filename: tvault-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.2.8.dist-info/RECORD
+Filename: tvault-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/parse_utils.py

```diff
@@ -78,28 +78,33 @@
 
 
 def print_util(diff_dict):
     large_space = 40
     space = 30
     ret_str = ""
 
-    ret_str += "=" * large_space + "MODEL DIFF" + "=" * large_space + "\n"
-    ret_str += diff_dict["model"] + "\n"
+    if len(diff_dict["model"]) > 0:
+        ret_str += "=" * large_space + "MODEL DIFF" + "=" * large_space + "\n"
+        ret_str += diff_dict["model"] + "\n"
 
     if len(diff_dict["src"].keys()) > 0:
         ret_str += "=" * large_space + "SRC DIFF" + "=" * large_space + "\n"
         for k, v in diff_dict["src"].items():
             ret_str += "=" * space + f"{k}" + "=" * space + "\n"
             ret_str += v + "\n"
 
     if len(diff_dict["func"].keys()) > 0:
         ret_str += "=" * large_space + "FUNC DIFF" + "=" * large_space + "\n"
         for k, v in diff_dict["func"].items():
             ret_str += "=" * space + f"{k}" + "=" * space + "\n"
             ret_str += v + "\n"
+
+    if len(diff_dict["optimizer"]) > 0:
+        ret_str += "=" * large_space + "OPTIM DIFF" + "=" * large_space + "\n"
+        ret_str += diff_dict["optimizer"] + "\n"
     return ret_str
 
 
 def extract_diff(prev_model, cur_model):
     diff_dict = dict()
     # 1. get model diff using string
     model_diff = [
@@ -146,10 +151,21 @@
         else:
             func_diff_dict[p_func] = "function removed"
     for c_func, c_source in cur_model["external_func"].items():
         if c_func not in prev_model["external_func"].keys():
             func_diff_dict[c_func] = "function added"
     diff_dict["func"] = func_diff_dict
 
+    # 4. Check optimizer diff
+    opt_diff = [
+        e
+        for e in difflib.ndiff(
+            prev_model["optimizer"].split("\n"), cur_model["optimizer"].split("\n")
+        )
+    ]
+    filter_opt_diff = [l for l in opt_diff if not l.startswith("? ")]
+    opt_diff = "\n".join(filter_opt_diff)
+    diff_dict["optimizer"] = opt_diff
+
     ret_str = print_util(diff_dict)
 
     return ret_str, diff_dict
```

## tvault/torchvault.py

```diff
@@ -245,15 +245,18 @@
             for k, v in diff_dict["src"].items():
                 feed_gpt += v + "\n"
 
         if len(diff_dict["func"].keys()) > 0:
             for k, v in diff_dict["func"].items():
                 feed_gpt += v + "\n"
 
-        print("=" * 20 + "Source Diff" + "=" * 20)
+        if len(diff_dict["optimizer"]) > 0:
+            feed_gpt += diff_dict["optimizer"] + "\n"
+
+        print("=" * 20 + "GPT FED INPUT" + "=" * 20)
         print(feed_gpt)
         model = "gpt-3.5-turbo"
         query = f"This is a string diff of two pytorch models. Please explain the difference of the two models. You do not need to explain model itself. Only elaborate on model differences. Only refer to diff sentences that starts with + or - signs. Do not refer to any other code parts. Use bulletpoints.\n{feed_gpt}"
         messages = [
             {
                 "role": "system",
                 "content": "You are a very talented machine learning engineer. Your job is to explain difference of two pytorch models in easy words. You are expected to answer in smallest number of senteces as possible.",
```

## Comparing `tvault-0.2.8.dist-info/LICENSE` & `tvault-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvault-0.2.8.dist-info/RECORD` & `tvault-0.2.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tvault/__init__.py,sha256=XV3fMuqbI9ErJxH59gLGAV-YlC5uYV_wdzQFLflMGoE,1455
 tvault/model_diff.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tvault/model_log.py,sha256=ZD1LeL1wBRKQEZaAfZEcjYP7w76yeD0eMRAnI-fBOiA,4789
-tvault/parse_utils.py,sha256=1gNwxk5UScEHIF_TG1te3r_gsYtFUaZTkWziLczvZ8I,5737
-tvault/torchvault.py,sha256=E88y2zTJKA9yAHE32vkOnf9IGrghqBasRcBe78aFOVI,12413
-tvault-0.2.8.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
-tvault-0.2.8.dist-info/METADATA,sha256=srgiLBc_c4juJwtw72Rc0al0N9d4Jp_l6rct8cnu1Rc,380
-tvault-0.2.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tvault-0.2.8.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
-tvault-0.2.8.dist-info/RECORD,,
+tvault/parse_utils.py,sha256=ZP34OV4DTXQCGlv-faswTq0md_wxdIOS7aLeP39RKoQ,6290
+tvault/torchvault.py,sha256=E0w1GFOVrZmxrDNZpswn_cTxhRXqE4BkZJQ1a_ASa6M,12514
+tvault-0.2.9.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
+tvault-0.2.9.dist-info/METADATA,sha256=c4Iz1Ap4-vWnLaTin0mtsQSwTTV4KOfsdbcxQsRHWDo,380
+tvault-0.2.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+tvault-0.2.9.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
+tvault-0.2.9.dist-info/RECORD,,
```

