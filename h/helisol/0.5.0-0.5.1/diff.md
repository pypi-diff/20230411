# Comparing `tmp/helisol-0.5.0.tar.gz` & `tmp/helisol-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\helisol-0.5.0.tar", last modified: Thu Mar 30 08:17:01 2023, max compression
+gzip compressed data, was "dist\helisol-0.5.1.tar", last modified: Tue Apr 11 10:14:56 2023, max compression
```

## Comparing `helisol-0.5.0.tar` & `helisol-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 08:17:01.921898 helisol-0.5.0/
--rw-rw-rw-   0        0        0       89 2023-03-29 14:23:27.000000 helisol-0.5.0/.gitignore
--rw-rw-rw-   0        0        0    19169 2023-03-29 16:48:06.000000 helisol-0.5.0/ExampleAnalemma.ipynb
--rw-rw-rw-   0        0        0    36121 2023-03-29 14:14:42.000000 helisol-0.5.0/ExampleShadow.ipynb
--rw-rw-rw-   0        0        0    35823 2021-01-25 16:42:42.000000 helisol-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      134 2023-03-29 14:24:01.000000 helisol-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11855 2023-03-30 08:17:01.922896 helisol-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     8477 2023-03-30 07:52:08.000000 helisol-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 08:17:01.733072 helisol-0.5.0/data/
--rw-rw-rw-   0        0        0     1861 2023-03-28 11:48:42.000000 helisol-0.5.0/data/Ephemerides_Aug2023.tsv
--rw-rw-rw-   0        0        0     1018 2023-03-28 11:48:42.000000 helisol-0.5.0/data/Ephemerides_March2023_47N_2E.tsv
-drwxrwxrwx   0        0        0        0 2023-03-30 08:17:01.806124 helisol-0.5.0/helisol/
--rw-rw-rw-   0        0        0     1492 2023-03-29 13:00:34.000000 helisol-0.5.0/helisol/__init__.py
--rw-rw-rw-   0        0        0     1329 2023-03-08 16:14:05.000000 helisol-0.5.0/helisol/__main__.py
--rw-rw-rw-   0        0        0      948 2023-03-28 11:46:18.000000 helisol-0.5.0/helisol/config.py
--rw-rw-rw-   0        0        0     6706 2023-03-30 07:32:40.000000 helisol-0.5.0/helisol/earth.py
--rw-rw-rw-   0        0        0    18760 2023-03-30 07:50:38.000000 helisol-0.5.0/helisol/general.py
--rw-rw-rw-   0        0        0     4282 2023-03-28 11:46:18.000000 helisol-0.5.0/helisol/locations.py
--rw-rw-rw-   0        0        0    15084 2023-03-29 14:10:38.000000 helisol-0.5.0/helisol/sun.py
--rw-rw-rw-   0        0        0     6939 2023-03-29 13:01:50.000000 helisol-0.5.0/helisol/tables.py
-drwxrwxrwx   0        0        0        0 2023-03-30 08:17:01.876690 helisol-0.5.0/helisol.egg-info/
--rw-rw-rw-   0        0        0    11855 2023-03-30 08:16:58.000000 helisol-0.5.0/helisol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-03-30 08:16:59.000000 helisol-0.5.0/helisol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 08:16:58.000000 helisol-0.5.0/helisol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-03-30 08:16:58.000000 helisol-0.5.0/helisol.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-30 08:16:58.000000 helisol-0.5.0/helisol.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 08:17:01.907068 helisol-0.5.0/locations/
--rw-rw-rw-   0        0        0      487 2023-03-28 11:46:18.000000 helisol-0.5.0/locations/global.json
--rw-rw-rw-   0        0        0     1107 2023-03-30 08:17:01.952965 helisol-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0       93 2021-01-01 10:57:17.000000 helisol-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 08:17:01.911057 helisol-0.5.0/tests/
--rw-rw-rw-   0        0        0     7114 2023-03-30 07:52:38.000000 helisol-0.5.0/tests/test_helisol.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:14:56.858271 helisol-0.5.1/
+-rw-rw-rw-   0        0        0       89 2023-03-29 14:23:27.000000 helisol-0.5.1/.gitignore
+-rw-rw-rw-   0        0        0    19169 2023-03-29 16:48:06.000000 helisol-0.5.1/ExampleAnalemma.ipynb
+-rw-rw-rw-   0        0        0    36121 2023-03-29 14:14:42.000000 helisol-0.5.1/ExampleShadow.ipynb
+-rw-rw-rw-   0        0        0    35823 2021-01-25 16:42:42.000000 helisol-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      134 2023-03-29 14:24:01.000000 helisol-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12156 2023-04-11 10:14:56.859267 helisol-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8746 2023-04-11 10:02:39.000000 helisol-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 10:14:56.717647 helisol-0.5.1/data/
+-rw-rw-rw-   0        0        0     1861 2023-03-28 11:48:42.000000 helisol-0.5.1/data/Ephemerides_Aug2023.tsv
+-rw-rw-rw-   0        0        0     1018 2023-03-28 11:48:42.000000 helisol-0.5.1/data/Ephemerides_March2023_47N_2E.tsv
+drwxrwxrwx   0        0        0        0 2023-04-11 10:14:56.803426 helisol-0.5.1/helisol/
+-rw-rw-rw-   0        0        0     1492 2023-03-29 13:00:34.000000 helisol-0.5.1/helisol/__init__.py
+-rw-rw-rw-   0        0        0     1329 2023-03-08 16:14:05.000000 helisol-0.5.1/helisol/__main__.py
+-rw-rw-rw-   0        0        0      948 2023-03-28 11:46:18.000000 helisol-0.5.1/helisol/config.py
+-rw-rw-rw-   0        0        0     9371 2023-04-11 09:52:00.000000 helisol-0.5.1/helisol/earth.py
+-rw-rw-rw-   0        0        0    18743 2023-03-30 11:40:25.000000 helisol-0.5.1/helisol/general.py
+-rw-rw-rw-   0        0        0     4282 2023-03-28 11:46:18.000000 helisol-0.5.1/helisol/locations.py
+-rw-rw-rw-   0        0        0    15084 2023-03-29 14:10:38.000000 helisol-0.5.1/helisol/sun.py
+-rw-rw-rw-   0        0        0     6939 2023-03-29 13:01:50.000000 helisol-0.5.1/helisol/tables.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:14:56.840318 helisol-0.5.1/helisol.egg-info/
+-rw-rw-rw-   0        0        0    12156 2023-04-11 10:14:55.000000 helisol-0.5.1/helisol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-04-11 10:14:55.000000 helisol-0.5.1/helisol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 10:14:55.000000 helisol-0.5.1/helisol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-11 10:14:55.000000 helisol-0.5.1/helisol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 10:14:55.000000 helisol-0.5.1/helisol.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 10:14:56.844308 helisol-0.5.1/locations/
+-rw-rw-rw-   0        0        0      487 2023-03-28 11:46:18.000000 helisol-0.5.1/locations/global.json
+-rw-rw-rw-   0        0        0     1107 2023-04-11 10:14:56.870275 helisol-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0       93 2021-01-01 10:57:17.000000 helisol-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 10:14:56.851312 helisol-0.5.1/tests/
+-rw-rw-rw-   0        0        0     7566 2023-04-11 10:08:19.000000 helisol-0.5.1/tests/test_helisol.py
```

### Comparing `helisol-0.5.0/ExampleAnalemma.ipynb` & `helisol-0.5.1/ExampleAnalemma.ipynb`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/ExampleShadow.ipynb` & `helisol-0.5.1/ExampleShadow.ipynb`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/LICENSE` & `helisol-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/PKG-INFO` & `helisol-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helisol
-Version: 0.5.0
+Version: 0.5.1
 Summary: Get precise position of sun in sky (height, azimuth) at given location and time, get sunrise and sunset time, generate sundials.
 Home-page: https://github.com/ovinc/helisol
 Author: Olivier Vincent
 Author-email: ovinc.py@gmail.com
 License: GNU GPLv3
 Description: # About
         
