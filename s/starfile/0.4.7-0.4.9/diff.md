# Comparing `tmp/starfile-0.4.7.tar.gz` & `tmp/starfile-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfile-0.4.7.tar", last modified: Tue Sep 14 10:48:21 2021, max compression
+gzip compressed data, was "starfile-0.4.9.tar", last modified: Fri Oct  8 13:39:50 2021, max compression
```

## Comparing `starfile-0.4.7.tar` & `starfile-0.4.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.278295 starfile-0.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.274295 starfile-0.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.274295 starfile-0.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-09-14 10:48:12.000000 starfile-0.4.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      408 2021-09-14 10:48:12.000000 starfile-0.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-09-14 10:48:12.000000 starfile-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5685 2021-09-14 10:48:21.278295 starfile-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4996 2021-09-14 10:48:12.000000 starfile-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-09-14 10:48:12.000000 starfile-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-09-14 10:48:12.000000 starfile-0.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      972 2021-09-14 10:48:21.278295 starfile-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-09-14 10:48:12.000000 starfile-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.278295 starfile-0.4.7/starfile/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-09-14 10:48:12.000000 starfile-0.4.7/starfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2021-09-14 10:48:12.000000 starfile-0.4.7/starfile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-09-14 10:48:12.000000 starfile-0.4.7/starfile/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6204 2021-09-14 10:48:12.000000 starfile-0.4.7/starfile/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2021-09-14 10:48:12.000000 starfile-0.4.7/starfile/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5004 2021-09-14 10:48:12.000000 starfile-0.4.7/starfile/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.278295 starfile-0.4.7/starfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5685 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-14 10:48:21.000000 starfile-0.4.7/starfile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.278295 starfile-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.278295 starfile-0.4.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)    12768 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/default_pipeline.star
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/one_loop.star
--rw-r--r--   0 runner    (1001) docker     (121)     7418 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/postprocess.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 10:48:21.278295 starfile-0.4.7/tests/data/relion_tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)     6125 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/relion_tutorial/run_it025_optimiser_2D.star
--rw-r--r--   0 runner    (1001) docker     (121)     6251 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/relion_tutorial/run_it025_optimiser_3D.star
--rw-r--r--   0 runner    (1001) docker     (121)      691 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/relion_tutorial/run_it025_sampling_2D.star
--rw-r--r--   0 runner    (1001) docker     (121)     6115 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/relion_tutorial/run_it025_sampling_3D.star
--rw-r--r--   0 runner    (1001) docker     (121)      935 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/rln3.1_data_style.star
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/single_line_end_of_multiblock.star
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/single_line_middle_of_multiblock.star
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/two_basic_blocks.star
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/data/two_single_line_loop_blocks.star
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/test_functional_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     5911 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/test_read_write_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/test_writing.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2021-09-14 10:48:12.000000 starfile-0.4.7/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.228899 starfile-0.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.224899 starfile-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.228899 starfile-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-10-08 13:39:38.000000 starfile-0.4.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2021-10-08 13:39:38.000000 starfile-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-10-08 13:39:38.000000 starfile-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5685 2021-10-08 13:39:50.228899 starfile-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4996 2021-10-08 13:39:38.000000 starfile-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-10-08 13:39:38.000000 starfile-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2021-10-08 13:39:38.000000 starfile-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2021-10-08 13:39:50.232899 starfile-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2021-10-08 13:39:38.000000 starfile-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.228899 starfile-0.4.9/starfile/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-08 13:39:38.000000 starfile-0.4.9/starfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2021-10-08 13:39:38.000000 starfile-0.4.9/starfile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-10-08 13:39:38.000000 starfile-0.4.9/starfile/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6204 2021-10-08 13:39:38.000000 starfile-0.4.9/starfile/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2021-10-08 13:39:38.000000 starfile-0.4.9/starfile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-10-08 13:39:38.000000 starfile-0.4.9/starfile/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.228899 starfile-0.4.9/starfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5685 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-10-08 13:39:50.000000 starfile-0.4.9/starfile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.228899 starfile-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1580 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.228899 starfile-0.4.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    12768 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/default_pipeline.star
+-rw-r--r--   0 runner    (1001) docker     (121)     4888 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/one_loop.star
+-rw-r--r--   0 runner    (1001) docker     (121)     7418 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/postprocess.star
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 13:39:50.228899 starfile-0.4.9/tests/data/relion_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)     6125 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/relion_tutorial/run_it025_optimiser_2D.star
+-rw-r--r--   0 runner    (1001) docker     (121)     6251 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/relion_tutorial/run_it025_optimiser_3D.star
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/relion_tutorial/run_it025_sampling_2D.star
+-rw-r--r--   0 runner    (1001) docker     (121)     6115 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/relion_tutorial/run_it025_sampling_3D.star
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/rln3.1_data_style.star
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/single_line_end_of_multiblock.star
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/single_line_middle_of_multiblock.star
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/two_basic_blocks.star
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/data/two_single_line_loop_blocks.star
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/test_functional_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5911 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/test_read_write_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/test_writing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2021-10-08 13:39:38.000000 starfile-0.4.9/tests/utils.py
```

### Comparing `starfile-0.4.7/.github/workflows/test_and_deploy.yml` & `starfile-0.4.9/.github/workflows/test_and_deploy.yml`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools pytest
           pip install -e .
-      # this runs the platform-specific tests declared in tox.ini
+
       - name: Test with pytest
         run: pytest
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
         uses: codecov/codecov-action@v1
```

