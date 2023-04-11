# Comparing `tmp/ds2g-1.0.0.tar.gz` & `tmp/ds2g-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds2g-1.0.0.tar", last modified: Fri Jun 10 11:59:09 2022, max compression
+gzip compressed data, was "ds2g-1.0.1.tar", last modified: Tue Apr 11 10:03:45 2023, max compression
```

## Comparing `ds2g-1.0.0.tar` & `ds2g-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 code      (1000) code      (1000)        0 2022-06-10 11:59:09.699774 ds2g-1.0.0/
--rw-r--r--   0 code      (1000) code      (1000)        0 2022-06-10 11:02:32.000000 ds2g-1.0.0/LICENSE
--rw-r--r--   0 code      (1000) code      (1000)        0 2022-06-10 11:02:39.000000 ds2g-1.0.0/MANIFEST.in
--rw-r--r--   0 code      (1000) code      (1000)      424 2022-06-10 11:59:09.699774 ds2g-1.0.0/PKG-INFO
--rw-r--r--   0 code      (1000) code      (1000)        0 2022-06-10 11:02:46.000000 ds2g-1.0.0/README.md
--rw-r--r--   0 code      (1000) code      (1000)      747 2022-06-10 11:37:18.000000 ds2g-1.0.0/pyproject.toml
--rw-r--r--   0 code      (1000) code      (1000)       38 2022-06-10 11:59:09.699774 ds2g-1.0.0/setup.cfg
--rw-r--r--   0 code      (1000) code      (1000)       49 2022-06-10 11:45:36.000000 ds2g-1.0.0/setup.py
-drwxr-xr-x   0 code      (1000) code      (1000)        0 2022-06-10 11:59:09.699774 ds2g-1.0.0/src/
-drwxr-xr-x   0 code      (1000) code      (1000)        0 2022-06-10 11:59:09.699774 ds2g-1.0.0/src/ds2g/
--rw-r--r--   0 code      (1000) code      (1000)     1590 2022-06-10 11:28:45.000000 ds2g-1.0.0/src/ds2g/TrackingService.py
--rw-r--r--   0 code      (1000) code      (1000)      115 2022-06-10 11:51:02.000000 ds2g-1.0.0/src/ds2g/__init__.py
--rw-r--r--   0 code      (1000) code      (1000)       98 2022-06-10 11:11:12.000000 ds2g-1.0.0/src/ds2g/__main__.py
-drwxr-xr-x   0 code      (1000) code      (1000)        0 2022-06-10 11:59:09.699774 ds2g-1.0.0/src/ds2g.egg-info/
--rw-r--r--   0 code      (1000) code      (1000)      424 2022-06-10 11:59:09.000000 ds2g-1.0.0/src/ds2g.egg-info/PKG-INFO
--rw-r--r--   0 code      (1000) code      (1000)      317 2022-06-10 11:59:09.000000 ds2g-1.0.0/src/ds2g.egg-info/SOURCES.txt
--rw-r--r--   0 code      (1000) code      (1000)        1 2022-06-10 11:59:09.000000 ds2g-1.0.0/src/ds2g.egg-info/dependency_links.txt
--rw-r--r--   0 code      (1000) code      (1000)       44 2022-06-10 11:59:09.000000 ds2g-1.0.0/src/ds2g.egg-info/entry_points.txt
--rw-r--r--   0 code      (1000) code      (1000)       78 2022-06-10 11:59:09.000000 ds2g-1.0.0/src/ds2g.egg-info/requires.txt
--rw-r--r--   0 code      (1000) code      (1000)        5 2022-06-10 11:59:09.000000 ds2g-1.0.0/src/ds2g.egg-info/top_level.txt
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.880348 ds2g-1.0.1/
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.1/LICENSE
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.1/MANIFEST.in
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      424 2023-04-11 10:03:45.880203 ds2g-1.0.1/PKG-INFO
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        0 2022-11-10 14:16:28.000000 ds2g-1.0.1/README.md
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      794 2023-04-11 07:18:03.000000 ds2g-1.0.1/pyproject.toml
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       38 2023-04-11 10:03:45.880390 ds2g-1.0.1/setup.cfg
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       49 2022-11-10 14:16:28.000000 ds2g-1.0.1/setup.py
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.877544 ds2g-1.0.1/src/
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.878949 ds2g-1.0.1/src/ds2g/
+-rw-r--r--   0 martinlimberger   (501) staff       (20)     2598 2023-04-11 09:53:30.000000 ds2g-1.0.1/src/ds2g/TrackingService.py
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      115 2023-04-11 09:06:04.000000 ds2g-1.0.1/src/ds2g/__init__.py
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       98 2023-04-11 07:51:43.000000 ds2g-1.0.1/src/ds2g/__main__.py
+drwxr-xr-x   0 martinlimberger   (501) staff       (20)        0 2023-04-11 10:03:45.880001 ds2g-1.0.1/src/ds2g.egg-info/
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      424 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/PKG-INFO
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      317 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/SOURCES.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        1 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/dependency_links.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)       44 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/entry_points.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)      107 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/requires.txt
+-rw-r--r--   0 martinlimberger   (501) staff       (20)        5 2023-04-11 10:03:45.000000 ds2g-1.0.1/src/ds2g.egg-info/top_level.txt
```

