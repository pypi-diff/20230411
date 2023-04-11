# Comparing `tmp/perprof-py-1.1.3.tar.gz` & `tmp/perprof-py-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perprof-py-1.1.3.tar", last modified: Tue Mar 21 19:28:00 2023, max compression
+gzip compressed data, was "perprof-py-1.1.4.tar", last modified: Tue Apr 11 18:41:45 2023, max compression
```

## Comparing `perprof-py-1.1.3.tar` & `perprof-py-1.1.4.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.403554 perprof-py-1.1.3/
--rw-r--r--   0 abel      (1000) abel      (1000)      146 2023-03-21 19:25:49.000000 perprof-py-1.1.3/AUTHORS
--rw-r--r--   0 abel      (1000) abel      (1000)    32472 2023-03-21 19:25:49.000000 perprof-py-1.1.3/LICENSE
--rw-r--r--   0 abel      (1000) abel      (1000)    44661 2023-03-21 19:28:00.403554 perprof-py-1.1.3/PKG-INFO
--rw-r--r--   0 abel      (1000) abel      (1000)     6519 2023-03-21 19:25:49.000000 perprof-py-1.1.3/README.md
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.400221 perprof-py-1.1.3/perprof/
--rw-r--r--   0 abel      (1000) abel      (1000)      184 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/__init__.py
--rw-r--r--   0 abel      (1000) abel      (1000)     2535 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/bokeh.py
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.400221 perprof-py-1.1.3/perprof/examples/
--rw-r--r--   0 abel      (1000) abel      (1000)    67276 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/examples/alpha.table
--rw-r--r--   0 abel      (1000) abel      (1000)    66400 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/examples/beta.table
--rw-r--r--   0 abel      (1000) abel      (1000)    62057 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/examples/gamma.table
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.400221 perprof-py-1.1.3/perprof/locale/
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.400221 perprof-py-1.1.3/perprof/locale/en/
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.403554 perprof-py-1.1.3/perprof/locale/en/LC_MESSAGES/
--rw-r--r--   0 abel      (1000) abel      (1000)      386 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/locale/en/LC_MESSAGES/perprof.mo
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.400221 perprof-py-1.1.3/perprof/locale/pt/
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.403554 perprof-py-1.1.3/perprof/locale/pt/LC_MESSAGES/
--rw-r--r--   0 abel      (1000) abel      (1000)     8392 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/locale/pt/LC_MESSAGES/perprof.mo
--rw-r--r--   0 abel      (1000) abel      (1000)    13124 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/main.py
--rw-r--r--   0 abel      (1000) abel      (1000)     3733 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/matplotlib.py
--rw-r--r--   0 abel      (1000) abel      (1000)     8172 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/parse.py
--rw-r--r--   0 abel      (1000) abel      (1000)     7110 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/prof.py
--rw-r--r--   0 abel      (1000) abel      (1000)     7586 2023-03-21 19:25:49.000000 perprof-py-1.1.3/perprof/tikz.py
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.403554 perprof-py-1.1.3/perprof_py.egg-info/
--rw-r--r--   0 abel      (1000) abel      (1000)    44661 2023-03-21 19:28:00.000000 perprof-py-1.1.3/perprof_py.egg-info/PKG-INFO
--rw-r--r--   0 abel      (1000) abel      (1000)      565 2023-03-21 19:28:00.000000 perprof-py-1.1.3/perprof_py.egg-info/SOURCES.txt
--rw-r--r--   0 abel      (1000) abel      (1000)        1 2023-03-21 19:28:00.000000 perprof-py-1.1.3/perprof_py.egg-info/dependency_links.txt
--rw-r--r--   0 abel      (1000) abel      (1000)       46 2023-03-21 19:28:00.000000 perprof-py-1.1.3/perprof_py.egg-info/entry_points.txt
--rw-r--r--   0 abel      (1000) abel      (1000)      125 2023-03-21 19:28:00.000000 perprof-py-1.1.3/perprof_py.egg-info/requires.txt
--rw-r--r--   0 abel      (1000) abel      (1000)        8 2023-03-21 19:28:00.000000 perprof-py-1.1.3/perprof_py.egg-info/top_level.txt
--rw-r--r--   0 abel      (1000) abel      (1000)     1415 2023-03-21 19:25:49.000000 perprof-py-1.1.3/pyproject.toml
--rw-r--r--   0 abel      (1000) abel      (1000)       38 2023-03-21 19:28:00.403554 perprof-py-1.1.3/setup.cfg
--rw-r--r--   0 abel      (1000) abel      (1000)      296 2023-03-21 19:25:49.000000 perprof-py-1.1.3/setup.py
-drwxr-xr-x   0 abel      (1000) abel      (1000)        0 2023-03-21 19:28:00.403554 perprof-py-1.1.3/tests/
--rw-r--r--   0 abel      (1000) abel      (1000)     6009 2023-03-21 19:25:49.000000 perprof-py-1.1.3/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.701322 perprof-py-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-11 18:41:03.000000 perprof-py-1.1.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-04-11 18:41:03.000000 perprof-py-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-04-11 18:41:45.701322 perprof-py-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-11 18:41:03.000000 perprof-py-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.697322 perprof-py-1.1.4/perprof/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/bokeh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.697322 perprof-py-1.1.4/perprof/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    67276 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/examples/alpha.table
+-rw-r--r--   0 runner    (1001) docker     (123)    66400 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/examples/beta.table
+-rw-r--r--   0 runner    (1001) docker     (123)    62057 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/examples/gamma.table
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.693323 perprof-py-1.1.4/perprof/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.693323 perprof-py-1.1.4/perprof/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.697322 perprof-py-1.1.4/perprof/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/locale/en/LC_MESSAGES/perprof.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.693323 perprof-py-1.1.4/perprof/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.697322 perprof-py-1.1.4/perprof/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/locale/pt/LC_MESSAGES/perprof.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/prof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/profile_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/solver_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-04-11 18:41:03.000000 perprof-py-1.1.4/perprof/tikz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.701322 perprof-py-1.1.4/perprof_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-04-11 18:41:45.000000 perprof-py-1.1.4/perprof_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 18:41:45.000000 perprof-py-1.1.4/perprof_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:41:45.000000 perprof-py-1.1.4/perprof_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 18:41:45.000000 perprof-py-1.1.4/perprof_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-11 18:41:45.000000 perprof-py-1.1.4/perprof_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 18:41:45.000000 perprof-py-1.1.4/perprof_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-11 18:41:03.000000 perprof-py-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:41:45.701322 perprof-py-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-11 18:41:03.000000 perprof-py-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:41:45.701322 perprof-py-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-11 18:41:03.000000 perprof-py-1.1.4/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-11 18:41:03.000000 perprof-py-1.1.4/tests/test_profile_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-11 18:41:03.000000 perprof-py-1.1.4/tests/test_solver_data.py
```

### Comparing `perprof-py-1.1.3/LICENSE` & `perprof-py-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `perprof-py-1.1.3/PKG-INFO` & `perprof-py-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perprof-py
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python module for performance profiling (as described by Dolan and Moré)
 Author-email: Abel Soares Siqueira <abel.s.siqueira@gmail.com>, Raniere Gaia Costa da Silva <raniere@ime.unicamp.br>, Luiz Rafael dos Santos <l.r.santos@ufsc.br>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -629,20 +629,25 @@
 Project-URL: documentation, https://perprof-py.readthedocs.org/en/latest/
 Keywords: benchmark,comparison,performance profile
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: publishing
+Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS
 
 # perprof-py
 
-[![Build Status](https://travis-ci.org/abelsiqueira/perprof-py.svg?branch=master)](https://travis-ci.org/abelsiqueira/perprof-py)
+[![Tests](https://github.com/abelsiqueira/perprof-py/actions/workflows/tests.yml/badge.svg)](https://github.com/abelsiqueira/perprof-py/actions/workflows/tests.yml)
+[![Lint](https://github.com/abelsiqueira/perprof-py/actions/workflows/lint.yml/badge.svg)](https://github.com/abelsiqueira/perprof-py/actions/workflows/lint.yml)
+![PyPI](https://img.shields.io/pypi/v/perprof-py)
+[![](https://img.shields.io/badge/docs-latest-blue)](https://abelsiqueira.github.io/perprof-py/latest)
+[![](https://img.shields.io/badge/docs-dev-blue)](https://abelsiqueira.github.io/perprof-py/dev)
 
 A Python module for performance profiling (as described by [Dolan and
 Moré](http://arxiv.org/abs/cs/0102001)) with TikZ and matplotlib output.
 
 ## Reference
 
 When using this software for publications, please cite the paper below, which
@@ -651,134 +656,39 @@
 > Siqueira, A. S., Costa da Silva, R. G. and Santos, L.-R., (2016).
 Perprof-py: A Python Package for Performance Profile of Mathematical
 Optimization Software. Journal of Open Research Software. 4(1), p.e12.
 DOI: [http://doi.org/10.5334/jors.81](http://doi.org/10.5334/jors.81).
 
 ## License
 
-Copyright (C) 2013-2017 Abel Soares Siqueira, Raniere Gaia Costa da Silva, Luiz Rafael dos Santos.
+Copyright (C) 2013-2023 Abel Soares Siqueira, Raniere Gaia Costa da Silva, Luiz Rafael dos Santos.
 Licensed under the GNU GPL v3.
 
 This program is free software: you can redistribute it and/or modify it under
 the terms of the GNU General Public License as published by the Free Software
 Foundation, either version 3 of the License, or (at your option) any later
 version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the [GNU General Public License](LICENSE) for more
 details.
 
-## Documentation
+## Install
 
-Read the documentation on [Read the Docs](https://perprof-py.readthedocs.org/en/latest/).
-
-### Install
-
-See [all the instructions at documentation](https://perprof-py.readthedocs.org/en/latest/install.html).
-
-### How to use
-
-#### Input file format
+```bash
+python -m pip install perprof-py
+```
 
-See [all the instructions at documentation](https://perprof-py.readthedocs.org/en/latest/file-format.html).
+For more details, see the [documentation](https://abelsiqueira.github.io/perprof-py/latest).
 
-#### Command-line arguments
+## How to use
 
 ```bash
