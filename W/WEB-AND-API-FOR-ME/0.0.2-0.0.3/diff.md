# Comparing `tmp/WEB_AND_API_FOR_ME-0.0.2.tar.gz` & `tmp/WEB_AND_API_FOR_ME-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WEB_AND_API_FOR_ME-0.0.2.tar", last modified: Tue Apr 11 19:35:33 2023, max compression
+gzip compressed data, was "WEB_AND_API_FOR_ME-0.0.3.tar", last modified: Tue Apr 11 19:49:23 2023, max compression
```

## Comparing `WEB_AND_API_FOR_ME-0.0.2.tar` & `WEB_AND_API_FOR_ME-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 19:35:33.366109 WEB_AND_API_FOR_ME-0.0.2/
--rw-rw-rw-   0        0        0       65 2023-04-11 19:35:33.366109 WEB_AND_API_FOR_ME-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 19:35:33.365110 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/
--rw-rw-rw-   0        0        0       65 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-04-11 19:35:33.370126 WEB_AND_API_FOR_ME-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      204 2023-04-11 19:35:31.000000 WEB_AND_API_FOR_ME-0.0.2/setup.py
--rw-rw-rw-   0        0        0      637 2023-04-11 17:59:26.000000 WEB_AND_API_FOR_ME-0.0.2/ws_api.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:49:23.383013 WEB_AND_API_FOR_ME-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-11 19:49:23.342695 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/
+drwxrwxrwx   0        0        0        0 2023-04-11 19:49:23.350217 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/
+-rw-rw-rw-   0        0        0     1808 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/Zayavki_Resource.py
+-rw-rw-rw-   0        0        0      125 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/__all_models.py
+-rw-rw-rw-   0        0        0      916 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/db_session.py
+-rw-rw-rw-   0        0        0      480 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/division.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/informationUser.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/solo_zayavki.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/target.py
+-rw-rw-rw-   0        0        0      973 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/data/user.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:49:23.354733 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/forms/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/forms/glavnaya.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/forms/lichniy.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/forms/login.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/forms/odinochnoe.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/forms/user.py
+-rw-rw-rw-   0        0        0     8418 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:49:23.354733 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/test/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:48:48.000000 WEB_AND_API_FOR_ME-0.0.3/MY_WEB_AND_API/test/main.py
+-rw-rw-rw-   0        0        0       65 2023-04-11 19:49:23.383013 WEB_AND_API_FOR_ME-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 19:49:23.382011 WEB_AND_API_FOR_ME-0.0.3/WEB_AND_API_FOR_ME.egg-info/
+-rw-rw-rw-   0        0        0       65 2023-04-11 19:49:23.000000 WEB_AND_API_FOR_ME-0.0.3/WEB_AND_API_FOR_ME.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-04-11 19:49:23.000000 WEB_AND_API_FOR_ME-0.0.3/WEB_AND_API_FOR_ME.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:49:23.000000 WEB_AND_API_FOR_ME-0.0.3/WEB_AND_API_FOR_ME.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-11 19:49:23.000000 WEB_AND_API_FOR_ME-0.0.3/WEB_AND_API_FOR_ME.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 19:49:23.000000 WEB_AND_API_FOR_ME-0.0.3/WEB_AND_API_FOR_ME.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-04-11 19:49:23.384518 WEB_AND_API_FOR_ME-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      204 2023-04-11 19:49:17.000000 WEB_AND_API_FOR_ME-0.0.3/setup.py
```

