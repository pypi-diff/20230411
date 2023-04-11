# Comparing `tmp/naruno_remote_app-0.56.0.tar.gz` & `tmp/naruno_remote_app-0.56.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_remote_app-0.56.0.tar", last modified: Mon Apr 10 18:13:18 2023, max compression
+gzip compressed data, was "naruno_remote_app-0.56.1.tar", last modified: Tue Apr 11 06:16:18 2023, max compression
```

## Comparing `naruno_remote_app-0.56.0.tar` & `naruno_remote_app-0.56.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:18.676705 naruno_remote_app-0.56.0/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 18:13:18.676705 naruno_remote_app-0.56.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:18.676705 naruno_remote_app-0.56.0/naruno_remote_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-10 18:13:18.000000 naruno_remote_app-0.56.0/naruno_remote_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-10 18:13:18.000000 naruno_remote_app-0.56.0/naruno_remote_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:13:18.000000 naruno_remote_app-0.56.0/naruno_remote_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:13:18.000000 naruno_remote_app-0.56.0/naruno_remote_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 18:13:18.000000 naruno_remote_app-0.56.0/naruno_remote_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:13:18.000000 naruno_remote_app-0.56.0/naruno_remote_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:13:18.676705 naruno_remote_app-0.56.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-10 18:13:01.000000 naruno_remote_app-0.56.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-11 06:16:02.000000 naruno_remote_app-0.56.1/setup.py
```

