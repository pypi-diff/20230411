# Comparing `tmp/RsaIt-0.0.2.tar.gz` & `tmp/RsaIt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RsaIt-0.0.2.tar", last modified: Mon Apr 10 08:12:34 2023, max compression
+gzip compressed data, was "RsaIt-0.0.3.tar", last modified: Tue Apr 11 04:52:57 2023, max compression
```

## Comparing `RsaIt-0.0.2.tar` & `RsaIt-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xiaobo     (501) staff       (20)        0 2023-04-10 08:12:34.425692 RsaIt-0.0.2/
--rw-r--r--   0 xiaobo     (501) staff       (20)      817 2023-04-10 08:12:34.425543 RsaIt-0.0.2/PKG-INFO
--rw-r--r--   0 xiaobo     (501) staff       (20)       31 2023-04-10 06:59:49.000000 RsaIt-0.0.2/README.md
-drwxr-xr-x   0 xiaobo     (501) staff       (20)        0 2023-04-10 08:12:34.425029 RsaIt-0.0.2/RsaIt.egg-info/
--rw-r--r--   0 xiaobo     (501) staff       (20)      817 2023-04-10 08:12:34.000000 RsaIt-0.0.2/RsaIt.egg-info/PKG-INFO
--rw-r--r--   0 xiaobo     (501) staff       (20)      207 2023-04-10 08:12:34.000000 RsaIt-0.0.2/RsaIt.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobo     (501) staff       (20)        1 2023-04-10 08:12:34.000000 RsaIt-0.0.2/RsaIt.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobo     (501) staff       (20)       19 2023-04-10 08:12:34.000000 RsaIt-0.0.2/RsaIt.egg-info/requires.txt
--rw-r--r--   0 xiaobo     (501) staff       (20)       12 2023-04-10 08:12:34.000000 RsaIt-0.0.2/RsaIt.egg-info/top_level.txt
-drwxr-xr-x   0 xiaobo     (501) staff       (20)        0 2023-04-10 08:12:34.425362 RsaIt-0.0.2/rsa_confirm/
--rw-r--r--   0 xiaobo     (501) staff       (20)       21 2023-04-10 08:08:50.000000 RsaIt-0.0.2/rsa_confirm/__init__.py
--rw-r--r--   0 xiaobo     (501) staff       (20)      194 2023-04-10 07:49:10.000000 RsaIt-0.0.2/rsa_confirm/_core.py
--rw-r--r--   0 xiaobo     (501) staff       (20)       38 2023-04-10 08:12:34.425736 RsaIt-0.0.2/setup.cfg
--rw-r--r--   0 xiaobo     (501) staff       (20)     1755 2023-04-10 08:12:31.000000 RsaIt-0.0.2/setup.py
+drwxr-xr-x   0 xiaobo     (501) staff       (20)        0 2023-04-11 04:52:57.471451 RsaIt-0.0.3/
+-rw-r--r--   0 xiaobo     (501) staff       (20)      817 2023-04-11 04:52:57.471324 RsaIt-0.0.3/PKG-INFO
+-rw-r--r--   0 xiaobo     (501) staff       (20)       31 2023-04-10 06:59:49.000000 RsaIt-0.0.3/README.md
+drwxr-xr-x   0 xiaobo     (501) staff       (20)        0 2023-04-11 04:52:57.470534 RsaIt-0.0.3/RsaIt.egg-info/
+-rw-r--r--   0 xiaobo     (501) staff       (20)      817 2023-04-11 04:52:57.000000 RsaIt-0.0.3/RsaIt.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobo     (501) staff       (20)      207 2023-04-11 04:52:57.000000 RsaIt-0.0.3/RsaIt.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobo     (501) staff       (20)        1 2023-04-11 04:52:57.000000 RsaIt-0.0.3/RsaIt.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobo     (501) staff       (20)       19 2023-04-11 04:52:57.000000 RsaIt-0.0.3/RsaIt.egg-info/requires.txt
+-rw-r--r--   0 xiaobo     (501) staff       (20)       12 2023-04-11 04:52:57.000000 RsaIt-0.0.3/RsaIt.egg-info/top_level.txt
+drwxr-xr-x   0 xiaobo     (501) staff       (20)        0 2023-04-11 04:52:57.470980 RsaIt-0.0.3/rsa_confirm/
+-rw-r--r--   0 xiaobo     (501) staff       (20)       21 2023-04-10 08:16:49.000000 RsaIt-0.0.3/rsa_confirm/__init__.py
+-rw-r--r--   0 xiaobo     (501) staff       (20)     3830 2023-04-11 04:51:04.000000 RsaIt-0.0.3/rsa_confirm/_core.py
+-rw-r--r--   0 xiaobo     (501) staff       (20)       38 2023-04-11 04:52:57.471574 RsaIt-0.0.3/setup.cfg
+-rw-r--r--   0 xiaobo     (501) staff       (20)     1755 2023-04-11 04:52:55.000000 RsaIt-0.0.3/setup.py
```

### Comparing `RsaIt-0.0.2/PKG-INFO` & `RsaIt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsaIt
-Version: 0.0.2
+Version: 0.0.3
 Summary: upload pypi test-RsaConfirm
 Home-page: https://github.com/LottoDog/rsa_confirm.git
 Author: xiaobo666
 Author-email: knightforiu@163.com
 License: Apache 2.0
 Keywords: RsaConfirm
 Platform: UNKNOWN
```

### Comparing `RsaIt-0.0.2/RsaIt.egg-info/PKG-INFO` & `RsaIt-0.0.3/RsaIt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsaIt
-Version: 0.0.2
+Version: 0.0.3
 Summary: upload pypi test-RsaConfirm
 Home-page: https://github.com/LottoDog/rsa_confirm.git
 Author: xiaobo666
 Author-email: knightforiu@163.com
 License: Apache 2.0
 Keywords: RsaConfirm
 Platform: UNKNOWN
```

### Comparing `RsaIt-0.0.2/setup.py` & `RsaIt-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="RsaIt",
-    version="0.0.2",
+    version="0.0.3",
     author="xiaobo666",
     author_email="knightforiu@163.com",
     description="upload pypi test-RsaConfirm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LottoDog/rsa_confirm.git",
     packages=setuptools.find_packages(),
```

