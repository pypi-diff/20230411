# Comparing `tmp/riemann-0.9.0.tar.gz` & `tmp/riemann-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riemann-0.9.0.tar", last modified: Sun Jan  1 07:31:56 2023, max compression
+gzip compressed data, was "riemann-1.0.0a1.tar", last modified: Tue Apr 11 15:16:46 2023, max compression
```

## Comparing `riemann-0.9.0.tar` & `riemann-1.0.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-01-01 07:31:56.388940 riemann-0.9.0/
--rw-rw-rw-   0        0        0     1085 2022-11-19 19:02:44.000000 riemann-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     3993 2023-01-01 07:31:56.387945 riemann-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2953 2022-11-23 18:43:36.000000 riemann-0.9.0/README.md
--rw-rw-rw-   0        0        0     1121 2023-01-01 07:30:50.000000 riemann-0.9.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-01 07:31:56.385937 riemann-0.9.0/riemann.egg-info/
--rw-rw-rw-   0        0        0     3993 2023-01-01 07:31:56.000000 riemann-0.9.0/riemann.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-01-01 07:31:56.000000 riemann-0.9.0/riemann.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-01 07:31:56.000000 riemann-0.9.0/riemann.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-01-01 07:31:56.000000 riemann-0.9.0/riemann.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6756 2023-01-01 07:28:55.000000 riemann-0.9.0/riemann.py
--rw-rw-rw-   0        0        0       42 2023-01-01 07:31:56.388940 riemann-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 15:16:46.825995 riemann-1.0.0a1/
+-rw-rw-rw-   0        0        0     1085 2022-11-19 19:02:44.000000 riemann-1.0.0a1/LICENSE
+-rw-rw-rw-   0        0        0     3502 2023-04-11 15:16:46.825995 riemann-1.0.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     2514 2023-01-06 20:40:44.000000 riemann-1.0.0a1/README.md
+-rw-rw-rw-   0        0        0     1078 2023-04-11 15:14:54.000000 riemann-1.0.0a1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-11 15:16:46.825995 riemann-1.0.0a1/riemann.egg-info/
+-rw-rw-rw-   0        0        0     3502 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8605 2023-04-11 15:10:16.000000 riemann-1.0.0a1/riemann.py
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:16:46.825995 riemann-1.0.0a1/setup.cfg
```

### Comparing `riemann-0.9.0/LICENSE` & `riemann-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `riemann-0.9.0/PKG-INFO` & `riemann-1.0.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,77 @@
 Metadata-Version: 2.1
 Name: riemann
-Version: 0.9.0
+Version: 1.0.0a1
 Summary: A package for computing Riemann summations in n-dimensional space
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 Project-URL: Homepage, https://github.com/JacobLee23/riemann
 Project-URL: Documentation, https://riemann-py.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/JacobLee23/riemann/issues/
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # riemann
 
 ![Repository Logo](docs/_static/riemann-logo.png)
 
-**Riemann** is a pure-Python package for computing Riemann sums of functions in $n$-dimensional space.
+**Riemann**, a pure-Python package for computing Riemann sums of functions of several real variables.
 
 [![GitHub](https://img.shields.io/github/license/JacobLee23/riemann)](https://github.com/JacobLee23/riemann/blob/master/LICENSE)
 ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/JacobLee23/riemann)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/riemann)](https://pypi.org/project/riemann)
 [![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/Jacoblee23/riemann)](https://github.com/JacobLee23/riemann/tags)
 
 ***
 
 ## Basic Usage
 
-**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function over a closed interval. The below code snippet computes the Riemann sum of $f(x) = x^{2}$ over the interval $[0, 2]$ using 10 partitions along the $x$ axis.
+**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function over a closed interval. The below code snippet computes the Riemann sum of $f(x) = x^{2}$ over the interval $[0, 1]$ using 10 partitions along the $x$ axis.
 
 ```python
 >>> import riemann