-$ perprof -h
-usage: perprof [-h] (--bokeh | --mp | --tikz | --raw | --table)
-               [--html | --eps | --pdf | --png | --ps | --svg | --tex]
-               [--standalone] [--pgfplotcompat PGFPLOTCOMPAT]
-               [--lang {en,pt_BR}] [--free-format] [--pdf-verbose]
-               [--black-and-white] [--background BACKGROUND]
-               [--page-background PAGE_BACKGROUND] [--semilog]
-               [--success SUCCESS] [--maxtime MAXTIME] [--mintime MINTIME]
-               [--compare {exitflag,optimalvalues}] [--unconstrained]
-               [--infeasibility-tolerance INFEASIBILITY_TOLERANCE]
-               [--title TITLE] [--no-title] [--xlabel XLABEL]
-               [--ylabel YLABEL] [-c] [-s SUBSET] [--tau TAU] [-f] [-o OUTPUT]
-               [--demo]
-               [file_name ...]
-
-A python module for performance profiling (as described by Dolan and Moré).
-
-positional arguments:
-  file_name             The name of the files to be used for the performance
-                        profiling (for demo use `--demo`)
-
-options:
-  -h, --help            show this help message and exit
-  --lang {en,pt_BR}, -l {en,pt_BR}
-                        Set language for plot
-  --free-format         When parsing file handle all non `c` character as `d`
-  --pdf-verbose         Print output of pdflatex
-  --black-and-white     Use only black color.
-  --background BACKGROUND
-                        RGB values separated by commas for the background
-                        color of the plot. (Values in the 0,255 range)
-  --page-background PAGE_BACKGROUND
-                        RGB values separated by commas for the background
-                        color of the page. (Values in the 0,255 range)
-  --semilog             Use logarithmic scale for the x axis of the plot
-  --success SUCCESS     Flags that are interpreted as success, separated by
-                        commas. Default: `c`
-  --maxtime MAXTIME     Sets a maximum time for a solved problem. Any problem
-                        with a time greater than this will be considered
-                        failed.
-  --mintime MINTIME     Sets a minimum time for a solved problem. Any problem
-                        with a time smaller than this will have the time set
-                        to this.
-  --compare {exitflag,optimalvalues}
-                        Choose the type of comparison to be made.
-  --unconstrained       Set the problems to unconstrained, which implies that
-                        there is no primal feasibility to check.
-  --infeasibility-tolerance INFEASIBILITY_TOLERANCE
-                        Tolerance for the primal and dual infeasibilities
-  --title TITLE         Set the title to be show on top of the performance
-                        profile
-  --no-title            Removes title
-  --xlabel XLABEL       Set the x label of the performance profile
-  --ylabel YLABEL       Set the y label of the performance profile
-  -c, --cache           Enable cache.
-  -s SUBSET, --subset SUBSET
-                        Name of a file with a subset of problems to compare
-  --tau TAU             Limit the x-axis based this value
-  -f, --force           Force overwrite the output file
-  -o OUTPUT, --output OUTPUT
-                        Name of the file to use as output (the correct
-                        extension will be add)
-  --demo                Use examples files as input
-
-Backend options:
-  --bokeh               Use bokeh as backend for the plot. Default output:
-                        HTML
-  --mp                  Use matplotlib as backend for the plot. Default
-                        output: PNG
-  --tikz                Use LaTex/TikZ/pgfplots as backend for the plot.
-                        Default output: PDF
-  --raw                 Print raw data. Default output: standard output
-  --table               Print table of robustness and efficiency
-
-Output formats:
-  --html                The output file will be a HTML file
-  --eps                 The output file will be a EPS file
-  --pdf                 The output file will be a PDF file
-  --png                 The output file will be a PNG file
-  --ps                  The output file will be a PS file
-  --svg                 The output file will be a SVG file
-  --tex                 The output file will be a (La)TeX file
-
-TikZ options:
-  --standalone          Create the header as a standalone to the tex file,
-                        enabling compilation of the result
-  --pgfplotcompat PGFPLOTCOMPAT
-                        Set pgfplots backwards compatibility mode to given
-                        version
+perprof-py FILES BACKEND
 ```
 
+For more details on the FILES format and the available backends, see the [documentation](https://abelsiqueira.github.io/perprof-py/latest).
+
 ## Getting Help
 
-If you didn't find something at the documentation,
-want to report a bug,
-or request a new feature,
-please open a [issue](https://github.com/abelsiqueira/perprof-py/issues).
+If you didn't find something at the documentation, want to report a bug, or request a new feature, please open an [issue](https://github.com/abelsiqueira/perprof-py/issues).
```

