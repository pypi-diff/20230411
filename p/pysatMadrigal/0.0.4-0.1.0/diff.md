# Comparing `tmp/pysatMadrigal-0.0.4.tar.gz` & `tmp/pysatMadrigal-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysatMadrigal-0.0.4.tar", last modified: Fri Jun 11 17:09:44 2021, max compression
+gzip compressed data, was "pysatMadrigal-0.1.0.tar", last modified: Tue Apr 11 17:11:45 2023, max compression
```

## Comparing `pysatMadrigal-0.0.4.tar` & `pysatMadrigal-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.314977 pysatMadrigal-0.0.4/
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.304003 pysatMadrigal-0.0.4/.github/
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.305669 pysatMadrigal-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 aburrell   (503) staff       (20)      674 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 aburrell   (503) staff       (20)      762 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 aburrell   (503) staff       (20)      419 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 aburrell   (503) staff       (20)     1957 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/.github/pull_request_template.md
--rw-r--r--   0 aburrell   (503) staff       (20)      880 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/.gitignore
--rw-r--r--   0 aburrell   (503) staff       (20)      831 2021-06-02 12:18:40.000000 pysatMadrigal-0.0.4/.travis.yml
--rw-r--r--   0 aburrell   (503) staff       (20)      858 2021-06-02 12:18:40.000000 pysatMadrigal-0.0.4/.zenodo.json
--rw-r--r--   0 aburrell   (503) staff       (20)     1450 2021-06-02 12:43:52.000000 pysatMadrigal-0.0.4/CHANGELOG.md
--rw-r--r--   0 aburrell   (503) staff       (20)     3232 2021-06-04 17:11:50.000000 pysatMadrigal-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 aburrell   (503) staff       (20)     5505 2021-06-04 17:11:50.000000 pysatMadrigal-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 aburrell   (503) staff       (20)     1513 2020-07-10 17:49:06.000000 pysatMadrigal-0.0.4/LICENSE
--rw-r--r--   0 aburrell   (503) staff       (20)      227 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/MANIFEST.in
--rw-r--r--   0 aburrell   (503) staff       (20)     4370 2021-06-11 17:09:44.315131 pysatMadrigal-0.0.4/PKG-INFO
--rw-r--r--   0 aburrell   (503) staff       (20)     2682 2021-06-11 17:06:21.000000 pysatMadrigal-0.0.4/README.md
--rw-r--r--   0 aburrell   (503) staff       (20)      333 2020-07-10 17:49:06.000000 pysatMadrigal-0.0.4/description.txt
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.306856 pysatMadrigal-0.0.4/pysatMadrigal/
--rw-r--r--   0 aburrell   (503) staff       (20)       96 2021-01-21 18:16:05.000000 pysatMadrigal-0.0.4/pysatMadrigal/__init__.py
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.310768 pysatMadrigal-0.0.4/pysatMadrigal/instruments/
--rw-r--r--   0 aburrell   (503) staff       (20)      283 2021-01-21 18:16:05.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/__init__.py
--rw-r--r--   0 aburrell   (503) staff       (20)     7943 2021-06-02 17:07:17.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/dmsp_ivm.py
--rw-r--r--   0 aburrell   (503) staff       (20)     6852 2021-06-08 13:47:25.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/gnss_tec.py
--rw-r--r--   0 aburrell   (503) staff       (20)    11706 2021-06-02 12:18:49.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/jro_isr.py
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.313377 pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/
--rw-r--r--   0 aburrell   (503) staff       (20)      142 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/__init__.py
--rw-r--r--   0 aburrell   (503) staff       (20)     6442 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/dmsp.py
--rw-r--r--   0 aburrell   (503) staff       (20)    33476 2021-06-04 18:07:32.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/general.py
--rw-r--r--   0 aburrell   (503) staff       (20)     2911 2021-06-04 17:11:50.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/gnss.py
--rw-r--r--   0 aburrell   (503) staff       (20)     4107 2021-02-26 20:21:00.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/jro.py
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.313721 pysatMadrigal-0.0.4/pysatMadrigal/instruments/templates/
--rw-r--r--   0 aburrell   (503) staff       (20)     5970 2021-06-02 17:07:17.000000 pysatMadrigal-0.0.4/pysatMadrigal/instruments/templates/madrigal_pandas.py
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.314620 pysatMadrigal-0.0.4/pysatMadrigal/utils/
--rw-r--r--   0 aburrell   (503) staff       (20)       52 2021-01-21 18:16:05.000000 pysatMadrigal-0.0.4/pysatMadrigal/utils/__init__.py
--rw-r--r--   0 aburrell   (503) staff       (20)    12206 2021-06-02 13:13:54.000000 pysatMadrigal-0.0.4/pysatMadrigal/utils/coords.py
--rw-r--r--   0 aburrell   (503) staff       (20)        6 2021-06-02 12:19:33.000000 pysatMadrigal-0.0.4/pysatMadrigal/version.txt
-drwxr-xr-x   0 aburrell   (503) staff       (20)        0 2021-06-11 17:09:44.308949 pysatMadrigal-0.0.4/pysatMadrigal.egg-info/
--rw-r--r--   0 aburrell   (503) staff       (20)     4370 2021-06-11 17:09:43.000000 pysatMadrigal-0.0.4/pysatMadrigal.egg-info/PKG-INFO
--rw-r--r--   0 aburrell   (503) staff       (20)     1090 2021-06-11 17:09:44.000000 pysatMadrigal-0.0.4/pysatMadrigal.egg-info/SOURCES.txt
--rw-r--r--   0 aburrell   (503) staff       (20)        1 2021-06-11 17:09:43.000000 pysatMadrigal-0.0.4/pysatMadrigal.egg-info/dependency_links.txt
--rw-r--r--   0 aburrell   (503) staff       (20)        1 2020-07-10 17:50:46.000000 pysatMadrigal-0.0.4/pysatMadrigal.egg-info/not-zip-safe
--rw-r--r--   0 aburrell   (503) staff       (20)       43 2021-06-11 17:09:43.000000 pysatMadrigal-0.0.4/pysatMadrigal.egg-info/requires.txt
--rw-r--r--   0 aburrell   (503) staff       (20)       14 2021-06-11 17:09:43.000000 pysatMadrigal-0.0.4/pysatMadrigal.egg-info/top_level.txt
--rw-r--r--   0 aburrell   (503) staff       (20)       48 2021-05-11 14:59:11.000000 pysatMadrigal-0.0.4/requirements.txt
--rw-r--r--   0 aburrell   (503) staff       (20)     1557 2021-06-11 17:09:44.315884 pysatMadrigal-0.0.4/setup.cfg
--rw-r--r--   0 aburrell   (503) staff       (20)      340 2021-01-21 18:16:05.000000 pysatMadrigal-0.0.4/setup.py
--rw-r--r--   0 aburrell   (503) staff       (20)       82 2021-06-02 12:18:40.000000 pysatMadrigal-0.0.4/test_requirements.txt
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.687049 pysatMadrigal-0.1.0/
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.672142 pysatMadrigal-0.1.0/.github/
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.674231 pysatMadrigal-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 aburrell  (5504) staff       (20)      674 2021-02-26 20:21:00.000000 pysatMadrigal-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)      762 2021-02-26 20:21:00.000000 pysatMadrigal-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)      419 2021-02-26 20:21:00.000000 pysatMadrigal-0.1.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1957 2021-02-26 20:21:00.000000 pysatMadrigal-0.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.675975 pysatMadrigal-0.1.0/.github/workflows/
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1255 2023-03-28 14:02:57.000000 pysatMadrigal-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1908 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1390 2023-03-28 14:02:57.000000 pysatMadrigal-0.1.0/.github/workflows/pysat_rc.yml
+-rw-r--r--   0 aburrell  (5504) staff       (20)      880 2021-02-26 20:21:00.000000 pysatMadrigal-0.1.0/.gitignore
+-rw-r--r--   0 aburrell  (5504) staff       (20)      858 2021-06-02 12:18:40.000000 pysatMadrigal-0.1.0/.zenodo.json
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3069 2023-03-28 14:05:55.000000 pysatMadrigal-0.1.0/CHANGELOG.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3232 2021-06-04 17:11:50.000000 pysatMadrigal-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)     5505 2021-06-04 17:11:50.000000 pysatMadrigal-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1513 2020-07-10 17:49:06.000000 pysatMadrigal-0.1.0/LICENSE
+-rw-r--r--   0 aburrell  (5504) staff       (20)      227 2021-02-26 20:21:00.000000 pysatMadrigal-0.1.0/MANIFEST.in
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3717 2023-04-11 17:11:45.687309 pysatMadrigal-0.1.0/PKG-INFO
+-rw-r--r--   0 aburrell  (5504) staff       (20)     2563 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/README.md
+-rw-r--r--   0 aburrell  (5504) staff       (20)      333 2020-07-10 17:49:06.000000 pysatMadrigal-0.1.0/description.txt
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.677298 pysatMadrigal-0.1.0/pysatMadrigal/
+-rw-r--r--   0 aburrell  (5504) staff       (20)       96 2021-01-21 18:16:05.000000 pysatMadrigal-0.1.0/pysatMadrigal/__init__.py
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.682157 pysatMadrigal-0.1.0/pysatMadrigal/instruments/
+-rw-r--r--   0 aburrell  (5504) staff       (20)      708 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/__init__.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     7714 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/dmsp_ivm.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    11701 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/gnss_tec.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    12122 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/jro_isr.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    12998 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/madrigal_pandas.py
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.685463 pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/
+-rw-r--r--   0 aburrell  (5504) staff       (20)      142 2021-02-26 20:21:00.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/__init__.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    14460 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/dmsp.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    60689 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/general.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     2841 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/gnss.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)     5723 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/jro.py
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.686667 pysatMadrigal-0.1.0/pysatMadrigal/utils/
+-rw-r--r--   0 aburrell  (5504) staff       (20)       52 2021-01-21 18:16:05.000000 pysatMadrigal-0.1.0/pysatMadrigal/utils/__init__.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)    14635 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/pysatMadrigal/utils/coords.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)        6 2023-03-28 14:06:08.000000 pysatMadrigal-0.1.0/pysatMadrigal/version.txt
+drwxr-xr-x   0 aburrell  (5504) staff       (20)        0 2023-04-11 17:11:45.679809 pysatMadrigal-0.1.0/pysatMadrigal.egg-info/
+-rw-r--r--   0 aburrell  (5504) staff       (20)     3717 2023-04-11 17:11:45.000000 pysatMadrigal-0.1.0/pysatMadrigal.egg-info/PKG-INFO
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1153 2023-04-11 17:11:45.000000 pysatMadrigal-0.1.0/pysatMadrigal.egg-info/SOURCES.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)        1 2023-04-11 17:11:45.000000 pysatMadrigal-0.1.0/pysatMadrigal.egg-info/dependency_links.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)        1 2023-04-11 17:11:45.000000 pysatMadrigal-0.1.0/pysatMadrigal.egg-info/not-zip-safe
+-rw-r--r--   0 aburrell  (5504) staff       (20)       53 2023-04-11 17:11:45.000000 pysatMadrigal-0.1.0/pysatMadrigal.egg-info/requires.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)       14 2023-04-11 17:11:45.000000 pysatMadrigal-0.1.0/pysatMadrigal.egg-info/top_level.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)       65 2023-03-28 14:02:57.000000 pysatMadrigal-0.1.0/requirements.txt
+-rw-r--r--   0 aburrell  (5504) staff       (20)     1708 2023-04-11 17:11:45.688543 pysatMadrigal-0.1.0/setup.cfg
+-rw-r--r--   0 aburrell  (5504) staff       (20)      361 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/setup.py
+-rw-r--r--   0 aburrell  (5504) staff       (20)      117 2023-04-11 17:10:55.000000 pysatMadrigal-0.1.0/test_requirements.txt
```

### Comparing `pysatMadrigal-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `pysatMadrigal-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `pysatMadrigal-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/.github/pull_request_template.md` & `pysatMadrigal-0.1.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/.gitignore` & `pysatMadrigal-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/.zenodo.json` & `pysatMadrigal-0.1.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/CODE_OF_CONDUCT.md` & `pysatMadrigal-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/CONTRIBUTING.md` & `pysatMadrigal-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/LICENSE` & `pysatMadrigal-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysatMadrigal-0.0.4/PKG-INFO` & `pysatMadrigal-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,101 +1,97 @@
 Metadata-Version: 2.1
 Name: pysatMadrigal
