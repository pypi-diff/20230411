# Comparing `tmp/pygoogalytics-0.2.5.tar.gz` & `tmp/pygoogalytics-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.2.5.tar", last modified: Wed Mar  8 12:36:42 2023, max compression
+gzip compressed data, was "pygoogalytics-0.2.6.tar", last modified: Tue Apr 11 08:53:11 2023, max compression
```

## Comparing `pygoogalytics-0.2.5.tar` & `pygoogalytics-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-03-08 12:36:42.573053 pygoogalytics-0.2.5/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.2.5/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.2.5/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-03-08 12:36:42.572919 pygoogalytics-0.2.5/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.2.5/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-03-08 12:36:42.571729 pygoogalytics-0.2.5/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-03-08 12:36:25.000000 pygoogalytics-0.2.5/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5729 2023-03-08 12:36:25.000000 pygoogalytics-0.2.5/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-03-08 12:36:42.572702 pygoogalytics-0.2.5/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.2.5/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.2.5/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    36515 2023-02-21 11:13:08.000000 pygoogalytics-0.2.5/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.2.5/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    40628 2023-03-07 20:05:15.000000 pygoogalytics-0.2.5/pygoogalytics/kwp_wrappers.py
--rw-r--r--   0 joshua     (501) staff       (20)     2409 2023-03-07 19:50:49.000000 pygoogalytics-0.2.5/pygoogalytics/resource_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.2.5/pygoogalytics/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-03-08 12:36:42.572417 pygoogalytics-0.2.5/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-03-08 12:36:42.000000 pygoogalytics-0.2.5/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      512 2023-03-08 12:36:42.000000 pygoogalytics-0.2.5/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-03-08 12:36:42.000000 pygoogalytics-0.2.5/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-03-08 12:36:42.000000 pygoogalytics-0.2.5/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-03-08 12:36:42.000000 pygoogalytics-0.2.5/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-03-08 12:36:42.573092 pygoogalytics-0.2.5/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-03-08 12:36:25.000000 pygoogalytics-0.2.5/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.050288 pygoogalytics-0.2.6/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.2.6/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.2.6/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-11 08:53:11.050143 pygoogalytics-0.2.6/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.2.6/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.048104 pygoogalytics-0.2.6/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-11 08:52:41.000000 pygoogalytics-0.2.6/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5729 2023-03-08 12:36:25.000000 pygoogalytics-0.2.6/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.049730 pygoogalytics-0.2.6/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.2.6/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.2.6/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    36524 2023-04-11 08:51:56.000000 pygoogalytics-0.2.6/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.2.6/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    40628 2023-03-07 20:05:15.000000 pygoogalytics-0.2.6/pygoogalytics/kwp_wrappers.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2409 2023-03-07 19:50:49.000000 pygoogalytics-0.2.6/pygoogalytics/resource_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.2.6/pygoogalytics/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.048898 pygoogalytics-0.2.6/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-11 08:53:11.050333 pygoogalytics-0.2.6/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-11 08:52:31.000000 pygoogalytics-0.2.6/setup.py
```

### Comparing `pygoogalytics-0.2.5/LICENCE.txt` & `pygoogalytics-0.2.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/LICENSE` & `pygoogalytics-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/PKG-INFO` & `pygoogalytics-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.5
+Version: 0.2.6
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.5/README.md` & `pygoogalytics-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics/__init__.py` & `pygoogalytics-0.2.6/pygoogalytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.2.5/pygoogalytics/client.py` & `pygoogalytics-0.2.6/pygoogalytics/client.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.2.6/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.2.6/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.2.6/pygoogalytics/googalytics_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         except Exception as http_e:
             _api_status = "Other Error"
             _api_error = repr(http_e)
             pga_logger.debug(f"{self.__class__.__name__}.api_test() :: GSC api failed")
             # The HttpError for GSC contains this unhelpful "See also this answer to a question..."
             # which is just a link to an FAQ with a 404 error
 
-        self._api_test_gsc = {'status': _api_status, 'error': _api_error, 'timestamp': datetime.datetime.now()}
+        self._api_test_gsc = {'status': _api_status, 'error': _api_error, 'timestamp': datetime.datetime.utcnow()}
 
     @property
     def api_test_gsc(self) -> dict:
         if self._api_test_gsc.get('status') is None:
             self._perform_api_test_gsc()
         return self._api_test_gsc
 
@@ -141,15 +141,15 @@
             _api_status = "HttpError"
             _api_error = repr(http_e)
             pga_logger.debug(f"{self.__class__.__name__}.api_test() :: GA api failed")
         except Exception as http_e:
             _api_status = "Other Error"
             _api_error = repr(http_e)
             pga_logger.debug(f"{self.__class__.__name__}.api_test() :: GA api failed")
-        self._api_test_ga3 = {'status': _api_status, 'error': _api_error, 'timestamp': datetime.datetime.now()}
+        self._api_test_ga3 = {'status': _api_status, 'error': _api_error, 'timestamp': datetime.datetime.utcnow()}
 
     @property
     def api_test_ga4(self) -> dict:
         return self._api_test_ga4
 
     # *****************************************************************************************
 
@@ -773,15 +773,15 @@
             ga3_df.add_new_user_column()
             ga3_df.add_shopping_stage_all_column()
             ga3_df.add_has_site_search_column()
 
         return ga3_df
 
     def urlinspection_dict(self, url: str, inspection_index: int = None) -> dict:
-        _now = datetime.datetime.now()
+        _now = datetime.datetime.utcnow()
         _d = {"record_date": _now.date(),
               "record_time": _now.time(),
               "url": url}
 
         try:
             response = self.get_inspection_response(url)
         except Exception as _e:
```

### Comparing `pygoogalytics-0.2.5/pygoogalytics/googlepandas.py` & `pygoogalytics-0.2.6/pygoogalytics/googlepandas.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.2.6/pygoogalytics/kwp_wrappers.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics/resource_utils.py` & `pygoogalytics-0.2.6/pygoogalytics/resource_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics/utils.py` & `pygoogalytics-0.2.6/pygoogalytics/utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.2.6/pygoogalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.5
+Version: 0.2.6
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.5/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.2.6/pygoogalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.5/setup.py` & `pygoogalytics-0.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.2.5',
+    version='0.2.6',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

