# Comparing `tmp/pyastroweatherio-0.23.0.dev2.tar.gz` & `tmp/pyastroweatherio-0.23.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.23.0.dev2.tar", last modified: Mon Apr 10 15:39:40 2023, max compression
+gzip compressed data, was "pyastroweatherio-0.23.0.dev3.tar", last modified: Tue Apr 11 11:27:34 2023, max compression
```

## Comparing `pyastroweatherio-0.23.0.dev2.tar` & `pyastroweatherio-0.23.0.dev3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/
--rw-r--r--   0 markus    (1000) markus    (1000)     1071 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev2/LICENSE
--rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     3076 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev2/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:39:40.051071 pyastroweatherio-0.23.0.dev2/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    24589 2023-04-10 15:39:21.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4473 2023-04-08 14:28:26.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-10 15:29:18.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/dataclasses.py
--rw-r--r--   0 markus    (1000) markus    (1000)      337 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    14814 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-10 15:39:40.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/top_level.txt
--rw-r--r--   0 markus    (1000) markus    (1000)       79 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1174 2023-04-10 15:39:35.000000 pyastroweatherio-0.23.0.dev2/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.0.dev3/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3538 2023-04-10 18:28:08.000000 pyastroweatherio-0.23.0.dev3/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-11 11:27:34.575760 pyastroweatherio-0.23.0.dev3/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    25576 2023-04-11 11:25:21.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4473 2023-04-08 14:28:26.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-10 15:29:18.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-04-10 18:40:11.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    14262 2023-04-10 18:34:19.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-11 11:27:34.000000 pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2023-04-11 11:27:34.583760 pyastroweatherio-0.23.0.dev3/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1174 2023-04-11 11:26:18.000000 pyastroweatherio-0.23.0.dev3/setup.py
```

### Comparing `pyastroweatherio-0.23.0.dev2/LICENSE` & `pyastroweatherio-0.23.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev2/PKG-INFO` & `pyastroweatherio-0.23.0.dev3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.0.dev2
+Version: 0.23.0.dev3
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.23.0.dev2/README.md` & `pyastroweatherio-0.23.0.dev3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pyAstroWeatherIO
 
