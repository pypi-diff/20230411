# Comparing `tmp/python-hostingde-0.8.0.tar.gz` & `tmp/python-hostingde-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hostingde-0.8.0.tar", last modified: Thu Apr  6 15:26:18 2023, max compression
+gzip compressed data, was "python-hostingde-0.8.1.tar", last modified: Tue Apr 11 10:29:43 2023, max compression
```

## Comparing `python-hostingde-0.8.0.tar` & `python-hostingde-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.601296 python-hostingde-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1064 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8368 2023-04-06 15:26:18.601296 python-hostingde-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7347 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.593296 python-hostingde-0.8.0/hostingde/
--rw-r--r--   0 root         (0) root         (0)      131 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-06 15:26:15.000000 python-hostingde-0.8.0/hostingde/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.593296 python-hostingde-0.8.0/hostingde/account/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/account/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/account/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.593296 python-hostingde-0.8.0/hostingde/account/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/account/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/api.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.593296 python-hostingde-0.8.0/hostingde/dns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/dns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22828 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/dns/dns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.593296 python-hostingde-0.8.0/hostingde/dns/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/dns/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/dns/requests/create_new_zone.py
--rw-r--r--   0 root         (0) root         (0)      206 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/dns/requests/delete_zone.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/dns/requests/update_records_request.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/dns/requests/update_zone_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.593296 python-hostingde-0.8.0/hostingde/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5563 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/domain/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.593296 python-hostingde-0.8.0/hostingde/domain/requests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/domain/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      920 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/domain/requests/check_availability.py
--rw-r--r--   0 root         (0) root         (0)      179 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/domain/requests/register_domain.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/hostingde.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/job_waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.597296 python-hostingde-0.8.0/hostingde/model/
--rw-r--r--   0 root         (0) root         (0)     2854 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/account.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/domain.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/domain_contact.py
--rw-r--r--   0 root         (0) root         (0)    12691 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/filter.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/job.py
--rw-r--r--   0 root         (0) root         (0)     4779 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/record.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/soa_values.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/sort.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/zone.py
--rw-r--r--   0 root         (0) root         (0)     6620 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/model/zone_config.py
--rw-r--r--   0 root         (0) root         (0)     4779 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/paginator.py
--rw-r--r--   0 root         (0) root         (0)     3095 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/hostingde/session.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 15:26:18.601296 python-hostingde-0.8.0/python_hostingde.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8368 2023-04-06 15:26:18.000000 python-hostingde-0.8.0/python_hostingde.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1290 2023-04-06 15:26:18.000000 python-hostingde-0.8.0/python_hostingde.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 15:26:18.000000 python-hostingde-0.8.0/python_hostingde.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-04-06 15:26:18.000000 python-hostingde-0.8.0/python_hostingde.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-06 15:26:18.000000 python-hostingde-0.8.0/python_hostingde.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-06 15:26:18.601296 python-hostingde-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1748 2023-04-06 15:26:14.000000 python-hostingde-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.063388 python-hostingde-0.8.1/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8368 2023-04-11 10:29:43.063388 python-hostingde-0.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7347 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.059388 python-hostingde-0.8.1/hostingde/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-11 10:29:40.000000 python-hostingde-0.8.1/hostingde/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.059388 python-hostingde-0.8.1/hostingde/account/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/account/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.059388 python-hostingde-0.8.1/hostingde/account/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/account/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/api.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.059388 python-hostingde-0.8.1/hostingde/dns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/dns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22828 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/dns/dns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.059388 python-hostingde-0.8.1/hostingde/dns/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/dns/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/dns/requests/create_new_zone.py
+-rw-r--r--   0 root         (0) root         (0)      206 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/dns/requests/delete_zone.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/dns/requests/update_records_request.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/dns/requests/update_zone_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.063388 python-hostingde-0.8.1/hostingde/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5563 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/domain/domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.063388 python-hostingde-0.8.1/hostingde/domain/requests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/domain/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      920 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/domain/requests/check_availability.py
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/domain/requests/register_domain.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/hostingde.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/job_waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.063388 python-hostingde-0.8.1/hostingde/model/
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/account.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/domain.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/domain_contact.py
+-rw-r--r--   0 root         (0) root         (0)    12691 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/filter.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/job.py
+-rw-r--r--   0 root         (0) root         (0)     4779 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/record.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/soa_values.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/sort.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/zone.py
+-rw-r--r--   0 root         (0) root         (0)     6620 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/model/zone_config.py
+-rw-r--r--   0 root         (0) root         (0)     4779 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/paginator.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/hostingde/session.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:29:43.063388 python-hostingde-0.8.1/python_hostingde.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8368 2023-04-11 10:29:43.000000 python-hostingde-0.8.1/python_hostingde.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-04-11 10:29:43.000000 python-hostingde-0.8.1/python_hostingde.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:29:43.000000 python-hostingde-0.8.1/python_hostingde.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-11 10:29:43.000000 python-hostingde-0.8.1/python_hostingde.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-11 10:29:43.000000 python-hostingde-0.8.1/python_hostingde.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-11 10:29:43.063388 python-hostingde-0.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-04-11 10:29:39.000000 python-hostingde-0.8.1/setup.py
```

### Comparing `python-hostingde-0.8.0/LICENSE` & `python-hostingde-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/PKG-INFO` & `python-hostingde-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hostingde
-Version: 0.8.0
+Version: 0.8.1
 Summary: Interact with HostingDe API
 Home-page: https://github.com/cancom/python-hostingde
 Author: CANCOM OpenSource
 Author-email: opensource@cancom.de
 License: MIT
 Project-URL: Source, https://github.com/cancom/python-hostingde
 Project-URL: Bug Reports, https://github.com/cancom/python-hostingde/issues
