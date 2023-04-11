# Comparing `tmp/doubleagent-1.62.tar.gz` & `tmp/doubleagent-1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doubleagent-1.62.tar", last modified: Tue Apr 11 06:42:28 2023, max compression
+gzip compressed data, was "doubleagent-1.63.tar", last modified: Tue Apr 11 07:00:52 2023, max compression
```

## Comparing `doubleagent-1.62.tar` & `doubleagent-1.63.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 06:42:28.697201 doubleagent-1.62/
--rw-rw-rw-   0        0        0      305 2023-04-11 06:42:28.697201 doubleagent-1.62/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 06:42:28.683199 doubleagent-1.62/doubleagent/
--rw-rw-rw-   0        0        0      910 2023-04-11 06:26:19.000000 doubleagent-1.62/doubleagent/__init__.py
--rw-rw-rw-   0        0        0      287 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/alldel.py
--rw-rw-rw-   0        0        0      375 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/alpacomposite.py
--rw-rw-rw-   0        0        0      164 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/cases.py
--rw-rw-rw-   0        0        0      167 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/errorboy.py
--rw-rw-rw-   0        0        0      313 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/horizonpaste.py
--rw-rw-rw-   0        0        0       80 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/listsplit.py
--rw-rw-rw-   0        0        0      174 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/ll2l.py
--rw-rw-rw-   0        0        0       92 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/mix.py
--rw-rw-rw-   0        0        0      694 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/multiplesplit.py
--rw-rw-rw-   0        0        0      191 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/overlapchecker.py
--rw-rw-rw-   0        0        0      128 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/picklemaker.py
--rw-rw-rw-   0        0        0      139 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/picklereader.py
--rw-rw-rw-   0        0        0      252 2023-04-11 06:41:48.000000 doubleagent-1.62/doubleagent/pinset.py
--rw-rw-rw-   0        0        0      116 2023-04-11 06:24:55.000000 doubleagent-1.62/doubleagent/readfile.py
--rw-rw-rw-   0        0        0     1717 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/rectangularcroplocation.py
--rw-rw-rw-   0        0        0      820 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/removeAlpha.py
--rw-rw-rw-   0        0        0      109 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/report.py
--rw-rw-rw-   0        0        0      710 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/rightreplace.py
--rw-rw-rw-   0        0        0      589 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/roundimage.py
--rw-rw-rw-   0        0        0       56 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/s2l.py
--rw-rw-rw-   0        0        0     3293 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/seleupdate.py
--rw-rw-rw-   0        0        0      915 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/speedcases.py
--rw-rw-rw-   0        0        0      103 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/sublist.py
--rw-rw-rw-   0        0        0     2085 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/txt2crop.py
--rw-rw-rw-   0        0        0      151 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/unanimous.py
--rw-rw-rw-   0        0        0      323 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/verticalpaste.py
--rw-rw-rw-   0        0        0      296 2023-02-01 02:33:29.000000 doubleagent-1.62/doubleagent/whiterbg.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:42:28.695202 doubleagent-1.62/doubleagent.egg-info/
--rw-rw-rw-   0        0        0      305 2023-04-11 06:42:28.000000 doubleagent-1.62/doubleagent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-04-11 06:42:28.000000 doubleagent-1.62/doubleagent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 06:42:28.000000 doubleagent-1.62/doubleagent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 06:42:28.000000 doubleagent-1.62/doubleagent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 06:42:28.697201 doubleagent-1.62/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-04-11 05:58:21.000000 doubleagent-1.62/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:00:52.910813 doubleagent-1.63/
+-rw-rw-rw-   0        0        0      305 2023-04-11 07:00:52.910813 doubleagent-1.63/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 07:00:52.902811 doubleagent-1.63/doubleagent/
+-rw-rw-rw-   0        0        0      938 2023-04-11 06:45:08.000000 doubleagent-1.63/doubleagent/__init__.py
+-rw-rw-rw-   0        0        0      287 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/alldel.py
+-rw-rw-rw-   0        0        0      375 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/alpacomposite.py
+-rw-rw-rw-   0        0        0      164 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/cases.py
+-rw-rw-rw-   0        0        0      167 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/errorboy.py
+-rw-rw-rw-   0        0        0      313 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/horizonpaste.py
+-rw-rw-rw-   0        0        0       80 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/listsplit.py
+-rw-rw-rw-   0        0        0      174 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/ll2l.py
+-rw-rw-rw-   0        0        0       92 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/mix.py
+-rw-rw-rw-   0        0        0      694 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/multiplesplit.py
+-rw-rw-rw-   0        0        0      191 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/overlapchecker.py
+-rw-rw-rw-   0        0        0      128 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/picklemaker.py
+-rw-rw-rw-   0        0        0      139 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/picklereader.py
+-rw-rw-rw-   0        0        0      252 2023-04-11 06:41:48.000000 doubleagent-1.63/doubleagent/pinset.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 06:46:03.000000 doubleagent-1.63/doubleagent/readfile.py
+-rw-rw-rw-   0        0        0     1717 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/rectangularcroplocation.py
+-rw-rw-rw-   0        0        0      820 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/removeAlpha.py
+-rw-rw-rw-   0        0        0      109 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/report.py
+-rw-rw-rw-   0        0        0      710 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/rightreplace.py
+-rw-rw-rw-   0        0        0      589 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/roundimage.py
+-rw-rw-rw-   0        0        0       56 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/s2l.py
+-rw-rw-rw-   0        0        0     3293 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/seleupdate.py
+-rw-rw-rw-   0        0        0      915 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/speedcases.py
+-rw-rw-rw-   0        0        0      103 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/sublist.py
+-rw-rw-rw-   0        0        0     2085 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/txt2crop.py
+-rw-rw-rw-   0        0        0      151 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/unanimous.py
+-rw-rw-rw-   0        0        0      323 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/verticalpaste.py
+-rw-rw-rw-   0        0        0      296 2023-02-01 02:33:29.000000 doubleagent-1.63/doubleagent/whiterbg.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:00:52.909813 doubleagent-1.63/doubleagent.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-04-11 07:00:52.000000 doubleagent-1.63/doubleagent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-04-11 07:00:52.000000 doubleagent-1.63/doubleagent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:00:52.000000 doubleagent-1.63/doubleagent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 07:00:52.000000 doubleagent-1.63/doubleagent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:00:52.911814 doubleagent-1.63/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-04-11 06:45:17.000000 doubleagent-1.63/setup.py
```

### Comparing `doubleagent-1.62/doubleagent/__init__.py` & `doubleagent-1.63/doubleagent/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 from .picklemaker import picklemaker
 from .picklereader import picklereader
 from .rectangularcroplocation import rectangularcroplocation
 from .whiterbg import whiterbg
 from .alldel import alldel
 from .sublist import sublist
 from .errorboy import errorboy
-from .readfile import readfile
+from .readfile import readfile
+from .pinset import pinset
```

### Comparing `doubleagent-1.62/doubleagent/multiplesplit.py` & `doubleagent-1.63/doubleagent/multiplesplit.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent/rectangularcroplocation.py` & `doubleagent-1.63/doubleagent/rectangularcroplocation.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent/removeAlpha.py` & `doubleagent-1.63/doubleagent/removeAlpha.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent/rightreplace.py` & `doubleagent-1.63/doubleagent/rightreplace.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent/roundimage.py` & `doubleagent-1.63/doubleagent/roundimage.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent/seleupdate.py` & `doubleagent-1.63/doubleagent/seleupdate.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent/speedcases.py` & `doubleagent-1.63/doubleagent/speedcases.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent/txt2crop.py` & `doubleagent-1.63/doubleagent/txt2crop.py`

 * *Files identical despite different names*

### Comparing `doubleagent-1.62/doubleagent.egg-info/SOURCES.txt` & `doubleagent-1.63/doubleagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