@@ -27,15 +27,15 @@
         
         - Sunset, sunrise and solar noon are within the displayed precision of each other (1 second for noon, 1 minute for sunset/sunrise)
         
         - Right ascension and equation of time are within the displayed precision of each other (1 second in time)
         
         - Declination deviates less than 2.5 arc-seconds (0.0007°, or 0.17 seconds in time).
         
-        - Sun to Earth distance deviates less than 1600 km.
+        - Sun to Earth distance deviates less than 1600 km; extracted aphelion and perihelion dates extracted from the extrema of this distance seem to be off by a few hours depending on the year.
         
         
         # Install
         
         ```bash
         pip install helisol
         ```
@@ -56,14 +56,18 @@
         earth = Earth('Sept. 9, 2003')
         
         # Update to current time
         earth.update()
         
         # Update to specific time
         earth.update(utc_time='2023-03-21, 12:00')
+        
+        # Min and max sun-eath distance
+        Earth(2019).orbit.perihelion()  # specific year
+        Earth().orbit.aphelion()        # current year
         ```
         
         
         ## Sun absolute position
         
         ```python
         from helisol import Sun
```

### Comparing `helisol-0.5.0/README.md` & `helisol-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 - Sunset, sunrise and solar noon are within the displayed precision of each other (1 second for noon, 1 minute for sunset/sunrise)
 
 - Right ascension and equation of time are within the displayed precision of each other (1 second in time)
 
 - Declination deviates less than 2.5 arc-seconds (0.0007°, or 0.17 seconds in time).
 
