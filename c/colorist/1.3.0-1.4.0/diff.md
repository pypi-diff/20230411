# Comparing `tmp/colorist-1.3.0.tar.gz` & `tmp/colorist-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorist-1.3.0.tar", last modified: Mon Mar 27 19:54:45 2023, max compression
+gzip compressed data, was "colorist-1.4.0.tar", last modified: Mon Apr 10 22:26:56 2023, max compression
```

## Comparing `colorist-1.3.0.tar` & `colorist-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,70 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-03-27 19:54:45.733554 colorist-1.3.0/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1084 2023-01-25 13:58:40.000000 colorist-1.3.0/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      193 2023-01-25 13:58:40.000000 colorist-1.3.0/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    17717 2023-03-27 19:54:45.733641 colorist-1.3.0/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    15833 2023-03-27 19:48:01.000000 colorist-1.3.0/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:58:40.000000 colorist-1.3.0/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1409 2023-03-27 19:54:45.734021 colorist-1.3.0/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-03-27 19:54:45.730540 colorist-1.3.0/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-03-27 19:54:45.731551 colorist-1.3.0/src/colorist/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1432 2023-01-25 13:58:40.000000 colorist-1.3.0/src/colorist/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3946 2023-03-27 19:53:45.000000 colorist-1.3.0/src/colorist/__main__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-03-27 19:54:45.732693 colorist-1.3.0/src/colorist/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       64 2023-01-25 13:58:40.000000 colorist-1.3.0/src/colorist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      531 2023-03-27 19:53:45.000000 colorist-1.3.0/src/colorist/helper/print.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-03-27 19:54:45.733438 colorist-1.3.0/src/colorist/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      253 2023-01-25 13:58:40.000000 colorist-1.3.0/src/colorist/model/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      528 2023-03-27 19:53:45.000000 colorist-1.3.0/src/colorist/model/background_bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      473 2023-03-27 19:53:45.000000 colorist-1.3.0/src/colorist/model/background_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      467 2023-03-27 19:53:45.000000 colorist-1.3.0/src/colorist/model/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      433 2023-03-27 19:53:45.000000 colorist-1.3.0/src/colorist/model/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      556 2023-03-27 19:53:45.000000 colorist-1.3.0/src/colorist/model/effect.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.3.0/src/colorist/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-03-27 19:47:43.000000 colorist-1.3.0/src/colorist/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-03-27 19:54:45.732369 colorist-1.3.0/src/colorist.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    17717 2023-03-27 19:54:45.000000 colorist-1.3.0/src/colorist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      636 2023-03-27 19:54:45.000000 colorist-1.3.0/src/colorist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-03-27 19:54:45.000000 colorist-1.3.0/src/colorist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.3.0/src/colorist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       96 2023-03-27 19:54:45.000000 colorist-1.3.0/src/colorist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2023-03-27 19:54:45.000000 colorist-1.3.0/src/colorist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.478059 colorist-1.4.0/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1687 2023-04-02 10:14:25.000000 colorist-1.4.0/INSTALLATION.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.4.0/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 10:14:25.000000 colorist-1.4.0/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    22625 2023-04-10 22:26:56.478197 colorist-1.4.0/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    18625 2023-04-10 22:24:39.000000 colorist-1.4.0/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:58:40.000000 colorist-1.4.0/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1436 2023-04-10 22:26:56.478548 colorist-1.4.0/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.467869 colorist-1.4.0/src/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.470110 colorist-1.4.0/src/colorist/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2456 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.472041 colorist-1.4.0/src/colorist/constants/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/constants/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2229 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/constants/ansi.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/constants/ascii.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.473784 colorist-1.4.0/src/colorist/helper/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.4.0/src/colorist/helper/.coverage
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.474492 colorist-1.4.0/src/colorist/helper/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.468147 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.474941 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1399 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/convert.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      564 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/error.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/generate.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/helper/print.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      316 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/validate.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.475481 colorist-1.4.0/src/colorist/model/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1508 2023-04-09 22:59:24.000000 colorist-1.4.0/src/colorist/model/README.MD
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.476001 colorist-1.4.0/src/colorist/model/abc/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-10 22:22:29.000000 colorist-1.4.0/src/colorist/model/abc/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-10 22:22:29.000000 colorist-1.4.0/src/colorist/model/abc/effect.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/abc/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/abc/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.476439 colorist-1.4.0/src/colorist/model/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      417 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      412 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.476884 colorist-1.4.0/src/colorist/model/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      420 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      415 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.477012 colorist-1.4.0/src/colorist/print/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.477469 colorist-1.4.0/src/colorist/print/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2509 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1320 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      518 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      355 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1395 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.477933 colorist-1.4.0/src/colorist/print/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2331 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1142 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      498 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      335 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.4.0/src/colorist/py.typed
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2023-04-10 22:24:39.000000 colorist-1.4.0/src/colorist/version.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.471135 colorist-1.4.0/src/colorist.egg-info/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    22625 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1756 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.4.0/src/colorist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/top_level.txt
```

### Comparing `colorist-1.3.0/PKG-INFO` & `colorist-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,221 +1,182 @@
-Metadata-Version: 2.1
-Name: colorist
-Version: 1.3.0
-Summary: Colorist for Python
-Home-page: https://github.com/jakob-bagterp/colorist-for-python
-Author: Jakob Bagterp
-Author-email: jakob_bagterp@hotmail.com
-Maintainer: Jakob Bagterp
-Maintainer-email: jakob_bagterp@hotmail.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/jakob-bagterp/colorist-for-python/issues
-Keywords: python,colors,terminal
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE.md
-
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.3.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
 ![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
-[![MIT license](https://img.shields.io/static/v1?label=license&message=MIT&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
+[![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 Colorist for Python 🌈
-Lightweight Python package that makes it easy and fast to print terminal messages in colors.
-
-## Prerequisites
-* Python 3.10 or higher
-
-## Installation
-### PyPI
-Assuming that Python is installed already, execute this command in the terminal:
-
-```shell
-pip3 install colorist
-```
-
-If you already have installed Colorist for Python, use this command to upgrade to latest version:
-
-```shell
-pip3 install --upgrade colorist
-```
-
-### Homebrew
-If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Colorist for Python:
-
-```shell
-brew tap jakob-bagterp/colorist
-```
-
-And then install:
+Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
-```shell
-brew install colorist
-```
+Ready to try? [Learn how to install](https://github.com/jakob-bagterp/colorist-for-python/blob/master/INSTALLATION.md).
 
-## Text Colors
-### Getting Started
-#### Full Terminal Output
+## Getting Started
+### Print Line of Colored Text
 How to print a full line of colored text in the terminal:
 
 ```python
 from colorist import green, yellow, red
 
 green("This is GREEN!")
 yellow("This is YELLOW!")
 red("This is RED!")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red text color](/assets/images/examples/color_full_text_green_yellow_red.png)
+![Example of full line of green, yellow, red colored text printed in a terminal window](/assets/images/examples/color_full_text_green_yellow_red.png)
 
-#### Custom Terminal Output
-How to customize terminal messages and change color inside a paragraph:
+### Print Mixed Text Colors
+How to customize colors inside a paragraph and print it in the terminal:
 
 ```python
 from colorist import Color
 
 print(f"I want {Color.RED}red{Color.OFF} color inside this paragraph")
 
 print(f"Both {Color.GREEN}green{Color.OFF} and {Color.YELLOW}yellow{Color.OFF} are nice colors")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red text color](/assets/images/examples/color_custom_text_green_yellow_red.png)
+![Example of white text mixed with green, yellow, red colors printed in a terminal window](/assets/images/examples/color_custom_text_green_yellow_red.png)
 
+## Other Styling Options
+### Print Bright Colors
+Most terminals support bright colors that stand more out:
 
 ```python
 from colorist import BrightColor
 
 print(f"I want {BrightColor.CYAN}cyan{BrightColor.OFF} color inside this paragraph")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with cyan text color](/assets/images/examples/bright_color_custom_text_cyan.png)
+![Example of white text mixed with cyan printed in a terminal window](/assets/images/examples/bright_color_custom_text_cyan.png)
 
 Remember to use `Color.OFF` or `BrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
 
-##### Other String Formats
-It's easier and more readable to use f-strings as in the examples above, but you can also use string format:
+### Print Background Colors
+```python
+from colorist import bg_green, bg_yellow, bg_red
+
+bg_green("This is GREEN background!")
+bg_yellow("This is YELLOW background!")
+bg_red("This is RED background!")
+```
+
+How it appears in the terminal:
+
+![Example of white text and colored backgrounds if green, yellow, red printed in a terminal window](/assets/images/examples/bg_color_full_text_green_yellow_red.png)
+
+Background colors can also be mixed inside a paragraph:
+
+```python
+from colorist import BgColor
+
+print(f"I want {BgColor.RED}red{BgColor.OFF} background color inside this paragraph")
+
+print(f"Both {BgColor.GREEN}green{BgColor.OFF} and {BgColor.YELLOW}yellow{BgColor.OFF} are nice background colors")
+```
+
+How it appears in the terminal:
+
+![Example of black, green, yellow, red background colors mixed inside paragraph printed in a terminal window](/assets/images/examples/bg_color_custom_text_green_yellow_red.png)
+
+
+```python
+from colorist import BgBrightColor
+
+print(f"I want {BgBrightColor.CYAN}cyan{BgBrightColor.OFF} background color inside this paragraph")
+```
+
+How it appears in the terminal:
+
+![Example of white text on a cyan background color printed in a terminal window](/assets/images/examples/bg_bright_color_custom_text_cyan.png)
+
+As with text colors, remember to use `BgColor.OFF` or `BgBrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
+
+### Other String Formats
+It's often easier and more readable to use [f-strings](https://peps.python.org/pep-0498/) as in the examples above, but f-strings aren't supported in some earlier versions of Python. Instead, you can also use string formatting or concatenation:
 
 ```python
 from colorist import Color
 
 print("I want {0}red{1} color inside this paragraph".format(Color.RED, Color.OFF))
+print("I want " + Color.RED + "red" + Color.OFF + " color inside this paragraph")
 ```
 
-How it appears in the terminal:
+Both options appear the same in the terminal:
 
 ![Example of terminal message with red text color](/assets/images/examples/color_custom_text_red.png)
 
-### Supported Text Colors
-| Color | Full Text Function | Custom | Example |
-| ----- | ------------------ | ------ | ------- |
-| ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
-| ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
-| ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
-| ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
-| ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
-| ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
-| ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
-| ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
-| - | - | `Color.OFF` | - |
-| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
-| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
-| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
-| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
-| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
-| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
-| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
-| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
-| - | - | `BrightColor.OFF` | - |
+### Print RGB and HSL Colors
+Note that not all terminals support RGB or HSL colors. If your terminal does support such advanced colors, read on.
 
-## Background Colors
-### Getting Started
-#### Full Terminal Output
-How to print a full line of text with colored background in the terminal:
+#### RGB Colors
+Try the `rgb` and `bg_rgb` methods for a full line of colored text. The values for red, green, blue can be an integer between `0-255`.
 
 ```python
-from colorist import bg_green, bg_yellow, bg_red
+from colorist import rgb, bg_rgb
 
-bg_green("This is GREEN background!")
-bg_yellow("This is YELLOW background!")
-bg_red("This is RED background!")
+rgb("I want this text in blue RGB colors", 0, 128, 255)
+bg_rgb("I want this background in blue RGB colors", 0, 128, 255)
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red background color](/assets/images/examples/bg_color_full_text_green_yellow_red.png)
+![Example of text in RGB colors printed in a terminal window](/assets/images/examples/rgb_full_text.png)
 
-#### Custom Terminal Output
-How to customize terminal messages and change background color inside a paragraph:
+Or customize the styling of text and background with the `ColorRGB` and `BgColorRGB` classes:
 
 ```python
-from colorist import BgColor
+from colorist import ColorRGB, BgColorRGB
 
-print(f"I want {BgColor.RED}red{BgColor.OFF} background color inside this paragraph")
+dusty_pink = ColorRGB(194, 145, 164)
+bg_steel_blue = BgColorRGB(70, 130, 180)
 
-print(f"Both {BgColor.GREEN}green{BgColor.OFF} and {BgColor.YELLOW}yellow{BgColor.OFF} are nice background colors")
+print(f"I want to use {dusty_pink}dusty pink{dusty_pink.OFF} and {bg_steel_blue}steel blue{bg_steel_blue.OFF} colors inside this paragraph")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red background color](/assets/images/examples/bg_color_custom_text_green_yellow_red.png)
+![Another example of text in RGB colors printed in a terminal window](/assets/images/examples/rgb_custom_text.png)
+
+#### HSL Colors
+Similarly, you can also output colors in HSL with the `hsl` and `bg_hsl` methods. The value for hue can be between `0-360` degrees, while saturation and lightness can be a percentage between `0-100` %:
 
 ```python
-from colorist import BgBrightColor
+from colorist import hsl, bg_hsl
 
-print(f"I want {BgBrightColor.CYAN}cyan{BgBrightColor.OFF} background color inside this paragraph")
+hsl("I want this text in green HSL colors", 120, 50, 50)
+bg_hsl("I want this background in green HSL colors", 120, 50, 50)
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with cyan background color](/assets/images/examples/bg_bright_color_custom_text_cyan.png)
+![Example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_full_text.png)
 
-As with text colors, remember to use `BgColor.OFF` or `BgBrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
+Or customize the styling of text and background with the `ColorHSL` and `BgColorHSL` classes:
 
-### Supported Background Colors
-| Color | Full Text Function | Custom | Example |
-| ----- | ------------------ | ------ | ------- |
-| ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
-| ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
-| ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
-| ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
-| ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
-| ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
-| ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
-| ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
-| - | - | `BgColor.OFF` | - |
-| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
-| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
-| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
-| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
-| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
-| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
-| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
-| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
-| - | - | `BgBrightColor.OFF` | - |
+```python
+from colorist import ColorHSL, BgColorHSL
 
-## Effects
-### Getting Started
-In addition to colors, Colorist for Python can also add effects to text messages in the terminal.
+mustard_green = ColorHSL(60, 56, 43)
+bg_steel_gray = BgColorHSL(190, 2, 49)
+
+print(f"I want to use {mustard_green}mustard green{mustard_green.OFF} and {bg_steel_gray}steel blue{bg_steel_gray.OFF} colors inside this paragraph")
+```
+
+How it appears in the terminal:
+
+![Another example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_custom_text.png)
 
-#### Full Terminal Output
-How to print a full line of text effect in the terminal:
+### Print Effects and Other Styles
+In addition to colors, Colorist can also add effects when you print text in the terminal. How to print a full line of text with effects:
 
 ```python
 from colorist import effect_blink
 
 effect_blink("This is BLINKING!")
 ```
 
@@ -231,15 +192,14 @@
 effect_blink("This is BLINKING!", Color.CYAN)
 ```
 
 How it appears in the terminal:
 
 ![Example of terminal message with blinking, cyan-colored text](/assets/images/examples/effect_full_text_blink_cyan.gif)
 
-#### Custom Terminal Output
 How to customize terminal messages and change effect inside a paragraph:
 
 ```python
 from colorist import Effect
 
 print(f"I want {Effect.UNDERLINE}underlined text{Effect.UNDERLINE_OFF} inside this paragraph")
 
@@ -260,38 +220,80 @@
 
 How it appears in the terminal:
 
 ![Example of terminal message with red and blinking text](/assets/images/examples/effect_custom_text_blink_red.gif)
 
 Similar to `Color.OFF`, remember to turn off an effect with the relevant reset option (e.g `Effect.BOLD_OFF`, `Effect.DIM_OFF`, etc. or even just `Effect.OFF`) every time you want to revert back to the default terminal text style. Otherwise the effect may spill over and into other terminal messages.
 
-### Supported Effects
+# Supported Colors and Styles
+Colorist is based on [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code), a standard that defines colors, styling and effects for text in terminal windows. Note that most terminals support all color options, but not all:
+
+| Category                                               | Color Options                                      |
+| ------------------------------------------------------ | -------------------------------------------------- |
+| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                       |
+| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                     |
+| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL` |
+
+## Foreground Text
+| Color | Full Text Function | Custom | Example |
+| ----- | ------------------ | ------ | ------- |
+| ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
+| ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
+| ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
+| ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
+| ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
+| ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
+| ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
+| ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
+| - | - | `Color.OFF` | - |
+| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
+| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
+| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
+| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
+| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
+| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
+| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
+| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
+| - | - | `BrightColor.OFF` | - |
+
+## Background
+| Color | Full Text Function | Custom | Example |
+| ----- | ------------------ | ------ | ------- |
+| ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
+| ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
+| ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
+| ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
+| ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
+| ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
+| ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
+| ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
+| - | - | `BgColor.OFF` | - |
+| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
+| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
+| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
+| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
+| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
+| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
+| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
+| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
+| - | - | `BgBrightColor.OFF` | - |
+
+## Effects
 | Effect           | Full Text Function         | Custom             | Reset                  | Example    |
 | ---------------- | -------------------------- | ------------------ | ---------------------- | ---------- |
 | **Bold**         | `effect_bold("text")`      | `Effect.BOLD`      | `Effect.BOLD_OFF`      | ![Example of terminal message with bold text](/assets/images/examples/effect_map/bold_full_text_140x16.png) |
 | Dim              | `effect_dim("text")`       | `Effect.DIM`       | `Effect.DIM_OFF`       | ![Example of terminal message with dimmed text](/assets/images/examples/effect_map/dim_full_text_140x16.png) |
 | <u>Underline</u> | `effect_underline("text")` | `Effect.UNDERLINE` | `Effect.UNDERLINE_OFF` | ![Example of terminal message with underlined text](/assets/images/examples/effect_map/underline_full_text_140x16.png) |
 | Blink            | `effect_blink("text")`     | `Effect.BLINK`     | `Effect.BLINK_OFF`     | ![Example of terminal message with blinking text](/assets/images/examples/effect_map/blink_full_text_140x16.gif) |
 | Reverse          | `effect_reverse("text")`   | `Effect.REVERSE`   | `Effect.REVERSE_OFF`   | ![Example of terminal message with reversed text color and background](/assets/images/examples/effect_map/reverse_full_text_140x16.png) |
 | Hide             | `effect_hide("text")`      | `Effect.HIDE`      | `Effect.HIDE_OFF`      | ![Example of terminal message with hidden text](/assets/images/examples/effect_map/hide_full_text_140x16.png) |
 | -                | -                          | -                  | `Effect.OFF`           | -          |
 
+# Thank You for Supporting
 ## Donate
 This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/colorist-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/colorist-for-python/issues).
-
-# MIT License
-
-Copyright (c) 2022 – present Jakob Bagterp
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `colorist-1.3.0/setup.cfg` & `colorist-1.4.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -2,48 +2,48 @@
 name = colorist
 version = attr: colorist.__version__
 author = Jakob Bagterp
 author_email = jakob_bagterp@hotmail.com
 maintainer = Jakob Bagterp
 maintainer_email = jakob_bagterp@hotmail.com
 description = Colorist for Python
-long_description = file: README.md, LICENSE.md
+long_description = file: README.md, INSTALLATION.md, LICENSE.md
 long_description_content_type = text/markdown
 keywords = 
 	python
 	colors
 	terminal
 url = https://github.com/jakob-bagterp/colorist-for-python
 project_urls = 
 	Bug Tracker = https://github.com/jakob-bagterp/colorist-for-python/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
-	License :: OSI Approved :: MIT License
+	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
-license = MIT License
+license = 3-Clause BSD License
 license_files = LICENSE.md
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
-	coverage ==7.2.2
+	coverage ==7.2.3
 	flake8 ==6.0.0
-	mypy ==1.1.1
-	pytest ==7.2.2
+	mypy ==1.2.0
+	pytest ==7.3.0
 	pytest-cov ==4.0.0
-	tox ==4.4.8
+	tox ==4.4.11
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 colorist = py.typed
```

### Comparing `colorist-1.3.0/src/colorist.egg-info/PKG-INFO` & `colorist-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,205 @@
 Metadata-Version: 2.1
 Name: colorist
-Version: 1.3.0
+Version: 1.4.0
 Summary: Colorist for Python
 Home-page: https://github.com/jakob-bagterp/colorist-for-python
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
-License: MIT License
+License: 3-Clause BSD License
 Project-URL: Bug Tracker, https://github.com/jakob-bagterp/colorist-for-python/issues
 Keywords: python,colors,terminal
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.3.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
 ![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
-[![MIT license](https://img.shields.io/static/v1?label=license&message=MIT&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
+[![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 Colorist for Python 🌈
-Lightweight Python package that makes it easy and fast to print terminal messages in colors.
-
-## Prerequisites
-* Python 3.10 or higher
-
-## Installation
-### PyPI
-Assuming that Python is installed already, execute this command in the terminal:
-
-```shell
-pip3 install colorist
-```
-
-If you already have installed Colorist for Python, use this command to upgrade to latest version:
-
-```shell
-pip3 install --upgrade colorist
-```
-
-### Homebrew
-If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Colorist for Python:
-
-```shell
-brew tap jakob-bagterp/colorist
-```
-
-And then install:
+Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
-```shell
-brew install colorist
-```
+Ready to try? [Learn how to install](https://github.com/jakob-bagterp/colorist-for-python/blob/master/INSTALLATION.md).
 
-## Text Colors
-### Getting Started
-#### Full Terminal Output
+## Getting Started
+### Print Line of Colored Text
 How to print a full line of colored text in the terminal:
 
 ```python
 from colorist import green, yellow, red
 
 green("This is GREEN!")
 yellow("This is YELLOW!")
 red("This is RED!")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red text color](/assets/images/examples/color_full_text_green_yellow_red.png)
+![Example of full line of green, yellow, red colored text printed in a terminal window](/assets/images/examples/color_full_text_green_yellow_red.png)
 
-#### Custom Terminal Output
-How to customize terminal messages and change color inside a paragraph:
+### Print Mixed Text Colors
+How to customize colors inside a paragraph and print it in the terminal:
 
 ```python
 from colorist import Color
 
 print(f"I want {Color.RED}red{Color.OFF} color inside this paragraph")
 
 print(f"Both {Color.GREEN}green{Color.OFF} and {Color.YELLOW}yellow{Color.OFF} are nice colors")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red text color](/assets/images/examples/color_custom_text_green_yellow_red.png)
+![Example of white text mixed with green, yellow, red colors printed in a terminal window](/assets/images/examples/color_custom_text_green_yellow_red.png)
 
+## Other Styling Options
+### Print Bright Colors
+Most terminals support bright colors that stand more out:
 
 ```python
 from colorist import BrightColor
 
 print(f"I want {BrightColor.CYAN}cyan{BrightColor.OFF} color inside this paragraph")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with cyan text color](/assets/images/examples/bright_color_custom_text_cyan.png)
+![Example of white text mixed with cyan printed in a terminal window](/assets/images/examples/bright_color_custom_text_cyan.png)
 
 Remember to use `Color.OFF` or `BrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
 
-##### Other String Formats
-It's easier and more readable to use f-strings as in the examples above, but you can also use string format:
+### Print Background Colors
+```python
+from colorist import bg_green, bg_yellow, bg_red
+
+bg_green("This is GREEN background!")
+bg_yellow("This is YELLOW background!")
+bg_red("This is RED background!")
+```
+
+How it appears in the terminal:
+
+![Example of white text and colored backgrounds if green, yellow, red printed in a terminal window](/assets/images/examples/bg_color_full_text_green_yellow_red.png)
+
+Background colors can also be mixed inside a paragraph:
+
+```python
+from colorist import BgColor
+
+print(f"I want {BgColor.RED}red{BgColor.OFF} background color inside this paragraph")
+
+print(f"Both {BgColor.GREEN}green{BgColor.OFF} and {BgColor.YELLOW}yellow{BgColor.OFF} are nice background colors")
+```
+
+How it appears in the terminal:
+
+![Example of black, green, yellow, red background colors mixed inside paragraph printed in a terminal window](/assets/images/examples/bg_color_custom_text_green_yellow_red.png)
+
+
+```python
+from colorist import BgBrightColor
+
+print(f"I want {BgBrightColor.CYAN}cyan{BgBrightColor.OFF} background color inside this paragraph")
+```
+
+How it appears in the terminal:
+
+![Example of white text on a cyan background color printed in a terminal window](/assets/images/examples/bg_bright_color_custom_text_cyan.png)
+
+As with text colors, remember to use `BgColor.OFF` or `BgBrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
+
+### Other String Formats
+It's often easier and more readable to use [f-strings](https://peps.python.org/pep-0498/) as in the examples above, but f-strings aren't supported in some earlier versions of Python. Instead, you can also use string formatting or concatenation:
 
 ```python
 from colorist import Color
 
 print("I want {0}red{1} color inside this paragraph".format(Color.RED, Color.OFF))
+print("I want " + Color.RED + "red" + Color.OFF + " color inside this paragraph")
 ```
 
-How it appears in the terminal:
+Both options appear the same in the terminal:
 
 ![Example of terminal message with red text color](/assets/images/examples/color_custom_text_red.png)
 
-### Supported Text Colors
-| Color | Full Text Function | Custom | Example |
-| ----- | ------------------ | ------ | ------- |
-| ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
-| ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
-| ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
-| ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
-| ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
-| ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
-| ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
-| ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
-| - | - | `Color.OFF` | - |
-| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
-| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
-| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
-| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
-| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
-| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
-| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
-| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
-| - | - | `BrightColor.OFF` | - |
+### Print RGB and HSL Colors
+Note that not all terminals support RGB or HSL colors. If your terminal does support such advanced colors, read on.
 
-## Background Colors
-### Getting Started
-#### Full Terminal Output
-How to print a full line of text with colored background in the terminal:
+#### RGB Colors
+Try the `rgb` and `bg_rgb` methods for a full line of colored text. The values for red, green, blue can be an integer between `0-255`.
 
 ```python
-from colorist import bg_green, bg_yellow, bg_red
+from colorist import rgb, bg_rgb
 
-bg_green("This is GREEN background!")
-bg_yellow("This is YELLOW background!")
-bg_red("This is RED background!")
+rgb("I want this text in blue RGB colors", 0, 128, 255)
+bg_rgb("I want this background in blue RGB colors", 0, 128, 255)
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red background color](/assets/images/examples/bg_color_full_text_green_yellow_red.png)
+![Example of text in RGB colors printed in a terminal window](/assets/images/examples/rgb_full_text.png)
 
-#### Custom Terminal Output
-How to customize terminal messages and change background color inside a paragraph:
+Or customize the styling of text and background with the `ColorRGB` and `BgColorRGB` classes:
 
 ```python
-from colorist import BgColor
+from colorist import ColorRGB, BgColorRGB
 
-print(f"I want {BgColor.RED}red{BgColor.OFF} background color inside this paragraph")
+dusty_pink = ColorRGB(194, 145, 164)
+bg_steel_blue = BgColorRGB(70, 130, 180)
 
-print(f"Both {BgColor.GREEN}green{BgColor.OFF} and {BgColor.YELLOW}yellow{BgColor.OFF} are nice background colors")
+print(f"I want to use {dusty_pink}dusty pink{dusty_pink.OFF} and {bg_steel_blue}steel blue{bg_steel_blue.OFF} colors inside this paragraph")
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with green, yellow, red background color](/assets/images/examples/bg_color_custom_text_green_yellow_red.png)
+![Another example of text in RGB colors printed in a terminal window](/assets/images/examples/rgb_custom_text.png)
+
+#### HSL Colors
+Similarly, you can also output colors in HSL with the `hsl` and `bg_hsl` methods. The value for hue can be between `0-360` degrees, while saturation and lightness can be a percentage between `0-100` %:
 
 ```python
-from colorist import BgBrightColor
+from colorist import hsl, bg_hsl
 
-print(f"I want {BgBrightColor.CYAN}cyan{BgBrightColor.OFF} background color inside this paragraph")
+hsl("I want this text in green HSL colors", 120, 50, 50)
+bg_hsl("I want this background in green HSL colors", 120, 50, 50)
 ```
 
 How it appears in the terminal:
 
-![Example of terminal message with cyan background color](/assets/images/examples/bg_bright_color_custom_text_cyan.png)
+![Example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_full_text.png)
 
-As with text colors, remember to use `BgColor.OFF` or `BgBrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
+Or customize the styling of text and background with the `ColorHSL` and `BgColorHSL` classes:
 
-### Supported Background Colors
-| Color | Full Text Function | Custom | Example |
-| ----- | ------------------ | ------ | ------- |
-| ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
-| ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
-| ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
-| ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
-| ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
-| ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
-| ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
-| ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
-| - | - | `BgColor.OFF` | - |
-| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
-| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
-| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
-| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
-| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
-| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
-| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
-| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
-| - | - | `BgBrightColor.OFF` | - |
+```python
+from colorist import ColorHSL, BgColorHSL
 
-## Effects
-### Getting Started
-In addition to colors, Colorist for Python can also add effects to text messages in the terminal.
+mustard_green = ColorHSL(60, 56, 43)
+bg_steel_gray = BgColorHSL(190, 2, 49)
+
+print(f"I want to use {mustard_green}mustard green{mustard_green.OFF} and {bg_steel_gray}steel blue{bg_steel_gray.OFF} colors inside this paragraph")
+```
+
+How it appears in the terminal:
+
+![Another example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_custom_text.png)
 
-#### Full Terminal Output
-How to print a full line of text effect in the terminal:
+### Print Effects and Other Styles
+In addition to colors, Colorist can also add effects when you print text in the terminal. How to print a full line of text with effects:
 
 ```python
 from colorist import effect_blink
 
 effect_blink("This is BLINKING!")
 ```
 
@@ -231,15 +215,14 @@
 effect_blink("This is BLINKING!", Color.CYAN)
 ```
 
 How it appears in the terminal:
 
 ![Example of terminal message with blinking, cyan-colored text](/assets/images/examples/effect_full_text_blink_cyan.gif)
 
-#### Custom Terminal Output
 How to customize terminal messages and change effect inside a paragraph:
 
 ```python
 from colorist import Effect
 
 print(f"I want {Effect.UNDERLINE}underlined text{Effect.UNDERLINE_OFF} inside this paragraph")
 
@@ -260,38 +243,137 @@
 
 How it appears in the terminal:
 
 ![Example of terminal message with red and blinking text](/assets/images/examples/effect_custom_text_blink_red.gif)
 
 Similar to `Color.OFF`, remember to turn off an effect with the relevant reset option (e.g `Effect.BOLD_OFF`, `Effect.DIM_OFF`, etc. or even just `Effect.OFF`) every time you want to revert back to the default terminal text style. Otherwise the effect may spill over and into other terminal messages.
 
-### Supported Effects
+# Supported Colors and Styles
+Colorist is based on [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code), a standard that defines colors, styling and effects for text in terminal windows. Note that most terminals support all color options, but not all:
+
+| Category                                               | Color Options                                      |
+| ------------------------------------------------------ | -------------------------------------------------- |
+| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                       |
+| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                     |
+| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL` |
+
+## Foreground Text
+| Color | Full Text Function | Custom | Example |
+| ----- | ------------------ | ------ | ------- |
+| ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
+| ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
+| ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
+| ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
+| ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
+| ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
+| ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
+| ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
+| - | - | `Color.OFF` | - |
+| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
+| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
+| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
+| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
+| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
+| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
+| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
+| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
+| - | - | `BrightColor.OFF` | - |
+
+## Background
+| Color | Full Text Function | Custom | Example |
+| ----- | ------------------ | ------ | ------- |
+| ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
+| ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
+| ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
+| ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
+| ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
+| ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
+| ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
+| ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
+| - | - | `BgColor.OFF` | - |
+| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
+| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
+| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
+| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
+| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
+| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
+| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
+| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
+| - | - | `BgBrightColor.OFF` | - |
+
+## Effects
 | Effect           | Full Text Function         | Custom             | Reset                  | Example    |
 | ---------------- | -------------------------- | ------------------ | ---------------------- | ---------- |
 | **Bold**         | `effect_bold("text")`      | `Effect.BOLD`      | `Effect.BOLD_OFF`      | ![Example of terminal message with bold text](/assets/images/examples/effect_map/bold_full_text_140x16.png) |
 | Dim              | `effect_dim("text")`       | `Effect.DIM`       | `Effect.DIM_OFF`       | ![Example of terminal message with dimmed text](/assets/images/examples/effect_map/dim_full_text_140x16.png) |
 | <u>Underline</u> | `effect_underline("text")` | `Effect.UNDERLINE` | `Effect.UNDERLINE_OFF` | ![Example of terminal message with underlined text](/assets/images/examples/effect_map/underline_full_text_140x16.png) |
 | Blink            | `effect_blink("text")`     | `Effect.BLINK`     | `Effect.BLINK_OFF`     | ![Example of terminal message with blinking text](/assets/images/examples/effect_map/blink_full_text_140x16.gif) |
 | Reverse          | `effect_reverse("text")`   | `Effect.REVERSE`   | `Effect.REVERSE_OFF`   | ![Example of terminal message with reversed text color and background](/assets/images/examples/effect_map/reverse_full_text_140x16.png) |
 | Hide             | `effect_hide("text")`      | `Effect.HIDE`      | `Effect.HIDE_OFF`      | ![Example of terminal message with hidden text](/assets/images/examples/effect_map/hide_full_text_140x16.png) |
 | -                | -                          | -                  | `Effect.OFF`           | -          |
 
+# Thank You for Supporting
 ## Donate
 This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/colorist-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/colorist-for-python/issues).
 
-# MIT License
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.3.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
+
+# 🌈 How to Install Colorist for Python 🌈
+## Prerequisites
+* Python 3.10 or higher
+* Terminal that supports color (i.e. [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code))
+
+## Installation
+### PyPI
+Assuming that Python is installed already, execute this command in the terminal:
+
+```shell
+pip3 install colorist
+```
+
+If you already have installed Colorist for Python, use this command to upgrade to latest version:
+
+```shell
+pip3 install --upgrade colorist
+```
+
+### Homebrew
+If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Colorist for Python:
+
+```shell
+brew tap jakob-bagterp/colorist
+```
+
+And then install:
+
+```shell
+brew install colorist
+```
+
+## Getting Started
+Ready to go? [Learn how to use Colorist](https://github.com/jakob-bagterp/colorist-for-python/blob/master/README.md).
+
+# 3-Clause BSD License
+
+Copyright (c) 2022 – present, Jakob Bagterp
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-Copyright (c) 2022 – present Jakob Bagterp
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