### Comparing `perprof-py-1.1.3/perprof/bokeh.py` & `perprof-py-1.1.4/perprof/bokeh.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 BOKEH_COLOR_LIST = ["blue", "green", "red", "cyan", "magenta", "yellow"]
 
 
 class Profiler(prof.Pdata):
     """The profiler using bokeh."""
 
     def __init__(self, parser_options, profiler_options):
-        """
-        :param dict parser_options: parser options.
+        """Initialize Profiler with Bokeh.
 
-        :param dict profiler_options: profiler options
+        Args:
+            parser_options (dict): parser options.
+            profiler_options (dict): profiler options
         """
         if profiler_options["output"] is None:
             self.output = f'performance-profile.{profiler_options["output_format"]}'
         else:
             self.output = (
                 f'{profiler_options["output"]}.{profiler_options["output_format"]}'
             )
```

### Comparing `perprof-py-1.1.3/perprof/examples/alpha.table` & `perprof-py-1.1.4/perprof/examples/alpha.table`

 * *Files identical despite different names*

### Comparing `perprof-py-1.1.3/perprof/examples/beta.table` & `perprof-py-1.1.4/perprof/examples/beta.table`

 * *Files identical despite different names*

### Comparing `perprof-py-1.1.3/perprof/examples/gamma.table` & `perprof-py-1.1.4/perprof/examples/gamma.table`

 * *Files identical despite different names*

### Comparing `perprof-py-1.1.3/perprof/locale/pt/LC_MESSAGES/perprof.mo` & `perprof-py-1.1.4/perprof/locale/pt/LC_MESSAGES/perprof.mo`

 * *Files identical despite different names*

### Comparing `perprof-py-1.1.3/perprof/main.py` & `perprof-py-1.1.4/perprof/main.py`

 * *Files identical despite different names*

### Comparing `perprof-py-1.1.3/perprof/matplotlib.py` & `perprof-py-1.1.4/perprof/matplotlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 _ = THIS_TRANSLATION.gettext
 
 
 class Profiler(prof.Pdata):
     """The profiler using matplotlib."""
 
     def __init__(self, parser_options, profiler_options):
-        """
-        :param dict parser_options: parser options.
+        """Intialize Profiler with Matplotlib.
 
-        :param dict profiler_options: profiler options
+        Args:
+            parser_options (dict): parser options.
+            profiler_options (dict): profiler options
         """
         if profiler_options["output"] is None:
             self.output = f'performance-profile.{profiler_options["output_format"]}'
         else:
             self.output = (
                 f'{profiler_options["output"]}.{profiler_options["output_format"]}'
             )