-Version: 0.0.4
+Version: 0.1.0
 Summary: 'Madrigal instrument support for the pysat ecosystem'
 Home-page: https://github.com/pysat/pysatMadrigal
 Author: Angeline G. Burrell, et al.
 Author-email: pysat.developers@gmail.com
-License: UNKNOWN
-Description: <div align="left">
-                <img height="0" width="0px">
-                <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatMadrigal/main/docs/figures/pysatMadrigal.png" alt="pysatMadrigal" title="pysatMadrigal"</img>
-        </div>
-        
-        # pysatMadrigal
-        [![Documentation Status](https://readthedocs.org/projects/pysatmadrigal/badge/?version=latest)](https://pysatmadrigal.readthedocs.io/en/latest/?badge=latest)
-        [![Build Status](https://travis-ci.org/pysat/pysatMadrigal.svg?branch=main)](https://travis-ci.com/pysat/pysatMadrigal)
-        [![Coverage Status](https://coveralls.io/repos/github/pysat/pysatMadrigal/badge.svg?branch=main)](https://coveralls.io/github/pysat/pysatMadrigal?branch=main)
-        [![DOI](https://zenodo.org/badge/258384773.svg)](https://zenodo.org/badge/latestdoi/258384773)
-        [![PyPI version](https://badge.fury.io/py/pysatMadrigal.svg)](https://badge.fury.io/py/pysatMadrigal)
-        
-        pysatMadrigal allows users to import data from the Madrigal database into
-        pysat ([pysat documentation](http://pysat.readthedocs.io/en/latest/)).
-        
-        
-        # Installation
-        
-        The following instructions provide a guide for installing pysatMadrigal and
-        give some examples on how to use the routines.
-        
-        ## Prerequisites
-        
-        pysatMadrigal uses common Python modules, as well as modules developed by and
-        for the Space Physics community.  This module officially supports Python 3.7+.
-        
-        | Common modules | Community modules |
-        | -------------- | ----------------- |
-        | h5py           | madrigalWeb       |
-        | numpy          | pysat >= 3.0.0    |
-        | pandas         |                   |
-        | xarray         |                   |
-        
-        
-        ## PyPi Installation
-        ```
-        pip install pysatMadrigal
-        ```
-        
-        ## GitHub Installation
-        ```
-        git clone https://github.com/pysat/pysatMadrigal.git
-        ```
-        
-        Change directories into the repository folder and run the setup.py file.  For
-        a local install use the "--user" flag after "install".
-        
-        ```
-        cd pysatMadrigal/
-        python setup.py install
-        ```
-        
-        Note: pre-0.1.0 version
-        -----------------------
-        pysatMadrigal is currently provided as an alpha pre-release.  Feedback and
-        contributions are appreciated.
-        
-        # Examples
-        
-        The instrument modules are portable and designed to be run like any pysat
-        instrument.
-        
-        ```
-        import pysat
-        from pysatMadrigal.instruments import dmsp_ivm
-        ivm = pysat.Instrument(inst_module=dmsp_ivm, tag='utd', inst_id='f15')
-        ```
-        
-        Another way to use the instruments in an external repository is to register the
-        instruments.  This only needs to be done the first time you load an instrument.
-        Afterward, pysat will identify them using the `platform` and `name` keywords.
-        
-        ```
-        pysat.utils.registry.register('pysatMadrigal.instruments.dmsp_ivm')
-        dst = pysat.Instrument('dmsp', 'ivm', tag='utd', inst_id='f15')
-        ```
-        
 Keywords: pysat,ionosphere,Madrigal,CEDAR,thermosphere,GPS,GNSS,TEC,Jicamarca,DMSP,ISR,Incoherent scatter radar
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="left">
+        <img height="0" width="0px">
+        <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatMadrigal/main/docs/figures/pysatMadrigal.png" alt="pysatMadrigal" title="pysatMadrigal"</img>
+</div>
+
+# pysatMadrigal
+[![Documentation Status](https://readthedocs.org/projects/pysatmadrigal/badge/?version=latest)](https://pysatmadrigal.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/pysat/pysatMadrigal/badge.svg?branch=main)](https://coveralls.io/github/pysat/pysatMadrigal?branch=main)
+[![DOI](https://zenodo.org/badge/258384773.svg)](https://zenodo.org/badge/latestdoi/258384773)
+[![PyPI version](https://badge.fury.io/py/pysatMadrigal.svg)](https://badge.fury.io/py/pysatMadrigal)
+
+pysatMadrigal allows users to import data from the Madrigal database into
+pysat ([pysat documentation](http://pysat.readthedocs.io/en/latest/)).
+
+
+# Installation
+
+The following instructions provide a guide for installing pysatMadrigal and
+give some examples on how to use the routines.
+
+## Prerequisites
+
+pysatMadrigal uses common Python modules, as well as modules developed by and
+for the Space Physics community.  This module officially supports Python 3.7+.
+
+| Common modules | Community modules |
+| -------------- | ----------------- |
+| h5py           | madrigalWeb>=2.6  |
+| numpy          | pysat >= 3.0.3    |
+| pandas         |                   |
+| xarray         |                   |
+
+
+## PyPi Installation
+```
+pip install pysatMadrigal
+```
+
+## GitHub Installation
+```
+git clone https://github.com/pysat/pysatMadrigal.git
+```
+
+Change directories into the repository folder and run the setup.py file.  For
+a local install use the "--user" flag after "install".
+
+```
+cd pysatMadrigal/
+python setup.py install
+```
+
+# Examples
+
+The instrument modules are portable and designed to be run like any pysat
+instrument.
+
+```
+import pysat
+from pysatMadrigal.instruments import dmsp_ivm
+ivm = pysat.Instrument(inst_module=dmsp_ivm, tag='utd', inst_id='f15')
+```
+
+Another way to use the instruments in an external repository is to register the
+instruments.  This only needs to be done the first time you load an instrument.
+Afterward, pysat will identify them using the `platform` and `name` keywords.
+
+```
+pysat.utils.registry.register('pysatMadrigal.instruments.dmsp_ivm')
+dst = pysat.Instrument('dmsp', 'ivm', tag='utd', inst_id='f15')
+```
```

### Comparing `pysatMadrigal-0.0.4/README.md` & `pysatMadrigal-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="left">
         <img height="0" width="0px">
         <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatMadrigal/main/docs/figures/pysatMadrigal.png" alt="pysatMadrigal" title="pysatMadrigal"</img>
 </div>
 
 # pysatMadrigal
 [![Documentation Status](https://readthedocs.org/projects/pysatmadrigal/badge/?version=latest)](https://pysatmadrigal.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.org/pysat/pysatMadrigal.svg?branch=main)](https://travis-ci.com/pysat/pysatMadrigal)
+[![Build Status](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/pysat/pysatMadrigal/badge.svg?branch=main)](https://coveralls.io/github/pysat/pysatMadrigal?branch=main)
 [![DOI](https://zenodo.org/badge/258384773.svg)](https://zenodo.org/badge/latestdoi/258384773)
 [![PyPI version](https://badge.fury.io/py/pysatMadrigal.svg)](https://badge.fury.io/py/pysatMadrigal)
 
 pysatMadrigal allows users to import data from the Madrigal database into
 pysat ([pysat documentation](http://pysat.readthedocs.io/en/latest/)).
 
@@ -22,16 +22,16 @@
 ## Prerequisites
 
 pysatMadrigal uses common Python modules, as well as modules developed by and
 for the Space Physics community.  This module officially supports Python 3.7+.
 
 | Common modules | Community modules |
 | -------------- | ----------------- |
-| h5py           | madrigalWeb       |
-| numpy          | pysat >= 3.0.0    |
+| h5py           | madrigalWeb>=2.6  |
+| numpy          | pysat >= 3.0.3    |
 | pandas         |                   |
 | xarray         |                   |
 
 
 ## PyPi Installation
 ```
 pip install pysatMadrigal
@@ -46,19 +46,14 @@
 a local install use the "--user" flag after "install".
 
 ```
 cd pysatMadrigal/
 python setup.py install
 ```
 
-Note: pre-0.1.0 version
------------------------
-pysatMadrigal is currently provided as an alpha pre-release.  Feedback and
-contributions are appreciated.
-
 # Examples
 
 The instrument modules are portable and designed to be run like any pysat
 instrument.
 
 ```
 import pysat
```

### Comparing `pysatMadrigal-0.0.4/pysatMadrigal/instruments/dmsp_ivm.py` & `pysatMadrigal-0.1.0/pysatMadrigal/instruments/dmsp_ivm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 #!/usr/bin/env python
 # Full license can be found in License.md
 # Full author list can be found in .zenodo.json file
 # DOI:10.5281/zenodo.3824979
 # ----------------------------------------------------------------------------
 # -*- coding: utf-8 -*-
-"""Supports the Ion Velocity Meter (IVM)
-onboard the Defense Meteorological Satellite Program (DMSP).
+"""Supports the Defense Meteorological Satellite Program (DMSP) IVM instruments.
 
-The IVM is comprised of the Retarding Potential Analyzer (RPA) and
-Drift Meter (DM). The RPA measures the energy of plasma along the
-direction of satellite motion. By fitting these measurements
-to a theoretical description of plasma the number density, plasma
-composition, plasma temperature, and plasma motion may be determined.
-The DM directly measures the arrival angle of plasma. Using the reported
-motion of the satellite the angle is converted into ion motion along
-two orthogonal directions, perpendicular to the satellite track. The IVM is
-part of the Special Sensor for Ions, Electrons, and Scintillations (SSIES)
-instrument suite on DMSP.
-
-Downloads data from the National Science Foundation Madrigal Database.
-The routine is configured to utilize data files with instrument
-performance flags generated at the Center for Space Sciences at the
-University of Texas at Dallas.
+The Ion Velocity Meter (IVM) is comprised of the Retarding Potential Analyzer
+(RPA) and Drift Meter (DM). The RPA measures the energy of plasma along the
+direction of satellite motion. By fitting these measurements to a theoretical
+description of plasma the number density, plasma composition, plasma
+temperature, and plasma motion may be determined. The DM directly measures the
+arrival angle of plasma. Using the reported motion of the satellite the angle is
+converted into ion motion along two orthogonal directions, perpendicular to the
+satellite track. The IVM is part of the Special Sensor for Ions, Electrons, and
+Scintillations (SSIES) instrument suite on DMSP.
+
+Downloads data from the National Science Foundation Madrigal Database. The
+routine is configured to utilize data files with instrument performance flags
+generated at the Center for Space Sciences at the University of Texas at Dallas.
 
 Properties
 ----------
 platform
     'dmsp'
 name
     'ivm'
@@ -54,15 +51,16 @@
 
 import datetime as dt
 import functools
 import numpy as np
 
 from pysat import logger
 
-from pysatMadrigal.instruments.methods import general, dmsp
+from pysatMadrigal.instruments.methods import dmsp
+from pysatMadrigal.instruments.methods import general
 
 # ----------------------------------------------------------------------------
 # Instrument attributes
 
 platform = 'dmsp'
 name = 'ivm'
 tags = {'utd': 'UTDallas DMSP data processing', '': 'Level 2 data processing'}
@@ -107,66 +105,52 @@
     'f18': {tag: dt.datetime(2017, 12, 30) for tag in inst_ids['f18']}}
 
 # ----------------------------------------------------------------------------
 # Instrument methods
 
 
 def init(self):
-    """Initializes the Instrument object with values specific to DMSP IVM
-
-    Runs once upon instantiation.
-
-    Parameters
-    ----------
-    self : pysat.Instrument
-        This object
-
-    """
-
+    """Initialize the Instrument object with values specific to DMSP IVM."""
     logger.info(general.cedar_rules())
     self.acknowledgements = general.cedar_rules()
     self.references = dmsp.references(self.name)
     return
 
 
 def clean(self):
-    """Routine to return DMSP IVM data cleaned to the specified level
+    """Clean DMSP IVM data to the specified level.
 
     Note
     ----
     Supports 'clean', 'dusty', 'dirty'
 
     'clean' enforces that both RPA and DM flags are <= 1
     'dusty' <= 2
     'dirty' <= 3
-    'none' Causes pysat to skip this routine
 
-    Routine is called by pysat, and not by the end user directly.
+    When called directly by pysat, a clean level of 'none' causes pysat to skip
+    this routine.
 
     """
-
     if self.tag == 'utd':
         if self.clean_level == 'clean':
-            idx, = np.where((self['rpa_flag_ut'] <= 1)
-                            & (self['idm_flag_ut'] <= 1))
+            iclean, = np.where((self['rpa_flag_ut'] <= 1)
+                               & (self['idm_flag_ut'] <= 1))
         elif self.clean_level == 'dusty':
-            idx, = np.where((self['rpa_flag_ut'] <= 2)
-                            & (self['idm_flag_ut'] <= 2))
+            iclean, = np.where((self['rpa_flag_ut'] <= 2)
+                               & (self['idm_flag_ut'] <= 2))
         elif self.clean_level == 'dirty':
-            idx, = np.where((self['rpa_flag_ut'] <= 3)
-                            & (self['idm_flag_ut'] <= 3))
-        else:
-            idx = slice(0, self.index.shape[0])
+            iclean, = np.where((self['rpa_flag_ut'] <= 3)
+                               & (self['idm_flag_ut'] <= 3))
     else:
-        if self.clean_level in ['clean', 'dusty', 'dirty']:
-            logger.warning('this level 1 data has no quality flags')
-        idx = slice(0, self.index.shape[0])
+        logger.warning('this level 1 data has no quality flags')
+        iclean = slice(0, self.index.shape[0])
 
     # Downselect data based upon cleaning conditions above
-    self.data = self[idx]
+    self.data = self[iclean]
 
     return
 
 
 # ----------------------------------------------------------------------------
 # Instrument functions
 #
@@ -184,36 +168,36 @@
 
 # Set the load routine
 load = general.load
 
 
 def download(date_array, tag='', inst_id='', data_path=None, user=None,
              password=None, file_type='hdf5'):
-    """Downloads data from Madrigal.
+    """Download data from Madrigal.
 
     Parameters
     ----------
     date_array : array-like
         list of datetimes to download data for. The sequence of dates need not
         be contiguous.
-    tag : string
+    tag : str
         Tag identifier used for particular dataset. This input is provided by
         pysat. (default='')
-    inst_id : string
+    inst_id : str
         Satellite ID string identifier used for particular dataset. This input
         is provided by pysat. (default='')
-    data_path : string
+    data_path : str
         Path to directory to download data to. (default=None)
-    user : string
+    user : str
         User string input used for download. Provided by user and passed via
-        pysat. If an account is required for dowloads this routine here must
+        pysat. If an account is required for downloads this routine here must
         error if user not supplied. (default=None)
-    password : string
+    password : str
         Password for data download. (default=None)
-    file_type : string
+    file_type : str
         File format for Madrigal data. (default='hdf5')
 
     Note
     ----
     The user's names should be provided in field user. Ritu Karidhal should
     be entered as Ritu+Karidhal
```

### Comparing `pysatMadrigal-0.0.4/pysatMadrigal/instruments/jro_isr.py` & `pysatMadrigal-0.1.0/pysatMadrigal/instruments/jro_isr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
+#!/usr/bin/env python
+# Full license can be found in License.md
+# Full author list can be found in .zenodo.json file
+# DOI:10.5281/zenodo.3824979
+# ----------------------------------------------------------------------------
 # -*- coding: utf-8 -*-.
-"""Supports the Incoherent Scatter Radar at the Jicamarca Radio Observatory
-
-The Incoherent Scatter Radar (ISR) at the Jicamarca Radio Observatory (JRO)
-observes ion drifts, line-of-sight neutral winds, electron density and
-temperature, ion temperature, and ion composition through three overarching
-experiments.
-
-Downloads data from the JRO Madrigal Database.
+"""Supports the Incoherent Scatter Radar at the Jicamarca Radio Observatory.
 
 Properties
 ----------
 platform
     'jro'
 name
     'isr'
@@ -26,108 +24,104 @@
     jro.download(pysat.datetime(2017, 12, 30), pysat.datetime(2017, 12, 31),
                  user='Firstname+Lastname', password='email@address.com')
     jro.load(2017, 363)
 
 
 Note
 ----
-    Please provide name and email when downloading data with this routine.
+The Incoherent Scatter Radar (ISR) at the Jicamarca Radio Observatory (JRO)
+observes ion drifts, line-of-sight neutral winds, electron density and
+temperature, ion temperature, and ion composition through three overarching
+experiments.
+
+Downloads data from the JRO Madrigal Database.
+
+Please provide name (user) and email (password) when downloading data with this
+routine.
 
 """
 
 import datetime as dt
 import functools
 import numpy as np
 
 from pysat import logger
 
-from pysatMadrigal.instruments.methods import general, jro
+from pysatMadrigal.instruments.methods import general
+from pysatMadrigal.instruments.methods import jro
 
 # ----------------------------------------------------------------------------
 # Instrument attributes
 
 platform = 'jro'
 name = 'isr'
 tags = {'drifts': 'Drifts and wind', 'drifts_ave': 'Averaged drifts',
         'oblique_stan': 'Standard Faraday rotation double-pulse',
         'oblique_rand': 'Randomized Faraday rotation double-pulse',
         'oblique_long': 'Long pulse Faraday rotation'}
 inst_ids = {'': list(tags.keys())}
 
 pandas_format = False
 
-# Local attributes
-jro_fname1 = 'jro{{year:4d}}{{month:02d}}{{day:02d}}'
-jro_fname2 = '.{{version:03d}}.{file_type}'
-supported_tags = {ss: {'drifts': jro_fname1 + "drifts" + jro_fname2,
-                       'drifts_ave': jro_fname1 + "drifts_avg" + jro_fname2,
-                       'oblique_stan': jro_fname1 + jro_fname2,
-                       'oblique_rand': jro_fname1 + "?" + jro_fname2,
-                       'oblique_long': jro_fname1 + "?" + jro_fname2}
-                  for ss in inst_ids.keys()}
-remote_tags = {ss: {kk: supported_tags[ss][kk].format(file_type='hdf5')
-                    for kk in inst_ids[ss]} for ss in inst_ids.keys()}
-
 # Madrigal tags
 madrigal_inst_code = 10
 madrigal_tag = {'': {'drifts': "1910", 'drifts_ave': "1911",
                      'oblique_stan': "1800", 'oblique_rand': "1801",
                      'oblique_long': "1802"}, }
 
+# Local attributes
+jro_fname = general.madrigal_file_format_str(madrigal_inst_code, verbose=False)
+supported_tags = {ss: {'drifts': jro_fname.replace("*", "drifts"),
+                       'drifts_ave': jro_fname.replace("*", "drifts_avg"),
+                       'oblique_stan': jro_fname.replace("*", ""),
+                       'oblique_rand': jro_fname.replace("*", "?"),
+                       'oblique_long': jro_fname.replace("*", "?")}
+                  for ss in inst_ids.keys()}
+remote_tags = {ss: {kk: supported_tags[ss][kk].format(file_type='hdf5')
+                    for kk in inst_ids[ss]} for ss in inst_ids.keys()}
+
 # ----------------------------------------------------------------------------
 # Instrument test attributes
 
 _test_dates = {'': {'drifts': dt.datetime(2010, 1, 19),
                     'drifts_ave': dt.datetime(2010, 1, 19),
                     'oblique_stan': dt.datetime(2010, 4, 19),
                     'oblique_rand': dt.datetime(2000, 11, 9),
                     'oblique_long': dt.datetime(2010, 4, 12)}}
 
+
 # ----------------------------------------------------------------------------
 # Instrument methods
 
-# Madrigal will sometimes include multiple days within a file
-# labeled with a single date.
-# Filter out this extra data using the pysat nanokernel processing queue.
-# To ensure this function is always applied first, we set the filter
-# function as the default function for (JRO).
-# Default function is run first by the nanokernel on every load call.
-preprocess = general.filter_data_single_date
-
-
 def init(self):
-    """Initializes the Instrument object with values specific to JRO ISR
-    """
-
+    """Initialize the Instrument object with values specific to JRO ISR."""
     ackn_str = '\n'.join([jro.acknowledgements(), general.cedar_rules()])
 
     logger.info(ackn_str)
     self.acknowledgements = ackn_str
     self.references = jro.references()
 
     return
 
 
 def clean(self):
-    """Routine to return JRO ISR data cleaned to the specified level
+    """Clean the JRO ISR data cleaned to the specified level.
 
     Note
     ----
     Supports 'clean'
     'clean' is unknown for oblique modes, over 200 km for drifts
     'dusty' is the same as clean
     'Dirty' is the same as clean
-    'None' None
 
-    Routine is called by pysat, and not by the end user directly.
+    When called by pysat, a clean level of None will skip this routine.
 
     """
-
     # Default to selecting all of the data
-    idx = {'gdalt': [i for i in range(self.data.indexes['gdalt'].shape[0])]}
+    iclean = {'gdalt': [i for i in range(self.data.indexes['gdalt'].shape[0])]}
 
     if self.tag.find('oblique') == 0:
         # Oblique profile cleaning
         logger.info(' '.join(['The double pulse, coded pulse, and long pulse',
                               'modes implemented at Jicamarca have different',
                               'limitations arising from different degrees of',
                               'precision and accuracy. Users should consult',
@@ -138,27 +132,38 @@
             logger.warning('this level 2 data has no quality flags')
     else:
         # Ion drift cleaning
         if self.clean_level in ['clean', 'dusty', 'dirty']:
             if self.clean_level in ['clean', 'dusty']:
                 logger.warning('this level 2 data has no quality flags')
 
-            ida, = np.where((self.data.indexes['gdalt'] > 200.0))
-            idx['gdalt'] = np.unique(ida)
-        else:
-            logger.warning(' '.join(["interpretation of drifts below 200 km",
-                                     "should always be done in partnership",
-                                     "with the contact people"]))
+            idalt, = np.where((self.data.indexes['gdalt'] > 200.0))
+            iclean['gdalt'] = np.unique(idalt)
 
-    # downselect data based upon cleaning conditions above
-    self.data = self[idx]
+    # Downselect data based upon cleaning conditions above
+    self.data = self[iclean]
 
     return
 
 
+def preprocess(self):
+    """Preprocess data to default loaded data to a single day."""
+    # Madrigal will sometimes include multiple days within a file
+    # labeled with a single date. This routine filters out this extra data
+    # using the pysat nanokernel processing queue.
+    general.filter_data_single_date(self)
+
+    # Warn the user about low altitude drifts if no cleaning is being performed
+    if self.clean_level == 'none' or self.clean_level is None:
+        logger.warning(' '.join(["interpretation of drifts below 200 km",
+                                 "should always be done in partnership",
+                                 "with the contact people"]))
+    return
+
+
 # ----------------------------------------------------------------------------
 # Instrument functions
 #
 # Use the default Madrigal and pysat methods
 
 # Support listing the local files
 list_files = functools.partial(general.list_files,
@@ -169,15 +174,15 @@
                                       supported_tags=remote_tags,
                                       inst_code=madrigal_inst_code,
                                       kindats=madrigal_tag)
 
 
 def download(date_array, tag='', inst_id='', data_path=None, user=None,
              password=None, file_type='hdf5'):
-    """Downloads data from Madrigal.
+    """Download data from Madrigal.
 
     Parameters
     ----------
     date_array : array-like
         list of datetimes to download data for. The sequence of dates need not
         be contiguous.
     tag : str
@@ -196,56 +201,59 @@
         Password for data download. (default=None)
     file_type : str
         File format for Madrigal data. (default='hdf5')
 
     Notes
     -----
     The user's names should be provided in field user. Ruby Payne-Scott should
-    be entered as Ruby+Payne-Scott
+    be entered as "Ruby Payne-Scott"
 
     The password field should be the user's email address. These parameters
     are passed to Madrigal when downloading.
 
     The affiliation field is set to pysat to enable tracking of pysat
     downloads.
 
     """
     general.download(date_array, inst_code=str(madrigal_inst_code),
                      kindat=madrigal_tag[inst_id][tag], data_path=data_path,
                      user=user, password=password, file_type=file_type)
+    return
 
 
-def load(fnames, tag=None, inst_id=None):
-    """ Routine to load the JRO ISR data
+def load(fnames, tag='', inst_id=''):
+    """Load the JRO ISR data.
 
     Parameters
     -----------
     fnames : list
         List of filenames
-    tag : str or NoneType
+    tag : str
         tag name used to identify particular data set to be loaded.
-        This input is nominally provided by pysat itself. (default=None)
-    inst_id : str or NoneType
+        This input is nominally provided by pysat itself. (default='')
+    inst_id : str
         Instrument ID used to identify particular data set to be loaded.
-        This input is nominally provided by pysat itself. (default=None)
+        This input is nominally provided by pysat itself. (default='')
 
     Returns
     --------
     data : xarray.Dataset
         Object containing satellite data
     meta : pysat.Meta
         Object containing metadata such as column names and units
 
     """
     # Define the xarray coordinate dimensions (apart from time)
     xcoords = {'drifts': {('time', 'gdalt', 'gdlatr', 'gdlonr', 'kindat',
-                           'kinst'): ['nwlos', 'range', 'vipn2', 'dvipn2',
+                           'kinst'): ['nwlos', 'range', 'vipn', 'dvipn', 'vipe',
+                                      'dvipe', 'vipn2', 'dvipn2',
                                       'vipe1', 'dvipe1', 'vi72', 'dvi72',
-                                      'vi82', 'dvi82', 'paiwl', 'pacwl',
-                                      'pbiwl', 'pbcwl', 'pciel', 'pccel',
+                                      'vi82', 'dvi82', 'vi7', 'dvi7', 'vi8',
+                                      'dvi8', 'paiwl', 'pacwl', 'pbiwl',
+                                      'pbcwl', 'pciel', 'pccel',
                                       'pdiel', 'pdcel', 'jro10', 'jro11'],
                           ('time', ): ['year', 'month', 'day', 'hour', 'min',
                                        'sec', 'spcst', 'pl', 'cbadn', 'inttms',
                                        'azdir7', 'eldir7', 'azdir8', 'eldir8',
                                        'jro14', 'jro15', 'jro16', 'ut1_unix',
                                        'ut2_unix', 'recno']},
                'drifts_ave': {('time', 'gdalt', 'gdlatr', 'gdlonr', 'kindat',
```

### Comparing `pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/gnss.py` & `pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/gnss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 #!/usr/bin/env python
 # Full license can be found in License.md
 # Full author list can be found in .zenodo.json file
 # DOI:10.5281/zenodo.3824979
 # ----------------------------------------------------------------------------
 # -*- coding: utf-8 -*-
-"""Methods supporting the Global Navigation Satellite System platform
-"""
+"""Methods supporting the Global Navigation Satellite System platform."""
 
 
 def acknowledgements(name):
-    """Provide the acknowledgements for different GNSS instruments
+    """Provide the acknowledgements for different GNSS instruments.
 
     Parameters
     ----------
     name : str
         Instrument name
 
     Returns
     -------
     ackn : str
         Acknowledgement information to provide in studies using this data
 
     """
-
     ackn = {'tec': ''.join(["GPS TEC data products and access through the ",
                             "Madrigal distributed data system are provided to ",
                             "the community by the Massachusetts Institute of ",
                             "Technology under support from U.S. National ",
                             "Science Foundation grant AGS-1242204. Data for ",
                             "the TEC processing is provided by the following ",
                             "organizations: UNAVCO, Scripps Orbit and ",
@@ -47,28 +45,24 @@
                             "REseau NAtional GPS permanent, and GeoNet—the ",
                             "official source of geological hazard information ",
                             "for New Zealand."])}
 
     return ackn[name]
 
 
-def references(name, tag):
-    """Provides suggested references for the specified data set
+def references(name):
+    """Provide suggested references for the specified data set.
 
     Parameters
     ----------
     name : str
         Instrument name
-    tag : str
-        Instrument tag
 
     Returns
     -------
     refs : str
         Suggested Instrument reference(s)
 
     """
+    refs = {'tec': "Rideout and Coster (2006) doi:10.1007/s10291-006-0029-5"}
 
-    refs = {'tec':
-            {'vtec': "Rideout and Coster (2006) doi:10.1007/s10291-006-0029-5"}}
-
-    return refs[name][tag]
+    return refs[name]
```

### Comparing `pysatMadrigal-0.0.4/pysatMadrigal/instruments/methods/jro.py` & `pysatMadrigal-0.1.0/pysatMadrigal/instruments/methods/jro.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python
 # Full license can be found in License.md
 # Full author list can be found in .zenodo.json file
 # DOI:10.5281/zenodo.3824979
 # ----------------------------------------------------------------------------
 # -*- coding: utf-8 -*-
-"""Methods supporting the Jicamarca Radio Observatory (JRO) platform
-"""
+"""Methods supporting the Jicamarca Radio Observatory (JRO) platform."""
 
 import numpy as np
 
 from pysat import logger
 
 from pysatMadrigal.utils import coords
 
 
 def acknowledgements():
-    """Provides acknowlegements for the JRO instruments and experiments
+    """Provide acknowlegements for the JRO instruments and experiments.
 
     Returns
     -------
     ackn : str
         String providing acknowledgement text for studies using JRO data
 
     """
@@ -27,87 +26,127 @@
                      "Instituto Geofisico del Peru operated with support from",
                      "the NSF AGS-1433968 through Cornell University."])
 
     return ackn
 
 
 def references():
-    """Provides references for the JRO instruments and experiments
+    """Provide references for the JRO instruments and experiments.
 
     Returns
     -------
     refs : str
         String providing reference guidenance for the JRO experiments
 
     """
-
     refs = "Depends on the radar experiment; contact PI"
     return refs
 
 
 def calc_measurement_loc(inst):
-    """ Calculate the instrument measurement location in geographic coordinates
+    """Calculate the instrument measurement location in geographic coordinates.
 
     Parameters
     ----------
     inst : pysat.Instrument
         JRO ISR Instrument object
 
+    Raises
+    ------
+    ValueError
+        If no appropriate azimuth and elevation angles are found, if no range
+        variable is found, or if multiple range variables are found.
+
+
     Note
     ----
     Adds 'gdlat#', 'gdlon#' to the instrument, for all directions that
     have azimuth and elevation keys that match the format 'eldir#' and 'azdir#'
+    or 'azm' and 'elm' (in this case # will be replaced with '_bm')
 
     """
-
-    az_keys = [kk[5:] for kk in list(inst.data.keys())
-               if kk.find('azdir') == 0]
-    el_keys = [kk[5:] for kk in list(inst.data.keys())
-               if kk.find('eldir') == 0]
     good_dir = list()
+    good_pre = list()
+
+    # Assume the 'dir#' format is used
+    az_keys = [kk[5:] for kk in inst.variables if kk.find('azdir') == 0]
+    el_keys = [kk[5:] for kk in inst.variables if kk.find('eldir') == 0]
 
     for i, kk in enumerate(az_keys):
         if kk in el_keys:
             try:
-                good_dir.append(int(kk))
+                good_dir.append("{:d}".format(int(kk)))
+                good_pre.append('dir{:s}'.format(kk))
             except ValueError:
-                logger.warning("unknown direction number [{:}]".format(kk))
+                logger.warning("Unknown direction number [{:}]".format(kk))
 
-    # Calculate the geodetic latitude and longitude for each direction
+    # Assume the 'm' format is used
+    if 'azm' in inst.variables and 'elm' in inst.variables:
+        good_dir.append('_bm')
+        good_pre.append('m')
+
+    # Test the success of finding the azimuths and elevations
     if len(good_dir) == 0:
         raise ValueError("No matching azimuth and elevation data included")
 
-    for dd in good_dir:
+    # Set common meta data variables. Includes determining the longitude range,
+    # which is only possible because JRO is in the western hemisphere.
+    lon_min = 0.0 if inst['gdlonr'] > 0.0 else -180.0
+    lon_max = 360.0 + lon_min
+    notes = 'Calculated using {:s}'.format(__name__)
+
+    # Get the range key
+    range_data = None
+    for rkey in ['range', 'rgate']:
+        if rkey in inst.variables:
+            if range_data is None:
+                if rkey == 'rgate':
+                    range_data = inst['gdalt']
+                else:
+                    range_data = inst[rkey]
+            else:
+                raise ValueError('Multiple range variables found')
+
+    if range_data is None:
+        raise ValueError('No range variable found')
+
+    # Calculate the geodetic latitude and longitude for each direction
+    for i, dd in enumerate(good_dir):
         # Format the direction location keys
-        az_key = 'azdir{:d}'.format(dd)
-        el_key = 'eldir{:d}'.format(dd)
-        lat_key = 'gdlat{:d}'.format(dd)
-        lon_key = 'gdlon{:d}'.format(dd)
+        az_key = 'az{:s}'.format(good_pre[i])
+        el_key = 'el{:s}'.format(good_pre[i])
+        lat_key = 'gdlat{:s}'.format(dd)
+        lon_key = 'gdlon{:s}'.format(dd)
+
         # JRO is located 520 m above sea level (jro.igp.gob.pe./english/)
         # Also, altitude has already been calculated
         gdaltr = np.ones(shape=inst['gdlonr'].shape) * 0.52
         gdlat, gdlon, _ = coords.local_horizontal_to_global_geo(inst[az_key],
                                                                 inst[el_key],
-                                                                inst['range'],
+                                                                range_data,
                                                                 inst['gdlatr'],
                                                                 inst['gdlonr'],
                                                                 gdaltr,
                                                                 geodetic=True)
 
         # Assigning as data, to ensure that the number of coordinates match
         # the number of data dimensions
         inst.data = inst.data.assign({lat_key: gdlat, lon_key: gdlon})
 
         # Add metadata for the new data values
-        bm_label = "Beam {:d} ".format(dd)
+        bm_label = "Beam" if dd[0] == "_" else "Beam {:s} ".format(dd)
         inst.meta[lat_key] = {inst.meta.labels.units: 'degrees',
                               inst.meta.labels.name: bm_label + 'latitude',
+                              inst.meta.labels.notes: notes,
                               inst.meta.labels.desc: bm_label + 'latitude',
                               inst.meta.labels.min_val: -90.0,
                               inst.meta.labels.max_val: 90.0,
                               inst.meta.labels.fill_val: np.nan}
         inst.meta[lon_key] = {inst.meta.labels.units: 'degrees',
+                              inst.meta.labels.notes: notes,
                               inst.meta.labels.name: bm_label + 'longitude',
                               inst.meta.labels.desc: bm_label + 'longitude',
+                              inst.meta.labels.min_val: lon_min,
+                              inst.meta.labels.max_val: lon_max,
                               inst.meta.labels.fill_val: np.nan}
 
     return
```

### Comparing `pysatMadrigal-0.0.4/pysatMadrigal/utils/coords.py` & `pysatMadrigal-0.1.0/pysatMadrigal/utils/coords.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-"""
-Coordinate transformation functions
-
-"""
+#!/usr/bin/env python
+# Full license can be found in License.md
+# Full author list can be found in .zenodo.json file
+# DOI:10.5281/zenodo.3824979
+# ----------------------------------------------------------------------------
+"""Coordinate transformation functions."""
 
 import numpy as np
 
 
 def geodetic_to_geocentric(lat_in, lon_in=None, inverse=False):
-    """Converts position from geodetic to geocentric or vice-versa.
+    """Convert position from geodetic to geocentric or vice-versa.
 
     Parameters
     ----------
     lat_in : float
         latitude in degrees.
     lon_in : float or NoneType
         longitude in degrees.  Remains unchanged, so does not need to be
@@ -27,15 +29,16 @@
     lon_out : float or NoneType
         longitude [degree] (geocentric/detic if inverse=False/True)
     rad_earth : float
         Earth radius [km] (geocentric/detic if inverse=False/True)
 
     Note
     -----
-    Uses WGS-84 values
+    Uses WGS-84 values. Tested against:
+    https://www.vcalc.com/wiki/vcalc/geodetic+to+geocentric+latitude
 
     References
     ----------
     Based on J.M. Ruohoniemi's geopack and R.J. Barnes radar.pro
 
     """
     rad_eq = 6378.1370  # WGS-84 semi-major axis
@@ -67,16 +70,15 @@
     lon_out = lon_in
 
     return lat_out, lon_out, rad_earth
 
 
 def geodetic_to_geocentric_horizontal(lat_in, lon_in, az_in, el_in,
                                       inverse=False):
-    """Converts from local horizontal coordinates in a geodetic system to local
-    horizontal coordinates in a geocentric system
+    """Convert from geodetic to geocentric local horizontal coordinates.
 
     Parameters
     ----------
     lat_in : float
         latitude in degrees of the local horizontal coordinate system center
     lon_in : float
         longitude in degrees of the local horizontal coordinate system center
@@ -103,99 +105,152 @@
         elevation in degrees of the converted horizontal coordinate system
 
     References
     ----------
     Based on J.M. Ruohoniemi's geopack and R.J. Barnes radar.pro
 
     """
-
     az = np.radians(az_in)
     el = np.radians(el_in)
 
     # Transform the location of the local horizontal coordinate system center
     lat_out, lon_out, rad_earth = geodetic_to_geocentric(lat_in, lon_in,
                                                          inverse=inverse)
 
-    # Calcualte the deviation from vertical in radians
+    # Calculate the deviation from vertical in radians
     dev_vert = np.radians(lat_in - lat_out)
 
     # Calculate cartesian coordinated in local system
-    x_local = np.cos(el) * np.sin(az)
-    y_local = np.cos(el) * np.cos(az)
-    z_local = np.sin(el)
+    x_local = np.cos(el) * np.sin(az)  # W-E axis
+    y_local = np.cos(el) * np.cos(az)  # N-S axis
+    z_local = np.sin(el)  # Vertical axis
 
-    # Now rotate system about the x axis to align local vertical vector
+    # Now rotate system about the x-axis (W-E) to align local vertical vector
     # with Earth radial vector
     x_out = x_local
     y_out = y_local * np.cos(dev_vert) + z_local * np.sin(dev_vert)
     z_out = -y_local * np.sin(dev_vert) + z_local * np.cos(dev_vert)
 
     # Transform the azimuth and elevation angles
     az_out = np.degrees(np.arctan2(x_out, y_out))
     el_out = np.degrees(np.arctan(z_out / np.sqrt(x_out**2 + y_out**2)))
 
     return lat_out, lon_out, rad_earth, az_out, el_out
 
 
-def spherical_to_cartesian(az_in, el_in, r_in, inverse=False):
-    """Convert a position from spherical to cartesian, or vice-versa
+def local_spherical_to_cartesian(az_in, el_in, r_in, inverse=False):
+    """Convert a position from spherical to cartesian, or vice-versa.
 
     Parameters
     ----------
     az_in : float
         azimuth/longitude in degrees or cartesian x in km (inverse=False/True)
     el_in : float
         elevation/latitude in degrees or cartesian y in km (inverse=False/True)
     r_in : float
         distance from origin in km or cartesian z in km (inverse=False/True)
-    inverse : boolian
+    inverse : bool
         False to go from spherical to cartesian and True for the inverse
+        (default=False)
 
     Returns
     -------
     x_out : float
         cartesian x in km or azimuth/longitude in degrees (inverse=False/True)
     y_out : float
         cartesian y in km or elevation/latitude in degrees (inverse=False/True)
     z_out : float
         cartesian z in km or distance from origin in km (inverse=False/True)
 
     Note
     -----
-    This transform is the same for local or global spherical/cartesian
-    transformations.
+    This transform differs from the standard by defining azimuth as starting
+    at zero from the positive y-axis instead of the positive x-axis.
 
     Returns elevation angle (angle from the xy plane) rather than zenith angle
     (angle from the z-axis)
 
     """
-
     if inverse:
         # Cartesian to Spherical
         xy_sq = az_in**2 + el_in**2
         z_out = np.sqrt(xy_sq + r_in**2)  # This is r
         y_out = np.degrees(np.arctan2(np.sqrt(xy_sq), r_in))  # This is zenith
         y_out = 90.0 - y_out  # This is the elevation
-        x_out = np.degrees(np.arctan2(el_in, az_in))  # This is azimuth
+        x_out = np.degrees(np.arctan2(az_in, el_in))  # This is azimuth
     else:
         # Spherical coordinate system uses zenith angle (degrees from the
         # z-axis) and not the elevation angle (degrees from the x-y plane)
         zen_in = np.radians(90.0 - el_in)
 
+        # Spherical to Cartesian: varies from standard to have azimuth
+        # start from zero at the y-axis
+        x_out = r_in * np.sin(zen_in) * np.sin(np.radians(az_in))
+        y_out = r_in * np.sin(zen_in) * np.cos(np.radians(az_in))
+        z_out = r_in * np.cos(zen_in)
+
+    return x_out, y_out, z_out
+
+
+def spherical_to_cartesian(theta_in, phi_in, r_in, inverse=False):
+    """Convert a position from spherical to cartesian, or vice-versa.
+
+    Parameters
+    ----------
+    theta_in : float
+        theta in degrees or cartesian x (inverse=False/True)
+    phi_in : float
+        phi in degrees or cartesian y (inverse=False/True)
+    r_in : float
+        distance from origin or cartesian z (inverse=False/True)
+    inverse : bool
+        False to go from spherical to cartesian and True for the inverse
+        (default=False)
+
+    Returns
+    -------
+    x_out : float
+        cartesian x or theta in degrees (inverse=False/True)
+    y_out : float
+        cartesian y or phi in degrees (inverse=False/True)
+    z_out : float
+        cartesian z or radial distance from origin (inverse=False/True)
+
+    Note
+    ----
+    This transform differs from the standard by defining azimuth as starting
+    at zero from the positive y-axis instead of the positive x-axis.
+
+    Returns elevation angle (angle from the xy plane) rather than zenith angle
+    (angle from the z-axis)
+
+    """
+    if inverse:
+        # Cartesian to Spherical
+        xy_sq = theta_in**2 + phi_in**2
+        z_out = np.sqrt(xy_sq + r_in**2)  # This is r
+        y_out = np.degrees(np.arctan2(np.sqrt(xy_sq), r_in))  # This is zenith
+        y_out = 90.0 - y_out  # This is the elevation or phi
+        x_out = np.degrees(np.arctan2(phi_in, theta_in))  # This is theta
+    else:
+        # Spherical coordinate system uses zenith angle (degrees from the
+        # z-axis) and not the elevation angle (degrees from the x-y plane)
+        zen_in = np.radians(90.0 - phi_in)
+
         # Spherical to Cartesian
-        x_out = r_in * np.sin(zen_in) * np.cos(np.radians(az_in))
-        y_out = r_in * np.sin(zen_in) * np.sin(np.radians(az_in))
+        x_out = r_in * np.sin(zen_in) * np.cos(np.radians(theta_in))
+        y_out = r_in * np.sin(zen_in) * np.sin(np.radians(theta_in))
         z_out = r_in * np.cos(zen_in)
 
     return x_out, y_out, z_out
 
 
 def global_to_local_cartesian(x_in, y_in, z_in, lat_cent, lon_cent, rad_cent,
                               inverse=False):
-    """Converts a position from global to local cartesian or vice-versa
+    """Convert a position from global to local cartesian or vice-versa.
 
     Parameters
     ----------
     x_in : float
         global or local cartesian x in km (inverse=False/True)
     y_in : float
         global or local cartesian y in km (inverse=False/True)
@@ -218,50 +273,53 @@
         local or global cartesian x in km (inverse=False/True)
     y_out : float
         local or global cartesian y in km (inverse=False/True)
     z_out : float
         local or global cartesian z in km (inverse=False/True)
 
     Note
-    -----
+    ----
     The global cartesian coordinate system has its origin at the center of the
     Earth, while the local system has its origin specified by the input
     latitude, longitude, and radius.  The global system has x intersecting
     the equatorial plane and the prime meridian, z pointing North along the
     rotational axis, and y completing the right-handed coodinate system.
     The local system has z pointing up, y pointing North, and x pointing East.
 
     """
-
     # Get the global cartesian coordinates of local origin
     x_cent, y_cent, z_cent = spherical_to_cartesian(lon_cent, lat_cent,
                                                     rad_cent)
 
     # Get the amount of rotation needed to align the x-axis with the
     # Earth's rotational axis
     ax_rot = np.radians(90.0 - lat_cent)
 
     # Get the amount of rotation needed to align the global x-axis with the
     # prime meridian
-    mer_rot = np.radians(lon_cent - 90.0)
+    mer_rot = np.radians(lon_cent + 90.0)
 
     if inverse:
+        # Local to global conversion
+        #
         # Rotate about the x-axis to align the z-axis with the Earth's
         # rotational axis
         xrot = x_in
         yrot = y_in * np.cos(ax_rot) - z_in * np.sin(ax_rot)
         zrot = y_in * np.sin(ax_rot) + z_in * np.cos(ax_rot)
 
         # Rotate about the global z-axis to get the global x-axis aligned
         # with the prime meridian and translate the local center to the
         # global origin
         x_out = xrot * np.cos(mer_rot) - yrot * np.sin(mer_rot) + x_cent
         y_out = xrot * np.sin(mer_rot) + yrot * np.cos(mer_rot) + y_cent
         z_out = zrot + z_cent
     else:
+        # Global to local conversion
+        #
         # Translate global origin to the local origin
         xtrans = x_in - x_cent
         ytrans = y_in - y_cent
         ztrans = z_in - z_cent
 
         # Rotate about the global z-axis to get the local x-axis pointing East
         xrot = xtrans * np.cos(-mer_rot) - ytrans * np.sin(-mer_rot)
@@ -274,16 +332,15 @@
         z_out = yrot * np.sin(-ax_rot) + zrot * np.cos(-ax_rot)
 
     return x_out, y_out, z_out
 
 
 def local_horizontal_to_global_geo(az, el, dist, lat_orig, lon_orig, alt_orig,
                                    geodetic=True):
-    """ Convert from local horizontal coordinates to geodetic or geocentric
-    coordinates
+    """Convert from local horizontal coords to geodetic or geocentric coords.
 
     Parameters
     ----------
     az : float
         Azimuth (angle from North) of point in degrees
     el : float
         Elevation (angle from ground) of point in degrees
@@ -310,30 +367,29 @@
         Distance to the point from the centre of the Earth in km
 
     References
     ----------
     Based on J.M. Ruohoniemi's geopack and R.J. Barnes radar.pro
 
     """
-
     # If the data are in geodetic coordiantes, convert to geocentric
     if geodetic:
-        (glat, glon, rearth, gaz, gel) = \
-            geodetic_to_geocentric_horizontal(lat_orig, lon_orig, az, el,
-                                              inverse=False)
+        (glat, glon, rearth, gaz, gel) = geodetic_to_geocentric_horizontal(
+            lat_orig, lon_orig, az, el, inverse=False)
         grad = rearth + alt_orig
     else:
         glat = lat_orig
         glon = lon_orig
         grad = alt_orig + 6371.0  # Add the mean earth radius in km
         gaz = az
         gel = el
 
     # Convert from local horizontal to local cartesian coordiantes
-    x_loc, y_loc, z_loc = spherical_to_cartesian(gaz, gel, dist, inverse=False)
+    x_loc, y_loc, z_loc = local_spherical_to_cartesian(gaz, gel, dist,
+                                                       inverse=False)
 
     # Convert from local to global cartesian coordiantes
     x_glob, y_glob, z_glob = global_to_local_cartesian(x_loc, y_loc, z_loc,
                                                        glat, glon, grad,
                                                        inverse=True)
 
     # Convert from global cartesian to geocentric coordinates
```

### Comparing `pysatMadrigal-0.0.4/pysatMadrigal.egg-info/PKG-INFO` & `pysatMadrigal-0.1.0/pysatMadrigal.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,101 +1,97 @@
 Metadata-Version: 2.1
 Name: pysatMadrigal
-Version: 0.0.4
+Version: 0.1.0
 Summary: 'Madrigal instrument support for the pysat ecosystem'
 Home-page: https://github.com/pysat/pysatMadrigal
 Author: Angeline G. Burrell, et al.
 Author-email: pysat.developers@gmail.com
-License: UNKNOWN
-Description: <div align="left">
-                <img height="0" width="0px">
-                <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatMadrigal/main/docs/figures/pysatMadrigal.png" alt="pysatMadrigal" title="pysatMadrigal"</img>
-        </div>
-        
-        # pysatMadrigal
-        [![Documentation Status](https://readthedocs.org/projects/pysatmadrigal/badge/?version=latest)](https://pysatmadrigal.readthedocs.io/en/latest/?badge=latest)
-        [![Build Status](https://travis-ci.org/pysat/pysatMadrigal.svg?branch=main)](https://travis-ci.com/pysat/pysatMadrigal)
-        [![Coverage Status](https://coveralls.io/repos/github/pysat/pysatMadrigal/badge.svg?branch=main)](https://coveralls.io/github/pysat/pysatMadrigal?branch=main)
-        [![DOI](https://zenodo.org/badge/258384773.svg)](https://zenodo.org/badge/latestdoi/258384773)
-        [![PyPI version](https://badge.fury.io/py/pysatMadrigal.svg)](https://badge.fury.io/py/pysatMadrigal)
-        
-        pysatMadrigal allows users to import data from the Madrigal database into
-        pysat ([pysat documentation](http://pysat.readthedocs.io/en/latest/)).
-        
-        
-        # Installation
-        
-        The following instructions provide a guide for installing pysatMadrigal and
-        give some examples on how to use the routines.
-        
-        ## Prerequisites
-        
-        pysatMadrigal uses common Python modules, as well as modules developed by and
-        for the Space Physics community.  This module officially supports Python 3.7+.
-        
-        | Common modules | Community modules |
-        | -------------- | ----------------- |
-        | h5py           | madrigalWeb       |
-        | numpy          | pysat >= 3.0.0    |
-        | pandas         |                   |
-        | xarray         |                   |
-        
-        
-        ## PyPi Installation
-        ```
-        pip install pysatMadrigal
-        ```
-        
-        ## GitHub Installation
-        ```
-        git clone https://github.com/pysat/pysatMadrigal.git
-        ```
-        
-        Change directories into the repository folder and run the setup.py file.  For
-        a local install use the "--user" flag after "install".
-        
-        ```
-        cd pysatMadrigal/
-        python setup.py install
-        ```
-        
-        Note: pre-0.1.0 version
-        -----------------------
-        pysatMadrigal is currently provided as an alpha pre-release.  Feedback and
-        contributions are appreciated.
-        
-        # Examples
-        
-        The instrument modules are portable and designed to be run like any pysat
-        instrument.
-        
-        ```
-        import pysat
-        from pysatMadrigal.instruments import dmsp_ivm
-        ivm = pysat.Instrument(inst_module=dmsp_ivm, tag='utd', inst_id='f15')
-        ```
-        
-        Another way to use the instruments in an external repository is to register the
-        instruments.  This only needs to be done the first time you load an instrument.
-        Afterward, pysat will identify them using the `platform` and `name` keywords.
-        
-        ```
-        pysat.utils.registry.register('pysatMadrigal.instruments.dmsp_ivm')
-        dst = pysat.Instrument('dmsp', 'ivm', tag='utd', inst_id='f15')
-        ```
-        
 Keywords: pysat,ionosphere,Madrigal,CEDAR,thermosphere,GPS,GNSS,TEC,Jicamarca,DMSP,ISR,Incoherent scatter radar
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="left">
+        <img height="0" width="0px">
+        <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatMadrigal/main/docs/figures/pysatMadrigal.png" alt="pysatMadrigal" title="pysatMadrigal"</img>
+</div>
+
+# pysatMadrigal
+[![Documentation Status](https://readthedocs.org/projects/pysatmadrigal/badge/?version=latest)](https://pysatmadrigal.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/pysat/pysatMadrigal/badge.svg?branch=main)](https://coveralls.io/github/pysat/pysatMadrigal?branch=main)
+[![DOI](https://zenodo.org/badge/258384773.svg)](https://zenodo.org/badge/latestdoi/258384773)
+[![PyPI version](https://badge.fury.io/py/pysatMadrigal.svg)](https://badge.fury.io/py/pysatMadrigal)
+
+pysatMadrigal allows users to import data from the Madrigal database into
+pysat ([pysat documentation](http://pysat.readthedocs.io/en/latest/)).
+
+
+# Installation
+
+The following instructions provide a guide for installing pysatMadrigal and
+give some examples on how to use the routines.
+
+## Prerequisites
+
+pysatMadrigal uses common Python modules, as well as modules developed by and
+for the Space Physics community.  This module officially supports Python 3.7+.
+
+| Common modules | Community modules |
+| -------------- | ----------------- |
+| h5py           | madrigalWeb>=2.6  |
+| numpy          | pysat >= 3.0.3    |
+| pandas         |                   |
+| xarray         |                   |
+
+
+## PyPi Installation
+```
+pip install pysatMadrigal
+```
+
+## GitHub Installation
+```
+git clone https://github.com/pysat/pysatMadrigal.git
+```
+
+Change directories into the repository folder and run the setup.py file.  For
+a local install use the "--user" flag after "install".
+
+```
+cd pysatMadrigal/
+python setup.py install
+```
+
+# Examples
+
+The instrument modules are portable and designed to be run like any pysat
+instrument.
+
+```
+import pysat
+from pysatMadrigal.instruments import dmsp_ivm
+ivm = pysat.Instrument(inst_module=dmsp_ivm, tag='utd', inst_id='f15')
+```
+
+Another way to use the instruments in an external repository is to register the
+instruments.  This only needs to be done the first time you load an instrument.
+Afterward, pysat will identify them using the `platform` and `name` keywords.
+
+```
+pysat.utils.registry.register('pysatMadrigal.instruments.dmsp_ivm')
+dst = pysat.Instrument('dmsp', 'ivm', tag='utd', inst_id='f15')
+```
```

### Comparing `pysatMadrigal-0.0.4/pysatMadrigal.egg-info/SOURCES.txt` & `pysatMadrigal-0.1.0/pysatMadrigal.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .gitignore
-.travis.yml
 .zenodo.json
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
@@ -12,27 +11,30 @@
 setup.cfg
 setup.py
 test_requirements.txt
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
+.github/workflows/docs.yml
+.github/workflows/main.yml
+.github/workflows/pysat_rc.yml
 pysatMadrigal/__init__.py
 pysatMadrigal/version.txt
 pysatMadrigal.egg-info/PKG-INFO
 pysatMadrigal.egg-info/SOURCES.txt
 pysatMadrigal.egg-info/dependency_links.txt
 pysatMadrigal.egg-info/not-zip-safe
 pysatMadrigal.egg-info/requires.txt
 pysatMadrigal.egg-info/top_level.txt
 pysatMadrigal/instruments/__init__.py
 pysatMadrigal/instruments/dmsp_ivm.py
 pysatMadrigal/instruments/gnss_tec.py
 pysatMadrigal/instruments/jro_isr.py
+pysatMadrigal/instruments/madrigal_pandas.py
 pysatMadrigal/instruments/methods/__init__.py
 pysatMadrigal/instruments/methods/dmsp.py
 pysatMadrigal/instruments/methods/general.py
 pysatMadrigal/instruments/methods/gnss.py
 pysatMadrigal/instruments/methods/jro.py
-pysatMadrigal/instruments/templates/madrigal_pandas.py
 pysatMadrigal/utils/__init__.py
 pysatMadrigal/utils/coords.py
```

### Comparing `pysatMadrigal-0.0.4/setup.cfg` & `pysatMadrigal-0.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -15,55 +15,59 @@
 	GNSS
 	TEC
 	Jicamarca
 	DMSP
 	ISR
 	Incoherent scatter radar
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Topic :: Scientific/Engineering :: Physics
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Operating System :: MacOS :: MacOS X
 	Operating System :: POSIX :: Linux
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
-python_requires = >= 3.5
+python_requires = >= 3.6
 setup_requires = setuptools >= 38.6; pip >= 10
 include_package_data = True
 zip_safe = False
 packages = find:
 install_requires = h5py
 	madrigalWeb
 	numpy
+	packaging
 	pandas
 	pysat
 	xarray
 
 [coverage:report]
-omit = */instruments/templates/
+omit = */instruments/templates/*
 
 [flake8]
 max-line-length = 80
 ignore = W503
 
 [tool:pytest]
 markers = 
 	all_inst: tests all instruments
 	download: tests for downloadable instruments
 	no_download: tests for instruments without download support
+	load_options: tests for instruments with additional options
 	first: first tests to run
 	second: second tests to run
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

