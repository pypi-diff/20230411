# Comparing `tmp/Benchmark-4dn-0.5.8.tar.gz` & `tmp/Benchmark-4dn-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Benchmark-4dn-0.5.8.tar", last modified: Tue Nov 12 20:29:00 2019, max compression
+gzip compressed data, was "dist/Benchmark-4dn-0.5.9.tar", last modified: Sat Nov 30 22:25:35 2019, max compression
```

## Comparing `Benchmark-4dn-0.5.8.tar` & `Benchmark-4dn-0.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 carl       (502) staff       (20)        0 2019-11-12 20:29:00.000000 Benchmark-4dn-0.5.8/
-drwxr-xr-x   0 carl       (502) staff       (20)        0 2019-11-12 20:29:00.000000 Benchmark-4dn-0.5.8/Benchmark/
--rw-r--r--   0 carl       (502) staff       (20)        0 2019-05-15 13:24:15.000000 Benchmark-4dn-0.5.8/Benchmark/__init__.py
--rw-r--r--   0 carl       (502) staff       (20)      127 2019-11-12 20:26:40.000000 Benchmark-4dn-0.5.8/Benchmark/_version.py
-drwxr-xr-x   0 carl       (502) staff       (20)        0 2019-11-12 20:29:00.000000 Benchmark-4dn-0.5.8/Benchmark/aws/
--rw-r--r--   0 carl       (502) staff       (20)   112589 2019-05-15 13:24:15.000000 Benchmark-4dn-0.5.8/Benchmark/aws/Amazon EC2 Instance Comparison.csv
--rw-r--r--   0 carl       (502) staff       (20)    21262 2019-11-12 20:26:40.000000 Benchmark-4dn-0.5.8/Benchmark/bfunctions.py
--rw-r--r--   0 carl       (502) staff       (20)      305 2019-05-15 13:24:15.000000 Benchmark-4dn-0.5.8/Benchmark/byteformat.py
--rw-r--r--   0 carl       (502) staff       (20)     7035 2019-06-07 15:10:57.000000 Benchmark-4dn-0.5.8/Benchmark/classes.py
--rw-r--r--   0 carl       (502) staff       (20)     2460 2019-11-12 20:26:40.000000 Benchmark-4dn-0.5.8/Benchmark/run.py
-drwxr-xr-x   0 carl       (502) staff       (20)        0 2019-11-12 20:29:00.000000 Benchmark-4dn-0.5.8/Benchmark_4dn.egg-info/
--rw-r--r--   0 carl       (502) staff       (20)        1 2019-11-12 20:28:59.000000 Benchmark-4dn-0.5.8/Benchmark_4dn.egg-info/dependency_links.txt
--rw-r--r--   0 carl       (502) staff       (20)     3805 2019-11-12 20:28:59.000000 Benchmark-4dn-0.5.8/Benchmark_4dn.egg-info/PKG-INFO
--rw-r--r--   0 carl       (502) staff       (20)      377 2019-11-12 20:28:59.000000 Benchmark-4dn-0.5.8/Benchmark_4dn.egg-info/SOURCES.txt
--rw-r--r--   0 carl       (502) staff       (20)       16 2019-11-12 20:28:59.000000 Benchmark-4dn-0.5.8/Benchmark_4dn.egg-info/top_level.txt
--rw-r--r--   0 carl       (502) staff       (20)     3805 2019-11-12 20:29:00.000000 Benchmark-4dn-0.5.8/PKG-INFO
--rw-r--r--   0 carl       (502) staff       (20)     2318 2019-06-07 15:10:57.000000 Benchmark-4dn-0.5.8/README.md
--rw-r--r--   0 carl       (502) staff       (20)       38 2019-11-12 20:29:00.000000 Benchmark-4dn-0.5.8/setup.cfg
--rw-r--r--   0 carl       (502) staff       (20)     1565 2019-10-15 15:02:51.000000 Benchmark-4dn-0.5.8/setup.py
-drwxr-xr-x   0 carl       (502) staff       (20)        0 2019-11-12 20:29:00.000000 Benchmark-4dn-0.5.8/tests/
--rw-r--r--   0 carl       (502) staff       (20)        0 2019-05-15 13:24:15.000000 Benchmark-4dn-0.5.8/tests/__init__.py
--rw-r--r--   0 carl       (502) staff       (20)    16292 2019-11-12 20:26:40.000000 Benchmark-4dn-0.5.8/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-30 22:25:35.000000 Benchmark-4dn-0.5.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-30 22:25:35.000000 Benchmark-4dn-0.5.9/Benchmark_4dn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-30 22:25:34.000000 Benchmark-4dn-0.5.9/Benchmark_4dn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     3805 2019-11-30 22:25:34.000000 Benchmark-4dn-0.5.9/Benchmark_4dn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      377 2019-11-30 22:25:34.000000 Benchmark-4dn-0.5.9/Benchmark_4dn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2019-11-30 22:25:34.000000 Benchmark-4dn-0.5.9/Benchmark_4dn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3805 2019-11-30 22:25:35.000000 Benchmark-4dn-0.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2318 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-30 22:25:35.000000 Benchmark-4dn-0.5.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16292 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/tests/test.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-30 22:25:35.000000 Benchmark-4dn-0.5.9/Benchmark/
+-rw-r--r--   0 root         (0) root         (0)    21262 2019-11-30 22:23:56.000000 Benchmark-4dn-0.5.9/Benchmark/bfunctions.py
+-rw-r--r--   0 root         (0) root         (0)     7035 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/Benchmark/classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-30 22:25:35.000000 Benchmark-4dn-0.5.9/Benchmark/aws/
+-rw-r--r--   0 root         (0) root         (0)   112589 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/Benchmark/aws/Amazon EC2 Instance Comparison.csv
+-rw-r--r--   0 root         (0) root         (0)      305 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/Benchmark/byteformat.py
+-rw-r--r--   0 root         (0) root         (0)      127 2019-11-30 22:24:01.000000 Benchmark-4dn-0.5.9/Benchmark/_version.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/Benchmark/run.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-11-30 22:23:19.000000 Benchmark-4dn-0.5.9/Benchmark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-11-30 22:25:35.000000 Benchmark-4dn-0.5.9/setup.cfg
```

### Comparing `Benchmark-4dn-0.5.8/Benchmark/aws/Amazon EC2 Instance Comparison.csv` & `Benchmark-4dn-0.5.9/Benchmark/aws/Amazon EC2 Instance Comparison.csv`

 * *Files identical despite different names*

### Comparing `Benchmark-4dn-0.5.8/Benchmark/bfunctions.py` & `Benchmark-4dn-0.5.9/Benchmark/bfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from Benchmark.byteformat import B2GB, B2MB, MB2GB, GB2MB
 from Benchmark.classes import BenchmarkResult
 
 
 def encode_rnaseq_stranded(input_json):
     assert 'input_size_in_bytes' in input_json
