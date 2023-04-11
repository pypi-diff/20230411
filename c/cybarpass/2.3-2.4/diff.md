# Comparing `tmp/cybarpass-2.3.tar.gz` & `tmp/cybarpass-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybarpass-2.3.tar", last modified: Tue Apr 11 02:55:26 2023, max compression
+gzip compressed data, was "cybarpass-2.4.tar", last modified: Tue Apr 11 03:15:19 2023, max compression
```

## Comparing `cybarpass-2.3.tar` & `cybarpass-2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-04 05:34:16.625403 cybarpass-2.3/LICENSE
--rw-r--r--   0        0        0     2820 2023-04-04 18:43:24.247855 cybarpass-2.3/README.md
--rw-r--r--   0        0        0      686 2023-04-11 02:55:26.669422 cybarpass-2.3/pyproject.toml
--rw-r--r--   0        0        0       91 2023-04-11 02:54:27.204769 cybarpass-2.3/src/cybarpass/__init__.py
--rwxr-xr-x   0        0        0     1194 2023-04-10 03:36:16.270388 cybarpass-2.3/src/cybarpass/__main__.py
--rw-r--r--   0        0        0      333 2023-04-04 18:28:31.775227 cybarpass-2.3/src/cybarpass/__runner.py
--rw-r--r--   0        0        0     5284 2023-04-10 02:59:38.483057 cybarpass-2.3/src/cybarpass/app.py
--rw-r--r--   0        0        0     1164 2023-04-04 18:21:15.006563 cybarpass-2.3/src/cybarpass/passgen.py
--rw-r--r--   0        0        0  2493977 2023-04-10 03:22:04.313188 cybarpass-2.3/src/cybarpass/words
--rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 cybarpass-2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-04 05:34:16.625403 cybarpass-2.4/LICENSE
+-rw-r--r--   0        0        0     2606 2023-04-11 03:14:21.721048 cybarpass-2.4/README.md
+-rw-r--r--   0        0        0      686 2023-04-11 03:15:19.664818 cybarpass-2.4/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-11 03:09:55.079403 cybarpass-2.4/src/cybarpass/__init__.py
+-rwxr-xr-x   0        0        0     1066 2023-04-11 03:09:17.947859 cybarpass-2.4/src/cybarpass/__main__.py
+-rw-r--r--   0        0        0      333 2023-04-04 18:28:31.775227 cybarpass-2.4/src/cybarpass/__runner.py
+-rw-r--r--   0        0        0     5426 2023-04-11 03:08:14.523960 cybarpass-2.4/src/cybarpass/app.py
+-rw-r--r--   0        0        0     1164 2023-04-11 03:08:17.828937 cybarpass-2.4/src/cybarpass/passgen.py
+-rw-r--r--   0        0        0  2493977 2023-04-10 03:22:04.313188 cybarpass-2.4/src/cybarpass/words
+-rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 cybarpass-2.4/PKG-INFO
```

### Comparing `cybarpass-2.3/LICENSE` & `cybarpass-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cybarpass-2.3/README.md` & `cybarpass-2.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # CybarPass
 
 ## Minimalistic Passphrase Generation script with GUI
 
-<img width="562" alt="image" src="https://user-images.githubusercontent.com/50134239/229692629-20cb301f-b577-4e9b-9299-b25516116861.png">
+<img width="562" alt="image" src="https://user-images.githubusercontent.com/50134239/231045484-9d4fa669-832f-45a6-8389-0b702a6fe86e.png">
 
 ### Dependencies
 
 -   Python \>= 3.9
 -   `tkinter` module
 
 **PS**: Also requires a word list file where each word is on a new line. You can supply your own, or, on MacOS and Linux, use `/usr/share/dict/words`.
@@ -15,19 +15,16 @@
 
 1.  Open terminal and run `python3 -m pip install cybarpass`
 2.  Set a shell alias: `alias cybarpass="python3 -m cybarpass"`
 3.  Run according to the instructions below
 
 ### Usage
 
-1.  GUI mode: run `cybarpass` in the terminal
-2.  GUI mode with word list preload: run
-    `cybarpass -g /path/to/word/list`
-3.  CLI mode: run `cybarpass /path/to/word/list` with optional parameter
-    `-n`
+1.  CLI mode: run `cybarpass` with optional parameter `-n`
+2.  GUI mode: run `cybarpass -g`
 
 #### Help Screen
 
 > output of `cybarpass -h`
 
 ```
 usage: cybarpass [-h] [-n NUM] [-g] [WORD_LIST]
@@ -38,18 +35,15 @@
   WORD_LIST          Path to dictionary file
 
 options:
   -h, --help         show this help message and exit
   -n NUM, --len NUM  Minimum length of passphrase
   -g, --gui          Run the program in GUI mode
 
-Launch without arguments for GUI mode
-or use -g | --gui with /path/to/word/list to preload the file
-
-PS: -n | --len has no effect in GUI mode
+NOTE: -n | --len has no effect in GUI mode
 ```
 
 #### Example Runs
 
 ```sh
 $ cybarpass -h
```

