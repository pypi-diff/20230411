# Comparing `tmp/biobb_dna-3.9.0.tar.gz` & `tmp/biobb_dna-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_dna-3.9.0.tar", last modified: Tue Dec 27 11:51:24 2022, max compression
+gzip compressed data, was "dist/biobb_dna-4.0.0.tar", last modified: Tue Apr 11 13:43:39 2023, max compression
```

## Comparing `biobb_dna-3.9.0.tar` & `biobb_dna-4.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4022 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3248 2022-12-27 11:49:25.000000 biobb_dna-3.9.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      156 2022-12-27 11:49:12.000000 biobb_dna-3.9.0/biobb_dna/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/backbone/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       74 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/biobb_dna/backbone/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12716 2022-12-27 11:27:41.000000 biobb_dna-3.9.0/biobb_dna/backbone/bipopulations.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13441 2022-12-27 11:27:50.000000 biobb_dna-3.9.0/biobb_dna/backbone/canonicalag.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11630 2022-12-27 11:27:46.000000 biobb_dna-3.9.0/biobb_dna/backbone/puckering.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/curvesplus/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       74 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/biobb_dna/curvesplus/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10820 2022-12-27 11:31:59.000000 biobb_dna-3.9.0/biobb_dna/curvesplus/biobb_canal.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11646 2022-12-27 11:33:16.000000 biobb_dna-3.9.0/biobb_dna/curvesplus/biobb_canion.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13211 2022-12-27 11:34:04.000000 biobb_dna-3.9.0/biobb_dna/curvesplus/biobb_curves.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/dna/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573       76 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/biobb_dna/dna/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10978 2022-12-27 11:36:19.000000 biobb_dna-3.9.0/biobb_dna/dna/dna_averages.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13420 2022-12-27 11:37:17.000000 biobb_dna-3.9.0/biobb_dna/dna/dna_bimodality.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11436 2022-12-27 11:38:18.000000 biobb_dna-3.9.0/biobb_dna/dna/dna_timeseries.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/interbp_correlations/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      100 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/biobb_dna/interbp_correlations/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15574 2022-12-27 11:39:35.000000 biobb_dna-3.9.0/biobb_dna/interbp_correlations/interbpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15212 2022-12-27 11:42:18.000000 biobb_dna-3.9.0/biobb_dna/interbp_correlations/interhpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10019 2022-12-27 11:43:01.000000 biobb_dna-3.9.0/biobb_dna/interbp_correlations/interseqcorr.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/intrabp_correlations/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      100 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/biobb_dna/intrabp_correlations/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15867 2022-12-27 11:44:00.000000 biobb_dna-3.9.0/biobb_dna/intrabp_correlations/intrabpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15752 2022-12-27 11:44:38.000000 biobb_dna-3.9.0/biobb_dna/intrabp_correlations/intrahpcorr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9915 2022-12-27 11:45:11.000000 biobb_dna-3.9.0/biobb_dna/intrabp_correlations/intraseqcorr.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/stiffness/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573       73 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/biobb_dna/stiffness/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10183 2022-12-27 11:46:08.000000 biobb_dna-3.9.0/biobb_dna/stiffness/average_stiffness.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12644 2022-12-27 11:46:53.000000 biobb_dna-3.9.0/biobb_dna/stiffness/basepair_stiffness.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:33:51.000000 biobb_dna-3.9.0/biobb_dna/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna/utils/
--rw-r--r--   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:33:52.000000 biobb_dna-3.9.0/biobb_dna/utils/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573      900 2022-05-26 11:33:52.000000 biobb_dna-3.9.0/biobb_dna/utils/constants.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1362 2022-05-26 11:33:52.000000 biobb_dna-3.9.0/biobb_dna/utils/loader.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573      341 2022-05-26 11:33:52.000000 biobb_dna-3.9.0/biobb_dna/utils/transform.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4022 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1262 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      981 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       55 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       10 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/biobb_dna.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2022-12-27 11:51:24.000000 biobb_dna-3.9.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2448 2022-12-27 11:48:57.000000 biobb_dna-3.9.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5962 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5188 2023-04-11 13:42:33.000000 biobb_dna-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      156 2023-04-11 13:42:16.000000 biobb_dna-4.0.0/biobb_dna/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/backbone/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       74 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/biobb_dna/backbone/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12716 2022-12-27 11:27:41.000000 biobb_dna-4.0.0/biobb_dna/backbone/bipopulations.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13441 2022-12-27 11:27:50.000000 biobb_dna-4.0.0/biobb_dna/backbone/canonicalag.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11630 2022-12-27 11:27:46.000000 biobb_dna-4.0.0/biobb_dna/backbone/puckering.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/curvesplus/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       74 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/biobb_dna/curvesplus/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10820 2022-12-27 11:31:59.000000 biobb_dna-4.0.0/biobb_dna/curvesplus/biobb_canal.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11646 2022-12-27 11:33:16.000000 biobb_dna-4.0.0/biobb_dna/curvesplus/biobb_canion.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13210 2022-12-27 11:55:41.000000 biobb_dna-4.0.0/biobb_dna/curvesplus/biobb_curves.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/dna/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       76 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/biobb_dna/dna/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10978 2022-12-27 11:36:19.000000 biobb_dna-4.0.0/biobb_dna/dna/dna_averages.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13420 2022-12-27 11:37:17.000000 biobb_dna-4.0.0/biobb_dna/dna/dna_bimodality.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11436 2022-12-27 11:38:18.000000 biobb_dna-4.0.0/biobb_dna/dna/dna_timeseries.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/interbp_correlations/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      100 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/biobb_dna/interbp_correlations/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15574 2022-12-27 11:39:35.000000 biobb_dna-4.0.0/biobb_dna/interbp_correlations/interbpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15212 2022-12-27 11:42:18.000000 biobb_dna-4.0.0/biobb_dna/interbp_correlations/interhpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10019 2022-12-27 11:43:01.000000 biobb_dna-4.0.0/biobb_dna/interbp_correlations/interseqcorr.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/intrabp_correlations/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      100 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/biobb_dna/intrabp_correlations/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15867 2022-12-27 11:44:00.000000 biobb_dna-4.0.0/biobb_dna/intrabp_correlations/intrabpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15752 2022-12-27 11:44:38.000000 biobb_dna-4.0.0/biobb_dna/intrabp_correlations/intrahpcorr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9915 2022-12-27 11:45:11.000000 biobb_dna-4.0.0/biobb_dna/intrabp_correlations/intraseqcorr.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/stiffness/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       73 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/biobb_dna/stiffness/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10183 2022-12-27 11:46:08.000000 biobb_dna-4.0.0/biobb_dna/stiffness/average_stiffness.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12644 2022-12-27 11:46:53.000000 biobb_dna-4.0.0/biobb_dna/stiffness/basepair_stiffness.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:33:51.000000 biobb_dna-4.0.0/biobb_dna/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna/utils/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:33:52.000000 biobb_dna-4.0.0/biobb_dna/utils/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      900 2022-05-26 11:33:52.000000 biobb_dna-4.0.0/biobb_dna/utils/constants.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1363 2023-03-06 08:33:07.000000 biobb_dna-4.0.0/biobb_dna/utils/loader.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      341 2022-05-26 11:33:52.000000 biobb_dna-4.0.0/biobb_dna/utils/transform.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5962 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1262 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      981 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       55 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       10 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/biobb_dna.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 13:43:39.000000 biobb_dna-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2448 2023-04-11 13:42:00.000000 biobb_dna-4.0.0/setup.py
```

### Comparing `biobb_dna-3.9.0/LICENSE` & `biobb_dna-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/backbone/bipopulations.py` & `biobb_dna-4.0.0/biobb_dna/backbone/bipopulations.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/backbone/canonicalag.py` & `biobb_dna-4.0.0/biobb_dna/backbone/canonicalag.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/backbone/puckering.py` & `biobb_dna-4.0.0/biobb_dna/backbone/puckering.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/curvesplus/biobb_canal.py` & `biobb_dna-4.0.0/biobb_dna/curvesplus/biobb_canal.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/curvesplus/biobb_canion.py` & `biobb_dna-4.0.0/biobb_dna/curvesplus/biobb_canion.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/curvesplus/biobb_curves.py` & `biobb_dna-4.0.0/biobb_dna/curvesplus/biobb_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             * **stdlib_path** (*str*) - ('standard') Path to Curves' standard library files for nucleotides. If not specified will look for 'standard' files in current directory.
             * **itst** (*int*) - (0) Iteration start index.
             * **itnd** (*int*) - (0) Iteration end index.
             * **itdel** (*int*) - (1) Iteration delimiter. 
             * **ions** (*bool*) - (False) If True, helicoidal analysis of ions (or solvent molecules) around solute is carried out.
             * **test** (*bool*) - (False) If True, provide addition output in .lis file on fitting and axis generation.
             * **line** (*bool*) - (False) if True, find the best linear helical axis.
