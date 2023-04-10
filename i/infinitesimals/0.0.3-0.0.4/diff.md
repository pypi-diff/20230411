# Comparing `tmp/infinitesimals-0.0.3.tar.gz` & `tmp/infinitesimals-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinitesimals-0.0.3.tar", last modified: Mon Apr 10 21:38:19 2023, max compression
+gzip compressed data, was "infinitesimals-0.0.4.tar", last modified: Mon Apr 10 22:04:28 2023, max compression
```

## Comparing `infinitesimals-0.0.3.tar` & `infinitesimals-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:38:19.995757 infinitesimals-0.0.3/
--rw-rw-rw-   0        0        0      221 2023-04-10 21:36:21.000000 infinitesimals-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      966 2023-04-10 21:38:19.994760 infinitesimals-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.3/README.txt
--rw-rw-rw-   0        0        0     3282 2023-04-10 20:33:46.000000 infinitesimals-0.0.3/example.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:38:19.991768 infinitesimals-0.0.3/infinitesimals.egg-info/
--rw-rw-rw-   0        0        0      966 2023-04-10 21:38:19.000000 infinitesimals-0.0.3/infinitesimals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-10 21:38:19.000000 infinitesimals-0.0.3/infinitesimals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 21:38:19.000000 infinitesimals-0.0.3/infinitesimals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 21:38:19.000000 infinitesimals-0.0.3/infinitesimals.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-10 21:38:19.000000 infinitesimals-0.0.3/infinitesimals.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:38:19.995757 infinitesimals-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      885 2023-04-10 21:38:16.000000 infinitesimals-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:38:19.993763 infinitesimals-0.0.3/src/
--rw-rw-rw-   0        0        0    10188 2023-04-10 20:45:12.000000 infinitesimals-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:04:28.211332 infinitesimals-0.0.4/
+-rw-rw-rw-   0        0        0      292 2023-04-10 22:04:22.000000 infinitesimals-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1037 2023-04-10 22:04:28.209338 infinitesimals-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:04:28.202356 infinitesimals-0.0.4/infinitesimals.egg-info/
+-rw-rw-rw-   0        0        0     1037 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-10 22:04:28.000000 infinitesimals-0.0.4/infinitesimals.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:04:28.211332 infinitesimals-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-04-10 22:01:49.000000 infinitesimals-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:04:28.208340 infinitesimals-0.0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:59:32.000000 infinitesimals-0.0.4/src/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-04-10 22:01:57.000000 infinitesimals-0.0.4/src/example.py
+-rw-rw-rw-   0        0        0    10188 2023-04-10 20:45:12.000000 infinitesimals-0.0.4/src/infinitesimals.py
```

### Comparing `infinitesimals-0.0.3/LICENSE.txt` & `infinitesimals-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.3/PKG-INFO` & `infinitesimals-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.3
+Version: 0.0.4
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -26,7 +26,11 @@
 0.0.2 (10/04/2023)
 -------------------
 - Fixed install_requires
 
 0.0.3 (10/04/2023)
 -------------------
 - Fixed __init__ directory
+
+0.0.4 (10/04/2023)
+-------------------
+- Fixed __init__ directory
```

### Comparing `infinitesimals-0.0.3/example.py` & `infinitesimals-0.0.4/src/example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from __init__ import *
-import __init__ as infintesimals
+import infinitesimals
+from infinitesimals import *
 from math import floor, ceil
 from sys import float_info
 
 """Example program for demonstrating the capabilities of the infinitesimal library"""
 
 
 def main():
-
     print('initializing hyperreals is easy')
     x = HyperReal(1, 2, 1)  # also try "x = 1.0 + 2.0 * ε + (ε ** 2)" or "1.0 + 2.0 * epsilon + (epsilon ** 2)"
     print(x == (1.0 + 2.0 * ε + (ε ** 2)) == (1.0 + 2.0 * epsilon + (epsilon ** 2)), '\n')
 
     print('ε really is an infinitesimal, and not just a really small number')
     smallest_float = float_info.min  # 2.2250738585072014e-308
     print(0 < ε < smallest_float)
@@ -24,27 +23,27 @@
     print('every hyperreal, x, has a standard part st(x)==x.st, and infinitesimal part inf(x)==x.inf')
     print(f'{x=}, st(x)={x.st}, inf(x)={x.inf}', '\n')
 
     print('pythonic alternative for displaying hyperreals')
     print(repr(x), '\n')
 
     print('you can set how many terms will be used in calculations\n')
-    infintesimals.PRECISION = 10
+    infinitesimals.PRECISION = 10
 
     print('they support all elementary operations')
     print(f'1 / x = {1 / x}')
     print(f'x % 1 = {x % 1}')
     print(f'2 ** x = {2 ** x}\n')
 
     print('and common elementary operations')
     print(f'exp(x) = {exp(x)}')
     print(f'log(x) = {log(x)}')
     print(f'sin(x) = {sin(x)}\n')
 
-    infintesimals.PRECISION = 32  # default precision
+    infinitesimals.PRECISION = 32  # default precision
 
     print('their rounding behaviour is also consistent')
     print(f'floor(1 - ε) = {floor(1 - ε)}')
     print(f'ceil(10 + ε) = {ceil(10 + ε)}')
     print(f'round(0.5 + ε) = {round(0.5 + ε)}')
     print(f'round(0.5 - ε) = {round(0.5 - ε)}\n')
 
@@ -88,9 +87,10 @@
     except ZeroDivisionError as e:
         print(f'ZeroDivisionError: {e}')
         print('at the moment, infinities are not supported, but plan on being in a future version\n')
 
     print('hope you enjoy the infinitesimals library!')
     print('try commenting out various pieces code to play around with different features and limitations')
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `infinitesimals-0.0.3/infinitesimals.egg-info/PKG-INFO` & `infinitesimals-0.0.4/infinitesimals.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.3
+Version: 0.0.4
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -26,7 +26,11 @@
 0.0.2 (10/04/2023)
 -------------------
 - Fixed install_requires
 
 0.0.3 (10/04/2023)
 -------------------
 - Fixed __init__ directory
+
+0.0.4 (10/04/2023)
+-------------------
+- Fixed __init__ directory
```

### Comparing `infinitesimals-0.0.3/setup.py` & `infinitesimals-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='infinitesimals',
-    version='0.0.3',
+    version='0.0.4',
     description='A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
     keywords=['math', 'infinitesimal', 'infinitesimals', 'hyperreal', 'analysis', 'nonstandard analysis'],
     classifiers=classifiers,
-    packages=['src'],
+    packages=find_packages(),
     install_requires=['numpy', 'scipy']
 )
```

### Comparing `infinitesimals-0.0.3/src/__init__.py` & `infinitesimals-0.0.4/src/infinitesimals.py`

 * *Files identical despite different names*

