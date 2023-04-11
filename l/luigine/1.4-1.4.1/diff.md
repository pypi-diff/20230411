# Comparing `tmp/luigine-1.4.tar.gz` & `tmp/luigine-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luigine-1.4.tar", last modified: Wed Mar 29 06:09:34 2023, max compression
+gzip compressed data, was "luigine-1.4.1.tar", last modified: Tue Apr 11 02:13:15 2023, max compression
```

## Comparing `luigine-1.4.tar` & `luigine-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-03-29 06:09:34.684123 luigine-1.4/
--rw-r--r--   0 kjn        (501) staff       (20)     1071 2022-09-27 13:51:52.000000 luigine-1.4/LICENSE
--rw-r--r--   0 kjn        (501) staff       (20)       24 2022-09-27 13:51:52.000000 luigine-1.4/MANIFEST.in
--rw-r--r--   0 kjn        (501) staff       (20)      202 2023-03-29 06:09:34.683963 luigine-1.4/PKG-INFO
--rw-r--r--   0 kjn        (501) staff       (20)     2233 2022-09-27 13:51:52.000000 luigine-1.4/README.md
--rw-r--r--   0 kjn        (501) staff       (20)       56 2023-03-29 06:02:42.000000 luigine-1.4/requirements.txt
--rw-r--r--   0 kjn        (501) staff       (20)       38 2023-03-29 06:09:34.684176 luigine-1.4/setup.cfg
--rw-r--r--   0 kjn        (501) staff       (20)      724 2023-03-29 05:40:56.000000 luigine-1.4/setup.py
-drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-03-29 06:09:34.669155 luigine-1.4/src/
-drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-03-29 06:09:34.682962 luigine-1.4/src/luigine/
--rw-r--r--   0 kjn        (501) staff       (20)      186 2022-09-27 13:51:52.000000 luigine-1.4/src/luigine/__init__.py
--rw-r--r--   0 kjn        (501) staff       (20)    19338 2023-03-29 05:59:37.000000 luigine-1.4/src/luigine/abc.py
--rw-r--r--   0 kjn        (501) staff       (20)     2510 2022-09-27 13:51:52.000000 luigine-1.4/src/luigine/utils.py
-drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-03-29 06:09:34.683763 luigine-1.4/src/luigine.egg-info/
--rw-r--r--   0 kjn        (501) staff       (20)      202 2023-03-29 06:09:34.000000 luigine-1.4/src/luigine.egg-info/PKG-INFO
--rw-r--r--   0 kjn        (501) staff       (20)      293 2023-03-29 06:09:34.000000 luigine-1.4/src/luigine.egg-info/SOURCES.txt
--rw-r--r--   0 kjn        (501) staff       (20)        1 2023-03-29 06:09:34.000000 luigine-1.4/src/luigine.egg-info/dependency_links.txt
--rw-r--r--   0 kjn        (501) staff       (20)       56 2023-03-29 06:09:34.000000 luigine-1.4/src/luigine.egg-info/requires.txt
--rw-r--r--   0 kjn        (501) staff       (20)        8 2023-03-29 06:09:34.000000 luigine-1.4/src/luigine.egg-info/top_level.txt
+drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-04-11 02:13:15.327992 luigine-1.4.1/
+-rw-r--r--   0 kjn        (501) staff       (20)     1071 2022-09-27 13:51:52.000000 luigine-1.4.1/LICENSE
+-rw-r--r--   0 kjn        (501) staff       (20)       24 2022-09-27 13:51:52.000000 luigine-1.4.1/MANIFEST.in
+-rw-r--r--   0 kjn        (501) staff       (20)      204 2023-04-11 02:13:15.327821 luigine-1.4.1/PKG-INFO
+-rw-r--r--   0 kjn        (501) staff       (20)     2233 2022-09-27 13:51:52.000000 luigine-1.4.1/README.md
+-rw-r--r--   0 kjn        (501) staff       (20)       49 2023-04-11 01:41:23.000000 luigine-1.4.1/requirements.txt
+-rw-r--r--   0 kjn        (501) staff       (20)       38 2023-04-11 02:13:15.328049 luigine-1.4.1/setup.cfg
+-rw-r--r--   0 kjn        (501) staff       (20)      726 2023-04-11 02:09:05.000000 luigine-1.4.1/setup.py
+drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-04-11 02:13:15.324379 luigine-1.4.1/src/
+drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-04-11 02:13:15.326346 luigine-1.4.1/src/luigine/
+-rw-r--r--   0 kjn        (501) staff       (20)      186 2022-09-27 13:51:52.000000 luigine-1.4.1/src/luigine/__init__.py
+-rw-r--r--   0 kjn        (501) staff       (20)    18901 2023-04-11 01:40:56.000000 luigine-1.4.1/src/luigine/abc.py
+-rw-r--r--   0 kjn        (501) staff       (20)     2510 2022-09-27 13:51:52.000000 luigine-1.4.1/src/luigine/utils.py
+drwxr-xr-x   0 kjn        (501) staff       (20)        0 2023-04-11 02:13:15.327439 luigine-1.4.1/src/luigine.egg-info/
+-rw-r--r--   0 kjn        (501) staff       (20)      204 2023-04-11 02:13:15.000000 luigine-1.4.1/src/luigine.egg-info/PKG-INFO
+-rw-r--r--   0 kjn        (501) staff       (20)      293 2023-04-11 02:13:15.000000 luigine-1.4.1/src/luigine.egg-info/SOURCES.txt
+-rw-r--r--   0 kjn        (501) staff       (20)        1 2023-04-11 02:13:15.000000 luigine-1.4.1/src/luigine.egg-info/dependency_links.txt
+-rw-r--r--   0 kjn        (501) staff       (20)       49 2023-04-11 02:13:15.000000 luigine-1.4.1/src/luigine.egg-info/requires.txt
+-rw-r--r--   0 kjn        (501) staff       (20)        8 2023-04-11 02:13:15.000000 luigine-1.4.1/src/luigine.egg-info/top_level.txt
```

### Comparing `luigine-1.4/LICENSE` & `luigine-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luigine-1.4/README.md` & `luigine-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `luigine-1.4/setup.py` & `luigine-1.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 setup(
     name='luigine',
-    version='1.4',
+    version='1.4.1',
     author='Hiroshi Kajino',
     url='https://github.com/kanojikajino/luigine',
     author_email='hiroshi.kajino.1989@gmail.com',
     package_dir={'': 'src'},
     packages=find_packages(where='src', exclude=['*.tests', '*.tests.*', 'tests.*', 'tests']),
     test_suite='tests',
     include_package_data=True,
```