-    r = BenchmarkResult(size=150,
+    r = BenchmarkResult(size=200,
                         mem=GB2MB(64),
                         cpu=16,
                         exclude_t=True)
     return(r.as_dict())
 
 
 def encode_rnaseq_unstranded(input_json):
     assert 'input_size_in_bytes' in input_json
-    r = BenchmarkResult(size=150,
+    r = BenchmarkResult(size=200,
                         mem=GB2MB(64),
                         cpu=16,
                         exclude_t=True)
     return(r.as_dict())
 
 
 def mergebed(input_json):
```

### Comparing `Benchmark-4dn-0.5.8/Benchmark/classes.py` & `Benchmark-4dn-0.5.9/Benchmark/classes.py`

 * *Files identical despite different names*

### Comparing `Benchmark-4dn-0.5.8/Benchmark/run.py` & `Benchmark-4dn-0.5.9/Benchmark/run.py`

 * *Files identical despite different names*

### Comparing `Benchmark-4dn-0.5.8/Benchmark_4dn.egg-info/PKG-INFO` & `Benchmark-4dn-0.5.9/Benchmark_4dn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Benchmark-4dn
-Version: 0.5.8
+Version: 0.5.9
 Summary: Benchmark functions that returns total space, mem, cpu given                 input size and parameters for the CWL workflows
 Home-page: https://github.com/SooLee/Benchmark/
 Author: Soo Lee
 Author-email: duplexa@gmail.com
 License: MIT
 Description: The repo contains a benchmarking script for some of the CWL workflows used by 4DN-DCIC (https://github.com/4dn-dcic/pipelines-cwl), that returns total space, mem and CPUs required per given input size and a recommended AWS EC2 instance type.
```

### Comparing `Benchmark-4dn-0.5.8/PKG-INFO` & `Benchmark-4dn-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Benchmark-4dn
-Version: 0.5.8
+Version: 0.5.9
 Summary: Benchmark functions that returns total space, mem, cpu given                 input size and parameters for the CWL workflows
 Home-page: https://github.com/SooLee/Benchmark/
 Author: Soo Lee
 Author-email: duplexa@gmail.com
 License: MIT
 Description: The repo contains a benchmarking script for some of the CWL workflows used by 4DN-DCIC (https://github.com/4dn-dcic/pipelines-cwl), that returns total space, mem and CPUs required per given input size and a recommended AWS EC2 instance type.
```

### Comparing `Benchmark-4dn-0.5.8/README.md` & `Benchmark-4dn-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `Benchmark-4dn-0.5.8/setup.py` & `Benchmark-4dn-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `Benchmark-4dn-0.5.8/tests/test.py` & `Benchmark-4dn-0.5.9/tests/test.py`

 * *Files identical despite different names*