```

### Comparing `perprof-py-1.1.3/perprof/parse.py` & `perprof-py-1.1.4/perprof/parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,40 +23,46 @@
 _ = THIS_TRANSLATION.gettext
 
 
 def _error_message(filename, line_number, details):
     """
     Format the error message.
 
-    :param str filename: name of the file with the error
-    :param int line_number: number of the line with the error
-    :param str details: details about the error
-    :return str: the error message
+    Args:
+        filename (str): name of the file with the error
+        line_number (int): number of the line with the error
+        details (str): details about the error
+
+    Returns:
+        error (str): the error message
     """
     return _("ERROR when reading line #{} of {}:\n    {}").format(
         line_number, filename, details
     )
 
 
 def _str_sanitize(str2sanitize):
     """
     Sanitize the problem name for LaTeX.
 
-    :param str str2sanitize: string to be sanitize
-    :return: sanitized string
+    Args:
+        str2sanitize (str): string to be sanitize
+    Returns:
+        output (std): sanitized string
     """
     return str2sanitize.replace("_", "-")
 
 
 def _parse_yaml(options, yaml_header):
     """
     Parse the yaml header.
 
-    :param dict options: the local options for the parser
-    :param str yaml_header: The YAML header
+    Args:
+        options (dict): the local options for the parser
+        yaml_header (str): The YAML header
     """
     import yaml
 
     metadata = yaml.load(yaml_header, Loader=yaml.FullLoader)
     for opt in metadata:
         if opt not in options:
             raise ValueError("'" + opt + "'" + _(" is not a valid option for YAML."))
