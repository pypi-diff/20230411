# Comparing `tmp/requests-toolkit-stable-0.9.1.tar.gz` & `tmp/requests-toolkit-stable-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-toolkit-stable-0.9.1.tar", last modified: Fri Oct 28 20:29:00 2022, max compression
+gzip compressed data, was "requests-toolkit-stable-0.9.2.tar", last modified: Sat Oct 29 05:08:13 2022, max compression
```

## Comparing `requests-toolkit-stable-0.9.1.tar` & `requests-toolkit-stable-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 leoxiang  (1000) leoxiang  (1000)        0 2022-10-28 20:29:00.578080 requests-toolkit-stable-0.9.1/
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1066 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.1/LICENSE
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1977 2022-10-28 20:29:00.578080 requests-toolkit-stable-0.9.1/PKG-INFO
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1559 2022-10-28 13:27:52.000000 requests-toolkit-stable-0.9.1/README.md
-drwxrwxr-x   0 leoxiang  (1000) leoxiang  (1000)        0 2022-10-28 20:29:00.578080 requests-toolkit-stable-0.9.1/requests_toolkit/
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      268 2022-10-28 14:00:35.000000 requests-toolkit-stable-0.9.1/requests_toolkit/__init__.py
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     4242 2022-10-26 07:30:01.000000 requests-toolkit-stable-0.9.1/requests_toolkit/_academic.py
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     3586 2022-10-28 19:53:09.000000 requests-toolkit-stable-0.9.1/requests_toolkit/_air_quality.py
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      903 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.1/requests_toolkit/_thesis_info.py
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1355 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.1/requests_toolkit/_weather_query.py
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1734 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.1/requests_toolkit/_ytb_channel_info.py
-drwxrwxr-x   0 leoxiang  (1000) leoxiang  (1000)        0 2022-10-28 20:29:00.578080 requests-toolkit-stable-0.9.1/requests_toolkit_stable.egg-info/
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1977 2022-10-28 20:29:00.000000 requests-toolkit-stable-0.9.1/requests_toolkit_stable.egg-info/PKG-INFO
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      458 2022-10-28 20:29:00.000000 requests-toolkit-stable-0.9.1/requests_toolkit_stable.egg-info/SOURCES.txt
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)        1 2022-10-28 20:29:00.000000 requests-toolkit-stable-0.9.1/requests_toolkit_stable.egg-info/dependency_links.txt
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)       29 2022-10-28 20:29:00.000000 requests-toolkit-stable-0.9.1/requests_toolkit_stable.egg-info/requires.txt
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)       17 2022-10-28 20:29:00.000000 requests-toolkit-stable-0.9.1/requests_toolkit_stable.egg-info/top_level.txt
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)       38 2022-10-28 20:29:00.578080 requests-toolkit-stable-0.9.1/setup.cfg
--rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      719 2022-10-28 20:28:36.000000 requests-toolkit-stable-0.9.1/setup.py
+drwxrwxr-x   0 leoxiang  (1000) leoxiang  (1000)        0 2022-10-29 05:08:13.846225 requests-toolkit-stable-0.9.2/
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1066 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.2/LICENSE
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1977 2022-10-29 05:08:13.846225 requests-toolkit-stable-0.9.2/PKG-INFO
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1559 2022-10-28 13:27:52.000000 requests-toolkit-stable-0.9.2/README.md
+drwxrwxr-x   0 leoxiang  (1000) leoxiang  (1000)        0 2022-10-29 05:08:13.842224 requests-toolkit-stable-0.9.2/requests_toolkit/
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      268 2022-10-28 14:00:35.000000 requests-toolkit-stable-0.9.2/requests_toolkit/__init__.py
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     4242 2022-10-26 07:30:01.000000 requests-toolkit-stable-0.9.2/requests_toolkit/_academic.py
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     3585 2022-10-29 05:04:09.000000 requests-toolkit-stable-0.9.2/requests_toolkit/_air_quality.py
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      903 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.2/requests_toolkit/_thesis_info.py
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1355 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.2/requests_toolkit/_weather_query.py
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1734 2022-10-24 08:48:07.000000 requests-toolkit-stable-0.9.2/requests_toolkit/_ytb_channel_info.py
+drwxrwxr-x   0 leoxiang  (1000) leoxiang  (1000)        0 2022-10-29 05:08:13.846225 requests-toolkit-stable-0.9.2/requests_toolkit_stable.egg-info/
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)     1977 2022-10-29 05:08:13.000000 requests-toolkit-stable-0.9.2/requests_toolkit_stable.egg-info/PKG-INFO
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      458 2022-10-29 05:08:13.000000 requests-toolkit-stable-0.9.2/requests_toolkit_stable.egg-info/SOURCES.txt
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)        1 2022-10-29 05:08:13.000000 requests-toolkit-stable-0.9.2/requests_toolkit_stable.egg-info/dependency_links.txt
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)       29 2022-10-29 05:08:13.000000 requests-toolkit-stable-0.9.2/requests_toolkit_stable.egg-info/requires.txt
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)       17 2022-10-29 05:08:13.000000 requests-toolkit-stable-0.9.2/requests_toolkit_stable.egg-info/top_level.txt
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)       38 2022-10-29 05:08:13.846225 requests-toolkit-stable-0.9.2/setup.cfg
+-rw-rw-r--   0 leoxiang  (1000) leoxiang  (1000)      719 2022-10-29 05:04:38.000000 requests-toolkit-stable-0.9.2/setup.py
```

### Comparing `requests-toolkit-stable-0.9.1/LICENSE` & `requests-toolkit-stable-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-toolkit-stable-0.9.1/PKG-INFO` & `requests-toolkit-stable-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-toolkit-stable
-Version: 0.9.1
+Version: 0.9.2
 Summary: A package of APIs using requests.
 Home-page: https://github.com/leoxiang66/requests-toolkit
 Author: Tao Xiang
 Author-email: tao.xiang@tum.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `requests-toolkit-stable-0.9.1/README.md` & `requests-toolkit-stable-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `requests-toolkit-stable-0.9.1/requests_toolkit/_academic.py` & `requests-toolkit-stable-0.9.2/requests_toolkit/_academic.py`

 * *Files identical despite different names*

### Comparing `requests-toolkit-stable-0.9.1/requests_toolkit/_air_quality.py` & `requests-toolkit-stable-0.9.2/requests_toolkit/_air_quality.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 aqi_values.append((city,prov, aqi))
                 if return_frequency and len(aqi_values) % return_frequency ==0:
                     aqi_values.sort(key=lambda x: x[2])
                     yield aqi_values
 
 
         aqi_values.sort(key= lambda x: x[2])
