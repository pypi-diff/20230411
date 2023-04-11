# Comparing `tmp/astronomica-0.0.0.tar.gz` & `tmp/astronomica-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.0.tar", last modified: Mon Apr 10 18:35:08 2023, max compression
+gzip compressed data, was "astronomica-0.0.1.tar", last modified: Tue Apr 11 00:24:21 2023, max compression
```

## Comparing `astronomica-0.0.0.tar` & `astronomica-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:08.360664 astronomica-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 18:34:58.000000 astronomica-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-10 18:35:08.360664 astronomica-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-10 18:34:58.000000 astronomica-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:08.360664 astronomica-0.0.0/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:34:58.000000 astronomica-0.0.0/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-10 18:34:58.000000 astronomica-0.0.0/astronomica/astronomica.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:35:08.360664 astronomica-0.0.0/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-10 18:35:08.000000 astronomica-0.0.0/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-10 18:35:08.000000 astronomica-0.0.0/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:35:08.000000 astronomica-0.0.0/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 18:35:08.000000 astronomica-0.0.0/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:35:08.360664 astronomica-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-10 18:34:58.000000 astronomica-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:24:21.925651 astronomica-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 00:24:12.000000 astronomica-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 00:24:21.925651 astronomica-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-11 00:24:12.000000 astronomica-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:24:21.925651 astronomica-0.0.1/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 00:24:12.000000 astronomica-0.0.1/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15793 2023-04-11 00:24:12.000000 astronomica-0.0.1/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 00:24:12.000000 astronomica-0.0.1/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:24:21.925651 astronomica-0.0.1/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 00:24:21.000000 astronomica-0.0.1/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:24:21.925651 astronomica-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 00:24:12.000000 astronomica-0.0.1/setup.py
```

### Comparing `astronomica-0.0.0/LICENSE` & `astronomica-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.0/PKG-INFO` & `astronomica-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -69,16 +69,25 @@
 
 This method returns the current lunar phase
 
 ```python
 daysSinceJ2000()
 ```
 
+
 This method returns the days since Jan 1st 2000 Epoch
 
+```python
+sun = Sun(lat, long)
+sun.get_local_sunrise_time()
+sun.get_local_sunset_time()
+```
+
+These methods return the sunrise and sunset time
+
 
 ```python
 decimalHours(now) # now is the chosen time
 ```
 
 This method returns the decimal hours for a given time
 
@@ -96,14 +105,20 @@
 
 ```python
 azimuth(lat, long)
 ```
 
 This method returns the current solar azimuth in degrees for a given latitude and longitude <b>east</b>
 
+```python
+map_star(star)
+```
+
+This method returns the type of star based on its name. 
+
 ## Observer Class
 
 ```
 observer = Observer(lat, long, desired_planet_for_calculations, date=datetime.datetime.now())
 ```
 
 ### Methods in class
```

### Comparing `astronomica-0.0.0/README.md` & `astronomica-0.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,16 +57,25 @@
 
 This method returns the current lunar phase
 
 ```python
 daysSinceJ2000()
 ```
 
+
 This method returns the days since Jan 1st 2000 Epoch
 
+```python
+sun = Sun(lat, long)
+sun.get_local_sunrise_time()
+sun.get_local_sunset_time()
+```
+
+These methods return the sunrise and sunset time
+
 
 ```python
 decimalHours(now) # now is the chosen time
 ```
 
 This method returns the decimal hours for a given time
 
@@ -84,14 +93,20 @@
 
 ```python
 azimuth(lat, long)
 ```
 
 This method returns the current solar azimuth in degrees for a given latitude and longitude <b>east</b>
 
+```python
+map_star(star)
+```
+
+This method returns the type of star based on its name. 
+
 ## Observer Class
 
 ```
 observer = Observer(lat, long, desired_planet_for_calculations, date=datetime.datetime.now())
 ```
 
 ### Methods in class
```

### Comparing `astronomica-0.0.0/astronomica/astronomica.py` & `astronomica-0.0.1/astronomica/astronomica.py`

 * *Files 18% similar despite different names*

```diff
@@ -471,7 +471,79 @@
         w = w_table[key]
         v = self.true_anomaly()
         r = self.distance_to_sun()
         xplanet = r * (math.cos(horse) * math.cos(w + v) - math.sin(horse) * math.cos(i) * math.sin(w + v))
         yplanet = r * (math.sin(horse)*math.cos(w + v) + math.cos(horse ) *math.cos(i) * math.sin(w + v))
         zplanet = r * math.sin(i) * math.sin(w + v)
         return xplanet, yplanet, zplanet