->>> from riemann import Dimension
+>>> from riemann import Interval
 >>> f = lambda x: x ** 2
->>> dim_x = Dimension(0, 2, 10, riemann.LOWER)
->>> dim_x
-Dimension(a=0, b=2, n=10, method=Method(name='lower'))
->>> riemann.rsum(f, dim_x)
-Decimal('2.28')
+>>> intervals = [Interval(0, 1, 10)]
+>>> methods = [riemann.LEFT]
+>>> riemann.rsum(f, intervals, methods)
+Decimal('0.285')
 ```
 
-However, **Riemann** is not restricted to computing Riemann sums only over one dimension. A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensional interval. The below code snippet computes the Riemann sum of $f(x, y) = x^{2} y^{2}$ over the interval $x \in [0, 2], y \in [0, 4]$ using 10 partitions along the $x$ axis and 10 partitions along the $y$ axis.
+However, **Riemann** is not restricted to computing Riemann sums only over one dimension. A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensional interval. The below code snippet computes the Riemann sum of $f(x, y) = x^{2} + y^{2}$ over the interval $x \in [0, 1], y \in [0, 1]$ using 10 partitions along the $x$ axis and 10 partitions along the $y$ axis.
 
 ```python
 >>> import riemann
->>> from riemann import Dimension
->>> f = lambda x, y: (x ** 2) * (y ** 2)
->>> dim_x = Dimension(0, 2, 10, riemann.MIDDLE)
->>> dim_x
-Dimension(a=0, b=2, n=10, method=Method(name='middle'))
->>> dim_y = Dimension(0, 4, 10, riemann.MIDDLE)
->>> dim_y
-Dimension(a=0, b=4, n=10, method=Method(name='middle'))
->>> riemann.rsum(f, dim_x, dim_y)
-Decimal('56.6048')
+>>> from riemann import Interval
+>>> f = lambda x, y: x ** 2 + y ** 2
+>>> intervals = [Interval(0, 1, 10), Interval(0, 1, 10)]
+>>> methods = [riemann.LEFT, riemann.LEFT]
+>>> riemann.rsum(f, intervals, methods)
+Decimal('0.57')
 ```
 
-The sole requirement is that the number of parameters taken by the function passed as the `func` argument to `riemann.rsum` equals the number of `riemann.Dimension` objects passed.
-
 ## Features
 
 - Fast computation of Riemann sum.
 - Support for computation of multi-dimensional Riemann sum.
 - Built-in support for left, middle, and right Riemann sum methods.
-- Support for custom Riemann sum methods (using the :py:class:`riemann.Method` class).
 
 ## Requirements
 
-**Riemann** requires Python 3.7+. This project does not require any additional dependencies.
+**Riemann** requires Python 3.5+. This project does not require any additional dependencies.
 
 ## Installation
 
 ```console
 $ pip install riemann
 ```
```

### Comparing `riemann-0.9.0/pyproject.toml` & `riemann-1.0.0a1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel >= 0.29.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "riemann"
-version = "0.9.0"
+version = "1.0.0-a.1"
 authors = [
   { name="Jacob Lee", email="Jacob.J.Lee@outlook.com" },
 ]
 description = "A package for computing Riemann summations in n-dimensional space"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
-  "Development Status :: 1 - Planning",
+  "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Mathematics",
 ]
```

### Comparing `riemann-0.9.0/riemann.egg-info/PKG-INFO` & `riemann-1.0.0a1/riemann.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,77 @@
 Metadata-Version: 2.1
 Name: riemann
-Version: 0.9.0
+Version: 1.0.0a1
 Summary: A package for computing Riemann summations in n-dimensional space
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 Project-URL: Homepage, https://github.com/JacobLee23/riemann
 Project-URL: Documentation, https://riemann-py.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/JacobLee23/riemann/issues/
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # riemann
 
 ![Repository Logo](docs/_static/riemann-logo.png)
 
