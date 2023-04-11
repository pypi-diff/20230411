# Comparing `tmp/sm-search-connector-poc-interface-0.2.2.tar.gz` & `tmp/sm-search-connector-poc-interface-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sm-search-connector-poc-interface-0.2.2.tar", last modified: Mon Apr 10 01:07:37 2023, max compression
+gzip compressed data, was "sm-search-connector-poc-interface-0.2.3.tar", last modified: Tue Apr 11 17:40:27 2023, max compression
```

## Comparing `sm-search-connector-poc-interface-0.2.2.tar` & `sm-search-connector-poc-interface-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:07:37.053883 sm-search-connector-poc-interface-0.2.2/
--rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-10 01:07:37.053567 sm-search-connector-poc-interface-0.2.2/PKG-INFO
--rw-r--r--   0 shrmitul   (505) staff       (20)       38 2023-04-10 01:07:37.053981 sm-search-connector-poc-interface-0.2.2/setup.cfg
--rw-r--r--   0 shrmitul   (505) staff       (20)      361 2023-04-10 01:07:27.000000 sm-search-connector-poc-interface-0.2.2/setup.py
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:07:37.051319 sm-search-connector-poc-interface-0.2.2/sm-search-connector-poc-interface/
--rw-r--r--   0 shrmitul   (505) staff       (20)       86 2023-04-10 01:04:33.000000 sm-search-connector-poc-interface-0.2.2/sm-search-connector-poc-interface/__init__.py
--rw-r--r--   0 shrmitul   (505) staff       (20)      199 2023-04-09 23:58:40.000000 sm-search-connector-poc-interface-0.2.2/sm-search-connector-poc-interface/interface.py
-drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-10 01:07:37.053171 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/
--rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-10 01:07:36.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/PKG-INFO
--rw-r--r--   0 shrmitul   (505) staff       (20)      329 2023-04-10 01:07:37.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/SOURCES.txt
--rw-r--r--   0 shrmitul   (505) staff       (20)        1 2023-04-10 01:07:36.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/dependency_links.txt
--rw-r--r--   0 shrmitul   (505) staff       (20)       34 2023-04-10 01:07:36.000000 sm-search-connector-poc-interface-0.2.2/sm_search_connector_poc_interface.egg-info/top_level.txt
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-11 17:40:27.850452 sm-search-connector-poc-interface-0.2.3/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-11 17:40:27.850144 sm-search-connector-poc-interface-0.2.3/PKG-INFO
+-rw-r--r--   0 shrmitul   (505) staff       (20)      490 2023-04-11 17:15:21.000000 sm-search-connector-poc-interface-0.2.3/README.md
+-rw-r--r--   0 shrmitul   (505) staff       (20)       38 2023-04-11 17:40:27.850534 sm-search-connector-poc-interface-0.2.3/setup.cfg
+-rw-r--r--   0 shrmitul   (505) staff       (20)      361 2023-04-11 17:40:05.000000 sm-search-connector-poc-interface-0.2.3/setup.py
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-11 17:40:27.847542 sm-search-connector-poc-interface-0.2.3/sm-search-connector-poc-interface/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      124 2023-04-11 17:28:50.000000 sm-search-connector-poc-interface-0.2.3/sm-search-connector-poc-interface/__init__.py
+-rw-r--r--   0 shrmitul   (505) staff       (20)      307 2023-04-11 17:32:19.000000 sm-search-connector-poc-interface-0.2.3/sm-search-connector-poc-interface/interface.py
+-rw-r--r--   0 shrmitul   (505) staff       (20)      182 2023-04-11 17:28:50.000000 sm-search-connector-poc-interface-0.2.3/sm-search-connector-poc-interface/searchRequest.py
+-rw-r--r--   0 shrmitul   (505) staff       (20)      191 2023-04-11 17:32:35.000000 sm-search-connector-poc-interface-0.2.3/sm-search-connector-poc-interface/searchResponse.py
+drwxr-xr-x   0 shrmitul   (505) staff       (20)        0 2023-04-11 17:40:27.849533 sm-search-connector-poc-interface-0.2.3/sm_search_connector_poc_interface.egg-info/
+-rw-r--r--   0 shrmitul   (505) staff       (20)      187 2023-04-11 17:40:27.000000 sm-search-connector-poc-interface-0.2.3/sm_search_connector_poc_interface.egg-info/PKG-INFO
+-rw-r--r--   0 shrmitul   (505) staff       (20)      442 2023-04-11 17:40:27.000000 sm-search-connector-poc-interface-0.2.3/sm_search_connector_poc_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 shrmitul   (505) staff       (20)        1 2023-04-11 17:40:27.000000 sm-search-connector-poc-interface-0.2.3/sm_search_connector_poc_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 shrmitul   (505) staff       (20)       34 2023-04-11 17:40:27.000000 sm-search-connector-poc-interface-0.2.3/sm_search_connector_poc_interface.egg-info/top_level.txt
```

