# Comparing `tmp/pandacolumns-0.2.1.tar.gz` & `tmp/pandacolumns-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.2.1.tar", last modified: Mon Apr 10 22:56:17 2023, max compression
+gzip compressed data, was "pandacolumns-0.2.2.tar", last modified: Mon Apr 10 23:37:31 2023, max compression
```

## Comparing `pandacolumns-0.2.1.tar` & `pandacolumns-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:56:17.144163 pandacolumns-0.2.1/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:56:17.143153 pandacolumns-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 22:56:17.123878 pandacolumns-0.2.1/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.1/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2155 2023-04-10 22:55:37.000000 pandacolumns-0.2.1/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:56:17.141995 pandacolumns-0.2.1/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:56:17.144163 pandacolumns-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 22:55:48.000000 pandacolumns-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:37:31.480957 pandacolumns-0.2.2/
+-rw-rw-rw-   0        0        0      171 2023-04-10 23:37:31.479946 pandacolumns-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 23:37:31.461612 pandacolumns-0.2.2/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.2/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-04-10 23:37:04.000000 pandacolumns-0.2.2/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:37:31.478439 pandacolumns-0.2.2/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 23:37:31.000000 pandacolumns-0.2.2/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-10 23:37:31.000000 pandacolumns-0.2.2/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 23:37:31.000000 pandacolumns-0.2.2/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 23:37:31.000000 pandacolumns-0.2.2/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 23:37:31.000000 pandacolumns-0.2.2/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 23:37:31.480957 pandacolumns-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 23:37:22.000000 pandacolumns-0.2.2/setup.py
```

