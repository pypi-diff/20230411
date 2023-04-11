# Comparing `tmp/hdr-plot-0.6.1.tar.gz` & `tmp/hdr-plot-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdr-plot-0.6.1.tar", last modified: Mon Apr 10 09:35:33 2023, max compression
+gzip compressed data, was "hdr-plot-0.6.2.tar", last modified: Tue Apr 11 12:36:50 2023, max compression
```

## Comparing `hdr-plot-0.6.1.tar` & `hdr-plot-0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.425914 hdr-plot-0.6.1/
--rw-r--r--   0 bruno      (501) staff       (20)    11357 2018-05-07 20:20:13.000000 hdr-plot-0.6.1/LICENSE
--rw-r--r--   0 bruno      (501) staff       (20)     2888 2023-04-10 09:35:33.425748 hdr-plot-0.6.1/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)     2418 2023-03-24 13:56:46.000000 hdr-plot-0.6.1/README.md
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.424679 hdr-plot-0.6.1/bin/
--rwxr-xr-x   0 bruno      (501) staff       (20)      594 2023-03-24 15:45:01.000000 hdr-plot-0.6.1/bin/hdr-plot
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.424931 hdr-plot-0.6.1/hdr_plot/
--rw-r--r--   0 bruno      (501) staff       (20)       18 2018-06-26 23:05:06.000000 hdr-plot-0.6.1/hdr_plot/__init__.py
--rwxr-xr-x   0 bruno      (501) staff       (20)     8885 2023-04-10 09:33:12.000000 hdr-plot-0.6.1/hdr_plot/hdr_plot.py
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-10 09:35:33.425549 hdr-plot-0.6.1/hdr_plot.egg-info/
--rw-r--r--   0 bruno      (501) staff       (20)     2888 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)      240 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (501) staff       (20)        1 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (501) staff       (20)       18 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/requires.txt
--rw-r--r--   0 bruno      (501) staff       (20)        9 2023-04-10 09:35:33.000000 hdr-plot-0.6.1/hdr_plot.egg-info/top_level.txt
--rw-r--r--   0 bruno      (501) staff       (20)       38 2023-04-10 09:35:33.425964 hdr-plot-0.6.1/setup.cfg
--rw-r--r--   0 bruno      (501) staff       (20)      742 2023-04-10 09:33:39.000000 hdr-plot-0.6.1/setup.py
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-11 12:36:50.373711 hdr-plot-0.6.2/
+-rw-r--r--   0 bruno      (501) staff       (20)    11357 2018-05-07 20:20:13.000000 hdr-plot-0.6.2/LICENSE
+-rw-r--r--   0 bruno      (501) staff       (20)     2889 2023-04-11 12:36:50.373561 hdr-plot-0.6.2/PKG-INFO
+-rw-r--r--   0 bruno      (501) staff       (20)     2419 2023-04-10 09:41:23.000000 hdr-plot-0.6.2/README.md
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-11 12:36:50.372544 hdr-plot-0.6.2/bin/
+-rwxr-xr-x   0 bruno      (501) staff       (20)      594 2023-03-24 15:45:01.000000 hdr-plot-0.6.2/bin/hdr-plot
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-11 12:36:50.372794 hdr-plot-0.6.2/hdr_plot/
+-rw-r--r--   0 bruno      (501) staff       (20)       18 2018-06-26 23:05:06.000000 hdr-plot-0.6.2/hdr_plot/__init__.py
+-rwxr-xr-x   0 bruno      (501) staff       (20)     8885 2023-04-11 12:35:45.000000 hdr-plot-0.6.2/hdr_plot/hdr_plot.py
+drwxr-xr-x   0 bruno      (501) staff       (20)        0 2023-04-11 12:36:50.373392 hdr-plot-0.6.2/hdr_plot.egg-info/
+-rw-r--r--   0 bruno      (501) staff       (20)     2889 2023-04-11 12:36:50.000000 hdr-plot-0.6.2/hdr_plot.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (501) staff       (20)      240 2023-04-11 12:36:50.000000 hdr-plot-0.6.2/hdr_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (501) staff       (20)        1 2023-04-11 12:36:50.000000 hdr-plot-0.6.2/hdr_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (501) staff       (20)       18 2023-04-11 12:36:50.000000 hdr-plot-0.6.2/hdr_plot.egg-info/requires.txt
+-rw-r--r--   0 bruno      (501) staff       (20)        9 2023-04-11 12:36:50.000000 hdr-plot-0.6.2/hdr_plot.egg-info/top_level.txt
+-rw-r--r--   0 bruno      (501) staff       (20)       38 2023-04-11 12:36:50.373757 hdr-plot-0.6.2/setup.cfg
+-rw-r--r--   0 bruno      (501) staff       (20)      742 2023-04-11 12:36:05.000000 hdr-plot-0.6.2/setup.py
```

### Comparing `hdr-plot-0.6.1/LICENSE` & `hdr-plot-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdr-plot-0.6.1/PKG-INFO` & `hdr-plot-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdr-plot
-Version: 0.6.1
+Version: 0.6.2
 Summary: A simple HdrHistogram plotting script.
 Home-page: https://github.com/BrunoBonacci/hdr-plot
 Author: Bruno Bonacci
 Author-email: bonacci.bruno@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -74,14 +74,14 @@
 
     hdr-plot --output myplot.png --title "My plot" ./sample/file1.out ./sample/file2.out ./sample/file3.out
 
 Please note that the name of the file is used as label for the plot legend.
 
 ## Acknowledgements
 
