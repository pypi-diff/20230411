# Comparing `tmp/passbolt-1.23.tar.gz` & `tmp/passbolt-1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/passbolt-1.23.tar", last modified: Tue Nov 16 20:48:40 2021, max compression
+gzip compressed data, was "passbolt-1.24.tar", last modified: Tue Apr 11 21:29:38 2023, max compression
```

## Comparing `passbolt-1.23.tar` & `passbolt-1.24.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 dlynch     (501) staff       (20)        0 2021-11-16 20:48:40.792612 passbolt-1.23/
--rw-r--r--   0 dlynch     (501) staff       (20)     9317 2021-11-16 20:48:40.792350 passbolt-1.23/PKG-INFO
-drwxr-xr-x   0 dlynch     (501) staff       (20)        0 2021-11-16 20:48:40.790345 passbolt-1.23/passbolt/
--rw-r--r--   0 dlynch     (501) staff       (20)        0 2021-11-16 18:45:46.000000 passbolt-1.23/passbolt/__init__.py
--rw-r--r--   0 dlynch     (501) staff       (20)    23056 2021-11-16 20:36:13.000000 passbolt-1.23/passbolt/passbolt.py
-drwxr-xr-x   0 dlynch     (501) staff       (20)        0 2021-11-16 20:48:40.791892 passbolt-1.23/passbolt.egg-info/
--rw-r--r--   0 dlynch     (501) staff       (20)     9317 2021-11-16 20:48:40.000000 passbolt-1.23/passbolt.egg-info/PKG-INFO
--rw-r--r--   0 dlynch     (501) staff       (20)      224 2021-11-16 20:48:40.000000 passbolt-1.23/passbolt.egg-info/SOURCES.txt
--rw-r--r--   0 dlynch     (501) staff       (20)        1 2021-11-16 20:48:40.000000 passbolt-1.23/passbolt.egg-info/dependency_links.txt
--rw-r--r--   0 dlynch     (501) staff       (20)       31 2021-11-16 20:48:40.000000 passbolt-1.23/passbolt.egg-info/requires.txt
--rw-r--r--   0 dlynch     (501) staff       (20)        9 2021-11-16 20:48:40.000000 passbolt-1.23/passbolt.egg-info/top_level.txt
--rw-r--r--   0 dlynch     (501) staff       (20)      103 2021-11-16 18:45:46.000000 passbolt-1.23/pyproject.toml
--rw-r--r--   0 dlynch     (501) staff       (20)       38 2021-11-16 20:48:40.792689 passbolt-1.23/setup.cfg
--rw-r--r--   0 dlynch     (501) staff       (20)      759 2021-11-16 20:48:18.000000 passbolt-1.23/setup.py
+drwxrwxrwx   0 dlynch    (1000) dlynch    (1000)        0 2023-04-11 17:29:39.528187 passbolt-1.24/
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)     1073 2023-04-11 17:13:29.000000 passbolt-1.24/LICENSE
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)    10192 2023-04-11 17:29:39.526187 passbolt-1.24/PKG-INFO
+drwxrwxrwx   0 dlynch    (1000) dlynch    (1000)        0 2023-04-11 17:29:39.467188 passbolt-1.24/passbolt/
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)        0 2023-04-11 17:13:29.000000 passbolt-1.24/passbolt/__init__.py
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)    23290 2023-04-11 17:13:29.000000 passbolt-1.24/passbolt/passbolt.py
+drwxrwxrwx   0 dlynch    (1000) dlynch    (1000)        0 2023-04-11 17:29:39.516189 passbolt-1.24/passbolt.egg-info/
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)    10192 2023-04-11 17:29:39.000000 passbolt-1.24/passbolt.egg-info/PKG-INFO
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)      232 2023-04-11 17:29:39.000000 passbolt-1.24/passbolt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)        1 2023-04-11 17:29:39.000000 passbolt-1.24/passbolt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)       31 2023-04-11 17:29:39.000000 passbolt-1.24/passbolt.egg-info/requires.txt
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)        9 2023-04-11 17:29:39.000000 passbolt-1.24/passbolt.egg-info/top_level.txt
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)      103 2023-04-11 17:13:29.000000 passbolt-1.24/pyproject.toml
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)       38 2023-04-11 17:29:39.529189 passbolt-1.24/setup.cfg
+-rwxrwxrwx   0 dlynch    (1000) dlynch    (1000)      759 2023-04-11 17:21:26.000000 passbolt-1.24/setup.py
```

### Comparing `passbolt-1.23/PKG-INFO` & `passbolt-1.24/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passbolt
-Version: 1.23
+Version: 1.24
 Summary: Passbolt python module
 Home-page: https://github.com/daniel-lynch/passbolt
 Author: Daniel Lynch
 Author-email: daniel.lynch2016@gmail.com
 License: MIT
 Description: # Readme
         
@@ -33,15 +33,36 @@
               ```
               from passbolt.passbolt import passbolt
         
               key = open("passbolt_private.asc", "r").read()
               passphrase = open("passphrase", "r").read().replace('\n', '')
               Passbolt = passbolt(key, passphrase, "https://passbolt.example.com")
               ```
