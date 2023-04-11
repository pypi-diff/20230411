# Comparing `tmp/logo_standardizer-1.0.0.tar.gz` & `tmp/logo_standardizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logo_standardizer-1.0.0.tar", last modified: Tue Apr 11 16:03:29 2023, max compression
+gzip compressed data, was "logo_standardizer-1.0.1.tar", last modified: Tue Apr 11 16:11:18 2023, max compression
```

## Comparing `logo_standardizer-1.0.0.tar` & `logo_standardizer-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 16:03:29.470441 logo_standardizer-1.0.0/
--rw-rw-rw-   0        0        0     1103 2023-04-10 10:50:11.000000 logo_standardizer-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1339 2023-04-11 16:03:29.470441 logo_standardizer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-04-11 16:01:26.000000 logo_standardizer-1.0.0/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 14:56:41.000000 logo_standardizer-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      764 2023-04-11 16:03:29.473434 logo_standardizer-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 16:03:29.430434 logo_standardizer-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 16:03:29.451454 logo_standardizer-1.0.0/src/logo_standardizer/
--rw-rw-rw-   0        0        0        0 2023-04-10 11:01:38.000000 logo_standardizer-1.0.0/src/logo_standardizer/__init__.py
--rw-rw-rw-   0        0        0     7930 2023-04-10 09:41:20.000000 logo_standardizer-1.0.0/src/logo_standardizer/logo_standardize.py
-drwxrwxrwx   0        0        0        0 2023-04-11 16:03:29.467451 logo_standardizer-1.0.0/src/logo_standardizer.egg-info/
--rw-rw-rw-   0        0        0     1339 2023-04-11 16:03:29.000000 logo_standardizer-1.0.0/src/logo_standardizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-11 16:03:29.000000 logo_standardizer-1.0.0/src/logo_standardizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 16:03:29.000000 logo_standardizer-1.0.0/src/logo_standardizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-11 16:03:29.000000 logo_standardizer-1.0.0/src/logo_standardizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-11 16:03:29.000000 logo_standardizer-1.0.0/src/logo_standardizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 16:11:18.021646 logo_standardizer-1.0.1/
+-rw-rw-rw-   0        0        0     1103 2023-04-10 10:50:11.000000 logo_standardizer-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1336 2023-04-11 16:11:18.021646 logo_standardizer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-04-11 16:10:35.000000 logo_standardizer-1.0.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 14:56:41.000000 logo_standardizer-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      764 2023-04-11 16:11:18.023634 logo_standardizer-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 16:11:17.977609 logo_standardizer-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 16:11:18.004641 logo_standardizer-1.0.1/src/logo_standardizer/
+-rw-rw-rw-   0        0        0        0 2023-04-10 11:01:38.000000 logo_standardizer-1.0.1/src/logo_standardizer/__init__.py
+-rw-rw-rw-   0        0        0     7930 2023-04-10 09:41:20.000000 logo_standardizer-1.0.1/src/logo_standardizer/logo_standardize.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:11:18.019607 logo_standardizer-1.0.1/src/logo_standardizer.egg-info/
+-rw-rw-rw-   0        0        0     1336 2023-04-11 16:11:17.000000 logo_standardizer-1.0.1/src/logo_standardizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-11 16:11:17.000000 logo_standardizer-1.0.1/src/logo_standardizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 16:11:17.000000 logo_standardizer-1.0.1/src/logo_standardizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-11 16:11:17.000000 logo_standardizer-1.0.1/src/logo_standardizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-11 16:11:17.000000 logo_standardizer-1.0.1/src/logo_standardizer.egg-info/top_level.txt
```

### Comparing `logo_standardizer-1.0.0/LICENSE` & `logo_standardizer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logo_standardizer-1.0.0/PKG-INFO` & `logo_standardizer-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logo_standardizer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Smart logo standardizer
 Author: Mohammed Elsiddig (Jubii)
 Author-email: mohammedjelsiddig@gmail.com
 Keywords: python,logo,standardization,logo standardizer,logo resizer,logo standardize,resize,standardize
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 ## Description
 
 A smart logo standardizer that detects both the logo and the background of an unstandardized logo picture and  transforms it into the desired logo standards for app circled or general front-end display.
 
 ## Installation
 
-\$ pip install -i logo-standardizer==1.0.0
+\$ pip install logo-standardizer==1.0.1
 
 ## Usage
 
 A brief example of how to use the package:
 
 ```python
 from logo_standardizer import logo_standardize
```

### Comparing `logo_standardizer-1.0.0/README.md` & `logo_standardizer-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Description
 
 A smart logo standardizer that detects both the logo and the background of an unstandardized logo picture and  transforms it into the desired logo standards for app circled or general front-end display.
 
 ## Installation
 
-\$ pip install -i logo-standardizer==1.0.0
+\$ pip install logo-standardizer==1.0.1
 
 ## Usage
 
 A brief example of how to use the package:
 
 ```python
 from logo_standardizer import logo_standardize
```

### Comparing `logo_standardizer-1.0.0/setup.cfg` & `logo_standardizer-1.0.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6f67 6f5f 7374 616e 6461 7264   = logo_standard
 00000020: 697a 6572 0d0a 7665 7273 696f 6e20 3d20  izer..version = 
-00000030: 312e 302e 300d 0a61 7574 686f 7220 3d20  1.0.0..author = 
+00000030: 312e 302e 310d 0a61 7574 686f 7220 3d20  1.0.1..author = 
 00000040: 4d6f 6861 6d6d 6564 2045 6c73 6964 6469  Mohammed Elsiddi
 00000050: 6720 284a 7562 6969 290d 0a61 7574 686f  g (Jubii)..autho
 00000060: 725f 656d 6169 6c20 3d20 6d6f 6861 6d6d  r_email = mohamm
 00000070: 6564 6a65 6c73 6964 6469 6740 676d 6169  edjelsiddig@gmai
 00000080: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000090: 6f6e 203d 2053 6d61 7274 206c 6f67 6f20  on = Smart logo 
 000000a0: 7374 616e 6461 7264 697a 6572 0d0a 6c6f  standardizer..lo
```

### Comparing `logo_standardizer-1.0.0/src/logo_standardizer/logo_standardize.py` & `logo_standardizer-1.0.1/src/logo_standardizer/logo_standardize.py`

 * *Files identical despite different names*

### Comparing `logo_standardizer-1.0.0/src/logo_standardizer.egg-info/PKG-INFO` & `logo_standardizer-1.0.1/src/logo_standardizer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logo-standardizer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Smart logo standardizer
 Author: Mohammed Elsiddig (Jubii)
 Author-email: mohammedjelsiddig@gmail.com
 Keywords: python,logo,standardization,logo standardizer,logo resizer,logo standardize,resize,standardize
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 ## Description
 
 A smart logo standardizer that detects both the logo and the background of an unstandardized logo picture and  transforms it into the desired logo standards for app circled or general front-end display.
 
 ## Installation
 
-\$ pip install -i logo-standardizer==1.0.0
+\$ pip install logo-standardizer==1.0.1
 
 ## Usage
 
 A brief example of how to use the package:
 
 ```python
 from logo_standardizer import logo_standardize
```

