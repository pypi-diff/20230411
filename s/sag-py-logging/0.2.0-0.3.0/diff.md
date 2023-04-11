# Comparing `tmp/sag-py-logging-0.2.0.tar.gz` & `tmp/sag-py-logging-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-logging-0.2.0.tar", last modified: Thu Apr  6 12:01:24 2023, max compression
+gzip compressed data, was "sag-py-logging-0.3.0.tar", last modified: Tue Apr 11 06:18:13 2023, max compression
```

## Comparing `sag-py-logging-0.2.0.tar` & `sag-py-logging-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:01:24.171465 sag-py-logging-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-06 12:01:24.171465 sag-py-logging-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:01:24.171465 sag-py-logging-0.2.0/sag_py_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/sag_py_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/sag_py_logging/console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/sag_py_logging/log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/sag_py_logging/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/sag_py_logging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:01:24.171465 sag-py-logging-0.2.0/sag_py_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-06 12:01:24.000000 sag-py-logging-0.2.0/sag_py_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-06 12:01:24.000000 sag-py-logging-0.2.0/sag_py_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 12:01:24.000000 sag-py-logging-0.2.0/sag_py_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 12:01:24.000000 sag-py-logging-0.2.0/sag_py_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 12:01:24.000000 sag-py-logging-0.2.0/sag_py_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-06 12:01:24.171465 sag-py-logging-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:01:24.171465 sag-py-logging-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/tests/test_console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-06 12:01:13.000000 sag-py-logging-0.2.0/tests/test_log_config_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.028520 sag-py-logging-0.3.0/sag_py_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/log_config_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/sag_py_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_log_config_processors.py
```

### Comparing `sag-py-logging-0.2.0/LICENSE.txt` & `sag-py-logging-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.2.0/PKG-INFO` & `sag-py-logging-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.2.0
+Version: 0.3.0
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: jinja
+Provides-Extra: toml
 License-File: LICENSE.txt
 
 # sag_py_logging
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_logging/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_logging)
@@ -42,50 +44,90 @@
 
 ## How to use
 
 ### Installation
 
 pip install sag-py-logging
 
+pip install sag-py-logging[jinia] (optional for templating)
+
+pip install sag-py-logging[toml] (optional for toml file support)
+
 ### Initialize logging from json
 
 Add the following as early as possible to your application code:
 
 ```python
 from sag_py_logging.log_config_initializer import init_logging
+from sag_py_logging.log_config_loader import JsonLoader, TomlLoader
+from sag_py_logging.log_config_processors import FormatProcessor, JinjaProcessor
 
 placeholder_container = { "host": "myhost.com", ...}
 
-init_logging("./log_config.json", config.logging_config)
+# For toml config with jinja templating
+init_logging(
+    "./log_config.toml",
+    loader=TomlLoader(),
+    processors=[JinjaProcessor(placeholder_container.__dict__)]
+)
+
+# For json config with format templating
+init_logging(
+    "./log_config.json",
+    loader=JsonLoader(),
+    processors=[FormatProcessor(placeholder_container.__dict__)]
+)
+
 ```
 
 Init logging returns the log configuration as dictionary if needed for further processing.
 
-### The json configuration
+### The configuration
 
+Json config:
 ```json
 {
     "version": 1,
-    "disable_existing_loggers": "true",
+    "disable_existing_loggers": false,
     "root": {
         "handlers": ["myhandler"],
         "level": "INFO"
     },
     "handlers": {
         "myhandler": {
             "host": "${host}",
             "formatter": "handler_formatter"
         }
     }
 }
 ```
+
+Toml config:
+```toml
+version = 1
+disable_existing_loggers = false
+
+[root]
+handlers = ["myhandler"]
+level = "INFO"
+
+[handlers.myhandler]
+host = "${host}"
+formatter = "handler_formatter"
+
+```
 This is a very basic sample on the format of the file including placeholders.
 
 Read the following for a full schema reference: https://docs.python.org/3/library/logging.config.html#configuration-dictionary-schema
 
+Read more on string templating here: https://docs.python.org/3/library/string.html#template-strings
+
+Or if you use jinja templating there: https://jinja.palletsprojects.com/en/3.1.x/templates/#template-designer-documentation
+
+
 ### Configure extra field logging
 
 It is possible to add a filter that extends log entries by a field for extra fields.
 
 The filter is added like that if you initialize logging by code:
 ```python
 from sag_py_logging.console_extra_field_filter import ConsoleExtraFieldFilter
```

### Comparing `sag-py-logging-0.2.0/README.md` & `sag-py-logging-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,50 +19,90 @@
 
 ## How to use
 
 ### Installation
 
 pip install sag-py-logging
 
+pip install sag-py-logging[jinia] (optional for templating)
+
+pip install sag-py-logging[toml] (optional for toml file support)
+
 ### Initialize logging from json
 
 Add the following as early as possible to your application code:
 
 ```python
 from sag_py_logging.log_config_initializer import init_logging
+from sag_py_logging.log_config_loader import JsonLoader, TomlLoader
+from sag_py_logging.log_config_processors import FormatProcessor, JinjaProcessor
 
 placeholder_container = { "host": "myhost.com", ...}
 
-init_logging("./log_config.json", config.logging_config)
+# For toml config with jinja templating
+init_logging(
+    "./log_config.toml",
+    loader=TomlLoader(),
+    processors=[JinjaProcessor(placeholder_container.__dict__)]
+)
+
+# For json config with format templating
+init_logging(
+    "./log_config.json",
+    loader=JsonLoader(),
+    processors=[FormatProcessor(placeholder_container.__dict__)]
+)
+
 ```
 
 Init logging returns the log configuration as dictionary if needed for further processing.
 
