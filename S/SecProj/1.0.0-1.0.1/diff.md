# Comparing `tmp/SecProj-1.0.0.tar.gz` & `tmp/SecProj-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecProj-1.0.0.tar", last modified: Tue Apr  4 03:16:05 2023, max compression
+gzip compressed data, was "SecProj-1.0.1.tar", last modified: Tue Apr 11 16:45:50 2023, max compression
```

## Comparing `SecProj-1.0.0.tar` & `SecProj-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-04 03:16:05.958527 SecProj-1.0.0/
--rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-04-02 19:56:40.000000 SecProj-1.0.0/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)     3177 2023-04-04 03:16:05.958527 SecProj-1.0.0/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)     2831 2023-04-04 03:02:39.000000 SecProj-1.0.0/README.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-04 03:16:05.958527 SecProj-1.0.0/SecProj.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)     3177 2023-04-04 03:16:05.000000 SecProj-1.0.0/SecProj.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      216 2023-04-04 03:16:05.000000 SecProj-1.0.0/SecProj.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-04 03:16:05.000000 SecProj-1.0.0/SecProj.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       27 2023-04-04 03:16:05.000000 SecProj-1.0.0/SecProj.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        8 2023-04-04 03:16:05.000000 SecProj-1.0.0/SecProj.egg-info/top_level.txt
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-04 03:16:05.958527 SecProj-1.0.0/secproj/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-04-02 19:57:42.000000 SecProj-1.0.0/secproj/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3386 2023-04-04 02:32:09.000000 SecProj-1.0.0/secproj/core.py
--rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-04 03:16:05.958527 SecProj-1.0.0/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)      676 2023-04-04 03:15:21.000000 SecProj-1.0.0/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-11 16:45:50.094201 SecProj-1.0.1/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1069 2023-04-02 19:56:40.000000 SecProj-1.0.1/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)     3189 2023-04-11 16:45:50.094201 SecProj-1.0.1/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     2843 2023-04-11 16:29:47.000000 SecProj-1.0.1/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-11 16:45:50.094201 SecProj-1.0.1/SecProj.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     3189 2023-04-11 16:45:50.000000 SecProj-1.0.1/SecProj.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      216 2023-04-11 16:45:50.000000 SecProj-1.0.1/SecProj.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2023-04-11 16:45:50.000000 SecProj-1.0.1/SecProj.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       36 2023-04-11 16:45:50.000000 SecProj-1.0.1/SecProj.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        8 2023-04-11 16:45:50.000000 SecProj-1.0.1/SecProj.egg-info/top_level.txt
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2023-04-11 16:45:50.094201 SecProj-1.0.1/secproj/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2023-04-02 19:57:42.000000 SecProj-1.0.1/secproj/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3454 2023-04-11 16:44:27.000000 SecProj-1.0.1/secproj/core.py
+-rw-r--r--   0 felix     (1000) felix     (1000)       38 2023-04-11 16:45:50.094201 SecProj-1.0.1/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)      687 2023-04-11 16:45:11.000000 SecProj-1.0.1/setup.py
```

### Comparing `SecProj-1.0.0/LICENSE` & `SecProj-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SecProj-1.0.0/PKG-INFO` & `SecProj-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecProj
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple tools to help you secure your projects in a more simple manner, allowing for simple and secure development.
 Home-page: https://github.com/basegodfelix/secproj
 Author: Felix Hernandez
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 with the additional encryption of the information being stored on the hard drive creates two layers of security when coding.
 
 Of course all of this is for nothing if your systems are breached and these files get copied because then the values can be decrypted.
 It is up to each person using these tools to secure the key and env files accordingly.
 
 The gitignore overwrite is disabled by default because it can create a nuisance for developers but it can easily be enabled.
 # Dependencies
-This code is very simple and only has two dependencies, cryptography and python-dotenv.
+This code is very simple and only has three dependencies: cryptography, python-dotenv and requests.
 # Installation
 ```
 pip install secproj
 ```
 # Usage
 ## Create Encrypted Variables
 NOTE: _You can signal which part of a string you want encrypted by wrapping it in $$$, or you can just encrypt the whole string by not wrapping it._