-A special thank to [@Manuelbernhardt](https://github.com/manuelbernhardt)for providing PRs for a lot of improvements!
+A special thank to [@Manuelbernhardt](https://github.com/manuelbernhardt) for providing PRs for a lot of improvements!
 
 ## License
 
 Copyright © 2018-2023 Bruno Bonacci - Distributed under the [Apache License v 2.0](http://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `hdr-plot-0.6.1/README.md` & `hdr-plot-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,12 +59,12 @@
 
     hdr-plot --output myplot.png --title "My plot" ./sample/file1.out ./sample/file2.out ./sample/file3.out
 
 Please note that the name of the file is used as label for the plot legend.
 
 ## Acknowledgements
 
-A special thank to [@Manuelbernhardt](https://github.com/manuelbernhardt)for providing PRs for a lot of improvements!
+A special thank to [@Manuelbernhardt](https://github.com/manuelbernhardt) for providing PRs for a lot of improvements!
 
 ## License
 
 Copyright © 2018-2023 Bruno Bonacci - Distributed under the [Apache License v 2.0](http://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `hdr-plot-0.6.1/bin/hdr-plot` & `hdr-plot-0.6.2/bin/hdr-plot`

 * *Files identical despite different names*

### Comparing `hdr-plot-0.6.1/hdr_plot/hdr_plot.py` & `hdr-plot-0.6.2/hdr_plot/hdr_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     max = data['Latency'].max()
 
     def get_percentile_latency(percentile):
         df = (data.loc[data['Percentile'] >= percentile]['Latency'])
         if not df.empty:
             return df.iloc[0]
         else:
-            return 0.0
+            return max
 
     percentiles = {
         'p50': 0.50,
         'p90': 0.90,
         'p99': 0.99,
         'p999': 0.999,
         'p9999': 0.9999,
```

### Comparing `hdr-plot-0.6.1/hdr_plot.egg-info/PKG-INFO` & `hdr-plot-0.6.2/hdr_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdr-plot
-Version: 0.6.1
+Version: 0.6.2
 Summary: A simple HdrHistogram plotting script.
 Home-page: https://github.com/BrunoBonacci/hdr-plot
 Author: Bruno Bonacci
 Author-email: bonacci.bruno@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -74,14 +74,14 @@
 
     hdr-plot --output myplot.png --title "My plot" ./sample/file1.out ./sample/file2.out ./sample/file3.out
 
 Please note that the name of the file is used as label for the plot legend.
 
 ## Acknowledgements
 
-A special thank to [@Manuelbernhardt](https://github.com/manuelbernhardt)for providing PRs for a lot of improvements!
+A special thank to [@Manuelbernhardt](https://github.com/manuelbernhardt) for providing PRs for a lot of improvements!
 
 ## License
 
 Copyright © 2018-2023 Bruno Bonacci - Distributed under the [Apache License v 2.0](http://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `hdr-plot-0.6.1/setup.py` & `hdr-plot-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hdr-plot",
-    version="0.6.1",
+    version="0.6.2",
     author="Bruno Bonacci",
     author_email="bonacci.bruno@gmail.com",
     description="A simple HdrHistogram plotting script.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BrunoBonacci/hdr-plot",
     packages=setuptools.find_packages(),
```