### Comparing `luigine-1.4/src/luigine/abc.py` & `luigine-1.4.1/src/luigine/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,31 +99,23 @@
         the name of directory where the output of this task is stored
     output_ext : str
         extension of the output file
     '''
 
     __no_hash_keys__ = []
     hash_num = luigi.IntParameter(default=10)
-    use_mlflow = luigi.BoolParameter(default=False)
     remove_output_file = luigi.BoolParameter(default=False)
     copy_output_to_top = luigi.Parameter(default='')
     output_ext = luigi.Parameter(default='pklz')
     working_dir = luigi.Parameter()  # used for argparse
     _working_dir = ''  # containing full path
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.param_name = ''
-        if self.use_mlflow:
-            import mlflow
-            self.mlflow = mlflow
-            mlflow.set_tracking_uri(str(self._working_dir / 'mlruns'))
-            if mlflow.active_run() is None:
-                mlflow.set_experiment(self.__class__.__name__)
-                mlflow.start_run()
 
         # md5checksum of input files
         if self.input_file():
             for each_input_file in self.input_file():
                 self.param_name = self.param_name + checksum(each_input_file)[:self.hash_num] + '_'
 
         param_kwargs = deepcopy(self.__dict__['param_kwargs'])
@@ -224,16 +216,14 @@
             with open(self.output().path, 'wb') as f:
                 pickle.dump(obj, f)
         elif self.output_ext == 'dill':
             with open(self.output().path, 'wb') as f:
                 dill.dump(obj, f)
         else:
             raise ValueError('ext {} is not supported'.format(self.output_ext))
-        if self.use_mlflow:
-            self.mlflow.log_artifact(self.output().path)
 
     def check_input(self, input_list):
         ''' check the input format
         '''
         return True
 
     def check_output(self, res):
```

### Comparing `luigine-1.4/src/luigine/utils.py` & `luigine-1.4.1/src/luigine/utils.py`

 * *Files identical despite different names*

