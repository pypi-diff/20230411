# Comparing `tmp/qin_plot-1.0.2.tar.gz` & `tmp/qin_plot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qin_plot-1.0.2.tar", last modified: Tue Apr 11 09:40:19 2023, max compression
+gzip compressed data, was "qin_plot-1.0.3.tar", last modified: Tue Apr 11 09:55:02 2023, max compression
```

## Comparing `qin_plot-1.0.2.tar` & `qin_plot-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:19.315094 qin_plot-1.0.2/
--rw-rw-rw-   0        0        0     1069 2022-08-21 09:38:01.000000 qin_plot-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2022-08-21 09:44:51.000000 qin_plot-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      709 2023-04-11 09:40:19.315094 qin_plot-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      450 2022-10-02 05:44:48.000000 qin_plot-1.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:19.314094 qin_plot-1.0.2/qin_plot.egg-info/
--rw-rw-rw-   0        0        0      709 2023-04-11 09:40:19.000000 qin_plot-1.0.2/qin_plot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-11 09:40:19.000000 qin_plot-1.0.2/qin_plot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:40:19.000000 qin_plot-1.0.2/qin_plot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 09:40:19.000000 qin_plot-1.0.2/qin_plot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:40:19.000000 qin_plot-1.0.2/qin_plot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 09:40:19.315094 qin_plot-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-04-11 09:40:04.000000 qin_plot-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:55:02.621968 qin_plot-1.0.3/
+-rw-rw-rw-   0        0        0     1069 2022-08-21 09:38:01.000000 qin_plot-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-08-21 09:44:51.000000 qin_plot-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      709 2023-04-11 09:55:02.621968 qin_plot-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2022-10-02 05:44:48.000000 qin_plot-1.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 09:55:02.619965 qin_plot-1.0.3/qin_plot.egg-info/
+-rw-rw-rw-   0        0        0      709 2023-04-11 09:55:02.000000 qin_plot-1.0.3/qin_plot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-11 09:55:02.000000 qin_plot-1.0.3/qin_plot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:55:02.000000 qin_plot-1.0.3/qin_plot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 09:55:02.000000 qin_plot-1.0.3/qin_plot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:55:02.000000 qin_plot-1.0.3/qin_plot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:55:02.621968 qin_plot-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-04-11 09:54:11.000000 qin_plot-1.0.3/setup.py
```

### Comparing `qin_plot-1.0.2/LICENSE` & `qin_plot-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qin_plot-1.0.2/PKG-INFO` & `qin_plot-1.0.3/qin_plot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qin_plot
-Version: 1.0.2
+Name: qin-plot
+Version: 1.0.3
 Summary: plot_ML
 Home-page: https://pymatsci.readthedocs.io/en/latest/
 Author: C.L. Qin
 Author-email: clqin@foxmail.com
 License: MIT License (MIT)
 Requires-Python: >=3
 License-File: LICENSE
```

### Comparing `qin_plot-1.0.2/qin_plot.egg-info/PKG-INFO` & `qin_plot-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qin-plot
-Version: 1.0.2
+Name: qin_plot
+Version: 1.0.3
 Summary: plot_ML
 Home-page: https://pymatsci.readthedocs.io/en/latest/
 Author: C.L. Qin
 Author-email: clqin@foxmail.com
 License: MIT License (MIT)
 Requires-Python: >=3
 License-File: LICENSE
```

