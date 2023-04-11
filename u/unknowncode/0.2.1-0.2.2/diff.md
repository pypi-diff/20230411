# Comparing `tmp/unknowncode-0.2.1.tar.gz` & `tmp/unknowncode-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unknowncode-0.2.1.tar", max compression
+gzip compressed data, was "unknowncode-0.2.2.tar", max compression
```

## Comparing `unknowncode-0.2.1.tar` & `unknowncode-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2038 2023-03-31 13:34:42.788602 unknowncode-0.2.1/docs/README.md
--rw-r--r--   0        0        0      498 2023-03-31 13:35:55.948503 unknowncode-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      500 2023-03-31 13:35:59.492498 unknowncode-0.2.1/unknowncode/__init__.py
--rw-r--r--   0        0        0     2705 2023-03-31 13:36:10.933391 unknowncode-0.2.1/setup.py
--rw-r--r--   0        0        0     2520 2023-03-31 13:36:10.937464 unknowncode-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2038 2023-03-31 13:34:42.788602 unknowncode-0.2.2/docs/README.md
+-rw-r--r--   0        0        0      498 2023-04-11 14:02:54.010297 unknowncode-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-04-11 14:02:58.734293 unknowncode-0.2.2/unknowncode/__init__.py
+-rw-r--r--   0        0        0     2705 2023-04-11 14:03:22.863012 unknowncode-0.2.2/setup.py
+-rw-r--r--   0        0        0     2520 2023-04-11 14:03:22.863427 unknowncode-0.2.2/PKG-INFO
```

### Comparing `unknowncode-0.2.1/docs/README.md` & `unknowncode-0.2.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `unknowncode-0.2.1/setup.py` & `unknowncode-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['unknowncode']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'unknowncode',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Small portions of code I use, gathered into one group for ease of access. Like a mod library for a game. Built with poetry',
     'long_description': '# UnknownCode Guide/Compendium\n\n## This file is a list of all the information and commands in unknowncode.\nArguments in **Bold** are required arguments.\nArguments in *Italics* are optional arguments\n\n##### custom_response(**response_list**,**cap_sense**,**prompt**)\n> response_list is a list of (guess what?) allowed responses, anything you want a user to be able to reply with\nExample: `response_list = ["Sure","Yeah!"]`\ncap_sense is wether you want it to be Case Sensitive. If True then it will be Case Sensitive.\nprompt is any string that you want the user to respond to\nExample: `prompt = "Are you ready to code?"`\n\n##### yes_no(**prompt**)\n> yes_no() is a preset version of custom_response_input, preset with a list of ["Yes","yes","Y","y"]`.\nprompt is any string that you want the user to respond to\nExample: `prompt = "Are you ready to code?"`\nIf the user respondses with anything that is Yes or Y (includng lowercase)\n\n\n\n# UnknownCode Changelog 0.2.0 (Last version 0.1.0)\n\n##### Added:\n>README.md\nCHANGELOG.md\ncustom_response()\n#\n# UnknownCode Guide/Compendium\n###### (version 0.2.1)\n---\nArguments in **Bold** are required arguments.\nArguments in *Italics* are optional arguments\n\n##### custom_response(**response_list**,**cap_sense**,**prompt**)\n#\n> response_list is a list of (guess what?) allowed responses, anything you want a user to be able to reply with\nExample: `response_list = ["Sure","Yeah!"]`\ncap_sense is wether you want it to be Case Sensitive. If True then it will be Case Sensitive.\nprompt is any string that you want the user to respond to\nExample: `prompt = "Are you ready to code?"`\n\n##### yes_no(**prompt**)\n#\n> yes_no() is a preset version of custom_response_input, preset with a list of ["Yes","yes","Y","y"]`.\nprompt is any string that you want the user to respond to\nExample: `prompt = "Are you ready to code?"`\nIf the user respondses with anything that is Yes or Y (includng lowercase)\n\n#\n---\n#\n\n## UnknownCode Changelog 0.2.1 (Last version 0.2.1)\n\n##### Added:\n#\n>README.md\nCHANGELOG.md\ncustom_response()',
     'author': 'UnknownSources',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `unknowncode-0.2.1/PKG-INFO` & `unknowncode-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unknowncode
-Version: 0.2.1
+Version: 0.2.2
 Summary: Small portions of code I use, gathered into one group for ease of access. Like a mod library for a game. Built with poetry
 License: MIT
 Keywords: library,Quality of Life,QoL
 Author: UnknownSources
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

