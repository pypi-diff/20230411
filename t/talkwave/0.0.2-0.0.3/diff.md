# Comparing `tmp/talkwave-0.0.2.tar.gz` & `tmp/talkwave-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkwave-0.0.2.tar", last modified: Tue Apr 11 08:14:26 2023, max compression
+gzip compressed data, was "talkwave-0.0.3.tar", last modified: Tue Apr 11 16:12:10 2023, max compression
```

## Comparing `talkwave-0.0.2.tar` & `talkwave-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:26.686118 talkwave-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-11 08:14:10.000000 talkwave-0.0.2/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-11 08:14:10.000000 talkwave-0.0.2/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 08:14:10.000000 talkwave-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 08:14:26.686118 talkwave-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-11 08:14:10.000000 talkwave-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-11 08:14:10.000000 talkwave-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-11 08:14:26.686118 talkwave-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-11 08:14:10.000000 talkwave-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:26.686118 talkwave-0.0.2/talkwave/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-11 08:14:10.000000 talkwave-0.0.2/talkwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-11 08:14:10.000000 talkwave-0.0.2/talkwave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-11 08:14:10.000000 talkwave-0.0.2/talkwave/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-11 08:14:10.000000 talkwave-0.0.2/talkwave/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:26.686118 talkwave-0.0.2/talkwave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 08:14:26.000000 talkwave-0.0.2/talkwave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 08:14:26.000000 talkwave-0.0.2/talkwave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:14:26.000000 talkwave-0.0.2/talkwave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 08:14:26.000000 talkwave-0.0.2/talkwave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 08:14:26.000000 talkwave-0.0.2/talkwave.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:14:26.686118 talkwave-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-11 08:14:10.000000 talkwave-0.0.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:12:10.042144 talkwave-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-11 16:12:01.000000 talkwave-0.0.3/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-11 16:12:01.000000 talkwave-0.0.3/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 16:12:01.000000 talkwave-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 16:12:10.042144 talkwave-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-11 16:12:01.000000 talkwave-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-11 16:12:01.000000 talkwave-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-11 16:12:10.042144 talkwave-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-11 16:12:01.000000 talkwave-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:12:10.042144 talkwave-0.0.3/talkwave/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-11 16:12:01.000000 talkwave-0.0.3/talkwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-11 16:12:01.000000 talkwave-0.0.3/talkwave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-11 16:12:01.000000 talkwave-0.0.3/talkwave/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-11 16:12:01.000000 talkwave-0.0.3/talkwave/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:12:10.042144 talkwave-0.0.3/talkwave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 16:12:10.000000 talkwave-0.0.3/talkwave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-11 16:12:10.000000 talkwave-0.0.3/talkwave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:12:10.000000 talkwave-0.0.3/talkwave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 16:12:10.000000 talkwave-0.0.3/talkwave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:12:10.000000 talkwave-0.0.3/talkwave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:12:10.042144 talkwave-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-11 16:12:01.000000 talkwave-0.0.3/tests/test_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-11 16:12:01.000000 talkwave-0.0.3/tests/test_main.py
```

### Comparing `talkwave-0.0.2/LICENSE-APACHE` & `talkwave-0.0.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.2/LICENSE-MIT` & `talkwave-0.0.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.2/PKG-INFO` & `talkwave-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkwave
-Version: 0.0.2
+Version: 0.0.3
 Summary: TalkWave is an AI chatbot for developers written in Python.
 Home-page: https://github.com/sebastienrousseau/talkwave
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache License 2.0
 Keywords: talkwave,chatbot,AI,machine learningnatural language processing OpenAI GPT-3 GPT3 GPT python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `talkwave-0.0.2/README.md` & `talkwave-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.2/pyproject.toml` & `talkwave-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkwave"
-version = "0.0.2"
+version = "0.0.3"
 description = "TalkWave is an AI chatbot for developers written in Python."
 authors = ["Sebastien Rousseau <sebastian.rousseau at gmail.com>"]
 license = "Apache Software License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `talkwave-0.0.2/setup.cfg` & `talkwave-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = talkwave
-version = 0.0.2
+version = 0.0.3
 author = Sebastian Rousseau
 author_email = sebastian.rousseau@gmail.com
 description = TalkWave is an AI chatbot for developers written in Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sebastienrousseau/talkwave
 license = Apache Software License
```

### Comparing `talkwave-0.0.2/setup.py` & `talkwave-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 TEST_DEPENDENCIES = [
     "coverage>=7.2.3",
     "pytest-cov>=4.0.0",
     "pytest>=7.3.0",
 ]
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 URL = 'https://github.com/sebastienrousseau/talkwave'
 
 setup(
     name='talkwave',
     version=VERSION,
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

### Comparing `talkwave-0.0.2/talkwave/__init__.py` & `talkwave-0.0.3/talkwave/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,8 +95,8 @@
 - [MIT license](https://opensource.org/licenses/MIT)
 
 """
 
 """The Python talkwave module."""
 __all__ = ["__version__"]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

### Comparing `talkwave-0.0.2/talkwave/__main__.py` & `talkwave-0.0.3/talkwave/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # set the directory where the data is stored, value is a string from an
 # environment variable "DIR_PATH" (required).
 dir_path = os.path.join(os.path.dirname(os.path.realpath(
     __file__)), os.environ.get('DIR_PATH', 'data'))
 
 if __name__ == "__main__":
     # Set the title and description of the program
-    title = "TalkWave 🐍 (v0.0.2)"
+    title = "TalkWave 🐍 (v0.0.3)"
     description = "An AI chatbot for developers"
 
     # Print the title and description of the program
     title_table = tabulate([[title], [description]], tablefmt="rounded_grid")
     print()
     print(title_table)
     print()
```

### Comparing `talkwave-0.0.2/talkwave/frontend.py` & `talkwave-0.0.3/talkwave/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,19 @@
             max_tokens,
             temperature,
             user_id,
             rate_limit_seconds,
             stop,
             output_format
         )
-        return render_template('index.html', response=response, prompt=request.form['prompt'])
+        return render_template(
+            'index.html',
+            response=response,
+            prompt=request.form['prompt']
+        )
     else:
         return render_template('index.html')
 
 
 if __name__ == '__main__':
     """
     This block of code starts the Flask app if the script is run as the
```

### Comparing `talkwave-0.0.2/talkwave.egg-info/PKG-INFO` & `talkwave-0.0.3/talkwave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkwave
-Version: 0.0.2
+Version: 0.0.3
 Summary: TalkWave is an AI chatbot for developers written in Python.
 Home-page: https://github.com/sebastienrousseau/talkwave
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache License 2.0
 Keywords: talkwave,chatbot,AI,machine learningnatural language processing OpenAI GPT-3 GPT3 GPT python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `talkwave-0.0.2/tests/test_main.py` & `talkwave-0.0.3/tests/test_main.py`

 * *Files identical despite different names*