+
+
+
+star_catalog = {
+    'Sun': 'G2V',
+    'Sirius': 'A1V',
+    'Betelgeuse': 'M2Iab',
+    'Rigel': 'B8Ia',
+    'Vega': 'A0Va',
+    'Alpha Centauri A': 'G2V',
+    'Alpha Centauri B': 'K1V',
+    'Proxima Centauri': 'M5Ve',
+    'Polaris': 'F7Ib',
+    'Capella': 'G5III',
+    'Arcturus': 'K1.5III',
+    'Aldebaran': 'K5III',
+    'Deneb': 'A2Ia',
+    'Antares': 'M1.5Iab-IbB',
+    'Altair': 'A7V',
+    'Fomalhaut': 'A3V',
+    'Spica': 'B1III-IV',
+    'Bellatrix': 'B2III',
+    'Regulus': 'B7V',
+    'Mizar': 'A2V',
+    'Castor': 'A1V',
+    'Pollux': 'K0III',
+    'Achernar': 'B3Vp',
+    'Acrux': 'B0.5IV',
+    'Alnair': 'B7IV-V',
+    'Atria': 'K2Ib-IIa',
+    'Canopus': 'F0Ib',
+    'Gamma Velorum': 'WC8+O9I',
+    'Hadar': 'B1IV',
+    'Miaplacidus': 'A0III',
+    'Naos': 'O5If',
+    'Rigil Kentaurus': 'G2V+K1V',
+    'Sadr': 'F8Ib',
+    'Shaula': 'B0.5IV-V',
+    'Suhail': 'K4Ib-II',
+    'Vega': 'A0Va',
+    'Achernar': 'B3Vpe',
+    'Adhara': 'B2II',
+    'Albireo A': 'K3II-III',
+    'Albireo B': 'B8V',
+    'Alcor': 'A5V',
+    'Alioth': 'A0p',
+    'Alkaid': 'B3V',
+    'Alnath': 'B7III',
+    'Alnilam': 'B0Ia',
+    'Alnitak': 'O9.5Ib',
+    'Alpha Aurigae': 'A7IV',
+    'Alpha Boötis': 'K2III',
+    'Alpha Camelopardalis': 'A3V',
+    'Alpha Carinae': 'F0Ia',
+    'Alpha Cephei': 'A7IV',
+    'Alpha Columbae': 'B5III',
+    'Alpha Crucis': 'B0.5IV',
+    'Alpha Eridani': 'K0III',
+    'Alpha Geminorum': 'A1V',
+    'Alpha Herculis': 'K3II',
+    'Alpha Leporis': 'B5V',
+    'Alpha Lupi': 'B1.5III',
+    'Alpha Ophiuchi': 'A5III',
+    'Alpha Pavonis': 'B2IV',
+    'Alpha Pegasi': 'B9III',
+    'Alpha Persei': 'F5Ib',
+}
+def map_star(star):
+    type = star_catalog.get(star, "Star not currently supported")
+    return type
+
+
```

### Comparing `astronomica-0.0.0/astronomica.egg-info/PKG-INFO` & `astronomica-0.0.1/astronomica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -69,16 +69,25 @@
 
 This method returns the current lunar phase
 
 ```python
 daysSinceJ2000()
 ```
 
+
 This method returns the days since Jan 1st 2000 Epoch
 
+```python
+sun = Sun(lat, long)
+sun.get_local_sunrise_time()
+sun.get_local_sunset_time()
+```
+
+These methods return the sunrise and sunset time
+
 
 ```python
 decimalHours(now) # now is the chosen time
 ```
 
 This method returns the decimal hours for a given time
 
@@ -96,14 +105,20 @@
 
 ```python
 azimuth(lat, long)
 ```
 
 This method returns the current solar azimuth in degrees for a given latitude and longitude <b>east</b>
 
+```python
+map_star(star)
+```
+
+This method returns the type of star based on its name. 
+
 ## Observer Class
 
 ```
 observer = Observer(lat, long, desired_planet_for_calculations, date=datetime.datetime.now())
 ```
 
 ### Methods in class
```

### Comparing `astronomica-0.0.0/setup.py` & `astronomica-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.0',
+    version='0.0.1',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/astronomica',
     project_urls = {
```

