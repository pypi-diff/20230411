# Comparing `tmp/solvency2_data-0.1.5.tar.gz` & `tmp/solvency2_data-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/solvency2_data-0.1.5.tar", last modified: Tue Jan 28 14:54:26 2020, max compression
+gzip compressed data, was "dist/solvency2_data-0.1.7.tar", last modified: Mon Feb 24 07:02:22 2020, max compression
```

## Comparing `solvency2_data-0.1.5.tar` & `solvency2_data-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-28 14:54:26.316327 solvency2_data-0.1.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)      263 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3189 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3563 2020-01-28 14:54:26.316327 solvency2_data-0.1.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-28 14:54:26.312329 solvency2_data-0.1.5/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4948 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1214 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      776 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2020-01-28 14:54:26.316327 solvency2_data-0.1.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-28 14:54:26.312329 solvency2_data-0.1.5/solvency2_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/solvency2_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16265 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/solvency2_data/solvency2_data.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-28 14:54:26.316327 solvency2_data-0.1.5/solvency2_data.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3563 2020-01-28 14:54:26.000000 solvency2_data-0.1.5/solvency2_data.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2020-01-28 14:54:26.000000 solvency2_data-0.1.5/solvency2_data.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-28 14:54:26.000000 solvency2_data-0.1.5/solvency2_data.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-28 14:54:26.000000 solvency2_data-0.1.5/solvency2_data.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-01-28 14:54:26.000000 solvency2_data-0.1.5/solvency2_data.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-01-28 14:54:26.000000 solvency2_data-0.1.5/solvency2_data.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-28 14:54:26.316327 solvency2_data-0.1.5/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-28 14:54:26.316327 solvency2_data-0.1.5/tests/test_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/tests/test_data/README.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12421 2020-01-28 14:53:39.000000 solvency2_data-0.1.5/tests/test_solvency2_data.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      263 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3189 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3875 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.960959 solvency2_data-0.1.7/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      615 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/authors.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4948 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      304 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1214 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      776 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/usage.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      461 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.960959 solvency2_data-0.1.7/solvency2_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/solvency2_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16290 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/solvency2_data/solvency2_data.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/solvency2_data.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3875 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      615 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/tests/test_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/tests/test_data/README.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12421 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/tests/test_solvency2_data.py
```

### Comparing `solvency2_data-0.1.5/CONTRIBUTING.rst` & `solvency2_data-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/LICENSE` & `solvency2_data-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/PKG-INFO` & `solvency2_data-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: solvency2_data
-Version: 0.1.5
+Version: 0.1.7
 Summary: Package for reading the Solvency 2 Risk-Free Interest Rate Term Structures from the zip-files on the EIOPA website and deriving the term structures for alternative extrapolations
 Home-page: https://github.com/DeNederlandscheBank/solvency2-data
 Author: De Nederlandsche Bank
 Author-email: ECDB_berichten@dnb.nl
 License: MIT/X license
 Description: ==============
         solvency2-data
@@ -71,19 +71,34 @@
         * Development releases.
         
         0.1.1 (2019-11-6)
         -----------------
         
         * First release on PyPI.
         
-        0.1.5 (2020-28-1)
+        0.1.3
+        -----
+        
+        * First working version.
+        
+        0.1.4 (2019-11-28)
+        ------------------
+        
+        * Solvency 2 shocked curves added.
+        
+        0.1.5 (2020-1-28)
         -----------------
         
         * Spreads from PD_Cod Excel file added
         
+        0.1.7 (2020-2-23)
+        -----------------
+        
+        * Broken links from EIOPA website fixed
+        
 Keywords: solvency2_data
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `solvency2_data-0.1.5/README.rst` & `solvency2_data-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/docs/Makefile` & `solvency2_data-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/docs/conf.py` & `solvency2_data-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/docs/installation.rst` & `solvency2_data-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/docs/make.bat` & `solvency2_data-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/docs/usage.rst` & `solvency2_data-0.1.7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/setup.py` & `solvency2_data-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     keywords='solvency2_data',
     name='solvency2_data',
     packages=find_packages(include=['solvency2_data', 'solvency2_data.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/DeNederlandscheBank/solvency2-data',
-    version='0.1.5',
+    version='0.1.7',
     zip_safe=False,
 )
```

### Comparing `solvency2_data-0.1.5/solvency2_data/solvency2_data.py` & `solvency2_data-0.1.7/solvency2_data/solvency2_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Main module."""
 
 __author__ = """De Nederlandsche Bank"""
 __email__ = 'ECDB_berichten@dnb.nl'
-__version__ = '0.1.5'
+__version__ = '0.1.7'
 
 from datetime import datetime, timedelta
 from urllib.request import urlopen
 import zipfile
 import os
 import numpy as np
 from numpy.linalg import inv
@@ -56,16 +56,16 @@
      'path_excelfile': '',
      'name_excelfile': 'EIOPA_RFR_20171231_Term_Structures.xlsx'}
     """
     
     cache = RFR_reference_date(input_date, cache)
 
     reference_date = cache['reference_date']
-    cache['url'] = "https://eiopa.europa.eu/Publications/Standards/"
-    cache['name_zipfile'] = "EIOPA_RFR_" + reference_date + ".zip"
+    cache['url'] = "https://www.eiopa.europa.eu/sites/default/files/risk_free_interest_rate/"
+    cache['name_zipfile'] = "eiopa_rfr_" + reference_date + ".zip"
     cache['name_excelfile'] = "EIOPA_RFR_" + reference_date + "_Term_Structures" + ".xlsx"
     cache['name_excelfile_spreads'] = "EIOPA_RFR_" + reference_date + "_PD_Cod" + ".xlsx"
     
     return cache
     
 def download_RFR(input_date = None, cache = {}):
     """Downloads the zipfile from the EIOPA website and extracts the Excel file
```

### Comparing `solvency2_data-0.1.5/solvency2_data.egg-info/PKG-INFO` & `solvency2_data-0.1.7/solvency2_data.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: solvency2-data
-Version: 0.1.5
+Version: 0.1.7
 Summary: Package for reading the Solvency 2 Risk-Free Interest Rate Term Structures from the zip-files on the EIOPA website and deriving the term structures for alternative extrapolations
 Home-page: https://github.com/DeNederlandscheBank/solvency2-data
 Author: De Nederlandsche Bank
 Author-email: ECDB_berichten@dnb.nl
 License: MIT/X license
 Description: ==============
         solvency2-data
@@ -71,19 +71,34 @@
         * Development releases.
         
         0.1.1 (2019-11-6)
         -----------------
         
         * First release on PyPI.
         
-        0.1.5 (2020-28-1)
+        0.1.3
+        -----
+        
+        * First working version.
+        
+        0.1.4 (2019-11-28)
+        ------------------
+        
+        * Solvency 2 shocked curves added.
+        
+        0.1.5 (2020-1-28)
         -----------------
         
         * Spreads from PD_Cod Excel file added
         
+        0.1.7 (2020-2-23)
+        -----------------
+        
+        * Broken links from EIOPA website fixed
+        
 Keywords: solvency2_data
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `solvency2_data-0.1.5/solvency2_data.egg-info/SOURCES.txt` & `solvency2_data-0.1.7/solvency2_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.1.5/tests/test_solvency2_data.py` & `solvency2_data-0.1.7/tests/test_solvency2_data.py`

 * *Files identical despite different names*

