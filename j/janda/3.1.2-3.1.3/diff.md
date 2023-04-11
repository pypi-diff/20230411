# Comparing `tmp/janda-3.1.2.tar.gz` & `tmp/janda-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janda-3.1.2.tar", last modified: Sun Feb 12 00:08:34 2023, max compression
+gzip compressed data, was "janda-3.1.3.tar", last modified: Tue Apr 11 15:49:47 2023, max compression
```

## Comparing `janda-3.1.2.tar` & `janda-3.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 00:08:34.639527 janda-3.1.2/
--rw-rw-rw-   0        0        0     1086 2023-02-12 00:03:41.000000 janda-3.1.2/LICENSE
--rw-rw-rw-   0        0        0       85 2023-02-12 00:03:41.000000 janda-3.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    24854 2023-02-12 00:08:34.637488 janda-3.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    23483 2023-02-12 00:03:41.000000 janda-3.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-12 00:08:34.537505 janda-3.1.2/janda/
--rw-rw-rw-   0        0        0      335 2023-02-12 00:06:44.000000 janda-3.1.2/janda/__init__.py
--rw-rw-rw-   0        0        0     2225 2023-02-12 00:03:41.000000 janda-3.1.2/janda/asmhentai.py
--rw-rw-rw-   0        0        0     1760 2023-02-12 00:03:41.000000 janda-3.1.2/janda/hentai2read.py
--rw-rw-rw-   0        0        0     2425 2023-02-12 00:03:41.000000 janda-3.1.2/janda/hentaifox.py
--rw-rw-rw-   0        0        0     2718 2023-02-12 00:03:41.000000 janda-3.1.2/janda/nhentai.py
--rw-rw-rw-   0        0        0     2886 2023-02-12 00:03:41.000000 janda-3.1.2/janda/pururin.py
--rw-rw-rw-   0        0        0     1433 2023-02-12 00:03:41.000000 janda-3.1.2/janda/simply_hentai.py
--rw-rw-rw-   0        0        0     2594 2023-02-12 00:03:41.000000 janda-3.1.2/janda/thentai.py
-drwxrwxrwx   0        0        0        0 2023-02-12 00:08:34.586489 janda-3.1.2/janda/utils/
--rw-rw-rw-   0        0        0        0 2023-02-12 00:03:41.000000 janda-3.1.2/janda/utils/__init__.py
--rw-rw-rw-   0        0        0     3262 2023-02-12 00:03:41.000000 janda-3.1.2/janda/utils/client.py
--rw-rw-rw-   0        0        0      776 2023-02-12 00:03:41.000000 janda-3.1.2/janda/utils/request.py
-drwxrwxrwx   0        0        0        0 2023-02-12 00:08:34.581486 janda-3.1.2/janda.egg-info/
--rw-rw-rw-   0        0        0    24854 2023-02-12 00:08:34.000000 janda-3.1.2/janda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-02-12 00:08:34.000000 janda-3.1.2/janda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 00:08:34.000000 janda-3.1.2/janda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-02-12 00:08:34.000000 janda-3.1.2/janda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-12 00:08:34.000000 janda-3.1.2/janda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       14 2023-02-12 00:03:41.000000 janda-3.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-12 00:08:34.639527 janda-3.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2077 2023-02-12 00:06:25.000000 janda-3.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 00:08:34.635490 janda-3.1.2/test/
--rw-rw-rw-   0        0        0      698 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_api.py
--rw-rw-rw-   0        0        0      214 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_asmhentai.py
--rw-rw-rw-   0        0        0       40 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_build.py
--rw-rw-rw-   0        0        0      249 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_hentai2read.py
--rw-rw-rw-   0        0        0      225 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_hentaifox.py
--rw-rw-rw-   0        0        0      218 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_nhentai.py
--rw-rw-rw-   0        0        0      217 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_pururin.py
--rw-rw-rw-   0        0        0      237 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_simplyh.py
--rw-rw-rw-   0        0        0      218 2023-02-12 00:03:41.000000 janda-3.1.2/test/test_thentai.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:49:47.910861 janda-3.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-04-11 15:32:01.000000 janda-3.1.3/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-04-11 15:32:01.000000 janda-3.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    24854 2023-04-11 15:49:47.908866 janda-3.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    23483 2023-04-11 15:32:01.000000 janda-3.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 15:49:47.782867 janda-3.1.3/janda/
+-rw-rw-rw-   0        0        0      335 2023-04-11 15:40:10.000000 janda-3.1.3/janda/__init__.py
+-rw-rw-rw-   0        0        0     2225 2023-04-11 15:32:01.000000 janda-3.1.3/janda/asmhentai.py
+-rw-rw-rw-   0        0        0     1760 2023-04-11 15:32:01.000000 janda-3.1.3/janda/hentai2read.py
+-rw-rw-rw-   0        0        0     2425 2023-04-11 15:32:01.000000 janda-3.1.3/janda/hentaifox.py
+-rw-rw-rw-   0        0        0     2718 2023-04-11 15:32:01.000000 janda-3.1.3/janda/nhentai.py
+-rw-rw-rw-   0        0        0     2886 2023-04-11 15:32:01.000000 janda-3.1.3/janda/pururin.py
+-rw-rw-rw-   0        0        0     1433 2023-04-11 15:32:01.000000 janda-3.1.3/janda/simply_hentai.py
+-rw-rw-rw-   0        0        0     2594 2023-04-11 15:32:01.000000 janda-3.1.3/janda/thentai.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:49:47.884889 janda-3.1.3/janda/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 15:32:01.000000 janda-3.1.3/janda/utils/__init__.py
+-rw-rw-rw-   0        0        0     3267 2023-04-11 15:38:45.000000 janda-3.1.3/janda/utils/client.py
+-rw-rw-rw-   0        0        0      776 2023-04-11 15:32:01.000000 janda-3.1.3/janda/utils/request.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:49:47.875859 janda-3.1.3/janda.egg-info/
+-rw-rw-rw-   0        0        0    24854 2023-04-11 15:49:47.000000 janda-3.1.3/janda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-11 15:49:47.000000 janda-3.1.3/janda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:49:47.000000 janda-3.1.3/janda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 15:49:47.000000 janda-3.1.3/janda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 15:49:47.000000 janda-3.1.3/janda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 15:32:58.000000 janda-3.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:49:47.911937 janda-3.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2077 2023-04-11 15:32:01.000000 janda-3.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:49:47.905861 janda-3.1.3/test/
+-rw-rw-rw-   0        0        0      698 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_api.py
+-rw-rw-rw-   0        0        0      214 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_asmhentai.py
+-rw-rw-rw-   0        0        0       40 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_build.py
+-rw-rw-rw-   0        0        0      249 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_hentai2read.py
+-rw-rw-rw-   0        0        0      225 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_hentaifox.py
+-rw-rw-rw-   0        0        0      218 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_nhentai.py
+-rw-rw-rw-   0        0        0      217 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_pururin.py
+-rw-rw-rw-   0        0        0      237 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_simplyh.py
+-rw-rw-rw-   0        0        0      218 2023-04-11 15:32:01.000000 janda-3.1.3/test/test_thentai.py
```

### Comparing `janda-3.1.2/LICENSE` & `janda-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/PKG-INFO` & `janda-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janda
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python library for Jandapress, doujinshi api
 Home-page: https://github.com/sinkaroid/janda
 Author: sinkaroid
 Author-email: anakmancasan@gmail.com
 License: MIT
 Project-URL: Documentation, https://sinkaroid.github.io/janda
 Project-URL: Issue tracker, https://github.com/sinkaroid/janda/issues/new/choose
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: janda Version: 3.1.2 Summary: Python library for
+Metadata-Version: 2.1 Name: janda Version: 3.1.3 Summary: Python library for
 Jandapress, doujinshi api Home-page: https://github.com/sinkaroid/janda Author:
 sinkaroid Author-email: anakmancasan@gmail.com License: MIT Project-URL:
 Documentation, https://sinkaroid.github.io/janda Project-URL: Issue tracker,
 https://github.com/sinkaroid/janda/issues/new/choose Project-URL: Funding,
 https://github.com/sponsors/sinkaroid Project-URL: Discord, https://discord.gg/
 8wj4vM5hHM Keywords:
 doujinshi,library,hentai,api,nhentai,pururin,hentaifox,hentai2read,simply-