@@ -64,22 +70,28 @@
 
 
 # pylint: disable=too-many-branches,too-many-statements,too-many-locals
 def parse_file(filename, parser_options):
     """
     Parse one file.
 
-    :param str filename: name of the file to be parser
-    :param dict parser_options: dictionary with the options:
-        list subset: list with the name of the problems to use
-        list success: list with strings to mark sucess
-        int mintime: minimum time running the solver
-        int maxtime: maximum time running the solver
+    Args:
+        filename (str): name of the file to be parser
+        parser_options (dict):
+            dictionary with the following keys:
+
+            - subset (list): list with the name of the problems to use
+            - success (list): list with strings to mark sucess
+            - mintime (float): minimum time running the solver
+            - maxtime (float): maximum time running the solver
         bool free_format: if False request that fail be mark with ``d``
-    :return: performance profile data and name of the solver
+
+    Returns:
+        data (dict): performance profile data
+        algname (str): name of the solver
     """
     options = parser_options.copy()
     options["algname"] = _str_sanitize(filename)
     colopts = ["name", "exit", "time", "fval", "primal", "dual"]
     col = {}
     for colopt in colopts:
         # Columns starts at 1 but indexing at 0
```

### Comparing `perprof-py-1.1.3/perprof/prof.py` & `perprof-py-1.1.4/perprof/prof.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,33 @@
 _ = THIS_TRANSLATION.gettext
 
 
 def load_data(parser_options):
     """
     Load the data.
 
-    :param dict parser_options: the configuration dicionary
+    Args:
+        parser_options (dict): the configuration dicionary
     """
     data = {}
     for file_ in parser_options["files"]:
         data_tmp, solver_name = parse.parse_file(file_, parser_options)
         data[solver_name] = data_tmp
     return data
 
 
 class Pdata:
     """Store data for performance profile."""
 
     def __init__(self, parser_options, profiler_options):
