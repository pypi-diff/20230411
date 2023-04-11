# Comparing `tmp/llm4gpt-2023.4.11.14.33.49.tar.gz` & `tmp/llm4gpt-2023.4.11.14.35.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.11.14.33.49.tar", last modified: Tue Apr 11 06:33:49 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.11.14.35.6.tar", last modified: Tue Apr 11 06:35:06 2023, max compression
```

## Comparing `llm4gpt-2023.4.11.14.33.49.tar` & `llm4gpt-2023.4.11.14.35.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:33:49.653018 llm4gpt-2023.4.11.14.33.49/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.11.14.33.49/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-11 06:33:49.653115 llm4gpt-2023.4.11.14.33.49/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.11.14.33.49/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:33:49.650853 llm4gpt-2023.4.11.14.33.49/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.11.14.33.49/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:33:49.651180 llm4gpt-2023.4.11.14.33.49/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:33:49.651672 llm4gpt-2023.4.11.14.33.49/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/llm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/llm/llm4gpt.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:33:49.652606 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1370 2023-04-11 06:33:49.000000 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-04-11 06:33:49.000000 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 06:33:49.000000 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-11 06:33:49.000000 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 06:33:49.000000 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-11 06:33:49.000000 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 06:33:49.000000 llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-11 06:33:49.653394 llm4gpt-2023.4.11.14.33.49/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1519 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:33:49.652866 llm4gpt-2023.4.11.14.33.49/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.33.49/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:35:06.478313 llm4gpt-2023.4.11.14.35.6/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.11.14.35.6/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1369 2023-04-11 06:35:06.478408 llm4gpt-2023.4.11.14.35.6/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      553 2023-04-11 06:33:00.000000 llm4gpt-2023.4.11.14.35.6/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:35:06.476381 llm4gpt-2023.4.11.14.35.6/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-11 04:38:41.000000 llm4gpt-2023.4.11.14.35.6/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:35:06.476618 llm4gpt-2023.4.11.14.35.6/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:35:06.477051 llm4gpt-2023.4.11.14.35.6/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/llm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/llm/llm4gpt.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:35:06.477904 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1369 2023-04-11 06:35:06.000000 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-04-11 06:35:06.000000 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 06:35:06.000000 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-11 06:35:06.000000 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 06:35:06.000000 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-11 06:35:06.000000 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-11 06:35:06.000000 llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-11 06:35:06.478698 llm4gpt-2023.4.11.14.35.6/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1511 2023-04-11 06:35:05.000000 llm4gpt-2023.4.11.14.35.6/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 06:35:06.478189 llm4gpt-2023.4.11.14.35.6/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.14.35.6/tox.ini
```

### Comparing `llm4gpt-2023.4.11.14.33.49/.gitignore` & `llm4gpt-2023.4.11.14.35.6/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/.travis.yml` & `llm4gpt-2023.4.11.14.35.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/CONTRIBUTING.rst` & `llm4gpt-2023.4.11.14.35.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/LICENSE` & `llm4gpt-2023.4.11.14.35.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/Makefile` & `llm4gpt-2023.4.11.14.35.6/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/PKG-INFO` & `llm4gpt-2023.4.11.14.35.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.11.14.33.49
+Version: 2023.4.11.14.35.6
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.11.14.33.49/README.md` & `llm4gpt-2023.4.11.14.35.6/README.md`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/README.rst` & `llm4gpt-2023.4.11.14.35.6/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/docs/Makefile` & `llm4gpt-2023.4.11.14.35.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/docs/conf.py` & `llm4gpt-2023.4.11.14.35.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/docs/installation.rst` & `llm4gpt-2023.4.11.14.35.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/docs/make.bat` & `llm4gpt-2023.4.11.14.35.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/llm/clis/cli.py` & `llm4gpt-2023.4.11.14.35.6/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.11.14.33.49
+Version: 2023.4.11.14.35.6
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.11.14.33.49/llm4gpt.egg-info/SOURCES.txt` & `llm4gpt-2023.4.11.14.35.6/llm4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.14.33.49/setup.py` & `llm4gpt-2023.4.11.14.35.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords='llm4gpt',
     name='llm4gpt',
-    packages=find_packages(include=['llm4gpt', 'llm4gpt.*']),
+    packages=find_packages(include=['llm', 'llm.*']),
 
     test_suite='tests',
     url='https://github.com/yuanjie-ai/llm4gpt',
     version=version, # '0.0.0',
     zip_safe=False,
 )
```

### Comparing `llm4gpt-2023.4.11.14.33.49/tests/test_llm4gpt.py` & `llm4gpt-2023.4.11.14.35.6/tests/test_llm4gpt.py`

 * *Files identical despite different names*

