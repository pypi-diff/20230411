# Comparing `tmp/cryptographyComplements-0.2.5.tar.gz` & `tmp/cryptographyComplements-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.2.5.tar", last modified: Sun Apr  9 19:59:25 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.2.6.tar", last modified: Mon Apr 10 21:59:08 2023, max compression
```

## Comparing `cryptographyComplements-0.2.5.tar` & `cryptographyComplements-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 19:59:25.202017 cryptographyComplements-0.2.5/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-04-09 19:59:25.200645 cryptographyComplements-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.5/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:59:25.197551 cryptographyComplements-0.2.5/cryptographyComplements/
--rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.5/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     1631 2023-04-09 18:34:14.000000 cryptographyComplements-0.2.5/cryptographyComplements/ciphers.py
--rw-rw-rw-   0        0        0    10180 2023-04-09 19:58:33.000000 cryptographyComplements-0.2.5/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2510 2023-04-07 19:28:48.000000 cryptographyComplements-0.2.5/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     2252 2023-03-31 15:53:30.000000 cryptographyComplements-0.2.5/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:59:25.199643 cryptographyComplements-0.2.5/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      279 2023-04-09 19:59:25.000000 cryptographyComplements-0.2.5/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 19:59:25.202017 cryptographyComplements-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-09 19:59:13.000000 cryptographyComplements-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:59:08.067495 cryptographyComplements-0.2.6/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-04-10 21:59:08.066147 cryptographyComplements-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.6/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:59:08.055642 cryptographyComplements-0.2.6/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.6/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.6/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    10286 2023-04-10 21:53:29.000000 cryptographyComplements-0.2.6/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2575 2023-04-10 21:54:35.000000 cryptographyComplements-0.2.6/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     2332 2023-04-10 21:55:09.000000 cryptographyComplements-0.2.6/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:59:08.065085 cryptographyComplements-0.2.6/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-04-10 21:59:07.000000 cryptographyComplements-0.2.6/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 21:59:08.067495 cryptographyComplements-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-10 21:59:02.000000 cryptographyComplements-0.2.6/setup.py
```

### Comparing `cryptographyComplements-0.2.5/LICENSE` & `cryptographyComplements-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.5/PKG-INFO` & `cryptographyComplements-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.2.5/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.2.6/cryptographyComplements/mathFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"In this script you can find all the mathematical functions relative to Number Theory and Group Theory."
 from cryptographyComplements.tools import Numbers # required class, because contains functions used by some of them below
 
 def EulerTotientFunction(number: int):
     "Calculate, from a given number, the Euler Totient function."
     if not isinstance(number, int):
         return None
```

### Comparing `cryptographyComplements-0.2.5/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.2.6/cryptographyComplements/primalityTests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"In this script you can find all the Primality Test functions."
 from cryptographyComplements.tools import Numbers
 def EulerTotientPrimalityTest(n: int):
     "Using the equation: p - 1 = phi(p), you can verify if a number is prime. \nThis primality test is deterministic but numbers greater than 2^60 requires to much time, and computational power, to be calculated using this primality test."
 
     from cryptographyComplements.mathFunctions import EulerTotientFunction
 
     if not isinstance(n, int) and not isinstance(n, float):
```

### Comparing `cryptographyComplements-0.2.5/cryptographyComplements/tools.py` & `cryptographyComplements-0.2.6/cryptographyComplements/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"In this script you can find additional functions to reduce the code written."
 class Numbers:
 
     def isOdd(args):
         "Check if one or more numbers, entered in input, are odd."
 
         if isinstance(args, int):
             if args % 2 == 1:
```

### Comparing `cryptographyComplements-0.2.5/setup.py` & `cryptographyComplements-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cryptographyComplements',
-    version='0.2.5',
+    version='0.2.6',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

