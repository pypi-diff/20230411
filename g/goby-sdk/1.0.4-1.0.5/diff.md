# Comparing `tmp/goby_sdk-1.0.4.tar.gz` & `tmp/goby_sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goby_sdk-1.0.4.tar", last modified: Tue Apr 11 01:49:10 2023, max compression
+gzip compressed data, was "goby_sdk-1.0.5.tar", last modified: Tue Apr 11 01:52:10 2023, max compression
```

## Comparing `goby_sdk-1.0.4.tar` & `goby_sdk-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 01:49:10.925994 goby_sdk-1.0.4/
--rw-rw-rw-   0        0        0      188 2023-04-11 01:49:10.924994 goby_sdk-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2023-04-10 10:45:08.000000 goby_sdk-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 01:49:10.892607 goby_sdk-1.0.4/goby_sdk/
-drwxrwxrwx   0        0        0        0 2023-04-11 01:49:10.907590 goby_sdk-1.0.4/goby_sdk/V1/
--rw-rw-rw-   0        0        0        0 2023-04-03 07:20:55.000000 goby_sdk-1.0.4/goby_sdk/V1/__init__.py
--rw-rw-rw-   0        0        0     4976 2023-04-10 03:43:42.000000 goby_sdk-1.0.4/goby_sdk/V1/api.py
-drwxrwxrwx   0        0        0        0 2023-04-11 01:49:10.922995 goby_sdk-1.0.4/goby_sdk/V1/lib/
--rw-rw-rw-   0        0        0        0 2023-04-03 08:10:31.000000 goby_sdk-1.0.4/goby_sdk/V1/lib/__init__.py
--rw-rw-rw-   0        0        0     3805 2023-04-04 07:08:58.000000 goby_sdk-1.0.4/goby_sdk/V1/lib/asset_page.py
--rw-rw-rw-   0        0        0     1095 2023-04-04 07:07:49.000000 goby_sdk-1.0.4/goby_sdk/V1/lib/base_page.py
--rw-rw-rw-   0        0        0     1610 2023-04-04 07:09:05.000000 goby_sdk-1.0.4/goby_sdk/V1/lib/config_page.py
--rw-rw-rw-   0        0        0     4911 2023-04-10 03:26:09.000000 goby_sdk-1.0.4/goby_sdk/V1/lib/home_page.py
--rw-rw-rw-   0        0        0     1515 2023-04-04 07:09:53.000000 goby_sdk-1.0.4/goby_sdk/V1/lib/report_page.py
--rw-rw-rw-   0        0        0     3391 2023-04-04 07:10:18.000000 goby_sdk-1.0.4/goby_sdk/V1/lib/vulnerability_management_page.py
--rw-rw-rw-   0        0        0        0 2023-04-03 07:20:26.000000 goby_sdk-1.0.4/goby_sdk/__init__.py
--rw-rw-rw-   0        0        0      175 2023-04-11 01:49:00.000000 goby_sdk-1.0.4/goby_sdk/version.py
-drwxrwxrwx   0        0        0        0 2023-04-11 01:49:10.903592 goby_sdk-1.0.4/goby_sdk.egg-info/
--rw-rw-rw-   0        0        0      188 2023-04-11 01:49:10.000000 goby_sdk-1.0.4/goby_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-04-11 01:49:10.000000 goby_sdk-1.0.4/goby_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 01:49:10.000000 goby_sdk-1.0.4/goby_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 01:49:10.000000 goby_sdk-1.0.4/goby_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 01:49:10.000000 goby_sdk-1.0.4/goby_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 01:49:10.925994 goby_sdk-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-04-11 01:48:44.000000 goby_sdk-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:52:10.647480 goby_sdk-1.0.5/
+-rw-rw-rw-   0        0        0      199 2023-04-11 01:52:10.646493 goby_sdk-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1404 2023-04-10 10:45:08.000000 goby_sdk-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 01:52:10.609959 goby_sdk-1.0.5/goby_sdk/
+drwxrwxrwx   0        0        0        0 2023-04-11 01:52:10.625488 goby_sdk-1.0.5/goby_sdk/V1/
+-rw-rw-rw-   0        0        0        0 2023-04-03 07:20:55.000000 goby_sdk-1.0.5/goby_sdk/V1/__init__.py
+-rw-rw-rw-   0        0        0     4976 2023-04-10 03:43:42.000000 goby_sdk-1.0.5/goby_sdk/V1/api.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:52:10.639482 goby_sdk-1.0.5/goby_sdk/V1/lib/
+-rw-rw-rw-   0        0        0        0 2023-04-03 08:10:31.000000 goby_sdk-1.0.5/goby_sdk/V1/lib/__init__.py
+-rw-rw-rw-   0        0        0     3805 2023-04-04 07:08:58.000000 goby_sdk-1.0.5/goby_sdk/V1/lib/asset_page.py
+-rw-rw-rw-   0        0        0     1095 2023-04-04 07:07:49.000000 goby_sdk-1.0.5/goby_sdk/V1/lib/base_page.py
+-rw-rw-rw-   0        0        0     1610 2023-04-04 07:09:05.000000 goby_sdk-1.0.5/goby_sdk/V1/lib/config_page.py
+-rw-rw-rw-   0        0        0     4911 2023-04-10 03:26:09.000000 goby_sdk-1.0.5/goby_sdk/V1/lib/home_page.py
+-rw-rw-rw-   0        0        0     1515 2023-04-04 07:09:53.000000 goby_sdk-1.0.5/goby_sdk/V1/lib/report_page.py
+-rw-rw-rw-   0        0        0     3391 2023-04-04 07:10:18.000000 goby_sdk-1.0.5/goby_sdk/V1/lib/vulnerability_management_page.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 07:20:26.000000 goby_sdk-1.0.5/goby_sdk/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-04-11 01:49:00.000000 goby_sdk-1.0.5/goby_sdk/version.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:52:10.620820 goby_sdk-1.0.5/goby_sdk.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-04-11 01:52:10.000000 goby_sdk-1.0.5/goby_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-04-11 01:52:10.000000 goby_sdk-1.0.5/goby_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 01:52:10.000000 goby_sdk-1.0.5/goby_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 01:52:10.000000 goby_sdk-1.0.5/goby_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 01:52:10.000000 goby_sdk-1.0.5/goby_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 01:52:10.647480 goby_sdk-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      357 2023-04-11 01:51:57.000000 goby_sdk-1.0.5/setup.py
```

### Comparing `goby_sdk-1.0.4/README.md` & `goby_sdk-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.4/goby_sdk/V1/api.py` & `goby_sdk-1.0.5/goby_sdk/V1/api.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.4/goby_sdk/V1/lib/asset_page.py` & `goby_sdk-1.0.5/goby_sdk/V1/lib/asset_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.4/goby_sdk/V1/lib/base_page.py` & `goby_sdk-1.0.5/goby_sdk/V1/lib/base_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.4/goby_sdk/V1/lib/config_page.py` & `goby_sdk-1.0.5/goby_sdk/V1/lib/config_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.4/goby_sdk/V1/lib/home_page.py` & `goby_sdk-1.0.5/goby_sdk/V1/lib/home_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.4/goby_sdk/V1/lib/report_page.py` & `goby_sdk-1.0.5/goby_sdk/V1/lib/report_page.py`

 * *Files identical despite different names*

### Comparing `goby_sdk-1.0.4/goby_sdk/V1/lib/vulnerability_management_page.py` & `goby_sdk-1.0.5/goby_sdk/V1/lib/vulnerability_management_page.py`

 * *Files identical despite different names*

