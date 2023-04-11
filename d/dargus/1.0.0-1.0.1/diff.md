# Comparing `tmp/dargus-1.0.0.tar.gz` & `tmp/dargus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-sa2qc9r_/dargus-1.0.0.tar", last modified: Tue Feb 21 15:07:27 2023, max compression
+gzip compressed data, was "/home/dapregi/dev/argus/dist/.tmp-f4ae7f3i/dargus-1.0.1.tar", last modified: Tue Apr 11 13:56:45 2023, max compression
```

## Comparing `dargus-1.0.0.tar` & `dargus-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-02-21 15:07:27.000000 dargus-1.0.0/
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.0.0/LICENSE
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-02-21 15:07:27.000000 dargus-1.0.0/PKG-INFO
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       73 2023-02-17 13:43:50.000000 dargus-1.0.0/README.md
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus/
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)        0 2020-07-29 10:38:30.000000 dargus-1.0.0/dargus/__init__.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    12936 2023-02-21 14:33:18.000000 dargus-1.0.0/dargus/argus.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1379 2023-02-21 14:32:30.000000 dargus-1.0.0/dargus/argus_cli.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1724 2023-02-16 16:37:40.000000 dargus-1.0.0/dargus/argus_config.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       43 2020-07-29 10:38:30.000000 dargus-1.0.0/dargus/argus_exceptions.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-02-06 09:28:40.000000 dargus-1.0.0/dargus/commons.py
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1567 2023-02-06 09:22:09.000000 dargus-1.0.0/dargus/utils.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)      889 2020-07-29 10:38:30.000000 dargus-1.0.0/dargus/validation_result.py
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)     7118 2023-02-21 14:33:18.000000 dargus-1.0.0/dargus/validator.py
-drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus.egg-info/
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus.egg-info/PKG-INFO
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus.egg-info/SOURCES.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus.egg-info/dependency_links.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus.egg-info/entry_points.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus.egg-info/requires.txt
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-02-21 15:07:27.000000 dargus-1.0.0/dargus.egg-info/top_level.txt
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-02-21 15:07:19.000000 dargus-1.0.0/pyproject.toml
--rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-02-21 15:07:27.000000 dargus-1.0.0/setup.cfg
--rw-r--r--   0 dapregi   (1000) dapregi   (1000)       92 2023-02-17 14:07:57.000000 dargus-1.0.0/setup.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-11 13:56:45.000000 dargus-1.0.1/
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)    11357 2020-07-29 10:38:30.000000 dargus-1.0.1/LICENSE
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-11 13:56:45.000000 dargus-1.0.1/PKG-INFO
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)       73 2023-02-17 13:43:50.000000 dargus-1.0.1/README.md
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus/
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)        0 2020-07-29 10:38:30.000000 dargus-1.0.1/dargus/__init__.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13118 2023-03-29 12:05:47.000000 dargus-1.0.1/dargus/argus.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1940 2023-04-11 13:10:00.000000 dargus-1.0.1/dargus/argus_cli.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     2224 2023-03-29 12:05:47.000000 dargus-1.0.1/dargus/argus_config.py
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)       43 2020-07-29 10:38:30.000000 dargus-1.0.1/dargus/argus_exceptions.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      928 2023-02-06 09:28:40.000000 dargus-1.0.1/dargus/commons.py
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)     1567 2023-02-06 09:22:09.000000 dargus-1.0.1/dargus/utils.py
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)      889 2020-07-29 10:38:30.000000 dargus-1.0.1/dargus/validation_result.py
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)     7118 2023-02-21 14:33:18.000000 dargus-1.0.1/dargus/validator.py
+drwxrwxr-x   0 dapregi   (1000) dapregi   (1000)        0 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)    13751 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/PKG-INFO
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)      410 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/SOURCES.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        1 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/dependency_links.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       49 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/entry_points.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       29 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/requires.txt
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)        7 2023-04-11 13:56:45.000000 dargus-1.0.1/dargus.egg-info/top_level.txt
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)     1042 2023-04-11 13:50:24.000000 dargus-1.0.1/pyproject.toml
+-rw-rw-r--   0 dapregi   (1000) dapregi   (1000)       38 2023-04-11 13:56:45.000000 dargus-1.0.1/setup.cfg
+-rw-r--r--   0 dapregi   (1000) dapregi   (1000)       92 2023-02-17 14:07:57.000000 dargus-1.0.1/setup.py
```

### Comparing `dargus-1.0.0/LICENSE` & `dargus-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dargus-1.0.0/PKG-INFO` & `dargus-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.0.0/dargus/argus.py` & `dargus-1.0.1/dargus/argus.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,24 +46,24 @@
         self.validation = validation
 
     def __str__(self):
         return str(self.__dict__)
 
 
 class Argus:
