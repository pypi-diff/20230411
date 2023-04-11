# Comparing `tmp/biobb_flexserv-3.9.1.tar.gz` & `tmp/biobb_flexserv-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_flexserv-3.9.1.tar", last modified: Wed Mar 29 10:11:01 2023, max compression
+gzip compressed data, was "dist/biobb_flexserv-4.0.0.tar", last modified: Tue Apr 11 15:02:18 2023, max compression
```

## Comparing `biobb_flexserv-3.9.1.tar` & `biobb_flexserv-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)    11357 2022-10-26 12:37:34.000000 biobb_flexserv-3.9.1/LICENSE
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     1018 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/PKG-INFO
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     3844 2023-03-29 10:05:54.000000 biobb_flexserv-3.9.1/README.md
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       79 2023-03-29 10:06:03.000000 biobb_flexserv-3.9.1/biobb_flexserv/__init__.py
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv/flexserv/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       61 2022-10-26 12:59:17.000000 biobb_flexserv-3.9.1/biobb_flexserv/flexserv/__init__.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7225 2023-03-29 08:21:04.000000 biobb_flexserv-3.9.1/biobb_flexserv/flexserv/bd_run.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7731 2023-03-29 08:21:27.000000 biobb_flexserv-3.9.1/biobb_flexserv/flexserv/dmd_run.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7304 2023-03-29 08:21:53.000000 biobb_flexserv-3.9.1/biobb_flexserv/flexserv/nma_run.py
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)      193 2023-03-29 08:49:32.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/__init__.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     6161 2023-03-29 08:26:47.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_animate.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7558 2023-01-20 08:16:15.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_bfactor.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     6870 2023-03-29 08:27:45.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_collectivity.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7235 2023-03-29 08:28:04.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_evecs.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)    11403 2023-01-26 08:55:48.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_hinges.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7907 2023-03-29 08:28:34.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_info.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     6805 2023-03-29 08:28:48.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_lindemann.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)    16439 2023-03-29 08:29:37.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_similarity.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7511 2023-03-29 08:29:54.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_stiffness.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     6157 2023-03-29 08:51:55.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_unzip.py
--rwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     7450 2023-03-29 08:44:27.000000 biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_zip.py
-drwxr-xr-x   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        0 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv.egg-info/
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     1018 2023-03-29 10:11:00.000000 biobb_flexserv-3.9.1/biobb_flexserv.egg-info/PKG-INFO
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)      888 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv.egg-info/SOURCES.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)        1 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv.egg-info/dependency_links.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)      762 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv.egg-info/entry_points.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       20 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv.egg-info/requires.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       15 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/biobb_flexserv.egg-info/top_level.txt
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)       38 2023-03-29 10:11:01.000000 biobb_flexserv-3.9.1/setup.cfg
--rw-r--r--   0 hospital (800236490) IRBBARCELONA\Domain Users (1791188573)     2331 2023-03-29 10:05:59.000000 biobb_flexserv-3.9.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      982 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5872 2023-04-11 15:01:07.000000 biobb_flexserv-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2023-04-11 15:00:50.000000 biobb_flexserv-4.0.0/biobb_flexserv/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       61 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7225 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/bd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7731 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/dmd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7304 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/nma_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      193 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6161 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_animate.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7558 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_bfactor.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6870 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_collectivity.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7235 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_evecs.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11403 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_hinges.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7907 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_info.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6805 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_lindemann.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16439 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_similarity.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7511 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_stiffness.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6157 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_unzip.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7450 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_zip.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      982 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      888 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      762 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       15 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2331 2023-04-11 14:59:22.000000 biobb_flexserv-4.0.0/setup.py
```

### Comparing `biobb_flexserv-3.9.1/LICENSE` & `biobb_flexserv-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/PKG-INFO` & `biobb_flexserv-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: biobb_flexserv
-Version: 3.9.1
+Version: 4.0.0
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-License: UNKNOWN
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 biobb_flexserv allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.
-
```

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/flexserv/bd_run.py` & `biobb_flexserv-4.0.0/biobb_flexserv/flexserv/bd_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/flexserv/dmd_run.py` & `biobb_flexserv-4.0.0/biobb_flexserv/flexserv/dmd_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/flexserv/nma_run.py` & `biobb_flexserv-4.0.0/biobb_flexserv/flexserv/nma_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_animate.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_animate.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_bfactor.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_bfactor.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_collectivity.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_collectivity.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_evecs.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_evecs.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_hinges.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_hinges.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_info.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_info.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_lindemann.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_lindemann.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_similarity.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_similarity.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_stiffness.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_stiffness.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_unzip.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_unzip.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv/pcasuite/pcz_zip.py` & `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_zip.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv.egg-info/PKG-INFO` & `biobb_flexserv-4.0.0/biobb_flexserv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: biobb-flexserv
-Version: 3.9.1
+Version: 4.0.0
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-License: UNKNOWN
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 biobb_flexserv allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.
-
```

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv.egg-info/SOURCES.txt` & `biobb_flexserv-4.0.0/biobb_flexserv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/biobb_flexserv.egg-info/entry_points.txt` & `biobb_flexserv-4.0.0/biobb_flexserv.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-3.9.1/setup.py` & `biobb_flexserv-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexserv",
-    version="3.9.1",
+    version="4.0.0",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.",
     long_description="biobb_flexserv allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexserv",
     project_urls={
         "Documentation": "http://biobb_flexserv.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     include_package_data=True,
-    install_requires=['biobb_common==3.9.0'],
+    install_requires=['biobb_common==4.0.0'],
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "bd_run = biobb_flexserv.flexserv.bd_run:main",
             "dmd_run = biobb_flexserv.flexserv.dmd_run:main",
             "nma_run = biobb_flexserv.flexserv.nma_run:main",
             "pcz_zip = biobb_flexserv.pcasuite.pcz_zip:main",
```