```

### Comparing `SecProj-1.0.0/README.md` & `SecProj-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with the additional encryption of the information being stored on the hard drive creates two layers of security when coding.
 
 Of course all of this is for nothing if your systems are breached and these files get copied because then the values can be decrypted.
 It is up to each person using these tools to secure the key and env files accordingly.
 
 The gitignore overwrite is disabled by default because it can create a nuisance for developers but it can easily be enabled.
 # Dependencies
-This code is very simple and only has two dependencies, cryptography and python-dotenv.
+This code is very simple and only has three dependencies: cryptography, python-dotenv and requests.
 # Installation
 ```
 pip install secproj
 ```
 # Usage
 ## Create Encrypted Variables
 NOTE: _You can signal which part of a string you want encrypted by wrapping it in $$$, or you can just encrypt the whole string by not wrapping it._
```

### Comparing `SecProj-1.0.0/SecProj.egg-info/PKG-INFO` & `SecProj-1.0.1/SecProj.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecProj
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple tools to help you secure your projects in a more simple manner, allowing for simple and secure development.
 Home-page: https://github.com/basegodfelix/secproj
 Author: Felix Hernandez
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 with the additional encryption of the information being stored on the hard drive creates two layers of security when coding.
 
 Of course all of this is for nothing if your systems are breached and these files get copied because then the values can be decrypted.
 It is up to each person using these tools to secure the key and env files accordingly.
 
 The gitignore overwrite is disabled by default because it can create a nuisance for developers but it can easily be enabled.
 # Dependencies
-This code is very simple and only has two dependencies, cryptography and python-dotenv.
+This code is very simple and only has three dependencies: cryptography, python-dotenv and requests.
 # Installation
 ```
 pip install secproj
 ```
 # Usage
 ## Create Encrypted Variables
 NOTE: _You can signal which part of a string you want encrypted by wrapping it in $$$, or you can just encrypt the whole string by not wrapping it._
```

### Comparing `SecProj-1.0.0/secproj/core.py` & `SecProj-1.0.1/secproj/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import sys
 import dotenv
+import requests
 from cryptography.fernet import Fernet
 
 class Secure(object):
     def __init__(self,gitignore_overwrite=False):
         self.active_path = sys.path[0]
         self.data_path = self.active_path + '/data/'
         self.key_file = self.data_path + 'enc.key'
         self.dotenv_file = self.data_path + ".env"
         self.gitignore_file = self.active_path + "/.gitignore"
-        self.base_ignore_file = os.path.dirname(os.path.abspath(__file__)) + "/ignore.txt"
+        self.base_ignore_file = "https://raw.githubusercontent.com/basegodfelix/secproj/main/secproj/ignore.txt"
 
         if not os.path.exists(self.data_path):
             os.makedirs(self.data_path)
 
         if not os.path.isfile(self.dotenv_file):
             with open(self.dotenv_file, "x") as mk:
                 mk.close()
@@ -46,16 +47,17 @@
             with open(self.key_file, 'wb') as f:
                 f.write(self.key)
             self.enc = Fernet(self.key)
 
     def overwrite_gitignore(self):
         try:
             contents = ""
-            with open(self.base_ignore_file, "r") as reader:
-                contents = reader.read()
+            resp = requests.get(self.base_ignore_file)
+            if resp.status_code == 200:
+                contents = resp.text
             if contents != "":
                 with open(self.gitignore_file, "w") as writer:
                     writer.write(contents)
             return True
         except:
             return False
```

### Comparing `SecProj-1.0.0/setup.py` & `SecProj-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     path = os.path.dirname(os.path.abspath(__file__))
     with open(os.path.join(path, 'README.md'), encoding='utf-8') as f:
         tmp = f.read()
     return tmp
 
 setuptools.setup(
     name="SecProj",
-    version="1.0.0",
+    version="1.0.1",
     author="Felix Hernandez",
     description="Simple tools to help you secure your projects in a more simple manner, allowing for simple and secure development.",
     packages=["secproj"],
-    install_requires=["cryptography","python-dotenv"],
+    install_requires=["cryptography","python-dotenv","requests"],
     url="https://github.com/basegodfelix/secproj",
     long_description = read(),
     long_description_content_type = 'text/markdown',
     license="MIT"
 )
```

