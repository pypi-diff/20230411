# Comparing `tmp/Clean Business Chart-0.1.1.tar.gz` & `tmp/Clean Business Chart-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Clean Business Chart-0.1.1.tar", last modified: Wed Mar 29 18:56:47 2023, max compression
+gzip compressed data, was "Clean Business Chart-0.1.2.tar", last modified: Tue Apr 11 21:01:34 2023, max compression
```

## Comparing `Clean Business Chart-0.1.1.tar` & `Clean Business Chart-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 18:56:47.637812 Clean Business Chart-0.1.1/
--rw-rw-rw-   0        0        0      178 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3801 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.1/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 18:56:47.582085 Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/
--rw-rw-rw-   0        0        0     2609 2023-03-29 18:56:46.000000 Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2023-03-29 18:56:47.000000 Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 18:56:46.000000 Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-26 19:27:13.000000 Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2023-03-29 18:56:46.000000 Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-29 18:56:46.000000 Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      272 2023-03-29 18:53:24.000000 Clean Business Chart-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1099 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2609 2023-03-29 18:56:47.637812 Clean Business Chart-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1188 2023-03-29 18:55:44.000000 Clean Business Chart-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 18:56:47.597938 Clean Business Chart-0.1.1/clean_business_chart/
--rw-rw-rw-   0        0        0      664 2023-03-29 18:36:58.000000 Clean Business Chart-0.1.1/clean_business_chart/__init__.py
--rw-rw-rw-   0        0        0    26196 2023-03-28 19:36:41.000000 Clean Business Chart-0.1.1/clean_business_chart/clean_business_chart.py
--rw-rw-rw-   0        0        0    70941 2023-03-29 18:33:15.000000 Clean Business Chart-0.1.1/clean_business_chart/columnchartwithwaterfall.py
--rw-rw-rw-   0        0        0     8548 2023-03-13 17:56:42.000000 Clean Business Chart-0.1.1/clean_business_chart/deltachart.py
--rw-rw-rw-   0        0        0    18511 2023-03-27 19:05:56.000000 Clean Business Chart-0.1.1/clean_business_chart/general_functions.py
--rw-rw-rw-   0        0        0    11072 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/clean_business_chart/multiplier.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:56:47.613584 Clean Business Chart-0.1.1/docs/
--rw-rw-rw-   0        0        0      641 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/authors.rst
--rw-rw-rw-   0        0        0     5127 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/history.rst
--rw-rw-rw-   0        0        0      337 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     1281 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/installation.rst
--rwxrwxrwx   0        0        0      818 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/readme.rst
--rw-rw-rw-   0        0        0      150 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/docs/usage.rst
--rw-rw-rw-   0        0        0      463 2023-03-29 18:56:47.640983 Clean Business Chart-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1817 2023-03-28 19:59:09.000000 Clean Business Chart-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:56:47.613584 Clean Business Chart-0.1.1/tests/
--rw-rw-rw-   0        0        0       51 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:56:47.635693 Clean Business Chart-0.1.1/tests/clean_business_chart/
--rw-rw-rw-   0        0        0    10634 2023-03-24 20:49:07.000000 Clean Business Chart-0.1.1/tests/clean_business_chart/test_columnchartwithwaterfall.py
--rw-rw-rw-   0        0        0     1692 2023-03-13 18:07:00.000000 Clean Business Chart-0.1.1/tests/clean_business_chart/test_deltachart.py
--rw-rw-rw-   0        0        0     5988 2023-03-27 18:50:18.000000 Clean Business Chart-0.1.1/tests/clean_business_chart/test_general_functions.py
--rw-rw-rw-   0        0        0     7490 2023-03-06 20:13:44.000000 Clean Business Chart-0.1.1/tests/clean_business_chart/test_multiplier.py
--rw-rw-rw-   0        0        0      624 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.1/tests/test_clean_business_chart.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:01:34.890656 Clean Business Chart-0.1.2/
+-rw-rw-rw-   0        0        0      178 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3801 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.2/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 21:01:34.729853 Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/
+-rw-rw-rw-   0        0        0     3218 2023-04-11 21:01:33.000000 Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2023-04-11 21:01:34.000000 Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:01:33.000000 Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-26 19:27:13.000000 Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2023-04-11 21:01:33.000000 Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-11 21:01:33.000000 Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      514 2023-04-11 20:41:13.000000 Clean Business Chart-0.1.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-02-26 18:49:53.000000 Clean Business Chart-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3218 2023-04-11 21:01:34.890656 Clean Business Chart-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1473 2023-04-11 20:48:20.000000 Clean Business Chart-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 21:01:34.750669 Clean Business Chart-0.1.2/clean_business_chart/
+-rw-rw-rw-   0        0        0      652 2023-04-11 20:56:40.000000 Clean Business Chart-0.1.2/clean_business_chart/__init__.py
+-rw-rw-rw-   0        0        0    63552 2023-03-24 20:12:08.000000 Clean Business Chart-0.1.2/clean_business_chart/barchartwithwaterfall.py
+-rw-rw-rw-   0        0        0    26196 2023-03-28 19:36:41.000000 Clean Business Chart-0.1.2/clean_business_chart/clean_business_chart.py
+-rw-rw-rw-   0        0        0    70078 2023-04-11 19:44:43.000000 Clean Business Chart-0.1.2/clean_business_chart/columnchartwithwaterfall.py
+-rw-rw-rw-   0        0        0     8397 2023-04-02 20:40:31.000000 Clean Business Chart-0.1.2/clean_business_chart/deltachart.py
+-rw-rw-rw-   0        0        0    18511 2023-03-27 19:05:56.000000 Clean Business Chart-0.1.2/clean_business_chart/general_functions.py
+-rw-rw-rw-   0        0        0    11072 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/clean_business_chart/multiplier.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:01:34.852185 Clean Business Chart-0.1.2/docs/
+-rw-rw-rw-   0        0        0      641 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     5127 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/history.rst
+-rw-rw-rw-   0        0        0      337 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1281 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      818 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/readme.rst
+-rw-rw-rw-   0        0        0      150 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/docs/usage.rst
+-rw-rw-rw-   0        0        0      463 2023-04-11 21:01:34.895553 Clean Business Chart-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2023-04-11 20:37:09.000000 Clean Business Chart-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:01:34.871951 Clean Business Chart-0.1.2/tests/
+-rw-rw-rw-   0        0        0       51 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:01:34.888590 Clean Business Chart-0.1.2/tests/clean_business_chart/
+-rw-rw-rw-   0        0        0    30441 2023-04-11 20:20:20.000000 Clean Business Chart-0.1.2/tests/clean_business_chart/test_columnchartwithwaterfall.py
+-rw-rw-rw-   0        0        0     1662 2023-04-02 20:44:53.000000 Clean Business Chart-0.1.2/tests/clean_business_chart/test_deltachart.py
+-rw-rw-rw-   0        0        0     5988 2023-03-27 18:50:18.000000 Clean Business Chart-0.1.2/tests/clean_business_chart/test_general_functions.py
+-rw-rw-rw-   0        0        0     7490 2023-03-06 20:13:44.000000 Clean Business Chart-0.1.2/tests/clean_business_chart/test_multiplier.py
+-rw-rw-rw-   0        0        0      624 2023-02-26 18:49:54.000000 Clean Business Chart-0.1.2/tests/test_clean_business_chart.py
```

### Comparing `Clean Business Chart-0.1.1/CONTRIBUTING.rst` & `Clean Business Chart-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/PKG-INFO` & `Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Clean-Business-Chart
-Version: 0.1.1
+Version: 0.1.2
 Summary: Clean Business Chart is a Python package for IBCS-like charts based on matplotlib.
 Home-page: https://github.com/marcelw1323/clean_business_chart
 Author: Marcel Wuijtenburg
 Author-email: marcelw1323@gmail.com
 License: MIT license
-Keywords: clean business chart,IBCS,business chart,clean business charts,business charts
+Keywords: clean business chart,IBCS,business chart,clean business charts,business charts,chart,charts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -50,14 +50,22 @@
 
 
 Features
 --------
 
 * ColumnWithWaterfall, the first chart released with clean-business-chart!
 * added support for pandas in version 0.1.1
