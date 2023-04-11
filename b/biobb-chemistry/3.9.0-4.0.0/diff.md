# Comparing `tmp/biobb_chemistry-3.9.0.tar.gz` & `tmp/biobb_chemistry-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_chemistry-3.9.0.tar", last modified: Tue Dec 27 10:34:19 2022, max compression
+gzip compressed data, was "dist/biobb_chemistry-4.0.0.tar", last modified: Tue Apr 11 11:51:34 2023, max compression
```

## Comparing `biobb_chemistry-3.9.0.tar` & `biobb_chemistry-4.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:32:59.000000 biobb_chemistry-3.9.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4170 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3356 2022-12-27 10:30:59.000000 biobb_chemistry-3.9.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       91 2022-12-27 10:30:38.000000 biobb_chemistry-3.9.0/biobb_chemistry/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry/acpype/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      114 2022-05-26 11:32:59.000000 biobb_chemistry-3.9.0/biobb_chemistry/acpype/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11573 2022-12-27 09:42:51.000000 biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_ac.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10483 2022-12-27 09:46:18.000000 biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_cns.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10499 2022-12-27 09:49:48.000000 biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_gmx.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9797 2022-12-27 09:49:07.000000 biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5418 2022-09-19 11:23:08.000000 biobb_chemistry-3.9.0/biobb_chemistry/acpype/common.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry/ambertools/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       81 2022-05-26 11:32:59.000000 biobb_chemistry-3.9.0/biobb_chemistry/ambertools/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     1842 2022-09-19 11:30:27.000000 biobb_chemistry-3.9.0/biobb_chemistry/ambertools/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11046 2022-12-27 10:17:07.000000 biobb_chemistry-3.9.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6988 2022-12-27 10:17:20.000000 biobb_chemistry-3.9.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry/babelm/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      110 2022-05-26 11:32:59.000000 biobb_chemistry-3.9.0/biobb_chemistry/babelm/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12001 2022-12-27 10:17:31.000000 biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_add_hydrogens.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12030 2022-12-27 10:17:38.000000 biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_convert.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9735 2022-12-27 10:17:47.000000 biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_minimize.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12049 2022-12-27 10:17:52.000000 biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_remove_hydrogens.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7325 2022-09-19 11:42:11.000000 biobb_chemistry-3.9.0/biobb_chemistry/babelm/common.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:32:59.000000 biobb_chemistry-3.9.0/biobb_chemistry/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4170 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      996 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      712 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       16 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/biobb_chemistry.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2022-12-27 10:34:19.000000 biobb_chemistry-3.9.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2037 2022-12-27 10:30:27.000000 biobb_chemistry-3.9.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:32:59.000000 biobb_chemistry-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6236 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5422 2023-04-11 11:48:48.000000 biobb_chemistry-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       91 2023-04-11 11:48:09.000000 biobb_chemistry-4.0.0/biobb_chemistry/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry/acpype/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      114 2022-05-26 11:32:59.000000 biobb_chemistry-4.0.0/biobb_chemistry/acpype/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11573 2022-12-27 09:42:51.000000 biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_ac.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10483 2022-12-27 09:46:18.000000 biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_cns.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10499 2022-12-27 09:49:48.000000 biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_gmx.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9797 2022-12-27 09:49:07.000000 biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5418 2022-09-19 11:23:08.000000 biobb_chemistry-4.0.0/biobb_chemistry/acpype/common.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry/ambertools/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       81 2022-05-26 11:32:59.000000 biobb_chemistry-4.0.0/biobb_chemistry/ambertools/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1842 2022-09-19 11:30:27.000000 biobb_chemistry-4.0.0/biobb_chemistry/ambertools/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11046 2022-12-27 10:17:07.000000 biobb_chemistry-4.0.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6988 2022-12-27 10:17:20.000000 biobb_chemistry-4.0.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry/babelm/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      110 2022-05-26 11:32:59.000000 biobb_chemistry-4.0.0/biobb_chemistry/babelm/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12001 2022-12-27 10:17:31.000000 biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_add_hydrogens.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12030 2022-12-27 10:17:38.000000 biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_convert.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9735 2022-12-27 10:17:47.000000 biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_minimize.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12049 2022-12-27 10:17:52.000000 biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_remove_hydrogens.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7325 2022-09-19 11:42:11.000000 biobb_chemistry-4.0.0/biobb_chemistry/babelm/common.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:32:59.000000 biobb_chemistry-4.0.0/biobb_chemistry/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6236 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      996 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      712 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       16 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/biobb_chemistry.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 11:51:34.000000 biobb_chemistry-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2037 2023-04-11 11:47:55.000000 biobb_chemistry-4.0.0/setup.py
```

### Comparing `biobb_chemistry-3.9.0/LICENSE` & `biobb_chemistry-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_ac.py` & `biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_ac.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_cns.py` & `biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_cns.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_gmx.py` & `biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_gmx.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py` & `biobb_chemistry-4.0.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/acpype/common.py` & `biobb_chemistry-4.0.0/biobb_chemistry/acpype/common.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/ambertools/common.py` & `biobb_chemistry-4.0.0/biobb_chemistry/ambertools/common.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py` & `biobb_chemistry-4.0.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py` & `biobb_chemistry-4.0.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_add_hydrogens.py` & `biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_add_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_convert.py` & `biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_convert.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_minimize.py` & `biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_minimize.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/babelm/babel_remove_hydrogens.py` & `biobb_chemistry-4.0.0/biobb_chemistry/babelm/babel_remove_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry/babelm/common.py` & `biobb_chemistry-4.0.0/biobb_chemistry/babelm/common.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry.egg-info/SOURCES.txt` & `biobb_chemistry-4.0.0/biobb_chemistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/biobb_chemistry.egg-info/entry_points.txt` & `biobb_chemistry-4.0.0/biobb_chemistry.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-3.9.0/setup.py` & `biobb_chemistry-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_chemistry",
-    version="3.9.0",
+    version="4.0.0",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_chemistry",
     project_urls={
         "Documentation": "https://biobb-chemistry.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==3.9.0'],
+    install_requires=['biobb_common==4.0.0'],
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "acpype_params_ac = biobb_chemistry.acpype.acpype_params_ac:main",
             "acpype_params_cns = biobb_chemistry.acpype.acpype_params_cns:main",
             "acpype_params_gmx_opls = biobb_chemistry.acpype.acpype_params_gmx_opls:main",
             "acpype_params_gmx = biobb_chemistry.acpype.acpype_params_gmx:main",
```

