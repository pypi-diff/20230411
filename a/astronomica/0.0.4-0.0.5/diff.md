# Comparing `tmp/astronomica-0.0.4.tar.gz` & `tmp/astronomica-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.4.tar", last modified: Tue Apr 11 17:58:29 2023, max compression
+gzip compressed data, was "astronomica-0.0.5.tar", last modified: Tue Apr 11 18:29:25 2023, max compression
```

## Comparing `astronomica-0.0.4.tar` & `astronomica-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:58:29.104708 astronomica-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 17:58:19.000000 astronomica-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-11 17:58:29.104708 astronomica-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-11 17:58:19.000000 astronomica-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:58:29.104708 astronomica-0.0.4/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/astronomica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/libconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 17:58:19.000000 astronomica-0.0.4/astronomica/suntiming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:58:29.104708 astronomica-0.0.4/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 17:58:29.000000 astronomica-0.0.4/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:58:29.104708 astronomica-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 17:58:19.000000 astronomica-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:29:25.281341 astronomica-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 18:29:14.000000 astronomica-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-11 18:29:25.281341 astronomica-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-11 18:29:14.000000 astronomica-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:29:25.281341 astronomica-0.0.5/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18143 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/libconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:29:25.281341 astronomica-0.0.5/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:29:25.281341 astronomica-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 18:29:14.000000 astronomica-0.0.5/setup.py
```

### Comparing `astronomica-0.0.4/LICENSE` & `astronomica-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.4/PKG-INFO` & `astronomica-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # astronomica
 
 ## Introduction and Purpose
 <b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation. This library does not depend on Astropy or Skyfield, but requires their installation for conversion purposes - some of our functions include interoperability of libraries - skyfield units to astropy units, etc.
 
 ### Note of Usage:
-<b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community.
+<b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community. You can also join our reddit community at https://www.reddit.com/r/pythonlibraries/ 
 
 
 ## Usage:
 Here is a very simple usage example of Astronomica:
 
 ```python
```

### Comparing `astronomica-0.0.4/README.md` & `astronomica-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # astronomica
 
 ## Introduction and Purpose
 <b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation. This library does not depend on Astropy or Skyfield, but requires their installation for conversion purposes - some of our functions include interoperability of libraries - skyfield units to astropy units, etc.
 
 ### Note of Usage:
-<b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community.
+<b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community. You can also join our reddit community at https://www.reddit.com/r/pythonlibraries/ 
 
 
 ## Usage:
 Here is a very simple usage example of Astronomica:
 
 ```python
```

### Comparing `astronomica-0.0.4/astronomica/astronomica.py` & `astronomica-0.0.5/astronomica/astronomica.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,29 +250,28 @@
     L = eclipticLongitude(M)
     H = solarHourAngle(long, localSiderealTime(long).raw)
     dec = declination(L, 0)
     return math.degrees(math.atan2(math.sin(H), math.cos(H) * math.sin(lat) - math.tan(dec) * math.cos(lat)))
 
 
 class Observer:
-    def __init__(self, latitude, longitude, planet, date=datetime.datetime.now()):
+    def __init__(self, latitude, longitude, planet):
         self.lat = latitude
         self.long = -longitude  # convert to longitude west from just longitude
-        self.dateToCalculate = date
         self.planet = planet
         self.meanA = None
         self.ceq = None
         self.v = None
         self.perihelion = None
         self.obliquity = None
         self.dist = None
         self.eclipticlong = None
 
     def julian_date(self):
-        JD = local_julian_date(self.dateToCalculate)
+        JD = local_julian_date(datetime.datetime.now())
         return JD
 
     def mean_anomaly(self):
         # formula from https://www.aa.quae.nl/en/reken/zonpositie.html
         # formula is M = (M0 + M1 * (J - J2000)) mod 360˚
         J2000 = 2451545
         m_list = [
```

### Comparing `astronomica-0.0.4/astronomica/libconversion.py` & `astronomica-0.0.5/astronomica/libconversion.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.4/astronomica/suntiming.py` & `astronomica-0.0.5/astronomica/suntiming.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.4/astronomica.egg-info/PKG-INFO` & `astronomica-0.0.5/astronomica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # astronomica
 
 ## Introduction and Purpose
 <b>Astronomica</b> is a simple python library based on formulas pioneered at https://www.aa.quae.nl/en/reken/zonpositie.html, and https://astronomica.w3spaces.com/. Scroll below to check out the documentation. This library does not depend on Astropy or Skyfield, but requires their installation for conversion purposes - some of our functions include interoperability of libraries - skyfield units to astropy units, etc.
 
 ### Note of Usage:
-<b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community.
+<b>Astronomica is 100% free</b>!! It is also <b>driven by the <i>community</i></b>, so we welcome tips, bug fixes, and more methods added by users and the general python & astronomy community. You can also join our reddit community at https://www.reddit.com/r/pythonlibraries/ 
 
 
 ## Usage:
 Here is a very simple usage example of Astronomica:
 
 ```python
```

### Comparing `astronomica-0.0.4/setup.py` & `astronomica-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.4',
+    version='0.0.5',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/astronomica',
     project_urls = {
```

