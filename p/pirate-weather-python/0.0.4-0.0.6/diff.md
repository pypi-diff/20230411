# Comparing `tmp/pirate-weather-python-0.0.4.tar.gz` & `tmp/pirate-weather-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pirate-weather-python-0.0.4.tar", last modified: Thu Apr  6 11:20:45 2023, max compression
+gzip compressed data, was "dist/pirate-weather-python-0.0.6.tar", last modified: Tue Apr 11 12:45:29 2023, max compression
```

## Comparing `pirate-weather-python-0.0.4.tar` & `pirate-weather-python-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather/types/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/types/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/types/languages.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/types/units.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/types/weather.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7966 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1476 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4395 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/forecast.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1698 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/request_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      494 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/pirate_weather/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      661 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       45 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/pirate_weather_python.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6488 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/tests/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      332 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/tests/mokcs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1654 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/tests/test_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5224 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/tests/test_forecast.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      316 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/tests/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4450 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2023-04-06 11:20:43.000000 pirate-weather-python-0.0.4/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-06 11:20:45.000000 pirate-weather-python-0.0.4/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather/types/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/types/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/types/languages.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/types/units.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/types/weather.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7966 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1476 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      283 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4318 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/forecast.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1698 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/request_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      494 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/pirate_weather/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather_python.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      661 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       45 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/pirate_weather_python.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6488 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/tests/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      332 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/tests/mokcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1654 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/tests/test_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5224 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/tests/test_forecast.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      316 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/tests/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4450 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2023-04-11 12:45:26.000000 pirate-weather-python-0.0.6/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-11 12:45:28.000000 pirate-weather-python-0.0.6/setup.cfg
```

### Comparing `pirate-weather-python-0.0.4/pirate_weather/types/languages.py` & `pirate-weather-python-0.0.6/pirate_weather/types/languages.py`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/pirate_weather/api.py` & `pirate-weather-python-0.0.6/pirate_weather/api.py`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/pirate_weather/base.py` & `pirate-weather-python-0.0.6/pirate_weather/base.py`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/pirate_weather/forecast.py` & `pirate-weather-python-0.0.6/pirate_weather/forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from datetime import datetime
 from typing import List
 
 from . import base
 
 
 class CurrentlyForecast(base.AutoInit):
-    time: datetime
+    time: int
     summary: str = None
     icon: str
     nearest_storm_distance: int
     nearest_storm_bearing: int
     precip_intensity: float
     precip_intensity_error: float
     precip_probability: float
@@ -26,28 +25,28 @@
     cloud_cover: float
     uv_index: int
     visibility: float
     ozone: float
 
 
 class MinutelyForecastItem(base.AutoInit):
-    time: datetime
+    time: int
     precip_intensity: float
     precip_intensity_error: float
     precip_probability: float
     precip_type: str
 
 
 class MinutelyForecast(base.BaseWeather):
     data: List[MinutelyForecastItem]
     data_class = MinutelyForecastItem
 
 
 class HourlyForecastItem(base.AutoInit):
-    time: datetime
+    time: int
     summary: str = None
     icon: str
     precip_intensity: float
     precip_probability: float
     precip_type: str
     precipAccumulation: float
     temperature: float
@@ -66,67 +65,67 @@
 
 class HourlyForecast(base.BaseWeather):
     data: List[HourlyForecastItem]
     data_class = HourlyForecastItem
 
 
 class DailyForecastItem(base.AutoInit):
-    time: datetime
+    time: int
     summary: str = None
     icon: str
-    sunrise_time: datetime
-    sunset_time: datetime
+    sunrise_time: int
+    sunset_time: int
     moon_phase: float
     precip_intensity: float
     precip_intensity_max: float
-    precip_intensity_max_time: datetime
+    precip_intensity_max_time: int
     precip_probability: float
     precip_type: str
     precipAccumulation: float
     temperature_high: float
-    temperature_high_time: datetime
+    temperature_high_time: int
     temperature_low: float
-    temperature_low_time: datetime
+    temperature_low_time: int
     apparent_temperature_high: float
-    apparent_temperature_high_time: datetime
+    apparent_temperature_high_time: int
     apparent_temperature_low: float
-    apparent_temperature_low_time: datetime
+    apparent_temperature_low_time: int
     dew_point: float
     humidity: float
     pressure: float
     wind_speed: float
     wind_gust: float
-    wind_gust_time: datetime
+    wind_gust_time: int
     wind_bearing: int
     cloud_cover: float
     uv_index: int
-    uv_index_time: datetime
+    uv_index_time: int
     visibility: int
     ozone: float
     temperature_min: float
-    temperature_min_time: datetime
+    temperature_min_time: int
     temperature_max: float
-    temperature_max_time: datetime
+    temperature_max_time: int
     apparent_temperature_min: float
-    apparent_temperature_min_time: datetime
+    apparent_temperature_min_time: int
     apparent_temperature_max: float
-    apparent_temperature_max_time: datetime
+    apparent_temperature_max_time: int
 
 
 class DailyForecast(base.BaseWeather):
     data: List[DailyForecastItem]
     data_class = DailyForecastItem
 
 
 class Alert(base.AutoInit):
     title: str
     regions: list
     severity: str
-    time: datetime
-    expires: datetime
+    time: int
+    expires: int
     description: str
     uri: str
 
 
 class Flags(base.AutoInit):
     sources: List[str]
     sources_class = str
@@ -144,26 +143,26 @@
     hourly: HourlyForecast
     daily: DailyForecast
     alerts: List[Alert]
     flags: Flags
     offset: int
 
     def __init__(
-        self,
-        latitude: float,
-        longitude: float,
-        timezone: str,
-        currently: dict = None,
-        minutely: dict = None,
-        hourly: dict = None,
-        daily: dict = None,
-        alerts: [dict] = None,
-        flags: dict = None,
-        offset: int = None,
-        elevation: int = None,
+            self,
+            latitude: float,
+            longitude: float,
+            timezone: str,
+            currently: dict = None,
+            minutely: dict = None,
+            hourly: dict = None,
+            daily: dict = None,
+            alerts: [dict] = None,
+            flags: dict = None,
+            offset: int = None,
+            elevation: int = None,
     ):
         self.latitude = latitude
         self.longitude = longitude
         self.timezone = timezone
 
         self.currently = CurrentlyForecast(
             timezone=timezone, **(currently or {}))
```

