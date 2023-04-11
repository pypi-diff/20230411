# Comparing `tmp/cybarpass-2.2.tar.gz` & `tmp/cybarpass-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybarpass-2.2.tar", last modified: Tue Apr  4 18:35:39 2023, max compression
+gzip compressed data, was "cybarpass-2.3.tar", last modified: Tue Apr 11 02:55:26 2023, max compression
```

## Comparing `cybarpass-2.2.tar` & `cybarpass-2.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-04 05:34:16.625403 cybarpass-2.2/LICENSE
--rw-r--r--   0        0        0     2820 2023-04-04 18:31:40.317028 cybarpass-2.2/README.md
--rw-r--r--   0        0        0      686 2023-04-04 18:35:39.874331 cybarpass-2.2/pyproject.toml
--rw-r--r--   0        0        0       91 2023-04-04 18:28:38.010653 cybarpass-2.2/src/cybarpass/__init__.py
--rwxr-xr-x   0        0        0     1138 2023-04-04 18:10:31.140013 cybarpass-2.2/src/cybarpass/__main__.py
--rw-r--r--   0        0        0      333 2023-04-04 18:28:31.775227 cybarpass-2.2/src/cybarpass/__runner.py
--rw-r--r--   0        0        0     5348 2023-04-04 18:27:54.865690 cybarpass-2.2/src/cybarpass/app.py
--rw-r--r--   0        0        0     1164 2023-04-04 18:21:15.006563 cybarpass-2.2/src/cybarpass/passgen.py
--rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 cybarpass-2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-04 05:34:16.625403 cybarpass-2.3/LICENSE
+-rw-r--r--   0        0        0     2820 2023-04-04 18:43:24.247855 cybarpass-2.3/README.md
+-rw-r--r--   0        0        0      686 2023-04-11 02:55:26.669422 cybarpass-2.3/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-11 02:54:27.204769 cybarpass-2.3/src/cybarpass/__init__.py
+-rwxr-xr-x   0        0        0     1194 2023-04-10 03:36:16.270388 cybarpass-2.3/src/cybarpass/__main__.py
+-rw-r--r--   0        0        0      333 2023-04-04 18:28:31.775227 cybarpass-2.3/src/cybarpass/__runner.py
+-rw-r--r--   0        0        0     5284 2023-04-10 02:59:38.483057 cybarpass-2.3/src/cybarpass/app.py
+-rw-r--r--   0        0        0     1164 2023-04-04 18:21:15.006563 cybarpass-2.3/src/cybarpass/passgen.py
+-rw-r--r--   0        0        0  2493977 2023-04-10 03:22:04.313188 cybarpass-2.3/src/cybarpass/words
+-rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 cybarpass-2.3/PKG-INFO
```

### Comparing `cybarpass-2.2/LICENSE` & `cybarpass-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cybarpass-2.2/README.md` & `cybarpass-2.3/README.md`

 * *Files identical despite different names*

### Comparing `cybarpass-2.2/pyproject.toml` & `cybarpass-2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "cybarpass"
-version = "2.2"
+version = "2.3"
 authors = [
     { name = "cybardev", email = "sheikh@cybar.dev" },
 ]
 description = "Minimalistic Passphrase Generation script with GUI"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cybarpass-2.2/src/cybarpass/__main__.py` & `cybarpass-2.3/src/cybarpass/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python3
 
+import os
+import sys
 import argparse
 from .__runner import run
 
 if __name__ == "__main__":
     # argument parsing
     parser = argparse.ArgumentParser(
         description="Generate a secure passphrase",
@@ -15,15 +17,15 @@
     )
     parser.add_argument(
         "filename",
         help="Path to dictionary file",
         metavar="WORD_LIST",
         type=str,
         nargs="?",
-        default=None,
+        default=f"{os.path.dirname(sys.argv[0])}/words",
     )
     parser.add_argument(
         "-n",
         "--len",
         help="Minimum length of passphrase",
         dest="char_limit",
         metavar="NUM",
```

### Comparing `cybarpass-2.2/src/cybarpass/app.py` & `cybarpass-2.3/src/cybarpass/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tkinter.filedialog import askopenfilename
 from tkinter.ttk import Combobox, Frame
 from .passgen import PassGen
 
 # map of constants
 CONST = MappingProxyType(
     {
-        "win-title": "PassGen",
+        "win-title": "CybarPass",
         "win-width": 450,
         "win-height": 200,
         "pass-strength": {"Low": 16, "Medium": 24, "High": 32},
     }
 )
 
 
@@ -84,17 +84,15 @@
         self.__lbl_password.grid(row=0, column=0)
 
     def entry_password(self) -> None:
         self.__entry_password = tk.Entry(
             self.__container,
             textvariable=self.__txt_password,
         )
-        self.__entry_password.grid(
-            row=0, column=1, columnspan=2, sticky=tk.EW, padx=16
-        )
+        self.__entry_password.grid(row=0, column=1, columnspan=2, sticky=tk.EW, padx=16)
 
     # --- word list UI items --- #
 
     def lbl_word_list(self) -> None:
         self.__lbl_password = tk.Label(self.__container, text="Word List:")
         self.__lbl_password.grid(row=1, column=0)
 
@@ -121,17 +119,15 @@
         self.__lbl_password.grid(row=2, column=0)
 
     def combo_strength(self) -> None:
         self.__strength = Combobox(self.__container, width=18)
         self.__strength["values"] = tuple(CONST["pass-strength"].keys())
         self.__strength["state"] = "readonly"
         self.__strength.current(0)
-        self.__strength.grid(
-            row=2, column=1, columnspan=2, sticky=tk.EW, padx=16
-        )
+        self.__strength.grid(row=2, column=1, columnspan=2, sticky=tk.EW, padx=16)
 
     # --- action button group --- #
 
     def btn_generate(self) -> None:
         self.__btn_generate = tk.Button(
             self.__container,
             text="Generate",
@@ -159,17 +155,15 @@
 
     def __word_file(self, filename) -> None:
         if filename:
             self.__word_list_filename.set(filename)
             self.__passgen.word_list = self.__word_list_filename.get()
 
     def __show_pass(self) -> None:
-        self.__passgen.char_limit = CONST["pass-strength"][
-            self.__strength.get()
-        ]
+        self.__passgen.char_limit = CONST["pass-strength"][self.__strength.get()]
         self.__txt_password.set(self.__passgen.passphrase)
 
     def __copy_pass(self, passphrase: str) -> None:
         if passphrase:
             self.__container.clipboard_clear()
             self.__container.clipboard_append(passphrase)
```

### Comparing `cybarpass-2.2/src/cybarpass/passgen.py` & `cybarpass-2.3/src/cybarpass/passgen.py`

 * *Files identical despite different names*

### Comparing `cybarpass-2.2/PKG-INFO` & `cybarpass-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybarpass
-Version: 2.2
+Version: 2.3
 Summary: Minimalistic Passphrase Generation script with GUI
 Home-page: https://pass.cybar.dev
 Author-Email: cybardev <sheikh@cybar.dev>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://pass.cybar.dev
```