-    def __init__(self, test_folder, config_fpath, out_fpath=None):
+    def __init__(self, test_folder, argus_config, out_fpath=None):
         self.test_folder = test_folder
-        self.config_fpath = config_fpath
-        with open(config_fpath, 'r') as fhand:
-            self.config = yaml.safe_load(fhand)
+
+        self.config = argus_config
 
         if out_fpath is None:
             t = datetime.now().strftime('%Y%m%d%H%M%S')
             self.out_fpath = os.path.join(test_folder, 'argus_out_' + t + '.json')
         else:
+            os.makedirs(os.path.dirname(out_fpath), exist_ok=True)
             self.out_fpath = out_fpath
 
         self.suites = []
 
         self.suite_ids = []
         self.test_ids = []
         self.task_ids = []
@@ -78,15 +78,15 @@
         self.async_jobs = []
         self.validation_results = []
 
         self._parse_files(self.test_folder)
         self._generate_headers()
         self._generate_token()
 
-        if 'validator' in self.config:
+        if 'validator' in self.config and self.config['validator'] is not None:
             import importlib.util
             val_path = self.config['validator']
             val_fname = os.path.basename(val_path)
             val_name = val_fname[:-3] if val_fname.endswith('.py') else val_fname
             cls_name = ''.join(x.title() for x in val_name.split('_'))
             spec = importlib.util.spec_from_file_location(cls_name, val_path)
             foo = importlib.util.module_from_spec(spec)
@@ -97,26 +97,26 @@
             )
         else:
             self.validator = Validator(
                 validation=self.config.get('validation')
             )
 
     def _generate_headers(self):
-        if 'rest' in self.config and self.config['rest'] and self.config['rest']['headers']:
+        if 'rest' in self.config and self.config['rest'] is not None and self.config['rest']['headers']:
             self.headers = self.config['rest']['headers']
 
     @staticmethod
     def _login(auth, field):
         url = create_url(auth['url'], auth.get('pathParams'),
                          auth.get('queryParams'))
         response = query(url, method=auth.get('method'), headers=auth.get('headers'), body=auth.get('body'))
         return get_item(response.json(), field)
 
     def _generate_token(self):
-        if 'authentication' in self.config:
+        if 'authentication' in self.config and self.config['authentication'] is not None:
             auth = self.config['authentication']
             token_func = re.findall(r'^(.+)\((.+)\)$', auth['token'])
             if token_func:
                 if token_func[0][0] == 'env':
                     self.token = os.environ[token_func[1]]
                 elif token_func[0][0] == 'login':
                     self.token = self._login(auth, token_func[0][1])
@@ -142,15 +142,15 @@
         if id_ is None:
             raise ValueError('Field "id" is required for each suite')
         if id_ in self.suite_ids:
             raise ValueError('Duplicated suite IDs "{}"'.format(id_))
         self.suite_ids.append(id_)
 
         # Filtering suites to run
