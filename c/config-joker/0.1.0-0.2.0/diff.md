# Comparing `tmp/config_joker-0.1.0.tar.gz` & `tmp/config_joker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_joker-0.1.0.tar", max compression
+gzip compressed data, was "config_joker-0.2.0.tar", max compression
```

## Comparing `config_joker-0.1.0.tar` & `config_joker-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1083 2023-04-04 01:35:47.633704 config_joker-0.1.0/LICENSE
--rw-r--r--   0        0        0      639 2023-04-05 01:32:03.673229 config_joker-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-04 02:48:51.887021 config_joker-0.1.0/config_joker/__init__.py
--rw-r--r--   0        0        0     1293 2023-04-05 01:44:05.797405 config_joker-0.1.0/config_joker/config.py
--rw-r--r--   0        0        0        0 2023-04-04 02:48:43.263208 config_joker-0.1.0/config_joker/sources/__init__.py
--rw-r--r--   0        0        0      422 2023-04-04 03:07:58.416142 config_joker-0.1.0/config_joker/sources/environment.py
--rw-r--r--   0        0        0      303 2023-04-04 02:54:28.927985 config_joker-0.1.0/config_joker/sources/source.py
--rw-r--r--   0        0        0      402 2023-04-04 01:50:25.436814 config_joker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 config_joker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-04 01:35:47.633704 config_joker-0.2.0/LICENSE
+-rw-r--r--   0        0        0      730 2023-04-11 01:35:43.700475 config_joker-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-04 02:48:51.887021 config_joker-0.2.0/config_joker/__init__.py
+-rw-r--r--   0        0        0     1293 2023-04-05 01:44:05.797405 config_joker-0.2.0/config_joker/config.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:48:43.263208 config_joker-0.2.0/config_joker/sources/__init__.py
+-rw-r--r--   0        0        0      422 2023-04-04 03:07:58.416142 config_joker-0.2.0/config_joker/sources/environment.py
+-rw-r--r--   0        0        0      360 2023-04-11 01:44:37.188523 config_joker-0.2.0/config_joker/sources/source.py
+-rw-r--r--   0        0        0      680 2023-04-11 03:34:20.915789 config_joker-0.2.0/config_joker/sources/yamlfile.py
+-rw-r--r--   0        0        0        0 2023-04-11 02:22:08.615358 config_joker-0.2.0/config_joker/utils/__init__.py
+-rw-r--r--   0        0        0      997 2023-04-11 03:33:33.152316 config_joker-0.2.0/config_joker/utils/parser.py
+-rw-r--r--   0        0        0      403 2023-04-11 03:46:30.706740 config_joker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 config_joker-0.2.0/PKG-INFO
```

### Comparing `config_joker-0.1.0/LICENSE` & `config_joker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `config_joker-0.1.0/config_joker/config.py` & `config_joker-0.2.0/config_joker/config.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.1.0/PKG-INFO` & `config_joker-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: config-joker
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package to ease usage of different configuration conditions in your projects.
 Author: Joao Pedro Mendes Goulart
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: regex (>=2023.3.23,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # config-joker
 A package to ease usage of different configuration conditions in your projects.
 
 ## How to use in
 
@@ -22,17 +22,18 @@
     from config_joker.sources.environment import EnvironmentSource
     from config_joker.config import Config
 
 Initialize the config class implementing the sources you want to use:
 
     config = Config(
             sources=[
-                EnvironmentSource(})
+                EnvironmentSource()
             ]
         )
 
 Find the configurations you want to use:
 
     import os
     os.environ['env_variable'] = '1'
     number_one_from_env_source_as_int = config.required(key='env_variable', value_type=int)
 
+The value stored in number_one_from_env_source_as_int will be the number one as an integer.
```