-- Sun to Earth distance deviates less than 1600 km.
+- Sun to Earth distance deviates less than 1600 km; extracted aphelion and perihelion dates extracted from the extrema of this distance seem to be off by a few hours depending on the year.
 
 
 # Install
 
 ```bash
 pip install helisol
 ```
@@ -48,14 +48,18 @@
 earth = Earth('Sept. 9, 2003')
 
 # Update to current time
 earth.update()
 
 # Update to specific time
 earth.update(utc_time='2023-03-21, 12:00')
+
+# Min and max sun-eath distance
+Earth(2019).orbit.perihelion()  # specific year
+Earth().orbit.aphelion()        # current year
 ```
 
 
 ## Sun absolute position
 
 ```python
 from helisol import Sun
```

### Comparing `helisol-0.5.0/data/Ephemerides_Aug2023.tsv` & `helisol-0.5.1/data/Ephemerides_Aug2023.tsv`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/data/Ephemerides_March2023_47N_2E.tsv` & `helisol-0.5.1/data/Ephemerides_March2023_47N_2E.tsv`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/helisol/__init__.py` & `helisol-0.5.1/helisol/__init__.py`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/helisol/__main__.py` & `helisol-0.5.1/helisol/__main__.py`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/helisol/config.py` & `helisol-0.5.1/helisol/config.py`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/helisol/earth.py` & `helisol-0.5.1/helisol/earth.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 from .general import sin, cos, tan
 
 
 perturb_planet_coeffs = CONSTANTS['planet perturbation coefficients']
 perturb_planet_longitude = CONSTANTS['planet perturbation longitude']
 perturb_planet_radius = CONSTANTS['planet perturbation radius']
 
+durations_fdays = {'day': 1,         # durations in fractions of days
+                   'hour': 1 / 24,
+                   'minute': 1 / (24 * 60),
+                   'second': 1 / (24 * 3600)}
+
+extrem_funcs = {'min': np.argmin, 'max': np.argmax}
+
 
 class EarthOrbit:
     """Store general characteristics of earth orbit"""
 
     def __init__(self, utc_time=None):
         """Init earth orbit object from specific date/time.
 
@@ -53,15 +60,16 @@
     def __repr__(self):
         year = self.time.utc.date().year
         return f'Earth Orbit in {year}'
 
     @property
     def excentricity(self):
         """Excentricity of earth's orbit"""
-        return 0.016709 - 0.000042 * self.time.julian_centuries
+        t = self.time.julian_centuries
+        return 0.016_708_634 - 0.000_042_037 * t - 0.000_000_1267 * t**2
 
     @property
     def axial_tilt(self):
         """Earth's axial tilt (epsilon)"""
         t = self.time.julian_centuries
         eps0 = AngleFromDegrees(23 + 26 / 60 + (21.5 - 46.8 * t) / 3600)
         d_eps = AngleFromSeconds(9.2 * cos(self.nutation))  # tilt nutation
@@ -116,14 +124,76 @@
         """Perturbations from planets, moon, etc. on earth-sun distance"""
         perturb = 0
         for coeff_name, (ampl, func) in perturb_planet_radius.items():
             ag = self.correc_planets_angle(coeff_name)
             perturb += ampl * getattr(ag, func)()
         return Distance(au=perturb)
 
+    @staticmethod
+    def _find_local_extremum(date_min, date_max, kind='min', resolution='hour'):
+        """Resolution can be day, hour, minute, second"""
+        t1 = Time(date_min)
+        t2 = Time(date_max)
+        fmin = t1.fraction_of_day
+        fmax = fmin + (t2.utc - t1.utc).total_seconds() / (3600 * 24)
+        df = durations_fdays[resolution]
+        ff = np.arange(fmin, fmax, df)
+        times = [Time(t1, fraction_of_day=f) for f in ff]
+        earths = [Earth(time) for time in times]
+        radii = np.array([earth.distance.au for earth in earths])
+        i0 = extrem_funcs[kind](radii)
+        return Time(date_min, fraction_of_day=ff[i0])
+
+    @classmethod
+    def _find_extremum(cls, year, kind='min', resolution='minute'):
+        """Find perigee or apogee.
+
+        Parameters
+        ----------
+        year is e.g. 2023
+        kind is 'min' or 'max'
+        resolution in ('day', 'hour', 'minute', 'second')
+        """
+        start_date = 'Jan 01'
+        date_min = f'{start_date}, {year}'
+        date_max = f'{start_date}, {year + 1}'
+
+        for res in 'day', 'hour', 'minute', 'second':
+            date = cls._find_local_extremum(date_min=date_min,
+                                            date_max=date_max,
+                                            kind=kind,
+                                            resolution=res)
+            if res == resolution:
+                return date
+            f = date.fraction_of_day
+            df = durations_fdays[res]
+            fmin, fmax = f - df, f + df
+            date_min = Time(date, fraction_of_day=fmin)
+            date_max = Time(date, fraction_of_day=fmax)
+
+    def perihelion(self, resolution='minute'):
+        """Minimum sun-earth distance.
+
+        Parameter
+        ---------
+        - resolution (str): 'day', 'hour', 'minute' (default) or 'second'
+        """
+        year = self.time.utc.year
+        return self._find_extremum(year, kind='min', resolution=resolution)
+
+    def aphelion(self, resolution='minute'):
+        """Maximum sun-earth distance.
+
+        Parameter
+        ---------
+        - resolution (str): 'day', 'hour', 'minute' (default) or 'second'
+        """
+        year = self.time.utc.year
+        return self._find_extremum(year, kind='max', resolution=resolution)
+
 
 class Earth:
 
     def __init__(self, utc_time=None):
         """Init earth object from specific date/time.
 
         Parameters
@@ -190,10 +260,10 @@
         Δplanets = self.orbit.correc_planets
         return λs + Δψ + Δaberr + Δplanets
 
     @property
     def distance(self):
         e = self.orbit.excentricity
         nu = self.true_anomaly
-        R = 1.0000002 * (1 - e**2) / (1 + e * cos(nu))
+        R = 1.000_001_018 * (1 - e**2) / (1 + e * cos(nu))
         ΔR = self.orbit.correc_planets_distance
         return Distance(au=R) + ΔR
```