+* added date column support for pandas DataFrame and added translation of column headers inside the call in version 0.1.2
+
+
+Read more
+---------
+
+* README.MD on github: https://github.com/MarcelW1323/clean_business_chart/blob/main/README.md
+* LinkedIn Group on Clean Business Chart: https://www.linkedin.com/groups/12783685/
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
@@ -65,14 +73,21 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.1.2 (2023-04-11)
+------------------
+
+* Added date column in pandas DataFrame support in parameter data when calling the column chart with waterfall.
+* Also added translate_headers as a parameter in dictionary-form to rename the columns within the call.
+
+
 0.1.1 (2023-03-29)
 ------------------
 
 * Added pandas DataFrame support in parameter data when calling the column chart with waterfall.
 
 
 0.1.0 (2023-02-21)
```

### Comparing `Clean Business Chart-0.1.1/Clean_Business_Chart.egg-info/SOURCES.txt` & `Clean Business Chart-0.1.2/Clean_Business_Chart.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Clean_Business_Chart.egg-info/PKG-INFO
 Clean_Business_Chart.egg-info/SOURCES.txt
 Clean_Business_Chart.egg-info/dependency_links.txt
 Clean_Business_Chart.egg-info/not-zip-safe
 Clean_Business_Chart.egg-info/requires.txt
 Clean_Business_Chart.egg-info/top_level.txt
 clean_business_chart/__init__.py
+clean_business_chart/barchartwithwaterfall.py
 clean_business_chart/clean_business_chart.py
 clean_business_chart/columnchartwithwaterfall.py
 clean_business_chart/deltachart.py
 clean_business_chart/general_functions.py
 clean_business_chart/multiplier.py
 docs/Makefile
 docs/authors.rst
```

### Comparing `Clean Business Chart-0.1.1/LICENSE` & `Clean Business Chart-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/PKG-INFO` & `Clean Business Chart-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Clean Business Chart
-Version: 0.1.1
+Version: 0.1.2
 Summary: Clean Business Chart is a Python package for IBCS-like charts based on matplotlib.
 Home-page: https://github.com/marcelw1323/clean_business_chart
 Author: Marcel Wuijtenburg
 Author-email: marcelw1323@gmail.com
 License: MIT license
-Keywords: clean business chart,IBCS,business chart,clean business charts,business charts
+Keywords: clean business chart,IBCS,business chart,clean business charts,business charts,chart,charts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -50,14 +50,22 @@
 
 
 Features
 --------
 
 * ColumnWithWaterfall, the first chart released with clean-business-chart!
 * added support for pandas in version 0.1.1
+* added date column support for pandas DataFrame and added translation of column headers inside the call in version 0.1.2
+
+
+Read more
+---------
+
+* README.MD on github: https://github.com/MarcelW1323/clean_business_chart/blob/main/README.md
+* LinkedIn Group on Clean Business Chart: https://www.linkedin.com/groups/12783685/
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
@@ -65,14 +73,21 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.1.2 (2023-04-11)
+------------------
+
+* Added date column in pandas DataFrame support in parameter data when calling the column chart with waterfall.
+* Also added translate_headers as a parameter in dictionary-form to rename the columns within the call.
+
+
 0.1.1 (2023-03-29)
 ------------------
 
 * Added pandas DataFrame support in parameter data when calling the column chart with waterfall.
 
 
 0.1.0 (2023-02-21)
```

### Comparing `Clean Business Chart-0.1.1/README.rst` & `Clean Business Chart-0.1.2/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-====================
-Clean Business Chart
-====================
-
-
-.. image:: https://img.shields.io/pypi/v/clean_business_chart.svg
-        :target: https://pypi.python.org/pypi/clean_business_chart
-
-.. image:: https://img.shields.io/travis/marcelw1323/clean_business_chart.svg
-        :target: https://travis-ci.com/marcelw1323/clean_business_chart
-
-.. image:: https://readthedocs.org/projects/clean-business-chart/badge/?version=latest
-        :target: https://clean-business-chart.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-
-
-Clean Business Chart is a Python package for IBCS-like charts based on matplotlib.
-
-
-* Free software: MIT license
-* Documentation: https://clean-business-chart.readthedocs.io.
-
-
-Features
---------
-
-* ColumnWithWaterfall, the first chart released with clean-business-chart!
-* added support for pandas in version 0.1.1
-
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+====================
+Clean Business Chart
+====================
+
+
+.. image:: https://img.shields.io/pypi/v/clean_business_chart.svg
+        :target: https://pypi.python.org/pypi/clean_business_chart
+
+.. image:: https://img.shields.io/travis/marcelw1323/clean_business_chart.svg
+        :target: https://travis-ci.com/marcelw1323/clean_business_chart
+
+.. image:: https://readthedocs.org/projects/clean-business-chart/badge/?version=latest
+        :target: https://clean-business-chart.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+
+
+Clean Business Chart is a Python package for IBCS-like charts based on matplotlib.
+
+
+* Free software: MIT license
+* Documentation: https://clean-business-chart.readthedocs.io.
+
+
+Features
+--------
+
+* ColumnWithWaterfall, the first chart released with clean-business-chart!
+* added support for pandas in version 0.1.1
+* added date column support for pandas DataFrame and added translation of column headers inside the call in version 0.1.2
+
+
+Read more
+---------
+
+* README.MD on github: https://github.com/MarcelW1323/clean_business_chart/blob/main/README.md
+* LinkedIn Group on Clean Business Chart: https://www.linkedin.com/groups/12783685/
+
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `Clean Business Chart-0.1.1/clean_business_chart/__init__.py` & `Clean Business Chart-0.1.2/clean_business_chart/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""Top-level package for Clean Business Chart."""
-
-__author__ = """Marcel Wuijtenburg"""
-__email__ = 'marcelw1323@gmail.com'
-__version__ = '0.1.1'
-
-from .clean_business_chart import *              # Class GeneralChart with general variables for unity
-from .general_functions import *                 # Diverse set of functions to be used with all kind of charts
-from .multiplier import *                        # Class Multiplier
-from .deltachart import *                        # Class DeltaChart
-from .columnchartwithwaterfall import *          # Class ColumnWithWaterfall
-#from .barchartwithwaterfall import *             # Class BarWithWaterfall
-
+"""Top-level package for Clean Business Chart."""
+
+__author__ = """Marcel Wuijtenburg"""
+__email__ = 'marcelw1323@gmail.com'
+__version__ = '0.1.2'
+
+from .clean_business_chart import *              # Class GeneralChart with general variables for unity
+from .general_functions import *                 # Diverse set of functions to be used with all kind of charts
+from .multiplier import *                        # Class Multiplier
+from .deltachart import *                        # Class DeltaChart
+from .columnchartwithwaterfall import *          # Class ColumnWithWaterfall
+#from .barchartwithwaterfall import *             # Class BarWithWaterfall
+
+
```

### Comparing `Clean Business Chart-0.1.1/clean_business_chart/clean_business_chart.py` & `Clean Business Chart-0.1.2/clean_business_chart/clean_business_chart.py`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/clean_business_chart/columnchartwithwaterfall.py` & `Clean Business Chart-0.1.2/clean_business_chart/barchartwithwaterfall.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-"""ColumnWithWaterfall-module"""
+"""BarWithWaterfall-module"""
 
 import matplotlib.pyplot as plt                   # for most graphics
 from matplotlib import rcParams as mpl_rcp        # for font in _title
-#from matplotlib import __version__ as mpl_version
-import pandas as pd                               # for easy pandas support
 
 from clean_business_chart.clean_business_chart import GeneralChart 
 from clean_business_chart.general_functions    import plot_line_accross_axes, plot_line_within_ax, prepare_title, formatstring, optimize_data, \
-                                                      islist, isdictionary, isinteger, isstring, isfloat, isboolean, isdataframe, string_to_value
+                                                      islist, isdictionary, isinteger, isstring, isfloat, isboolean
 from clean_business_chart.multiplier           import Multiplier
 
 
