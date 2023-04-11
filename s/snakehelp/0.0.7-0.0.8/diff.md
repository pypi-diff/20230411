# Comparing `tmp/snakehelp-0.0.7.tar.gz` & `tmp/snakehelp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakehelp-0.0.7.tar", last modified: Sat Mar 25 18:08:12 2023, max compression
+gzip compressed data, was "snakehelp-0.0.8.tar", last modified: Tue Apr 11 12:16:44 2023, max compression
```

## Comparing `snakehelp-0.0.7.tar` & `snakehelp-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:12.400515 snakehelp-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-25 18:07:40.000000 snakehelp-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-25 18:07:40.000000 snakehelp-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-25 18:08:12.400515 snakehelp-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-25 18:08:12.400515 snakehelp-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-25 18:07:40.000000 snakehelp-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:12.400515 snakehelp-0.0.7/snakehelp/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/parameter_combinations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/snakehelp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-25 18:07:40.000000 snakehelp-0.0.7/snakehelp/test_parameter_combinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:12.400515 snakehelp-0.0.7/snakehelp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-25 18:08:12.000000 snakehelp-0.0.7/snakehelp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-25 18:08:12.000000 snakehelp-0.0.7/snakehelp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 18:08:12.000000 snakehelp-0.0.7/snakehelp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 18:08:12.000000 snakehelp-0.0.7/snakehelp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-25 18:08:12.000000 snakehelp-0.0.7/snakehelp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-25 18:08:12.000000 snakehelp-0.0.7/snakehelp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:12.400515 snakehelp-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-25 18:07:40.000000 snakehelp-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 18:08:12.400515 snakehelp-0.0.7/tests/property_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-25 18:07:40.000000 snakehelp-0.0.7/tests/property_tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-03-25 18:07:40.000000 snakehelp-0.0.7/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-25 18:07:40.000000 snakehelp-0.0.7/tests/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 12:16:10.000000 snakehelp-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 12:16:10.000000 snakehelp-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 12:16:44.512581 snakehelp-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-11 12:16:44.512581 snakehelp-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-11 12:16:10.000000 snakehelp-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/snakehelp/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/parameter_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/snakehelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/test_parameter_combinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/snakehelp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/tests/property_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/property_tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/test_plotting.py
```

### Comparing `snakehelp-0.0.7/LICENSE` & `snakehelp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.7/PKG-INFO` & `snakehelp-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakehelp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Snakehelp: Making snakemake easier to use.
 Home-page: https://github.com/ivargr/snakehelp
 Author: Ivar Grytten
 Author-email: ivar.grytten@gmail.com
 License: MIT license
 Keywords: snakehelp
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snakehelp-0.0.7/setup.py` & `snakehelp-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     include_package_data=True,
     keywords='snakehelp',
     name='snakehelp',
     packages=find_packages(include=['snakehelp', 'snakehelp.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ivargr/snakehelp',
-    version='0.0.7',
+    version='0.0.8',
     zip_safe=False,
 )
```

### Comparing `snakehelp-0.0.7/snakehelp/parameter_combinations.py` & `snakehelp-0.0.8/snakehelp/parameter_combinations.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.7/snakehelp/parameters.py` & `snakehelp-0.0.8/snakehelp/parameters.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.7/snakehelp/plotting.py` & `snakehelp-0.0.8/snakehelp/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         for parameter in self._plot_type.parameter_types():
             assert parameter in self._data, f"The plot type {self._plot_type} requires parameter {parameter} to be specified."
 
     def file_names(self):
         return self._parameter_combinations.get_files(**self._data)
 
-    def plot(self):
+    def plot(self, pretty_names_func=None):
         df = self._parameter_combinations.get_results_dataframe(**self._data)
         df.to_csv(self._out_base_name + ".csv", index=False)
 
         markdown_table = tabulate.tabulate(df, headers=df.columns, tablefmt="github")
         with open(self._out_base_name + ".txt", "w") as f:
             f.write(markdown_table + "\n")
 
@@ -127,16 +127,17 @@
             specification["text"] = self._plot_type.labels
 
         assert self._plot_type.type in plotting_functions, "Plot type %s not supported"
         func = plotting_functions[self._plot_type.type]
         fig = func(df, **specification, template="simple_white", title=title)
 
         # prettier facet titles, names, etc
-        #fig.for_each_annotation(lambda a: a.update(text=pretty_name(a.text.split("=")[-1])))
-        #fig.for_each_trace(lambda t: t.update(name=pretty_name(t.name)))
+        if pretty_names_func is not None:
+            fig.for_each_annotation(lambda a: a.update(text=pretty_names_func(a.text.split("=")[-1])))
+            fig.for_each_trace(lambda t: t.update(name=pretty_names_func(t.name)))
 
         if "text" in specification:
             fig.update_traces(textposition="bottom right")
 
         # fig.update_annotations(font=dict(size=20))
         # fig.update_layout(font=dict(size=20))
         if self._plot_type.layout is not None:
```

### Comparing `snakehelp-0.0.7/snakehelp/snakehelp.py` & `snakehelp-0.0.8/snakehelp/snakehelp.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.7/snakehelp/test_parameter_combinations.py` & `snakehelp-0.0.8/snakehelp/test_parameter_combinations.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.7/snakehelp.egg-info/PKG-INFO` & `snakehelp-0.0.8/snakehelp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakehelp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Snakehelp: Making snakemake easier to use.
 Home-page: https://github.com/ivargr/snakehelp
 Author: Ivar Grytten
 Author-email: ivar.grytten@gmail.com
 License: MIT license
 Keywords: snakehelp
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snakehelp-0.0.7/snakehelp.egg-info/SOURCES.txt` & `snakehelp-0.0.8/snakehelp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.7/tests/test_parameters.py` & `snakehelp-0.0.8/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.7/tests/test_plotting.py` & `snakehelp-0.0.8/tests/test_plotting.py`

 * *Files identical despite different names*

