# Comparing `tmp/goby_sdk-1.0.7.tar.gz` & `tmp/goby_sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goby_sdk-1.0.7.tar", last modified: Tue Apr 11 02:02:17 2023, max compression
+gzip compressed data, was "goby_sdk-1.0.8.tar", last modified: Tue Apr 11 02:03:32 2023, max compression
```

## Comparing `goby_sdk-1.0.7.tar` & `goby_sdk-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 02:02:17.852884 goby_sdk-1.0.7/
--rw-rw-rw-   0        0        0      199 2023-04-11 02:02:17.850896 goby_sdk-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2023-04-10 10:45:08.000000 goby_sdk-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 02:02:17.821543 goby_sdk-1.0.7/goby_sdk/
-drwxrwxrwx   0        0        0        0 2023-04-11 02:02:17.836860 goby_sdk-1.0.7/goby_sdk/V1/
--rw-rw-rw-   0        0        0        0 2023-04-03 07:20:55.000000 goby_sdk-1.0.7/goby_sdk/V1/__init__.py
--rw-rw-rw-   0        0        0     4976 2023-04-10 03:43:42.000000 goby_sdk-1.0.7/goby_sdk/V1/api.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:02:17.848897 goby_sdk-1.0.7/goby_sdk/V1/lib/
--rw-rw-rw-   0        0        0        0 2023-04-03 08:10:31.000000 goby_sdk-1.0.7/goby_sdk/V1/lib/__init__.py
--rw-rw-rw-   0        0        0     3805 2023-04-04 07:08:58.000000 goby_sdk-1.0.7/goby_sdk/V1/lib/asset_page.py
--rw-rw-rw-   0        0        0     1095 2023-04-04 07:07:49.000000 goby_sdk-1.0.7/goby_sdk/V1/lib/base_page.py
--rw-rw-rw-   0        0        0     1610 2023-04-04 07:09:05.000000 goby_sdk-1.0.7/goby_sdk/V1/lib/config_page.py
--rw-rw-rw-   0        0        0     4911 2023-04-10 03:26:09.000000 goby_sdk-1.0.7/goby_sdk/V1/lib/home_page.py
--rw-rw-rw-   0        0        0     1515 2023-04-04 07:09:53.000000 goby_sdk-1.0.7/goby_sdk/V1/lib/report_page.py
--rw-rw-rw-   0        0        0     3391 2023-04-04 07:10:18.000000 goby_sdk-1.0.7/goby_sdk/V1/lib/vulnerability_management_page.py
--rw-rw-rw-   0        0        0        0 2023-04-03 07:20:26.000000 goby_sdk-1.0.7/goby_sdk/__init__.py
--rw-rw-rw-   0        0        0      175 2023-04-11 01:49:00.000000 goby_sdk-1.0.7/goby_sdk/version.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:02:17.833860 goby_sdk-1.0.7/goby_sdk.egg-info/
--rw-rw-rw-   0        0        0      199 2023-04-11 02:02:17.000000 goby_sdk-1.0.7/goby_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-04-11 02:02:17.000000 goby_sdk-1.0.7/goby_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 02:02:17.000000 goby_sdk-1.0.7/goby_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 02:02:17.000000 goby_sdk-1.0.7/goby_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 02:02:17.000000 goby_sdk-1.0.7/goby_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 02:02:17.853884 goby_sdk-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-04-11 02:02:12.000000 goby_sdk-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:03:32.622180 goby_sdk-1.0.8/
+-rw-rw-rw-   0        0        0      199 2023-04-11 02:03:32.620177 goby_sdk-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1404 2023-04-10 10:45:08.000000 goby_sdk-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 02:03:32.589724 goby_sdk-1.0.8/goby_sdk/
+drwxrwxrwx   0        0        0        0 2023-04-11 02:03:32.601621 goby_sdk-1.0.8/goby_sdk/V1/
+-rw-rw-rw-   0        0        0        0 2023-04-03 07:20:55.000000 goby_sdk-1.0.8/goby_sdk/V1/__init__.py
+-rw-rw-rw-   0        0        0     4976 2023-04-10 03:43:42.000000 goby_sdk-1.0.8/goby_sdk/V1/api.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:03:32.618616 goby_sdk-1.0.8/goby_sdk/V1/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-03 08:10:31.000000 goby_sdk-1.0.8/goby_sdk/V1/lib/__init__.py
+-rw-rw-rw-   0        0        0     3805 2023-04-04 07:08:58.000000 goby_sdk-1.0.8/goby_sdk/V1/lib/asset_page.py
+-rw-rw-rw-   0        0        0     1095 2023-04-04 07:07:49.000000 goby_sdk-1.0.8/goby_sdk/V1/lib/base_page.py
+-rw-rw-rw-   0        0        0     1610 2023-04-04 07:09:05.000000 goby_sdk-1.0.8/goby_sdk/V1/lib/config_page.py
+-rw-rw-rw-   0        0        0     4911 2023-04-10 03:26:09.000000 goby_sdk-1.0.8/goby_sdk/V1/lib/home_page.py
+-rw-rw-rw-   0        0        0     1515 2023-04-04 07:09:53.000000 goby_sdk-1.0.8/goby_sdk/V1/lib/report_page.py
+-rw-rw-rw-   0        0        0     3391 2023-04-04 07:10:18.000000 goby_sdk-1.0.8/goby_sdk/V1/lib/vulnerability_management_page.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 07:20:26.000000 goby_sdk-1.0.8/goby_sdk/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-04-11 01:49:00.000000 goby_sdk-1.0.8/goby_sdk/version.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:03:32.598623 goby_sdk-1.0.8/goby_sdk.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-04-11 02:03:32.000000 goby_sdk-1.0.8/goby_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-04-11 02:03:32.000000 goby_sdk-1.0.8/goby_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:03:32.000000 goby_sdk-1.0.8/goby_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 02:03:32.000000 goby_sdk-1.0.8/goby_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 02:03:32.000000 goby_sdk-1.0.8/goby_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:03:32.622180 goby_sdk-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-04-11 02:03:30.000000 goby_sdk-1.0.8/setup.py
```

### Comparing `goby_sdk-1.0.7/README.md` & `goby_sdk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.7/goby_sdk/V1/api.py` & `goby_sdk-1.0.8/goby_sdk/V1/api.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.7/goby_sdk/V1/lib/asset_page.py` & `goby_sdk-1.0.8/goby_sdk/V1/lib/asset_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.7/goby_sdk/V1/lib/base_page.py` & `goby_sdk-1.0.8/goby_sdk/V1/lib/base_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.7/goby_sdk/V1/lib/config_page.py` & `goby_sdk-1.0.8/goby_sdk/V1/lib/config_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.7/goby_sdk/V1/lib/home_page.py` & `goby_sdk-1.0.8/goby_sdk/V1/lib/home_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.7/goby_sdk/V1/lib/report_page.py` & `goby_sdk-1.0.8/goby_sdk/V1/lib/report_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.7/goby_sdk/V1/lib/vulnerability_management_page.py` & `goby_sdk-1.0.8/goby_sdk/V1/lib/vulnerability_management_page.py`

 * *Files identical despite different names*

