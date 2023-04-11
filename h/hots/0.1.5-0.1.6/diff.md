# Comparing `tmp/hots-0.1.5.tar.gz` & `tmp/hots-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hots-0.1.5.tar", last modified: Thu Mar  9 16:27:42 2023, max compression
+gzip compressed data, was "hots-0.1.6.tar", last modified: Tue Apr 11 10:28:45 2023, max compression
```

## Comparing `hots-0.1.5.tar` & `hots-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:27:42.083215 hots-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-09 16:27:32.000000 hots-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-03-09 16:27:42.083215 hots-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-03-09 16:27:32.000000 hots-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-09 16:27:32.000000 hots-0.1.5/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-09 16:27:32.000000 hots-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 16:27:42.083215 hots-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-09 16:27:32.000000 hots-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:27:42.075215 hots-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:27:42.079215 hots-0.1.5/src/hots/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19578 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    50631 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/placement.py
--rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-09 16:27:32.000000 hots-0.1.5/src/hots/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:27:42.083215 hots-0.1.5/src/hots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-03-09 16:27:42.000000 hots-0.1.5/src/hots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-09 16:27:42.000000 hots-0.1.5/src/hots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:27:42.000000 hots-0.1.5/src/hots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-09 16:27:42.000000 hots-0.1.5/src/hots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:27:41.000000 hots-0.1.5/src/hots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-09 16:27:42.000000 hots-0.1.5/src/hots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-09 16:27:42.000000 hots-0.1.5/src/hots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:27:42.083215 hots-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-09 16:27:32.000000 hots-0.1.5/tests/test_packaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.111452 hots-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 10:28:28.000000 hots-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-11 10:28:45.111452 hots-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-11 10:28:28.000000 hots-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 10:28:28.000000 hots-0.1.6/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-11 10:28:28.000000 hots-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:28:45.111452 hots-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 10:28:28.000000 hots-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/src/hots/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19578 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56171 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/placement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-11 10:28:28.000000 hots-0.1.6/src/hots/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/src/hots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:28:44.000000 hots-0.1.6/src/hots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 10:28:45.000000 hots-0.1.6/src/hots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:45.107452 hots-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 10:28:28.000000 hots-0.1.6/tests/test_packaging.py
```

### Comparing `hots-0.1.5/LICENSE.txt` & `hots-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/PKG-INFO` & `hots-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hots
-Version: 0.1.5
+Version: 0.1.6
 Summary: Resource Allocation via Clustering
 Author-email: Smile R&D team <rnd@smile.fr>
 License: MIT
 Project-URL: Homepage, https://github.com/Smile-SA/hots
 Project-URL: Documentation, https://hots.readthedocs.io/en/latest/
 Keywords: Resource,Optimisation,Clustering,Planning
 Platform: any
@@ -20,17 +20,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-# **HOTS**
+<h1 align="center">
+<img src="doc/source/_static/hots_logo.png" width="250">
+</h1><br>
 
-> Hybrid Optimization for Time Series  
+> Hybrid Optimization for Time Series (HOTS)  
 > HOTS solves problems presented as time series using machine learning and optimization methods.  
 > The library supports multiple resource related problems (placement, allocation), presented as one or more metrics.
 
 ## Requirements for running HOTS
 
 HOTS works on any platform with Python 3.8 and up.
 
@@ -111,14 +113,16 @@
 - Marco Mariani
 - Gilles Lenfant
 - Soobash Daiboo
 - Kang Du
 - Amaury Sauret
 - SMILE R&D
 
