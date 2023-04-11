# Comparing `tmp/astronomica-0.0.3.tar.gz` & `tmp/astronomica-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.3.tar", last modified: Tue Apr 11 17:05:59 2023, max compression
+gzip compressed data, was "astronomica-0.0.4.tar", last modified: Tue Apr 11 17:58:29 2023, max compression
```

## Comparing `astronomica-0.0.3.tar` & `astronomica-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:05:59.636388 astronomica-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 17:05:47.000000 astronomica-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-11 17:05:59.636388 astronomica-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-11 17:05:47.000000 astronomica-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:05:59.632388 astronomica-0.0.3/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 17:05:47.000000 astronomica-0.0.3/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-11 17:05:47.000000 astronomica-0.0.3/astronomica/astronomica.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 17:05:47.000000 astronomica-0.0.3/astronomica/suntiming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:05:59.636388 astronomica-0.0.3/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:05:59.636388 astronomica-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 17:05:47.000000 astronomica-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:58:29.104708 astronomica-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 17:58:19.000000 astronomica-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-11 17:58:29.104708 astronomica-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-11 17:58:19.000000 astronomica-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:58:29.104708 astronomica-0.0.4/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/libconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:58:29.104708 astronomica-0.0.4/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:58:29.104708 astronomica-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 17:58:19.000000 astronomica-0.0.4/setup.py
```

### Comparing `astronomica-0.0.3/LICENSE` & `astronomica-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.3/PKG-INFO` & `astronomica-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: astronomica
-Version: 0.0.3
-Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
-Home-page: https://github.com/PyndyalaCoder/astronomica
-Author: Siddhu Pendyala
-Author-email: elcientifico.pendyala@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # astronomica
 
-## Astronomica Usage Exampe
-<b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation.
+## Introduction and Purpose
+<b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation. This library does not depend on Astropy or Skyfield, but requires their installation for conversion purposes - some of our functions include interoperability of libraries - skyfield units to astropy units, etc.
 
 ### Note of Usage:
 <b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community.
 
 
 ## Usage:
 Here is a very simple usage example of Astronomica:
@@ -35,14 +23,36 @@
   waitForFullMoon()
 
 ```
 
 ## Methods
 
 ```python
+fahrenheit_to_celsius(f)
+celsius_to_fahrenheit(c)
+miles_to_kilometers(m)
+pounds_to_kilograms(lb)
+kilometers_to_miles(km)
+kilograms_to_pounds(kg)
+inches_to_centimeters(inch)
+centimeters_to_inches(cm)
+au_to_km(au)
+km_to_au(km)
+light_years_to_km(ly)
+km_to_light_years(km)
+parsecs_to_light_years(pc)
+light_years_to_parsecs(ly)
+astropy_length_to_skyfield_length(length)
+astropy_time_to_skyfield_time(time)
+skyfield_time_to_astropy_time(time)
+```
+
+These functions all deal with conversions of units. The last three are for interoperability of astronomy libraries.
+
+```python
 local_julian_date(date=datetime.datetime.now())
 ```
 
 This method returns the current local <b>julian date</b>
 
 
 ```python
```

### Comparing `astronomica-0.0.3/astronomica/astronomica.py` & `astronomica-0.0.4/astronomica/astronomica.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.3/astronomica/suntiming.py` & `astronomica-0.0.4/astronomica/suntiming.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.3/setup.py` & `astronomica-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.3',
+    version='0.0.4',
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
-    install_requires=['astroquery', 'requests'],
+    install_requires=['astroquery', 'requests', 'astropy', 'skyfield'],
 )
```

