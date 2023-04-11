# Comparing `tmp/WEB_AND_API_FOR_ME-0.0.1.tar.gz` & `tmp/WEB_AND_API_FOR_ME-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WEB_AND_API_FOR_ME-0.0.1.tar", last modified: Tue Apr 11 19:15:23 2023, max compression
+gzip compressed data, was "WEB_AND_API_FOR_ME-0.0.2.tar", last modified: Tue Apr 11 19:35:33 2023, max compression
```

## Comparing `WEB_AND_API_FOR_ME-0.0.1.tar` & `WEB_AND_API_FOR_ME-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 19:15:23.409738 WEB_AND_API_FOR_ME-0.0.1/
--rw-rw-rw-   0        0        0       65 2023-04-11 19:15:23.409738 WEB_AND_API_FOR_ME-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 19:15:23.394320 WEB_AND_API_FOR_ME-0.0.1/WEB_AND_API_FOR_ME.egg-info/
--rw-rw-rw-   0        0        0       65 2023-04-11 19:15:23.000000 WEB_AND_API_FOR_ME-0.0.1/WEB_AND_API_FOR_ME.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-04-11 19:15:23.000000 WEB_AND_API_FOR_ME-0.0.1/WEB_AND_API_FOR_ME.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 19:15:23.000000 WEB_AND_API_FOR_ME-0.0.1/WEB_AND_API_FOR_ME.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-11 19:15:23.000000 WEB_AND_API_FOR_ME-0.0.1/WEB_AND_API_FOR_ME.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-04-11 19:15:23.000000 WEB_AND_API_FOR_ME-0.0.1/WEB_AND_API_FOR_ME.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 19:15:23.396320 WEB_AND_API_FOR_ME-0.0.1/WS/
-drwxrwxrwx   0        0        0        0 2023-04-11 19:15:23.403371 WEB_AND_API_FOR_ME-0.0.1/WS/data/
--rw-rw-rw-   0        0        0     1808 2023-04-11 17:59:26.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/Zayavki_Resource.py
--rw-rw-rw-   0        0        0      125 2023-04-01 15:34:04.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/__all_models.py
--rw-rw-rw-   0        0        0      916 2023-04-11 17:09:41.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/db_session.py
--rw-rw-rw-   0        0        0      480 2023-04-02 13:05:43.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/division.py
--rw-rw-rw-   0        0        0     1449 2023-04-02 13:05:43.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/informationUser.py
--rw-rw-rw-   0        0        0     1290 2023-04-04 08:38:04.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/solo_zayavki.py
--rw-rw-rw-   0        0        0      460 2023-04-02 13:05:43.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/target.py
--rw-rw-rw-   0        0        0      973 2023-04-02 13:05:43.000000 WEB_AND_API_FOR_ME-0.0.1/WS/data/user.py
-drwxrwxrwx   0        0        0        0 2023-04-11 19:15:23.407373 WEB_AND_API_FOR_ME-0.0.1/WS/forms/
--rw-rw-rw-   0        0        0      189 2023-03-27 08:32:20.000000 WEB_AND_API_FOR_ME-0.0.1/WS/forms/glavnaya.py
--rw-rw-rw-   0        0        0       66 2023-04-01 07:32:58.000000 WEB_AND_API_FOR_ME-0.0.1/WS/forms/lichniy.py
--rw-rw-rw-   0        0        0      506 2023-04-01 10:34:43.000000 WEB_AND_API_FOR_ME-0.0.1/WS/forms/login.py
--rw-rw-rw-   0        0        0     1228 2023-04-03 10:37:32.000000 WEB_AND_API_FOR_ME-0.0.1/WS/forms/odinochnoe.py
--rw-rw-rw-   0        0        0      532 2023-04-01 10:26:51.000000 WEB_AND_API_FOR_ME-0.0.1/WS/forms/user.py
--rw-rw-rw-   0        0        0     8418 2023-04-11 17:59:26.000000 WEB_AND_API_FOR_ME-0.0.1/WS/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 19:15:23.408723 WEB_AND_API_FOR_ME-0.0.1/WS/test/
--rw-rw-rw-   0        0        0     2617 2023-03-30 07:08:50.000000 WEB_AND_API_FOR_ME-0.0.1/WS/test/main.py
--rw-rw-rw-   0        0        0      130 2023-04-04 12:12:37.000000 WEB_AND_API_FOR_ME-0.0.1/WS/test.py
--rw-rw-rw-   0        0        0      190 2023-04-11 19:15:23.410734 WEB_AND_API_FOR_ME-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      204 2023-04-11 19:14:25.000000 WEB_AND_API_FOR_ME-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:35:33.366109 WEB_AND_API_FOR_ME-0.0.2/
+-rw-rw-rw-   0        0        0       65 2023-04-11 19:35:33.366109 WEB_AND_API_FOR_ME-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 19:35:33.365110 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/
+-rw-rw-rw-   0        0        0       65 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 19:35:33.000000 WEB_AND_API_FOR_ME-0.0.2/WEB_AND_API_FOR_ME.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-04-11 19:35:33.370126 WEB_AND_API_FOR_ME-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      204 2023-04-11 19:35:31.000000 WEB_AND_API_FOR_ME-0.0.2/setup.py
+-rw-rw-rw-   0        0        0      637 2023-04-11 17:59:26.000000 WEB_AND_API_FOR_ME-0.0.2/ws_api.py
```

