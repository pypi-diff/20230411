# Comparing `tmp/datayoga-1.8.0.tar.gz` & `tmp/datayoga-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datayoga-1.8.0.tar", max compression
+gzip compressed data, was "datayoga-1.9.0.tar", max compression
```

## Comparing `datayoga-1.8.0.tar` & `datayoga-1.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      497 2022-11-22 09:04:13.877360 datayoga-1.8.0/README.md
--rw-r--r--   0        0        0     1202 2022-11-22 09:04:39.325165 datayoga-1.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-22 09:04:13.877360 datayoga-1.8.0/src/datayoga/__init__.py
--rw-r--r--   0        0        0     4600 2022-11-22 09:04:13.877360 datayoga-1.8.0/src/datayoga/__main__.py
--rw-r--r--   0        0        0     1398 2022-11-22 09:04:13.877360 datayoga-1.8.0/src/datayoga/cli_helpers.py
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 datayoga-1.8.0/setup.py
--rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 datayoga-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      497 2022-11-23 19:28:55.950277 datayoga-1.9.0/README.md
+-rw-r--r--   0        0        0     1202 2022-11-23 19:29:20.762231 datayoga-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-23 19:28:55.950277 datayoga-1.9.0/src/datayoga/__init__.py
+-rw-r--r--   0        0        0     4600 2022-11-23 19:28:55.950277 datayoga-1.9.0/src/datayoga/__main__.py
+-rw-r--r--   0        0        0     1398 2022-11-23 19:28:55.950277 datayoga-1.9.0/src/datayoga/cli_helpers.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 datayoga-1.9.0/setup.py
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 datayoga-1.9.0/PKG-INFO
```

### Comparing `datayoga-1.8.0/pyproject.toml` & `datayoga-1.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datayoga"
-version = "1.8.0"
+version = "1.9.0"
 description = "DataYoga command line interface"
 authors = ["DataYoga <admin@datayoga.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = [
 ]
```

### Comparing `datayoga-1.8.0/src/datayoga/__main__.py` & `datayoga-1.9.0/src/datayoga/__main__.py`

 * *Files identical despite different names*

### Comparing `datayoga-1.8.0/src/datayoga/cli_helpers.py` & `datayoga-1.9.0/src/datayoga/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `datayoga-1.8.0/setup.py` & `datayoga-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
           'requests-mock>=1.9.3,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['datayoga = datayoga.__main__:main']}
 
 setup_kwargs = {
     'name': 'datayoga',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'DataYoga command line interface',
     'long_description': '# DataYoga CLI\n\n## Development\n\nTo set up environment in development mode:\n\n### Set Up Virtual Environment\n\n```bash\npython -m venv venv\nsource venv/bin/activate\n```\n\n### Upgrade `pip` to Latest Version\n\n> [Pip](https://pypi.org/project/pip) version 22 and up is needed for editable install.\n\n```bash\npython -m pip install --upgrade pip\n```\n\n### Install Dependencies\n\n```bash\ncd core\npython -m pip install -e .\n```\n\n## Run CLI in Development Mode\n\n```bash\npython ./cli/src/datayoga/__main__.py\n```\n',
     'author': 'DataYoga',
     'author_email': 'admin@datayoga.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `datayoga-1.8.0/PKG-INFO` & `datayoga-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datayoga
-Version: 1.8.0
+Version: 1.9.0
 Summary: DataYoga command line interface
 License: Apache-2.0
 Author: DataYoga
 Author-email: admin@datayoga.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

