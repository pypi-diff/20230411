# Comparing `tmp/ieegprep-1.0.0.tar.gz` & `tmp/ieegprep-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieegprep-1.0.0.tar", last modified: Fri Apr  7 22:43:53 2023, max compression
+gzip compressed data, was "ieegprep-1.1.0.tar", last modified: Tue Apr 11 16:44:56 2023, max compression
```

## Comparing `ieegprep-1.0.0.tar` & `ieegprep-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-07 22:43:53.508284 ieegprep-1.0.0/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35149 2023-02-15 23:27:00.000000 ieegprep-1.0.0/LICENSE
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1860 2023-04-07 22:43:53.508422 ieegprep-1.0.0/PKG-INFO
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      666 2023-04-07 22:00:01.000000 ieegprep-1.0.0/README.md
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-07 22:43:53.492478 ieegprep-1.0.0/ieegprep/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      277 2023-04-07 21:59:18.000000 ieegprep-1.0.0/ieegprep/__init__.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-07 22:43:53.499117 ieegprep-1.0.0/ieegprep/bids/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      266 2023-04-06 20:04:42.000000 ieegprep-1.0.0/ieegprep/bids/__init__.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    11121 2023-02-15 23:39:47.000000 ieegprep-1.0.0/ieegprep/bids/data_epoch.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    19133 2023-04-07 21:42:05.000000 ieegprep-1.0.0/ieegprep/bids/data_structure.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     9997 2023-02-15 23:39:13.000000 ieegprep-1.0.0/ieegprep/bids/rereferencing.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4809 2023-02-15 23:38:50.000000 ieegprep-1.0.0/ieegprep/bids/sidecars.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-07 22:43:53.503166 ieegprep-1.0.0/ieegprep/fileio/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    55051 2023-02-15 23:26:11.000000 ieegprep-1.0.0/ieegprep/fileio/BrainVisionReader.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46835 2023-02-15 23:26:19.000000 ieegprep-1.0.0/ieegprep/fileio/EdfReader.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    12613 2023-02-15 23:26:38.000000 ieegprep-1.0.0/ieegprep/fileio/IeegDataReader.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     9918 2023-02-15 23:26:28.000000 ieegprep-1.0.0/ieegprep/fileio/Mef3Reader.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      116 2023-02-15 23:37:39.000000 ieegprep-1.0.0/ieegprep/fileio/__init__.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-07 22:43:53.504749 ieegprep-1.0.0/ieegprep/utils/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     6124 2023-04-07 20:46:59.000000 ieegprep-1.0.0/ieegprep/utils/console.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7710 2023-04-06 22:10:19.000000 ieegprep-1.0.0/ieegprep/utils/misc.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-04-07 21:55:48.000000 ieegprep-1.0.0/ieegprep/version.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-07 22:43:53.495626 ieegprep-1.0.0/ieegprep.egg-info/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1860 2023-04-07 22:43:53.000000 ieegprep-1.0.0/ieegprep.egg-info/PKG-INFO
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      710 2023-04-07 22:43:53.000000 ieegprep-1.0.0/ieegprep.egg-info/SOURCES.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-04-07 22:43:53.000000 ieegprep-1.0.0/ieegprep.egg-info/dependency_links.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       55 2023-04-07 22:43:53.000000 ieegprep-1.0.0/ieegprep.egg-info/requires.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-04-07 22:43:53.000000 ieegprep-1.0.0/ieegprep.egg-info/top_level.txt
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1448 2023-04-07 22:38:36.000000 ieegprep-1.0.0/pyproject.toml
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      161 2023-04-07 22:43:53.511001 ieegprep-1.0.0/setup.cfg
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-07 22:43:53.507741 ieegprep-1.0.0/tests/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    15723 2023-02-15 23:32:38.000000 ieegprep-1.0.0/tests/test_fileio_bv_data.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    11480 2023-02-15 23:32:41.000000 ieegprep-1.0.0/tests/test_fileio_bv_perf.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    14659 2023-02-15 23:32:56.000000 ieegprep-1.0.0/tests/test_fileio_edf_data.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    10758 2023-02-15 23:32:59.000000 ieegprep-1.0.0/tests/test_fileio_edf_perf.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 16:44:56.245226 ieegprep-1.1.0/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35149 2023-02-15 23:27:00.000000 ieegprep-1.1.0/LICENSE
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     5833 2023-04-11 16:44:56.245379 ieegprep-1.1.0/PKG-INFO
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4639 2023-04-11 00:26:26.000000 ieegprep-1.1.0/README.md
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 16:44:56.221546 ieegprep-1.1.0/ieegprep/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      573 2023-04-11 16:15:59.000000 ieegprep-1.1.0/ieegprep/__init__.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 16:44:56.231248 ieegprep-1.1.0/ieegprep/bids/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      266 2023-04-06 20:04:42.000000 ieegprep-1.1.0/ieegprep/bids/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)   108220 2023-04-11 16:44:10.000000 ieegprep-1.1.0/ieegprep/bids/data_epoch.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    19133 2023-04-07 21:42:05.000000 ieegprep-1.1.0/ieegprep/bids/data_structure.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     9997 2023-02-15 23:39:13.000000 ieegprep-1.1.0/ieegprep/bids/rereferencing.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4809 2023-02-15 23:38:50.000000 ieegprep-1.1.0/ieegprep/bids/sidecars.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 16:44:56.237280 ieegprep-1.1.0/ieegprep/fileio/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    55051 2023-02-15 23:26:11.000000 ieegprep-1.1.0/ieegprep/fileio/BrainVisionReader.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46835 2023-02-15 23:26:19.000000 ieegprep-1.1.0/ieegprep/fileio/EdfReader.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    12613 2023-02-15 23:26:38.000000 ieegprep-1.1.0/ieegprep/fileio/IeegDataReader.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     9918 2023-02-15 23:26:28.000000 ieegprep-1.1.0/ieegprep/fileio/Mef3Reader.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      116 2023-02-15 23:37:39.000000 ieegprep-1.1.0/ieegprep/fileio/__init__.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 16:44:56.239364 ieegprep-1.1.0/ieegprep/utils/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     6124 2023-04-07 20:46:59.000000 ieegprep-1.1.0/ieegprep/utils/console.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7710 2023-04-06 22:10:19.000000 ieegprep-1.1.0/ieegprep/utils/misc.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-04-11 16:12:38.000000 ieegprep-1.1.0/ieegprep/version.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 16:44:56.226312 ieegprep-1.1.0/ieegprep.egg-info/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     5833 2023-04-11 16:44:56.000000 ieegprep-1.1.0/ieegprep.egg-info/PKG-INFO
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      750 2023-04-11 16:44:56.000000 ieegprep-1.1.0/ieegprep.egg-info/SOURCES.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-04-11 16:44:56.000000 ieegprep-1.1.0/ieegprep.egg-info/dependency_links.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       68 2023-04-11 16:44:56.000000 ieegprep-1.1.0/ieegprep.egg-info/requires.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-04-11 16:44:56.000000 ieegprep-1.1.0/ieegprep.egg-info/top_level.txt
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1470 2023-04-10 20:34:54.000000 ieegprep-1.1.0/pyproject.toml
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      177 2023-04-11 16:44:56.248271 ieegprep-1.1.0/setup.cfg
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 16:44:56.244599 ieegprep-1.1.0/tests/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1729 2023-04-10 22:59:47.000000 ieegprep-1.1.0/tests/test_epoch_by_channels_bv_perf.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    15723 2023-02-15 23:32:38.000000 ieegprep-1.1.0/tests/test_fileio_bv_data.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    11480 2023-02-15 23:32:41.000000 ieegprep-1.1.0/tests/test_fileio_bv_perf.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    14659 2023-02-15 23:32:56.000000 ieegprep-1.1.0/tests/test_fileio_edf_data.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    10758 2023-02-15 23:32:59.000000 ieegprep-1.1.0/tests/test_fileio_edf_perf.py
```

### Comparing `ieegprep-1.0.0/LICENSE` & `ieegprep-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/bids/data_structure.py` & `ieegprep-1.1.0/ieegprep/bids/data_structure.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/bids/rereferencing.py` & `ieegprep-1.1.0/ieegprep/bids/rereferencing.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/bids/sidecars.py` & `ieegprep-1.1.0/ieegprep/bids/sidecars.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/fileio/BrainVisionReader.py` & `ieegprep-1.1.0/ieegprep/fileio/BrainVisionReader.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/fileio/EdfReader.py` & `ieegprep-1.1.0/ieegprep/fileio/EdfReader.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/fileio/IeegDataReader.py` & `ieegprep-1.1.0/ieegprep/fileio/IeegDataReader.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/fileio/Mef3Reader.py` & `ieegprep-1.1.0/ieegprep/fileio/Mef3Reader.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/utils/console.py` & `ieegprep-1.1.0/ieegprep/utils/console.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep/utils/misc.py` & `ieegprep-1.1.0/ieegprep/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/ieegprep.egg-info/SOURCES.txt` & `ieegprep-1.1.0/ieegprep.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 ieegprep/fileio/BrainVisionReader.py
 ieegprep/fileio/EdfReader.py
 ieegprep/fileio/IeegDataReader.py
 ieegprep/fileio/Mef3Reader.py
 ieegprep/fileio/__init__.py
 ieegprep/utils/console.py
 ieegprep/utils/misc.py
