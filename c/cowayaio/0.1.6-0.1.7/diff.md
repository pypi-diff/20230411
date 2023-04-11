# Comparing `tmp/cowayaio-0.1.6.tar.gz` & `tmp/cowayaio-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cowayaio-0.1.6.tar", last modified: Fri Dec 30 02:49:43 2022, max compression
+gzip compressed data, was "cowayaio-0.1.7.tar", last modified: Tue Apr 11 18:07:47 2023, max compression
```

## Comparing `cowayaio-0.1.6.tar` & `cowayaio-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2022-12-30 02:49:43.819941 cowayaio-0.1.6/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2022-12-30 02:45:16.000000 cowayaio-0.1.6/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2022-12-30 02:49:43.819607 cowayaio-0.1.6/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       92 2022-12-30 02:45:16.000000 cowayaio-0.1.6/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2022-12-30 02:49:43.817251 cowayaio-0.1.6/cowayaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      523 2022-12-30 02:45:16.000000 cowayaio-0.1.6/cowayaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      984 2022-12-30 02:45:16.000000 cowayaio-0.1.6/cowayaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    18497 2022-12-30 02:45:16.000000 cowayaio-0.1.6/cowayaio/coway_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      663 2022-12-30 02:45:16.000000 cowayaio-0.1.6/cowayaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1016 2022-12-30 02:45:16.000000 cowayaio-0.1.6/cowayaio/purifier_model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2022-12-30 02:45:16.000000 cowayaio-0.1.6/cowayaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2022-12-30 02:49:43.819060 cowayaio-0.1.6/cowayaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2022-12-30 02:49:43.000000 cowayaio-0.1.6/cowayaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      324 2022-12-30 02:49:43.000000 cowayaio-0.1.6/cowayaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2022-12-30 02:49:43.000000 cowayaio-0.1.6/cowayaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2022-12-30 02:49:43.000000 cowayaio-0.1.6/cowayaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        9 2022-12-30 02:49:43.000000 cowayaio-0.1.6/cowayaio.egg-info/top_level.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2022-12-30 02:49:43.820104 cowayaio-0.1.6/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      985 2022-12-30 02:45:16.000000 cowayaio-0.1.6/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-04-11 18:07:47.991161 cowayaio-0.1.7/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-04-11 18:04:59.000000 cowayaio-0.1.7/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2023-04-11 18:07:47.990826 cowayaio-0.1.7/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       92 2023-04-11 18:04:59.000000 cowayaio-0.1.7/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-04-11 18:07:47.988431 cowayaio-0.1.7/cowayaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      523 2023-04-11 18:04:59.000000 cowayaio-0.1.7/cowayaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      984 2023-04-11 18:04:59.000000 cowayaio-0.1.7/cowayaio/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    19131 2023-04-11 18:04:59.000000 cowayaio-0.1.7/cowayaio/coway_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      663 2023-04-11 18:04:59.000000 cowayaio-0.1.7/cowayaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1016 2023-04-11 18:04:59.000000 cowayaio-0.1.7/cowayaio/purifier_model.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-04-11 18:04:59.000000 cowayaio-0.1.7/cowayaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-04-11 18:07:47.990305 cowayaio-0.1.7/cowayaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2023-04-11 18:07:47.000000 cowayaio-0.1.7/cowayaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      324 2023-04-11 18:07:47.000000 cowayaio-0.1.7/cowayaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-04-11 18:07:47.000000 cowayaio-0.1.7/cowayaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-04-11 18:07:47.000000 cowayaio-0.1.7/cowayaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        9 2023-04-11 18:07:47.000000 cowayaio-0.1.7/cowayaio.egg-info/top_level.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-04-11 18:07:47.991279 cowayaio-0.1.7/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      985 2023-04-11 18:04:59.000000 cowayaio-0.1.7/setup.py
```

### Comparing `cowayaio-0.1.6/LICENSE` & `cowayaio-0.1.7/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 RobertD502
+Copyright (c) 2023 RobertD502
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cowayaio-0.1.6/PKG-INFO` & `cowayaio-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowayaio
-Version: 0.1.6
+Version: 0.1.7
 Summary: A asynchronous python library for Coway Air Purifiers 
 Home-page: https://github.com/RobertD502/cowayaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/cowayaio/issues
 Project-URL: Source, https://github.com/RobertD502/cowayaio/