-class ColumnWithWaterfall(GeneralChart):
+class BarWithWaterfall(GeneralChart):
     """
-    Produces a column chart with a waterfall delta chart based on data of one year divided in 12 months
+    Produces a bar chart with a waterfall delta chart based on data of one category
     
     Minimal requirements to make the chart
     --------------------------------------
     import clean_business_chart as cbc
-    dataset = {'PY': [14, 16, 14, 17, 19, 17, 19, 22, 16, 17, 16, 22],      # 12 months of Previous Year data (optional)
-               'PL': [11, 10, 10, 10, 10, 10, 15, 14, 15, 15, 15, 19],      # 12 months of PLan data
-               'AC': [15, 13, 16, 7, 5, 6, 17, 11],                         # up to 12 months of ACtual data
-               'FC': [0, 0, 0, 0, 0, 0, 0, 0, 26, 22, 13, 29],              # up to 12 months of ForeCast data
-               'Year': 2022}                                                # the year to be mentioned in the chart
-    cbc.ColumnWithWaterfall(data=dataset)
+    #                               PY, PL, AC, FC
+    dataset =  { 'Spain'        : [ 30, 33, 53, 0 ],
+                 'Greece'       : [ 38, 33, 39, 0 ],
+                 'Sweden'       : [ 38, 35, 40, 0 ],
+                 'Germany'      : [ 90, 89, 93, 0 ],
+                 'Russia'       : [ 60, 56, 60, 0 ],
+                 'Italy'        : [ 15, 12, 14, 0 ],
+                 'Great Britain': [ 15, 13, 15, 0 ],
+                 'Slovenia'     : [  4,  5,  4, 0 ],
+                 'Denmark'      : [ 29, 35, 33, 0 ],
+                 'Netherlands'  : [ 39, 42, 38, 0 ],
+                 'France'       : [ 60, 77, 63, 0 ],
+                 'OTHER'        : [ 40, 37, 44, 0 ]}
+    cbc.BarWithWaterfall(data=dataset)
     
     Parameters
     ----------
-    data                    : A dictionary with minimal PL and AC or PY and AC detailinformation, a string with CSV-values or a list of lists is also supported. Read the documentation.
+    data                    : 
     positive_is_good        : On a variance chart it decides whether a positive number makes a good color (True) or a bad number (False).
                               Default: True (good color)
     preferred_base_scenario : PL, use PLaninfo as the base scenario in the main chart. PY uses Previous Year als the base scenario in the main chart
     title                   : A dictionary with optional values to make a title inspired by IBCS
                               Default: None (no title)
     measure                 : True -> measure, False -> ratio
                               Default: True (measure)
@@ -41,83 +47,166 @@
                               Default: None (no export of the chart to a file)
     force_pl_is_zero        : If PL are all zeros, can PL be ignored (False) or force that PL can be zero (True)
                               Default: False (PL can be ignored when all zeros)
     force_zero_decimals     : If True, we use integers for output. This gives a more clean chart, but can lack some detail in some cases
                               Default: False (don't force zero decimals)
     force_max_one_decimals  : If True, the maximum of decimals used is one. Know that force_zero_decimals has a higher priority than force_max_one_decimals.
                               Default: False (don't force max one decimals)
-    test                    : If True, only variables from the parent class are defined, together with other self-variables.
-                              This makes this module testable in an automatic way
-                              Default: False (this call it is not an automatic test)
     """
 
     def __init__(self, data=None, positive_is_good=True, preferred_base_scenario='PL', title=None, measure=True, multiplier='1', filename=None, 
-                 force_pl_is_zero=False, force_zero_decimals=False, force_max_one_decimals=False, test=False):
+                 force_pl_is_zero=False, force_zero_decimals=False, force_max_one_decimals=False):
         """
         This is the first function that will be called automatically. Here you'll find all the possible parameters to customize your experience.
         """
         super().__init__()                            # Get the variables from the parent class
-        self._other_columnwithwaterfall_variables()   # Get additional variables for this class
-        
-        # for use to test automatically
-        if test: return None
+        self._other_barwithwaterfall_variables()   # Get additional variables for this class
         
         # Store variables
         self.original_data          = data
         self.original_multiplier    = Multiplier(multiplier)
-        self.year                   = None
         self.positive_is_good       = positive_is_good
         self.base_scenario          = preferred_base_scenario
         self.hatch                  = self.hatch_pattern
         self.filename               = filename
         self.force_pl_is_zero       = force_pl_is_zero
         self.force_zero_decimals    = force_zero_decimals
         self.force_max_one_decimals = force_max_one_decimals
         
         # Make chart
         self.get_barwidth(measure)
-        self._check_data(data)
-        if self.year is None: raise ValueError("No 'Year' supplied in data.")
+        #self._check_data(data)
+        self.data = data   # Needs to be implemented in "check_data"
         self._make_subplots()
-        self.calculate_delta(base_scenario=self.base_scenario, compare_scenario_list=['AC', 'FC'], delta_name='main')
-        self._fill_leftside_ax()
-        self._fill_side_axsum()
-        self._fill_axcomments()
-        self._fill_main_ax()
-        self._show_delta()
-        self._fill_delta_ax_text()
+        #self.calculate_delta(base_scenario=self.base_scenario, compare_scenario_list=['AC', 'FC'], delta_name='main')
+        self.linewidth_bar = 1 # linewidth=1 is smaller than the columnchart  ## TECNICAL DEBT
+        self._fill_chart()
+        #self._fill_leftside_ax()
+        #self._fill_side_axsum()
+        #self._fill_axcomments()
+        #self._fill_main_ax()
+        #self._show_delta()
+        #self._fill_delta_ax_text()
 
-        # Add the title as the last element        
+        # Add the title as the last element 
+        self.multiplier = self.original_multiplier     ## TECHNICAL DEBT      
         self._title(title)
         
         # We are exporting the chart if the filename has a value
         if self.filename is not None:
             plt.savefig(self.filename, bbox_inches='tight', dpi=150)
         
         plt.show()
         
+    def _fill_chart(self):
+        ax = self.ax["main"]
+        data = self.data
+        base_scenario = self.base_scenario
+        scenariolist = ['PY', 'PL', 'AC', 'FC']
+        p  = scenariolist.index(base_scenario)
+        ac = scenariolist.index('AC')
+        fc = scenariolist.index('FC')
+        yvalue_p = list()
+        data_p   = list()
+        yvalue_c = list()
+        data_ac  = list()
+        data_fc  = list()
+        lasty = None
+        extray = 0.5
+        lenlist = len(list(data.keys())) - 1
+        lenlist2 = len(data.keys()) - 1
+        print("lenlist",lenlist,lenlist2)
+        
+        for y, category in enumerate(data.keys()):
+            y_used = y
+            if y == lenlist:
+                y_used+=extray
+            lasty = y_used
+            category_data = self.data[category]
+            #scenario_data = self.data[scenario]
+            self.get_barwidth(measure=True)
+            self.barshift             = self.barshift_value 
+            yvalue_p.append(0 - y_used + self.barshift * self.barwidth)
+            yvalue_c.append(0 - y_used - self.barshift * self.barwidth)
+            data_p.append(category_data[p])
+            data_ac.append(category_data[ac])
+            data_fc.append(category_data[fc])
+        
+        # PY of PL        
+        self._plot_barh(y=yvalue_p, width=data_p, scenario=base_scenario, height=self.barwidth, left=0)
+        #ax.barh(y=yvalue_p, width=data_p, color=self.colors[base_scenario][0], height=self.barwidth, linewidth=self.linewidth_bar, 
+        #        edgecolor=self.colors[base_scenario][1], label=base_scenario)
+        
+        # AC
+        self._plot_barh(y=yvalue_c, width=data_ac, scenario='AC', height=self.barwidth, left=0)
+        #ax.barh(y=yvalue_c, width=data_ac, color=self.colors['AC'][0], height=self.barwidth, linewidth=self.linewidth_bar, 
+        #        edgecolor=self.colors['AC'][1], label='AC')
+        
+        # FC
+        if data_fc != [0]*len(data_fc):
+            self._plot_barh(y=yvalue_c, width=data_fc, scenario='FC', height=self.barwidth, left=data_ac)
+            #ax.barh(y=yvalue_c, width=data_fc, color=self.colors['FC'][0], height=self.barwidth, left=data_ac, linewidth=self.linewidth_bar, 
+            #        edgecolor=self.colors['FC'][1], label='FC', hatch=self.hatch)
+        
+        totp = sum(data_p)
+        self._plot_barh(y=+1.5, width=totp, scenario=base_scenario, height=self.barwidth*1.2, left=0)
+        
+        tota = sum(data_ac)
+        self._plot_barh(y=-1*lasty-1.5, width=tota, scenario='AC', height=self.barwidth*1.2, left=0)
+        
+        totf = sum(data_fc)
+        if totf != 0:
+            self._plot_barh(y=-1*lasty-1.5, width=totf, scenario='FC', height=self.barwidth*1.2, left=tota)
+            
+
+    def _plot_barh(self, y, width, scenario, height, left=0):
+        ax = self.ax["main"]
+        # PY of PL
+        if scenario[0] == 'P':
+             ax.barh(y=y, width=width, color=self.colors[scenario][0], height=height, linewidth=self.linewidth_bar, 
+                edgecolor=self.colors[scenario][1], label=scenario)
+        
+        # AC
+        if scenario == 'AC':
+            ax.barh(y=y, width=width, color=self.colors['AC'][0], height=height, linewidth=self.linewidth_bar, 
+                edgecolor=self.colors['AC'][1], label='AC')
+        
+        # FC
+        if scenario == 'FC': ## and width != [0]*len(width):
+            if islist(y):
+                y2 = [i for j,i in enumerate(y) if width[j] != 0]
+                width2 = [i for i in width if i !=0]
+                left2 = [i for j,i in enumerate(left) if width[j] != 0]
+                print("y2", y2)
+                print("w2", width2)
+                ax.barh(y=y2, width=width2, color=self.colors['FC'][0], height=height, left=left2, linewidth=self.linewidth_bar, 
+                        edgecolor=self.colors['FC'][1], label='FC', hatch=self.hatch)
+    
+            else:
+                ax.barh(y=y, width=width, color=self.colors['FC'][0], height=height, left=left, linewidth=self.linewidth_bar, 
+                        edgecolor=self.colors['FC'][1], label='FC', hatch=self.hatch)
+    
+    
 
