# Comparing `tmp/astronomica-0.0.2.tar.gz` & `tmp/astronomica-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomica-0.0.2.tar", last modified: Tue Apr 11 02:49:24 2023, max compression
+gzip compressed data, was "astronomica-0.0.3.tar", last modified: Tue Apr 11 17:05:59 2023, max compression
```

## Comparing `astronomica-0.0.2.tar` & `astronomica-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:49:24.288350 astronomica-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 02:49:12.000000 astronomica-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 02:49:24.288350 astronomica-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-11 02:49:12.000000 astronomica-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:49:24.288350 astronomica-0.0.2/astronomica/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 02:49:12.000000 astronomica-0.0.2/astronomica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-04-11 02:49:12.000000 astronomica-0.0.2/astronomica/astronomica.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 02:49:12.000000 astronomica-0.0.2/astronomica/suntiming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:49:24.288350 astronomica-0.0.2/astronomica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 02:49:24.000000 astronomica-0.0.2/astronomica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:49:24.288350 astronomica-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-11 02:49:12.000000 astronomica-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:05:59.636388 astronomica-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 17:05:47.000000 astronomica-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-11 17:05:59.636388 astronomica-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-11 17:05:47.000000 astronomica-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:05:59.632388 astronomica-0.0.3/astronomica/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 17:05:47.000000 astronomica-0.0.3/astronomica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-11 17:05:47.000000 astronomica-0.0.3/astronomica/astronomica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-11 17:05:47.000000 astronomica-0.0.3/astronomica/suntiming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:05:59.636388 astronomica-0.0.3/astronomica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 17:05:59.000000 astronomica-0.0.3/astronomica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:05:59.636388 astronomica-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 17:05:47.000000 astronomica-0.0.3/setup.py
```

### Comparing `astronomica-0.0.2/LICENSE` & `astronomica-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.2/PKG-INFO` & `astronomica-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -69,17 +69,24 @@
 
 This method returns the current lunar phase
 
 ```python
 daysSinceJ2000()
 ```
 
-
 This method returns the days since Jan 1st 2000 Epoch
 
+
+```python
+definition_of(word)
+```
+
+This method returns the definition of an astronomy word for amateurs who are confused on what something means.
+
+
 ```python
 sun = Sun(lat, long)
 sun.get_local_sunrise_time()
 sun.get_local_sunset_time()
 ```
 
 These methods return the sunrise and sunset time
```

### Comparing `astronomica-0.0.2/README.md` & `astronomica-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,24 @@
 
 This method returns the current lunar phase
 
 ```python
 daysSinceJ2000()
 ```
 
-
 This method returns the days since Jan 1st 2000 Epoch
 
+
+```python
+definition_of(word)
+```
+
+This method returns the definition of an astronomy word for amateurs who are confused on what something means.
+
+
 ```python
 sun = Sun(lat, long)
 sun.get_local_sunrise_time()
 sun.get_local_sunset_time()
 ```
 
 These methods return the sunrise and sunset time
```

### Comparing `astronomica-0.0.2/astronomica/astronomica.py` & `astronomica-0.0.3/astronomica/astronomica.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 # import required libraries (math and datetime are always required, because of their uses)
 import math
 import datetime
 from astroquery.simbad import Simbad
+import requests
 
 class LST:
     def __init__(self, data):
         self.__dict__ = data
 
+
+def definition_of(word):
+    # make a request to the Wikipedia API
+    response = requests.get(f"https://en.wikipedia.org/api/rest_v1/page/summary/{word}")
+    # check if the request was successful
+    if response.status_code != 200:
+        return "Sorry, I could not find information on that word."
+    # extract the summary text from the response
+    summary = response.json()['extract']
+    return summary
+
+
 def get_object_equatorial_coords(obj_name):
     """
     :param obj_name: name of the SIMBAD object
     :return: the RA and declination of the object
     """
     # Query the SIMBAD database for the object
     result_table = Simbad.query_object(obj_name)
     # Extract the RA and Dec coordinates from the result table
     ra = result_table['RA'][0]
     dec = result_table['DEC'][0]
     # Return the RA and Dec coordinates as floats
     return ra, dec
 
