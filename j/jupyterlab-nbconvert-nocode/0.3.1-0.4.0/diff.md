# Comparing `tmp/jupyterlab_nbconvert_nocode-0.3.1.tar.gz` & `tmp/jupyterlab_nbconvert_nocode-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_nbconvert_nocode-0.3.1.tar", last modified: Mon Aug 16 03:45:08 2021, max compression
+gzip compressed data, was "jupyterlab_nbconvert_nocode-0.4.0.tar", last modified: Tue Apr 11 13:49:27 2023, max compression
```

## Comparing `jupyterlab_nbconvert_nocode-0.3.1.tar` & `jupyterlab_nbconvert_nocode-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.093901 jupyterlab_nbconvert_nocode-0.3.1/
--rw-r--r--   0 theocean154   (501) staff       (20)      415 2021-08-16 02:51:59.000000 jupyterlab_nbconvert_nocode-0.3.1/.bumpversion.cfg
--rw-r--r--   0 theocean154   (501) staff       (20)     1954 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 theocean154   (501) staff       (20)    11357 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/LICENSE
--rw-r--r--   0 theocean154   (501) staff       (20)      388 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/MANIFEST.in
--rw-r--r--   0 theocean154   (501) staff       (20)     1387 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/Makefile
--rw-r--r--   0 theocean154   (501) staff       (20)     1684 2021-08-16 03:45:08.094111 jupyterlab_nbconvert_nocode-0.3.1/PKG-INFO
--rw-r--r--   0 theocean154   (501) staff       (20)      966 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/README.md
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.083608 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/
--rw-r--r--   0 theocean154   (501) staff       (20)       48 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)      683 2021-08-16 02:51:59.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/_version.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.087440 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/nbconvert_functions/
--rw-r--r--   0 theocean154   (501) staff       (20)      110 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/nbconvert_functions/__init__.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.088881 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/
--rw-r--r--   0 theocean154   (501) staff       (20)       61 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)     1211 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/exporters.py
--rw-r--r--   0 theocean154   (501) staff       (20)      221 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/utils.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.089905 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/tests/
--rw-r--r--   0 theocean154   (501) staff       (20)        0 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/tests/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)      174 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/tests/test_all.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.086976 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/
--rw-r--r--   0 theocean154   (501) staff       (20)     1684 2021-08-16 03:45:07.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/PKG-INFO
--rw-r--r--   0 theocean154   (501) staff       (20)     1314 2021-08-16 03:45:07.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/SOURCES.txt
--rw-r--r--   0 theocean154   (501) staff       (20)        1 2021-08-16 03:45:07.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/dependency_links.txt
--rw-r--r--   0 theocean154   (501) staff       (20)      227 2021-08-16 03:45:07.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/entry_points.txt
--rw-r--r--   0 theocean154   (501) staff       (20)        1 2021-08-13 01:27:54.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/not-zip-safe
--rw-r--r--   0 theocean154   (501) staff       (20)      207 2021-08-16 03:45:07.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/requires.txt
--rw-r--r--   0 theocean154   (501) staff       (20)       28 2021-08-16 03:45:07.000000 jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/top_level.txt
--rw-r--r--   0 theocean154   (501) staff       (20)      127 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/pyproject.toml
--rw-r--r--   0 theocean154   (501) staff       (20)      407 2021-08-16 03:45:08.095007 jupyterlab_nbconvert_nocode-0.3.1/setup.cfg
--rw-r--r--   0 theocean154   (501) staff       (20)     2104 2021-08-13 01:24:28.000000 jupyterlab_nbconvert_nocode-0.3.1/setup.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.078413 jupyterlab_nbconvert_nocode-0.3.1/share/
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.078515 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.078618 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.079044 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.091153 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_html/
--rw-r--r--   0 theocean154   (501) staff       (20)      229 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_html/conf.json
--rw-r--r--   0 theocean154   (501) staff       (20)      366 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_html/index.html.j2
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.092341 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_html_email/
--rw-r--r--   0 theocean154   (501) staff       (20)      229 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_html_email/conf.json
--rw-r--r--   0 theocean154   (501) staff       (20)     5423 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_html_email/index.html.j2
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2021-08-16 03:45:08.093406 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_pdf/
--rw-r--r--   0 theocean154   (501) staff       (20)      127 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_pdf/conf.json
--rw-r--r--   0 theocean154   (501) staff       (20)     7694 2021-08-16 02:24:58.000000 jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_pdf/index.tex.j2
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.580429 jupyterlab_nbconvert_nocode-0.4.0/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5222 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1954 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11357 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      470 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1882 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1739 2023-04-11 13:49:27.580481 jupyterlab_nbconvert_nocode-0.4.0/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      966 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.576955 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       48 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       22 2023-04-11 13:47:45.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/_version.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.578027 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/nbconvert_functions/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      110 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/nbconvert_functions/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.578725 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       61 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1211 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/exporters.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      221 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.579328 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)   141973 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/tests/Test.ipynb
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/tests/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      174 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/tests/test_all.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.577917 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1739 2023-04-11 13:49:27.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1361 2023-04-11 13:49:27.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-11 13:49:27.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)      226 2023-04-11 13:49:27.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-11 13:49:27.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/not-zip-safe
+-rw-r--r--   0 timkpaine   (501) staff       (20)      442 2023-04-11 13:49:27.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       28 2023-04-11 13:49:27.000000 jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       73 2023-04-11 13:39:52.000000 jupyterlab_nbconvert_nocode-0.4.0/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)      803 2023-04-11 13:49:27.580826 jupyterlab_nbconvert_nocode-0.4.0/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2119 2023-04-11 13:49:24.000000 jupyterlab_nbconvert_nocode-0.4.0/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.574576 jupyterlab_nbconvert_nocode-0.4.0/share/
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.574618 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.574661 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.574830 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.579635 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_html/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      229 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_html/conf.json
+-rw-r--r--   0 timkpaine   (501) staff       (20)      366 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_html/index.html.j2
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.579940 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_html_email/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      229 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_html_email/conf.json
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5423 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_html_email/index.html.j2
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-11 13:49:27.580245 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_pdf/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      127 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_pdf/conf.json
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7694 2023-04-11 13:33:26.000000 jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_pdf/index.tex.j2
```

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/CONTRIBUTING.md` & `jupyterlab_nbconvert_nocode-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/LICENSE` & `jupyterlab_nbconvert_nocode-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/PKG-INFO` & `jupyterlab_nbconvert_nocode-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbconvert_nocode
-Version: 0.3.1
+Version: 0.4.0
 Summary: A simple helper library with 2 NBConvert exporters for PDF/HTML export with no code cells
 Home-page: https://github.com/timkpaine/jupyterlab_nbconvert_nocode
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: jupyter jupyterlab
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Jupyter
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: develop
 License-File: LICENSE
 
 # jupyterlab_nbconvert_nocode
 A simple helper library with 2 NBConvert exporters for PDF/HTML export with no code cells
 
 [![Build Status](https://github.com/timkpaine/jupyterlab_nbconvert_nocode/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/jupyterlab_nbconvert_nocode/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/timkpaine/jupyterlab_nbconvert_nocode/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/jupyterlab_nbconvert_nocode)
 [![GitHub issues](https://img.shields.io/github/issues/timkpaine/jupyterlab_nbconvert_nocode.svg)]()
 [![PyPI](https://img.shields.io/pypi/l/jupyterlab_nbconvert_nocode.svg)](https://pypi.python.org/pypi/jupyterlab_nbconvert_nocode)
 [![PyPI](https://img.shields.io/pypi/v/jupyterlab_nbconvert_nocode.svg)](https://pypi.python.org/pypi/jupyterlab_nbconvert_nocode)
 
 ![](https://raw.githubusercontent.com/timkpaine/jupyterlab_nbconvert_nocode/main/docs/1.png)
-
-
```

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/README.md` & `jupyterlab_nbconvert_nocode-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/exporters.py` & `jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/exporters.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/PKG-INFO` & `jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: jupyterlab-nbconvert-nocode
-Version: 0.3.1
+Version: 0.4.0
 Summary: A simple helper library with 2 NBConvert exporters for PDF/HTML export with no code cells
 Home-page: https://github.com/timkpaine/jupyterlab_nbconvert_nocode
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: jupyter jupyterlab
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Jupyter
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: develop
 License-File: LICENSE
 
 # jupyterlab_nbconvert_nocode
 A simple helper library with 2 NBConvert exporters for PDF/HTML export with no code cells
 
 [![Build Status](https://github.com/timkpaine/jupyterlab_nbconvert_nocode/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/jupyterlab_nbconvert_nocode/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/timkpaine/jupyterlab_nbconvert_nocode/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/jupyterlab_nbconvert_nocode)
 [![GitHub issues](https://img.shields.io/github/issues/timkpaine/jupyterlab_nbconvert_nocode.svg)]()
 [![PyPI](https://img.shields.io/pypi/l/jupyterlab_nbconvert_nocode.svg)](https://pypi.python.org/pypi/jupyterlab_nbconvert_nocode)
 [![PyPI](https://img.shields.io/pypi/v/jupyterlab_nbconvert_nocode.svg)](https://pypi.python.org/pypi/jupyterlab_nbconvert_nocode)
 
 ![](https://raw.githubusercontent.com/timkpaine/jupyterlab_nbconvert_nocode/main/docs/1.png)
-
-
```

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/jupyterlab_nbconvert_nocode.egg-info/SOURCES.txt` & `jupyterlab_nbconvert_nocode-0.4.0/jupyterlab_nbconvert_nocode.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.bumpversion.cfg
+CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 setup.cfg
@@ -16,14 +16,15 @@
 jupyterlab_nbconvert_nocode.egg-info/not-zip-safe
 jupyterlab_nbconvert_nocode.egg-info/requires.txt
 jupyterlab_nbconvert_nocode.egg-info/top_level.txt
 jupyterlab_nbconvert_nocode/nbconvert_functions/__init__.py
 jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/__init__.py
 jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/exporters.py
 jupyterlab_nbconvert_nocode/nbconvert_functions/hideinput/utils.py
+jupyterlab_nbconvert_nocode/tests/Test.ipynb
 jupyterlab_nbconvert_nocode/tests/__init__.py
 jupyterlab_nbconvert_nocode/tests/test_all.py
 share/jupyter/nbconvert/templates/hide_code_cells_html/conf.json
 share/jupyter/nbconvert/templates/hide_code_cells_html/index.html.j2
 share/jupyter/nbconvert/templates/hide_code_cells_html_email/conf.json
 share/jupyter/nbconvert/templates/hide_code_cells_html_email/index.html.j2
 share/jupyter/nbconvert/templates/hide_code_cells_pdf/conf.json
```

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/setup.py` & `jupyterlab_nbconvert_nocode-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 from codecs import open
 from os import path
 
-from jupyter_packaging import get_data_files, get_version
+from jupyter_packaging import get_data_files
 from setuptools import find_packages, setup
 
 pjoin = path.join
 
 name = "jupyterlab_nbconvert_nocode"
 here = path.abspath(path.dirname(__file__))
-version = get_version(pjoin(here, name, "_version.py"))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 requires = [
-    "jupyterlab>=1.0.0",
+    "jupyterlab>=3.5",
     "nbconvert>=6.0.0",
 ]
 
 dev_requires = requires + [
-    "black>=20.",
+    "black>=23",
     "bump2version>=1.0.0",
+    "check-manifest",
     "flake8>=3.7.8",
     "flake8-black>=0.2.1",
     "jupyter_packaging",
     "mock",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "Sphinx>=1.8.4",
     "sphinx-markdown-builder>=0.5.2",
 ]
 
 setup(
     name=name,
-    version=version,
+    version="0.4.0",
     description="A simple helper library with 2 NBConvert exporters for PDF/HTML export with no code cells",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timkpaine/jupyterlab_nbconvert_nocode",
     author="Tim Paine",
     author_email="t.paine154@gmail.com",
     license="Apache 2.0",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Jupyter",
     ],
     keywords="jupyter jupyterlab",
     packages=find_packages(
         exclude=[
             "tests",
         ]
     ),
-    python_requries=">=3.6",
+    python_requries=">=3.8",
     include_package_data=True,
     data_files=get_data_files(
         [
-            ("share", str(pjoin(here, "share")), "**"),
+            ("share", "share", "**"),
         ]
     ),
     zip_safe=False,
     entry_points={
         "nbconvert.exporters": [
             "pdf_nocode = jupyterlab_nbconvert_nocode.nbconvert_functions.hideinput.exporters:PDFHideCodeExporter",
             "html_nocode = jupyterlab_nbconvert_nocode.nbconvert_functions.hideinput.exporters:HTMLHideCodeExporter",
         ],
     },
     extras_require={
         "dev": dev_requires,
+        "develop": dev_requires,
     },
 )
```

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_html_email/index.html.j2` & `jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_html_email/index.html.j2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbconvert_nocode-0.3.1/share/jupyter/nbconvert/templates/hide_code_cells_pdf/index.tex.j2` & `jupyterlab_nbconvert_nocode-0.4.0/share/jupyter/nbconvert/templates/hide_code_cells_pdf/index.tex.j2`

 * *Files identical despite different names*