+tests/test_epoch_by_channels_bv_perf.py
 tests/test_fileio_bv_data.py
 tests/test_fileio_bv_perf.py
 tests/test_fileio_edf_data.py
 tests/test_fileio_edf_perf.py
```

### Comparing `ieegprep-1.0.0/pyproject.toml` & `ieegprep-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 name = "ieegprep"
 description = "A package to read and pre-process Intracranial Electroencephalography (iEEG) data that is structured according to the Brain Imaging Data Structure (BIDS)"
 readme = "README.md"
 license = { text="GPLv3" }
 requires-python = ">=3.8"
 dependencies = [
     "numpy >= 1.22.3",
+    "scipy >= 1.8.0",
     "pandas >= 1.4.2",
     "pymef >= 1.3.4",
     "psutil >= 5.9.4",
 ]
 keywords = ["intracranial", "electroencephalography", "ieeg", "BIDS"]
 authors = [{ name="Max van den Boom", email="m.a.vandenboom84@gmail.com" }]
 classifiers = [
```

### Comparing `ieegprep-1.0.0/tests/test_fileio_bv_data.py` & `ieegprep-1.1.0/tests/test_fileio_bv_data.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/tests/test_fileio_bv_perf.py` & `ieegprep-1.1.0/tests/test_fileio_bv_perf.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/tests/test_fileio_edf_data.py` & `ieegprep-1.1.0/tests/test_fileio_edf_data.py`

 * *Files identical despite different names*

### Comparing `ieegprep-1.0.0/tests/test_fileio_edf_perf.py` & `ieegprep-1.1.0/tests/test_fileio_edf_perf.py`

 * *Files identical despite different names*