+
 def get_spectral_info(obj_name):
     """
     Query the SIMBAD database for spectral information on the given object.
 
     :param obj_name: Name or identifier of the object.
     :return: A dictionary with the spectral information for the object.
     """
@@ -51,19 +65,22 @@
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() is not None else 0  # Convert to minutes
     return (time / 86400000) - (tzoffset / 1440) + 2440587.5  # return the Julian Date
 
 
 J1970 = 2440588
 dayMs = 24 * 60 * 60 * 1000
 
+
 def fromJulian(j):
     return datetime.datetime.fromtimestamp((j + 0.5 - J1970) * dayMs / 1000)
 
+
 LUNAR_MONTH = 29.530588853
 
+
 def get_lunar_age():
     percent = get_lunar_age_percent()
     age = percent * LUNAR_MONTH
     return age
 
 
 def get_lunar_age_percent():
@@ -94,14 +111,15 @@
         return "Waning Gibbous"
     elif age < 23.99361:
         return "Last Quarter"
     elif age < 27.68493:
         return "Waning Crescent"
     return "New"
 
+
 def solarMeanAnomaly(d):
     rad = math.pi / 180.0
     return rad * (357.5291 + 0.98560028 * d)
 
 
 def daysSinceJ2000():
     # get current date and time in UTC
@@ -122,14 +140,15 @@
     JD = 367 * Y - math.floor(7 * (Y + math.floor((M + 9) / 12)) / 4) + math.floor(
         275 * M / 9) + D + 1721013.5 + UT / 24
 
     # calculate number of days since J2000.0
     days = (JD - 2451545.0) + (UT - 12) / 24
     return days
 
+
 def declination(l, b):
     e = math.radians(23.4397)  # obliquity of the ecliptic in degrees
     return math.asin(
         math.sin(math.radians(b)) * math.cos(e) + math.cos(math.radians(b)) * math.sin(e) * math.sin(math.radians(l)))
 
 
 def sign(x):
@@ -196,14 +215,15 @@
     PI = math.pi
 
     C = rad * (1.9148 * math.sin(M) + 0.02 * math.sin(2 * M) + 0.0003 * math.sin(3 * M))  # equation of center
     P = rad * 102.9372  # perihelion of the Earth
 
     return M + C + P + PI
 
+
 def solarHourAngle(longitude, lst):
     """Calculate the solar hour angle for a given longitude and local sidereal time."""
     # Convert longitude and LST to radians
     longitude = math.radians(longitude)
     lst = math.radians(lst)
     # Calculate the solar noon for the given longitude
     solarNoon = longitude + (12 - 12 * 4.0 / 1440) * math.radians(360) / 24
@@ -273,15 +293,15 @@
             'mars': 3,
             'jupiter': 4,
             'saturn': 5,
             'uranus': 6,
             'neptune': 7,
             'pluto': 8,
         }
-        plan_number = planetMap.get(self.planet, 2) # if the planet is not found, calculate for earth
+        plan_number = planetMap.get(self.planet, 2)  # if the planet is not found, calculate for earth
         m_row = m_list[plan_number]
         M = (m_row[0] + m_row[1] * (local_julian_date() - J2000)) % 360
         self.meanA = M
         return M
 
     def equation_of_center(self):
         planet = self.planet
@@ -297,35 +317,35 @@
             "pluto": [28.3150, 4.3408, 0.9214, 0.2235, 0.0627, 0.0174]  # 0.0096 is the maximum error
         }
         # the formula used is from https://www.aa.quae.nl/en/reken/zonpositie.html#10
         # c = c1 * sin(m) + c2 * sin(2m) + c3 * sin(3m) + c4 * sin(4m) + c5 * sin(5m) + c6 * sin(6m)
         c = c_dict.get(planet, [1.9148, 0.0200, 0.0003, 0, 0, 0])
         m = self.mean_anomaly()
         center_eq = c[0] * math.sin(m) + c[1] * math.sin(2 * m) + c[2] * math.sin(3 * m) + c[3] * math.sin(4 * m) + \
-                    c[4] * math.sin(5 * m) + c[5] * math.sin(6 * m)
+            c[4] * math.sin(5 * m) + c[5] * math.sin(6 * m)
         self.ceq = center_eq
         return center_eq
 
     def true_anomaly(self):
         c = self.equation_of_center()
         m = self.mean_anomaly()
         self.v = c + m
         return m + c
 
     def set_perihelion_and_obliquity(self):