-    def _other_columnwithwaterfall_variables(self):
+    def _other_barwithwaterfall_variables(self):
         """
-        A collection of variables for columnchartwithwaterfall
+        A collection of variables for barchartwithwaterfall
         """
         # Supported scenario's
         self.p_scenarios       = ['PY', 'PL']              # Previous Year, PLan
         self.p_scenarios_prio  = ['PL', 'PY']              # Priority for the p-scenarios: First PLan, then Previous Year
         self.c_scenarios       = ['AC', 'FC']              # ACtual, ForeCast
         self.c_scenarios_prio  = ['AC', 'FC']              # Priority for the c-scenarios: First AC, then FC
         self.all_scenarios     = ['PY', 'PL', 'AC', 'FC']  # Previous Year, PLan, ACtual, ForeCast (in order of time)
         
         # Decimals
         self.decimals_details  = 0
         self.decimals_totals   = 0
         
-        # # Multipliers
-        # self.multipliers            = ('1', 'k', 'm', 'b')            # Multiplier 1 (one, 10^0), k (kilo, 10^3), m (million, 10^6), b (billion, 10^9)
-        # self.multipliers_value      = (1, 1000, 1000000, 1000000000)  # Values of the multipliers
+        # Multipliers
         self.multiplier             = None                            # Initial value
         self.multiplier_denominator = 1                               # Denominator is the diviser
         
         # Other
         self.filename          = None       # When filename is None, no export
         
 
@@ -248,25 +337,17 @@
         
         self.data               : Detail values for each scenario. Scenario is the key for the list of detail values
         
         self.data_total         : Total values for each scenario. Scenario is the key for the total value
         
         self.year               : Year of the data
         """
-        # Do we need to convert the data to a dictionary? We support string and list.
-        if isstring(data):
-            # data is in the form of a string. We need to convert it to a list of lists (easier step) to prepare the conversion to a dictionary
-            data = self._convert_data_string_to_list_of_lists(data)
-            # data is now in the form of a list of lists
-        if isdataframe(data):
-            # data is in the form of a pandas DataFrame
-            data = self._prepare_data_frame(data)
-            # data is now in the form of a dictionary
-        if islist(data):
-            # Data is in the form of a list (of lists). We need to convert it to a dictionary
+        if type(data) == type(""):
+            data = self._convert_data_string_to_dict(data)
+        elif type(data) == type(list()):
             data = self._convert_data_list_of_lists_to_dict(data)
         
         # Check for existence of data
         if data is None:
             raise ValueError("No data available. Dictionary expected {'PY': [12x#], 'PL': [12x#], 'AC': [up to 12x#], 'FC': [up to 12x] }")
         
         # Check for the existence of the base_scenario
@@ -358,263 +439,46 @@
                 self.base_scenario = temp_list[0]
         
         
         # Optimize multiplier and data        
         self._optimize_multiplier()
 
 
-    def _convert_data_string_to_list_of_lists(self, data_string):
+    def _convert_data_string_to_dict(self, data_string):
         """
-        If the data is like a string, this function sees it as a CSV-file pasted in a string and will make it first to a list of lists.
+        If the data is like a string, this function sees it as a CSV-file pasted in a string and will make it first to a list of lists and then calls an other function to make it a dictionary.
 
         Parameters
         ----------
         data_string : data_string contains a string-like CSV-file.
         
         Returns
         -------
-        data_list   : data_list contains a list of lists
-        """
-        # Check if the data_string is not a string
-        if not isstring(data_string):
+        data_dict   : data_dict contains a dictionary with the scenario's as a key and the detail values as a list
+       """
+        # Check if the data is a string
+        if type(data_string) != type(''):
             raise ValueError(str(data_string)+" is not a string")
         
         # Split the string into lines, based on the 'new line'-character
         lines = data_string.splitlines()
         
         # Create an empty list to receive each line (as a list). So we end with the variable data_list as a list of lists.
         data_list = list()
         for line in lines:
             if len(line.strip()) == 0:
                 # skip the empty line
                 continue
-            splitted_line = line.strip().split(',')
+            splitted_line = line.split(',')
             data_list.append(splitted_line)
         
