# Comparing `tmp/astronomica-0.0.1.tar.gz` & `tmp/astronomica-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.1.tar", last modified: Tue Apr 11 00:24:21 2023, max compression
+gzip compressed data, was "astronomica-0.0.2.tar", last modified: Tue Apr 11 02:49:24 2023, max compression
```

## Comparing `astronomica-0.0.1.tar` & `astronomica-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:24:21.925651 astronomica-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 00:24:12.000000 astronomica-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 00:24:21.925651 astronomica-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-11 00:24:12.000000 astronomica-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:24:21.925651 astronomica-0.0.1/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 00:24:12.000000 astronomica-0.0.1/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15793 2023-04-11 00:24:12.000000 astronomica-0.0.1/astronomica/astronomica.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 00:24:12.000000 astronomica-0.0.1/astronomica/suntiming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:24:21.925651 astronomica-0.0.1/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:24:21.925651 astronomica-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 00:24:12.000000 astronomica-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:49:24.288350 astronomica-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 02:49:12.000000 astronomica-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 02:49:24.288350 astronomica-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-11 02:49:12.000000 astronomica-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:49:24.288350 astronomica-0.0.2/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 02:49:12.000000 astronomica-0.0.2/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-04-11 02:49:12.000000 astronomica-0.0.2/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 02:49:12.000000 astronomica-0.0.2/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:49:24.288350 astronomica-0.0.2/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:49:24.288350 astronomica-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-11 02:49:12.000000 astronomica-0.0.2/setup.py
```

### Comparing `astronomica-0.0.1/LICENSE` & `astronomica-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.1/PKG-INFO` & `astronomica-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
```

### Comparing `astronomica-0.0.1/README.md` & `astronomica-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.1/astronomica/astronomica.py` & `astronomica-0.0.2/astronomica/astronomica.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,55 @@
 # import required libraries (math and datetime are always required, because of their uses)
 import math
 import datetime
+from astroquery.simbad import Simbad
 
 class LST:
     def __init__(self, data):
         self.__dict__ = data
 
+def get_object_equatorial_coords(obj_name):
+    """
+    :param obj_name: name of the SIMBAD object
+    :return: the RA and declination of the object
+    """
+    # Query the SIMBAD database for the object
+    result_table = Simbad.query_object(obj_name)
+    # Extract the RA and Dec coordinates from the result table
+    ra = result_table['RA'][0]
+    dec = result_table['DEC'][0]
+    # Return the RA and Dec coordinates as floats
+    return ra, dec
+
+def get_spectral_info(obj_name):
+    """
+    Query the SIMBAD database for spectral information on the given object.
+
+    :param obj_name: Name or identifier of the object.
+    :return: A dictionary with the spectral information for the object.
+    """
+    # Query the SIMBAD database for the object
+    result_table = Simbad.query_object(obj_name)
+    # Check if the result table is empty
+    if result_table is None:
+        return {'error': f'No results found for object {obj_name}'}
+    # Check if the spectral type is present in the result table
+    if 'SP_TYPE' in result_table.columns:
+        spectral_type = result_table['SP_TYPE'][0]
+    else:
+        spectral_type = 'N/A'
+    # Check if the spectral class is present in the result table
+    if 'SP_BIBCODE' in result_table.columns:
+        spectral_class = result_table['SP_BIBCODE'][0]
+    else:
+        spectral_class = 'N/A'
+    # Return the spectral information as a dictionary
+    return {'spectral_type': spectral_type, 'spectral_class': spectral_class}
+
+
 def local_julian_date(date=datetime.datetime.now()):
     time = date.timestamp() * 1000  # Convert to milliseconds
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() is not None else 0  # Convert to minutes
     return (time / 86400000) - (tzoffset / 1440) + 2440587.5  # return the Julian Date
 
 
 J1970 = 2440588
```

### Comparing `astronomica-0.0.1/astronomica/suntiming.py` & `astronomica-0.0.2/astronomica/suntiming.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.1/astronomica.egg-info/PKG-INFO` & `astronomica-0.0.2/astronomica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
```

### Comparing `astronomica-0.0.1/setup.py` & `astronomica-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.1',
+    version='0.0.2',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/astronomica',
     project_urls = {
         "Bug Tracker": "https://github.com/PyndyalaCoder/astronomica/issues"
     },
     license='MIT',
     packages=['astronomica'],
-    install_requires=[],
+    install_requires=['astroquery'],
 )
```

