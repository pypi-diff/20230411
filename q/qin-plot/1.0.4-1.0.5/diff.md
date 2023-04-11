# Comparing `tmp/qin_plot-1.0.4.tar.gz` & `tmp/qin_plot-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qin_plot-1.0.4.tar", last modified: Tue Apr 11 12:07:11 2023, max compression
+gzip compressed data, was "qin_plot-1.0.5.tar", last modified: Tue Apr 11 12:12:38 2023, max compression
```

## Comparing `qin_plot-1.0.4.tar` & `qin_plot-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:07:10.999671 qin_plot-1.0.4/
--rw-rw-rw-   0        0        0     1069 2022-08-21 09:38:01.000000 qin_plot-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       34 2022-08-21 09:44:51.000000 qin_plot-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      709 2023-04-11 12:07:10.997676 qin_plot-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      450 2022-10-02 05:44:48.000000 qin_plot-1.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 12:07:10.996676 qin_plot-1.0.4/qin_plot.egg-info/
--rw-rw-rw-   0        0        0      709 2023-04-11 12:07:10.000000 qin_plot-1.0.4/qin_plot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-11 12:07:10.000000 qin_plot-1.0.4/qin_plot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:07:10.000000 qin_plot-1.0.4/qin_plot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 12:07:10.000000 qin_plot-1.0.4/qin_plot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       63 2023-04-11 12:07:10.000000 qin_plot-1.0.4/qin_plot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 12:07:10.999671 qin_plot-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-04-11 12:06:57.000000 qin_plot-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:12:38.051790 qin_plot-1.0.5/
+-rw-rw-rw-   0        0        0     1069 2022-08-21 09:38:01.000000 qin_plot-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-08-21 09:44:51.000000 qin_plot-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      709 2023-04-11 12:12:38.050764 qin_plot-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2022-10-02 05:44:48.000000 qin_plot-1.0.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 12:12:38.045777 qin_plot-1.0.5/qin_plot/
+-rw-rw-rw-   0        0        0        0 2022-08-18 06:49:30.000000 qin_plot-1.0.5/qin_plot/__init__.py
+-rw-rw-rw-   0        0        0     8753 2020-04-22 21:05:22.000000 qin_plot-1.0.5/qin_plot/composition.py
+-rw-rw-rw-   0        0        0    14099 2023-04-11 09:26:44.000000 qin_plot-1.0.5/qin_plot/figures.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:12:38.049768 qin_plot-1.0.5/qin_plot.egg-info/
+-rw-rw-rw-   0        0        0      709 2023-04-11 12:12:38.000000 qin_plot-1.0.5/qin_plot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-11 12:12:38.000000 qin_plot-1.0.5/qin_plot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 12:12:38.000000 qin_plot-1.0.5/qin_plot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 12:12:38.000000 qin_plot-1.0.5/qin_plot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 12:12:38.000000 qin_plot-1.0.5/qin_plot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 12:12:38.051790 qin_plot-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-04-11 12:12:27.000000 qin_plot-1.0.5/setup.py
```

### Comparing `qin_plot-1.0.4/LICENSE` & `qin_plot-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qin_plot-1.0.4/PKG-INFO` & `qin_plot-1.0.5/qin_plot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qin_plot
-Version: 1.0.4
+Name: qin-plot
+Version: 1.0.5
 Summary: plot_ML
 Home-page: https://pymatsci.readthedocs.io/en/latest/
 Author: C.L. Qin
 Author-email: clqin@foxmail.com
 License: MIT License (MIT)
 Requires-Python: >=3
 License-File: LICENSE
```

### Comparing `qin_plot-1.0.4/qin_plot.egg-info/PKG-INFO` & `qin_plot-1.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qin-plot
-Version: 1.0.4
+Name: qin_plot
+Version: 1.0.5
 Summary: plot_ML
 Home-page: https://pymatsci.readthedocs.io/en/latest/
 Author: C.L. Qin
 Author-email: clqin@foxmail.com
 License: MIT License (MIT)
 Requires-Python: >=3
 License-File: LICENSE
```

