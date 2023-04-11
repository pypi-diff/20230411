# Comparing `tmp/cleopatra-0.2.7.tar.gz` & `tmp/cleopatra-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleopatra-0.2.7.tar", max compression
+gzip compressed data, was "cleopatra-0.3.0.tar", last modified: Tue Apr 11 15:48:53 2023, max compression
```

## Comparing `cleopatra-0.2.7.tar` & `cleopatra-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,23 @@
--rw-r--r--   0        0        0     1069 2022-09-18 17:34:36.036000 cleopatra-0.2.7/cleopatra/__init__.py
--rw-r--r--   0        0        0    33111 2023-01-13 19:52:00.288638 cleopatra-0.2.7/cleopatra/array.py
--rw-r--r--   0        0        0    35591 2022-03-20 16:22:07.110000 cleopatra-0.2.7/LICENSE.md
--rw-r--r--   0        0        0     2044 2023-01-31 15:35:30.422124 cleopatra-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5081 2023-01-31 15:39:36.466608 cleopatra-0.2.7/README.md
--rw-r--r--   0        0        0     5791 1970-01-01 00:00:00.000000 cleopatra-0.2.7/setup.py
--rw-r--r--   0        0        0     6428 1970-01-01 00:00:00.000000 cleopatra-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.285976 cleopatra-0.3.0/
+-rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0     6829 2023-04-11 15:48:53.285976 cleopatra-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5081 2023-04-11 15:41:59.000000 cleopatra-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.133428 cleopatra-0.3.0/cleopatra/
+-rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/__init__.py
+-rw-rw-rw-   0        0        0    34725 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/array.py
+-rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/statistics.py
+-rw-rw-rw-   0        0        0     6499 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.175884 cleopatra-0.3.0/cleopatra.egg-info/
+-rw-rw-rw-   0        0        0     6829 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-04-11 15:48:53.000000 cleopatra-0.3.0/cleopatra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:48:53.285976 cleopatra-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1689 2023-04-11 15:41:59.000000 cleopatra-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.251482 cleopatra-0.3.0/tests/
+-rw-rw-rw-   0        0        0     7940 2023-04-11 15:41:59.000000 cleopatra-0.3.0/tests/test_plot_array.py
+-rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.0/tests/test_statistics.py
+-rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.0/tests/test_styles.py
```

### Comparing `cleopatra-0.2.7/cleopatra/__init__.py` & `cleopatra-0.3.0/cleopatra/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # documentation format
 __author__ = "Mostafa Farrag"
 __email__ = "moah.farag@gmail.com"
 __docformat__ = "restructuredtext"
 
 # Let users know if they're missing any of our hard dependencies
-hard_dependencies = ()  # ("numpy", "pandas", "gdal")
+hard_dependencies = ()
 missing_dependencies = []
 
 for dependency in hard_dependencies:
     try:
         __import__(dependency)
     except ImportError as e:
         missing_dependencies.append(dependency)
