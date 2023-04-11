# Comparing `tmp/my_python_package007-0.4.9.tar.gz` & `tmp/my_python_package007-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_python_package007-0.4.9.tar", last modified: Thu Mar 30 06:14:20 2023, max compression
+gzip compressed data, was "my_python_package007-0.5.6.tar", last modified: Tue Apr 11 10:08:59 2023, max compression
```

## Comparing `my_python_package007-0.4.9.tar` & `my_python_package007-0.5.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:14:20.976549 my_python_package007-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-30 06:14:20.976549 my_python_package007-0.4.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:14:20.972549 my_python_package007-0.4.9/my_python_package007.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-30 06:14:20.000000 my_python_package007-0.4.9/my_python_package007.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-30 06:14:20.000000 my_python_package007-0.4.9/my_python_package007.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 06:14:20.000000 my_python_package007-0.4.9/my_python_package007.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 06:14:20.000000 my_python_package007-0.4.9/my_python_package007.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 06:14:20.000000 my_python_package007-0.4.9/my_python_package007.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 06:14:20.976549 my_python_package007-0.4.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-03-30 06:14:06.000000 my_python_package007-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 06:14:20.976549 my_python_package007-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-30 06:14:06.000000 my_python_package007-0.4.9/tests/test_my_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:59.898688 my_python_package007-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 10:08:59.898688 my_python_package007-0.5.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:59.894688 my_python_package007-0.5.6/my_python_package007.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:08:59.000000 my_python_package007-0.5.6/my_python_package007.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:08:59.898688 my_python_package007-0.5.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-04-11 10:08:45.000000 my_python_package007-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:08:59.894688 my_python_package007-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 10:08:45.000000 my_python_package007-0.5.6/tests/test_my_module.py
```