```

### Comparing `cowayaio-0.1.6/cowayaio/__init__.py` & `cowayaio-0.1.7/cowayaio/__init__.py`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.6/cowayaio/constants.py` & `cowayaio-0.1.7/cowayaio/constants.py`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.6/cowayaio/coway_client.py` & `cowayaio-0.1.7/cowayaio/coway_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,15 +231,19 @@
         """Return MCU version for a single purifier."""
 
         params = {
             'deviceId': device_attr['device_id'],
         }
 
         response = await self._post_endpoint(Endpoint_JSON.MCU_VERSION, params)
-        return response['body']
+        try:
+            mcu_version = response['body']
+        except KeyError:
+            raise CowayError(f'Coway API error: Coway server failed to return purifier MCU version.')
+        return mcu_version
 
     async def async_get_control_status(self, device_attr: dict[str, Any]) -> tuple[dict, bool]:
         """Returns power state, mode, speed, etc. for a single purifier."""
 
         params = {
             'barcode': device_attr['device_id'],
             'dvcBrandCd': device_attr['device_brand'],
@@ -247,15 +251,20 @@
             'stationCd': '',
             'resetDttm': '',
             'dvcTypeCd': device_attr['device_type'],
             'refreshFlag': 'true'
         }
 
         response = await self._post_endpoint(Endpoint_JSON.STATUS, params)
-        return response['body']['controlStatus'], response['body']['netStatus']
+        try:
+            control_status = response['body']['controlStatus']
+            net_status = response['body']['netStatus']
+        except KeyError:
+            raise CowayError(f'Coway API error: Coway server failed to return purifier control status.')
+        return control_status, net_status
 
     async def async_get_quality_status(self, device_attr: dict[str, Any]) -> tuple[list, list, list]:
         """Returns data for prefilter, max2 filter, and air quality sensors."""
 
         params = {
             'barcode': device_attr['device_id'],
             'dvcBrandCd': device_attr['device_brand'],
@@ -263,15 +272,21 @@
             'stationCd': '',
             'resetDttm': '',
             'dvcTypeCd': device_attr['device_type'],
             'refreshFlag': 'true'
         }
 
         response = await self._post_endpoint(Endpoint_JSON.FILTERS, params)
-        return response['body']['filterList'], response['body']['prodStatus'], response['body']['IAQ']
+        try:
+            filter_list = response['body']['filterList']
+            prod_status = response['body']['prodStatus']
+            iaq = response['body']['IAQ']
+        except KeyError:
+            raise CowayError(f'Coway API error: Coway server failed to return purifier quality status.')
+        return filter_list, prod_status, iaq
 
 
     """
     **************************************************************************************************************************************************
 
                                                             Functions for controlling purifiers
 
@@ -295,15 +310,15 @@
         await self.async_control_purifier(device_attr, '0002', '2')
 
     async def async_set_eco_mode(self, device_attr: dict[str, str]) -> None:
         """Set Purifier to Eco Mode.
         Only applies to AIRMEGA AP-1512HHS models.
         """
 
-        await self.async_control_purifier(device_attr, '0002', '6')        
+        await self.async_control_purifier(device_attr, '0002', '6')
 
     async def async_set_fan_speed(self, device_attr: dict[str, str], speed: str) -> None:
         """Speed can be 1, 2, or 3 represented as a string."""
 
         await self.async_control_purifier(device_attr, '0003', speed)
 
     async def async_set_light(self, device_attr: dict[str, str], light_on: bool) -> None:
```

### Comparing `cowayaio-0.1.6/cowayaio/exceptions.py` & `cowayaio-0.1.7/cowayaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.6/cowayaio/purifier_model.py` & `cowayaio-0.1.7/cowayaio/purifier_model.py`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.6/cowayaio/str_enum.py` & `cowayaio-0.1.7/cowayaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.6/cowayaio.egg-info/PKG-INFO` & `cowayaio-0.1.7/cowayaio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowayaio
-Version: 0.1.6
+Version: 0.1.7
 Summary: A asynchronous python library for Coway Air Purifiers 
 Home-page: https://github.com/RobertD502/cowayaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/cowayaio/issues
 Project-URL: Source, https://github.com/RobertD502/cowayaio/
```

### Comparing `cowayaio-0.1.6/setup.py` & `cowayaio-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cowayaio",
-    version="0.1.6",
+    version="0.1.7",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="A asynchronous python library for Coway Air Purifiers ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/cowayaio',
     keywords='coway, iocare, iocare api, coway api, airmega',
```

