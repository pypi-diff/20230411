# Comparing `tmp/lilyanncabinets-0.5.2.tar.gz` & `tmp/lilyanncabinets-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilyanncabinets-0.5.2.tar", last modified: Thu Mar 30 15:19:06 2023, max compression
+gzip compressed data, was "lilyanncabinets-1.5.1.tar", last modified: Tue Apr 11 08:05:03 2023, max compression
```

## Comparing `lilyanncabinets-0.5.2.tar` & `lilyanncabinets-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 15:19:06.306504 lilyanncabinets-0.5.2/
--rw-rw-rw-   0        0        0        0 2023-03-27 21:28:54.000000 lilyanncabinets-0.5.2/LICENSE
--rw-rw-rw-   0        0        0      679 2023-03-30 15:19:06.306504 lilyanncabinets-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-03-30 15:17:24.000000 lilyanncabinets-0.5.2/README.md
--rw-rw-rw-   0        0        0      108 2023-03-27 21:24:36.000000 lilyanncabinets-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0      607 2023-03-30 15:19:06.310352 lilyanncabinets-0.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-30 15:19:06.284875 lilyanncabinets-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-30 15:19:06.297926 lilyanncabinets-0.5.2/src/lilyanncabinets/
--rw-rw-rw-   0        0        0        0 2023-03-27 21:30:52.000000 lilyanncabinets-0.5.2/src/lilyanncabinets/__init__.py
--rw-rw-rw-   0        0        0      212 2023-03-30 15:10:59.000000 lilyanncabinets-0.5.2/src/lilyanncabinets/main.py
-drwxrwxrwx   0        0        0        0 2023-03-30 15:19:06.305926 lilyanncabinets-0.5.2/src/lilyanncabinets.egg-info/
--rw-rw-rw-   0        0        0      679 2023-03-30 15:19:06.000000 lilyanncabinets-0.5.2/src/lilyanncabinets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-03-30 15:19:06.000000 lilyanncabinets-0.5.2/src/lilyanncabinets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 15:19:06.000000 lilyanncabinets-0.5.2/src/lilyanncabinets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-03-30 15:19:06.000000 lilyanncabinets-0.5.2/src/lilyanncabinets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.659424 lilyanncabinets-1.5.1/
+-rw-rw-rw-   0        0        0        0 2023-03-27 21:28:54.000000 lilyanncabinets-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     1487 2023-04-11 08:05:03.659424 lilyanncabinets-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2023-04-11 08:04:47.000000 lilyanncabinets-1.5.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-27 21:24:36.000000 lilyanncabinets-1.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      607 2023-04-11 08:05:03.664423 lilyanncabinets-1.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.636422 lilyanncabinets-1.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.643422 lilyanncabinets-1.5.1/src/lilyanncabinets/
+-rw-rw-rw-   0        0        0        0 2023-03-27 21:30:52.000000 lilyanncabinets-1.5.1/src/lilyanncabinets/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-03-30 15:10:59.000000 lilyanncabinets-1.5.1/src/lilyanncabinets/main.py
+-rw-rw-rw-   0        0        0      777 2023-04-11 07:55:31.000000 lilyanncabinets-1.5.1/src/lilyanncabinets/sheets.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.658424 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/
+-rw-rw-rw-   0        0        0     1487 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/top_level.txt
```

### Comparing `lilyanncabinets-0.5.2/setup.cfg` & `lilyanncabinets-1.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 696c 7961 6e6e 6361 6269 6e65   = lilyanncabine
-00000020: 7473 0d0a 7665 7273 696f 6e20 3d20 302e  ts..version = 0.
-00000030: 352e 320d 0a61 7574 686f 7220 3d20 4a6f  5.2..author = Jo
+00000020: 7473 0d0a 7665 7273 696f 6e20 3d20 312e  ts..version = 1.
+00000030: 352e 310d 0a61 7574 686f 7220 3d20 4a6f  5.1..author = Jo
 00000040: 7365 7068 2043 616c 6967 6975 7269 0d0a  seph Caligiuri..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 206a  author_email = j
 00000060: 6361 6c69 6769 7572 6931 4067 6d61 696c  caligiuri1@gmail
 00000070: 2e63 6f6d 0d0a 6465 7363 7269 7074 696f  .com..descriptio
 00000080: 6e20 3d20 5061 636b 6167 6520 666f 7220  n = Package for 
 00000090: 7573 6520 6279 204c 696c 7920 416e 6e20  use by Lily Ann 
 000000a0: 4361 6269 6e65 7473 0d0a 6c6f 6e67 5f64  Cabinets..long_d
```