-        return data_list
-
-    def _convert_dataframe_to_list_of_lists_old_(self, dataframe):
-        """
-        If the data is a pandas DataFrame, this function will make it to a list of lists.
-
-        Parameters
-        ----------
-        dataframe : pandas DataFrame containing the columns Year and Month mandatory and the columns PY, PL, AC and/or FC.
-        
-        Returns
-        -------
-        data_list   : data_list contains a list of lists
-        """
-        # Check if the dataframe is not a pandas DataFrame
-        if not isdataframe(dataframe):
-            raise ValueError(str(dataframe)+" is not a pandas DataFrame")
-
-        dataframe = self._data_frame_keep_only_relevant_columns(dataframe)
-        dataframe = self._data_frame_aggregate(dataframe)
-
-        data_list = [dataframe.columns.tolist()] + dataframe.values.tolist()
-
-        return data_list
-
-    def _data_frame_keep_only_relevant_columns(self, dataframe):
-        """
-        If the data is a pandas DataFrame, this function will narrow this DataFrame down to the needed columns.
-
-        Parameters
-        ----------
-        dataframe        : pandas DataFrame with a lot of columns.
-        
-        Returns
-        -------
-        export_dataframe : pandas DataFrame with at most the columns 'Year', 'Month', 'PY', 'PL', 'AC' and 'FC'
-        """
-        # Check if the dataframe is not a pandas DataFrame
-        if not isdataframe(dataframe):
-            raise ValueError(str(dataframe)+" is not a pandas DataFrame")
-
-        wanted_headers = ['Year', 'Month', 'PY', 'PL', 'AC', 'FC']
-
-        # Determine which wanted headers are available in the dataframe
-        available_headers = [x for x in wanted_headers if x in dataframe.columns]
-
-        # We only need the data from the columns for the purpose of this chart
-        export_dataframe = dataframe[available_headers].copy()
-        
-        return export_dataframe
-
-    def _data_frame_aggregate(self, dataframe):
-        """
-        If the data is a pandas DataFrame, this function will aggregate this DataFrame by 'Year' and 'Month'.
-        
-        Precondition: The dataframe should only have te needed columns.
-
-        Parameters
-        ----------
-        dataframe        : pandas DataFrame with hopefully a 'Year' and 'Month' column.
-        
-        Returns
-        -------
-        export_dataframe : aggregated pandas DataFrame, aggregated by 'Year' and 'Month'
-        """
-        # Check if the dataframe is not a pandas DataFrame
-        if not isdataframe(dataframe):
-            raise ValueError(str(dataframe)+" is not a pandas DataFrame")
-
-        # We need the Year and Month columns
-        needed_headers = ['Year', 'Month']
-
-        # Determine which needed headers are available in the dataframe
-        available_headers = [x for x in needed_headers if x in dataframe.columns]
-
-        if available_headers != needed_headers:
-            raise ValueError("Expected columns in the DataFrame: "+str(needed_headers)+". But found only these columns: "+str(available_headers))
-
-        # Aggregate data
-        export_dataframe = dataframe.groupby(available_headers).sum().reset_index()
-        
-        return export_dataframe
-
-    def _data_frame_full_year(self, dataframe):
-        """
-        If the data is a pandas DataFrame, this function will make incomplete years complete by adding missing months.
-        
-        Precondition: The dataframe dataframe needs to be aggregated by Year and Month and only contains the data from one year.
-
-        Parameters
-        ----------
-        dataframe        : pandas DataFrame with data from one year.
-        
-        Returns
-        -------
-        export_dataframe : pandas DataFrame with 12 rows, one for each month
-        """
-        # Check if the dataframe is not a pandas DataFrame
-        if not isdataframe(dataframe):
-            raise ValueError(str(dataframe)+" is not a pandas DataFrame")
-
-        # We need the Year and Month columns
-        needed_headers = ['Year', 'Month']
-
-        # Determine which needed headers are available in the dataframe
-        available_headers = [x for x in needed_headers if x in dataframe.columns]
-        
-        if available_headers != needed_headers:
-            raise ValueError("Expected columns in the DataFrame: "+str(needed_headers)+". But found only these columns: "+str(available_headers))
-
-        min_year = dataframe['Year'].min()
-        max_year = dataframe['Year'].max()
-        if min_year != max_year:
-            raise ValueError("More than one year in DataFrame. Min year:"+str(min_year)+". Max year:"+str(max_year))
-        
-        year = [str(min_year)] * 12
-        month = [ ('00'+str(x))[-2:] for x in range(1,13)]  # Gives the numbers 1 to 12, both inclusive
-        df = pd.DataFrame({'Year':year, 'Month':month})
-
-        # Fill full year
-        export_dataframe = pd.merge(df, dataframe, how='left' ,on=['Year', 'Month'])
-        export_dataframe = export_dataframe.fillna(0)
-        
-        return export_dataframe
-    
-    def _convert_year_month_to_string_dataframe(self, dataframe):
-        """
-        If the data is a pandas DataFrame, this function will convert the year and month to string values (containing numbers) for convenient sorting.
-        
-        Precondition: The dataframe dataframe needs to be aggregated by Year and Month.
-
-        Parameters
-        ----------
-        dataframe        : pandas DataFrame, aggregated by Year and Month.
-        
-        Returns
-        -------
-        export_dataframe : pandas DataFrame sorted by Year and Month
-        """
-        # Check if the dataframe is not a pandas DataFrame
-        if not isdataframe(dataframe):
-            raise ValueError(str(dataframe)+" is not a pandas DataFrame")
-
-        # We need the Year and Month columns
-        needed_headers = ['Year', 'Month']
-
-        # Determine which needed headers are available in the dataframe
-        available_headers = [x for x in needed_headers if x in dataframe.columns]
-
-        if available_headers != needed_headers:
-            raise ValueError("Expected columns in the DataFrame: "+str(needed_headers)+". But found only these columns: "+str(available_headers))
-
-        # Convert year to string. Convert month to string with length=2, filled with leading zeros if value < 10
-        dataframe['Year'] = dataframe['Year'].apply(int).apply(str)
-        dataframe['Month'] = dataframe['Month'].apply(int).apply(str).str.zfill(2)
-        
-        # Sort dataframe by Year and Month
-        export_dataframe = dataframe.sort_values(['Year', 'Month'], ascending = [True, True]).copy()
-        
-        return export_dataframe
-
-    def _prepare_data_frame(self, dataframe):
-        """
-        This function orchestrates other functions to transform a pandas DataFrame into a dictionary of scenarios.
-
-        Parameters
-        ----------
-        dataframe         : pandas DataFrame
-        
-        Returns
-        -------
-        export_dictionary : dictionary with for each available scenario a list of 12 values and one value for the Year
-        """
-        # If the dataframe has more columns than relevant, only keep the relevant columns
-        dataframe = self._data_frame_keep_only_relevant_columns(dataframe)
-        
-        # It is possible that the dataframe has more detailed lines (especially when removing non-relevant columns). Aggregate them on Year/Month-level
-        dataframe = self._data_frame_aggregate(dataframe)
-        
-        # Convert year and month to strings and sort the dataframe on year and month
-        dataframe = self._convert_year_month_to_string_dataframe(dataframe)
-        
-        # Determine the max-year and the year before the max-year. These will be the actual (AC) and previous year (PY)
-        max_year        = dataframe['Year'].max()
-        before_max_year = str(int(max_year)-1)
-
-        # Split the dataframes in the actual and previous year
-        df_ac = dataframe[dataframe['Year'] == max_year].copy()
-        df_py = dataframe[dataframe['Year'] == before_max_year].copy()
-        
-        # Complete dataframe for missing month-values. Nothing worse than incomplete time-axis
-        df_ac = self._data_frame_full_year(df_ac)
-        df_py = self._data_frame_full_year(df_py)
-        
-        if 'PY' in df_ac.columns:
-            if 'AC' in df_py.columns:
-                if not (df_ac['PY'] == df_py['AC']).all():
-                    raise ValueError(str(max_year)+"-DataFrame previous year does not match "+str(before_max_year)+ "-Dataframe", df_ac, df_py)
-                # else:
-                #    Everything is fine, go further
-            # else:
-            #    No actual values in previous year dataframe
-        else:
-            # No previous year values in actual dataframe
-            if 'AC' in df_py.columns:
-                # We can use the actual values in te previous year dataframe as previous year values in the actual dataframe
-                df_ac['PY'] = df_py['AC'].copy()
-        
-        # Transform the DataFrame into a dictionary
-        export_dictionary = df_ac.to_dict(orient='list')
-        export_dictionary['Year'] = max_year
-        if 'Month' in export_dictionary:
-            del export_dictionary['Month']
-        # Convert the values (that can be of type string) from the scenarios in integer or float values
-        for scenario in ['PY', 'PL', 'AC', 'FC']:
-            if scenario in export_dictionary.keys():
-                valuelist = export_dictionary[scenario]
-                export_dictionary[scenario] = string_to_value(valuelist)
+        # Convert the list of lists to a dictionary
+        data_dict = self._convert_data_list_of_lists_to_dict(data_list)
 
-        return export_dictionary
-        
+        return data_dict
 
     def _convert_data_list_of_lists_to_dict(self, data_list):
         """
         Makes a dictionary out of a list of lists.
  
         Parameters
         ----------
@@ -624,38 +488,36 @@
         --------------
         self.all_scenarios : all possible supported scenario's
         
         Returns
         -------
         checked_data_dict  : checked_data_dict contains a dictionary with the scenario's as a key and the detail values as a list
        """
-        # Check if the data is not a list (ValueError), because we need a list (containing more lists)
-        if not islist(data_list):
+        # Check if the data is a list
+        if type(data_list) != type(list()):
             raise ValueError(str(data_list)+" is not a list")
         
         # Headers will ultimately contain the needed headers of the 'CSV'-list-structure
         headers = None
         headerlength = 0
         
         # Data_dict will contain the dictionary of lists to return from this function
         data_dict  = dict()
-        
-        # We keep track of the year_month-combinations for completeness (all 12 month from a year) and for uniqueness (each combination occurs one times)
         year_month = list()
         
         # Process each element of the list (which should be a list by themself)
         for element_list in data_list:
             # Is the element_list containing data?
             if len(element_list) == 0:
                 # skip the empty line
                 continue
             
-            # Check again if the element_list is not a list (ValueError), because we need a list at this level
-            if not islist(element_list):
-                raise ValueError("The element "+str(element_list)+" is not a list")
+            # Check again if the element_list is a list
+            if type(element_list) != type(list()):
+                raise ValueError(str(element_list)+" is not a list")
         
             if headers is None:
                 # Headers has no headervalues right now, use this first line as headers
                 # The element_list usable as header must contain Year and Month information or else we can not prepare the data for the charts later
                 if "Year" not in element_list or "Month" not in element_list:
                     raise ValueError("Year and Month needs to be in the first line of the dataset"+str(element_list))
                 headerline = [i for i in ["Year", "Month"]+self.all_scenarios if i in element_list]