### Comparing `helisol-0.5.0/helisol/general.py` & `helisol-0.5.1/helisol/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,32 +44,32 @@
 CONSTANTS['average motion coefficients'] = a
 CONSTANTS['nutation coefficients'] = (125.04, -1934.136)
 
 CONSTANTS['anomaly iterations'] = 3
 CONSTANTS['sunset iterations'] = 2
 
 
-perturb_planet_coeffs = {'A': (351.52, 22518.443),              # Venus 1
-                         'B': (253.14, 45036.886),              # Venus 2
-                         'C': (157.23, 32964.467),              # Jupiter
-                         'D': (297.85, 445267.112),   # Moon
-                         'E': (252.08, 20.190),                   # Long period
-                         'H': (353.40, 65928.7155)}              # H
+perturb_planet_coeffs = {'A': (351.52, 22518.4428),         # Venus 1
+                         'B': (253.14, 45036.8857),         # Venus 2
+                         'C': (157.23, 32964.4673),         # Jupiter
+                         'D': (297.85, 445267.1117),        # Moon
+                         'E': (252.08, 20.190),             # Long period
+                         'H': (42.43, 65928.9358)}          # H
 
 perturb_planet_longitude = {'A': (134e-5, 'cos'),
                             'B': (153e-5, 'cos'),
                             'C': (200e-5, 'cos'),
                             'D': (180e-5, 'sin'),
                             'E': (196e-5, 'sin')}
 