-        return aqi_values
+        yield aqi_values
 
 
 if __name__ == '__main__':
     # print(AirQualityQuery.__get__provinces__('china'))
     generator = AirQualityQuery.air_quality_by_country('china', 10)
     for i in generator:
         print(i)
```

### Comparing `requests-toolkit-stable-0.9.1/requests_toolkit/_thesis_info.py` & `requests-toolkit-stable-0.9.2/requests_toolkit/_thesis_info.py`

 * *Files identical despite different names*

### Comparing `requests-toolkit-stable-0.9.1/requests_toolkit/_weather_query.py` & `requests-toolkit-stable-0.9.2/requests_toolkit/_weather_query.py`

 * *Files identical despite different names*

### Comparing `requests-toolkit-stable-0.9.1/requests_toolkit/_ytb_channel_info.py` & `requests-toolkit-stable-0.9.2/requests_toolkit/_ytb_channel_info.py`

 * *Files identical despite different names*

### Comparing `requests-toolkit-stable-0.9.1/requests_toolkit_stable.egg-info/PKG-INFO` & `requests-toolkit-stable-0.9.2/requests_toolkit_stable.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-toolkit-stable
-Version: 0.9.1
+Version: 0.9.2
 Summary: A package of APIs using requests.
 Home-page: https://github.com/leoxiang66/requests-toolkit
 Author: Tao Xiang
 Author-email: tao.xiang@tum.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `requests-toolkit-stable-0.9.1/setup.py` & `requests-toolkit-stable-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'requests',
     "xmltodict",
     'tqdm'
 ]
 
 setup(
     name="requests-toolkit-stable",
-    version="0.9.1",
+    version="0.9.2",
     author="Tao Xiang",
     author_email="tao.xiang@tum.de",
     description="A package of APIs using requests.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/leoxiang66/requests-toolkit",
     packages=find_packages(),
```