@@ -799,27 +661,22 @@
         self.fig      : Figure-object for the generated plot and subplots
 
         self.ax       : Dictionary of axesobjects for the generated subplots
 
         """
         self.ax = dict()
         
-        scenarios = self.filter_scenarios(scenario_list=['PY', 'PL'])
-        if len(scenarios) == 2:
-            left_width = 1.8
-        else:
-            left_width = 1.4
-        
-        self.fig, (self.ax["left"], self.ax["main"], self.ax["sum"], self.ax["comment"]) = \
-                   plt.subplots(nrows=1, ncols=4, sharey='row', figsize=(15,6),
-                                gridspec_kw={'width_ratios': [left_width, 15, 1.4, 1.2]})
+        self.fig, self.ax["main"] = \
+                   plt.subplots(nrows=1, ncols=1, #sharey='row', 
+                                figsize=(6,6))#,
+                                #gridspec_kw={'width_ratios': [left_width, 15, 1.4, 1.2]})
                                 #width_ratios=[left_width, 15, 1.2, 1.2]) # From matplotlib-version 3.6.0 and above
 
-        #plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=0.15, hspace=None)   # wspace is for the space between the subplots
-        self.fig.set_facecolor('white')   # Make a white background so the export to a file will have a white background
+        ##plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=0.15, hspace=None)   # wspace is for the space between the subplots
+        #self.fig.set_facecolor('white')   # Make a white background so the export to a file will have a white background
 
     
     def _fill_main_ax(self):
         """
         Fill all the components of the main ax:
            plot bars for the comparison scenario, AC and/or FC
            put text on the bars
@@ -1281,26 +1138,20 @@
         
         title_text = prepare_title(title, multiplier=self.multiplier.get_multiplier_string())
         # Check if there is a title prepared
         if title_text == None:
             # No title
             return
         
-        # Determine in which ax the title needs to start
-        scenario = self.filter_scenarios(scenario_list=['PY', 'PL'])
-        if len(scenario) == 0:
-           # No Previous Year or Plan
-           ax = self.ax["main"]
-        else:
-           # The left ax
-           ax = self.ax["left"]
+        ax = self.ax["main"]
            
         #from matplotlib import rcParams as mpl_rcp  # This line is on top of this module, but only needed for this below.
         mpl_rcp['mathtext.rm'] = self.font           # import matplotlib as mpl : mpl.rcParams['mathtext.rm'] = self.font   ## This should do the same, but imports a whole matplotlib
         
         
         # Get the current limits of the axis
         limits = ax.axis()  # 4th value. Also possible with ax.get_ylim(), but then 2nd value
+        print(limits)
         
         # Plot the title
         #### Need to think of a good strategy to fit the title at best!