-        """
-        :param dict parser_options: parser configuration.
+        """Initialize Pdata.
 
-        :param dict profiler_options: profiler configuration
+        Args:
+            parser_options (dict): parser configuration.
+            profiler_options (dict): profiler configuration
         """
         self.data = load_data(parser_options)
         self.cache = profiler_options["cache"]
         self.force = profiler_options["force"]
         self.semilog = profiler_options["semilog"]
         self.black_and_white = profiler_options["black_and_white"]
         self.background = profiler_options["background"]
@@ -73,23 +75,25 @@
 
         return str2output[:-2]
 
     def get_set_solvers(self):
         """
         Get the set of solvers to use.
 
-        :return: list of solvers
+        Returns:
+            solvers (list[dict]): list of solvers
         """
         return self.solvers
 
     def get_set_problems(self):
         """
         Get the set of problems to use.
 
-        :return: list of problems
+        Returns:
+            problems (list[str]): list of problems
         """
         return self.problems
 
     def scale(self):
         """Scale time."""
         times_set = set()
         for problem in self.problems:
```

### Comparing `perprof-py-1.1.3/perprof/tikz.py` & `perprof-py-1.1.4/perprof/tikz.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 _ = THIS_TRANSLATION.gettext
 
 
 class Profiler(prof.Pdata):
     """The profiler using TikZ."""
 
     def __init__(self, parser_options, profiler_options):
-        """
-        :param dict parser_options: parser options.
+        """Initialize Profiler with TikZ.
 
-        :param dict profiler_options: profiler options
+        Args:
+            parser_options (dict): parser options.
+            profiler_options (dict): profiler options
         """
         if profiler_options["output"] is None:
             self.output = sys.stdout
         else:
             self.output = f'{profiler_options["output"]}.tex'
             self.output = os.path.abspath(self.output)
         self.standalone = profiler_options["standalone"]
```

### Comparing `perprof-py-1.1.3/perprof_py.egg-info/PKG-INFO` & `perprof-py-1.1.4/perprof_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perprof-py
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python module for performance profiling (as described by Dolan and Moré)
 Author-email: Abel Soares Siqueira <abel.s.siqueira@gmail.com>, Raniere Gaia Costa da Silva <raniere@ime.unicamp.br>, Luiz Rafael dos Santos <l.r.santos@ufsc.br>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -629,20 +629,25 @@
 Project-URL: documentation, https://perprof-py.readthedocs.org/en/latest/
 Keywords: benchmark,comparison,performance profile
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: publishing
+Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS
 
 # perprof-py
 
