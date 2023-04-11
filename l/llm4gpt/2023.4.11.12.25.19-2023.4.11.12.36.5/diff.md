# Comparing `tmp/llm4gpt-2023.4.11.12.25.19.tar.gz` & `tmp/llm4gpt-2023.4.11.12.36.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4gpt-2023.4.11.12.25.19.tar", last modified: Tue Apr 11 04:25:19 2023, max compression
+gzip compressed data, was "llm4gpt-2023.4.11.12.36.5.tar", last modified: Tue Apr 11 04:36:05 2023, max compression
```

## Comparing `llm4gpt-2023.4.11.12.25.19.tar` & `llm4gpt-2023.4.11.12.36.5.tar`

### file list

```diff
@@ -1,33 +1,53 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:25:19.901341 llm4gpt-2023.4.11.12.25.19/
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-11 04:25:19.901492 llm4gpt-2023.4.11.12.25.19/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:25:19.900090 llm4gpt-2023.4.11.12.25.19/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:25:19.900950 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-11 04:25:19.000000 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      523 2023-04-11 04:25:19.000000 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 04:25:19.000000 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-11 04:25:19.000000 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 04:25:19.000000 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-11 04:25:19.000000 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 04:25:19.000000 llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-11 04:25:19.901834 llm4gpt-2023.4.11.12.25.19/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1519 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:25:19.901208 llm4gpt-2023.4.11.12.25.19/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.25.19/tests/test_llm4gpt.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:36:05.566176 llm4gpt-2023.4.11.12.36.5/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:36:05.562546 llm4gpt-2023.4.11.12.36.5/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      318 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1206 2023-04-11 04:36:04.000000 llm4gpt-2023.4.11.12.36.5/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1195 2023-04-11 04:36:05.566269 llm4gpt-2023.4.11.12.36.5/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:36:05.564005 llm4gpt-2023.4.11.12.36.5/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      379 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      224 2023-04-11 04:32:30.000000 llm4gpt-2023.4.11.12.36.5/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:36:05.564235 llm4gpt-2023.4.11.12.36.5/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:36:05.564609 llm4gpt-2023.4.11.12.36.5/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/llm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/llm/llm4gpt.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:36:05.565805 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1195 2023-04-11 04:36:05.000000 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      780 2023-04-11 04:36:05.000000 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 04:36:05.000000 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-11 04:36:05.000000 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 04:36:05.000000 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-11 04:36:05.000000 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-11 04:36:05.000000 llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-11 04:36:05.566550 llm4gpt-2023.4.11.12.36.5/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1519 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-11 04:36:05.566063 llm4gpt-2023.4.11.12.36.5/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4gpt-2023.4.11.12.36.5/tox.ini
```

### Comparing `llm4gpt-2023.4.11.12.25.19/CONTRIBUTING.rst` & `llm4gpt-2023.4.11.12.36.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/LICENSE` & `llm4gpt-2023.4.11.12.36.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/PKG-INFO` & `llm4gpt-2023.4.11.12.36.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.11.12.25.19
+Version: 2023.4.11.12.36.5
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.11.12.25.19/README.rst` & `llm4gpt-2023.4.11.12.36.5/README.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/docs/Makefile` & `llm4gpt-2023.4.11.12.36.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/docs/conf.py` & `llm4gpt-2023.4.11.12.36.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/docs/installation.rst` & `llm4gpt-2023.4.11.12.36.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/docs/make.bat` & `llm4gpt-2023.4.11.12.36.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/llm4gpt.egg-info/PKG-INFO` & `llm4gpt-2023.4.11.12.36.5/llm4gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4gpt
-Version: 2023.4.11.12.25.19
+Version: 2023.4.11.12.36.5
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: LLM4GPT
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4gpt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4gpt-2023.4.11.12.25.19/setup.py` & `llm4gpt-2023.4.11.12.36.5/setup.py`

 * *Files identical despite different names*

### Comparing `llm4gpt-2023.4.11.12.25.19/tests/test_llm4gpt.py` & `llm4gpt-2023.4.11.12.36.5/tests/test_llm4gpt.py`

 * *Files identical despite different names*