```

### Comparing `janda-3.1.2/README.md` & `janda-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/asmhentai.py` & `janda-3.1.3/janda/asmhentai.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/hentai2read.py` & `janda-3.1.3/janda/hentai2read.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/hentaifox.py` & `janda-3.1.3/janda/hentaifox.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/nhentai.py` & `janda-3.1.3/janda/nhentai.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/pururin.py` & `janda-3.1.3/janda/pururin.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/simply_hentai.py` & `janda-3.1.3/janda/simply_hentai.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/thentai.py` & `janda-3.1.3/janda/thentai.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda/utils/client.py` & `janda-3.1.3/janda/utils/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from janda import __version__
 
-JANDA = "https://janda.mod.land"
+JANDA = "https://janda.sinkaroid.org"
 
 
 class Api:
     """Api class
 
     This class is used to parse the data from the api.
```

### Comparing `janda-3.1.2/janda/utils/request.py` & `janda-3.1.3/janda/utils/request.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/janda.egg-info/PKG-INFO` & `janda-3.1.3/janda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janda
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python library for Jandapress, doujinshi api
 Home-page: https://github.com/sinkaroid/janda
 Author: sinkaroid
 Author-email: anakmancasan@gmail.com
 License: MIT
 Project-URL: Documentation, https://sinkaroid.github.io/janda
 Project-URL: Issue tracker, https://github.com/sinkaroid/janda/issues/new/choose
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: janda Version: 3.1.2 Summary: Python library for
+Metadata-Version: 2.1 Name: janda Version: 3.1.3 Summary: Python library for
 Jandapress, doujinshi api Home-page: https://github.com/sinkaroid/janda Author:
 sinkaroid Author-email: anakmancasan@gmail.com License: MIT Project-URL:
 Documentation, https://sinkaroid.github.io/janda Project-URL: Issue tracker,
 https://github.com/sinkaroid/janda/issues/new/choose Project-URL: Funding,
 https://github.com/sponsors/sinkaroid Project-URL: Discord, https://discord.gg/
 8wj4vM5hHM Keywords:
 doujinshi,library,hentai,api,nhentai,pururin,hentaifox,hentai2read,simply-
```

### Comparing `janda-3.1.2/janda.egg-info/SOURCES.txt` & `janda-3.1.3/janda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/setup.py` & `janda-3.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `janda-3.1.2/test/test_api.py` & `janda-3.1.3/test/test_api.py`

 * *Files identical despite different names*