### Comparing `starfile-0.4.7/LICENSE` & `starfile-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/PKG-INFO` & `starfile-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfile
-Version: 0.4.7
+Version: 0.4.9
 Summary: STAR file reading and writing in python.
 Home-page: https://github.com/alisterburt/starfile
 Author: Alister Burt
 Author-email: alisterburt@gmail.com
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `starfile-0.4.7/README.md` & `starfile-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/setup.cfg` & `starfile-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/starfile/__main__.py` & `starfile-0.4.9/starfile/__main__.py`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/starfile/functions.py` & `starfile-0.4.9/starfile/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     else:
         return star.dataframes
 
 
 def write(data: Union[pd.DataFrame, Dict[str, pd.DataFrame], List[pd.DataFrame]],
           filename: PathLike,
           float_format: str = '%.6f', sep: str = '\t', na_rep: str = '<NA>',
-          overwrite: bool = False):
+          overwrite: bool = False, force_loop: bool = False):
     """
     Write dataframes from pandas dataframe(s) to a star file
 
     data can be a single dataframe, a list of dataframes or a dict of dataframes
     float format defaults to 6 digits after the decimal point
     """
-    StarWriter(data, filename=filename, float_format=float_format, overwrite=overwrite)
+    StarWriter(data, filename=filename, float_format=float_format, overwrite=overwrite,
+               na_rep=na_rep, sep=sep, force_loop=force_loop)
```

### Comparing `starfile-0.4.7/starfile/parser.py` & `starfile-0.4.9/starfile/parser.py`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/starfile/utils.py` & `starfile-0.4.9/starfile/utils.py`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/starfile/writer.py` & `starfile-0.4.9/starfile/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 
 __version__ = get_distribution("starfile").version
 
 
 class StarWriter:
     def __init__(self, dataframes: Union[pd.DataFrame, Dict[pd.DataFrame], List[pd.DataFrame]],
                  filename: PathLike, overwrite: bool = False, float_format: str = '%.6f',
-                 sep: str = '\t', na_rep: str = '<NA>'):
+                 sep: str = '\t', na_rep: str = '<NA>', force_loop: bool = False):
         self.overwrite = overwrite
         self.filename = filename
         self.dataframes = dataframes
         self.float_format = float_format
         self.sep = sep
         self.na_rep = na_rep
+        self.force_loop = force_loop
         self.buffer = TextBuffer()
         self.write_star_file()
 
     @property
     def dataframes(self):
         """
         Ordered dictionary of pandas dataframes
@@ -126,17 +127,17 @@
         self.buffer.add_line(self.get_block_name(df))
         self.buffer.add_blank_lines(1)
         self.buffer.append_to_file_and_clear(self.filename)
 
     def write_block(self, df: pd.DataFrame):
         self.add_block_name_to_buffer(df)
 
-        if df.shape[0] == 1:
+        if (df.shape[0] == 1) and not self.force_loop:
             self._write_simple_block(df)
-        elif df.shape[0] > 1:
+        elif (df.shape[0] > 1) or self.force_loop:
             self._write_loop_block(df)
         self.buffer.add_blank_lines(2)
         self.buffer.append_to_file_and_clear(self.filename)
 
     def _write_simple_block(self, df: pd.DataFrame):
         lines = [f'_{column_name}\t\t\t{df[column_name].iloc[0]}'
                  for column_name in df.columns]
```

### Comparing `starfile-0.4.7/starfile.egg-info/PKG-INFO` & `starfile-0.4.9/starfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfile
-Version: 0.4.7
+Version: 0.4.9
 Summary: STAR file reading and writing in python.
 Home-page: https://github.com/alisterburt/starfile
 Author: Alister Burt
 Author-email: alisterburt@gmail.com
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `starfile-0.4.7/starfile.egg-info/SOURCES.txt` & `starfile-0.4.9/starfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/constants.py` & `starfile-0.4.9/tests/constants.py`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/default_pipeline.star` & `starfile-0.4.9/tests/data/default_pipeline.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/one_loop.star` & `starfile-0.4.9/tests/data/one_loop.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/postprocess.star` & `starfile-0.4.9/tests/data/postprocess.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/relion_tutorial/run_it025_optimiser_2D.star` & `starfile-0.4.9/tests/data/relion_tutorial/run_it025_optimiser_2D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/relion_tutorial/run_it025_optimiser_3D.star` & `starfile-0.4.9/tests/data/relion_tutorial/run_it025_optimiser_3D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/relion_tutorial/run_it025_sampling_2D.star` & `starfile-0.4.9/tests/data/relion_tutorial/run_it025_sampling_2D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/relion_tutorial/run_it025_sampling_3D.star` & `starfile-0.4.9/tests/data/relion_tutorial/run_it025_sampling_3D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/rln3.1_data_style.star` & `starfile-0.4.9/tests/data/rln3.1_data_style.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/data/single_line_end_of_multiblock.star` & `starfile-0.4.9/tests/data/single_line_end_of_multiblock.star`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/test_functional_interface.py` & `starfile-0.4.9/tests/test_functional_interface.py`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/test_parsing.py` & `starfile-0.4.9/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/test_read_write_round_trip.py` & `starfile-0.4.9/tests/test_read_write_round_trip.py`

 * *Files identical despite different names*

### Comparing `starfile-0.4.7/tests/test_writing.py` & `starfile-0.4.9/tests/test_writing.py`

 * *Files identical despite different names*