### Comparing `pirate-weather-python-0.0.4/pirate_weather/request_manager.py` & `pirate-weather-python-0.0.6/pirate_weather/request_manager.py`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/pirate_weather_python.egg-info/PKG-INFO` & `pirate-weather-python-0.0.6/pirate_weather_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pirate-weather-python
-Version: 0.0.4
+Version: 0.0.6
 Summary: The Pirate Weather API wrapper
 Home-page: https://github.com/bakobako/pirate-weather-python
 Author: bakobako
 Author-email: adam.bako@keboola.com
 License: GPLv3 License
-Download-URL: https://github.com/bakobako/pirate-weather-python/archive/0.0.4.tar.gz
+Download-URL: https://github.com/bakobako/pirate-weather-python/archive/0.0.6.tar.gz
 Description: View on github
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pirate-weather-python-0.0.4/pirate_weather_python.egg-info/SOURCES.txt` & `pirate-weather-python-0.0.6/pirate_weather_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/tests/data.py` & `pirate-weather-python-0.0.6/tests/data.py`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/tests/test_base.py` & `pirate-weather-python-0.0.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/tests/test_forecast.py` & `pirate-weather-python-0.0.6/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/README.md` & `pirate-weather-python-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pirate-weather-python-0.0.4/setup.py` & `pirate-weather-python-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import find_packages, setup
 
-__version__ = "0.0.4"
+__version__ = "0.0.6"
 
 
 with open(os.path.join(
         os.path.abspath(os.path.dirname(__file__)), "README.md")
 ) as f:
     README = f.read()
```

### Comparing `pirate-weather-python-0.0.4/PKG-INFO` & `pirate-weather-python-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pirate-weather-python
-Version: 0.0.4
+Version: 0.0.6
 Summary: The Pirate Weather API wrapper
 Home-page: https://github.com/bakobako/pirate-weather-python
 Author: bakobako
 Author-email: adam.bako@keboola.com
 License: GPLv3 License
-Download-URL: https://github.com/bakobako/pirate-weather-python/archive/0.0.4.tar.gz
+Download-URL: https://github.com/bakobako/pirate-weather-python/archive/0.0.6.tar.gz
 Description: View on github
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