-        perihelion_longitude_and_obliquity= [
-            (230.3265,0.0351),
-             (73.7576,2.6376),
-              (102.9373,23.4393),
-               (71.0041,25.1918),
-                (237.1015,3.1189),
-                 (99.4587,26.7285),
-                  (5.4634,82.2298),
-                   (182.2100,27.8477),
-                    (184.5484,119.6075),
+        perihelion_longitude_and_obliquity = [
+            (230.3265, 0.0351),
+            (73.7576, 2.6376),
+            (102.9373, 23.4393),
+            (71.0041, 25.1918),
+            (237.1015, 3.1189),
+            (99.4587, 26.7285),
+            (5.4634, 82.2298),
+            (182.2100, 27.8477),
+            (184.5484, 119.6075),
         ]
         planetMap = {
             'mercury': 0,
             'venus': 1,
             'earth': 2,
             'mars': 3,
             'jupiter': 4,
@@ -336,15 +356,15 @@
         }
         key = planetMap.get(self.planet, 2)
         datatuple = perihelion_longitude_and_obliquity[key]
         self.perihelion = datatuple[0]
         self.obliquity = math.radians(datatuple[1])
 
     def ecliptical_longitude(self):
-        self.set_perihelion_and_obliquity() # setup information
+        self.set_perihelion_and_obliquity()  # setup information
         peri = self.perihelion
         L = self.mean_anomaly() + peri
         Lsun = L + 180
         long = (Lsun + self.equation_of_center()) % 360
         self.eclipticlong = math.radians(long)
         return math.radians(long)
 
@@ -355,23 +375,23 @@
         return {
             'ra': math.degrees(asun),
             'dec': math.degrees(decsun)
         }
 
     def local_solar_transit(self):
         Jtable = [
-            [45.3497, 11.4556, 0,175.9386],
+            [45.3497, 11.4556, 0, 175.9386],
             [52.1268, -0.2516, 0.0099, -116.7505],
             [0.0009, 0.0053, -0.0068, 1.0000000],
             [0.9047, 0.0305, -0.0082, 1.027491],
-            [0.3345, 0.0064, 0,0.4135778],
+            [0.3345, 0.0064, 0, 0.4135778],
             [0.0766, 0.0078, -0.0040, 0.4440276],
             [0.1260, -0.0106, 0.0850, -0.7183165],
             [0.3841, 0.0019, -0.0066, 0.6712575],
-            [4.5635,-0.5024, 0.3429, 6.387672]
+            [4.5635, -0.5024, 0.3429, 6.387672]
         ]
         planetMap = {
             'mercury': 0,
             'venus': 1,
             'earth': 2,
             'mars': 3,
             'jupiter': 4,
@@ -382,17 +402,17 @@
         }
         plannumber = planetMap.get(self.planet, 2)
         Jrow = Jtable[plannumber]
         j0 = Jrow[0]
         j1 = Jrow[1]
         j2 = Jrow[2]
         j3 = Jrow[3]
-        nx = (local_julian_date() - 2451545 -j0)/j3 - self.long /360
+        nx = (local_julian_date() - 2451545 - j0) / j3 - self.long / 360
         n = math.floor(nx)
-        jx = local_julian_date() + j3 * (n-nx)
+        jx = local_julian_date() + j3 * (n - nx)
         self.set_perihelion_and_obliquity()  # setup information
         peri = self.perihelion
         L = self.mean_anomaly() + peri
         lsun = L + 180
         jtransit = jx + j1 * math.sin(math.radians(self.mean_anomaly())) + j2 * math.sin(2 * math.radians(lsun))
         return jtransit + 1
 
@@ -429,15 +449,15 @@
             'uranus': 6,
             'neptune': 7,
             'pluto': 8,
         }
         key = planetMap.get(self.planet, 2)
         e = e_table[key]
         square = square_table[key]
