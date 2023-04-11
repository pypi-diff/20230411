# Comparing `tmp/biobb_io-3.9.0.tar.gz` & `tmp/biobb_io-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_io-3.9.0.tar", last modified: Tue Dec 27 15:12:10 2022, max compression
+gzip compressed data, was "dist/biobb_io-4.0.0.tar", last modified: Tue Apr 11 15:27:38 2023, max compression
```

## Comparing `biobb_io-3.9.0.tar` & `biobb_io-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:12:10.000000 biobb_io-3.9.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:34:05.000000 biobb_io-3.9.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4173 2022-12-27 15:12:10.000000 biobb_io-3.9.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3388 2022-12-27 15:10:59.000000 biobb_io-3.9.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573       57 2022-12-27 15:10:51.000000 biobb_io-3.9.0/biobb_io/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io/api/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      241 2022-08-16 10:29:02.000000 biobb_io-3.9.0/biobb_io/api/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5062 2022-12-27 14:58:05.000000 biobb_io-3.9.0/biobb_io/api/alphafold.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5422 2022-12-27 14:59:15.000000 biobb_io-3.9.0/biobb_io/api/api_binding_site.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5464 2022-12-27 14:59:52.000000 biobb_io-3.9.0/biobb_io/api/canonical_fasta.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13177 2022-08-16 09:57:15.000000 biobb_io-3.9.0/biobb_io/api/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4944 2022-12-27 15:00:34.000000 biobb_io-3.9.0/biobb_io/api/drugbank.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5278 2022-12-27 15:01:27.000000 biobb_io-3.9.0/biobb_io/api/ideal_sdf.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5344 2022-12-27 15:01:59.000000 biobb_io-3.9.0/biobb_io/api/ligand.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4885 2022-12-27 15:03:35.000000 biobb_io-3.9.0/biobb_io/api/memprotmd_sim.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4836 2022-12-27 15:02:32.000000 biobb_io-3.9.0/biobb_io/api/memprotmd_sim_list.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7193 2022-12-27 15:03:06.000000 biobb_io-3.9.0/biobb_io/api/memprotmd_sim_search.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5371 2022-12-27 15:04:07.000000 biobb_io-3.9.0/biobb_io/api/mmcif.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5688 2022-12-27 15:07:46.000000 biobb_io-3.9.0/biobb_io/api/pdb.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7278 2022-12-27 15:06:55.000000 biobb_io-3.9.0/biobb_io/api/pdb_cluster_zip.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6907 2022-12-27 15:07:14.000000 biobb_io-3.9.0/biobb_io/api/pdb_variants.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5175 2022-12-27 15:08:17.000000 biobb_io-3.9.0/biobb_io/api/structure_info.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:34:05.000000 biobb_io-3.9.0/biobb_io/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4173 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      716 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      652 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2022-12-27 15:12:10.000000 biobb_io-3.9.0/biobb_io.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2022-12-27 15:12:10.000000 biobb_io-3.9.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2001 2022-12-27 15:10:33.000000 biobb_io-3.9.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:27:38.000000 biobb_io-4.0.0/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:34:05.000000 biobb_io-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6091 2023-04-11 15:27:38.000000 biobb_io-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5306 2023-04-11 15:26:58.000000 biobb_io-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       57 2023-04-11 15:26:44.000000 biobb_io-4.0.0/biobb_io/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io/api/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      241 2022-08-16 10:29:02.000000 biobb_io-4.0.0/biobb_io/api/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5062 2023-01-11 12:35:16.000000 biobb_io-4.0.0/biobb_io/api/alphafold.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5422 2022-12-27 14:59:15.000000 biobb_io-4.0.0/biobb_io/api/api_binding_site.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5464 2022-12-27 14:59:52.000000 biobb_io-4.0.0/biobb_io/api/canonical_fasta.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13177 2022-08-16 09:57:15.000000 biobb_io-4.0.0/biobb_io/api/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4944 2022-12-27 15:00:34.000000 biobb_io-4.0.0/biobb_io/api/drugbank.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5278 2022-12-27 15:01:27.000000 biobb_io-4.0.0/biobb_io/api/ideal_sdf.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5344 2022-12-27 15:01:59.000000 biobb_io-4.0.0/biobb_io/api/ligand.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4885 2022-12-27 15:03:35.000000 biobb_io-4.0.0/biobb_io/api/memprotmd_sim.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4836 2022-12-27 15:02:32.000000 biobb_io-4.0.0/biobb_io/api/memprotmd_sim_list.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7193 2022-12-27 15:03:06.000000 biobb_io-4.0.0/biobb_io/api/memprotmd_sim_search.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5371 2022-12-27 15:04:07.000000 biobb_io-4.0.0/biobb_io/api/mmcif.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5688 2022-12-27 15:07:46.000000 biobb_io-4.0.0/biobb_io/api/pdb.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7278 2022-12-27 15:06:55.000000 biobb_io-4.0.0/biobb_io/api/pdb_cluster_zip.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6907 2022-12-27 15:07:14.000000 biobb_io-4.0.0/biobb_io/api/pdb_variants.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5175 2022-12-27 15:08:17.000000 biobb_io-4.0.0/biobb_io/api/structure_info.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:34:05.000000 biobb_io-4.0.0/biobb_io/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6091 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      716 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      652 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        9 2023-04-11 15:27:38.000000 biobb_io-4.0.0/biobb_io.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 15:27:38.000000 biobb_io-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2001 2023-04-11 15:26:32.000000 biobb_io-4.0.0/setup.py
```

### Comparing `biobb_io-3.9.0/LICENSE` & `biobb_io-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/alphafold.py` & `biobb_io-4.0.0/biobb_io/api/alphafold.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/api_binding_site.py` & `biobb_io-4.0.0/biobb_io/api/api_binding_site.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/canonical_fasta.py` & `biobb_io-4.0.0/biobb_io/api/canonical_fasta.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/common.py` & `biobb_io-4.0.0/biobb_io/api/common.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/drugbank.py` & `biobb_io-4.0.0/biobb_io/api/drugbank.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/ideal_sdf.py` & `biobb_io-4.0.0/biobb_io/api/ideal_sdf.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/ligand.py` & `biobb_io-4.0.0/biobb_io/api/ligand.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/memprotmd_sim.py` & `biobb_io-4.0.0/biobb_io/api/memprotmd_sim.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/memprotmd_sim_list.py` & `biobb_io-4.0.0/biobb_io/api/memprotmd_sim_list.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/memprotmd_sim_search.py` & `biobb_io-4.0.0/biobb_io/api/memprotmd_sim_search.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/mmcif.py` & `biobb_io-4.0.0/biobb_io/api/mmcif.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/pdb.py` & `biobb_io-4.0.0/biobb_io/api/pdb.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/pdb_cluster_zip.py` & `biobb_io-4.0.0/biobb_io/api/pdb_cluster_zip.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/pdb_variants.py` & `biobb_io-4.0.0/biobb_io/api/pdb_variants.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io/api/structure_info.py` & `biobb_io-4.0.0/biobb_io/api/structure_info.py`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io.egg-info/SOURCES.txt` & `biobb_io-4.0.0/biobb_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/biobb_io.egg-info/entry_points.txt` & `biobb_io-4.0.0/biobb_io.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_io-3.9.0/setup.py` & `biobb_io-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_io",
-    version="3.9.0",
+    version="4.0.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_io is the Biobb module collection to fetch data to be consumed by the rest of the Biobb building blocks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_io",
     project_urls={
         "Documentation": "http://biobb_io.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs',]),
-    install_requires=['biobb_common==3.9.0'],
+    install_requires=['biobb_common==4.0.0'],
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "alphafold = biobb_io.api.alphafold:main",
             "api_binding_site = biobb_io.api.api_binding_site:main",
             "canonical_fasta = biobb_io.api.canonical_fasta:main",
             "drugbank = biobb_io.api.drugbank:main",
```