-Wrapper for the 7Timer AstroWeather REST API. Designed to work with Home Assistant and the custom [AstroWeather](https://github.com/mawinkler/astroweather) integration.
+Wrapper for the ***7Timer*** and ***MET Norway Weather*** REST API. Designed to work with Home Assistant and the custom [AstroWeather](https://github.com/mawinkler/astroweather) integration.
 
-This module communicates with the API endpoint of 7Timer ([documentation](http://www.7timer.info/doc.php)). It retrieves current weather data for astronomical observations:
+This module communicates with the API endpoint of ***7Timer*** ([documentation](http://www.7timer.info/doc.php)) and ***MET Norway Weather*** ([documentation](https://api.met.no/weatherapi/locationforecast/2.0/documentation)). It retrieves current weather data for astronomical observations:
+
+***7Timer***
 
 Observation | Range | Meaning
 ----------- | ----- | -------
 **Cloud Cover** | 1 to 9 | 1 = <6% to 9 = >94%
 **Lifted Index** | -10 to 15 | -10 = <-7 to 15 = >11
 **Seeing** | 1 to 8 | 1 = <0.5" to 8 = >2.5"
 **Transparency** | 1 to 8 | 1 = <0.3 to 8 = >1
@@ -27,14 +29,25 @@
 || lightsnowday, lightsnownight | Precipitation rate less than 4mm/hr
 || rainday, rainnight | Precipitation rate over 4mm/hr
 || snowday, snownight | Precipitation rate over 4mm/hr
 || rainsnowday, rainsnownight | Precipitation type to be ice pellets or freezing rain
 
 For astronimical observations, the lower the values are the better it is (besides 2m temperature).
 
+***MET Norway Weather***
+
+Observation | Range
+----------- | -----
+**Cloud Area Fraction** | 0% to 100%
+**Cloud Area Fraction High** | 0% to 100%
+**Cloud Area Fraction Medium** | 0% to 100%
+**Cloud Area Fraction Low** | 0% to 100%
+
+The Cloud Area Fraction of Met Norway supersedes Cloud Cover of 7Timer currently.
+
 In addition to the weather data, some calculations for the astronomical twilight and Moon setting, rising and phase are implemented. They indicate the darkness you can expect the upcoming night.
 
 ## Functions
 
 The module exposes the following function:
 
 ### AstroWeather(latitude, longitude, elevation)
@@ -64,9 +77,9 @@
 **transparency_weight**
 
 (int)(Optional) Seeing weight for condition calculation, default=1
 
 ## Setup
 
 ```sh
-pip3 install . --user
+pip3 install .
 ```
```

### Comparing `pyastroweatherio-0.23.0.dev2/pyastroweatherio/client.py` & `pyastroweatherio-0.23.0.dev3/pyastroweatherio/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Define a client to interact with 7Timer."""
 import asyncio
 import json
 import logging
 from datetime import datetime, timedelta
 from typing import Optional
+from decimal import Decimal
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientError
-from decimal import Decimal
 
 from pyastroweatherio.const import (
     BASE_URL_SEVENTIMER,
     BASE_URL_MET,
     DEFAULT_TIMEOUT,
     DEFAULT_CACHE_TIMEOUT,
     DEFAULT_ELEVATION,
     DEFAULT_TIMEZONE,
     DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
     DEFAULT_CONDITION_SEEING_WEIGHT,
     DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
     HOME_LATITUDE,
     HOME_LONGITUDE,
     STIMER_OUTPUT,
-    FORECAST_TYPE_DAILY,
+    # FORECAST_TYPE_DAILY,
     FORECAST_TYPE_HOURLY,
     MAGNUS_COEFFICIENT_A,
     MAGNUS_COEFFICIENT_B,
 )
 from pyastroweatherio.dataclasses import (
     ForecastData,
     LocationData,
@@ -46,29 +46,31 @@
         latitude=HOME_LATITUDE,
         longitude=HOME_LONGITUDE,
         elevation=DEFAULT_ELEVATION,
         timezone_info=DEFAULT_TIMEZONE,
         cloudcover_weight=DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
         seeing_weight=DEFAULT_CONDITION_SEEING_WEIGHT,
         transparency_weight=DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
+        metno_enabled=True,
     ):
         self._session: ClientSession = session
         self._latitude = latitude
         self._longitude = longitude
         self._elevation = elevation
         self._timezone_info = timezone_info
         self._weather_data_seventimer = []
         self._weather_data_seventimer_init = ""
-        self._weather_data_met = []
-        self._weather_data_met_init = ""
+        self._weather_data_metno = []
+        self._weather_data_metno_init = ""
         self._weather_data_seventimer_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
-        self._weather_data_met_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
+        self._weather_data_metno_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._cloudcover_weight = cloudcover_weight
         self._seeing_weight = seeing_weight
         self._transparency_weight = transparency_weight
+        self._metno_enabled = metno_enabled
         self.req = session
 
     # Public functions
     async def get_location_data(
         self,
     ) -> None:
         """Returns station Weather Forecast."""
@@ -95,38 +97,40 @@
     async def _get_location_data(self) -> None:
         """Return Forecast data"""
 
         cnv = ConversionFunctions()
         items = []
 
         await self.retrieve_data_seventimer()
-        await self.retrieve_data_met()
+        if self._metno_enabled:
+            await self.retrieve_data_metno()
         now = datetime.utcnow()
 
         # Anchor timestamp
         init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
-        # met.no
-        met_index = -1
+        # Met.no
+        metno_index = -1
         forecast_skipped = 0
         for row in self._weather_data_seventimer:
-            # Skip over past forecasts
+            # 7Timer: Skip over past forecasts
             forecast_time = init_ts + timedelta(hours=row["timepoint"])
             if now > forecast_time:
                 forecast_skipped += 1
                 continue
 
-            _LOGGER.debug("forecast_time: %s", str(forecast_time))
+            _LOGGER.debug("7Timer forecast time: %s", str(forecast_time))
 
-            # met.no
-            for datapoint in self._weather_data_met:
-                met_index = met_index + 1
-                if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
-                    break
-            _LOGGER.debug("met start index: %s", str(met_index))
+            # Met.no: Search for 7Timer forecast time
+            if self._metno_enabled:
+                for datapoint in self._weather_data_metno:
+                    metno_index += 1
+                    if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+                        break
+                _LOGGER.debug("Met.no start index: %s", str(metno_index))
 
             # Astro Routines
             astro_routines = AstronomicalRoutines(
                 self._latitude,
                 self._longitude,
                 self._elevation,
                 self._timezone_info,
@@ -165,36 +169,45 @@
                 "moon_next_setting": await astro_routines.moon_next_setting(),
                 "moon_phase": await astro_routines.moon_phase(),
                 "moon_altitude": await astro_routines.moon_altitude(),
                 "moon_azimuth": await astro_routines.moon_azimuth(),
                 "weather": row.get("weather", ""),
                 "deepsky_forecast": await self._deepsky_forecast(),
             }
-            # met.no
-            if datetime.strptime(self._weather_data_met[met_index].get("time"), "%Y-%m-%dT%H:%M:%SZ") == forecast_time:
-                _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
-                datails = self._weather_data_met[met_index].get("data", {}).get("instant", {}).get("details", {})
+            # Met.no
+            if (
+                self._metno_enabled
+                and datetime.strptime(
+                    self._weather_data_metno[metno_index].get("time"),
+                    "%Y-%m-%dT%H:%M:%SZ",
+                )
+                == forecast_time
+            ):
+                # _LOGGER.debug("Met.no Cloud Area Fraction timestamp match: %s", str(forecast_time))
+                datails = self._weather_data_metno[metno_index].get("data", {}).get("instant", {}).get("details", {})
                 # Overwrite cloudcover
                 item["cloudcover"] = int(datails.get("cloud_area_fraction", -1) / 12.5 + 1)
 
                 item["cloud_area_fraction"] = datails.get("cloud_area_fraction", -1)
                 item["cloud_area_fraction_high"] = datails.get("cloud_area_fraction_high", -1)
                 item["cloud_area_fraction_low"] = datails.get("cloud_area_fraction_low", -1)
                 item["cloud_area_fraction_medium"] = datails.get("cloud_area_fraction_medium", -1)
+
                 item["condition_percentage"] = await self.calc_condition_percentage(
                     item["cloud_area_fraction"] / 12.5 + 1,
                     row["seeing"],
                     row["transparency"],
                 )
             else:
-                _LOGGER.debug("No Cloud Area Fraction for: %s", str(forecast_time))
+                # _LOGGER.debug("Met.no no Cloud Area Fraction for: %s", str(forecast_time))
                 item["cloud_area_fraction"] = None
                 item["cloud_area_fraction_high"] = None
                 item["cloud_area_fraction_low"] = None
                 item["cloud_area_fraction_medium"] = None
+
                 item["condition_percentage"] = await self.calc_condition_percentage(
                     row["cloudcover"], row["seeing"], row["transparency"]
                 )
 
             items.append(LocationData(item))
             break
 
@@ -203,15 +216,16 @@
     async def _forecast_data(self, forecast_type, hours_to_show) -> None:
         """Return Forecast data for the Station."""
 
         cnv = ConversionFunctions()
         items = []
 
         await self.retrieve_data_seventimer()
-        await self.retrieve_data_met()
+        if self._metno_enabled:
+            await self.retrieve_data_metno()
         now = datetime.utcnow()
 
         # Create items
         cnt = 0
 
         # Anchor timestamp
         init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
@@ -220,28 +234,30 @@
         astro_routines = AstronomicalRoutines(
             self._latitude, self._longitude, self._elevation, self._timezone_info, now
         )
         utc_to_local_diff = astro_routines.utc_to_local_diff()
         _LOGGER.debug("UTC to local diff: %s", str(utc_to_local_diff))
         _LOGGER.debug("Forecast length: %s", str(len(self._weather_data_seventimer)))
 
-        met_index = -1
+        # Met.no
+        metno_index = -1
         for row in self._weather_data_seventimer:
-            # Skip over past forecasts
+            # 7Timer: Skip over past forecasts
             forecast_time = init_ts + timedelta(hours=row["timepoint"])
             if now > forecast_time:
                 continue
 
-            # met.no
-            if met_index == -1:
-                for datapoint in self._weather_data_met:
-                    met_index = met_index + 1
-                    if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
-                        break
-                _LOGGER.debug("met start index: %s", str(met_index))
+            # Met.no: Search for 7Timer forecast time
+            if self._metno_enabled:
+                if metno_index == -1:
+                    for datapoint in self._weather_data_metno:
+                        metno_index += 1
+                        if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+                            break
+                    _LOGGER.debug("Met.no start index: %s", str(metno_index))
 
             # Hour of day needs to be in local time
             hour_of_day = (forecast_time.hour + utc_to_local_diff) % 24
 
             cloudcover = row["cloudcover"]
             seeing = row["seeing"]
             transparency = row["transparency"]
@@ -262,61 +278,68 @@
                 "rh2m": row["rh2m"],
                 "wind10m": row["wind10m"],
                 "temp2m": row["temp2m"],
                 "dewpoint2m": await self.calc_dewpoint2m(row["rh2m"], row["temp2m"]),
                 "prec_type": row["prec_type"],
                 "weather": row.get("weather", ""),
             }
-            # met.no
+            # Met.no
             if (
-                datetime.strptime(
-                    self._weather_data_met[met_index + cnt].get("time"),
+                self._metno_enabled
+                and datetime.strptime(
+                    self._weather_data_metno[metno_index + cnt].get("time"),
                     "%Y-%m-%dT%H:%M:%SZ",
                 )
                 == forecast_time
             ):
-                _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
-                datails = self._weather_data_met[met_index + cnt].get("data", {}).get("instant", {}).get("details", {})
+                # _LOGGER.debug("Met.no Cloud Area Fraction timestamp match: %s", str(forecast_time))
+                datails = (
+                    self._weather_data_metno[metno_index + cnt].get("data", {}).get("instant", {}).get("details", {})
+                )
                 # Overwrite cloudcover
                 item["cloudcover"] = int(datails.get("cloud_area_fraction", -1) / 12.5 + 1)
 
                 item["cloud_area_fraction"] = datails.get("cloud_area_fraction", -1)
                 item["cloud_area_fraction_high"] = datails.get("cloud_area_fraction_high", -1)
                 item["cloud_area_fraction_low"] = datails.get("cloud_area_fraction_low", -1)
                 item["cloud_area_fraction_medium"] = datails.get("cloud_area_fraction_medium", -1)
+
                 item["condition_percentage"] = await self.calc_condition_percentage(
                     item["cloud_area_fraction"] / 12.5 + 1,
                     row["seeing"],
                     row["transparency"],
                 )
             else:
-                _LOGGER.debug("No Cloud Area Fraction for: %s", str(forecast_time))
+                # _LOGGER.debug("Met.no no Cloud Area Fraction for: %s", str(forecast_time))
                 item["cloud_area_fraction"] = None
                 item["cloud_area_fraction_high"] = None
                 item["cloud_area_fraction_low"] = None
                 item["cloud_area_fraction_medium"] = None
+
                 item["condition_percentage"] = await self.calc_condition_percentage(
                     row["cloudcover"], row["seeing"], row["transparency"]
                 )
             items.append(ForecastData(item))
+
             # Limit number of Hours
             cnt += 3
             if cnt >= hours_to_show:
                 break
 
         return items
 
     async def _deepsky_forecast(self):
         """Return Deepsky Forecast data"""
 
         cnv = ConversionFunctions()
         items = []
 
         await self.retrieve_data_seventimer()
-        await self.retrieve_data_met()
+        if self._metno_enabled:
+            await self.retrieve_data_metno()
         now = datetime.utcnow()
 
         # Create items
         cnt = 0
 
         # Anchor timestamp
         init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
@@ -329,27 +352,29 @@
 
         # Create forecast
         forecast_dayname = ""
         start_forecast_hour = 0
         start_weather = ""
         interval_points = []
 
-        met_index = -1
+        # Met.no
+        metno_index = -1
         for row in self._weather_data_seventimer:
             # Skip over past forecasts
             forecast_time = init_ts + timedelta(hours=row["timepoint"])
             if now > forecast_time:
                 continue
 
-            # met.no
-            if met_index == -1:
-                for datapoint in self._weather_data_met:
-                    met_index = met_index + 1
-                    if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
-                        break
+            # Met.no
+            if self._metno_enabled:
+                if metno_index == -1:
+                    for datapoint in self._weather_data_metno:
+                        metno_index += 1
+                        if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+                            break
 
             # Hour of day needs to be in local time
             hour_of_day = (forecast_time.hour + utc_to_local_diff) % 24
 
             # Skip daytime, we're only interested in the forecasts in
             # between 9pm to 3am.
             # Possible timestamps within the data:
@@ -364,36 +389,39 @@
                 cnt += 3
                 continue
 
             cloudcover = row["cloudcover"]
             seeing = row["seeing"]
             transparency = row["transparency"]
             cloud_area_fraction = 0
-            # met.no
+            # Met.no
             if (
-                datetime.strptime(
-                    self._weather_data_met[met_index + cnt].get("time"),
+                self._metno_enabled
+                and datetime.strptime(
+                    self._weather_data_metno[metno_index + cnt].get("time"),
                     "%Y-%m-%dT%H:%M:%SZ",
                 )
                 == forecast_time
             ):
-                # met.no
-                _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
-                datails = self._weather_data_met[met_index + cnt].get("data", {}).get("instant", {}).get("details", {})
+                # Met.no
+                # _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
+                datails = (
+                    self._weather_data_metno[metno_index + cnt].get("data", {}).get("instant", {}).get("details", {})
+                )
                 cloud_area_fraction = datails.get("cloud_area_fraction") / 12.5 + 1
-            else:
-                _LOGGER.debug("No Cloud Area Fraction for: %s", str(forecast_time))
+            # else:
+            #     _LOGGER.debug("No Cloud Area Fraction for: %s", str(forecast_time))
 
             if len(interval_points) == 0:
                 forecast_dayname = forecast_time.strftime("%A")
                 start_forecast_hour = hour_of_day
                 start_weather = row.get("weather", "")
 
             # Calculate Condition
-            if cloud_area_fraction > 0:
+            if self._metno_enabled and cloud_area_fraction > 0:
                 interval_points.append(await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency))
             else:
                 interval_points.append(await self.calc_condition_percentage(cloudcover, seeing, transparency))
 
             if len(interval_points) == 3:
                 item = {
                     "init": init_ts,
@@ -437,24 +465,24 @@
                 + self._seeing_weight * 8
                 + self._transparency_weight * 8
                 - self._cloudcover_weight
                 - self._seeing_weight
                 - self._transparency_weight
             )
         )
-        _LOGGER.debug(
-            "Calc condition cloudcover: %d(%d), seeing %d(%d), transparency: %d(%d), condition %d",
-            cloudcover,
-            self._cloudcover_weight,
-            seeing,
-            self._seeing_weight,
-            transparency,
-            self._transparency_weight,
-            condition,
-        )
+        # _LOGGER.debug(
+        #     "Calc condition cloudcover: %d(%d), seeing %d(%d), transparency: %d(%d), condition %d",
+        #     cloudcover,
+        #     self._cloudcover_weight,
+        #     seeing,
+        #     self._seeing_weight,
+        #     transparency,
+        #     self._transparency_weight,
+        #     condition,
+        # )
         return condition
 
     async def calc_dewpoint2m(self, rh2m, temp2m):
         """Calculate 2m Dew Point."""
         # α(T,RH) = ln(RH/100) + aT/(b+T)
         # Ts = (b × α(T,RH)) / (a - α(T,RH))
         alpha = float(Decimal(str(rh2m / 100)).ln()) + MAGNUS_COEFFICIENT_A * temp2m / (MAGNUS_COEFFICIENT_B + temp2m)
@@ -463,15 +491,15 @@
         return dewpoint
 
     async def retrieve_data_seventimer(self):
         """Retrieves current data from 7timer"""
 
         if ((datetime.now() - self._weather_data_seventimer_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
             self._weather_data_seventimer_timestamp = datetime.now()
-            _LOGGER.debug("Updating data")
+            _LOGGER.debug("Updating data from 7Timer")
 
             # Testing
             # json_data_astro = {"init": "2022060906"}
             # with open("astro.json") as json_file:
             #     astro_dataseries = json.load(json_file).get("dataseries", {})
             # with open("civil.json") as json_file:
             #     civil_dataseries = json.load(json_file).get("dataseries", {})
@@ -487,15 +515,15 @@
                 if astro["timepoint"] == civil["timepoint"]:
                     astro["weather"] = civil["weather"]
                     astro["rh2m"] = int(civil["rh2m"].replace("%", ""))
 
             self._weather_data_seventimer = astro_dataseries
             self._weather_data_seventimer_init = json_data_astro.get("init")
         else:
-            _LOGGER.debug("Using cached data")
+            _LOGGER.debug("Using cached data for 7Timer")
 
     async def async_request_seventimer(self, product="astro", method="get") -> dict:
         """Make a request against the 7timer API."""
 
         use_running_session = self._session and not self._session.closed
 
         if use_running_session:
@@ -528,61 +556,60 @@
                 # Testing
                 # json_string = json.dumps(data)
                 # with open(product + ".json", "w") as outfile:
                 #     outfile.write(json_string)
                 # /Testing
 
                 return data
-        except asyncio.TimeoutError:
-            raise RequestError("Request to endpoint timed out")
+        except asyncio.TimeoutError as tex:
+            raise RequestError(f"Request to endpoint timed out: {tex}") from None
         except ClientError as err:
             raise RequestError(f"Error requesting data: {err}") from None
 
         finally:
             if not use_running_session:
                 await session.close()
 
-    async def retrieve_data_met(self):
+    async def retrieve_data_metno(self):
         """Retrieves current data from met"""
 
-        if ((datetime.now() - self._weather_data_met_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
-            self._weather_data_met_timestamp = datetime.now()
-            _LOGGER.debug("Updating data")
+        if ((datetime.now() - self._weather_data_metno_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
+            self._weather_data_metno_timestamp = datetime.now()
+            _LOGGER.debug("Updating data from Met.no")
 
             # Testing
             # json_data_astro = {"init": "2022060906"}
             # with open("astro.json") as json_file:
             #     astro_dataseries = json.load(json_file).get("dataseries", {})
             # with open("civil.json") as json_file:
             #     civil_dataseries = json.load(json_file).get("dataseries", {})
             # -Testing
-            json_data_met = await self.async_request_met("met", "get")
+            json_data_metno = await self.async_request_met("met", "get")
 
-            dataseries = json_data_met.get("properties", {}).get("timeseries", [])
+            dataseries = json_data_metno.get("properties", {}).get("timeseries", [])
             # /Testing
 
-            self._weather_data_met = dataseries
-            self._weather_data_met_init = dataseries[0].get("time", None)
+            self._weather_data_metno = dataseries
+            self._weather_data_metno_init = dataseries[0].get("time", None)
         else:
-            _LOGGER.debug("Using cached data")
+            _LOGGER.debug("Using cached data for Met.no")
 
     async def async_request_met(self, product="met", method="get") -> dict:
         """Make a request against the 7timer API."""
 
         use_running_session = self._session and not self._session.closed
 
         if use_running_session:
             session = self._session
         else:
             session = ClientSession(
                 timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
             )
 
         # BASE_URL_MET = "https://api.met.no/weatherapi/locationforecast/2.0/complete?altitude=XX&lat=XX.XX&lon=XX.XX"
-        # STIMER_OUTPUT = "json"
         url = (
             str(f"{BASE_URL_MET}")
             + "?lon="
             + str("%.1f" % round(self._longitude, 2))
             + "&lat="
             + str("%.1f" % round(self._latitude, 2))
             + "&altitude="
@@ -599,15 +626,15 @@
                 # Testing
                 # json_string = json.dumps(data)
                 # with open(product + ".json", "w") as outfile:
                 #     outfile.write(json_string)
                 # /Testing
 
                 return data
-        except asyncio.TimeoutError:
-            raise RequestError("Request to endpoint timed out")
+        except asyncio.TimeoutError as tex:
+            raise RequestError(f"Request to endpoint timed out: {tex}") from None
         except ClientError as err:
             raise RequestError(f"Error requesting data: {err}") from None
 
         finally:
             if not use_running_session:
                 await session.close()
```

### Comparing `pyastroweatherio-0.23.0.dev2/pyastroweatherio/const.py` & `pyastroweatherio-0.23.0.dev3/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev2/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.23.0.dev3/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev2/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.23.0.dev3/pyastroweatherio/helper_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -142,17 +142,15 @@
             end = self._sun_observer.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer.date = timestamp
                 try:
                     self._sun_next_rising_astro = self.utc_to_local(
-                        self._sun_observer.next_rising(
-                            ephem.Sun(), use_center=True
-                        ).datetime()
+                        self._sun_observer.next_rising(ephem.Sun(), use_center=True).datetime()
                     )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
             self._sun_next_setting = self.utc_to_local(
@@ -164,121 +162,103 @@
             end = self._sun_observer.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer.date = timestamp
                 try:
                     self._sun_next_setting_astro = self.utc_to_local(
-                        self._sun_observer.next_setting(
-                            ephem.Sun(), use_center=True
-                        ).datetime()
+                        self._sun_observer.next_setting(ephem.Sun(), use_center=True).datetime()
                     )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         # Rise and Setting (Nautical)
         self._sun_observer_nautical.date = self.utc_to_local(self._forecast_time)
         self._sun.compute(self._sun_observer_nautical)
 
         try:
             self._sun_next_rising_nautical = self.utc_to_local(
-                self._sun_observer_nautical.next_rising(
-                    ephem.Sun(), use_center=True
-                ).datetime()
+                self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True).datetime()
             )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical rising
             start = self._sun_observer_nautical.date.datetime()
             end = self._sun_observer_nautical.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_nautical.date = timestamp
                 try:
                     self._sun_next_rising_nautical = self.utc_to_local(
-                        self._sun_observer_nautical.next_rising(
-                            ephem.Sun(), use_center=True
-                        ).datetime()
+                        self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True).datetime()
                     )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
             self._sun_next_setting_nautical = self.utc_to_local(
-                self._sun_observer_nautical.next_setting(
-                    ephem.Sun(), use_center=True
-                ).datetime()
+                self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True).datetime()
             )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical setting
             start = self._sun_observer_nautical.date.datetime()
             end = self._sun_observer_nautical.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_nautical.date = timestamp
                 try:
                     self._sun_next_setting_nautical = self.utc_to_local(
-                        self._sun_observer_nautical.next_setting(
-                            ephem.Sun(), use_center=True
-                        ).datetime()
+                        self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True).datetime()
                     )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         # Rise and Setting (Astronomical)
         self._sun_observer_astro.date = self.utc_to_local(self._forecast_time)
         self._sun.compute(self._sun_observer_astro)
 
         try:
             self._sun_next_rising_astro = self.utc_to_local(
-                self._sun_observer_astro.next_rising(
-                    ephem.Sun(), use_center=True
-                ).datetime()
+                self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True).datetime()
             )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical rising
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
                     self._sun_next_rising_astro = self.utc_to_local(
-                        self._sun_observer_astro.next_rising(
-                            ephem.Sun(), use_center=True
-                        ).datetime()
+                        self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True).datetime()
                     )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
             self._sun_next_setting_astro = self.utc_to_local(
-                self._sun_observer_astro.next_setting(
-                    ephem.Sun(), use_center=True
-                ).datetime()
+                self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True).datetime()
             )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical setting
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
                     self._sun_next_setting_astro = self.utc_to_local(
-                        self._sun_observer_astro.next_setting(
-                            ephem.Sun(), use_center=True
-                        ).datetime()
+                        self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True).datetime()
                     )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
     def calculate_moon(self):
         """Calculates moon rising and setting"""
@@ -296,26 +276,22 @@
 
         # Rise and Setting
         self._moon_observer.date = self._forecast_time
         self._moon.compute(self._moon_observer)
 
         try:
             self._moon_next_rising = self.utc_to_local(
-                self._moon_observer.next_rising(
-                    ephem.Moon(), use_center=True
-                ).datetime()
+                self._moon_observer.next_rising(ephem.Moon(), use_center=True).datetime()
             )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         try:
             self._moon_next_setting = self.utc_to_local(
-                self._moon_observer.next_setting(
-                    ephem.Moon(), use_center=True
-                ).datetime()
+                self._moon_observer.next_setting(ephem.Moon(), use_center=True).datetime()
             )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
     async def sun_next_rising(self) -> datetime:
         """Returns sun next rising"""
         if self._sun_next_rising is not None:
```

### Comparing `pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.23.0.dev3/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.0.dev2
+Version: 0.23.0.dev3
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.23.0.dev2/setup.py` & `pyastroweatherio-0.23.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.23.0.dev2",
+    version="0.23.0.dev3",
     license="MIT",
     description="Python Wrapper for 7Timer REST API",
     long_description=" ".join(
         ["Lightweight Python 3 module to receive data via", "REST API from 7Timer."],
     ),
     author="Markus Winkler",
     author_email="winkler.info@icloud.com",
```