-### The json configuration
+### The configuration
 
+Json config:
 ```json
 {
     "version": 1,
-    "disable_existing_loggers": "true",
+    "disable_existing_loggers": false,
     "root": {
         "handlers": ["myhandler"],
         "level": "INFO"
     },
     "handlers": {
         "myhandler": {
             "host": "${host}",
             "formatter": "handler_formatter"
         }
     }
 }
 ```
+
+Toml config:
+```toml
+version = 1
+disable_existing_loggers = false
+
+[root]
+handlers = ["myhandler"]
+level = "INFO"
+
+[handlers.myhandler]
+host = "${host}"
+formatter = "handler_formatter"
+
+```
 This is a very basic sample on the format of the file including placeholders.
 
 Read the following for a full schema reference: https://docs.python.org/3/library/logging.config.html#configuration-dictionary-schema
 
+Read more on string templating here: https://docs.python.org/3/library/string.html#template-strings
+
+Or if you use jinja templating there: https://jinja.palletsprojects.com/en/3.1.x/templates/#template-designer-documentation
+
+
 ### Configure extra field logging
 
 It is possible to add a filter that extends log entries by a field for extra fields.
 
 The filter is added like that if you initialize logging by code:
 ```python
 from sag_py_logging.console_extra_field_filter import ConsoleExtraFieldFilter
```

### Comparing `sag-py-logging-0.2.0/sag_py_logging/console_extra_field_filter.py` & `sag-py-logging-0.3.0/sag_py_logging/console_extra_field_filter.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.2.0/sag_py_logging.egg-info/PKG-INFO` & `sag-py-logging-0.3.0/sag_py_logging.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.2.0
+Version: 0.3.0
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: jinja
+Provides-Extra: toml
 License-File: LICENSE.txt
 
 # sag_py_logging
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_logging/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_logging)
@@ -42,50 +44,90 @@
 
 ## How to use
 
 ### Installation
 
 pip install sag-py-logging
 
+pip install sag-py-logging[jinia] (optional for templating)
+
+pip install sag-py-logging[toml] (optional for toml file support)
+
 ### Initialize logging from json
 
 Add the following as early as possible to your application code:
 
 ```python
 from sag_py_logging.log_config_initializer import init_logging
+from sag_py_logging.log_config_loader import JsonLoader, TomlLoader
+from sag_py_logging.log_config_processors import FormatProcessor, JinjaProcessor
 
 placeholder_container = { "host": "myhost.com", ...}
 
-init_logging("./log_config.json", config.logging_config)
+# For toml config with jinja templating
+init_logging(
+    "./log_config.toml",
+    loader=TomlLoader(),
+    processors=[JinjaProcessor(placeholder_container.__dict__)]
+)
+
+# For json config with format templating
+init_logging(
+    "./log_config.json",
+    loader=JsonLoader(),
+    processors=[FormatProcessor(placeholder_container.__dict__)]
+)
+
 ```
 
 Init logging returns the log configuration as dictionary if needed for further processing.
 
-### The json configuration
+### The configuration
 
+Json config:
 ```json
 {
     "version": 1,
-    "disable_existing_loggers": "true",
+    "disable_existing_loggers": false,
     "root": {
         "handlers": ["myhandler"],
         "level": "INFO"
     },
     "handlers": {
         "myhandler": {
             "host": "${host}",
             "formatter": "handler_formatter"
         }
     }
 }
 ```
+
+Toml config:
+```toml
+version = 1
+disable_existing_loggers = false
+
+[root]
+handlers = ["myhandler"]
+level = "INFO"
+
+[handlers.myhandler]
+host = "${host}"
+formatter = "handler_formatter"
+
+```
 This is a very basic sample on the format of the file including placeholders.
 
 Read the following for a full schema reference: https://docs.python.org/3/library/logging.config.html#configuration-dictionary-schema
 
+Read more on string templating here: https://docs.python.org/3/library/string.html#template-strings
+
+Or if you use jinja templating there: https://jinja.palletsprojects.com/en/3.1.x/templates/#template-designer-documentation
+
+
 ### Configure extra field logging
 
 It is possible to add a filter that extends log entries by a field for extra fields.
 
 The filter is added like that if you initialize logging by code:
 ```python
 from sag_py_logging.console_extra_field_filter import ConsoleExtraFieldFilter
```

### Comparing `sag-py-logging-0.2.0/setup.py` & `sag-py-logging-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     LONG_DESCRIPTION = fh.read()
 
 with open("requirements.txt", "r") as fin:
     REQS = fin.read().splitlines()
 
 setuptools.setup(
     name="sag-py-logging",
-    version="0.2.0",
+    version="0.3.0",
     description="Initialize logging from a configuration json",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_logging",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
@@ -25,14 +25,14 @@
         "Topic :: Software Development",
     ],
     keywords="logging, extra, fields",
     packages=setuptools.find_packages(exclude=["tests"]),
     package_data={"sag_py_logging": ["py.typed"]},
     python_requires=">=3.8",
     install_requires=REQS,
-    extras_require={"dev": ["pytest"]},
+    extras_require={"dev": ["pytest"], "jinja": ["Jinja2>=3.1.2"], "toml": ["tomli>=2.0.1"]},
     project_urls={
         "Documentation": "https://github.com/SamhammerAG/sag_py_logging",
         "Bug Reports": "https://github.com/SamhammerAG/sag_py_logging/issues",
         "Source": "https://github.com/SamhammerAG/sag_py_logging",
     },
 )
```

### Comparing `sag-py-logging-0.2.0/tests/test_console_extra_field_filter.py` & `sag-py-logging-0.3.0/tests/test_console_extra_field_filter.py`

 * *Files identical despite different names*

