# Comparing `tmp/pyastroweatherio-0.23.0.dev1.tar.gz` & `tmp/pyastroweatherio-0.23.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.23.0.dev1.tar", last modified: Mon Apr 10 15:32:10 2023, max compression
+gzip compressed data, was "pyastroweatherio-0.23.0.dev2.tar", last modified: Mon Apr 10 15:39:40 2023, max compression
```

## Comparing `pyastroweatherio-0.23.0.dev1.tar` & `pyastroweatherio-0.23.0.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/
--rw-r--r--   0 markus    (1000) markus    (1000)     1071 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev1/LICENSE
--rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     3076 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev1/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    24579 2023-04-10 15:28:51.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4473 2023-04-08 14:28:26.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-10 15:29:18.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/dataclasses.py
--rw-r--r--   0 markus    (1000) markus    (1000)      337 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    14814 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/top_level.txt
--rw-r--r--   0 markus    (1000) markus    (1000)       79 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1174 2023-04-10 15:32:07.000000 pyastroweatherio-0.23.0.dev1/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1071 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev2/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3076 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev2/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:39:40.051071 pyastroweatherio-0.23.0.dev2/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    24589 2023-04-10 15:39:21.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4473 2023-04-08 14:28:26.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-10 15:29:18.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/dataclasses.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      337 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    14814 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-10 15:39:40.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-10 15:39:39.000000 pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/top_level.txt
+-rw-r--r--   0 markus    (1000) markus    (1000)       79 2023-04-10 15:39:40.055071 pyastroweatherio-0.23.0.dev2/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1174 2023-04-10 15:39:35.000000 pyastroweatherio-0.23.0.dev2/setup.py
```

### Comparing `pyastroweatherio-0.23.0.dev1/LICENSE` & `pyastroweatherio-0.23.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev1/PKG-INFO` & `pyastroweatherio-0.23.0.dev2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.0.dev1
+Version: 0.23.0.dev2
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.23.0.dev1/README.md` & `pyastroweatherio-0.23.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev1/pyastroweatherio/client.py` & `pyastroweatherio-0.23.0.dev2/pyastroweatherio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                 "deepsky_forecast": await self._deepsky_forecast(),
             }
             # met.no
             if datetime.strptime(self._weather_data_met[met_index].get("time"), "%Y-%m-%dT%H:%M:%SZ") == forecast_time:
                 _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
                 datails = self._weather_data_met[met_index].get("data", {}).get("instant", {}).get("details", {})
                 # Overwrite cloudcover
-                item["cloudcover"] = datails.get("cloud_area_fraction", -1) / 12.5 + 1
+                item["cloudcover"] = int(datails.get("cloud_area_fraction", -1) / 12.5 + 1)
 
                 item["cloud_area_fraction"] = datails.get("cloud_area_fraction", -1)
                 item["cloud_area_fraction_high"] = datails.get("cloud_area_fraction_high", -1)
                 item["cloud_area_fraction_low"] = datails.get("cloud_area_fraction_low", -1)
                 item["cloud_area_fraction_medium"] = datails.get("cloud_area_fraction_medium", -1)
                 item["condition_percentage"] = await self.calc_condition_percentage(
                     item["cloud_area_fraction"] / 12.5 + 1,
@@ -273,15 +273,15 @@
                     "%Y-%m-%dT%H:%M:%SZ",
                 )
                 == forecast_time
             ):
                 _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
                 datails = self._weather_data_met[met_index + cnt].get("data", {}).get("instant", {}).get("details", {})
                 # Overwrite cloudcover
-                item["cloudcover"] = datails.get("cloud_area_fraction", -1) / 12.5 + 1
+                item["cloudcover"] = int(datails.get("cloud_area_fraction", -1) / 12.5 + 1)
 
                 item["cloud_area_fraction"] = datails.get("cloud_area_fraction", -1)
                 item["cloud_area_fraction_high"] = datails.get("cloud_area_fraction_high", -1)
                 item["cloud_area_fraction_low"] = datails.get("cloud_area_fraction_low", -1)
                 item["cloud_area_fraction_medium"] = datails.get("cloud_area_fraction_medium", -1)
                 item["condition_percentage"] = await self.calc_condition_percentage(
                     item["cloud_area_fraction"] / 12.5 + 1,
```

### Comparing `pyastroweatherio-0.23.0.dev1/pyastroweatherio/const.py` & `pyastroweatherio-0.23.0.dev2/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev1/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.23.0.dev2/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev1/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.23.0.dev2/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.23.0.dev2/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.23.0.dev1
+Version: 0.23.0.dev2
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.23.0.dev1/setup.py` & `pyastroweatherio-0.23.0.dev2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.23.0.dev1",
+    version="0.23.0.dev2",
     license="MIT",
     description="Python Wrapper for 7Timer REST API",
     long_description=" ".join(
         ["Lightweight Python 3 module to receive data via", "REST API from 7Timer."],
     ),
     author="Markus Winkler",
     author_email="winkler.info@icloud.com",
```

