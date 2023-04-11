# Comparing `tmp/f4-0.4.2.tar.gz` & `tmp/f4-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.4.2.tar", last modified: Mon Apr 10 19:25:21 2023, max compression
+gzip compressed data, was "f4-0.4.3.tar", last modified: Tue Apr 11 19:01:26 2023, max compression
```

## Comparing `f4-0.4.2.tar` & `f4-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-10 19:25:21.084073 f4-0.4.2/
--rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.4.2/LICENSE
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-10 19:25:21.084189 f4-0.4.2/PKG-INFO
--rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.4.2/README.md
--rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.4.2/pyproject.toml
--rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-10 19:25:21.084721 f4-0.4.2/setup.cfg
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-10 19:25:21.075219 f4-0.4.2/src/
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-10 19:25:21.080574 f4-0.4.2/src/f4/
--rwxr-xr-x   0 srp33      (501) staff       (20)    38076 2023-04-10 19:23:30.000000 f4-0.4.2/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (501) staff       (20)    49304 2023-04-03 18:58:04.000000 f4-0.4.2/src/f4/Parser.py
--rwxr-xr-x   0 srp33      (501) staff       (20)     8733 2023-04-04 23:15:09.000000 f4-0.4.2/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (501) staff       (20)      403 2023-03-31 04:56:48.000000 f4-0.4.2/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-10 19:25:21.082456 f4-0.4.2/src/f4.egg-info/
--rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-10 19:25:21.000000 f4-0.4.2/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-10 19:25:21.000000 f4-0.4.2/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-10 19:25:21.000000 f4-0.4.2/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-10 19:25:21.000000 f4-0.4.2/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-10 19:25:21.000000 f4-0.4.2/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-10 19:25:21.082763 f4-0.4.2/test/
--rwxr-xr-x   0 srp33      (501) staff       (20)    52523 2023-04-05 20:39:16.000000 f4-0.4.2/test/test.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.277722 f4-0.4.3/
+-rw-r--r--   0 srp33      (501) staff       (20)    11357 2023-02-09 00:36:34.000000 f4-0.4.3/LICENSE
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-11 19:01:26.277842 f4-0.4.3/PKG-INFO
+-rwxr-xr-x   0 srp33      (501) staff       (20)       67 2023-02-19 23:03:17.000000 f4-0.4.3/README.md
+-rw-r--r--   0 srp33      (501) staff       (20)      104 2023-02-09 00:40:41.000000 f4-0.4.3/pyproject.toml
+-rw-r--r--   0 srp33      (501) staff       (20)      733 2023-04-11 19:01:26.278326 f4-0.4.3/setup.cfg
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.272199 f4-0.4.3/src/
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.275648 f4-0.4.3/src/f4/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    38192 2023-04-11 18:58:51.000000 f4-0.4.3/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)    49304 2023-04-03 18:58:04.000000 f4-0.4.3/src/f4/Parser.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)     8733 2023-04-04 23:15:09.000000 f4-0.4.3/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (501) staff       (20)      403 2023-03-31 04:56:48.000000 f4-0.4.3/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.277165 f4-0.4.3/src/f4.egg-info/
+-rw-r--r--   0 srp33      (501) staff       (20)      584 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (501) staff       (20)      278 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        1 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (501) staff       (20)       67 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (501) staff       (20)        3 2023-04-11 19:01:26.000000 f4-0.4.3/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (501) staff       (20)        0 2023-04-11 19:01:26.277438 f4-0.4.3/test/
+-rwxr-xr-x   0 srp33      (501) staff       (20)    52520 2023-04-11 18:59:29.000000 f4-0.4.3/test/test.py
```

### Comparing `f4-0.4.2/LICENSE` & `f4-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.4.2/PKG-INFO` & `f4-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.4.2/setup.cfg` & `f4-0.4.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.4.2
+version = 0.4.3
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.4.2/src/f4/Builder.py` & `f4-0.4.3/src/f4/Builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,20 @@
                 compression_type = "zstd"
 
             print_message(f"Converting temp file at {tmp_tsv_file_path} to {f4_dest_file_path}", verbose)
             convert_delimited_file(tmp_tsv_file_path, f4_dest_file_path, compression_type=compression_type, num_parallel=num_parallel, verbose=verbose)
 
             remove(tmp_tsv_file_path)
 
-def build_indexes(f4_file_path, index_columns, tmp_dir_path, verbose=False):
+def build_indexes(f4_file_path, index_columns, tmp_dir_path=None, verbose=False):
+    if tmp_dir_path:
+        makedirs(tmp_dir_path, exist_ok=True)
+    else:
+        tmp_dir_path = mkdtemp()
+
     if isinstance(index_columns, str):
         build_one_column_index(f4_file_path, index_columns, tmp_dir_path, verbose)
     elif isinstance(index_columns, list):
         for index_column in index_columns:
             if isinstance(index_column, list):
                 if len(index_column) != 2:
                     raise Exception("If you pass a list as an index_column, it must have exactly two elements.")
```

### Comparing `f4-0.4.2/src/f4/Parser.py` & `f4-0.4.3/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.4.2/src/f4/Utilities.py` & `f4-0.4.3/src/f4/Utilities.py`

 * *Files identical despite different names*

### Comparing `f4-0.4.2/src/f4.egg-info/PKG-INFO` & `f4-0.4.3/src/f4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.4.2/test/test.py` & `f4-0.4.3/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,24 +837,24 @@
     # Inner join with compression
     test_inner_join(num_parallel = 1, compression_type = "zstd")
 
     # Clean up data files
     for file_path in glob.glob(f"{f4_file_path}*"):
         os.unlink(file_path)
 
-#run_all_small_tests()
+run_all_small_tests()
 
 #for compression_type in [None, "dictionary", "zstd"]:
-#for compression_type in [None, "zstd"]:
-for compression_type in [None]:
+for compression_type in [None, "zstd"]:
+#for compression_type in [None]:
 #for compression_type in ["dictionary"]:
 #for compression_type in ["zstd"]:
     # Medium tests
-    #run_larger_tests(num_parallel=1, size="medium", discrete1_index=11, numeric1_index=21, rebuild=True, compression_type=compression_type)
-    #run_larger_tests(num_parallel=2, size="medium", discrete1_index=11, numeric1_index=21, rebuild=True, compression_type=compression_type)
+    run_larger_tests(num_parallel=1, size="medium", discrete1_index=11, numeric1_index=21, rebuild=True, compression_type=compression_type)
+    run_larger_tests(num_parallel=2, size="medium", discrete1_index=11, numeric1_index=21, rebuild=True, compression_type=compression_type)
 
     # Large tests
     #num_parallel = 1
     num_parallel = 4
     #num_parallel = 16
     rebuild = True
     #rebuild = False
```

