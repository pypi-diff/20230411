# Comparing `tmp/snapctl-0.1.2.tar.gz` & `tmp/snapctl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapctl-0.1.2.tar", max compression
+gzip compressed data, was "snapctl-0.2.0.tar", max compression
```

## Comparing `snapctl-0.1.2.tar` & `snapctl-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0       36 2023-03-24 21:34:36.749470 snapctl-0.1.2/README.md
--rw-r--r--   0        0        0      378 2023-03-29 23:32:37.624723 snapctl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.1.2/snapctl/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.1.2/snapctl/__main__.py
--rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.1.2/snapctl/echo.py
--rw-r--r--   0        0        0     6883 2023-03-29 22:53:36.352929 snapctl-0.1.2/snapctl/main.py
--rw-r--r--   0        0        0     1237 2023-03-24 21:04:16.238728 snapctl-0.1.2/snapctl/utils.py
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 snapctl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.0/README.md
+-rw-r--r--   0        0        0      399 2023-04-11 05:17:16.404291 snapctl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.0/snapctl/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.0/snapctl/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.0/snapctl/commands/__init__.py
+-rw-r--r--   0        0        0     7704 2023-04-11 06:02:17.804521 snapctl-0.2.0/snapctl/commands/byosnap.py
+-rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.0/snapctl/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.0/snapctl/types/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.0/snapctl/types/definitions.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.0/snapctl/utils/__init__.py
+-rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.0/snapctl/utils/echo.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.0/PKG-INFO
```