```

### Comparing `cleopatra-0.2.7/LICENSE.md` & `cleopatra-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cleopatra-0.2.7/README.md` & `cleopatra-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.2.7
+pip install cleopatra==0.3.0
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
```

### Comparing `cleopatra-0.2.7/PKG-INFO` & `cleopatra-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,125 @@
-Metadata-Version: 2.1
-Name: cleopatra
-Version: 0.2.7
-Summary: visualization package
-Home-page: https://github.com/MAfarrag/cleopatra
-License: GNU General Public License v3
-Keywords: matplotlib,arrays,visualization
-Author: Mostafa Farrag
-Author-email: moah.farag@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: License :: Other/Proprietary License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: serapeum_utils (>=0.1.1,<0.2.0)
-Project-URL: Documentation, https://cleopatra.readthedocs.io/
-Project-URL: Repository, https://github.com/MAfarrag/cleopatra
-Description-Content-Type: text/markdown
-
-[![Python Versions](https://img.shields.io/pypi/pyversions/cleopatra.png)](https://img.shields.io/pypi/pyversions/cleopatra)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/MAfarrag/cleopatra.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/MAfarrag/cleopatra/context:python)
-[![Documentation Status](https://readthedocs.org/projects/cleopatra/badge/?version=latest)](https://cleopatra.readthedocs.io/en/latest/?badge=latest)
-[![codecov](https://codecov.io/github/Serapieum-of-alex/cleopatra/branch/main/graph/badge.svg?token=gHxH7ljIC3)](https://codecov.io/github/Serapieum-of-alex/cleopatra)
-
-![GitHub last commit](https://img.shields.io/github/last-commit/MAfarrag/cleopatra)
-![GitHub forks](https://img.shields.io/github/forks/MAfarrag/cleopatra?style=social)
-![GitHub Repo stars](https://img.shields.io/github/stars/MAfarrag/cleopatra?style=social)
-
-
-Current release info
-====================
-
-| Name | Downloads                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Version | Platforms |
-| --- |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| --- | --- |
-| [![Conda Recipe](https://img.shields.io/badge/recipe-cleopatra-green.svg)](https://anaconda.org/conda-forge/cleopatra) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/cleopatra.svg)](https://anaconda.org/conda-forge/cleopatra) [![Downloads](https://pepy.tech/badge/cleopatra)](https://pepy.tech/project/cleopatra) [![Downloads](https://pepy.tech/badge/cleopatra/month)](https://pepy.tech/project/cleopatra)  [![Downloads](https://pepy.tech/badge/cleopatra/week)](https://pepy.tech/project/cleopatra)  ![PyPI - Downloads](https://img.shields.io/pypi/dd/cleopatra?color=blue&style=flat-square) ![GitHub all releases](https://img.shields.io/github/downloads/MAfarrag/cleopatra/total) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cleopatra.svg)](https://anaconda.org/conda-forge/cleopatra) [![PyPI version](https://badge.fury.io/py/cleopatra.svg)](https://badge.fury.io/py/cleopatra) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cleopatra/badges/version.svg)](https://anaconda.org/conda-forge/cleopatra) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/cleopatra.svg)](https://anaconda.org/conda-forge/cleopatra) [![Join the chat at https://gitter.im/Hapi-Nile/Hapi](https://badges.gitter.im/Hapi-Nile/Hapi.svg)](https://gitter.im/Hapi-Nile/Hapi?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) |
-
-cleopatra - matplotlib utility package
-=====================================================================
-**cleopatra** is a matplotlib utility package
-
-cleopatra
-
-
-Installing cleopatra
-===============
-
-Installing `cleopatra` from the `conda-forge` channel can be achieved by:
-
-```
-conda install -c conda-forge cleopatra
-```
-
-It is possible to list all of the versions of `cleopatra` available on your platform with:
-
-```
-conda search cleopatra --channel conda-forge
-```
-
-## Install from Github
-to install the last development to time you can install the library from github
-```
-pip install git+https://github.com/MAfarrag/cleopatra
-```
-
-## pip
-to install the last release you can easly use pip
-```
-pip install cleopatra==0.2.7
-```
-
-Quick start
-===========
-
-```
-  >>> import cleopatra
-```
-
-[other code samples](https://cleopatra.readthedocs.io/en/latest/?badge=latest)
-
+Metadata-Version: 2.1
+Name: cleopatra
+Version: 0.3.0
+Summary: visualization package
+Home-page: https://github.com/MAfarrag/cleopatra
+Author: Mostafa Farrag
+Author-email: moah.farag@gmail.come
+License: GNU General Public License v3
+Keywords: matplotlib,arrays,visualization
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: AUTHORS.rst
+
+[![Python Versions](https://img.shields.io/pypi/pyversions/cleopatra.png)](https://img.shields.io/pypi/pyversions/cleopatra)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/MAfarrag/cleopatra.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/MAfarrag/cleopatra/context:python)
+[![Documentation Status](https://readthedocs.org/projects/cleopatra/badge/?version=latest)](https://cleopatra.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/github/Serapieum-of-alex/cleopatra/branch/main/graph/badge.svg?token=gHxH7ljIC3)](https://codecov.io/github/Serapieum-of-alex/cleopatra)
+
+![GitHub last commit](https://img.shields.io/github/last-commit/MAfarrag/cleopatra)
+![GitHub forks](https://img.shields.io/github/forks/MAfarrag/cleopatra?style=social)
+![GitHub Repo stars](https://img.shields.io/github/stars/MAfarrag/cleopatra?style=social)
+
+
+Current release info
+====================
+
+| Name | Downloads                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Version | Platforms |
+| --- |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| --- | --- |
+| [![Conda Recipe](https://img.shields.io/badge/recipe-cleopatra-green.svg)](https://anaconda.org/conda-forge/cleopatra) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/cleopatra.svg)](https://anaconda.org/conda-forge/cleopatra) [![Downloads](https://pepy.tech/badge/cleopatra)](https://pepy.tech/project/cleopatra) [![Downloads](https://pepy.tech/badge/cleopatra/month)](https://pepy.tech/project/cleopatra)  [![Downloads](https://pepy.tech/badge/cleopatra/week)](https://pepy.tech/project/cleopatra)  ![PyPI - Downloads](https://img.shields.io/pypi/dd/cleopatra?color=blue&style=flat-square) ![GitHub all releases](https://img.shields.io/github/downloads/MAfarrag/cleopatra/total) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cleopatra.svg)](https://anaconda.org/conda-forge/cleopatra) [![PyPI version](https://badge.fury.io/py/cleopatra.svg)](https://badge.fury.io/py/cleopatra) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cleopatra/badges/version.svg)](https://anaconda.org/conda-forge/cleopatra) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/cleopatra.svg)](https://anaconda.org/conda-forge/cleopatra) [![Join the chat at https://gitter.im/Hapi-Nile/Hapi](https://badges.gitter.im/Hapi-Nile/Hapi.svg)](https://gitter.im/Hapi-Nile/Hapi?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) |
+
+cleopatra - matplotlib utility package
+=====================================================================
+**cleopatra** is a matplotlib utility package
+
+cleopatra
+
+
+Installing cleopatra
+===============
+
+Installing `cleopatra` from the `conda-forge` channel can be achieved by:
+
+```
+conda install -c conda-forge cleopatra
+```
+
+It is possible to list all of the versions of `cleopatra` available on your platform with:
+
+```
+conda search cleopatra --channel conda-forge
+```
+
+## Install from Github
+to install the last development to time you can install the library from github
+```
+pip install git+https://github.com/MAfarrag/cleopatra
+```
+
+## pip
+to install the last release you can easly use pip
+```
+pip install cleopatra==0.3.0
+```
+
+Quick start
+===========
+
+```
+  >>> import cleopatra
+```
+
+[other code samples](https://cleopatra.readthedocs.io/en/latest/?badge=latest)
+
+
+=======
+History
+=======
+
+0.1.0 (2022-05-24)
+------------------
+
+* First release on PyPI.
+
+0.2.4 (2022-12-26)
+------------------
+
+* bump up numpy versions to 1.23.5, add pandas
+
+0.2.5 (2022-12-26)
+------------------
+
+* plot array with discrete bounds takes the bounds as a parameter
+
+0.2.6 (2023-01-31)
+------------------
+
+* bump up versions
+* add serapeum_utils as a dependency
+
+0.2.7 (2023-01-31)
+------------------
+* bump up numpy to version 1.24.1
+
+
+0.3.0 (2023-04-11)
+------------------
+* change API to work completly with numpy array inputs
+* chenge to conda config
+* add hpc-utils to filter and access arrays
+* restructure the whole modules to array, statistics, and styles modules.
+* all modules has classes.
+* save animation function using ffmpeg.
```