```

### Comparing `python-hostingde-0.8.0/README.md` & `python-hostingde-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/account/account.py` & `python-hostingde-0.8.1/hostingde/account/account.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/api.py` & `python-hostingde-0.8.1/hostingde/api.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/client.py` & `python-hostingde-0.8.1/hostingde/client.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/dns/dns.py` & `python-hostingde-0.8.1/hostingde/dns/dns.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/dns/requests/update_records_request.py` & `python-hostingde-0.8.1/hostingde/dns/requests/update_records_request.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/dns/requests/update_zone_request.py` & `python-hostingde-0.8.1/hostingde/dns/requests/update_zone_request.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/domain/domain.py` & `python-hostingde-0.8.1/hostingde/domain/domain.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/domain/requests/check_availability.py` & `python-hostingde-0.8.1/hostingde/domain/requests/check_availability.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/exceptions.py` & `python-hostingde-0.8.1/hostingde/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/hostingde.py` & `python-hostingde-0.8.1/hostingde/hostingde.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/job_waiter.py` & `python-hostingde-0.8.1/hostingde/job_waiter.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/__init__.py` & `python-hostingde-0.8.1/hostingde/model/__init__.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/account.py` & `python-hostingde-0.8.1/hostingde/model/account.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/domain.py` & `python-hostingde-0.8.1/hostingde/model/domain.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/domain_contact.py` & `python-hostingde-0.8.1/hostingde/model/domain_contact.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/filter.py` & `python-hostingde-0.8.1/hostingde/model/filter.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/job.py` & `python-hostingde-0.8.1/hostingde/model/job.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/record.py` & `python-hostingde-0.8.1/hostingde/model/record.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/soa_values.py` & `python-hostingde-0.8.1/hostingde/model/soa_values.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/sort.py` & `python-hostingde-0.8.1/hostingde/model/sort.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/zone.py` & `python-hostingde-0.8.1/hostingde/model/zone.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/model/zone_config.py` & `python-hostingde-0.8.1/hostingde/model/zone_config.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/paginator.py` & `python-hostingde-0.8.1/hostingde/paginator.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/hostingde/session.py` & `python-hostingde-0.8.1/hostingde/session.py`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/python_hostingde.egg-info/PKG-INFO` & `python-hostingde-0.8.1/python_hostingde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hostingde
-Version: 0.8.0
+Version: 0.8.1
 Summary: Interact with HostingDe API
 Home-page: https://github.com/cancom/python-hostingde
 Author: CANCOM OpenSource
 Author-email: opensource@cancom.de
 License: MIT
 Project-URL: Source, https://github.com/cancom/python-hostingde
 Project-URL: Bug Reports, https://github.com/cancom/python-hostingde/issues
```

### Comparing `python-hostingde-0.8.0/python_hostingde.egg-info/SOURCES.txt` & `python-hostingde-0.8.1/python_hostingde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-hostingde-0.8.0/setup.py` & `python-hostingde-0.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     packages=find_packages(exclude=["docs*", "tests*"]),
     install_requires=[
         "requests>=2.25.1",
         "marshmallow==3.10.0",
         "marshmallow-dataclass==8.3.1",
         "marshmallow-enum==1.5.1",
         "urllib3~=1.26.3",
-        "responses~=0.13.1",
     ],
     python_requires=">=3.6.0",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: POSIX",
```