+              
         
+        
+              or you will need the fingerprint of your private key store in gpg-agent and  the URI to your passbolt instance.
+              Then just call the passbolt class with those variables.
+        
+              ```
+              from passbolt.passbolt import passbolt
+        
+              Passbolt = passbolt(apiurl= "https://passbolt.example.com",fingerprint="BD51086546F2B05FE3207570848AD92005EABC")
+              ```
+              
+              
+              
+              and if you use a custom ca, you can specify a custom TLS CA certificate bundle :
+            
+              ```
+              from passbolt.passbolt import passbolt
+         
+              Passbolt = passbolt(apiurl= "https://passbolt.example.com",fingerprint="BD51086546F2B05FE3207570848AD92005EABC", verify="/etc/ipa/ca.crt")
+              ``` 
+              
           - Create a password:
         
               To create a password you will need the following:
         
                 - Resource name
                 - Password
                 - Username (optional)
```

### Comparing `passbolt-1.23/passbolt/passbolt.py` & `passbolt-1.24/passbolt/passbolt.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 import fnmatch
 import json
 from urllib.parse import unquote
 
 
 class passbolt:
 
-    def __init__(self, privatekey, passphrase, apiurl):
-        self.privatekey = privatekey
-        self.passphrase = passphrase
+    def __init__(self,privatekey=None, passphrase=None, apiurl=None, fingerprint=None, verify=True):
+        if fingerprint:
+            self.keyfingerprint = fingerprint
+            self.gpg = gnupg.GPG(use_agent=True)
+            self.passphrase = None
+        else:
+            self.privatekey = privatekey
+            self.passphrase = passphrase
+            self.gpg = gnupg.GPG()
+            # Importing our private key
+            self.imported_keys = self.gpg.import_keys(privatekey)
+            # Getting the fingerprint of our first privatekey
+            self.keyfingerprint = self.imported_keys.fingerprints[0]
+
         self.apiurl = apiurl
-        self.gpg = gnupg.GPG()
         self.session = requests.session()
-        self.session.verify = True
+        self.session.verify = verify
         self.apiversion = "?api-version=v3"
         self.loginurl = f"/auth/login.json{self.apiversion}"
 
-        # Importing our private key
-        self.imported_keys = self.gpg.import_keys(privatekey)
-
-        # Getting the fingerprint of our first privatekey
-        self.keyfingerprint = self.imported_keys.fingerprints[0]
-        
         # Giving our key Ultimate trust so that we can encrypt secrets with it.
         self.gpg.trust_keys(self.keyfingerprint, "TRUST_ULTIMATE")
 
         self.__login()
 
     def __login(self):
```

### Comparing `passbolt-1.23/passbolt.egg-info/PKG-INFO` & `passbolt-1.24/passbolt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passbolt
-Version: 1.23
+Version: 1.24
 Summary: Passbolt python module
 Home-page: https://github.com/daniel-lynch/passbolt
 Author: Daniel Lynch
 Author-email: daniel.lynch2016@gmail.com
 License: MIT
 Description: # Readme
         
@@ -33,15 +33,36 @@
               ```
               from passbolt.passbolt import passbolt
         
               key = open("passbolt_private.asc", "r").read()
               passphrase = open("passphrase", "r").read().replace('\n', '')
               Passbolt = passbolt(key, passphrase, "https://passbolt.example.com")
               ```
+              
         
+        
+              or you will need the fingerprint of your private key store in gpg-agent and  the URI to your passbolt instance.
+              Then just call the passbolt class with those variables.
+        
+              ```
+              from passbolt.passbolt import passbolt
+        
+              Passbolt = passbolt(apiurl= "https://passbolt.example.com",fingerprint="BD51086546F2B05FE3207570848AD92005EABC")
+              ```
+              
+              
+              
+              and if you use a custom ca, you can specify a custom TLS CA certificate bundle :
+            
+              ```
+              from passbolt.passbolt import passbolt
+         
+              Passbolt = passbolt(apiurl= "https://passbolt.example.com",fingerprint="BD51086546F2B05FE3207570848AD92005EABC", verify="/etc/ipa/ca.crt")
+              ``` 
+              
           - Create a password:
         
               To create a password you will need the following:
         
                 - Resource name
                 - Password
                 - Username (optional)
```

### Comparing `passbolt-1.23/setup.py` & `passbolt-1.24/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 import os
 
 def get_long_description():
     with open(os.path.join(
-        os.path.dirname(os.path.abspath(__file__)), 'README.md'
+        os.path.dirname(os.path.abspath(__file__)), 'readme.md'
     ), encoding='utf8') as fp:
         return fp.read()
 
 setup(
         name='passbolt',
-        version='1.23',
+        version='1.24',
         description='Passbolt python module',
         long_description=get_long_description(),
         long_description_content_type='text/markdown',
         author='Daniel Lynch',
         author_email='daniel.lynch2016@gmail.com',
         url='https://github.com/daniel-lynch/passbolt',
         license='MIT',
```