-        r = square/1 + e * math.cos(self.true_anomaly())
+        r = square / 1 + e * math.cos(self.true_anomaly())
         self.dist = r
         return r
 
     def planet_heliocentric_coordinates(self):
         square_table = [
             0.37073,
             0.72330,
@@ -508,18 +528,30 @@
         key = planetMap.get(self.planet, 2)
         i = i_table[key]
         horse = horse_table[key]
         w = w_table[key]
         v = self.true_anomaly()
         r = self.distance_to_sun()
         xplanet = r * (math.cos(horse) * math.cos(w + v) - math.sin(horse) * math.cos(i) * math.sin(w + v))
-        yplanet = r * (math.sin(horse)*math.cos(w + v) + math.cos(horse ) *math.cos(i) * math.sin(w + v))
+        yplanet = r * (math.sin(horse) * math.cos(w + v) + math.cos(horse) * math.cos(i) * math.sin(w + v))
         zplanet = r * math.sin(i) * math.sin(w + v)
         return xplanet, yplanet, zplanet
 
+    def planet_geocentric_coordinates(self):
+        earth = Observer(self.lat, self.long, 'earth')
+        x, y, z = earth.planet_heliocentric_coordinates()
+        xplanet, yplanet, zplanet = self.planet_heliocentric_coordinates()
+        return xplanet - x, yplanet - y, zplanet - z
+
+    def planet_geocentric_lat_long(self):
+        x, y, z = self.planet_geocentric_coordinates()
+        change = math.sqrt((x ** 2) + (y ** 2) + (z**2))
+        long = math.atan2(y, x)
+        lat = math.asin(z/change)
+        return lat, long
 
 
 star_catalog = {
     'Sun': 'G2V',
     'Sirius': 'A1V',
     'Betelgeuse': 'M2Iab',
     'Rigel': 'B8Ia',
@@ -550,16 +582,14 @@
     'Hadar': 'B1IV',
     'Miaplacidus': 'A0III',
     'Naos': 'O5If',
     'Rigil Kentaurus': 'G2V+K1V',
     'Sadr': 'F8Ib',
     'Shaula': 'B0.5IV-V',
     'Suhail': 'K4Ib-II',
-    'Vega': 'A0Va',
-    'Achernar': 'B3Vpe',
     'Adhara': 'B2II',
     'Albireo A': 'K3II-III',
     'Albireo B': 'B8V',
     'Alcor': 'A5V',
     'Alioth': 'A0p',
     'Alkaid': 'B3V',
     'Alnath': 'B7III',
@@ -578,12 +608,14 @@
     'Alpha Leporis': 'B5V',
     'Alpha Lupi': 'B1.5III',
     'Alpha Ophiuchi': 'A5III',
     'Alpha Pavonis': 'B2IV',
     'Alpha Pegasi': 'B9III',
     'Alpha Persei': 'F5Ib',
 }
+
+
 def map_star(star):
     type = star_catalog.get(star, "Star not currently supported")
     return type
 
-    
+
```

### Comparing `astronomica-0.0.2/astronomica/suntiming.py` & `astronomica-0.0.3/astronomica/suntiming.py`

 * *Files identical despite different names*

### Comparing `astronomica-0.0.2/astronomica.egg-info/PKG-INFO` & `astronomica-0.0.3/astronomica.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomica
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library that deals with astronomy and mathematical calculations. It also helps with Julian Dates
 Home-page: https://github.com/PyndyalaCoder/astronomica
 Author: Siddhu Pendyala
 Author-email: elcientifico.pendyala@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PyndyalaCoder/astronomica/issues
 Description-Content-Type: text/markdown
@@ -69,17 +69,24 @@
 
 This method returns the current lunar phase
 
 ```python
 daysSinceJ2000()
 ```
 
-
 This method returns the days since Jan 1st 2000 Epoch
 
+
+```python
+definition_of(word)
+```
+
+This method returns the definition of an astronomy word for amateurs who are confused on what something means.
+
+
 ```python
 sun = Sun(lat, long)
 sun.get_local_sunrise_time()
 sun.get_local_sunset_time()
 ```
 
 These methods return the sunrise and sunset time
```

### Comparing `astronomica-0.0.2/setup.py` & `astronomica-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='astronomica',
-    version='0.0.2',
+    version='0.0.3',
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
-    install_requires=['astroquery'],
+    install_requires=['astroquery', 'requests'],
 )
```