-[![Build Status](https://travis-ci.org/abelsiqueira/perprof-py.svg?branch=master)](https://travis-ci.org/abelsiqueira/perprof-py)
+[![Tests](https://github.com/abelsiqueira/perprof-py/actions/workflows/tests.yml/badge.svg)](https://github.com/abelsiqueira/perprof-py/actions/workflows/tests.yml)
+[![Lint](https://github.com/abelsiqueira/perprof-py/actions/workflows/lint.yml/badge.svg)](https://github.com/abelsiqueira/perprof-py/actions/workflows/lint.yml)
+![PyPI](https://img.shields.io/pypi/v/perprof-py)
+[![](https://img.shields.io/badge/docs-latest-blue)](https://abelsiqueira.github.io/perprof-py/latest)
+[![](https://img.shields.io/badge/docs-dev-blue)](https://abelsiqueira.github.io/perprof-py/dev)
 
 A Python module for performance profiling (as described by [Dolan and
 Moré](http://arxiv.org/abs/cs/0102001)) with TikZ and matplotlib output.
 
 ## Reference
 
 When using this software for publications, please cite the paper below, which
@@ -651,134 +656,39 @@
 > Siqueira, A. S., Costa da Silva, R. G. and Santos, L.-R., (2016).
 Perprof-py: A Python Package for Performance Profile of Mathematical
 Optimization Software. Journal of Open Research Software. 4(1), p.e12.
 DOI: [http://doi.org/10.5334/jors.81](http://doi.org/10.5334/jors.81).
 
 ## License
 
-Copyright (C) 2013-2017 Abel Soares Siqueira, Raniere Gaia Costa da Silva, Luiz Rafael dos Santos.
+Copyright (C) 2013-2023 Abel Soares Siqueira, Raniere Gaia Costa da Silva, Luiz Rafael dos Santos.
 Licensed under the GNU GPL v3.
 
 This program is free software: you can redistribute it and/or modify it under
 the terms of the GNU General Public License as published by the Free Software
 Foundation, either version 3 of the License, or (at your option) any later
 version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the [GNU General Public License](LICENSE) for more
 details.
 
-## Documentation
+## Install
 
-Read the documentation on [Read the Docs](https://perprof-py.readthedocs.org/en/latest/).
-
-### Install
-
-See [all the instructions at documentation](https://perprof-py.readthedocs.org/en/latest/install.html).
-
-### How to use
-
-#### Input file format
+```bash
+python -m pip install perprof-py
+```
 
-See [all the instructions at documentation](https://perprof-py.readthedocs.org/en/latest/file-format.html).
+For more details, see the [documentation](https://abelsiqueira.github.io/perprof-py/latest).
 
-#### Command-line arguments
+## How to use
 
 ```bash
-$ perprof -h
-usage: perprof [-h] (--bokeh | --mp | --tikz | --raw | --table)
-               [--html | --eps | --pdf | --png | --ps | --svg | --tex]
-               [--standalone] [--pgfplotcompat PGFPLOTCOMPAT]
-               [--lang {en,pt_BR}] [--free-format] [--pdf-verbose]
-               [--black-and-white] [--background BACKGROUND]
-               [--page-background PAGE_BACKGROUND] [--semilog]
-               [--success SUCCESS] [--maxtime MAXTIME] [--mintime MINTIME]
-               [--compare {exitflag,optimalvalues}] [--unconstrained]
-               [--infeasibility-tolerance INFEASIBILITY_TOLERANCE]
-               [--title TITLE] [--no-title] [--xlabel XLABEL]
-               [--ylabel YLABEL] [-c] [-s SUBSET] [--tau TAU] [-f] [-o OUTPUT]
-               [--demo]
-               [file_name ...]
-
-A python module for performance profiling (as described by Dolan and Moré).
-
-positional arguments:
-  file_name             The name of the files to be used for the performance
-                        profiling (for demo use `--demo`)
-
-options:
-  -h, --help            show this help message and exit
-  --lang {en,pt_BR}, -l {en,pt_BR}
-                        Set language for plot
-  --free-format         When parsing file handle all non `c` character as `d`
-  --pdf-verbose         Print output of pdflatex
-  --black-and-white     Use only black color.
-  --background BACKGROUND
-                        RGB values separated by commas for the background
-                        color of the plot. (Values in the 0,255 range)
-  --page-background PAGE_BACKGROUND
-                        RGB values separated by commas for the background
-                        color of the page. (Values in the 0,255 range)
-  --semilog             Use logarithmic scale for the x axis of the plot
-  --success SUCCESS     Flags that are interpreted as success, separated by
-                        commas. Default: `c`
-  --maxtime MAXTIME     Sets a maximum time for a solved problem. Any problem
-                        with a time greater than this will be considered
-                        failed.
-  --mintime MINTIME     Sets a minimum time for a solved problem. Any problem
-                        with a time smaller than this will have the time set
-                        to this.
-  --compare {exitflag,optimalvalues}
-                        Choose the type of comparison to be made.
-  --unconstrained       Set the problems to unconstrained, which implies that
-                        there is no primal feasibility to check.
-  --infeasibility-tolerance INFEASIBILITY_TOLERANCE
-                        Tolerance for the primal and dual infeasibilities
-  --title TITLE         Set the title to be show on top of the performance
-                        profile
-  --no-title            Removes title
-  --xlabel XLABEL       Set the x label of the performance profile
-  --ylabel YLABEL       Set the y label of the performance profile
-  -c, --cache           Enable cache.
-  -s SUBSET, --subset SUBSET
-                        Name of a file with a subset of problems to compare
-  --tau TAU             Limit the x-axis based this value
-  -f, --force           Force overwrite the output file
-  -o OUTPUT, --output OUTPUT
-                        Name of the file to use as output (the correct
-                        extension will be add)
-  --demo                Use examples files as input
-
-Backend options:
-  --bokeh               Use bokeh as backend for the plot. Default output:
-                        HTML
-  --mp                  Use matplotlib as backend for the plot. Default
-                        output: PNG
-  --tikz                Use LaTex/TikZ/pgfplots as backend for the plot.
-                        Default output: PDF
-  --raw                 Print raw data. Default output: standard output
-  --table               Print table of robustness and efficiency
-
-Output formats:
-  --html                The output file will be a HTML file
-  --eps                 The output file will be a EPS file
-  --pdf                 The output file will be a PDF file
-  --png                 The output file will be a PNG file
-  --ps                  The output file will be a PS file
-  --svg                 The output file will be a SVG file
-  --tex                 The output file will be a (La)TeX file
-
-TikZ options:
-  --standalone          Create the header as a standalone to the tex file,
-                        enabling compilation of the result
-  --pgfplotcompat PGFPLOTCOMPAT
-                        Set pgfplots backwards compatibility mode to given
-                        version
+perprof-py FILES BACKEND
 ```
 
+For more details on the FILES format and the available backends, see the [documentation](https://abelsiqueira.github.io/perprof-py/latest).
+
 ## Getting Help
 
-If you didn't find something at the documentation,
-want to report a bug,
-or request a new feature,
-please open a [issue](https://github.com/abelsiqueira/perprof-py/issues).
+If you didn't find something at the documentation, want to report a bug, or request a new feature, please open an [issue](https://github.com/abelsiqueira/perprof-py/issues).
```

### Comparing `perprof-py-1.1.3/perprof_py.egg-info/SOURCES.txt` & `perprof-py-1.1.4/perprof_py.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 setup.py
 perprof/__init__.py
 perprof/bokeh.py
 perprof/main.py
 perprof/matplotlib.py
 perprof/parse.py
 perprof/prof.py
+perprof/profile_data.py
+perprof/solver_data.py
 perprof/tikz.py
 perprof/examples/alpha.table
 perprof/examples/beta.table
 perprof/examples/gamma.table
 perprof/locale/en/LC_MESSAGES/perprof.mo
 perprof/locale/pt/LC_MESSAGES/perprof.mo
 perprof_py.egg-info/PKG-INFO
 perprof_py.egg-info/SOURCES.txt
 perprof_py.egg-info/dependency_links.txt
 perprof_py.egg-info/entry_points.txt
 perprof_py.egg-info/requires.txt
 perprof_py.egg-info/top_level.txt
-tests/test_all.py
+tests/test_all.py
+tests/test_profile_data.py
+tests/test_solver_data.py
```

### Comparing `perprof-py-1.1.3/pyproject.toml` & `perprof-py-1.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -14,31 +14,39 @@
 requires-python = ">=3.7"
 keywords = ["benchmark", "comparison", "performance profile"]
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python"
 ]
 dependencies = [
-  "pyyaml<6",
-  "matplotlib>=3",
-  "bokeh>=2",
+  "pyyaml>=5,<7",
+  "matplotlib>=3,<4",
+  "bokeh>=2,<3",
+  "pandas>=1,<2",
 ]
-version = "1.1.3"
+version = "1.1.4"
 
 [project.optional-dependencies]
 dev = [
   "black",
   "pre-commit",
   "prospector[with_pyroma]",
   "pylint",
   "pytest",
   "pytest-cov",
 ]
 publishing = [
-  "twine"
+  "build",
+  "twine",
+]
+docs = [
+  "mkdocs",
+  "mkdocstrings[python]",
+  "mkdocs-material",
+  "mike",
 ]
 
 [project.scripts]
 perprof = "perprof.main:main"
 
 [project.urls]
 repository = "https://github.com/abelsiqueira/perprof-py"
```

### Comparing `perprof-py-1.1.3/tests/test_all.py` & `perprof-py-1.1.4/tests/test_all.py`

 * *Files identical despite different names*