+As HOTS was created during a PhD, credits have to be given to academic supervisors, Céline Rouveirol and Frédéric Roupin, involved in the algorithm thinking.
+
 ## Links
 
 - [Project home](https://github.com/Smile-SA/hots)
 - [File issues (bugs, ...)](https://github.com/Smile-SA/hots/issues)
 - [PyPi package](https://pypi.org/project/hots/)
 - [Documentation](https://hots.readthedocs.io/en/latest/)
 - [PhD document](https://theses.hal.science/tel-03997934)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hots-0.1.5/README.md` & `hots-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# **HOTS**
+<h1 align="center">
+<img src="doc/source/_static/hots_logo.png" width="250">
+</h1><br>
 
-> Hybrid Optimization for Time Series  
+> Hybrid Optimization for Time Series (HOTS)  
 > HOTS solves problems presented as time series using machine learning and optimization methods.  
 > The library supports multiple resource related problems (placement, allocation), presented as one or more metrics.
 
 ## Requirements for running HOTS
 
 HOTS works on any platform with Python 3.8 and up.
 
@@ -85,14 +87,16 @@
 - Marco Mariani
 - Gilles Lenfant
 - Soobash Daiboo
 - Kang Du
 - Amaury Sauret
 - SMILE R&D
 
+As HOTS was created during a PhD, credits have to be given to academic supervisors, Céline Rouveirol and Frédéric Roupin, involved in the algorithm thinking.
+
 ## Links
 
 - [Project home](https://github.com/Smile-SA/hots)
 - [File issues (bugs, ...)](https://github.com/Smile-SA/hots/issues)
 - [PyPi package](https://pypi.org/project/hots/)
 - [Documentation](https://hots.readthedocs.io/en/latest/)
 - [PhD document](https://theses.hal.science/tel-03997934)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hots-0.1.5/pyproject.toml` & `hots-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 dependencies = [
     "click",
     "clusopt_core",
     "matplotlib",
     "networkx",
     "numpy",
     "pandas",
-    "plotly",
     "pyomo",
     "scikit-learn",
     "scipy",
     "tqdm",
 ]
 dynamic = [
     "version",
```

### Comparing `hots-0.1.5/src/hots/__init__.py` & `hots-0.1.6/src/hots/__init__.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/allocation.py` & `hots-0.1.6/src/hots/allocation.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/clustering.py` & `hots-0.1.6/src/hots/clustering.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/container.py` & `hots-0.1.6/src/hots/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from matplotlib import gridspec as gridspec
 from matplotlib import pyplot as plt
 
 import numpy as np
 
 import pandas as pd
 
-import plotly.express as px
-
 from . import init as it
 from . import plot
 
 # Definition of Container-related functions #
 
 
 def plot_data_all_containers(df_indiv, metric):
@@ -33,34 +31,35 @@
     pvt = pd.pivot_table(temp_df, columns=it.indiv_field,
                          index=it.tick_field, aggfunc='sum', values=metric)
     pvt.plot(ax=ax)
     fig.suptitle('%s use on all containers' % metric)
     plt.draw()
 
 
-def plot_all_data_all_containers_px(df_indiv, sep_time, metrics=None):
-    """Plot all metrics containers consumption.
-
-    :param df_indiv: _description_
-    :type df_indiv: pd.DataFrame
-    :param sep_time: _description_
-    :type sep_time: int
-    :param metrics: _description_, defaults to None
-    :type metrics: List[str], optional
-    """
-    # TODO several metrics ?
-    # TODO line_shape in params
-    metrics = metrics or it.metrics
-    fig = px.line(df_indiv, x=it.tick_field, y=metrics[0],
-                  color=it.host_field,
-                  line_group=it.indiv_field, hover_name=it.indiv_field,
-                  line_shape='spline', render_mode='svg',
-                  title='Resource usage on all individuals')
-    fig.add_vline(sep_time, line={'color': 'red', 'dash': 'dashdot'})
-    fig.show(it.renderer)
+# The following uses plotly : comment for the moment
+# def plot_all_data_all_containers_px(df_indiv, sep_time, metrics=None):
+#     """Plot all metrics containers consumption.
+
+#     :param df_indiv: _description_
+#     :type df_indiv: pd.DataFrame
+#     :param sep_time: _description_
+#     :type sep_time: int
+#     :param metrics: _description_, defaults to None
+#     :type metrics: List[str], optional
+#     """
+#     # TODO several metrics ?
+#     # TODO line_shape in params
+#     metrics = metrics or it.metrics
+#     fig = px.line(df_indiv, x=it.tick_field, y=metrics[0],
+#                   color=it.host_field,
+#                   line_group=it.indiv_field, hover_name=it.indiv_field,
+#                   line_shape='spline', render_mode='svg',
+#                   title='Resource usage on all individuals')
+#     fig.add_vline(sep_time, line={'color': 'red', 'dash': 'dashdot'})
+#     fig.show(it.renderer)
 
 
 def plot_all_data_all_containers(df_indiv, sep_time, metrics=None):
     """Plot all metrics containers consumption.
 
     :param df_indiv: _description_
     :type df_indiv: pd.DataFrame
```

### Comparing `hots-0.1.5/src/hots/init.py` & `hots-0.1.6/src/hots/init.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/instance.py` & `hots-0.1.6/src/hots/instance.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/main.py` & `hots-0.1.6/src/hots/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,38 +44,38 @@
 @click.option('-m', '--method', required=False, type=str, default='loop', help='Method used')
 @click.option('-c', '--cluster_method', required=False, type=str, default='loop-cluster',
               help='Method used for updating clustering')
 @click.option('-p', '--param', required=False, type=str, help='Use a specific parameter file')
 @click.option('-o', '--output', required=False, type=str,
               help='Use a specific directory for output')
 @click.option('-ec', '--tolclust', required=False, type=str,
-              help='Use specific value for epsilonC')
+              help='Use specific value for epsilonC (clustering conflict threshold)')
 @click.option('-ea', '--tolplace', required=False, type=str,
-              help='Use specific value for epsilonA')
+              help='Use specific value for epsilonA (placement conflict threshold)')
 def main(path, k, tau, method, cluster_method, param, output, tolclust, tolplace):
     """Use method to propose a placement solution for micro-services adjusted in time.
 
-    :param path: _description_
-    :type path: _type_
-    :param k: _description_
-    :type k: _type_
-    :param tau: _description_
-    :type tau: _type_
-    :param method: _description_
-    :type method: _type_
-    :param cluster_method: _description_
-    :type cluster_method: _type_
-    :param param: _description_
-    :type param: _type_
-    :param output: _description_
-    :type output: _type_
-    :param tolclust: _description_
-    :type tolclust: _type_
-    :param tolplace: _description_
-    :type tolplace: _type_
+    :param path: path to folder with data and parameters file
+    :type path: click.Path
+    :param k: number of clusters to use for clustering
+    :type k: int
+    :param tau: time window size for the loop
+    :type tau: int
+    :param method: method to use to solve initial problem
+    :type method: str
+    :param cluster_method: method to use to update clustering
+    :type cluster_method: str
+    :param param: parameter file to use
+    :type param: str
+    :param output: output folder to use
+    :type output: str
+    :param tolclust: threshold to use for clustering conflict
+    :type tolclust: str
+    :param tolplace: threshold to use for placement conflict
+    :type tolplace: str
     """
     # Initialization part
     main_time = time.time()
 
     if not path[-1] == '/':
         path += '/'
 
@@ -190,33 +190,33 @@
 
 
 def preprocess(
     path, k, tau, method, cluster_method, param, output, tolclust, tolplace
 ):
     """Load configuration, data and initialize needed objects.
 
-    :param path: _description_
+    :param path: initial folder path
     :type path: str
-    :param k: _description_
+    :param k: number of clusters to use for clustering
     :type k: int
-    :param tau: _description_
+    :param tau: time window size for loop
     :type tau: int
-    :param method: _description_
+    :param method: method to use to solve initial problem
     :type method: str
-    :param cluster_method: _description_
+    :param cluster_method: method to use to update clustering
     :type cluster_method: str
-    :param param: _description_
+    :param param: parameter file to use
     :type param: str
-    :param output: _description_
+    :param output: output folder to use
     :type output: str
-    :param tolclust: _description_
+    :param tolclust: threshold to use for clustering conflict
     :type tolclust: float
-    :param tolplace: _description_
+    :param tolplace: threshold to use for placement conflict
     :type tolplace: float
-    :return: _description_
+    :return: tuple with needed parameters, path to output and Instance object
     :rtype: Tuple[Dict, str, Instance]
     """
     # TODO what if we want tick < tau ?
     print('Preprocessing ...')
     (config, output_path) = it.read_params(path, k, tau, method, cluster_method, param, output)
     config = spec_params(config, [tolclust, tolplace])
     logging.basicConfig(filename=output_path + '/logs.log', filemode='w',
@@ -232,38 +232,39 @@
     return (config, output_path, instance)
 
 
 # TODO use Dict instead of List for genericity ?
 def spec_params(config, list_params):
     """Define specific parameters.
 
-    :param config: _description_
+    :param config: initial parameters set
     :type config: Dict
-    :param list_params: _description_
+    :param list_params: parameters list for threshold
     :type list_params: List
-    :return: _description_
+    :return: final parameters set
     :rtype: Dict
     """
     if list_params[0] is not None:
         config['loop']['tol_dual_clust'] = float(list_params[0])
     if list_params[1] is not None:
         config['loop']['tol_dual_place'] = float(list_params[1])
     return config
 
 
 def analysis_period(my_instance, config, method):
     """Perform all needed process during analysis period (T_init).
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param config: _description_
+    :param config: parameters set
     :type config: Dict
-    :param method: _description_
+    :param method: method used to solve initial problem
     :type method: str
-    :return: _description_
+    :return: tuple with Instance object, nodes data with new placement, clustering data and
+    clustering labels
     :rtype: Tuple[Instance, pd.DataFrame, pd.DataFrame, List]
     """
     df_host_evo = pd.DataFrame(columns=my_instance.df_host.columns)
     df_indiv_clust = pd.DataFrame()
     labels_ = []
 
     if method == 'init':
@@ -357,31 +358,31 @@
 
 
 def run_period(
     my_instance, df_host_evo, df_indiv_clust, labels_, config, output_path, method, cluster_method
 ):
     """Perform all needed process during evaluation period.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param df_host_evo: _description_
+    :param df_host_evo: evolving node data
     :type df_host_evo: pd.DataFrame
-    :param df_indiv_clust: _description_
+    :param df_indiv_clust: clustering individuals data
     :type df_indiv_clust: pd.DataFrame
-    :param labels_: _description_
+    :param labels_: clustering labels
     :type labels_: List
-    :param config: _description_
+    :param config: set parameters
     :type config: Dict
-    :param output_path: _description_
+    :param output_path: output folder path
     :type output_path: str
-    :param method: _description_
+    :param method: method to use to solve problem
     :type method: str
-    :param cluster_method: _description_
+    :param cluster_method: method to use for clustering
     :type cluster_method: str
-    :return: _description_
+    :return: evolving node data and number of nodes overloads
     :rtype: Tuple[pd.DataFrame, int]
     """
     nb_overloads = 0
     # Loops for evaluation
     if method in ['loop']:
         # loop 'streaming' progress
         it.results_file.write('\n### Loop process ###\n')
@@ -428,45 +429,46 @@
 def streaming_eval(
     my_instance, df_indiv_clust, labels_, mode, tick, constraints_dual,
     tol_clust, tol_move_clust, tol_open_clust, tol_place, tol_move_place, tol_step,
     cluster_method, solver, df_host_evo
 ):
     """Define the streaming process for evaluation.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param df_indiv_clust: _description_
+    :param df_indiv_clust: clustering individual data
     :type df_indiv_clust: pd.DataFrame
-    :param labels_: _description_
+    :param labels_: clustering labels
     :type labels_: List
-    :param mode: _description_
+    :param mode: mode used to trigger the loop
     :type mode: str
-    :param tick: _description_
+    :param tick: number of new datapoints before new loop
     :type tick: int
-    :param constraints_dual: _description_
+    :param constraints_dual: constraints type compared to trigger conflicts
     :type constraints_dual: List
-    :param tol_clust: _description_
+    :param tol_clust: threshold used for clustering conflicts
     :type tol_clust: float
-    :param tol_move_clust: _description_
+    :param tol_move_clust: threshold used for number of clustering moves
     :type tol_move_clust: float
-    :param tol_open_clust: _description_
+    :param tol_open_clust: threshold used for opening new cluster
     :type tol_open_clust: float
-    :param tol_place: _description_
+    :param tol_place: threshold used for placement conflicts
     :type tol_place: float
-    :param tol_move_place: _description_
+    :param tol_move_place: threshold used for number of placement moves
     :type tol_move_place: float
-    :param tol_step: _description_
+    :param tol_step: step to increment previous threshold
     :type tol_step: float
-    :param cluster_method: _description_
+    :param cluster_method: method used to update clustering
     :type cluster_method: str
-    :param solver: _description_
+    :param solver: solver used for pyomo
     :type solver: str
-    :param df_host_evo: _description_
+    :param df_host_evo: evolving node data
     :type df_host_evo: pd.DataFrame
-    :return: _description_
+    :return: figures to plot to see clustering and nodes evolution + evolving node data + number
+    of node overloads
     :rtype: Tuple[plt.Figure, plt.Figure, plt.Figure, List, pd.DataFrame, int]
     """
     fig_node, ax_node = plot.init_nodes_plot(
         my_instance.df_indiv, my_instance.dict_id_n, my_instance.sep_time,
         my_instance.df_host_meta[it.metrics[0]].max()
     )
     fig_clust, ax_clust = plot.init_plot_clustering(
@@ -678,42 +680,43 @@
 def progress_time_noloop(
     instance, fixing, tmin, tmax, labels_, loop_nb,
     constraints_dual, clustering_dual_values, placement_dual_values,
     tol_clust, tol_move_clust, tol_place, tol_move_place
 ):
     """We progress in time without performing the loop, checking node capacities.
 
-    :param instance: _description_
+    :param instance: Instance object
     :type instance: Instance
-    :param fixing: _description_
+    :param fixing: method used to fix node assignment if overload
     :type fixing: str
-    :param tmin: _description_
+    :param tmin: starting time of current window
     :type tmin: int
-    :param tmax: _description_
+    :param tmax: final time of current window
     :type tmax: int
-    :param labels_: _description_
-    :type labels_: _type_
-    :param loop_nb: _description_
-    :type loop_nb: _type_
-    :param constraints_dual: _description_
-    :type constraints_dual: _type_
-    :param clustering_dual_values: _description_
-    :type clustering_dual_values: _type_
-    :param placement_dual_values: _description_
-    :type placement_dual_values: _type_
-    :param tol_clust: _description_
-    :type tol_clust: _type_
-    :param tol_move_clust: _description_
-    :type tol_move_clust: _type_
-    :param tol_place: _description_
-    :type tol_place: _type_
-    :param tol_move_place: _description_
-    :type tol_move_place: _type_
-    :return: _description_
-    :rtype: Tuple[pd.DataFrame, int]
+    :param labels_: clustering labels
+    :type labels_: List
+    :param loop_nb: current loop number
+    :type loop_nb: int
+    :param constraints_dual: constraints type compared to trigger conflicts
+    :type constraints_dual: List
+    :param clustering_dual_values: previous loop dual values for clustering
+    :type clustering_dual_values: Dict
+    :param placement_dual_values: previous loop dual values for placement
+    :type placement_dual_values: Dict
+    :param tol_clust: threshold used for clustering conflicts
+    :type tol_clust: float
+    :param tol_move_clust: threshold used for number of clustering moves
+    :type tol_move_clust: float
+    :param tol_place: threshold used for placement conflicts
+    :type tol_place: float
+    :param tol_move_place: threshold used for number of placement moves
+    :type tol_move_place: float
+    :return: evolving node data + number of overloads + loop number + clustering and placement
+    changes
+    :rtype: Tuple[pd.DataFrame, int, int, int, int]
     """
     df_host_evo = pd.DataFrame(columns=instance.df_host.columns)
     nb_overload = 0
     nb_clust_changes = 0
     nb_place_changes = 0
     for tick in range(tmin, tmax + 1):
         df_host_tick = instance.df_indiv.loc[
@@ -770,33 +773,33 @@
 
 
 def pre_loop(
     my_instance, working_df_indiv, df_clust, w, u, constraints_dual, v, cluster_method, solver
 ):
     """Build optimization problems and solve them with T_init solutions.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param working_df_indiv: _description_
+    :param working_df_indiv: current loop data
     :type working_df_indiv: pd.DataFrame
-    :param df_clust: _description_
+    :param df_clust: clustering related data
     :type df_clust: pd.DataFrame
-    :param w: _description_
+    :param w: dissimilarity matrix
     :type w: np.array
-    :param u: _description_
+    :param u: clustering adjacency matrix
     :type u: np.array
-    :param constraints_dual: _description_
+    :param constraints_dual: constraints type compared to trigger conflicts
     :type constraints_dual: List
-    :param v: _description_
+    :param v: placement adjacency matrix
     :type v: np.array
-    :param cluster_method: _description_
+    :param cluster_method: method used to update clustering
     :type cluster_method: str
-    :param solver: _description_
+    :param solver: solver used for pyomo
     :type solver: str
-    :return: _description_
+    :return: optimization models and associated dual values
     :rtype: Tuple[mdl.Model, mdl.Model, Dict, Dict]
     """
     logging.info('Evaluation of problems with initial solutions')
     print('Building clustering model ...')
     start = time.time()
     clust_model = mdl.Model(
         1,
@@ -861,23 +864,23 @@
     return (clust_model, place_model,
             clustering_dual_values, placement_dual_values)
 
 
 def build_matrices(my_instance, tmin, tmax, labels_):
     """Build period dataframe and matrices to be used.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param tmin: _description_
+    :param tmin: starting time of current window
     :type tmin: int
-    :param tmax: _description_
+    :param tmax: final time of current window
     :type tmax: int
-    :param labels_: _description_
+    :param labels_: clustering labels
     :type labels_: List
-    :return: _description_
+    :return: current loop data, clustering data, dissimilarity matrix and adjacency matrices
     :rtype: Tuple[pd.DataFrame, pd.DataFrame, np.array, np.array, np.array]
     """
     working_df_indiv = my_instance.df_indiv[
         (my_instance.
          df_indiv[it.tick_field] >= tmin) & (
             my_instance.df_indiv[it.tick_field] <= tmax)]
     (df_clust, my_instance.dict_id_c) = clt.build_matrix_indiv_attr(
@@ -894,15 +897,67 @@
 def eval_sols(
         my_instance, working_df_indiv,
         cluster_method, w, u, v, clust_model, place_model,
         constraints_dual, clustering_dual_values, placement_dual_values,
         tol_clust, tol_move_clust, tol_open_clust, tol_place, tol_move_place,
         df_clust, cluster_profiles, labels_, loop_nb, solver
 ):
-    """Evaluate clustering and placement solutions."""
+    """Evaluate clustering and placement solutions.
+
+    :param my_instance: Instance object
+    :type my_instance: Instance
+    :param working_df_indiv: current loop data
+    :type working_df_indiv: pd.DataFrame
+    :param cluster_method: method used to update clustering
+    :type cluster_method: str
+    :param w: dissimilarity matrix
+    :type w: np.array
+    :param u: clustering adjacency matrix
+    :type u: np.array
+    :param v: placement adjacency matrix
+    :type v: np.array
+    :param clust_model: clustering optimization model
+    :type clust_model: mdl.Model
+    :param place_model: placement optimization model
+    :type place_model: mdl.Model
+    :param constraints_dual: constraints type compared to trigger conflicts
+    :type constraints_dual: List
+    :param clustering_dual_values: previous loop dual values for clustering
+    :type clustering_dual_values: Dict
+    :param placement_dual_values: previous loop dual values for placement
+    :type placement_dual_values: Dict
+    :param tol_clust: threshold used for clustering conflicts
+    :type tol_clust: float
+    :param tol_move_clust: threshold used for number of clustering moves
+    :type tol_move_clust: float
+    :param tol_open_clust: threshold used for opening new cluster
+    :type tol_open_clust: float
+    :param tol_place: threshold used for placement conflicts
+    :type tol_place: float
+    :param tol_move_place: threshold used for number of placement moves
+    :type tol_move_place: float
+    :param df_clust: clustering related data
+    :type df_clust: pd.DataFrame
+    :param cluster_profiles: computed clusters mean profiles
+    :type cluster_profiles: np.array
+    :param labels_: cluster labels
+    :type labels_: List
+    :param loop_nb: current loop number
+    :type loop_nb: int
+    :param solver: solver used for pyomo
+    :type solver: str
+    :return: number of changes in clustering and placement, silhouette score before and after loop,
+    number of nodes and edges in conflict graph + max and mean degree (clustering and placement),
+    optimization models and associated dual values, clustering related data, clusters mean profiles
+    and cluster labels
+    :rtype: Tuple[
+        int, int, float, float, int, int, float, float, int, int, float, float,
+        mdl.Model, mdl.Model, Dict, Dict, pd.DataFrame, np.array, List
+    ]
+    """
     # evaluate clustering
     start = time.time()
     it.clustering_file.write(
         'labels before change\n'
     )
     it.clustering_file.write(
         np.array2string(labels_, separator=',')
@@ -975,44 +1030,48 @@
 def eval_clustering(
     my_instance, w, u, clust_model, clustering_dual_values, constraints_dual,
     tol_clust, tol_move_clust, tol_open_clust,
     df_clust, cluster_profiles, labels_, loop_nb, solver
 ):
     """Evaluate current clustering solution and update it if needed.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param w: _description_
+    :param w: dissimilarity matrix
     :type w: np.array
-    :param u: _description_
+    :param u: clustering adjacency matrix
     :type u: np.array
-    :param clust_model: _description_
-    :type clust_model: _type_
-    :param clustering_dual_values: _description_
+    :param clust_model: clustering optimization model
+    :type clust_model: mdl.Model
+    :param clustering_dual_values: previous loop dual values for clustering
     :type clustering_dual_values: Dict
-    :param constraints_dual: _description_
-    :type constraints_dual: Dict
-    :param tol_clust: _description_
+    :param constraints_dual: constraints type compared to trigger conflicts
+    :type constraints_dual: List
+    :param tol_clust: threshold used for clustering conflicts
     :type tol_clust: float
-    :param tol_move_clust: _description_
+    :param tol_move_clust: threshold used for number of clustering moves
     :type tol_move_clust: float
-    :param tol_open_clust: _description_
+    :param tol_open_clust: threshold used for opening new cluster
     :type tol_open_clust: float
-    :param df_clust: _description_
+    :param df_clust: clustering related data
     :type df_clust: pd.DataFrame
-    :param cluster_profiles: _description_
+    :param cluster_profiles: computed clusters mean profiles
     :type cluster_profiles: np.array
-    :param labels_: _description_
+    :param labels_: cluster labels
     :type labels_: List
-    :param loop_nb: _description_
-    :type loop_nb: _type_
-    :param solver: _description_
-    :type solver: _type_
-    :return: _description_
-    :rtype: Tuple
+    :param loop_nb: current loop number
+    :type loop_nb: int
+    :param solver: solver used for pyomo
+    :type solver: str
+    :return: clustering variance matrix, number of changes in clustering, silhouette score before
+    and after the loop, clustering dual values, clustering optimization model, number of nodes and
+    edges in conflict graph + max and mean degree (clustering)
+    :rtype: Tuple[
+        np.array, int, float, float, Dict, mdl.Model, int, int, float, float
+    ]
     """
     nb_clust_changes_loop = 0
     logging.info('# Clustering evaluation #')
 
     init_loop_silhouette = clt.get_silhouette(df_clust, labels_)
 
     start = time.time()
@@ -1079,44 +1138,45 @@
 def eval_placement(
     my_instance, working_df_indiv, w, u, v, dv,
     placement_dual_values, constraints_dual, place_model, tol_place, tol_move_place,
     nb_clust_changes_loop, loop_nb, solver
 ):
     """Evaluate current clustering solution and update it if needed.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param working_df_indiv: _description_
+    :param working_df_indiv: current loop data
     :type working_df_indiv: pd.DataFrame
-    :param w: _description_
+    :param w: dissimilarity matrix
     :type w: np.array
-    :param u: _description_
+    :param u: clustering adjacency matrix
     :type u: np.array
-    :param v: _description_
+    :param v: placement adjacency matrix
     :type v: np.array
-    :param dv: _description_
+    :param dv: clustering variance matrix
     :type dv: np.array
-    :param placement_dual_values: _description_
+    :param placement_dual_values: previous loop dual values for placement
     :type placement_dual_values: Dict
-    :param constraints_dual: _description_
-    :type constraints_dual: Dict
-    :param place_model: _description_
-    :type place_model: _type_
-    :param tol_place: _description_
+    :param constraints_dual: constraints type compared to trigger conflicts
+    :type constraints_dual: List
+    :param place_model: placement optimization model
+    :type place_model: mdl.Model
+    :param tol_place: threshold used for placement conflicts
     :type tol_place: float
-    :param tol_move_place: _description_
+    :param tol_move_place: threshold used for number of placement moves
     :type tol_move_place: float
-    :param nb_clust_changes_loop: _description_
+    :param nb_clust_changes_loop: number of changes in clustering in current loop
     :type nb_clust_changes_loop: int
-    :param loop_nb: _description_
-    :type loop_nb: _type_
-    :param solver: _description_
+    :param loop_nb: current loop number
+    :type loop_nb: int
+    :param solver: solver used for pyomo
     :type solver: str
-    :return: _description_
-    :rtype: Tuple
+    :return: number of placement changes, dual values related to current placement, placement
+    optimization model, number of nodes and edges in conflict graph + max and mean degree
+    :rtype: Tuple[int, Dict, mdl.Model, int, int, float, float]
     """
     logging.info('# Placement evaluation #')
 
     start = time.time()
     # TODO update without re-creating from scratch ? Study
     place_model = mdl.Model(
         2,
@@ -1173,22 +1233,25 @@
             place_conf_nodes, place_conf_edges,
             place_max_deg, place_mean_deg)
 
 
 def loop_kmeans(my_instance, df_clust, labels_):
     """Update clustering via kmeans from scratch.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param df_clust: _description_
+    :param df_clust: clustering related data
     :type df_clust: pd.DataFrame
-    :param labels_: _description_
+    :param labels_: clustering labels
     :type labels_: List
-    :return: _description_
-    :rtype: Tuple
+    :return: clustering variance matrix, number of changes in clustering, silhouette score before
+    and after loop, null objects to match other return objects
+    :rtype: Tuple[
+        np.array, int, float, float, Dict, mdl.Model, int, int, float, float
+    ]
     """
     logging.info('# Clustering via k-means from scratch #')
     init_loop_silhouette = clt.get_silhouette(df_clust, labels_)
 
     new_labels_ = clt.perform_clustering(
         df_clust.drop('cluster', axis=1), 'kmeans', my_instance.nb_clusters)
     nb_clust_changes_loop = len(
@@ -1212,22 +1275,25 @@
             init_loop_silhouette, end_loop_silhouette,
             {}, None, 0, 0, 0, 0)
 
 
 def stream_km(my_instance, df_clust, labels_):
     """Update clustering via kmeans from scratch.
 
-    :param my_instance: _description_
+    :param my_instance: Instance object
     :type my_instance: Instance
-    :param df_clust: _description_
+    :param df_clust: clustering related data
     :type df_clust: pd.DataFrame
-    :param labels_: _description_
+    :param labels_: clustering labels
     :type labels_: List
-    :return: _description_
-    :rtype: Tuple
+    :return: clustering variance matrix, number of changes in clustering, silhouette score before
+    and after loop, null objects to match other return objects
+    :rtype: Tuple[
+        np.array, int, float, float, Dict, mdl.Model, int, int, float, float
+    ]
     """
     logging.info('# Clustering via streamkm #')
     init_loop_silhouette = clt.get_silhouette(df_clust, labels_)
 
     it.streamkm_model.partial_fit(df_clust.drop('cluster', axis=1))
     _, new_labels_ = it.streamkm_model.get_final_clusters(
         my_instance.nb_clusters, seed=my_instance.nb_clusters)
@@ -1256,31 +1322,31 @@
 
 def end_loop(
     working_df_indiv, tmin, nb_clust_changes, nb_place_changes, nb_overload,
     total_loop_time, loop_nb, df_host_evo
 ):
     """Perform all stuffs after last loop.
 
-    :param working_df_indiv: _description_
+    :param working_df_indiv: current loop data
     :type working_df_indiv: pd.DataFrame
-    :param tmin: _description_
+    :param tmin: starting time of current window
     :type tmin: int
-    :param nb_clust_changes: _description_
+    :param nb_clust_changes: number of changes in clustering
     :type nb_clust_changes: int
-    :param nb_place_changes: _description_
+    :param nb_place_changes: number of changes in placement
     :type nb_place_changes: int
-    :param nb_overload: _description_
+    :param nb_overload: number of node overload
     :type nb_overload: int
-    :param total_loop_time: _description_
+    :param total_loop_time: total running time for all loops
     :type total_loop_time: float
-    :param loop_nb: _description_
+    :param loop_nb: final loop number
     :type loop_nb: int
-    :param df_host_evo: _description_
+    :param df_host_evo: evolving node data
     :type df_host_evo: pd.DataFrame
-    :return: _description_
+    :return: evolving node data
     :rtype: pd.DataFrame
     """
     working_df_host = working_df_indiv.groupby(
         [working_df_indiv[it.tick_field], it.host_field],
         as_index=False).agg(it.dict_agg_metrics)
 
     (end_loop_obj_nodes, end_loop_obj_delta) = mdl.get_obj_value_host(
@@ -1307,19 +1373,19 @@
         )
     return df_host_evo
 
 
 def add_time(loop_nb, action, time):
     """Add an action time in times dataframe.
 
-    :param loop_nb: _description_
+    :param loop_nb: current loop number
     :type loop_nb: int
-    :param action: _description_
+    :param action: action / method we add time for
     :type action: str
-    :param time: _description_
+    :param time: running time of the action
     :type time: float
     """
     it.times_df = pd.concat(
         [
             it.times_df,
             pd.DataFrame.from_records([{
                 'num_loop': loop_nb,
```

### Comparing `hots-0.1.5/src/hots/model.py` & `hots-0.1.6/src/hots/model.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/node.py` & `hots-0.1.6/src/hots/node.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/placement.py` & `hots-0.1.6/src/hots/placement.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots/plot.py` & `hots-0.1.6/src/hots/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 
 import networkx as nx
 
 import numpy as np
 
 import pandas as pd
 
-import plotly.express as px
-import plotly.graph_objects as go
-from plotly.subplots import make_subplots
-
 import scipy.cluster.hierarchy as hac
 
 from . import init as it
 
 # Global variables
 # TODO manage big number of colors
 colors = ['blue', 'orange', 'green', 'red', 'purple',
@@ -273,39 +269,40 @@
     ax.axvline(x=sep_time, color='red', linestyle='--')
     ax.axhline(y=max_cap, color='red')
 
     plt.draw()
     return fig
 
 
-def plot_containers_groupby_nodes_px(
-    df_indiv, max_cap, sep_time, metrics=None
-):
-    """Plot containers consumption grouped by node.
-
-    :param df_indiv: _description_
-    :type df_indiv: pd.DataFrame
-    :param max_cap: _description_
-    :type max_cap: int
-    :param sep_time: _description_
-    :type sep_time: int
-    :param metrics: _description_, defaults to None
-    :type metrics: List[str], optional
-    """
-    # TODO several metrics ?
-    # TODO line_shape in params
-    metrics = metrics or it.metrics
-    pvt = pd.pivot_table(df_indiv, columns=it.host_field,
-                         index=df_indiv[it.tick_field],
-                         aggfunc='sum', values=metrics[0])
-    fig = px.line(pvt, line_shape='spline',
-                  title='Host CPU consumption')
-    fig.add_hline(max_cap, line={'color': 'red'})
-    fig.add_vline(sep_time, line={'color': 'red', 'dash': 'dashdot'})
-    fig.show(it.renderer)
+# The following uses plotly : comment for the moment
+# def plot_containers_groupby_nodes_px(
+#     df_indiv, max_cap, sep_time, metrics=None
+# ):
+#     """Plot containers consumption grouped by node.
+
+#     :param df_indiv: _description_
+#     :type df_indiv: pd.DataFrame
+#     :param max_cap: _description_
+#     :type max_cap: int
+#     :param sep_time: _description_
+#     :type sep_time: int
+#     :param metrics: _description_, defaults to None
+#     :type metrics: List[str], optional
+#     """
+#     # TODO several metrics ?
+#     # TODO line_shape in params
+#     metrics = metrics or it.metrics
+#     pvt = pd.pivot_table(df_indiv, columns=it.host_field,
+#                          index=df_indiv[it.tick_field],
+#                          aggfunc='sum', values=metrics[0])
+#     fig = px.line(pvt, line_shape='spline',
+#                   title='Host CPU consumption')
+#     fig.add_hline(max_cap, line={'color': 'red'})
+#     fig.add_vline(sep_time, line={'color': 'red', 'dash': 'dashdot'})
+#     fig.show(it.renderer)
 
 
 def plot_dendrogram(z_all, k):
     """Plot dendrogram for the hierarchical clustering building.
 
     :param z_all: _description_
     :type z_all: np.array
@@ -466,41 +463,42 @@
     # ax.plot(pvt)
     ax.axvline(x=sep_time, color='red', linestyle='--')
     ax.axhline(y=max_cap, color='red')
 
     return (fig, ax)
 
 
-def init_nodes_plot_px(df_indiv, sep_time, max_cap, metric=None):
-    """Initialize nodes consumption plot.
-
-    :param df_indiv: _description_
-    :type df_indiv: pd.DataFrame
-    :param sep_time: _description_
-    :type sep_time: int
-    :param max_cap: _description_
-    :type max_cap: int
-    :param metric: _description_, defaults to None
-    :type metric: str, optional
-    :return: _description_
-    :rtype: plt.Figure
-    """
-    metric = metric or it.metrics[0]
-    pvt = pd.pivot_table(
-        df_indiv.loc[
-            df_indiv[it.tick_field] <= sep_time],
-        columns=it.host_field,
-        index=df_indiv[it.tick_field],
-        aggfunc='sum', values=metric)
-    fig = px.line(pvt, line_shape='spline',
-                  title='Host CPU consumption')
-    fig.add_hline(max_cap, line={'color': 'red'})
-    fig.add_vline(sep_time, line={'color': 'red', 'dash': 'dashdot'})
-    fig.show(it.renderer)
-    return fig
+# The following uses plotly : comment for the moment
+# def init_nodes_plot_px(df_indiv, sep_time, max_cap, metric=None):
+#     """Initialize nodes consumption plot.
+
+#     :param df_indiv: _description_
+#     :type df_indiv: pd.DataFrame
+#     :param sep_time: _description_
+#     :type sep_time: int
+#     :param max_cap: _description_
+#     :type max_cap: int
+#     :param metric: _description_, defaults to None
+#     :type metric: str, optional
+#     :return: _description_
+#     :rtype: plt.Figure
+#     """
+#     metric = metric or it.metrics[0]
+#     pvt = pd.pivot_table(
+#         df_indiv.loc[
+#             df_indiv[it.tick_field] <= sep_time],
+#         columns=it.host_field,
+#         index=df_indiv[it.tick_field],
+#         aggfunc='sum', values=metric)
+#     fig = px.line(pvt, line_shape='spline',
+#                   title='Host CPU consumption')
+#     fig.add_hline(max_cap, line={'color': 'red'})
+#     fig.add_vline(sep_time, line={'color': 'red', 'dash': 'dashdot'})
+#     fig.show(it.renderer)
+#     return fig
 
 
 def update_nodes_plot(fig, ax, df, dict_id_n, metric=None):
     """Update nodes consumption plot with new data.
 
     :param fig: _description_
     :type fig: _type_
@@ -517,33 +515,34 @@
     temp_df = df.reset_index(drop=True)
     for n, data_n in temp_df.groupby(
             temp_df[it.host_field]):
         n_int = [k for k, v in dict_id_n.items() if v == n][0] % len(colors)
         ax.plot(data_n.groupby(data_n[it.tick_field])[metric].sum(), color=colors[n_int])
 
 
-def update_nodes_plot_px(fig, df, metric=None):
-    """Update nodes consumption plot with new data.
-
-    :param fig: _description_
-    :type fig: _type_
-    :param df: _description_
-    :type df: pd.DataFrame
-    :param metric: _description_, defaults to None
-    :type metric: str, optional
-    """
-    # TODO not open new tab each loop...
-    metric = metric or it.metrics[0]
-    pvt = pd.pivot_table(
-        df, columns=df[it.host_field],
-        index=df[it.tick_field], aggfunc='sum', values=metric)
-    for i, col in enumerate(fig.data):
-        fig.data[i]['y'] = pvt[pvt.columns[i]]
-        fig.data[i]['x'] = pvt.index
-    fig.show(it.renderer)
+# The following uses plotly : comment for the moment
+# def update_nodes_plot_px(fig, df, metric=None):
+#     """Update nodes consumption plot with new data.
+
+#     :param fig: _description_
+#     :type fig: _type_
+#     :param df: _description_
+#     :type df: pd.DataFrame
+#     :param metric: _description_, defaults to None
+#     :type metric: str, optional
+#     """
+#     # TODO not open new tab each loop...
+#     metric = metric or it.metrics[0]
+#     pvt = pd.pivot_table(
+#         df, columns=df[it.host_field],
+#         index=df[it.tick_field], aggfunc='sum', values=metric)
+#     for i, col in enumerate(fig.data):
+#         fig.data[i]['y'] = pvt[pvt.columns[i]]
+#         fig.data[i]['x'] = pvt.index
+#     fig.show(it.renderer)
 
 
 def init_plot_clustering(df_clust, metric=None):
     """Initialize clustering plot.
 
     :param df_clust: _description_
     :type df_clust: pd.DataFrame
@@ -611,38 +610,39 @@
             c_int = [k for k, v in dict_id_c.items() if v == row[0]][0]
             # ax_[k].plot(row[1], colors[k], label=c_int)
             ax_[k].plot(row[1], label=c_int)
         ax_[k].legend()
     return (fig, ax_)
 
 
-def init_plot_clustering_px(df_clust, dict_id_c, metric=None):
-    """Initialize clustering plot.
-
-    :param df_clust: _description_
-    :type df_clust: pd.DataFrame
-    :param dict_id_c: _description_
-    :type dict_id_c: Dict
-    :param metric: _description_, defaults to None
-    :type metric: str, optional
-    :return: _description_
-    :rtype: plt.Figure
-    """
-    metric = metric or it.metrics[0]
-    fig = make_subplots(rows=int(df_clust.cluster.max() + 1),
-                        shared_xaxes=True, cols=1)
-    for k, data in df_clust.groupby(['cluster']):
-        for row in data.drop(labels='cluster', axis=1).iterrows():
-            fig.append_trace(go.Scatter(
-                x=row[1].index,
-                y=row[1].values,
-                name=row[0]
-            ), row=k + 1, col=1)
-    fig.show(it.renderer)
-    return fig
+# The following uses plotly : comment for the moment
+# def init_plot_clustering_px(df_clust, dict_id_c, metric=None):
+#     """Initialize clustering plot.
+
+#     :param df_clust: _description_
+#     :type df_clust: pd.DataFrame
+#     :param dict_id_c: _description_
+#     :type dict_id_c: Dict
+#     :param metric: _description_, defaults to None
+#     :type metric: str, optional
+#     :return: _description_
+#     :rtype: plt.Figure
+#     """
+#     metric = metric or it.metrics[0]
+#     fig = make_subplots(rows=int(df_clust.cluster.max() + 1),
+#                         shared_xaxes=True, cols=1)
+#     for k, data in df_clust.groupby(['cluster']):
+#         for row in data.drop(labels='cluster', axis=1).iterrows():
+#             fig.append_trace(go.Scatter(
+#                 x=row[1].index,
+#                 y=row[1].values,
+#                 name=row[0]
+#             ), row=k + 1, col=1)
+#     fig.show(it.renderer)
+#     return fig
 
 
 def update_clustering_plot(fig, ax, df_clust, dict_id_c, metric=None):
     """Update clustering plot with new data.
 
     :param fig: _description_
     :type fig: _type_
@@ -699,56 +699,14 @@
     """
     for k, data in df_clust.groupby(['cluster']):
         for row in data.drop(labels='cluster', axis=1).iterrows():
             c_int = [k for k, v in dict_id_c.items() if v == row[0]][0]
             ax_[k].plot(row[1], colors[k], label=c_int)
 
 
-def update_clustering_plot_px(fig, df_clust, dict_id_c, tick=1, metric=None):
-    """Update clustering plot with new data.
-
-    :param fig: _description_
-    :type fig: _type_
-    :param df_clust: _description_
-    :type df_clust: pd.DataFrame
-    :param dict_id_c: _description_
-    :type dict_id_c: Dict
-    :param tick: _description_, defaults to 1
-    :type tick: int, optional
-    :param metric: _description_, defaults to None
-    :type metric: str, optional
-    """
-    pass
-    # for k, data in df_clust.groupby(['cluster']):
-    # for row in data.drop(labels='cluster', axis=1).iterrows():
-
-    # for i, col in enumerate(fig.data):
-    # c = fig.data[i]['name']
-    # c_df = df_clust.loc[c]
-    # c_clust = df_clust.loc[c, 'cluster']
-    # c_df = c_df.drop(labels='cluster', axis=0)
-    # print(fig.data[i], i)
-    # if fig.data[i]['row'] != c_clust:
-    #     fig.data[i]['row'] = c_clust
-    #     print('je change')
-
-    # fig.data[i]['y'] = np.append(fig.data[i]['y'], c_df.values[-tick:])
-    # fig.data[i]['x'] = np.append(fig.data[i]['x'], c_df.index[-tick:])
-
-    # fig.show(it.renderer)
-
-    # def plot_nodes_adding_containers(df_indiv: pd.DataFrame,
-    #                                   max_cap: int, sep_time: int):
-    #     """Plot nodes consumption showing allocated containers."""
-    #     fig, ax = plt.subplots()
-    #     fig.suptitle('Node CPU consumption')
-    #     # TODO generic
-    #     ax.set_ylim([0, max_cap + (max_cap * 0.2)])
-
-
 def plot_conflict_graph(graph):
     """Plot the conflict graph from dual values.
 
     :param graph: _description_
     :type graph: nx.Graph
     """
     fig, ax = plt.subplots()
```

### Comparing `hots-0.1.5/src/hots/tools.py` & `hots-0.1.6/src/hots/tools.py`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/src/hots.egg-info/PKG-INFO` & `hots-0.1.6/src/hots.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hots
-Version: 0.1.5
+Version: 0.1.6
 Summary: Resource Allocation via Clustering
 Author-email: Smile R&D team <rnd@smile.fr>
 License: MIT
 Project-URL: Homepage, https://github.com/Smile-SA/hots
 Project-URL: Documentation, https://hots.readthedocs.io/en/latest/
 Keywords: Resource,Optimisation,Clustering,Planning
 Platform: any
@@ -20,17 +20,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-# **HOTS**
+<h1 align="center">
+<img src="doc/source/_static/hots_logo.png" width="250">
+</h1><br>
 
-> Hybrid Optimization for Time Series  
+> Hybrid Optimization for Time Series (HOTS)  
 > HOTS solves problems presented as time series using machine learning and optimization methods.  
 > The library supports multiple resource related problems (placement, allocation), presented as one or more metrics.
 
 ## Requirements for running HOTS
 
 HOTS works on any platform with Python 3.8 and up.
 
@@ -111,14 +113,16 @@
 - Marco Mariani
 - Gilles Lenfant
 - Soobash Daiboo
 - Kang Du
 - Amaury Sauret
 - SMILE R&D
 
+As HOTS was created during a PhD, credits have to be given to academic supervisors, Céline Rouveirol and Frédéric Roupin, involved in the algorithm thinking.
+
 ## Links
 
 - [Project home](https://github.com/Smile-SA/hots)
 - [File issues (bugs, ...)](https://github.com/Smile-SA/hots/issues)
 - [PyPi package](https://pypi.org/project/hots/)
 - [Documentation](https://hots.readthedocs.io/en/latest/)
 - [PhD document](https://theses.hal.science/tel-03997934)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hots-0.1.5/src/hots.egg-info/SOURCES.txt` & `hots-0.1.6/src/hots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hots-0.1.5/tests/test_packaging.py` & `hots-0.1.6/tests/test_packaging.py`

 * *Files identical despite different names*

