# Comparing `tmp/cybarpass-2.4.tar.gz` & `tmp/cybarpass-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybarpass-2.4.tar", last modified: Tue Apr 11 03:15:19 2023, max compression
+gzip compressed data, was "cybarpass-2.5.tar", last modified: Tue Apr 11 03:38:47 2023, max compression
```

## Comparing `cybarpass-2.4.tar` & `cybarpass-2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-04 05:34:16.625403 cybarpass-2.4/LICENSE
--rw-r--r--   0        0        0     2606 2023-04-11 03:14:21.721048 cybarpass-2.4/README.md
--rw-r--r--   0        0        0      686 2023-04-11 03:15:19.664818 cybarpass-2.4/pyproject.toml
--rw-r--r--   0        0        0       91 2023-04-11 03:09:55.079403 cybarpass-2.4/src/cybarpass/__init__.py
--rwxr-xr-x   0        0        0     1066 2023-04-11 03:09:17.947859 cybarpass-2.4/src/cybarpass/__main__.py
--rw-r--r--   0        0        0      333 2023-04-04 18:28:31.775227 cybarpass-2.4/src/cybarpass/__runner.py
--rw-r--r--   0        0        0     5426 2023-04-11 03:08:14.523960 cybarpass-2.4/src/cybarpass/app.py
--rw-r--r--   0        0        0     1164 2023-04-11 03:08:17.828937 cybarpass-2.4/src/cybarpass/passgen.py
--rw-r--r--   0        0        0  2493977 2023-04-10 03:22:04.313188 cybarpass-2.4/src/cybarpass/words
--rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 cybarpass-2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-04 05:34:16.625403 cybarpass-2.5/LICENSE
+-rw-r--r--   0        0        0     2606 2023-04-11 03:14:21.721048 cybarpass-2.5/README.md
+-rw-r--r--   0        0        0      686 2023-04-11 03:38:47.930893 cybarpass-2.5/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-11 03:37:34.295089 cybarpass-2.5/src/cybarpass/__init__.py
+-rwxr-xr-x   0        0        0     1066 2023-04-11 03:37:27.968256 cybarpass-2.5/src/cybarpass/__main__.py
+-rw-r--r--   0        0        0      333 2023-04-11 03:37:31.027113 cybarpass-2.5/src/cybarpass/__runner.py
+-rw-r--r--   0        0        0     5426 2023-04-11 03:37:37.711909 cybarpass-2.5/src/cybarpass/app.py
+-rw-r--r--   0        0        0     1683 2023-04-11 03:37:40.330170 cybarpass-2.5/src/cybarpass/passgen.py
+-rw-r--r--   0        0        0  2493977 2023-04-10 03:22:04.313188 cybarpass-2.5/src/cybarpass/words
+-rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 cybarpass-2.5/PKG-INFO
```

### Comparing `cybarpass-2.4/LICENSE` & `cybarpass-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cybarpass-2.4/README.md` & `cybarpass-2.5/README.md`

 * *Files identical despite different names*

### Comparing `cybarpass-2.4/pyproject.toml` & `cybarpass-2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "cybarpass"
-version = "2.4"
+version = "2.5"
 authors = [
     { name = "cybardev", email = "sheikh@cybar.dev" },
 ]
 description = "Minimalistic Passphrase Generation script with GUI"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cybarpass-2.4/src/cybarpass/__main__.py` & `cybarpass-2.5/src/cybarpass/__main__.py`

 * *Files identical despite different names*

### Comparing `cybarpass-2.4/src/cybarpass/app.py` & `cybarpass-2.5/src/cybarpass/app.py`

 * *Files identical despite different names*

### Comparing `cybarpass-2.4/src/cybarpass/words` & `cybarpass-2.5/src/cybarpass/words`

 * *Files identical despite different names*

### Comparing `cybarpass-2.4/PKG-INFO` & `cybarpass-2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybarpass
-Version: 2.4
+Version: 2.5
 Summary: Minimalistic Passphrase Generation script with GUI
 Home-page: https://pass.cybar.dev
 Author-Email: cybardev <sheikh@cybar.dev>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://pass.cybar.dev
```

