# Comparing `tmp/astronomica-0.0.5.tar.gz` & `tmp/astronomica-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.5.tar", last modified: Tue Apr 11 18:29:25 2023, max compression
+gzip compressed data, was "astronomica-0.0.6.tar", last modified: Tue Apr 11 18:49:13 2023, max compression
```

## Comparing `astronomica-0.0.5.tar` & `astronomica-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:29:25.281341 astronomica-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 18:29:14.000000 astronomica-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-11 18:29:25.281341 astronomica-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-11 18:29:14.000000 astronomica-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:29:25.281341 astronomica-0.0.5/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18143 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/astronomica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/libconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 18:29:14.000000 astronomica-0.0.5/astronomica/suntiming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:29:25.281341 astronomica-0.0.5/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 18:29:25.000000 astronomica-0.0.5/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:29:25.281341 astronomica-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 18:29:14.000000 astronomica-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:13.095418 astronomica-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 18:49:03.000000 astronomica-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-11 18:49:13.095418 astronomica-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-11 18:49:03.000000 astronomica-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:13.095418 astronomica-0.0.6/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/libconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 18:49:03.000000 astronomica-0.0.6/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:49:13.095418 astronomica-0.0.6/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 18:49:13.000000 astronomica-0.0.6/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:49:13.095418 astronomica-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 18:49:03.000000 astronomica-0.0.6/setup.py
```

### Comparing `astronomica-0.0.5/LICENSE` & `astronomica-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.5/PKG-INFO` & `astronomica-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -57,14 +57,33 @@
 astropy_time_to_skyfield_time(time)
 skyfield_time_to_astropy_time(time)
 ```
 
 These functions all deal with conversions of units. The last three are for interoperability of astronomy libraries.
 
 ```python
+time()
+```
+
+returns the current time
+
+```python
+date()
+```
+
+returns the current date
+
+```python
+now = Date()
+now.now().__insert_time_element_here__
+```
+
+returns an object containing the time
+
+```python
 local_julian_date(date=datetime.datetime.now())
 ```
 
 This method returns the current local <b>julian date</b>
 
 
 ```python
```

### Comparing `astronomica-0.0.5/README.md` & `astronomica-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,33 @@
 astropy_time_to_skyfield_time(time)
 skyfield_time_to_astropy_time(time)
 ```
 
 These functions all deal with conversions of units. The last three are for interoperability of astronomy libraries.
 
 ```python
+time()
+```
+
+returns the current time
+
+```python
+date()
+```
+
+returns the current date
+
+```python
+now = Date()
+now.now().__insert_time_element_here__
+```
+
+returns an object containing the time
+
+```python
 local_julian_date(date=datetime.datetime.now())
 ```
 
 This method returns the current local <b>julian date</b>
 
 
 ```python
```

### Comparing `astronomica-0.0.5/astronomica/astronomica.py` & `astronomica-0.0.6/astronomica/astronomica.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,60 @@
 # import required libraries (math and datetime are always required, because of their uses)
 import math
 import datetime
 from astroquery.simbad import Simbad
 import requests
+import os
 
+
+def time():
+    time_str = os.popen('date +%H:%M:%S').read().strip()
+    return time_str
+
+
+def date():
+    date_str = os.popen('date +%D').read().strip()
+    return date_str
+
+
+def decimal_hours():
+    time_str = time()
+    new_time = time_str.split(':')
+    dec_hours = int(new_time[0]) + (int(new_time[1]) / 60) + (int(new_time[2]) / 3600)
+    return dec_hours
+
+
+class DateObject:
+    def __init__(self, data):
+        self.__dict__ = data
+        
+class Date:
+    def __init__(self):
+        self.minute = None
+        self.second = None
+        self.hour = None
+        self.day = None
+        self.year = None
+        self.month = None
+
+    def now(self):
+        hr, min, second = [int(part) for part in time().split(':')]
+        month, day, year = [int(part) for part in date().split('/')]
+        self.month, self.year, self.day = month, year, day
+        self.minute, self.second, self.hour = min, second, hr
+        current_time = {
+            'hour': self.hour,
+            'minute': self.minute,
+            'second': self.second,
+            'day': self.day,
+            'month': self.month,
+            'year': self.year,
+        }
+        return DateObject(current_time)
+    
 class LST:
     def __init__(self, data):
         self.__dict__ = data
 
 
 def definition_of(word):
     # make a request to the Wikipedia API
```

### Comparing `astronomica-0.0.5/astronomica/libconversion.py` & `astronomica-0.0.6/astronomica/libconversion.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.5/astronomica/suntiming.py` & `astronomica-0.0.6/astronomica/suntiming.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.5/astronomica.egg-info/PKG-INFO` & `astronomica-0.0.6/astronomica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -57,14 +57,33 @@
 astropy_time_to_skyfield_time(time)
 skyfield_time_to_astropy_time(time)
 ```
 
 These functions all deal with conversions of units. The last three are for interoperability of astronomy libraries.
 
 ```python
+time()
+```
+
+returns the current time
+
+```python
+date()
+```
+
+returns the current date
+
+```python
+now = Date()
+now.now().__insert_time_element_here__
+```
+
+returns an object containing the time
+
+```python
 local_julian_date(date=datetime.datetime.now())
 ```
 
 This method returns the current local <b>julian date</b>
 
 
 ```python
```

### Comparing `astronomica-0.0.5/setup.py` & `astronomica-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.5',
+    version='0.0.6',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/astronomica',
     project_urls = {
```