-        if 'suites' in self.config:
+        if 'suites' in self.config and self.config['suites'] is not None:
             if id_ not in self.config['suites']:
                 return None
 
         base_url = suite.get('baseUrl')
 
         tests = list(filter(
             None, [self._parse_test(test) for test in suite.get('tests')]
@@ -171,15 +171,15 @@
 
         tags = test.get('tags').split(',') if test.get('tags') else None
         path = test.get('path')
         method = test.get('method')
         async_ = test.get('async')
 
         # Filtering tests to run
-        if 'validation' in self.config:
+        if 'validation' in self.config and self.config['validation'] is not None:
             validation = self.config['validation']
             if 'ignore_async' in validation:
                 if async_ in validation['ignore_async']:
                     return None
             if 'ignore_method' in self.config['validation']:
                 if method in validation['ignore_method']:
                     return None
@@ -265,15 +265,15 @@
         if matrix_params is not None:
             matrix_params_list = self._parse_matrix_params(matrix_params)
             query_params_list = self._merge_params(id_, query_params, matrix_params_list)
         else:
             query_params_list = [query_params]
 
         # Adding default queryParams
-        if 'rest' in self.config and self.config['rest']['queryParams']:
+        if 'rest' in self.config and self.config['rest'] is not None and self.config['rest']['queryParams']:
             default_params = self.config['rest']['queryParams']
             for query_params in query_params_list:
                 for key in default_params:
                     if key not in query_params:
                         query_params[key] = default_params[key]
 
         # Parsing body matrix params
```

### Comparing `dargus-1.0.0/dargus/argus_cli.py` & `dargus-1.0.1/dargus/argus_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import sys
 import argparse
 
 from dargus.argus import Argus
+from dargus.argus_config import ArgusConfiguration
 
 
 class ArgusCLI:
 
     def __init__(self):
         self._parser = argparse.ArgumentParser(
             description='This program checks automatically all defined tests'
@@ -29,26 +30,40 @@
         parser = self.subparsers.add_parser('execute')
         parser.add_argument('config',
                             help='configuration YML file path')
         parser.add_argument('suite_dir',
                             help='test folder containing suite YML files')
         parser.add_argument('-o', '--output',
                             help='output file path')
-        # parser.add_argument('--suites',
-        #                     help='suites to run; overrule config file')
+        parser.add_argument('-v', '--validator',
+                            help='validator file path')
+        # parser.add_argument('-u', '--username',
+        #                     help='validator file path')
+        # parser.add_argument('-p', '--password',
+        #                     help='validator file path')
+        parser.add_argument('-s', '--suites',
+                            help='suites to run')
 
     def _stats(self):
         parser = self.subparsers.add_parser('stats')
         parser.add_argument('input', help='json file')
 
 
 def main():
 
     cli = ArgusCLI()
     args = cli.parser.parse_args()
 
-    client_generator = Argus(args.suite_dir, args.config, args.output)
+    argus_config = ArgusConfiguration(
+        args.config,
+        validator=args.validator,
+        # username=args.username,
+        # password=args.password
+        suites=args.suites
+    ).get_config()
+
+    client_generator = Argus(args.suite_dir, argus_config, args.output)
     client_generator.execute()
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `dargus-1.0.0/dargus/argus_config.py` & `dargus-1.0.1/dargus/argus_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 import json
 import requests
 import yaml
 
 
 class ArgusConfiguration(object):
-    def __init__(self, config_input):
+    def __init__(self, config_input, validator=None, username=None, password=None, suites=None):
         # Default config params
         self._config = {
             'authentication': None,
             'suites': None,
             'validation': None,
-            'validator': None
+            'validator': None,
+            'tests': None
         }
 
-        # Load config
-        self._configuration_input = config_input
+        self.load_config(config_input, validator, suites)
 
+        self._validate_configuration(self._config)
+
+    def load_config(self, config_input, validator, suites):
         if isinstance(config_input, dict):
-            self._config = config_input
+            for key in config_input:
+                self._config[key] = config_input[key]
         else:
-            self._config = self._get_dictionary_from_file(config_input)
+            config_dict = self._get_dictionary_from_file(config_input)
+            for key in config_dict:
+                self._config[key] = config_dict[key]
+
+        if validator is not None:
+            self._config['validator'] = validator
+
+        if suites is not None:
+            self._config['suites'] = suites.split(',')
 
-        self._validate_configuration(self._config)
 
     @staticmethod
     def _get_dictionary_from_file(config_fpath):
         try:
             config_fhand = open(config_fpath, 'r')
         except IOError:
             msg = 'Unable to read file "' + config_fpath + '"'
@@ -58,7 +69,10 @@
     @property
     def authentication(self):
         return self._config['authentication']
 
     @authentication.setter
     def authentication(self, new_authentication):
         self._config['authentication'] = new_authentication
+
+    def get_config(self):
+        return self._config
```

### Comparing `dargus-1.0.0/dargus/commons.py` & `dargus-1.0.1/dargus/commons.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.0/dargus/utils.py` & `dargus-1.0.1/dargus/utils.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.0/dargus/validation_result.py` & `dargus-1.0.1/dargus/validation_result.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.0/dargus/validator.py` & `dargus-1.0.1/dargus/validator.py`

 * *Files identical despite different names*

### Comparing `dargus-1.0.0/dargus.egg-info/PKG-INFO` & `dargus-1.0.1/dargus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargus
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python engine for testing and benchmarking REST web services
 Author-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 Maintainer-email: Daniel Perez-Gil <daniel.perez@zettagenomics.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dargus-1.0.0/pyproject.toml` & `dargus-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["dargus"]
 
 [project]
 name = "dargus"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python engine for testing and benchmarking REST web services"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
   {name="Daniel Perez-Gil", email="daniel.perez@zettagenomics.com"}
 ]
```

