# Comparing `tmp/llamabot-0.0.5.tar.gz` & `tmp/llamabot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamabot-0.0.5.tar", last modified: Mon Apr 10 22:48:22 2023, max compression
+gzip compressed data, was "llamabot-0.0.6.tar", last modified: Tue Apr 11 12:47:44 2023, max compression
```

## Comparing `llamabot-0.0.5.tar` & `llamabot-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.371590 llamabot-0.0.5/
--rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.5/MANIFEST.in
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-10 22:48:22.371441 llamabot-0.0.5/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     5647 2023-04-04 15:17:20.000000 llamabot-0.0.5/README.md
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.369794 llamabot-0.0.5/llamabot/
--rw-r--r--   0 ericmjl    (501) staff       (20)      284 2023-04-10 22:45:50.000000 llamabot-0.0.5/llamabot/__init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     5720 2023-04-10 22:47:57.000000 llamabot-0.0.5/llamabot/bot.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/preprocessing.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/schemas.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/utils.py
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.370635 llamabot-0.0.5/llamabot.egg-info/
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)      409 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/SOURCES.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/dependency_links.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/entry_points.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       90 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/requires.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/top_level.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)     1529 2023-04-10 22:48:19.000000 llamabot-0.0.5/pyproject.toml
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-10 22:48:22.371632 llamabot-0.0.5/setup.cfg
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.371231 llamabot-0.0.5/tests/
--rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.5/tests/test___init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.5/tests/test_cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.5/tests/test_models.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.620686 llamabot-0.0.6/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.6/MANIFEST.in
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-11 12:47:44.620551 llamabot-0.0.6/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     5647 2023-04-04 15:17:20.000000 llamabot-0.0.6/README.md
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.619249 llamabot-0.0.6/llamabot/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      284 2023-04-10 22:45:50.000000 llamabot-0.0.6/llamabot/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     5720 2023-04-11 12:47:19.000000 llamabot-0.0.6/llamabot/bot.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/preprocessing.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/schemas.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/utils.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.619998 llamabot-0.0.6/llamabot.egg-info/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)      409 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/SOURCES.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/dependency_links.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/entry_points.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       90 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/requires.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/top_level.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1529 2023-04-11 12:47:41.000000 llamabot-0.0.6/pyproject.toml
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-11 12:47:44.620725 llamabot-0.0.6/setup.cfg
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.620379 llamabot-0.0.6/tests/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.6/tests/test___init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.6/tests/test_cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.6/tests/test_models.py
```

### Comparing `llamabot-0.0.5/README.md` & `llamabot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `llamabot-0.0.5/llamabot/bot.py` & `llamabot-0.0.6/llamabot/bot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.0.5/llamabot/cli.py` & `llamabot-0.0.6/llamabot/cli.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.0.5/pyproject.toml` & `llamabot-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 namespaces = false
 
 [project]
 name = "llamabot"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
     "openai",
     "langchain",
     "typer"
 ]
 
 [project.optional-dependencies]
```

