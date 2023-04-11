# Comparing `tmp/all4scripts_zfullio-0.0.1.tar.gz` & `tmp/all4scripts_zfullio-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all4scripts_zfullio-0.0.1.tar", max compression
+gzip compressed data, was "all4scripts_zfullio-0.1.0.tar", max compression
```

## Comparing `all4scripts_zfullio-0.0.1.tar` & `all4scripts_zfullio-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1069 2022-08-09 03:27:15.960000 all4scripts_zfullio-0.0.1/LICENSE
--rw-r--r--   0        0        0      396 2022-08-09 06:24:08.390740 all4scripts_zfullio-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       64 2022-08-09 06:26:13.719504 all4scripts_zfullio-0.0.1/src/all4scripts_zfullio/__init__.py
--rwxr-xr-x   0        0        0     2064 2022-06-21 15:22:36.871000 all4scripts_zfullio-0.0.1/src/all4scripts_zfullio/allfoscript.py
--rw-r--r--   0        0        0      751 2022-08-09 06:30:03.957933 all4scripts_zfullio-0.0.1/setup.py
--rw-r--r--   0        0        0      392 2022-08-09 06:30:03.958134 all4scripts_zfullio-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2022-08-09 03:27:15.960000 all4scripts_zfullio-0.1.0/LICENSE
+-rwxr-xr-x   0        0        0      392 2023-04-11 03:07:52.454928 all4scripts_zfullio-0.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0       64 2022-08-09 06:26:13.719504 all4scripts_zfullio-0.1.0/src/all4scripts_zfullio/__init__.py
+-rwxr-xr-x   0        0        0     2064 2022-06-21 15:22:36.871000 all4scripts_zfullio-0.1.0/src/all4scripts_zfullio/allfoscript.py
+-rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 all4scripts_zfullio-0.1.0/PKG-INFO
```

### Comparing `all4scripts_zfullio-0.0.1/LICENSE` & `all4scripts_zfullio-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `all4scripts_zfullio-0.0.1/src/all4scripts_zfullio/allfoscript.py` & `all4scripts_zfullio-0.1.0/src/all4scripts_zfullio/allfoscript.py`

 * *Files identical despite different names*