### Comparing `cybarpass-2.3/pyproject.toml` & `cybarpass-2.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "cybarpass"
-version = "2.3"
+version = "2.4"
 authors = [
     { name = "cybardev", email = "sheikh@cybar.dev" },
 ]
 description = "Minimalistic Passphrase Generation script with GUI"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cybarpass-2.3/src/cybarpass/__main__.py` & `cybarpass-2.4/src/cybarpass/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 import argparse
 from .__runner import run
 
 if __name__ == "__main__":
     # argument parsing
     parser = argparse.ArgumentParser(
         description="Generate a secure passphrase",
-        epilog="Launch without arguments for GUI mode\n"
-        + "or use -g | --gui with /path/to/word/list to preload the file\n"
-        + "\nPS: -n | --len has no effect in GUI mode",
+        epilog="NOTE: -n | --len has no effect in GUI mode",
         allow_abbrev=False,
         formatter_class=argparse.RawTextHelpFormatter,
     )
     parser.add_argument(
         "filename",
         help="Path to dictionary file",
         metavar="WORD_LIST",
```

### Comparing `cybarpass-2.3/src/cybarpass/app.py` & `cybarpass-2.4/src/cybarpass/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,15 +84,21 @@
         self.__lbl_password.grid(row=0, column=0)
 
     def entry_password(self) -> None:
         self.__entry_password = tk.Entry(
             self.__container,
             textvariable=self.__txt_password,
         )
-        self.__entry_password.grid(row=0, column=1, columnspan=2, sticky=tk.EW, padx=16)
+        self.__entry_password.grid(
+            row=0,
+            column=1,
+            columnspan=2,
+            sticky=tk.EW,
+            padx=16,
+        )
 
     # --- word list UI items --- #
 
     def lbl_word_list(self) -> None:
         self.__lbl_password = tk.Label(self.__container, text="Word List:")
         self.__lbl_password.grid(row=1, column=0)
 
@@ -119,15 +125,21 @@
         self.__lbl_password.grid(row=2, column=0)
 
     def combo_strength(self) -> None:
         self.__strength = Combobox(self.__container, width=18)
         self.__strength["values"] = tuple(CONST["pass-strength"].keys())
         self.__strength["state"] = "readonly"
         self.__strength.current(0)
-        self.__strength.grid(row=2, column=1, columnspan=2, sticky=tk.EW, padx=16)
+        self.__strength.grid(
+            row=2,
+            column=1,
+            columnspan=2,
+            sticky=tk.EW,
+            padx=16,
+        )
 
     # --- action button group --- #
 
     def btn_generate(self) -> None:
         self.__btn_generate = tk.Button(
             self.__container,
             text="Generate",
```

### Comparing `cybarpass-2.3/src/cybarpass/passgen.py` & `cybarpass-2.4/src/cybarpass/passgen.py`

 * *Files identical despite different names*

### Comparing `cybarpass-2.3/src/cybarpass/words` & `cybarpass-2.4/src/cybarpass/words`

 * *Files identical despite different names*

### Comparing `cybarpass-2.3/PKG-INFO` & `cybarpass-2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybarpass
-Version: 2.3
+Version: 2.4
 Summary: Minimalistic Passphrase Generation script with GUI
 Home-page: https://pass.cybar.dev
 Author-Email: cybardev <sheikh@cybar.dev>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://pass.cybar.dev
@@ -13,15 +13,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # CybarPass
 
 ## Minimalistic Passphrase Generation script with GUI
 
-<img width="562" alt="image" src="https://user-images.githubusercontent.com/50134239/229692629-20cb301f-b577-4e9b-9299-b25516116861.png">
+<img width="562" alt="image" src="https://user-images.githubusercontent.com/50134239/231045484-9d4fa669-832f-45a6-8389-0b702a6fe86e.png">
 
 ### Dependencies
 
 -   Python \>= 3.9
 -   `tkinter` module
 
 **PS**: Also requires a word list file where each word is on a new line. You can supply your own, or, on MacOS and Linux, use `/usr/share/dict/words`.
@@ -30,19 +30,16 @@
 
 1.  Open terminal and run `python3 -m pip install cybarpass`
 2.  Set a shell alias: `alias cybarpass="python3 -m cybarpass"`
 3.  Run according to the instructions below
 
 ### Usage
 
-1.  GUI mode: run `cybarpass` in the terminal
-2.  GUI mode with word list preload: run
-    `cybarpass -g /path/to/word/list`
-3.  CLI mode: run `cybarpass /path/to/word/list` with optional parameter
-    `-n`
+1.  CLI mode: run `cybarpass` with optional parameter `-n`
+2.  GUI mode: run `cybarpass -g`
 
 #### Help Screen
 
 > output of `cybarpass -h`
 
 ```
 usage: cybarpass [-h] [-n NUM] [-g] [WORD_LIST]
@@ -53,18 +50,15 @@
   WORD_LIST          Path to dictionary file
 
 options:
   -h, --help         show this help message and exit
   -n NUM, --len NUM  Minimum length of passphrase
   -g, --gui          Run the program in GUI mode
 
-Launch without arguments for GUI mode
-or use -g | --gui with /path/to/word/list to preload the file
-
-PS: -n | --len has no effect in GUI mode
+NOTE: -n | --len has no effect in GUI mode
 ```
 
 #### Example Runs
 
 ```sh
 $ cybarpass -h
```

