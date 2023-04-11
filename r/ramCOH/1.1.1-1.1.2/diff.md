# Comparing `tmp/ramCOH-1.1.1.tar.gz` & `tmp/ramCOH-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramCOH-1.1.1.tar", last modified: Tue Apr 11 09:40:56 2023, max compression
+gzip compressed data, was "ramCOH-1.1.2.tar", last modified: Tue Apr 11 13:40:15 2023, max compression
```

## Comparing `ramCOH-1.1.1.tar` & `ramCOH-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.888039 ramCOH-1.1.1/
--rw-rw-rw-   0        0        0     1928 2022-03-17 08:07:39.000000 ramCOH-1.1.1/.gitignore
--rw-rw-rw-   0        0        0     1085 2022-03-17 08:07:39.000000 ramCOH-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       23 2023-03-06 13:35:09.000000 ramCOH-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2521 2023-04-11 09:40:56.887039 ramCOH-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      761 2023-04-11 09:28:08.000000 ramCOH-1.1.1/README.md
--rw-rw-rw-   0        0        0      799 2023-04-11 09:07:54.000000 ramCOH-1.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.737044 ramCOH-1.1.1/ramCOH/
--rw-rw-rw-   0        0        0       28 2023-03-03 16:13:03.000000 ramCOH-1.1.1/ramCOH/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.856044 ramCOH-1.1.1/ramCOH/raman/
--rw-rw-rw-   0        0        0     4801 2023-03-06 13:35:09.000000 ramCOH-1.1.1/ramCOH/raman/CO2.py
--rw-rw-rw-   0        0        0      137 2023-03-06 16:24:34.000000 ramCOH-1.1.1/ramCOH/raman/__init__.py
--rw-rw-rw-   0        0        0    22900 2023-04-07 09:46:43.000000 ramCOH-1.1.1/ramCOH/raman/baseclass.py
--rw-rw-rw-   0        0        0      762 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/raman/baseline_regions.py
--rw-rw-rw-   0        0        0    10484 2023-03-29 12:40:13.000000 ramCOH-1.1.1/ramCOH/raman/glass.py
--rw-rw-rw-   0        0        0     6173 2023-03-03 16:15:07.000000 ramCOH-1.1.1/ramCOH/raman/neon.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.869041 ramCOH-1.1.1/ramCOH/signal_processing/
--rw-rw-rw-   0        0        0        0 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/signal_processing/__init__.py
--rw-rw-rw-   0        0        0     7988 2023-03-03 16:15:28.000000 ramCOH-1.1.1/ramCOH/signal_processing/curve_fitting.py
--rw-rw-rw-   0        0        0     3644 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/signal_processing/curves.py
--rw-rw-rw-   0        0        0     7133 2023-03-03 16:15:45.000000 ramCOH-1.1.1/ramCOH/signal_processing/deconvolution.py
--rw-rw-rw-   0        0        0     8541 2023-04-06 12:27:33.000000 ramCOH-1.1.1/ramCOH/signal_processing/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.884037 ramCOH-1.1.1/ramCOH/static/
--rw-rw-rw-   0        0        0        2 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/static/__init__.py
--rw-rw-rw-   0        0        0     9547 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/static/neon_emissionLines.csv
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.778037 ramCOH-1.1.1/ramCOH.egg-info/
--rw-rw-rw-   0        0        0     2521 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 09:40:56.888039 ramCOH-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 13:40:15.653478 ramCOH-1.1.2/
+-rw-rw-rw-   0        0        0     1085 2022-03-17 08:07:39.000000 ramCOH-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       23 2023-03-06 13:35:09.000000 ramCOH-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2521 2023-04-11 13:40:15.652478 ramCOH-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2023-04-11 09:28:08.000000 ramCOH-1.1.2/README.md
+-rw-rw-rw-   0        0        0      799 2023-04-11 13:39:44.000000 ramCOH-1.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-11 13:40:15.597482 ramCOH-1.1.2/ramCOH/
+-rw-rw-rw-   0        0        0       28 2023-03-03 16:13:03.000000 ramCOH-1.1.2/ramCOH/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:40:15.636479 ramCOH-1.1.2/ramCOH/raman/
+-rw-rw-rw-   0        0        0      137 2023-03-06 16:24:34.000000 ramCOH-1.1.2/ramCOH/raman/__init__.py
+-rw-rw-rw-   0        0        0    22900 2023-04-07 09:46:43.000000 ramCOH-1.1.2/ramCOH/raman/baseclass.py
+-rw-rw-rw-   0        0        0      762 2023-03-03 13:39:43.000000 ramCOH-1.1.2/ramCOH/raman/baseline_regions.py
+-rw-rw-rw-   0        0        0     4801 2023-03-06 13:35:09.000000 ramCOH-1.1.2/ramCOH/raman/co2.py
+-rw-rw-rw-   0        0        0    10484 2023-03-29 12:40:13.000000 ramCOH-1.1.2/ramCOH/raman/glass.py
+-rw-rw-rw-   0        0        0     6173 2023-03-03 16:15:07.000000 ramCOH-1.1.2/ramCOH/raman/neon.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:40:15.646482 ramCOH-1.1.2/ramCOH/signal_processing/
+-rw-rw-rw-   0        0        0        0 2023-03-03 13:39:43.000000 ramCOH-1.1.2/ramCOH/signal_processing/__init__.py
+-rw-rw-rw-   0        0        0     7988 2023-03-03 16:15:28.000000 ramCOH-1.1.2/ramCOH/signal_processing/curve_fitting.py
+-rw-rw-rw-   0        0        0     3644 2023-03-03 13:39:43.000000 ramCOH-1.1.2/ramCOH/signal_processing/curves.py
+-rw-rw-rw-   0        0        0     7133 2023-03-03 16:15:45.000000 ramCOH-1.1.2/ramCOH/signal_processing/deconvolution.py
+-rw-rw-rw-   0        0        0     8541 2023-04-06 12:27:33.000000 ramCOH-1.1.2/ramCOH/signal_processing/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:40:15.650482 ramCOH-1.1.2/ramCOH/static/
+-rw-rw-rw-   0        0        0        2 2023-03-03 13:39:43.000000 ramCOH-1.1.2/ramCOH/static/__init__.py
+-rw-rw-rw-   0        0        0     9547 2023-03-03 13:39:43.000000 ramCOH-1.1.2/ramCOH/static/neon_emissionLines.csv
+drwxrwxrwx   0        0        0        0 2023-04-11 13:40:15.623479 ramCOH-1.1.2/ramCOH.egg-info/
+-rw-rw-rw-   0        0        0     2521 2023-04-11 13:40:15.000000 ramCOH-1.1.2/ramCOH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-04-11 13:40:15.000000 ramCOH-1.1.2/ramCOH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:40:15.000000 ramCOH-1.1.2/ramCOH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-11 13:40:15.000000 ramCOH-1.1.2/ramCOH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 13:40:15.000000 ramCOH-1.1.2/ramCOH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:40:15.653478 ramCOH-1.1.2/setup.cfg
```

### Comparing `ramCOH-1.1.1/LICENSE` & `ramCOH-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/PKG-INFO` & `ramCOH-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramCOH
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses
 Author: Thomas van Gerve
 License: MIT License
         
         Copyright (c) 2022 TDGerve
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ramCOH-1.1.1/README.md` & `ramCOH-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/pyproject.toml` & `ramCOH-1.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ramCOH"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
     {name = "Thomas van Gerve"},
 ]
 description = "Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