-**Riemann** is a pure-Python package for computing Riemann sums of functions in $n$-dimensional space.
+**Riemann**, a pure-Python package for computing Riemann sums of functions of several real variables.
 
 [![GitHub](https://img.shields.io/github/license/JacobLee23/riemann)](https://github.com/JacobLee23/riemann/blob/master/LICENSE)
 ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/JacobLee23/riemann)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/riemann)](https://pypi.org/project/riemann)
 [![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/Jacoblee23/riemann)](https://github.com/JacobLee23/riemann/tags)
 
 ***
 
 ## Basic Usage
 
-**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function over a closed interval. The below code snippet computes the Riemann sum of $f(x) = x^{2}$ over the interval $[0, 2]$ using 10 partitions along the $x$ axis.
+**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function over a closed interval. The below code snippet computes the Riemann sum of $f(x) = x^{2}$ over the interval $[0, 1]$ using 10 partitions along the $x$ axis.
 
 ```python
 >>> import riemann
->>> from riemann import Dimension
+>>> from riemann import Interval
 >>> f = lambda x: x ** 2
->>> dim_x = Dimension(0, 2, 10, riemann.LOWER)
->>> dim_x
-Dimension(a=0, b=2, n=10, method=Method(name='lower'))
->>> riemann.rsum(f, dim_x)
-Decimal('2.28')
+>>> intervals = [Interval(0, 1, 10)]
+>>> methods = [riemann.LEFT]
+>>> riemann.rsum(f, intervals, methods)
+Decimal('0.285')
 ```
 
-However, **Riemann** is not restricted to computing Riemann sums only over one dimension. A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensional interval. The below code snippet computes the Riemann sum of $f(x, y) = x^{2} y^{2}$ over the interval $x \in [0, 2], y \in [0, 4]$ using 10 partitions along the $x$ axis and 10 partitions along the $y$ axis.
+However, **Riemann** is not restricted to computing Riemann sums only over one dimension. A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensional interval. The below code snippet computes the Riemann sum of $f(x, y) = x^{2} + y^{2}$ over the interval $x \in [0, 1], y \in [0, 1]$ using 10 partitions along the $x$ axis and 10 partitions along the $y$ axis.
 
 ```python
 >>> import riemann
->>> from riemann import Dimension
->>> f = lambda x, y: (x ** 2) * (y ** 2)
->>> dim_x = Dimension(0, 2, 10, riemann.MIDDLE)
->>> dim_x
-Dimension(a=0, b=2, n=10, method=Method(name='middle'))
->>> dim_y = Dimension(0, 4, 10, riemann.MIDDLE)
->>> dim_y
-Dimension(a=0, b=4, n=10, method=Method(name='middle'))
->>> riemann.rsum(f, dim_x, dim_y)
-Decimal('56.6048')
+>>> from riemann import Interval
+>>> f = lambda x, y: x ** 2 + y ** 2
+>>> intervals = [Interval(0, 1, 10), Interval(0, 1, 10)]
+>>> methods = [riemann.LEFT, riemann.LEFT]
+>>> riemann.rsum(f, intervals, methods)
+Decimal('0.57')
 ```
 
-The sole requirement is that the number of parameters taken by the function passed as the `func` argument to `riemann.rsum` equals the number of `riemann.Dimension` objects passed.
-
 ## Features
 
 - Fast computation of Riemann sum.
 - Support for computation of multi-dimensional Riemann sum.
 - Built-in support for left, middle, and right Riemann sum methods.
-- Support for custom Riemann sum methods (using the :py:class:`riemann.Method` class).
 
 ## Requirements
 
-**Riemann** requires Python 3.7+. This project does not require any additional dependencies.
+**Riemann** requires Python 3.5+. This project does not require any additional dependencies.
 
 ## Installation
 
 ```console
 $ pip install riemann
 ```
```