-        ax.text(0 - self.barwidth*1.2, limits[3]*1.1, title_text, horizontalalignment='left', font=self.font, fontsize=self.fontsize, color=self.colors['text'], verticalalignment='bottom')
+        ax.text(0 - self.barwidth*1.2, limits[3]*1.5, title_text, horizontalalignment='left', font=self.font, fontsize=self.fontsize, color=self.colors['text'], verticalalignment='bottom')
```

### Comparing `Clean Business Chart-0.1.1/clean_business_chart/deltachart.py` & `Clean Business Chart-0.1.2/clean_business_chart/deltachart.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-"""DeltaChart-module"""
-
-from clean_business_chart.clean_business_chart import GeneralChart 
-
-class DeltaChart(GeneralChart):
-    """
-    The class DeltaChart helps you calculate a delta chart and prepare the visualisation of a delta chart.
-    
-    Capability:
-    Calculate
-    Prepare
-    Visualize
-
-    Examples:
-    ---------
-    ... to be documented ...
-    """
-    def __init__(self):
-        
-        print("DeltaChart-init")
-        
-        # Class variables
-        self.delta_value_list    = list()
-        self.delta_percent_list  = list()
-        self.delta_scenario_list = list()
-        self.delta_base_scenario = None
-        self.use_max_length      = None
-        
-        dataset = {'PY': [14, 16, 14, 17, 19, 17, 19, 22, 16, 17, 16, 22], 
-                   'PL': [11, 10, 10, 10, 10, 10, 15, 14, 15, 15, 15, 19],
-                   'AC': [15, 13, 16,  7,  5,  6, 17, 11],
-                   'FC': [ 0,  0,  0,  0,  0,  0,  0,  0, 26, 22, 13, 29]}
-                   
-        # TECHNICAL DEBT: Needed for the self.filter_scenarios
-        self.data_total = dataset
-                   
-        testvar = self.calculate_h(data=dataset, base_scenario='PL', compare_scenario_list=['AC', 'FC'])
-        print("Testvar\n",testvar)
-              
-
-    def calculate_h(self, data, base_scenario, compare_scenario_list, max_length=None, round_decimals_percentages=1):
-        """
-        Calculate the delta values for a horizontal delta chart
-        """
-        print("Calculate\ndata:", data, "\nbase_scenario:", base_scenario, "\ncompare_scenario_list:", compare_scenario_list)
-        self.delta_base_scenario = base_scenario                       # Get the value of the base scenario and put it in a class variable
-        self.use_max_length      = self._calculate_max_length(data=data, base_scenario=base_scenario, compare_scenario_list=compare_scenario_list, max_length=max_length)
-        print("self.use_max_length", self.use_max_length)
-        
-        # Initialize work variables
-        self.delta_value_list    = [0]  * self.use_max_length     # Make a list with only zeros to record the delta values
-        self.delta_percent_list  = [0]  * self.use_max_length     # Make a list with only zeros to record the delta percentages
-        self.delta_scenario_list = [''] * self.use_max_length     # Make a list with only empty scenarios to record the comparable scenario responsible for the delta 
-        
-        if base_scenario in data.keys():
-            work_base_list = list(data[base_scenario])            # Make a copy of the data-list for the base scenario because the work_base_list will be modified
-        else:
-            raise ValueError("Base_scenario", base_scenario, "not in the keys of de dictionary of the data.")
-
-        # A delta is the difference of the compare_scenario value and the base_scenario value. We need to record this difference and the scenario this difference belongs to.
-        # If the scenario alters, we add this information to the month-name if the related parameter add_scenario_to_month is True
-        # IBCS advices to display 'n.a.' (not available) if the relative variance can not be interpreted. This is often the case when you compare a positive value to a negative reference value (in the denominator)        
-        for new_scenario in self.filter_scenarios(scenario_list=compare_scenario_list):
-            for number, compare_element in enumerate(data[new_scenario]):
-                print("PRE Number:",number, "Scenario:", new_scenario, "Compare_element:", compare_element, "work_base_list[number]:", work_base_list[number])
-                work_base_list[number], self.delta_scenario_list[number], self.delta_value_list[number] = \
-                    self._calculate_element(old_scenario            = self.delta_scenario_list[number],
-                                            old_delta_value_element = self.delta_value_list[number],
-                                            base_element            = work_base_list[number], 
-                                            new_scenario            = new_scenario, 
-                                            compare_element         = compare_element)
-                print("POST Number:",number, "Scenario_list:", self.delta_scenario_list[number], "Value_list:", self.delta_value_list[number], "work_base_list[number]:", work_base_list[number])
-            print("Mid\n",self.delta_scenario_list,"\n",self.delta_value_list)
-        print("END\n",self.delta_scenario_list,"\n",self.delta_value_list)
-        print("TODO: calculate relative values")
-
-    def _calculate_element(self, old_scenario, old_delta_value_element, base_element, new_scenario, compare_element):
-        
-        
-        if compare_element is not None and compare_element != 0:
-            if len(old_scenario) != 0:
-                raise ValueError("New scenario "+str(new_scenario)+" on top of old scenario "+old_scenario+" not supported yet.")
-            else:
-                delta_scenario_element = new_scenario
-                delta_value_element    = old_delta_value_element + compare_element - base_element
-                return_base_element    = 0
-        else:
-            delta_scenario_element = old_scenario
-            delta_value_element    = old_delta_value_element
-            return_base_element    = base_element
-
-        return return_base_element, delta_scenario_element, delta_value_element
- 
-        
-    def _calculate_max_length(self, data, base_scenario, compare_scenario_list, max_length=None):
-        """
-        Calculate the max length of the lists, unless when max_length is already provided then use that provided max_length
-        """
-        print("\n_Calculate_max_length\ndata:", data, "\nbase_scenario:", base_scenario, "\ncompare_scenario_list:", compare_scenario_list)
-        if max_length is not None:
-            # Max_length is of an other type than None
-            if isinstance(max_length, int):
-                # Max_length is of type integer
-                if max_length > 0:
-                    # Max_length has a value greater than zero
-                    return max_length
-                else:
-                    # Max_length has a value of 0 or less
-                    raise ValueError("Variable max_length has a value of 0 or lower:"+str(max_length))
-            else:
-                # Max_length is not of type integer
-                raise TypeError("Variable max_length is not of type int, but has this value:"+str(max_length))
-        else:
-            # Max_length is of type None. We must calculate the max_length out of the data
-            scenarios  = self._calculate_concat_scenario(base_scenario=base_scenario, compare_scenario_list=compare_scenario_list)
-            print("Scenarios:", scenarios)
-            max_length = self._calculate_max_length_dataset(data=data, scenarios=scenarios)
-            print("max_length:", max_length)
-            return max_length
-
-
-    def _calculate_concat_scenario(self, base_scenario, compare_scenario_list):
-        """
-        Make a list of all scenario's of the parameters
-        """
-        scenarios = list()
-        scenarios.append(base_scenario)           # Add one string value to the list
-        scenarios.extend(compare_scenario_list)   # Add elements from a list to the list (and not add a list as one element to the list)
-        return scenarios
-
-    def _calculate_max_length_dataset(self, data, scenarios):
-        """
-        Determine the max length of the list of the scenarios
-        """
-        # Check type of parameters
-        if not isinstance(data, dict):
-            raise TypeError("Variable data is not of type dictionary, but of type:"+str(data))
-        if not isinstance(scenarios, list):
-            raise TypeError("Variable scenarios is not of type list, but of type:"+str(scenarios))
-        
-        max_length = None
-        for scenario in scenarios:
-            if scenario not in data.keys():
-                raise ValueError("Scenario "+str(scenario)+" not in the keys of dictionary data:"+str(data.keys()))
-            if max_length is None:
-                max_length = len(data[scenario])
-            else:
-                max_length = max(max_length, len(data[scenario]))
-        if max_length is None:
-            raise ValueError("Could not find data to determine max_length:"+str(max_length))
-        return max_length
+"""DeltaChart-module"""
+
+from clean_business_chart.clean_business_chart import GeneralChart 
+
+class DeltaChart(GeneralChart):
+    """
+    The class DeltaChart helps you calculate a delta chart and prepare the visualisation of a delta chart.
+    
+    Capability:
+    Calculate
+    Prepare
+    Visualize
+
+    Examples:
+    ---------
+    ... to be documented ...
+    """
+    def __init__(self):
+        
+        print("DeltaChart-init")
+        
+        # Class variables
+        self.delta_value_list    = list()
+        self.delta_percent_list  = list()
+        self.delta_scenario_list = list()
+        self.delta_base_scenario = None
+        self.use_max_length      = None
+        
+        dataset = {'PY': [14, 16, 14, 17, 19, 17, 19, 22, 16, 17, 16, 22], 
+                   'PL': [11, 10, 10, 10, 10, 10, 15, 14, 15, 15, 15, 19],
+                   'AC': [15, 13, 16,  7,  5,  6, 17, 11],
+                   'FC': [ 0,  0,  0,  0,  0,  0,  0,  0, 26, 22, 13, 29]}
+                   
+        # TECHNICAL DEBT: Needed for the self.filter_scenarios
+        self.data_total = dataset
+                   
+        testvar = self.calculate_h(data=dataset, base_scenario='PL', compare_scenario_list=['AC', 'FC'])
+        print("Testvar\n",testvar)
+              
+
+    def calculate_h(self, data, base_scenario, compare_scenario_list, max_length=None, round_decimals_percentages=1):
+        """
+        Calculate the delta values for a horizontal delta chart
+        """
+        print("Calculate\ndata:", data, "\nbase_scenario:", base_scenario, "\ncompare_scenario_list:", compare_scenario_list)
+        self.delta_base_scenario = base_scenario                       # Get the value of the base scenario and put it in a class variable
+        self.use_max_length      = self._calculate_max_length(data=data, base_scenario=base_scenario, compare_scenario_list=compare_scenario_list, max_length=max_length)
+        print("self.use_max_length", self.use_max_length)
+        
+        # Initialize work variables
+        self.delta_value_list    = [0]  * self.use_max_length     # Make a list with only zeros to record the delta values
+        self.delta_percent_list  = [0]  * self.use_max_length     # Make a list with only zeros to record the delta percentages
+        self.delta_scenario_list = [''] * self.use_max_length     # Make a list with only empty scenarios to record the comparable scenario responsible for the delta 
+        
+        if base_scenario in data.keys():
+            work_base_list = list(data[base_scenario])            # Make a copy of the data-list for the base scenario because the work_base_list will be modified
+        else:
+            raise ValueError("Base_scenario", base_scenario, "not in the keys of de dictionary of the data.")
+
+        # A delta is the difference of the compare_scenario value and the base_scenario value. We need to record this difference and the scenario this difference belongs to.
+        # If the scenario alters, we add this information to the month-name if the related parameter add_scenario_to_month is True
+        # IBCS advices to display 'n.a.' (not available) if the relative variance can not be interpreted. This is often the case when you compare a positive value to a negative reference value (in the denominator)        
+        for new_scenario in self.filter_scenarios(scenario_list=compare_scenario_list):
+            for number, compare_element in enumerate(data[new_scenario]):
+                print("PRE Number:",number, "Scenario:", new_scenario, "Compare_element:", compare_element, "work_base_list[number]:", work_base_list[number])
+                work_base_list[number], self.delta_scenario_list[number], self.delta_value_list[number] = \
+                    self._calculate_element(old_scenario            = self.delta_scenario_list[number],
+                                            old_delta_value_element = self.delta_value_list[number],
+                                            base_element            = work_base_list[number], 
+                                            new_scenario            = new_scenario, 
+                                            compare_element         = compare_element)
+                print("POST Number:",number, "Scenario_list:", self.delta_scenario_list[number], "Value_list:", self.delta_value_list[number], "work_base_list[number]:", work_base_list[number])
+            print("Mid\n",self.delta_scenario_list,"\n",self.delta_value_list)
+        print("END\n",self.delta_scenario_list,"\n",self.delta_value_list)
+        print("TODO: calculate relative values")
+
+    def _calculate_element(self, old_scenario, old_delta_value_element, base_element, new_scenario, compare_element):
+        
+        
+        if compare_element is not None and compare_element != 0:
+            if len(old_scenario) != 0:
+                raise ValueError("New scenario "+str(new_scenario)+" on top of old scenario "+old_scenario+" not supported yet.")
+            else:
+                delta_scenario_element = new_scenario
+                delta_value_element    = old_delta_value_element + compare_element - base_element
+                return_base_element    = 0
+        else:
+            delta_scenario_element = old_scenario
+            delta_value_element    = old_delta_value_element
+            return_base_element    = base_element
+
+        return return_base_element, delta_scenario_element, delta_value_element
+ 
+        
+    def _calculate_max_length(self, data, base_scenario, compare_scenario_list, max_length=None):
+        """
+        Calculate the max length of the lists, unless when max_length is already provided then use that provided max_length
+        """
+        print("\n_Calculate_max_length\ndata:", data, "\nbase_scenario:", base_scenario, "\ncompare_scenario_list:", compare_scenario_list)
+        if max_length is not None:
+            # Max_length is of an other type than None
+            if isinstance(max_length, int):
+                # Max_length is of type integer
+                if max_length > 0:
+                    # Max_length has a value greater than zero
+                    return max_length
+                else:
+                    # Max_length has a value of 0 or less
+                    raise ValueError("Variable max_length has a value of 0 or lower:"+str(max_length))
+            else:
+                # Max_length is not of type integer
+                raise TypeError("Variable max_length is not of type int, but has this value:"+str(max_length))
+        else:
+            # Max_length is of type None. We must calculate the max_length out of the data
+            scenarios  = self._calculate_concat_scenario(base_scenario=base_scenario, compare_scenario_list=compare_scenario_list)
+            print("Scenarios:", scenarios)
+            max_length = self._calculate_max_length_dataset(data=data, scenarios=scenarios)
+            print("max_length:", max_length)
+            return max_length
+
+
+    def _calculate_concat_scenario(self, base_scenario, compare_scenario_list):
+        """
+        Make a list of all scenario's of the parameters
+        """
+        scenarios = list()
+        scenarios.append(base_scenario)           # Add one string value to the list
+        scenarios.extend(compare_scenario_list)   # Add elements from a list to the list (and not add a list as one element to the list)
+        return scenarios
+
+    def _calculate_max_length_dataset(self, data, scenarios):
+        """
+        Determine the max length of the list of the scenarios
+        """
+        # Check type of parameters
+        if not isinstance(data, dict):
+            raise TypeError("Variable data is not of type dictionary, but of type:"+str(data))
+        if not isinstance(scenarios, list):
+            raise TypeError("Variable scenarios is not of type list, but of type:"+str(scenarios))
+        
+        max_length = None
+        for scenario in scenarios:
+            if scenario not in data.keys():
+                raise ValueError("Scenario "+str(scenario)+" not in the keys of dictionary data:"+str(data.keys()))
+            if max_length is None:
+                max_length = len(data[scenario])
+            else:
+                max_length = max(max_length, len(data[scenario]))
+        if max_length is None:
+            raise ValueError("Could not find data to determine max_length:"+str(max_length))
+        return max_length
```

### Comparing `Clean Business Chart-0.1.1/clean_business_chart/general_functions.py` & `Clean Business Chart-0.1.2/clean_business_chart/general_functions.py`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/clean_business_chart/multiplier.py` & `Clean Business Chart-0.1.2/clean_business_chart/multiplier.py`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/docs/Makefile` & `Clean Business Chart-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/docs/conf.py` & `Clean Business Chart-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/docs/installation.rst` & `Clean Business Chart-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/docs/make.bat` & `Clean Business Chart-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/setup.py` & `Clean Business Chart-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-from setuptools import setup, find_packages
-
-with open('README.rst') as readme_file:
-    readme = readme_file.read()
-
-with open('HISTORY.rst') as history_file:
-    history = history_file.read()
-
-requirements = ['matplotlib>=3.5.1',
-                'pandas>=1.3']
-
-test_requirements = ['pytest>=3', ]
-
-setup(
-    author="Marcel Wuijtenburg",
-    author_email='marcelw1323@gmail.com',
-    python_requires='>=3.6',
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Financial and Insurance Industry',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Topic :: Scientific/Engineering :: Visualization',
-    ],
-    description="Clean Business Chart is a Python package for IBCS-like charts based on matplotlib.",
-    install_requires=requirements,
-    license="MIT license",
-    long_description=readme + '\n\n' + history,
-    include_package_data=True,
-    keywords=['clean business chart', 'IBCS', 'business chart', 'clean business charts', 'business charts'],
-    name='Clean Business Chart',
-    packages=find_packages(include=['clean_business_chart', 'clean_business_chart.*']),
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/marcelw1323/clean_business_chart',
-    version='0.1.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+from setuptools import setup, find_packages
+
+with open('README.rst') as readme_file:
+    readme = readme_file.read()
+
+with open('HISTORY.rst') as history_file:
+    history = history_file.read()
+
+requirements = ['matplotlib>=3.5.1',
+                'pandas>=1.3']
+
+test_requirements = ['pytest>=3', ]
+
+setup(
+    author="Marcel Wuijtenburg",
+    author_email='marcelw1323@gmail.com',
+    python_requires='>=3.6',
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Financial and Insurance Industry',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Scientific/Engineering :: Visualization',
+    ],
+    description="Clean Business Chart is a Python package for IBCS-like charts based on matplotlib.",
+    install_requires=requirements,
+    license="MIT license",
+    long_description=readme + '\n\n' + history,
+    include_package_data=True,
+    keywords=['clean business chart', 'IBCS', 'business chart', 'clean business charts', 'business charts', 'chart', 'charts'],
+    name='Clean Business Chart',
+    packages=find_packages(include=['clean_business_chart', 'clean_business_chart.*']),
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/marcelw1323/clean_business_chart',
+    version='0.1.2',
+    zip_safe=False,
+)
+
```

### Comparing `Clean Business Chart-0.1.1/tests/clean_business_chart/test_deltachart.py` & `Clean Business Chart-0.1.2/tests/clean_business_chart/test_deltachart.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""test DeltaChart-module"""
-
-from clean_business_chart.deltachart import *
-import pytest
-        
-def test_calculate_h():
-    # Test 1 - good delta calculation 
-    dataset = {'PY': [14, 16, 14, 17, 19, 17, 19, 22, 16, 17, 16, 22], 
-               'PL': [11, 10, 10, 10, 10, 10, 15, 14, 15, 15, 15, 19],
-               'AC': [15, 13, 16,  7,  5,  6, 17, 11],
-               'FC': [ 0,  0,  0,  0,  0,  0,  0,  0, 26, 22, 13, 29]} 
-    deltachart = DeltaChart()               
-    deltachart.calculate_h(data=dataset, base_scenario='PL', compare_scenario_list=['AC', 'FC'])
-    expected = ['AC', 'AC', 'AC', 'AC', 'AC', 'AC', 'AC', 'AC', 'FC', 'FC', 'FC', 'FC']
-    actual   = deltachart.delta_scenario_list
-    message  = "Test 1a - delta_scenario_list: deltachart.calculate returned {0} instead of {1}".format(actual, expected)
-    assert actual == expected, message
-
-    expected = [4, 3, 6, -3, -5, -4, 2, -3, 11, 7, -2, 10]
-    actual   = deltachart.delta_value_list
-    message = "Test 1b - delta_value_list: deltachart.calculate returned {0} instead of {1}".format(actual, expected)
-    assert actual == expected, message
-
-    # Test 2 - delta calculation not supported yet
-    with pytest.raises(ValueError):
-        dataset = {'PY': [14, 16, 14, 17, 19, 17, 19, 22, 16, 17, 16, 22], 
-                   'PL': [11, 10, 10, 10, 10, 10, 15, 14, 15, 15, 15, 19],
-                   'AC': [15, 13, 16,  7,  5,  6, 17, 11],
-                   'FC': [ 0,  0,  0,  0,  0,  0,  0, 15, 26, 22, 13, 29]}  # Number 15 added
-        actual = DeltaChart()               
+"""test DeltaChart-module"""
+
+from clean_business_chart.deltachart import *
+import pytest
+        
+def test_calculate_h():
+    # Test 1 - good delta calculation 
+    dataset = {'PY': [14, 16, 14, 17, 19, 17, 19, 22, 16, 17, 16, 22], 
+               'PL': [11, 10, 10, 10, 10, 10, 15, 14, 15, 15, 15, 19],
+               'AC': [15, 13, 16,  7,  5,  6, 17, 11],
+               'FC': [ 0,  0,  0,  0,  0,  0,  0,  0, 26, 22, 13, 29]} 
+    deltachart = DeltaChart()               
+    deltachart.calculate_h(data=dataset, base_scenario='PL', compare_scenario_list=['AC', 'FC'])
+    expected = ['AC', 'AC', 'AC', 'AC', 'AC', 'AC', 'AC', 'AC', 'FC', 'FC', 'FC', 'FC']
+    actual   = deltachart.delta_scenario_list
+    message  = "Test 1a - delta_scenario_list: deltachart.calculate returned {0} instead of {1}".format(actual, expected)
+    assert actual == expected, message
+
+    expected = [4, 3, 6, -3, -5, -4, 2, -3, 11, 7, -2, 10]
+    actual   = deltachart.delta_value_list
+    message = "Test 1b - delta_value_list: deltachart.calculate returned {0} instead of {1}".format(actual, expected)
+    assert actual == expected, message
+
+    # Test 2 - delta calculation not supported yet
+    with pytest.raises(ValueError):
+        dataset = {'PY': [14, 16, 14, 17, 19, 17, 19, 22, 16, 17, 16, 22], 
+                   'PL': [11, 10, 10, 10, 10, 10, 15, 14, 15, 15, 15, 19],
+                   'AC': [15, 13, 16,  7,  5,  6, 17, 11],
+                   'FC': [ 0,  0,  0,  0,  0,  0,  0, 15, 26, 22, 13, 29]}  # Number 15 added
+        actual = DeltaChart()               
         actual.calculate_h(data=dataset, base_scenario='PL', compare_scenario_list=['AC', 'FC'])
```

### Comparing `Clean Business Chart-0.1.1/tests/clean_business_chart/test_general_functions.py` & `Clean Business Chart-0.1.2/tests/clean_business_chart/test_general_functions.py`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/tests/clean_business_chart/test_multiplier.py` & `Clean Business Chart-0.1.2/tests/clean_business_chart/test_multiplier.py`

 * *Files identical despite different names*

### Comparing `Clean Business Chart-0.1.1/tests/test_clean_business_chart.py` & `Clean Business Chart-0.1.2/tests/test_clean_business_chart.py`

 * *Files identical despite different names*

