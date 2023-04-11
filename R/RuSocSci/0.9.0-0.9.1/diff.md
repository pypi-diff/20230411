# Comparing `tmp/RuSocSci-0.9.0-py2.py3-none-any.whl.zip` & `tmp/RuSocSci-0.9.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 26273 bytes, number of entries: 11
--rwxr-xr-x  2.0 unx      421 b- defN 22-Jun-20 10:59 rusocsci/__init__.py
+Zip file size: 26272 bytes, number of entries: 11
+-rwxr-xr-x  2.0 unx      423 b- defN 23-Apr-11 11:57 rusocsci/__init__.py
 -rwxr-xr-x  2.0 unx     8373 b- defN 19-Jul-05 08:08 rusocsci/buttonbox.py
 -rwxr-xr-x  2.0 unx     6802 b- defN 18-Sep-14 07:47 rusocsci/buttonbox2.py
 -rwxr-xr-x  2.0 unx     3935 b- defN 19-Jul-05 08:32 rusocsci/extended.py
 -rwxr-xr-x  2.0 unx     2491 b- defN 19-Jul-04 09:34 rusocsci/joystick.py
 -rwxr-xr-x  2.0 unx     9630 b- defN 22-Jun-20 10:59 rusocsci/utils.py
--rwxr-xr-x  2.0 unx    35147 b- defN 22-Jun-20 10:59 RuSocSci-0.9.0.dist-info/LICENSE
--rwxr-xr-x  2.0 unx      934 b- defN 22-Jun-20 10:59 RuSocSci-0.9.0.dist-info/METADATA
--rwxr-xr-x  2.0 unx      110 b- defN 22-Jun-20 10:59 RuSocSci-0.9.0.dist-info/WHEEL
--rwxr-xr-x  2.0 unx        9 b- defN 22-Jun-20 10:59 RuSocSci-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 22-Jun-20 10:59 RuSocSci-0.9.0.dist-info/RECORD
-11 files, 68704 bytes uncompressed, 24847 bytes compressed:  63.8%
+-rwxr-xr-x  2.0 unx    35147 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/LICENSE
+-rwxr-xr-x  2.0 unx      934 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/METADATA
+-rwxr-xr-x  2.0 unx      110 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx        9 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      852 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/RECORD
+11 files, 68706 bytes uncompressed, 24846 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: rusocsci/joystick.py
 Comment: 
 
 Filename: rusocsci/utils.py
 Comment: 
 
-Filename: RuSocSci-0.9.0.dist-info/LICENSE
+Filename: RuSocSci-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: RuSocSci-0.9.0.dist-info/METADATA
+Filename: RuSocSci-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: RuSocSci-0.9.0.dist-info/WHEEL
+Filename: RuSocSci-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: RuSocSci-0.9.0.dist-info/top_level.txt
+Filename: RuSocSci-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: RuSocSci-0.9.0.dist-info/RECORD
+Filename: RuSocSci-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rusocsci/__init__.py

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2013-2022 Wilbert van Ham, Radboud University Nijmegen
 # Distributed under the terms of the GNU General Public License (GPL).
 
 #version info for RuSocSci
-__version__='0.9'
+__version__='0.9.1'
 __license__='GNU GPLv3 (or more recent equivalent)'
 __author__='Wilbert van Ham'
 __author_email__='wilbert.vanham@ru.nl'
 __maintainer_email__='wilbert.vanham@ru.nl'
 __url__='https://www.socsci.ru.nl/wilberth/python/rusocsci.html'
```

## Comparing `RuSocSci-0.9.0.dist-info/LICENSE` & `RuSocSci-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `RuSocSci-0.9.0.dist-info/METADATA` & `RuSocSci-0.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RuSocSci
-Version: 0.9.0
+Version: 0.9.1
 Summary: Support package for Radboud University Nijmegen, Faculty of Social Sciences hardware, with PsychoPy-like API.
 Home-page: https://www.socsci.ru.nl/wilberth/python/rusocsci.html
 Author: Wilbert van Ham
 Author-email: w.vanham@socsci.ru.nl
 License: GPLv3+
 Keywords: hardware
 Platform: UNKNOWN
```