-            * **fit** (*bool*) - (False) if True, fit a standard bases to the input coordinates (important for MD snapshots to avoid base distortions leading to noisy helical parameters).
+            * **fit** (*bool*) - (True) if True, fit a standard bases to the input coordinates (important for MD snapshots to avoid base distortions leading to noisy helical parameters).
             * **axfrm** (*bool*) - (False) if True, generates closely spaced helical axis frames as input for Canal and Canion.
             * **binary_path** (*str*) - (Cur+) Path to Curves+ executable, otherwise the program wil look for Cur+ executable in the binaries folder.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
     Examples:
         This is a use example of how to use the building block from Python::
 
@@ -92,15 +92,15 @@
         self.s2range = properties.get('s2range', None)
         self.itst = properties.get('itst', 0)
         self.itnd = properties.get('itnd', 0)
         self.itdel = properties.get('itdel', 1)
         self.ions = properties.get('ions', '.f.')
         self.test = properties.get('test', '.f.')
         self.line = properties.get('line', '.f.')
-        self.fit = properties.get('fit', '.f.')
+        self.fit = properties.get('fit', '.t.')
         self.axfrm = properties.get('axfrm', '.f.')
         self.properties = properties
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
```

### Comparing `biobb_dna-3.9.0/biobb_dna/dna/dna_averages.py` & `biobb_dna-4.0.0/biobb_dna/dna/dna_averages.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/dna/dna_bimodality.py` & `biobb_dna-4.0.0/biobb_dna/dna/dna_bimodality.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/dna/dna_timeseries.py` & `biobb_dna-4.0.0/biobb_dna/dna/dna_timeseries.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/interbp_correlations/interbpcorr.py` & `biobb_dna-4.0.0/biobb_dna/interbp_correlations/interbpcorr.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/interbp_correlations/interhpcorr.py` & `biobb_dna-4.0.0/biobb_dna/interbp_correlations/interhpcorr.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/interbp_correlations/interseqcorr.py` & `biobb_dna-4.0.0/biobb_dna/interbp_correlations/interseqcorr.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/intrabp_correlations/intrabpcorr.py` & `biobb_dna-4.0.0/biobb_dna/intrabp_correlations/intrabpcorr.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/intrabp_correlations/intrahpcorr.py` & `biobb_dna-4.0.0/biobb_dna/intrabp_correlations/intrahpcorr.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/intrabp_correlations/intraseqcorr.py` & `biobb_dna-4.0.0/biobb_dna/intrabp_correlations/intraseqcorr.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/stiffness/average_stiffness.py` & `biobb_dna-4.0.0/biobb_dna/stiffness/average_stiffness.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/stiffness/basepair_stiffness.py` & `biobb_dna-4.0.0/biobb_dna/stiffness/basepair_stiffness.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/utils/constants.py` & `biobb_dna-4.0.0/biobb_dna/utils/constants.py`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna/utils/loader.py` & `biobb_dna-4.0.0/biobb_dna/utils/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 
 
 def read_series(input_serfile, usecols=None):
     """Read .ser file"""
     extra_kwargs = dict(
         header=None,
-        sep='\s+',
+        sep='\\s+',
         index_col=0)
     ser_data = pd.read_csv(input_serfile, **extra_kwargs)
     if usecols is not None:
         if 0 in usecols:
             usecols.pop(usecols.index(0))
         ser_data = ser_data[[i+1 for i in usecols]]
     return ser_data
```

### Comparing `biobb_dna-3.9.0/biobb_dna.egg-info/SOURCES.txt` & `biobb_dna-4.0.0/biobb_dna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/biobb_dna.egg-info/entry_points.txt` & `biobb_dna-4.0.0/biobb_dna.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_dna-3.9.0/setup.py` & `biobb_dna-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_dna",
-    version="3.9.0",
+    version="4.0.0",
     author="Biobb developers",
     author_email="lucia.fabio@irbbarcelona.com",
     description="Biobb_dna is a package composed of different analyses for nucleic acid trajectories.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_dna",
     project_urls={
         "Documentation": "http://biobb_dna.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['adapters', 'docs', 'test']),
     install_requires=[
-        'biobb_common==3.9.0',
+        'biobb_common==4.0.0',
         'pandas==1.3.0',
         'scikit-learn==0.24.2'],
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "biobb_curves = biobb_dna.curvesplus.biobb_curves:main",
             "biobb_canal = biobb_dna.curvesplus.biobb_canal:main",
```