```

### Comparing `ramCOH-1.1.1/ramCOH/raman/CO2.py` & `ramCOH-1.1.2/ramCOH/raman/co2.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/raman/baseclass.py` & `ramCOH-1.1.2/ramCOH/raman/baseclass.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/raman/baseline_regions.py` & `ramCOH-1.1.2/ramCOH/raman/baseline_regions.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/raman/glass.py` & `ramCOH-1.1.2/ramCOH/raman/glass.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/raman/neon.py` & `ramCOH-1.1.2/ramCOH/raman/neon.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/signal_processing/curve_fitting.py` & `ramCOH-1.1.2/ramCOH/signal_processing/curve_fitting.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/signal_processing/curves.py` & `ramCOH-1.1.2/ramCOH/signal_processing/curves.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/signal_processing/deconvolution.py` & `ramCOH-1.1.2/ramCOH/signal_processing/deconvolution.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/signal_processing/functions.py` & `ramCOH-1.1.2/ramCOH/signal_processing/functions.py`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH/static/neon_emissionLines.csv` & `ramCOH-1.1.2/ramCOH/static/neon_emissionLines.csv`

 * *Files identical despite different names*

### Comparing `ramCOH-1.1.1/ramCOH.egg-info/PKG-INFO` & `ramCOH-1.1.2/ramCOH.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramCOH
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses
 Author: Thomas van Gerve
 License: MIT License
         
         Copyright (c) 2022 TDGerve
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ramCOH-1.1.1/ramCOH.egg-info/SOURCES.txt` & `ramCOH-1.1.2/ramCOH.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-.gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 ramCOH/__init__.py
 ramCOH.egg-info/PKG-INFO
 ramCOH.egg-info/SOURCES.txt
 ramCOH.egg-info/dependency_links.txt
 ramCOH.egg-info/requires.txt
 ramCOH.egg-info/top_level.txt
-ramCOH/raman/CO2.py
 ramCOH/raman/__init__.py
 ramCOH/raman/baseclass.py
 ramCOH/raman/baseline_regions.py
 ramCOH/raman/co2.py
 ramCOH/raman/glass.py
 ramCOH/raman/neon.py
 ramCOH/signal_processing/__init__.py
```