-perturb_planet_radius = {'A': (5.43e-6, 'sin'),
-                         'B': (15.75e-6, 'sin'),
-                         'C': (16.27e-6, 'sin'),
-                         'D': (30.76e-6, 'cos'),
-                         'H': (9.27e-6, 'sin')}
+perturb_planet_radius = {'A': (5.42e-6, 'sin'),
+                         'B': (15.76e-6, 'sin'),
+                         'C': (16.28e-6, 'sin'),
+                         'D': (30.84e-6, 'cos'),
+                         'H': (9.25e-6, 'sin')}
 
 CONSTANTS['planet perturbation coefficients'] = perturb_planet_coeffs
 CONSTANTS['planet perturbation longitude'] = perturb_planet_longitude
 CONSTANTS['planet perturbation radius'] = perturb_planet_radius
 
 astronomical_unit = 149_597_870_700  # in meters
```

### Comparing `helisol-0.5.0/helisol/locations.py` & `helisol-0.5.1/helisol/locations.py`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/helisol/sun.py` & `helisol-0.5.1/helisol/sun.py`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/helisol/tables.py` & `helisol-0.5.1/helisol/tables.py`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/helisol.egg-info/PKG-INFO` & `helisol-0.5.1/helisol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helisol
-Version: 0.5.0
+Version: 0.5.1
 Summary: Get precise position of sun in sky (height, azimuth) at given location and time, get sunrise and sunset time, generate sundials.
 Home-page: https://github.com/ovinc/helisol
 Author: Olivier Vincent
 Author-email: ovinc.py@gmail.com
 License: GNU GPLv3
 Description: # About
         
@@ -27,15 +27,15 @@
         
         - Sunset, sunrise and solar noon are within the displayed precision of each other (1 second for noon, 1 minute for sunset/sunrise)
         
         - Right ascension and equation of time are within the displayed precision of each other (1 second in time)
         
         - Declination deviates less than 2.5 arc-seconds (0.0007°, or 0.17 seconds in time).
         
-        - Sun to Earth distance deviates less than 1600 km.
+        - Sun to Earth distance deviates less than 1600 km; extracted aphelion and perihelion dates extracted from the extrema of this distance seem to be off by a few hours depending on the year.
         
         
         # Install
         
         ```bash
         pip install helisol
         ```
@@ -56,14 +56,18 @@
         earth = Earth('Sept. 9, 2003')
         
         # Update to current time
         earth.update()
         
         # Update to specific time
         earth.update(utc_time='2023-03-21, 12:00')
+        
+        # Min and max sun-eath distance
+        Earth(2019).orbit.perihelion()  # specific year
+        Earth().orbit.aphelion()        # current year
         ```
         
         
         ## Sun absolute position
         
         ```python
         from helisol import Sun
```

### Comparing `helisol-0.5.0/helisol.egg-info/SOURCES.txt` & `helisol-0.5.1/helisol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/setup.cfg` & `helisol-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `helisol-0.5.0/tests/test_helisol.py` & `helisol-0.5.1/tests/test_helisol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test helisol module with pytest"""
 
 from pathlib import Path
 import pandas as pd
 import numpy as np
 
 import helisol
-from helisol import Sun, Time, SunObservation, Distance, astronomical_unit
+from helisol import Earth, Sun, Time, SunObservation, Distance, astronomical_unit
 from helisol import Angle, AngleArray, AngleFromDegrees, AngleFromRadians
 from helisol import AngleFromMinutes, AngleFromSeconds
 from helisol import refraction
 
 DATA_FOLDER = Path(helisol.__file__).parent.parent / 'data'
 
 
@@ -62,14 +62,28 @@
 
 def test_distance():
     """Test Distance class"""
     d = Distance(au=1)
     assert round(d.km * 1000 / astronomical_unit, 6) == 1
 
 
+def test_aphelion():
+    """Test aphelion calculation from distance function"""
+    aph_time = Earth(2023).orbit.aphelion(resolution='hour')
+    assert aph_time.utc.month == 7
+    assert aph_time.utc.day == 6
+
+
+def test_perihelion():
+    """Test perihelion calculation from distance function"""
+    peri_time = Earth(2023).orbit.perihelion(resolution='hour')
+    assert peri_time.utc.month == 1
+    assert peri_time.utc.day == 4
+
+
 def test_sun():
     """Test sun object"""
     sun = Sun('Aug 10, 2023, 12:00')
     assert round(sun.declination.degrees, 1) == 15.6
     assert round(sun.equation_of_time.degrees, 1) == 1.4
     assert round(sun.right_ascension.degrees, 1) == 140.1
     assert round(sun.angular_diameter.degrees, 2) == 0.53
```

