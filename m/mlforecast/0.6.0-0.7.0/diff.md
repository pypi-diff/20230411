# Comparing `tmp/mlforecast-0.6.0.tar.gz` & `tmp/mlforecast-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforecast-0.6.0.tar", last modified: Fri Feb  3 03:20:47 2023, max compression
+gzip compressed data, was "mlforecast-0.7.0.tar", last modified: Tue Apr 11 03:21:28 2023, max compression
```

## Comparing `mlforecast-0.6.0.tar` & `mlforecast-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-02-03 03:20:47.235446 mlforecast-0.6.0/
--rw-rw-r--   0 jose      (1000) jose      (1000)     4398 2022-08-24 00:36:43.000000 mlforecast-0.6.0/CONTRIBUTING.md
--rw-rw-r--   0 jose      (1000) jose      (1000)    11336 2022-06-30 02:33:08.000000 mlforecast-0.6.0/LICENSE
--rw-rw-r--   0 jose      (1000) jose      (1000)      111 2022-08-10 00:50:44.000000 mlforecast-0.6.0/MANIFEST.in
--rw-rw-r--   0 jose      (1000) jose      (1000)     9149 2023-02-03 03:20:47.235446 mlforecast-0.6.0/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)     8254 2022-11-29 02:34:18.000000 mlforecast-0.6.0/README.md
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-02-03 03:20:47.231446 mlforecast-0.6.0/mlforecast/
--rw-rw-r--   0 jose      (1000) jose      (1000)      112 2023-02-03 03:12:30.000000 mlforecast-0.6.0/mlforecast/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    21208 2023-02-03 03:12:30.000000 mlforecast-0.6.0/mlforecast/_modidx.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     2325 2022-09-27 02:46:19.000000 mlforecast-0.6.0/mlforecast/_nbdev.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    26515 2023-02-03 03:12:29.000000 mlforecast-0.6.0/mlforecast/core.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-02-03 03:20:47.235446 mlforecast-0.6.0/mlforecast/distributed/
--rw-rw-r--   0 jose      (1000) jose      (1000)      146 2023-02-03 03:12:30.000000 mlforecast-0.6.0/mlforecast/distributed/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     4109 2023-02-03 03:12:29.000000 mlforecast-0.6.0/mlforecast/distributed/core.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    16824 2023-02-03 03:12:30.000000 mlforecast-0.6.0/mlforecast/distributed/forecast.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-02-03 03:20:47.235446 mlforecast-0.6.0/mlforecast/distributed/models/
--rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-02-03 03:12:30.000000 mlforecast-0.6.0/mlforecast/distributed/models/__init__.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      682 2023-02-03 03:12:28.000000 mlforecast-0.6.0/mlforecast/distributed/models/lgb.py
--rw-rw-r--   0 jose      (1000) jose      (1000)      444 2023-02-03 03:12:28.000000 mlforecast-0.6.0/mlforecast/distributed/models/xgb.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    25427 2023-02-03 03:12:28.000000 mlforecast-0.6.0/mlforecast/forecast.py
--rw-rw-r--   0 jose      (1000) jose      (1000)    20755 2023-02-03 03:12:28.000000 mlforecast-0.6.0/mlforecast/lgb_cv.py
--rw-rw-r--   0 jose      (1000) jose      (1000)     7011 2023-02-03 03:12:28.000000 mlforecast-0.6.0/mlforecast/utils.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-02-03 03:20:47.235446 mlforecast-0.6.0/mlforecast.egg-info/
--rw-rw-r--   0 jose      (1000) jose      (1000)     9149 2023-02-03 03:20:47.000000 mlforecast-0.6.0/mlforecast.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      635 2023-02-03 03:20:47.000000 mlforecast-0.6.0/mlforecast.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2023-02-03 03:20:47.000000 mlforecast-0.6.0/mlforecast.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2022-08-10 00:45:47.000000 mlforecast-0.6.0/mlforecast.egg-info/not-zip-safe
--rw-rw-r--   0 jose      (1000) jose      (1000)      214 2023-02-03 03:20:47.000000 mlforecast-0.6.0/mlforecast.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       11 2023-02-03 03:20:47.000000 mlforecast-0.6.0/mlforecast.egg-info/top_level.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)      990 2023-02-03 03:12:43.000000 mlforecast-0.6.0/settings.ini
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2023-02-03 03:20:47.235446 mlforecast-0.6.0/setup.cfg
--rw-rw-r--   0 jose      (1000) jose      (1000)     2595 2022-08-24 00:36:43.000000 mlforecast-0.6.0/setup.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/
+-rw-rw-r--   0 jose      (1000) jose      (1000)     4398 2022-08-24 00:36:43.000000 mlforecast-0.7.0/CONTRIBUTING.md
+-rw-rw-r--   0 jose      (1000) jose      (1000)    11336 2022-06-30 02:33:08.000000 mlforecast-0.7.0/LICENSE
+-rw-rw-r--   0 jose      (1000) jose      (1000)      111 2022-08-10 00:50:44.000000 mlforecast-0.7.0/MANIFEST.in
+-rw-rw-r--   0 jose      (1000) jose      (1000)    12376 2023-04-11 03:21:28.003682 mlforecast-0.7.0/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)    11481 2023-04-11 03:15:06.000000 mlforecast-0.7.0/README.md
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:27.999682 mlforecast-0.7.0/mlforecast/
+-rw-rw-r--   0 jose      (1000) jose      (1000)       90 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    28103 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/_modidx.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    21383 2023-04-11 03:17:40.000000 mlforecast-0.7.0/mlforecast/core.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/
+-rw-rw-r--   0 jose      (1000) jose      (1000)      102 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    25116 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/forecast.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/
+-rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/__init__.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/dask/
+-rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/dask/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)      714 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/dask/lgb.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)      527 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/dask/xgb.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/ray/
+-rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/ray/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)      450 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/ray/lgb.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)      552 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/ray/xgb.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:28.003682 mlforecast-0.7.0/mlforecast/distributed/models/spark/
+-rw-rw-r--   0 jose      (1000) jose      (1000)        0 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/distributed/models/spark/__init__.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)      836 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/spark/lgb.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)      862 2023-04-11 03:17:41.000000 mlforecast-0.7.0/mlforecast/distributed/models/spark/xgb.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    25498 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/forecast.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     5962 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/grouped_array.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)    22132 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/lgb_cv.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     2541 2023-04-11 03:17:42.000000 mlforecast-0.7.0/mlforecast/target_transforms.py
+-rw-rw-r--   0 jose      (1000) jose      (1000)     6309 2023-04-11 03:17:43.000000 mlforecast-0.7.0/mlforecast/utils.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-04-11 03:21:27.999682 mlforecast-0.7.0/mlforecast.egg-info/
+-rw-rw-r--   0 jose      (1000) jose      (1000)    12376 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)      962 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2022-08-10 00:45:47.000000 mlforecast-0.7.0/mlforecast.egg-info/not-zip-safe
+-rw-rw-r--   0 jose      (1000) jose      (1000)      304 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/requires.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       11 2023-04-11 03:21:27.000000 mlforecast-0.7.0/mlforecast.egg-info/top_level.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)     1043 2023-04-11 03:17:57.000000 mlforecast-0.7.0/settings.ini
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2023-04-11 03:21:28.003682 mlforecast-0.7.0/setup.cfg
+-rw-rw-r--   0 jose      (1000) jose      (1000)     2613 2023-03-31 03:20:59.000000 mlforecast-0.7.0/setup.py
```

### Comparing `mlforecast-0.6.0/CONTRIBUTING.md` & `mlforecast-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mlforecast-0.6.0/LICENSE` & `mlforecast-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlforecast-0.6.0/PKG-INFO` & `mlforecast-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.6.0
+Version: 0.7.0
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
@@ -18,25 +18,45 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: distributed
 Provides-Extra: dev
 License-File: LICENSE
 
-mlforecast
+Nixtla  
+[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
+ ![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+<div align="center">
+
+<center>
+<img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
+</center>
+<h1 align="center">
+Machine Learning 🤖 Forecast
+</h1>
+<h3 align="center">
+Scalable machine learning for time series forecasting
+</h3>
+
 [![CI](https://github.com/Nixtla/mlforecast/actions/workflows/ci.yaml/badge.svg)](https://github.com/Nixtla/mlforecast/actions/workflows/ci.yaml)
 [![Python](https://img.shields.io/pypi/pyversions/mlforecast.png)](https://pypi.org/project/mlforecast/)
 [![PyPi](https://img.shields.io/pypi/v/mlforecast?color=blue.png)](https://pypi.org/project/mlforecast/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/mlforecast?color=blue.png)](https://anaconda.org/conda-forge/mlforecast)
 [![License](https://img.shields.io/github/license/Nixtla/mlforecast.png)](https://github.com/Nixtla/mlforecast/blob/main/LICENSE)
 
+**mlforecast** is a framework to perform time series forecasting using
+machine learning models, with the option to scale to massive amounts of
+data using remote clusters.
+
+</div>
+
 ## Install
 
 ### PyPI
 
 `pip install mlforecast`
 
 If you want to perform distributed training, you can instead use
@@ -53,14 +73,90 @@
 Note that this installation comes with the required dependencies for the
 local interface. If you want to perform distributed training, you must
 install dask (`conda install -c conda-forge dask`) and either
 [LightGBM](https://github.com/microsoft/LightGBM/tree/master/python-package)
 or
 [XGBoost](https://xgboost.readthedocs.io/en/latest/install.html#python).
 
+## Quick Start
+
+**Minimal Example**
+
+``` python
+import lightgbm as lgb
+
+from mlforecast import MLForecast
+from sklearn.linear_model import LinearRegression
+
+mlf = MLForecast(
+    models = [LinearRegression(), lgb.LGBMRegressor()],
+    lags=[1, 12],
+    freq = 'M'
+)
+mlf.fit(df)
+mlf.predict(12)
+```
+
+**Get Started with this [quick
+guide](https://nixtla.github.io/mlforecast/docs/quick_start_local.html).**
+
+**Follow this [end-to-end
+walkthrough](https://nixtla.github.io/mlforecast/docs/end_to_end_walkthrough.html)
+for best practices.**
+
+## Why?
+
+Current Python alternatives for machine learning models are slow,
+inaccurate and don’t scale well. So we created a library that can be
+used to forecast in production environments. `MLForecast` includes
+efficient feature engineering to train any machine learning model (with
+`fit` and `predict` methods such as
+[`sklearn`](https://scikit-learn.org/stable/)) to fit millions of time
+series.
+
+## Features
+
+- Fastest implementations of feature engineering for time series
+  forecasting in Python.
+- Out-of-the-box compatibility with Spark, Dask, and Ray.
+- Probabilistic Forecasting with Conformal Prediction.
+- Support for exogenous variables and static covariates.
+- Familiar `sklearn` syntax: `.fit` and `.predict`.
+
+Missing something? Please open an issue or write us in
+[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
+
+## Examples and Guides
+
+📚 [End to End
+Walkthrough](https://nixtla.github.io/mlforecast/docs/end_to_end_walkthrough.html):
+model training, evaluation and selection for multiple time series.
+
+🔎 [Probabilistic
+Forecasting](https://nixtla.github.io/mlforecast/docs/prediction_intervals.html):
+use Conformal Prediction to produce prediciton intervals.
+
+👩‍🔬 [Cross
+Validation](https://nixtla.github.io/mlforecast/docs/cross_validation.html):
+robust model’s performance evaluation.
+
+🔌 [Predict Demand
+Peaks](https://nixtla.github.io/mlforecast/docs/electricity_peak_forecasting.html):
+electricity load forecasting for detecting daily peaks and reducing
+electric bills.
+
+📈 [Transfer
+Learning](https://nixtla.github.io/mlforecast/docs/transfer_learning.html):
+pretrain a model using a set of time series and then predict another one
+using that pretrained model.
+
+🌡️ [Distributed
+Training](https://nixtla.github.io/mlforecast/docs/quick_start_distributed.html):
+use a Dask cluster to train models at scale.
+
 ## How to use
 
 The following provides a very basic overview, for a more detailed
 description see the
 [documentation](https://nixtla.github.io/mlforecast/).
 
 ### Data setup
@@ -82,52 +178,52 @@
 ```
 
 <div>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
+      <th>unique_id</th>
       <th>ds</th>
       <th>y</th>
       <th>static_0</th>
     </tr>
-    <tr>
-      <th>unique_id</th>
-      <th></th>
-      <th></th>
-      <th></th>
-    </tr>
   </thead>
   <tbody>
     <tr>
-      <th>id_00</th>
+      <th>0</th>
+      <td>id_00</td>
       <td>2000-01-01</td>
       <td>1.751917</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>1</th>
+      <td>id_00</td>
       <td>2000-01-02</td>
       <td>9.196715</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>2</th>
+      <td>id_00</td>
       <td>2000-01-03</td>
       <td>18.577788</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>3</th>
+      <td>id_00</td>
       <td>2000-01-04</td>
       <td>24.520646</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>4</th>
+      <td>id_00</td>
       <td>2000-01-05</td>
       <td>33.418028</td>
       <td>72</td>
     </tr>
   </tbody>
 </table>
 </div>
@@ -159,14 +255,15 @@
 array, if they have additional arguments you can either supply a tuple
 (`transform_func`, `arg1`, `arg2`, …) or define new functions fixing the
 arguments. You can also define differences to apply to the series before
 fitting that will be restored when predicting.
 
 ``` python
 from mlforecast import MLForecast
+from mlforecast.target_transforms import Differences
 from numba import njit
 from window_ops.expanding import expanding_mean
 from window_ops.rolling import rolling_mean
 
 
 @njit
 def rolling_mean_28(x):
@@ -178,36 +275,28 @@
     freq='D',
     lags=[7, 14],
     lag_transforms={
         1: [expanding_mean],
         7: [rolling_mean_28]
     },
     date_features=['dayofweek'],
-    differences=[1],
+    target_transforms=[Differences([1])],
 )
 ```
 
 ### Training
 
 To compute the features and train the models call `fit` on your
-`Forecast` object. Here you have to specify the columns that:
-
-- Identify each serie (`id_col`). If the series identifier is the index
-  you can specify `id_col='index'`
-- Contain the timestamps (`time_col`). Can also be integers if your data
-  doesn’t have timestamps.
-- Are the series values (`target_col`)
-- Are static (`static_features`). These are features that don’t change
-  over time and can be repeated when predicting.
+`Forecast` object.
 
 ``` python
-fcst.fit(series, id_col='index', time_col='ds', target_col='y', static_features=['static_0'])
+fcst.fit(series)
 ```
 
-    MLForecast(models=[LGBMRegressor, XGBRegressor, RandomForestRegressor], freq=<Day>, lag_features=['lag-7', 'lag-14', 'expanding_mean_lag-1', 'rolling_mean_28_lag-7'], date_features=['dayofweek'], num_threads=1)
+    MLForecast(models=[LGBMRegressor, XGBRegressor, RandomForestRegressor], freq=<Day>, lag_features=['lag7', 'lag14', 'expanding_mean_lag1', 'rolling_mean_28_lag7'], date_features=['dayofweek'], num_threads=1)
 
 ### Predicting
 
 To get the forecasts for the next `n` days call `predict(n)` on the
 forecast object. This will automatically handle the updates required by
 the features using a recursive strategy.
 
@@ -217,120 +306,126 @@
 ```
 
 <div>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
+      <th>unique_id</th>
       <th>ds</th>
       <th>LGBMRegressor</th>
       <th>XGBRegressor</th>
       <th>RandomForestRegressor</th>
     </tr>
-    <tr>
-      <th>unique_id</th>
-      <th></th>
-      <th></th>
-      <th></th>
-      <th></th>
-    </tr>
   </thead>
   <tbody>
     <tr>
-      <th>id_00</th>
+      <th>0</th>
+      <td>id_00</td>
       <td>2000-04-04</td>
       <td>69.082830</td>
       <td>67.761337</td>
-      <td>68.184016</td>
+      <td>68.226556</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>1</th>
+      <td>id_00</td>
       <td>2000-04-05</td>
       <td>75.706024</td>
       <td>74.588699</td>
-      <td>75.470680</td>
+      <td>75.484774</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>2</th>
+      <td>id_00</td>
       <td>2000-04-06</td>
       <td>82.222473</td>
       <td>81.058289</td>
-      <td>82.846249</td>
+      <td>82.853684</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>3</th>
+      <td>id_00</td>
       <td>2000-04-07</td>
       <td>89.577638</td>
       <td>88.735947</td>
-      <td>90.201271</td>
+      <td>90.351212</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>4</th>
+      <td>id_00</td>
       <td>2000-04-08</td>
       <td>44.149095</td>
       <td>44.981384</td>
-      <td>46.096322</td>
+      <td>46.291173</td>
     </tr>
     <tr>
       <th>...</th>
       <td>...</td>
       <td>...</td>
       <td>...</td>
       <td>...</td>
+      <td>...</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>275</th>
+      <td>id_19</td>
       <td>2000-03-23</td>
-      <td>30.236012</td>
-      <td>31.949095</td>
-      <td>32.656369</td>
+      <td>30.151270</td>
+      <td>31.814825</td>
+      <td>32.592799</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>276</th>
+      <td>id_19</td>
       <td>2000-03-24</td>
-      <td>31.308269</td>
-      <td>32.765919</td>
-      <td>33.624488</td>
+      <td>31.418104</td>
+      <td>32.653374</td>
+      <td>33.563294</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>277</th>
+      <td>id_19</td>
       <td>2000-03-25</td>
-      <td>32.788550</td>
-      <td>33.628864</td>
-      <td>34.581486</td>
+      <td>32.843567</td>
+      <td>33.586033</td>
+      <td>34.530912</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>278</th>
+      <td>id_19</td>
       <td>2000-03-26</td>
-      <td>34.086976</td>
-      <td>34.508457</td>
-      <td>35.553173</td>
+      <td>34.127210</td>
+      <td>34.541473</td>
+      <td>35.507559</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>279</th>
+      <td>id_19</td>
       <td>2000-03-27</td>
-      <td>34.288968</td>
-      <td>35.411613</td>
-      <td>36.526505</td>
+      <td>34.329202</td>
+      <td>35.450943</td>
+      <td>36.425001</td>
     </tr>
   </tbody>
 </table>
-<p>280 rows × 4 columns</p>
+<p>280 rows × 5 columns</p>
 </div>
 
 ### Visualize results
 
 ``` python
 import matplotlib.pyplot as plt
 import pandas as pd
 
 fig, ax = plt.subplots(nrows=2, ncols=2, figsize=(12, 6), gridspec_kw=dict(hspace=0.3))
-for i, (cat, axi) in enumerate(zip(series.index.categories, ax.flat)):
-    pd.concat([series.loc[cat, ['ds', 'y']], predictions.loc[cat]]).set_index('ds').plot(ax=axi)
-    axi.set(title=cat, xlabel=None)
+for i, (uid, axi) in enumerate(zip(series['unique_id'].unique(), ax.flat)):
+    fltr = lambda df: df['unique_id'].eq(uid)
+    pd.concat([series.loc[fltr, ['ds', 'y']], predictions.loc[fltr]]).set_index('ds').plot(ax=axi)
+    axi.set(title=uid, xlabel=None)
     if i % 2 == 0:
         axi.legend().remove()
     else:
         axi.legend(bbox_to_anchor=(1.01, 1.0))
 fig.savefig('figs/index.png', bbox_inches='tight')
 plt.close()
 ```
@@ -338,7 +433,12 @@
 ![](https://raw.githubusercontent.com/Nixtla/mlforecast/main/figs/index.png)
 
 ## Sample notebooks
 
 - [m5](https://www.kaggle.com/code/lemuz90/m5-mlforecast-eval)
 - [m4](https://www.kaggle.com/code/lemuz90/m4-competition)
 - [m4-cv](https://www.kaggle.com/code/lemuz90/m4-competition-cv)
+
+## How to contribute
+
+See
+[CONTRIBUTING.md](https://github.com/Nixtla/mlforecast/blob/main/CONTRIBUTING.md).
```

### Comparing `mlforecast-0.6.0/README.md` & `mlforecast-0.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,38 @@
-mlforecast
+Nixtla  
+[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
+ ![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+<div align="center">
+
+<center>
+<img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
+</center>
+<h1 align="center">
+Machine Learning 🤖 Forecast
+</h1>
+<h3 align="center">
+Scalable machine learning for time series forecasting
+</h3>
+
 [![CI](https://github.com/Nixtla/mlforecast/actions/workflows/ci.yaml/badge.svg)](https://github.com/Nixtla/mlforecast/actions/workflows/ci.yaml)
 [![Python](https://img.shields.io/pypi/pyversions/mlforecast.png)](https://pypi.org/project/mlforecast/)
 [![PyPi](https://img.shields.io/pypi/v/mlforecast?color=blue.png)](https://pypi.org/project/mlforecast/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/mlforecast?color=blue.png)](https://anaconda.org/conda-forge/mlforecast)
 [![License](https://img.shields.io/github/license/Nixtla/mlforecast.png)](https://github.com/Nixtla/mlforecast/blob/main/LICENSE)
 
+**mlforecast** is a framework to perform time series forecasting using
+machine learning models, with the option to scale to massive amounts of
+data using remote clusters.
+
+</div>
+
 ## Install
 
 ### PyPI
 
 `pip install mlforecast`
 
 If you want to perform distributed training, you can instead use
@@ -29,14 +49,90 @@
 Note that this installation comes with the required dependencies for the
 local interface. If you want to perform distributed training, you must
 install dask (`conda install -c conda-forge dask`) and either
 [LightGBM](https://github.com/microsoft/LightGBM/tree/master/python-package)
 or
 [XGBoost](https://xgboost.readthedocs.io/en/latest/install.html#python).
 
+## Quick Start
+
+**Minimal Example**
+
+``` python
+import lightgbm as lgb
+
+from mlforecast import MLForecast
+from sklearn.linear_model import LinearRegression
+
+mlf = MLForecast(
+    models = [LinearRegression(), lgb.LGBMRegressor()],
+    lags=[1, 12],
+    freq = 'M'
+)
+mlf.fit(df)
+mlf.predict(12)
+```
+
+**Get Started with this [quick
+guide](https://nixtla.github.io/mlforecast/docs/quick_start_local.html).**
+
+**Follow this [end-to-end
+walkthrough](https://nixtla.github.io/mlforecast/docs/end_to_end_walkthrough.html)
+for best practices.**
+
+## Why?
+
+Current Python alternatives for machine learning models are slow,
+inaccurate and don’t scale well. So we created a library that can be
+used to forecast in production environments. `MLForecast` includes
+efficient feature engineering to train any machine learning model (with
+`fit` and `predict` methods such as
+[`sklearn`](https://scikit-learn.org/stable/)) to fit millions of time
+series.
+
+## Features
+
+- Fastest implementations of feature engineering for time series
+  forecasting in Python.
+- Out-of-the-box compatibility with Spark, Dask, and Ray.
+- Probabilistic Forecasting with Conformal Prediction.
+- Support for exogenous variables and static covariates.
+- Familiar `sklearn` syntax: `.fit` and `.predict`.
+
+Missing something? Please open an issue or write us in
+[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
+
+## Examples and Guides
+
+📚 [End to End
+Walkthrough](https://nixtla.github.io/mlforecast/docs/end_to_end_walkthrough.html):
+model training, evaluation and selection for multiple time series.
+
+🔎 [Probabilistic
+Forecasting](https://nixtla.github.io/mlforecast/docs/prediction_intervals.html):
+use Conformal Prediction to produce prediciton intervals.
+
+👩‍🔬 [Cross
+Validation](https://nixtla.github.io/mlforecast/docs/cross_validation.html):
+robust model’s performance evaluation.
+
+🔌 [Predict Demand
+Peaks](https://nixtla.github.io/mlforecast/docs/electricity_peak_forecasting.html):
+electricity load forecasting for detecting daily peaks and reducing
+electric bills.
+
+📈 [Transfer
+Learning](https://nixtla.github.io/mlforecast/docs/transfer_learning.html):
+pretrain a model using a set of time series and then predict another one
+using that pretrained model.
+
+🌡️ [Distributed
+Training](https://nixtla.github.io/mlforecast/docs/quick_start_distributed.html):
+use a Dask cluster to train models at scale.
+
 ## How to use
 
 The following provides a very basic overview, for a more detailed
 description see the
 [documentation](https://nixtla.github.io/mlforecast/).
 
 ### Data setup
@@ -58,52 +154,52 @@
 ```
 
 <div>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
+      <th>unique_id</th>
       <th>ds</th>
       <th>y</th>
       <th>static_0</th>
     </tr>
-    <tr>
-      <th>unique_id</th>
-      <th></th>
-      <th></th>
-      <th></th>
-    </tr>
   </thead>
   <tbody>
     <tr>
-      <th>id_00</th>
+      <th>0</th>
+      <td>id_00</td>
       <td>2000-01-01</td>
       <td>1.751917</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>1</th>
+      <td>id_00</td>
       <td>2000-01-02</td>
       <td>9.196715</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>2</th>
+      <td>id_00</td>
       <td>2000-01-03</td>
       <td>18.577788</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>3</th>
+      <td>id_00</td>
       <td>2000-01-04</td>
       <td>24.520646</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>4</th>
+      <td>id_00</td>
       <td>2000-01-05</td>
       <td>33.418028</td>
       <td>72</td>
     </tr>
   </tbody>
 </table>
 </div>
@@ -135,14 +231,15 @@
 array, if they have additional arguments you can either supply a tuple
 (`transform_func`, `arg1`, `arg2`, …) or define new functions fixing the
 arguments. You can also define differences to apply to the series before
 fitting that will be restored when predicting.
 
 ``` python
 from mlforecast import MLForecast
+from mlforecast.target_transforms import Differences
 from numba import njit
 from window_ops.expanding import expanding_mean
 from window_ops.rolling import rolling_mean
 
 
 @njit
 def rolling_mean_28(x):
@@ -154,36 +251,28 @@
     freq='D',
     lags=[7, 14],
     lag_transforms={
         1: [expanding_mean],
         7: [rolling_mean_28]
     },
     date_features=['dayofweek'],
-    differences=[1],
+    target_transforms=[Differences([1])],
 )
 ```
 
 ### Training
 
 To compute the features and train the models call `fit` on your
-`Forecast` object. Here you have to specify the columns that:
-
-- Identify each serie (`id_col`). If the series identifier is the index
-  you can specify `id_col='index'`
-- Contain the timestamps (`time_col`). Can also be integers if your data
-  doesn’t have timestamps.
-- Are the series values (`target_col`)
-- Are static (`static_features`). These are features that don’t change
-  over time and can be repeated when predicting.
+`Forecast` object.
 
 ``` python
-fcst.fit(series, id_col='index', time_col='ds', target_col='y', static_features=['static_0'])
+fcst.fit(series)
 ```
 
-    MLForecast(models=[LGBMRegressor, XGBRegressor, RandomForestRegressor], freq=<Day>, lag_features=['lag-7', 'lag-14', 'expanding_mean_lag-1', 'rolling_mean_28_lag-7'], date_features=['dayofweek'], num_threads=1)
+    MLForecast(models=[LGBMRegressor, XGBRegressor, RandomForestRegressor], freq=<Day>, lag_features=['lag7', 'lag14', 'expanding_mean_lag1', 'rolling_mean_28_lag7'], date_features=['dayofweek'], num_threads=1)
 
 ### Predicting
 
 To get the forecasts for the next `n` days call `predict(n)` on the
 forecast object. This will automatically handle the updates required by
 the features using a recursive strategy.
 
@@ -193,120 +282,126 @@
 ```
 
 <div>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
+      <th>unique_id</th>
       <th>ds</th>
       <th>LGBMRegressor</th>
       <th>XGBRegressor</th>
       <th>RandomForestRegressor</th>
     </tr>
-    <tr>
-      <th>unique_id</th>
-      <th></th>
-      <th></th>
-      <th></th>
-      <th></th>
-    </tr>
   </thead>
   <tbody>
     <tr>
-      <th>id_00</th>
+      <th>0</th>
+      <td>id_00</td>
       <td>2000-04-04</td>
       <td>69.082830</td>
       <td>67.761337</td>
-      <td>68.184016</td>
+      <td>68.226556</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>1</th>
+      <td>id_00</td>
       <td>2000-04-05</td>
       <td>75.706024</td>
       <td>74.588699</td>
-      <td>75.470680</td>
+      <td>75.484774</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>2</th>
+      <td>id_00</td>
       <td>2000-04-06</td>
       <td>82.222473</td>
       <td>81.058289</td>
-      <td>82.846249</td>
+      <td>82.853684</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>3</th>
+      <td>id_00</td>
       <td>2000-04-07</td>
       <td>89.577638</td>
       <td>88.735947</td>
-      <td>90.201271</td>
+      <td>90.351212</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>4</th>
+      <td>id_00</td>
       <td>2000-04-08</td>
       <td>44.149095</td>
       <td>44.981384</td>
-      <td>46.096322</td>
+      <td>46.291173</td>
     </tr>
     <tr>
       <th>...</th>
       <td>...</td>
       <td>...</td>
       <td>...</td>
       <td>...</td>
+      <td>...</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>275</th>
+      <td>id_19</td>
       <td>2000-03-23</td>
-      <td>30.236012</td>
-      <td>31.949095</td>
-      <td>32.656369</td>
+      <td>30.151270</td>
+      <td>31.814825</td>
+      <td>32.592799</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>276</th>
+      <td>id_19</td>
       <td>2000-03-24</td>
-      <td>31.308269</td>
-      <td>32.765919</td>
-      <td>33.624488</td>
+      <td>31.418104</td>
+      <td>32.653374</td>
+      <td>33.563294</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>277</th>
+      <td>id_19</td>
       <td>2000-03-25</td>
-      <td>32.788550</td>
-      <td>33.628864</td>
-      <td>34.581486</td>
+      <td>32.843567</td>
+      <td>33.586033</td>
+      <td>34.530912</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>278</th>
+      <td>id_19</td>
       <td>2000-03-26</td>
-      <td>34.086976</td>
-      <td>34.508457</td>
-      <td>35.553173</td>
+      <td>34.127210</td>
+      <td>34.541473</td>
+      <td>35.507559</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>279</th>
+      <td>id_19</td>
       <td>2000-03-27</td>
-      <td>34.288968</td>
-      <td>35.411613</td>
-      <td>36.526505</td>
+      <td>34.329202</td>
+      <td>35.450943</td>
+      <td>36.425001</td>
     </tr>
   </tbody>
 </table>
-<p>280 rows × 4 columns</p>
+<p>280 rows × 5 columns</p>
 </div>
 
 ### Visualize results
 
 ``` python
 import matplotlib.pyplot as plt
 import pandas as pd
 
 fig, ax = plt.subplots(nrows=2, ncols=2, figsize=(12, 6), gridspec_kw=dict(hspace=0.3))
-for i, (cat, axi) in enumerate(zip(series.index.categories, ax.flat)):
-    pd.concat([series.loc[cat, ['ds', 'y']], predictions.loc[cat]]).set_index('ds').plot(ax=axi)
-    axi.set(title=cat, xlabel=None)
+for i, (uid, axi) in enumerate(zip(series['unique_id'].unique(), ax.flat)):
+    fltr = lambda df: df['unique_id'].eq(uid)
+    pd.concat([series.loc[fltr, ['ds', 'y']], predictions.loc[fltr]]).set_index('ds').plot(ax=axi)
+    axi.set(title=uid, xlabel=None)
     if i % 2 == 0:
         axi.legend().remove()
     else:
         axi.legend(bbox_to_anchor=(1.01, 1.0))
 fig.savefig('figs/index.png', bbox_inches='tight')
 plt.close()
 ```
@@ -314,7 +409,12 @@
 ![](https://raw.githubusercontent.com/Nixtla/mlforecast/main/figs/index.png)
 
 ## Sample notebooks
 
 - [m5](https://www.kaggle.com/code/lemuz90/m5-mlforecast-eval)
 - [m4](https://www.kaggle.com/code/lemuz90/m4-competition)
 - [m4-cv](https://www.kaggle.com/code/lemuz90/m4-competition-cv)
+
+## How to contribute
+
+See
+[CONTRIBUTING.md](https://github.com/Nixtla/mlforecast/blob/main/CONTRIBUTING.md).
```

### Comparing `mlforecast-0.6.0/mlforecast/core.py` & `mlforecast-0.7.0/mlforecast/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 # %% auto 0
 __all__ = ['TimeSeries']
 
 # %% ../nbs/core.ipynb 3
 import concurrent.futures
 import inspect
-import reprlib
 import warnings
 from collections import Counter, OrderedDict
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from numba import njit
 from sklearn.base import BaseEstimator
-from window_ops.shift import shift_array
+
+from .grouped_array import GroupedArray
+from .target_transforms import BaseTargetTransform, Differences
 
 # %% ../nbs/core.ipynb 10
 date_features_dtypes = {
     "year": np.uint16,
     "month": np.uint8,
     "day": np.uint8,
     "hour": np.uint8,
@@ -38,196 +39,30 @@
     "is_month_end": np.uint8,
     "is_quarter_start": np.uint8,
     "is_quarter_end": np.uint8,
     "is_year_start": np.uint8,
     "is_year_end": np.uint8,
 }
 
-
-@njit
-def _append_new(data, indptr, new):
-    """Append each value of new to each group in data formed by indptr."""
-    n_series = len(indptr) - 1
-    new_data = np.empty(data.size + new.size, dtype=data.dtype)
-    new_indptr = indptr.copy()
-    new_indptr[1:] += np.arange(1, n_series + 1)
-    for i in range(n_series):
-        prev_slice = slice(indptr[i], indptr[i + 1])
-        new_slice = slice(new_indptr[i], new_indptr[i + 1] - 1)
-        new_data[new_slice] = data[prev_slice]
-        new_data[new_indptr[i + 1] - 1] = new[i]
-    return new_data, new_indptr
-
 # %% ../nbs/core.ipynb 11
-@njit
-def _identity(x: np.ndarray) -> np.ndarray:
-    """Do nothing to the input."""
-    return x
-
-
-def _as_tuple(x):
-    """Return a tuple from the input."""
-    if isinstance(x, tuple):
-        return x
-    return (x,)
-
-
-@njit(nogil=True)
-def _transform_series(data, indptr, updates_only, lag, func, *args) -> np.ndarray:
-    """Shifts every group in `data` by `lag` and computes `func(shifted, *args)`.
-
-    If `updates_only=True` only last value of the transformation for each group is returned,
-    otherwise the full transformation is returned"""
-    n_series = len(indptr) - 1
-    if updates_only:
-        out = np.empty_like(data[:n_series])
-        for i in range(n_series):
-            lagged = shift_array(data[indptr[i] : indptr[i + 1]], lag)
-            out[i] = func(lagged, *args)[-1]
-    else:
-        out = np.empty_like(data)
-        for i in range(n_series):
-            lagged = shift_array(data[indptr[i] : indptr[i + 1]], lag)
-            out[indptr[i] : indptr[i + 1]] = func(lagged, *args)
-    return out
-
-
-@njit
-def _diff(x, lag):
-    y = x.copy()
-    for i in range(lag):
-        y[i] = np.nan
-    for i in range(lag, x.size):
-        y[i] = x[i] - x[i - lag]
-    return y
-
-
-@njit
-def _apply_difference(data, indptr, new_data, new_indptr, d):
-    n_series = len(indptr) - 1
-    for i in range(n_series):
-        new_data[new_indptr[i] : new_indptr[i + 1]] = data[
-            indptr[i + 1] - d : indptr[i + 1]
-        ]
-        sl = slice(indptr[i], indptr[i + 1])
-        data[sl] = _diff(data[sl], d)
-
-
-@njit
-def _restore_difference(preds, data, indptr, d):
-    n_series = len(indptr) - 1
-    h = len(preds) // n_series
-    for i in range(n_series):
-        s = data[indptr[i] : indptr[i + 1]]
-        for j in range(min(h, d)):
-            preds[i * h + j] += s[j]
-        for j in range(d, h):
-            preds[i * h + j] += preds[i * h + j - d]
-
-
-@njit
-def _expand_target(data, indptr, max_horizon):
-    out = np.empty((data.size, max_horizon), dtype=data.dtype)
-    n_series = len(indptr) - 1
-    n = 0
-    for i in range(n_series):
-        serie = data[indptr[i] : indptr[i + 1]]
-        for j in range(serie.size):
-            upper = min(serie.size - j, max_horizon)
-            for k in range(upper):
-                out[n, k] = serie[j + k]
-            for k in range(upper, max_horizon):
-                out[n, k] = np.nan
-            n += 1
-    return out
-
-# %% ../nbs/core.ipynb 12
-class GroupedArray:
-    """Array made up of different groups. Can be thought of (and iterated) as a list of arrays.
-
-    All the data is stored in a single 1d array `data`.
-    The indices for the group boundaries are stored in another 1d array `indptr`."""
-
-    def __init__(self, data: np.ndarray, indptr: np.ndarray):
-        self.data = data
-        self.indptr = indptr
-        self.ngroups = len(indptr) - 1
-
-    def __len__(self) -> int:
-        return self.ngroups
-
-    def __getitem__(self, idx: int) -> np.ndarray:
-        return self.data[self.indptr[idx] : self.indptr[idx + 1]]
-
-    def __setitem__(self, idx: int, vals: np.ndarray):
-        if self[idx].size != vals.size:
-            raise ValueError(f"vals must be of size {self[idx].size}")
-        self[idx][:] = vals
-
-    @classmethod
-    def from_sorted_df(cls, df: pd.DataFrame, target_col: str) -> "GroupedArray":
-        grouped = df.groupby(level=0, observed=True)
-        sizes = grouped.size().values
-        indptr = np.append(0, sizes.cumsum())
-        data = df[target_col].values
-        if data.dtype not in (np.float32, np.float64):
-            # since all transformations generate nulls, we need a float dtype
-            data = data.astype(np.float32)
-        return cls(data, indptr)
-
-    def transform_series(
-        self, updates_only: bool, lag: int, func: Callable, *args
-    ) -> np.ndarray:
-        return _transform_series(self.data, self.indptr, updates_only, lag, func, *args)
-
-    def restore_difference(self, preds: np.ndarray, d: int):
-        _restore_difference(preds, self.data, self.indptr, d)
-
-    def expand_target(self, max_horizon: int) -> np.ndarray:
-        return _expand_target(self.data, self.indptr, max_horizon)
-
-    def take_from_groups(self, idx: Union[int, slice]) -> "GroupedArray":
-        """Takes `idx` from each group in the array."""
-        ranges = [
-            range(self.indptr[i], self.indptr[i + 1])[idx] for i in range(self.ngroups)
-        ]
-        items = [self.data[rng] for rng in ranges]
-        sizes = np.array([item.size for item in items])
-        data = np.hstack(items)
-        indptr = np.append(0, sizes.cumsum())
-        return GroupedArray(data, indptr)
-
-    def append(self, new: np.ndarray) -> "GroupedArray":
-        """Appends each element of `new` to each existing group. Returns a copy."""
-        if new.size != self.ngroups:
-            raise ValueError(f"new must be of size {self.ngroups}")
-        new_data, new_indptr = _append_new(self.data, self.indptr, new)
-        return GroupedArray(new_data, new_indptr)
-
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}(ndata={self.data.size}, ngroups={self.ngroups})"
-        )
-
-# %% ../nbs/core.ipynb 20
 def _build_transform_name(lag, tfm, *args) -> str:
     """Creates a name for a transformation based on `lag`, the name of the function and its arguments."""
     tfm_name = f"{tfm.__name__}_lag{lag}"
     func_params = inspect.signature(tfm).parameters
     func_args = list(func_params.items())[1:]  # remove input array argument
     changed_params = [
         f"{name}{value}"
         for value, (name, arg) in zip(args, func_args)
         if arg.default != value
     ]
     if changed_params:
         tfm_name += "_" + "_".join(changed_params)
     return tfm_name
 
-# %% ../nbs/core.ipynb 22
+# %% ../nbs/core.ipynb 13
 def _name_models(current_names):
     ctr = Counter(current_names)
     if not ctr:
         return []
     if max(ctr.values()) < 2:
         return current_names
     names = current_names.copy()
@@ -237,35 +72,65 @@
             name = f"{x}{count}"
             ctr[x] -= 1
         else:
             name = x
         names[-i] = name
     return names
 
-# %% ../nbs/core.ipynb 24
+# %% ../nbs/core.ipynb 15
+@njit
+def _identity(x: np.ndarray) -> np.ndarray:
+    """Do nothing to the input."""
+    return x
+
+
+def _as_tuple(x):
+    """Return a tuple from the input."""
+    if isinstance(x, tuple):
+        return x
+    return (x,)
+
+
+@njit
+def _expand_target(data, indptr, max_horizon):
+    out = np.empty((data.size, max_horizon), dtype=data.dtype)
+    n_series = len(indptr) - 1
+    n = 0
+    for i in range(n_series):
+        serie = data[indptr[i] : indptr[i + 1]]
+        for j in range(serie.size):
+            upper = min(serie.size - j, max_horizon)
+            for k in range(upper):
+                out[n, k] = serie[j + k]
+            for k in range(upper, max_horizon):
+                out[n, k] = np.nan
+            n += 1
+    return out
+
+# %% ../nbs/core.ipynb 16
 Freq = Union[int, str, pd.offsets.BaseOffset]
 Lags = Iterable[int]
 LagTransform = Union[Callable, Tuple[Callable, Any]]
 LagTransforms = Dict[int, List[LagTransform]]
 DateFeature = Union[str, Callable]
-Differences = Iterable[int]
 Models = Union[BaseEstimator, List[BaseEstimator], Dict[str, BaseEstimator]]
 
-# %% ../nbs/core.ipynb 25
+# %% ../nbs/core.ipynb 17
 class TimeSeries:
     """Utility class for storing and transforming time series data."""
 
     def __init__(
         self,
         freq: Optional[Freq] = None,
         lags: Optional[Lags] = None,
         lag_transforms: Optional[LagTransforms] = None,
         date_features: Optional[Iterable[DateFeature]] = None,
-        differences: Optional[Differences] = None,
+        differences: Optional[Iterable[int]] = None,
         num_threads: int = 1,
+        target_transforms: Optional[List[BaseTargetTransform]] = None,
     ):
         if isinstance(freq, str):
             self.freq = pd.tseries.frequencies.to_offset(freq)
         elif isinstance(freq, pd.offsets.BaseOffset):
             self.freq = freq
         elif isinstance(freq, int):
             self.freq = freq
@@ -278,16 +143,26 @@
             )
         if not isinstance(num_threads, int) or num_threads < 1:
             warnings.warn("Setting num_threads to 1.")
             num_threads = 1
         self.lags = [] if lags is None else list(lags)
         self.lag_transforms = {} if lag_transforms is None else lag_transforms
         self.date_features = [] if date_features is None else list(date_features)
-        self.differences = [] if differences is None else list(differences)
+        if differences is not None:
+            warnings.warn(
+                "The differences argument is deprecated and will be removed in a future version.\n"
+                "Please pass an `mlforecast.target_transforms.Differences` instance to the `target_transforms` argument instead."
+                ""
+            )
+            if target_transforms is None:
+                target_transforms = [Differences(differences)]
+            else:
+                target_transforms = [Differences(differences)] + target_transforms
         self.num_threads = num_threads
+        self.target_transforms = target_transforms
         for feature in self.date_features:
             if callable(feature) and feature.__name__ == "<lambda>":
                 raise ValueError(
                     "Can't use a lambda as a date feature because the function name gets used as the feature name."
                 )
 
         self.transforms: Dict[str, Tuple[Any, ...]] = OrderedDict()
@@ -324,17 +199,15 @@
         id_col: str,
         time_col: str,
         target_col: str,
         static_features: Optional[List[str]] = None,
         keep_last_n: Optional[int] = None,
     ) -> "TimeSeries":
         """Save the series values, ids and last dates."""
-        if id_col not in df and id_col != "index":
-            raise ValueError(f"Couldn't find {id_col} column.")
-        for col in (time_col, target_col):
+        for col in (id_col, time_col, target_col):
             if col not in df:
                 raise ValueError(f"Data doesn't contain {col} column")
         if df[target_col].isnull().any():
             raise ValueError(f"{target_col} column contains null values.")
         if pd.api.types.is_datetime64_dtype(df[time_col]):
             if self.freq == 1:
                 raise ValueError(
@@ -345,54 +218,43 @@
                 warnings.warn("Setting `freq=1` since time col is int.")
                 self.freq = 1
         else:
             raise ValueError(f"{time_col} must be either timestamp or integer.")
         self.id_col = id_col
         self.target_col = target_col
         self.time_col = time_col
-        if id_col != "index":
-            df = df.set_index(id_col)
         if static_features is None:
-            static_features = df.columns.drop([time_col, target_col])
+            static_features = df.columns.drop([id_col, time_col, target_col])
+        elif id_col in static_features:
+            raise ValueError(
+                "Cannot use the id_col as a static feature. Please create a separate column."
+            )
         self.static_features = (
-            df[static_features].groupby(level=0, observed=True).head(1)
-        )
-        sort_idxs = pd.core.sorting.lexsort_indexer([df.index, df[time_col]])
-        sorted_df = (
-            df[[time_col, target_col]].set_index(time_col, append=True).iloc[sort_idxs]
+            df.set_index(id_col)[static_features].groupby(id_col, observed=True).head(1)
         )
+        sort_idxs = pd.core.sorting.lexsort_indexer([df[id_col], df[time_col]])
         self.restore_idxs = np.empty(df.shape[0], dtype=np.int32)
         self.restore_idxs[sort_idxs] = np.arange(df.shape[0])
+        sorted_df = df[[id_col, time_col, target_col]].iloc[sort_idxs]
+        if self.target_transforms is not None:
+            for tfm in self.target_transforms:
+                tfm.set_column_names(id_col, time_col, target_col)
+                sorted_df = tfm.fit_transform(sorted_df)
+        sorted_df = sorted_df.set_index([id_col, time_col])
         self.uids = sorted_df.index.unique(level=0)
-        self.ga = GroupedArray.from_sorted_df(sorted_df, target_col)
-        if self.differences:
-            original_sizes = self.ga.indptr[1:].cumsum()
-            total_diffs = sum(self.differences)
-            small_series = self.uids[original_sizes < total_diffs]
-            if small_series.size:
-                msg = reprlib.repr(small_series.tolist())
-                raise ValueError(
-                    f"The following series are too short for the differences: {msg}"
-                )
-            self.original_values_ = []
-            n_series = len(self.ga.indptr) - 1
-            for d in self.differences:
-                new_data = np.empty_like(self.ga.data, shape=n_series * d)
-                new_indptr = d * np.arange(n_series + 1, dtype=np.int32)
-                _apply_difference(self.ga.data, self.ga.indptr, new_data, new_indptr, d)
-                self.original_values_.append(GroupedArray(new_data, new_indptr))
+        self.ga = GroupedArray.from_sorted_df(sorted_df, id_col, target_col)
         self.features_ = self._compute_transforms()
         if keep_last_n is not None:
             self.ga = self.ga.take_from_groups(slice(-keep_last_n, None))
         self._ga = GroupedArray(self.ga.data, self.ga.indptr)
         self.last_dates = sorted_df.index.get_level_values(self.time_col)[
             self.ga.indptr[1:] - 1
         ]
         self.features_order_ = (
-            df.columns.drop([self.time_col, self.target_col]).tolist() + self.features
+            df.columns.drop([id_col, time_col, target_col]).tolist() + self.features
         )
         return self
 
     def _apply_transforms(self, updates_only: bool = False) -> Dict[str, np.ndarray]:
         """Apply the transformations using the main process.
 
         If `updates_only` then only the updates are returned.
@@ -459,15 +321,16 @@
         dropna: bool = True,
         max_horizon: Optional[int] = None,
         return_X_y: bool = False,
     ) -> pd.DataFrame:
         """Add the features to `df`.
 
         if `dropna=True` then all the null rows are dropped."""
-        df = df.copy(deep=bool(self.differences) and not return_X_y)
+        modifies_target = bool(self.target_transforms)
+        df = df.copy(deep=modifies_target and not return_X_y)
 
         # lag transforms
         for feat in self.transforms.keys():
             df[feat] = self.features_[feat][self.restore_idxs]
 
         # date features
         dates = df[self.time_col]
@@ -476,40 +339,46 @@
         for feature in self.date_features:
             feat_name, feat_vals = self._compute_date_feature(dates, feature)
             df[feat_name] = feat_vals
 
         # target
         self.max_horizon = max_horizon
         if max_horizon is None:
-            if self.differences:
+            if modifies_target:
                 target = pd.Series(self.ga.data[self.restore_idxs], index=df.index)
             else:
                 target = df[self.target_col]
         else:
             target = pd.DataFrame(
                 self.ga.expand_target(max_horizon)[self.restore_idxs],
                 index=df.index,
                 columns=[f"{self.target_col}{i}" for i in range(max_horizon)],
             )
 
         # determine rows to keep
-        features = df.columns.drop(self.target_col)
         if dropna:
-            keep_rows = df[features].notnull().all(1).values
+            feature_nulls = df[self.features].isnull().any(axis=1)
+            target_nulls = target.isnull()
+            if target_nulls.ndim == 2:
+                # target nulls for each horizon are dropped in MLForecast.fit_models
+                # we just drop rows here for which all the target values are null
+                target_nulls = target_nulls.all(axis=1)
+            keep_rows = ~(feature_nulls | target_nulls).values
         else:
             keep_rows = np.full(df.shape[0], True)
 
         # assemble return
+        xs = df.columns.drop(self.target_col)
         if return_X_y:
-            return df.loc[keep_rows, features], target.loc[keep_rows]
+            return df.loc[keep_rows, xs], target.loc[keep_rows]
         if max_horizon is None:
-            if self.differences:
+            if modifies_target:
                 df[self.target_col] = target
         else:
-            df = pd.concat([df[features], target], axis=1)
+            df = pd.concat([df[xs], target], axis=1)
         return df.loc[keep_rows]
 
     def fit_transform(
         self,
         data: pd.DataFrame,
         id_col: str,
         time_col: str,
@@ -556,61 +425,49 @@
         else:
             features = self._apply_multithreaded_transforms(updates_only=True)
 
         for feature in self.date_features:
             feat_name, feat_vals = self._compute_date_feature(self.curr_dates, feature)
             features[feat_name] = feat_vals
 
-        features_df = pd.DataFrame(features, columns=self.features, index=self.uids)
-        results_df = self.static_features.join(features_df)
-        results_df[self.time_col] = self.curr_dates
-        return results_df
-
-    def _restore_differences(self, preds) -> None:
-        if not self.differences:
-            return
-        for d, ga in zip(reversed(self.differences), reversed(self.original_values_)):
-            ga.restore_difference(preds, d)
+        features_df = pd.DataFrame(features, columns=self.features)
+        features_df[self.id_col] = self.uids
+        features_df[self.time_col] = self.curr_dates
+        return self.static_features.merge(features_df, on=self.id_col)
 
     def _get_raw_predictions(self) -> np.ndarray:
-        preds = np.array(self.y_pred).ravel("F")
-        self._restore_differences(preds)
-        return preds
+        return np.array(self.y_pred).ravel("F")
 
     def _get_predictions(self) -> pd.DataFrame:
         """Get all the predicted values with their corresponding ids and datestamps."""
         n_preds = len(self.y_pred)
-        idx = pd.Index(
-            np.repeat(self.uids, n_preds),
-            name=self.id_col if self.id_col != "index" else None,
-            dtype=self.uids.dtype,
+        uids = pd.Series(
+            np.repeat(self.uids, n_preds), name=self.id_col, dtype=self.uids.dtype
         )
         df = pd.DataFrame(
             {
+                self.id_col: uids,
                 self.time_col: np.array(self.test_dates).ravel("F"),
                 f"{self.target_col}_pred": self._get_raw_predictions(),
             },
-            index=idx,
         )
         return df
 
     def _predict_setup(self) -> None:
         self.curr_dates = self.last_dates.copy()
         self.test_dates = []
         self.y_pred = []
         self.ga = GroupedArray(self._ga.data, self._ga.indptr)
 
     def _get_features_for_next_step(self, dynamic_dfs):
         new_x = self._update_features()
         if dynamic_dfs:
-            idx_name = new_x.index.name
-            new_x = new_x.reset_index()
             for df in dynamic_dfs:
                 new_x = new_x.merge(df, how="left")
-            new_x = new_x.sort_values(idx_name)
+            new_x = new_x.sort_values(self.id_col)
         nulls = new_x.isnull().any()
         if any(nulls):
             warnings.warn(f'Found null values in {", ".join(nulls[nulls].index)}.')
         return new_x[self.features_order_]
 
     def _predict_recursive(
         self,
@@ -627,26 +484,24 @@
             self._predict_setup()
             for _ in range(horizon):
                 new_x = self._get_features_for_next_step(dynamic_dfs)
                 if before_predict_callback is not None:
                     new_x = before_predict_callback(new_x)
                 predictions = model.predict(new_x)
                 if after_predict_callback is not None:
-                    predictions_serie = pd.Series(predictions, index=new_x.index)
+                    predictions_serie = pd.Series(predictions, index=self.uids)
                     predictions = after_predict_callback(predictions_serie).values
                 self._update_y(predictions)
             if i == 0:
                 preds = self._get_predictions()
                 preds = preds.rename(
                     columns={f"{self.target_col}_pred": name}, copy=False
                 )
             else:
                 preds[name] = self._get_raw_predictions()
-        if self.id_col != "index":
-            preds = preds.reset_index()
         return preds
 
     def _predict_multi(
         self,
         models: Dict[str, BaseEstimator],
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
@@ -663,51 +518,47 @@
         dates = np.hstack(
             [
                 date + (i + 1) * self.freq
                 for date in self.last_dates
                 for i in range(horizon)
             ]
         )
-        if self.id_col == "index":
-            result = pd.DataFrame({self.time_col: dates}, index=pd.Index(uids))
-        else:
-            result = pd.DataFrame(
-                {
-                    self.id_col: uids,
-                    self.time_col: dates,
-                }
-            )
-        for i, (name, model) in enumerate(models.items()):
+        result = pd.DataFrame({self.id_col: uids, self.time_col: dates})
+        for name, model in models.items():
             self._predict_setup()
             new_x = self._get_features_for_next_step(dynamic_dfs)
             if before_predict_callback is not None:
                 new_x = before_predict_callback(new_x)
             predictions = np.empty((new_x.shape[0], horizon))
             for i in range(horizon):
                 predictions[:, i] = model[i].predict(new_x)
             raw_preds = predictions.ravel()
-            self._restore_differences(raw_preds)
             result[name] = raw_preds
         return result
 
     def predict(
         self,
         models: Dict[str, Union[BaseEstimator, List[BaseEstimator]]],
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
     ) -> pd.DataFrame:
         if getattr(self, "max_horizon", None) is None:
-            return self._predict_recursive(
+            preds = self._predict_recursive(
                 models,
                 horizon,
                 dynamic_dfs,
                 before_predict_callback,
                 after_predict_callback,
             )
-        return self._predict_multi(
-            models,
-            horizon,
-            dynamic_dfs,
-            before_predict_callback,
-        )
+        else:
+            preds = self._predict_multi(
+                models,
+                horizon,
+                dynamic_dfs,
+                before_predict_callback,
+            )
+        if self.target_transforms is not None:
+            for tfm in self.target_transforms[::-1]:
+                preds = tfm.inverse_transform(preds)
+        return preds
```

### Comparing `mlforecast-0.6.0/mlforecast/distributed/forecast.py` & `mlforecast-0.7.0/mlforecast/forecast.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,218 +1,399 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/distributed.forecast.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/forecast.ipynb.
 
 # %% auto 0
-__all__ = ['DistributedMLForecast', 'DistributedForecast']
+__all__ = ['MLForecast']
 
-# %% ../../nbs/distributed.forecast.ipynb 5
+# %% ../nbs/forecast.ipynb 3
+import copy
 import warnings
-from typing import Callable, Iterable, List, Optional
+from typing import TYPE_CHECKING, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
-import dask.dataframe as dd
 import numpy as np
 import pandas as pd
-from dask.distributed import Client, default_client
-from sklearn.base import clone
+from sklearn.base import BaseEstimator, clone
 
 from mlforecast.core import (
     DateFeature,
-    Differences,
     Freq,
     LagTransforms,
     Lags,
     Models,
     TimeSeries,
     _name_models,
 )
-from .core import DistributedTimeSeries
-from ..utils import backtest_splits
 
-# %% ../../nbs/distributed.forecast.ipynb 7
-class DistributedMLForecast:
-    """Distributed pipeline encapsulation."""
+if TYPE_CHECKING:
+    from mlforecast.lgb_cv import LightGBMCV
+from .target_transforms import BaseTargetTransform
+from .utils import backtest_splits, PredictionIntervals
+
+# %% ../nbs/forecast.ipynb 6
+def _add_conformal_distribution_intervals(
+    fcst_df: pd.DataFrame,
+    cs_df: pd.DataFrame,
+    model_names: List[str],
+    level: List[Union[int, float]],
+    cs_n_windows: int,
+    cs_window_size: int,
+    n_series: int,
+) -> pd.DataFrame:
+    """
+    Adds conformal intervals to a `fcst_df` based on conformal scores `cs_df`.
+    `level` should be already sorted. This strategy creates forecasts paths
+    based on errors and calculate quantiles using those paths.
+    """
+    fcst_df = fcst_df.copy()
+    alphas = [100 - lv for lv in level]
+    cuts = [alpha / 200 for alpha in reversed(alphas)]
+    cuts.extend(1 - alpha / 200 for alpha in alphas)
+    for model in model_names:
+        scores = cs_df[model].values.reshape(cs_n_windows, n_series, cs_window_size)
+        mean = fcst_df[model].values.reshape(1, n_series, -1)
+        scores = np.vstack([mean - scores, mean + scores])
+        quantiles = np.quantile(
+            scores,
+            cuts,
+            axis=0,
+        )
+        quantiles = quantiles.reshape(len(cuts), -1)
+        lo_cols = [f"{model}-lo-{lv}" for lv in reversed(level)]
+        hi_cols = [f"{model}-hi-{lv}" for lv in level]
+        out_cols = lo_cols + hi_cols
+        for i, col in enumerate(out_cols):
+            fcst_df[col] = quantiles[i]
+    return fcst_df
+
+# %% ../nbs/forecast.ipynb 7
+def _add_conformal_error_intervals(
+    fcst_df: pd.DataFrame,
+    cs_df: pd.DataFrame,
+    model_names: List[str],
+    level: List[Union[int, float]],
+    cs_n_windows: int,
+    cs_window_size: int,
+    n_series: int,
+) -> pd.DataFrame:
+    """
+    Adds conformal intervals to a `fcst_df` based on conformal scores `cs_df`.
+    `level` should be already sorted. This startegy creates prediction intervals
+    based on the absolute errors.
+    """
+    fcst_df = fcst_df.copy()
+    cuts = [lv / 100 for lv in level]
+    for model in model_names:
+        mean = fcst_df[model].values.ravel()
+        quantiles = np.quantile(
+            cs_df[model].values.reshape(cs_n_windows, n_series, cs_window_size),
+            cuts,
+            axis=0,
+        )
+        quantiles = quantiles.reshape(len(cuts), -1)
+        lo_cols = [f"{model}-lo-{lv}" for lv in reversed(level)]
+        hi_cols = [f"{model}-hi-{lv}" for lv in level]
+        for i, col in enumerate(lo_cols):
+            fcst_df[col] = mean - quantiles[len(level) - 1 - i]
+        for i, col in enumerate(hi_cols):
+            fcst_df[col] = mean + quantiles[i]
+    return fcst_df
+
+# %% ../nbs/forecast.ipynb 8
+def _get_conformal_method(method: str):
+    available_methods = {
+        "conformal_distribution": _add_conformal_distribution_intervals,
+        "conformal_error": _add_conformal_error_intervals,
+    }
+    if method not in available_methods.keys():
+        raise ValueError(
+            f"prediction intervals method {method} not supported "
+            f'please choose one of {", ".join(available_methods.keys())}'
+        )
+    return available_methods[method]
 
+# %% ../nbs/forecast.ipynb 10
+class MLForecast:
     def __init__(
         self,
         models: Models,
         freq: Optional[Freq] = None,
         lags: Optional[Lags] = None,
         lag_transforms: Optional[LagTransforms] = None,
         date_features: Optional[Iterable[DateFeature]] = None,
-        differences: Optional[Differences] = None,
+        differences: Optional[Iterable[int]] = None,
         num_threads: int = 1,
-        client: Optional[Client] = None,
+        target_transforms: Optional[List[BaseTargetTransform]] = None,
     ):
-        """Create distributed forecast object
+        """Create forecast object
 
         Parameters
         ----------
         models : regressor or list of regressors
             Models that will be trained and used to compute the forecasts.
-        freq : str or int, optional (default=None)
-            Pandas offset alias, e.g. 'D', 'W-THU' or integer denoting the frequency of the series.
+        freq : str or int or pd.offsets.BaseOffset, optional (default=None)
+            Pandas offset, pandas offset alias, e.g. 'D', 'W-THU' or integer denoting the frequency of the series.
         lags : list of int, optional (default=None)
             Lags of the target to use as features.
         lag_transforms : dict of int to list of functions, optional (default=None)
             Mapping of target lags to their transformations.
         date_features : list of str or callable, optional (default=None)
             Features computed from the dates. Can be pandas date attributes or functions that will take the dates as input.
         differences : list of int, optional (default=None)
             Differences to take of the target before computing the features. These are restored at the forecasting step.
         num_threads : int (default=1)
             Number of threads to use when computing the features.
-        client : dask distributed client
-            Client to use for computing data and training the models.
+        target_transforms : list of transformers, optional(default=None)
+            Transformations that will be applied to the target before computing the features and restored after the forecasting step.
         """
         if not isinstance(models, dict) and not isinstance(models, list):
             models = [models]
         if isinstance(models, list):
             model_names = _name_models([m.__class__.__name__ for m in models])
             models_with_names = dict(zip(model_names, models))
         else:
             models_with_names = models
         self.models = models_with_names
-        self.client = client or default_client()
-        self.dts = DistributedTimeSeries(
-            TimeSeries(
-                freq, lags, lag_transforms, date_features, differences, num_threads
-            ),
-            self.client,
+        self.ts = TimeSeries(
+            freq=freq,
+            lags=lags,
+            lag_transforms=lag_transforms,
+            date_features=date_features,
+            differences=differences,
+            num_threads=num_threads,
+            target_transforms=target_transforms,
         )
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return (
             f'{self.__class__.__name__}(models=[{", ".join(self.models.keys())}], '
             f"freq={self.freq}, "
-            f"lag_features={list(self.dts._base_ts.transforms.keys())}, "
-            f"date_features={self.dts._base_ts.date_features}, "
-            f"num_threads={self.dts._base_ts.num_threads}, "
-            f"client={self.client})"
+            f"lag_features={list(self.ts.transforms.keys())}, "
+            f"date_features={self.ts.date_features}, "
+            f"num_threads={self.ts.num_threads})"
         )
 
     @property
     def freq(self):
-        return self.dts._base_ts.freq
+        return self.ts.freq
+
+    @classmethod
+    def from_cv(cls, cv: "LightGBMCV") -> "MLForecast":
+        if not hasattr(cv, "best_iteration_"):
+            raise ValueError("LightGBMCV object must be fitted first.")
+        import lightgbm as lgb
+
+        fcst = cls(
+            lgb.LGBMRegressor(**{**cv.params, "n_estimators": cv.best_iteration_})
+        )
+        fcst.ts = copy.deepcopy(cv.ts)
+        return fcst
 
     def preprocess(
         self,
-        data: dd.DataFrame,
-        id_col: str = "index",
+        data: pd.DataFrame,
+        id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
-    ) -> dd.DataFrame:
+        max_horizon: Optional[int] = None,
+        return_X_y: bool = False,
+    ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, Union[pd.Series, pd.DataFrame]]]:
         """Add the features to `data`.
 
         Parameters
         ----------
-        data : dask DataFrame
+        data : pandas DataFrame
             Series data in long format.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
         dropna : bool (default=True)
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
+        max_horizon: int, optional (default=None)
+            Train this many models, where each model will predict a specific horizon.
+        return_X_y: bool (default=False)
+            Return a tuple with the features and the target. If False will return a single dataframe.
 
         Returns
         -------
-        result : dask DataFrame.
-            `data` plus added features.
+        result : pandas DataFrame or tuple of pandas Dataframe and either a pandas Series or a pandas Dataframe (for multi-output regression).
+            `data` plus added features and target(s).
         """
-        if id_col in data:
-            warnings.warn(
-                "It is recommended to have id_col as the index, since setting the index is a slow operation."
-            )
-            data = data.set_index(id_col)
-            id_col = "index"
-        return self.dts.fit_transform(
-            data, id_col, time_col, target_col, static_features, dropna, keep_last_n
+        return self.ts.fit_transform(
+            data,
+            id_col=id_col,
+            time_col=time_col,
+            target_col=target_col,
+            static_features=static_features,
+            dropna=dropna,
+            keep_last_n=keep_last_n,
+            max_horizon=max_horizon,
+            return_X_y=return_X_y,
         )
 
     def fit_models(
         self,
-        X: dd.DataFrame,
-        y: dd.Series,
-    ) -> "DistributedMLForecast":
+        X: pd.DataFrame,
+        y: Union[pd.Series, pd.DataFrame],
+    ) -> "MLForecast":
         """Manually train models. Use this if you called `Forecast.preprocess` beforehand.
 
         Parameters
         ----------
-        X : dask DataFrame
+        X : pandas DataFrame
             Features.
-        y : dask Series.
+        y : pandas Series or pandas DataFrame (multi-output).
             Target.
 
         Returns
         -------
-        self : DistributedForecast
+        self : MLForecast
             Forecast object with trained models.
         """
-        self.models_ = {}
+        self.models_: Dict[str, Union[BaseEstimator, List[BaseEstimator]]] = {}
         for name, model in self.models.items():
-            self.models_[name] = clone(model).fit(X, y).model_
+            if y.ndim == 2 and y.shape[1] > 1:
+                self.models_[name] = []
+                for col in y:
+                    keep = y[col].notnull()
+                    self.models_[name].append(
+                        clone(model).fit(X.loc[keep], y.loc[keep, col])
+                    )
+            else:
+                self.models_[name] = clone(model).fit(X, y)
         return self
 
-    def fit(
+    def _conformity_scores(
         self,
-        data: dd.DataFrame,
+        data: pd.DataFrame,
         id_col: str,
         time_col: str,
         target_col: str,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
-    ) -> "DistributedMLForecast":
+        max_horizon: Optional[int] = None,
+        n_windows: int = 2,
+        window_size: int = 1,
+    ):
+        """Compute conformity scores.
+
+        We need at least two cross validation errors to compute
+        quantiles for prediction intervals (`n_windows=2`).
+
+        The exception is raised by the PredictionIntervals data class.
+
+        In this simplest case, we assume the width of the interval
+        is the same for all the forecasting horizon (`window_size=1`).
+        """
+        cv_results = self.cross_validation(
+            data=data,
+            n_windows=n_windows,
+            window_size=window_size,
+            refit=False,
+            id_col=id_col,
+            time_col=time_col,
+            target_col=target_col,
+            static_features=static_features,
+            dropna=dropna,
+            keep_last_n=keep_last_n,
+            max_horizon=max_horizon,
+            prediction_intervals=None,
+        )
+        # conformity score for each model
+        for model in self.models.keys():
+            # compute absolute error for each model
+            cv_results[model] = np.abs(cv_results[model] - cv_results[target_col])
+        return cv_results.drop("y", axis=1)
+
+    def fit(
+        self,
+        data: pd.DataFrame,
+        id_col: str = "unique_id",
+        time_col: str = "ds",
+        target_col: str = "y",
+        static_features: Optional[List[str]] = None,
+        dropna: bool = True,
+        keep_last_n: Optional[int] = None,
+        max_horizon: Optional[int] = None,
+        prediction_intervals: Optional[PredictionIntervals] = None,
+    ) -> "MLForecast":
         """Apply the feature engineering and train the models.
 
         Parameters
         ----------
-        data : dask DataFrame
+        data : pandas DataFrame
             Series data in long format.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
         dropna : bool (default=True)
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
+        max_horizon: int, optional (default=None)
+            Train this many models, where each model will predict a specific horizon.
+        prediction_intervals : PredictionIntervals, optional (default=None)
+            Configuration to calibrate prediction intervals (Conformal Prediction).
 
         Returns
         -------
-        self : DistributedForecast
+        self : MLForecast
             Forecast object with series values and trained models.
         """
-        train_ddf = self.preprocess(
-            data, id_col, time_col, target_col, static_features, dropna, keep_last_n
+        self._cs_df: Optional[pd.DataFrame] = None
+        if prediction_intervals is not None:
+            self.prediction_intervals = prediction_intervals
+            self._cs_df = self._conformity_scores(
+                data=data,
+                id_col=id_col,
+                time_col=time_col,
+                target_col=target_col,
+                static_features=static_features,
+                dropna=dropna,
+                keep_last_n=keep_last_n,
+                n_windows=prediction_intervals.n_windows,
+                window_size=prediction_intervals.window_size,
+            )
+        X, y = self.preprocess(
+            data,
+            id_col=id_col,
+            time_col=time_col,
+            target_col=target_col,
+            static_features=static_features,
+            dropna=dropna,
+            keep_last_n=keep_last_n,
+            max_horizon=max_horizon,
+            return_X_y=True,
         )
-        X, y = train_ddf.drop(columns=[time_col, target_col]), train_ddf[target_col]
-        self.fit_models(X, y)
-        return self
+        X = X[self.ts.features_order_]
+        return self.fit_models(X, y)
 
     def predict(
         self,
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
-        new_data: Optional[dd.DataFrame] = None,
-    ) -> dd.DataFrame:
+        new_data: Optional[pd.DataFrame] = None,
+        level: Optional[List[Union[int, float]]] = None,
+    ) -> pd.DataFrame:
         """Compute the predictions for the next `horizon` steps.
 
         Parameters
         ----------
         horizon : int
             Number of periods to predict.
         dynamic_dfs : list of pandas DataFrame, optional (default=None)
@@ -225,207 +406,215 @@
             Function to call on the predictions before updating the targets.
                 This function will take a pandas Series with the predictions and should return another one with the same structure.
                 The series identifier is on the index.
         new_data : pandas DataFrame, optional (default=None)
             Series data of new observations for which forecasts are to be generated.
                 This dataframe should have the same structure as the one used to fit the model, including any features and time series data.
                 If `new_data` is not None, the method will generate forecasts for the new observations.
-
+        level : list of ints or floats, optional (default=None)
+            Confidence levels between 0 and 100 for prediction intervals.
 
         Returns
         -------
-        result : dask DataFrame
+        result : pandas DataFrame
             Predictions for each serie and timestep, with one column per model.
         """
+        if not hasattr(self, "models_"):
+            raise ValueError(
+                "No fitted models found. You have to call fit or preprocess + fit_models."
+            )
+
         if new_data is not None:
-            ts_info = self.dts.ts[0].result()
-            if ts_info.id_col in new_data:
-                warnings.warn(
-                    "It is recommended to have id_col as the index, since setting the index is a slow operation."
-                )
-                ddf = new_data.set_index(ts_info.id_col)
-                ts_info.id_col = "index"
-            else:
-                ddf = new_data
-            new_dts = DistributedTimeSeries(
-                TimeSeries(
-                    self.dts._base_ts.freq,
-                    self.dts._base_ts.lags,
-                    self.dts._base_ts.lag_transforms,
-                    self.dts._base_ts.date_features,
-                    self.dts._base_ts.differences,
-                    self.dts._base_ts.num_threads,
-                ),
-                self.client,
+            new_ts = TimeSeries(
+                freq=self.ts.freq,
+                lags=self.ts.lags,
+                lag_transforms=self.ts.lag_transforms,
+                date_features=self.ts.date_features,
+                num_threads=self.ts.num_threads,
+                target_transforms=self.ts.target_transforms,
             )
-            new_dts.fit_transform(
-                ddf,
-                ts_info.id_col,
-                ts_info.time_col,
-                ts_info.target_col,
-                ts_info.static_features.columns,
-                ts_info.dropna,
-                ts_info.keep_last_n,
+            new_ts._fit(
+                new_data,
+                id_col=self.ts.id_col,
+                time_col=self.ts.time_col,
+                target_col=self.ts.target_col,
+                static_features=self.ts.static_features.columns,
+                keep_last_n=self.ts.keep_last_n,
             )
-            dts = new_dts
+            new_ts.max_horizon = self.ts.max_horizon
+            ts = new_ts
         else:
-            dts = self.dts
+            ts = self.ts
 
-        return dts.predict(
+        forecasts = ts.predict(
             self.models_,
             horizon,
             dynamic_dfs,
             before_predict_callback,
             after_predict_callback,
         )
+        if level is not None:
+            if self._cs_df is None:
+                warn_msg = (
+                    "Please rerun the `fit` method passing a proper value "
+                    "to prediction intervals to compute them."
+                )
+                warnings.warn(warn_msg, UserWarning)
+            else:
+                if self.prediction_intervals.window_size not in [1, horizon]:
+                    raise ValueError(
+                        "The `window_size` argument of PredictionIntervals "
+                        "should be equal to one or `horizon`. "
+                        "Please rerun the `fit` method passing a proper value "
+                        "to prediction intervals."
+                    )
+                if self.prediction_intervals.window_size != horizon:
+                    warn_msg = (
+                        "Prediction intervals are calculated using 1-step ahead cross-validation, "
+                        "with a constant width for all horizons. To vary the error by horizon, "
+                        "pass PredictionIntervals(window_size=horizon) to the `prediction_intervals` "
+                        "argument when refitting the model."
+                    )
+                    warnings.warn(warn_msg, UserWarning)
+                level_ = sorted(level)
+                model_names = self.models.keys()
+                conformal_method = _get_conformal_method(
+                    self.prediction_intervals.method
+                )
+                forecasts = conformal_method(
+                    forecasts,
+                    self._cs_df,
+                    model_names=list(model_names),
+                    level=level_,
+                    cs_window_size=self.prediction_intervals.window_size,
+                    cs_n_windows=self.prediction_intervals.n_windows,
+                    n_series=self.ts.ga.ngroups,
+                )
+        return forecasts
 
     def cross_validation(
         self,
         data: pd.DataFrame,
         n_windows: int,
         window_size: int,
-        id_col: str,
-        time_col: str,
-        target_col: str,
+        id_col: str = "unique_id",
+        time_col: str = "ds",
+        target_col: str = "y",
         step_size: Optional[int] = None,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
         refit: bool = True,
+        max_horizon: Optional[int] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
+        prediction_intervals: Optional[PredictionIntervals] = None,
+        level: Optional[List[Union[int, float]]] = None,
+        input_size: Optional[int] = None,
     ):
         """Perform time series cross validation.
         Creates `n_windows` splits where each window has `window_size` test periods,
         trains the models, computes the predictions and merges the actuals.
 
         Parameters
         ----------
-        data : dask DataFrame
+        data : pandas DataFrame
             Series data in long format.
         n_windows : int
             Number of windows to evaluate.
         window_size : int
             Number of test periods in each window.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         step_size : int, optional (default=None)
             Step size between each cross validation window. If None it will be equal to `window_size`.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
         dropna : bool (default=True)
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
+        max_horizon: int, optional (default=None)
+            Train this many models, where each model will predict a specific horizon.
         refit : bool (default=True)
             Retrain model for each cross validation window.
             If False, the models are trained at the beginning and then used to predict each window.
         before_predict_callback : callable, optional (default=None)
             Function to call on the features before computing the predictions.
                 This function will take the input dataframe that will be passed to the model for predicting and should return a dataframe with the same structure.
                 The series identifier is on the index.
         after_predict_callback : callable, optional (default=None)
             Function to call on the predictions before updating the targets.
                 This function will take a pandas Series with the predictions and should return another one with the same structure.
                 The series identifier is on the index.
+        prediction_intervals : PredictionIntervals, optional (default=None)
+            Configuration to calibrate prediction intervals (Conformal Prediction).
+        level : list of ints or floats, optional (default=None)
+            Confidence levels between 0 and 100 for prediction intervals.
+        input_size : int, optional (default=None)
+            Maximum training samples per serie in each window. If None, will use an expanding window.
 
         Returns
         -------
-        result : dask DataFrame
+        result : pandas DataFrame
             Predictions for each window with the series id, timestamp, last train date, target value and predictions from each model.
         """
+        if hasattr(self, "models_"):
+            warnings.warn(
+                "Excuting `cross_validation` after `fit` can produce unexpected errors"
+            )
         results = []
         self.cv_models_ = []
-        if id_col != "index":
-            data = data.set_index(id_col)
-
-        def renames(df):
-            mapper = {time_col: "ds", target_col: "y"}
-            df = df.rename(columns=mapper, copy=False)
-            df.index.name = "unique_id"
-            return df
-
-        data = data.map_partitions(renames)
-
-        if np.issubdtype(data["ds"].dtype.type, np.integer):
+        if np.issubdtype(data[time_col].dtype.type, np.integer):
             freq = 1
         else:
             freq = self.freq
 
-        splits = backtest_splits(data, n_windows, window_size, freq, step_size)
-        ex_cols_to_drop = ["y"]
+        splits = backtest_splits(
+            data,
+            n_windows=n_windows,
+            window_size=window_size,
+            id_col=id_col,
+            time_col=time_col,
+            freq=freq,
+            step_size=step_size,
+            input_size=input_size,
+        )
+        ex_cols_to_drop = [id_col, time_col, target_col]
         if static_features is not None:
             ex_cols_to_drop.extend(static_features)
-        has_ex = data.shape[1] > len(ex_cols_to_drop) + 1  # +1 due to time_col
-        for i_window, (train_end, train, valid) in enumerate(splits):
+        has_ex = not data.columns.drop(ex_cols_to_drop).empty
+        for i_window, (cutoffs, train, valid) in enumerate(splits):
             if refit or i_window == 0:
                 self.fit(
-                    train, "index", "ds", "y", static_features, dropna, keep_last_n
+                    train,
+                    id_col=id_col,
+                    time_col=time_col,
+                    target_col=target_col,
+                    static_features=static_features,
+                    dropna=dropna,
+                    keep_last_n=keep_last_n,
+                    max_horizon=max_horizon,
+                    prediction_intervals=prediction_intervals,
                 )
             self.cv_models_.append(self.models_)
-            dynamic_dfs = (
-                [
-                    self.client.compute(
-                        valid.drop(columns=ex_cols_to_drop).reset_index(), sync=True
-                    )
-                ]
-                if has_ex
-                else None
-            )
+            dynamic_dfs = [valid.drop(columns=[target_col])] if has_ex else None
             y_pred = self.predict(
                 window_size,
                 dynamic_dfs,
                 before_predict_callback,
                 after_predict_callback,
                 new_data=train if not refit else None,
+                level=level,
             )
-            result = valid[["ds", "y"]].copy()
-            result["cutoff"] = train_end
-
-            def merge_fn(res, pred):
-                return res.merge(pred, on=["unique_id", "ds"], how="left")
-
-            meta = {**result.dtypes.to_dict(), **y_pred.dtypes.to_dict()}
-            result = result.map_partitions(
-                merge_fn, y_pred, align_dataframes=False, meta=meta
-            )
-            if id_col != "index":
-                result = result.reset_index()
-            result = result.rename(
-                columns={"ds": time_col, "y": target_col, "unique_id": id_col}
+            y_pred = y_pred.merge(cutoffs, on=id_col, how="left")
+            result = valid[[id_col, time_col, target_col]].merge(
+                y_pred, on=[id_col, time_col]
             )
             results.append(result)
-
-        return dd.concat(results)
-
-# %% ../../nbs/distributed.forecast.ipynb 8
-class DistributedForecast(DistributedMLForecast):
-    def __init__(
-        self,
-        models: Models,
-        freq: Optional[Freq] = None,
-        lags: Optional[Lags] = None,
-        lag_transforms: Optional[LagTransforms] = None,
-        date_features: Optional[Iterable[DateFeature]] = None,
-        differences: Optional[Differences] = None,
-        num_threads: int = 1,
-        client: Optional[Client] = None,
-    ):
-        warning_msg = (
-            "The DistributedForecast class is deprecated and will be removed in a future version, "
-            "please use the DistributedMLForecast class instead."
-        )
-        warnings.warn(warning_msg, DeprecationWarning)
-        super().__init__(
-            models,
-            freq,
-            lags,
-            lag_transforms,
-            date_features,
-            differences,
-            num_threads,
-            client,
-        )
+        out = pd.concat(results)
+        cols_order = [id_col, time_col, "cutoff", target_col]
+        return out[cols_order + out.columns.drop(cols_order).tolist()]
```

### Comparing `mlforecast-0.6.0/mlforecast/distributed/models/lgb.py` & `mlforecast-0.7.0/mlforecast/distributed/models/dask/lgb.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/distributed.models.lgb.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../../../nbs/distributed.models.dask.lgb.ipynb.
 
 # %% auto 0
-__all__ = ['LGBMForecast']
+__all__ = ['DaskLGBMForecast']
 
-# %% ../../../nbs/distributed.models.lgb.ipynb 3
+# %% ../../../../nbs/distributed.models.dask.lgb.ipynb 3
 import warnings
 
 import lightgbm as lgb
 
-# %% ../../../nbs/distributed.models.lgb.ipynb 4
-class LGBMForecast(lgb.dask.DaskLGBMRegressor):
+# %% ../../../../nbs/distributed.models.dask.lgb.ipynb 4
+class DaskLGBMForecast(lgb.dask.DaskLGBMRegressor):
     if lgb.__version__ < "3.3.0":
         warnings.warn(
             "It is recommended to install LightGBM version >= 3.3.0, since "
             "the current LightGBM version might be affected by https://github.com/microsoft/LightGBM/issues/4026, "
             "which was fixed in 3.3.0"
         )
```

### Comparing `mlforecast-0.6.0/mlforecast/forecast.py` & `mlforecast-0.7.0/mlforecast/distributed/forecast.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,370 +1,476 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/forecast.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/distributed.forecast.ipynb.
 
 # %% auto 0
-__all__ = ['MLForecast', 'Forecast']
+__all__ = ['DistributedMLForecast']
 
-# %% ../nbs/forecast.ipynb 3
+# %% ../../nbs/distributed.forecast.ipynb 5
 import copy
-import warnings
-from typing import TYPE_CHECKING, Callable, Dict, Iterable, List, Optional, Tuple, Union
+from collections import namedtuple
+from typing import Any, Callable, Iterable, List, Optional
 
-import numpy as np
+import cloudpickle
+
+try:
+    import dask.dataframe as dd
+
+    DASK_INSTALLED = True
+except ModuleNotFoundError:
+    DASK_INSTALLED = False
+import fugue
+import fugue.api as fa
 import pandas as pd
-from sklearn.base import BaseEstimator, clone
+
+try:
+    from pyspark.ml.feature import VectorAssembler
+    from pyspark.sql import DataFrame as SparkDataFrame
+
+    SPARK_INSTALLED = True
+except ModuleNotFoundError:
+    SPARK_INSTALLED = False
+try:
+    from lightgbm_ray import RayDMatrix
+    from ray.data import Dataset as RayDataset
+
+    RAY_INSTALLED = True
+except ModuleNotFoundError:
+    RAY_INSTALLED = False
+from sklearn.base import clone
 
 from mlforecast.core import (
     DateFeature,
-    Differences,
     Freq,
     LagTransforms,
     Lags,
-    Models,
     TimeSeries,
     _name_models,
 )
+from ..utils import single_split
+from ..target_transforms import BaseTargetTransform
 
-if TYPE_CHECKING:
-    from mlforecast.lgb_cv import LightGBMCV
-from .utils import backtest_splits, _cotransform, PredictionIntervals
-
-# %% ../nbs/forecast.ipynb 6
-def _add_conformal_intervals(
-    fcst_df: pd.DataFrame,
-    cs_df: pd.DataFrame,
-    model_names: List[str],
-    level: List[Union[int, float]],
-    cs_n_windows: int,
-    cs_window_size: int,
-) -> pd.DataFrame:
-    """
-    Adds conformal intervals to a `fcst_df` based on conformal scores `cs_df`.
-    `level` should be already sorted.
-    """
-    cuts = [lv / 100 for lv in level]
-    for model in model_names:
-        quantiles = np.quantile(
-            cs_df[model].values.reshape(cs_n_windows, cs_window_size),
-            cuts,
-            axis=0,
-        ).T
-        lo_cols = [f"{model}-lo-{lv}" for lv in reversed(level)]
-        hi_cols = [f"{model}-hi-{lv}" for lv in level]
-        mean = fcst_df[model].values.reshape(-1, 1)
-        fcst_df[lo_cols] = mean - quantiles[:, ::-1]
-        fcst_df[hi_cols] = mean + quantiles
-    return fcst_df
-
-# %% ../nbs/forecast.ipynb 7
-def _schema_conformal_intervals(
-    model_names, level, id_col, time_col, dtypes, fcst_df_columns
-):
-    """Returns schema for conformal intervals."""
-    models_schema = ",".join(f"{model_name}:double" for model_name in model_names)
-    level_schema = ""
-    for model in model_names:
-        level_schema += ","
-        lo_cols = [f"{model}-lo-{lv}:double" for lv in reversed(level)]
-        hi_cols = [f"{model}-hi-{lv}:double" for lv in level]
-        level_schema += ",".join(lo_cols) + "," + ",".join(hi_cols)
-    id_col = id_col if id_col != "index" else fcst_df_columns[0]
-    id_col_type = (
-        dtypes.loc[id_col] if id_col != "index" else dtypes.loc[fcst_df_columns[0]]
-    )
-    if id_col_type == "category":
-        raise NotImplementedError(
-            "Use of `category` type to identify each time series is not yet implemented. "
-            f"Please transform your {id_col} to string to continue."
-        )
-    id_col_type = "string" if id_col_type == "object" else id_col_type
-    ts_col_type = f"{dtypes.loc[time_col]}".replace("64[ns]", "")
-    schema = (
-        f"{id_col}:{id_col_type},{time_col}:{ts_col_type},"
-        + models_schema
-        + level_schema
-    )
-    return schema, id_col
+# %% ../../nbs/distributed.forecast.ipynb 6
+WindowInfo = namedtuple(
+    "WindowInfo", ["n_windows", "window_size", "step_size", "i_window", "input_size"]
+)
+
+# %% ../../nbs/distributed.forecast.ipynb 7
+class DistributedMLForecast:
+    """Multi backend distributed pipeline"""
 
-# %% ../nbs/forecast.ipynb 12
-class MLForecast:
     def __init__(
         self,
-        models: Models,
+        models,
         freq: Optional[Freq] = None,
         lags: Optional[Lags] = None,
         lag_transforms: Optional[LagTransforms] = None,
         date_features: Optional[Iterable[DateFeature]] = None,
-        differences: Optional[Differences] = None,
+        differences: Optional[Iterable[int]] = None,
         num_threads: int = 1,
+        target_transforms: Optional[List[BaseTargetTransform]] = None,
+        engine=None,
+        num_partitions: Optional[int] = None,
     ):
-        """Create forecast object
+        """Create distributed forecast object
 
         Parameters
         ----------
         models : regressor or list of regressors
             Models that will be trained and used to compute the forecasts.
-        freq : str or int or pd.offsets.BaseOffset, optional (default=None)
-            Pandas offset, pandas offset alias, e.g. 'D', 'W-THU' or integer denoting the frequency of the series.
+        freq : str or int, optional (default=None)
+            Pandas offset alias, e.g. 'D', 'W-THU' or integer denoting the frequency of the series.
         lags : list of int, optional (default=None)
             Lags of the target to use as features.
         lag_transforms : dict of int to list of functions, optional (default=None)
             Mapping of target lags to their transformations.
         date_features : list of str or callable, optional (default=None)
             Features computed from the dates. Can be pandas date attributes or functions that will take the dates as input.
         differences : list of int, optional (default=None)
             Differences to take of the target before computing the features. These are restored at the forecasting step.
         num_threads : int (default=1)
             Number of threads to use when computing the features.
+        target_transforms : list of transformers, optional(default=None)
+            Transformations that will be applied to the target before computing the features and restored after the forecasting step.
+        engine : fugue execution engine, optional (default=None)
+            Dask Client, Spark Session, etc to use for the distributed computation.
+            If None will infer depending on the input type.
+        num_partitions: number of data partitions to use, optional (default=None)
+            If None, the default partitions provided by the AnyDataFrame used
+            by the `fit` and `cross_validation` methods will be used. If a Ray
+            Dataset is provided and `num_partitions` is None, the partitioning
+            will be done by the `id_col`.
         """
         if not isinstance(models, dict) and not isinstance(models, list):
             models = [models]
         if isinstance(models, list):
             model_names = _name_models([m.__class__.__name__ for m in models])
             models_with_names = dict(zip(model_names, models))
         else:
             models_with_names = models
         self.models = models_with_names
-        self.ts = TimeSeries(
-            freq, lags, lag_transforms, date_features, differences, num_threads
+        self._base_ts = TimeSeries(
+            freq=freq,
+            lags=lags,
+            lag_transforms=lag_transforms,
+            date_features=date_features,
+            differences=differences,
+            num_threads=num_threads,
+            target_transforms=target_transforms,
         )
+        self.engine = engine
+        self.num_partitions = num_partitions
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f'{self.__class__.__name__}(models=[{", ".join(self.models.keys())}], '
-            f"freq={self.freq}, "
-            f"lag_features={list(self.ts.transforms.keys())}, "
-            f"date_features={self.ts.date_features}, "
-            f"num_threads={self.ts.num_threads})"
+            f"freq={self._base_ts.freq}, "
+            f"lag_features={list(self._base_ts.transforms.keys())}, "
+            f"date_features={self._base_ts.date_features}, "
+            f"num_threads={self._base_ts.num_threads}, "
+            f"engine={self.engine})"
         )
 
-    @property
-    def freq(self):
-        return self.ts.freq
-
-    @classmethod
-    def from_cv(cls, cv: "LightGBMCV") -> "MLForecast":
-        if not hasattr(cv, "best_iteration_"):
-            raise ValueError("LightGBMCV object must be fitted first.")
-        import lightgbm as lgb
+    @staticmethod
+    def _preprocess_partition(
+        part: pd.DataFrame,
+        base_ts: TimeSeries,
+        id_col: str,
+        time_col: str,
+        target_col: str,
+        static_features: Optional[List[str]] = None,
+        dropna: bool = True,
+        keep_last_n: Optional[int] = None,
+        window_info: Optional[WindowInfo] = None,
+        fit_ts_only: bool = False,
+    ) -> List[List[Any]]:
+        ts = copy.deepcopy(base_ts)
+        if fit_ts_only:
+            ts._fit(
+                part,
+                id_col=id_col,
+                time_col=time_col,
+                target_col=target_col,
+                static_features=static_features,
+                keep_last_n=keep_last_n,
+            )
+            return [
+                [
+                    cloudpickle.dumps(ts),
+                    cloudpickle.dumps(None),
+                    cloudpickle.dumps(None),
+                ]
+            ]
+        if window_info is None:
+            train = part
+            valid = None
+        else:
+            max_dates = part.groupby(id_col, observed=True)[time_col].transform("max")
+            cutoffs, train_mask, valid_mask = single_split(
+                part,
+                i_window=window_info.i_window,
+                n_windows=window_info.n_windows,
+                window_size=window_info.window_size,
+                id_col=id_col,
+                time_col=time_col,
+                freq=base_ts.freq,
+                max_dates=max_dates,
+                step_size=window_info.step_size,
+                input_size=window_info.input_size,
+            )
+            train = part[train_mask]
+            valid_keep_cols = part.columns
+            if static_features is not None:
+                valid_keep_cols.drop(static_features)
+            valid = part.loc[valid_mask, valid_keep_cols].merge(cutoffs, on=id_col)
+        transformed = ts.fit_transform(
+            train,
+            id_col=id_col,
+            time_col=time_col,
+            target_col=target_col,
+            static_features=static_features,
+            dropna=dropna,
+            keep_last_n=keep_last_n,
+        )
+        return [
+            [
+                cloudpickle.dumps(ts),
+                cloudpickle.dumps(transformed),
+                cloudpickle.dumps(valid),
+            ]
+        ]
+
+    @staticmethod
+    def _retrieve_df(items: List[List[Any]]) -> Iterable[pd.DataFrame]:
+        for _, serialized_train, _ in items:
+            yield cloudpickle.loads(serialized_train)
 
-        fcst = cls(
-            lgb.LGBMRegressor(**{**cv.params, "n_estimators": cv.best_iteration_})
+    def _preprocess_partitions(
+        self,
+        data: fugue.AnyDataFrame,
+        id_col: str,
+        time_col: str,
+        target_col: str,
+        static_features: Optional[List[str]] = None,
+        dropna: bool = True,
+        keep_last_n: Optional[int] = None,
+        window_info: Optional[WindowInfo] = None,
+        fit_ts_only: bool = False,
+    ) -> List[Any]:
+        if self.num_partitions:
+            partition = dict(by=id_col, num=self.num_partitions, algo="coarse")
+        elif RAY_INSTALLED and isinstance(
+            data, RayDataset
+        ):  # num partitions is None but data is a RayDataset
+            # We need to add this because
+            # currently ray doesnt support partitioning a Dataset
+            # based on a column.
+            # If a Dataset is partitioned using `.repartition(num_partitions)`
+            # we will have akward results.
+            partition = dict(by=id_col)
+        else:
+            partition = None
+        return fa.transform(
+            data,
+            DistributedMLForecast._preprocess_partition,
+            params={
+                "base_ts": self._base_ts,
+                "id_col": id_col,
+                "time_col": time_col,
+                "target_col": target_col,
+                "static_features": static_features,
+                "dropna": dropna,
+                "keep_last_n": keep_last_n,
+                "window_info": window_info,
+                "fit_ts_only": fit_ts_only,
+            },
+            schema="ts:binary,train:binary,valid:binary",
+            engine=self.engine,
+            as_fugue=True,
+            partition=partition,
         )
-        fcst.ts = copy.deepcopy(cv.ts)
-        return fcst
 
-    def preprocess(
+    def _preprocess(
         self,
-        data: pd.DataFrame,
+        data: fugue.AnyDataFrame,
         id_col: str,
         time_col: str,
         target_col: str,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
-        max_horizon: Optional[int] = None,
-        return_X_y: bool = False,
-    ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, Union[pd.Series, pd.DataFrame]]]:
+        window_info: Optional[WindowInfo] = None,
+    ) -> fugue.AnyDataFrame:
+        self.id_col = id_col
+        self.time_col = time_col
+        self.target_col = target_col
+        self.static_features = static_features
+        self.dropna = dropna
+        self.keep_last_n = keep_last_n
+        self.partition_results = self._preprocess_partitions(
+            data=data,
+            id_col=id_col,
+            time_col=time_col,
+            target_col=target_col,
+            static_features=static_features,
+            dropna=dropna,
+            keep_last_n=keep_last_n,
+            window_info=window_info,
+        )
+        base_schema = str(fa.get_schema(data))
+        features_schema = ",".join(f"{feat}:double" for feat in self._base_ts.features)
+        res = fa.transform(
+            self.partition_results,
+            DistributedMLForecast._retrieve_df,
+            schema=f"{base_schema},{features_schema}",
+            engine=self.engine,
+        )
+        return fa.get_native_as_df(res)
+
+    def preprocess(
+        self,
+        data: fugue.AnyDataFrame,
+        id_col: str = "unique_id",
+        time_col: str = "ds",
+        target_col: str = "y",
+        static_features: Optional[List[str]] = None,
+        dropna: bool = True,
+        keep_last_n: Optional[int] = None,
+    ) -> fugue.AnyDataFrame:
         """Add the features to `data`.
 
         Parameters
         ----------
-        data : pandas DataFrame
+        data : dask or spark DataFrame.
             Series data in long format.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
         dropna : bool (default=True)
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
-        max_horizon: int, optional (default=None)
-            Train this many models, where each model will predict a specific horizon.
-        return_X_y: bool (default=False)
-            Return a tuple with the features and the target. If False will return a single dataframe.
 
         Returns
         -------
-        result : pandas DataFrame or tuple of pandas Dataframe and either a pandas Series or a pandas Dataframe (for multi-output regression).
-            `data` plus added features and target(s).
+        result : same type as input
+            data with added features.
         """
-        return self.ts.fit_transform(
+        return self._preprocess(
             data,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             static_features=static_features,
             dropna=dropna,
             keep_last_n=keep_last_n,
-            max_horizon=max_horizon,
-            return_X_y=return_X_y,
         )
 
-    def fit_models(
-        self,
-        X: pd.DataFrame,
-        y: Union[pd.Series, pd.DataFrame],
-    ) -> "MLForecast":
-        """Manually train models. Use this if you called `Forecast.preprocess` beforehand.
-
-        Parameters
-        ----------
-        X : pandas DataFrame
-            Features.
-        y : pandas Series or pandas DataFrame (multi-output).
-            Target.
-
-        Returns
-        -------
-        self : Forecast
-            Forecast object with trained models.
-        """
-        self.models_: Dict[str, Union[BaseEstimator, List[BaseEstimator]]] = {}
-        for name, model in self.models.items():
-            if y.ndim == 2 and y.shape[1] > 1:
-                self.models_[name] = []
-                for col in y:
-                    keep = y[col].notnull()
-                    self.models_[name].append(
-                        clone(model).fit(X.loc[keep], y.loc[keep, col])
-                    )
-            else:
-                self.models_[name] = clone(model).fit(X, y)
-        return self
-
-    def _conformity_scores(
+    def _fit(
         self,
-        data: pd.DataFrame,
+        data: fugue.AnyDataFrame,
         id_col: str,
         time_col: str,
         target_col: str,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
-        max_horizon: Optional[int] = None,
-        n_windows: int = 2,
-        window_size: int = 1,
-    ):
-        """Compute conformity scores.
-
-        We need at least two cross validation errors to compute
-        quantiles for prediction intervals (`n_windows=2`).
-
-        The exception is raised by the PredictionIntervals data class.
-
-        In this simplest case, we assume the width of the interval
-        is the same for all the forecasting horizon (`window_size=1`).
-        """
-        cv_results = self.cross_validation(
-            data=data,
-            n_windows=n_windows,
-            window_size=window_size,
-            refit=False,
+        window_info: Optional[WindowInfo] = None,
+    ) -> "DistributedMLForecast":
+        prep = self._preprocess(
+            data,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             static_features=static_features,
             dropna=dropna,
             keep_last_n=keep_last_n,
-            max_horizon=max_horizon,
-            prediction_intervals=None,
+            window_info=window_info,
         )
-        # conformity score for each model
-        for model in self.models.keys():
-            # compute absolute error for each model
-            cv_results[model] = np.abs(cv_results[model] - cv_results[target_col])
-        if id_col == "index":
-            cv_results = cv_results.reset_index()
-        return cv_results.drop("y", axis=1)
+        features = [
+            x
+            for x in fa.get_column_names(prep)
+            if x not in {id_col, time_col, target_col}
+        ]
+        self.models_ = {}
+        if SPARK_INSTALLED and isinstance(data, SparkDataFrame):
+            featurizer = VectorAssembler(inputCols=features, outputCol="features")
+            train_data = featurizer.transform(prep)[target_col, "features"]
+            for name, model in self.models.items():
+                trained_model = model._pre_fit(target_col).fit(train_data)
+                self.models_[name] = model.extract_local_model(trained_model)
+        elif DASK_INSTALLED and isinstance(data, dd.DataFrame):
+            X, y = prep[features], prep[target_col]
+            for name, model in self.models.items():
+                trained_model = clone(model).fit(X, y)
+                self.models_[name] = trained_model.model_
+        elif RAY_INSTALLED and isinstance(data, RayDataset):
+            X = RayDMatrix(
+                prep.select_columns(cols=features + [target_col]),
+                label=target_col,
+            )
+            for name, model in self.models.items():
+                trained_model = clone(model).fit(X, y=None)
+                self.models_[name] = trained_model.model_
+        else:
+            raise NotImplementedError(
+                "Only spark, dask, and ray engines are supported."
+            )
+        return self
 
     def fit(
         self,
-        data: pd.DataFrame,
-        id_col: str,
-        time_col: str,
-        target_col: str,
+        data: fugue.AnyDataFrame,
+        id_col: str = "unique_id",
+        time_col: str = "ds",
+        target_col: str = "y",
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
-        max_horizon: Optional[int] = None,
-        prediction_intervals: Optional[PredictionIntervals] = None,
-    ) -> "MLForecast":
+    ) -> "DistributedMLForecast":
         """Apply the feature engineering and train the models.
 
         Parameters
         ----------
-        data : pandas DataFrame
+        data : dask or spark DataFrame
             Series data in long format.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
         dropna : bool (default=True)
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
-        max_horizon: int, optional (default=None)
-            Train this many models, where each model will predict a specific horizon.
-        prediction_intervals : PredictionIntervals, optional (default=None)
-            Configuration to calibrate prediction intervals (Conformal Prediction).
 
         Returns
         -------
-        self : Forecast
+        self : DistributedMLForecast
             Forecast object with series values and trained models.
         """
-        self._cs_df: Optional[pd.DataFrame] = None
-        if prediction_intervals is not None:
-            self.prediction_intervals = prediction_intervals
-            self._cs_df = self._conformity_scores(
-                data=data,
-                id_col=id_col,
-                time_col=time_col,
-                target_col=target_col,
-                static_features=static_features,
-                dropna=dropna,
-                keep_last_n=keep_last_n,
-                n_windows=prediction_intervals.n_windows,
-                window_size=prediction_intervals.window_size,
-            )
-        X, y = self.preprocess(
+        return self._fit(
             data,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             static_features=static_features,
             dropna=dropna,
             keep_last_n=keep_last_n,
-            max_horizon=max_horizon,
-            return_X_y=True,
         )
-        features = X.columns.drop(time_col)
-        if id_col != "index" and id_col not in self.ts.static_features:
-            features = features.drop(id_col)
-        X = X[features]
-        return self.fit_models(X, y)
+
+    @staticmethod
+    def _predict(
+        items: List[List[Any]],
+        models,
+        horizon,
+        dynamic_dfs=None,
+        before_predict_callback=None,
+        after_predict_callback=None,
+    ) -> Iterable[pd.DataFrame]:
+        for serialized_ts, _, serialized_valid in items:
+            valid = cloudpickle.loads(serialized_valid)
+            ts = cloudpickle.loads(serialized_ts)
+            if valid is not None:
+                dynamic_features = valid.columns.drop(
+                    [ts.id_col, ts.time_col, ts.target_col]
+                )
+                if not dynamic_features.empty:
+                    dynamic_dfs = [valid.drop(columns=ts.target_col)]
+            res = ts.predict(
+                models=models,
+                horizon=horizon,
+                dynamic_dfs=dynamic_dfs,
+                before_predict_callback=before_predict_callback,
+                after_predict_callback=after_predict_callback,
+            )
+            if valid is not None:
+                res = res.merge(valid, how="left")
+            yield res
+
+    def _get_predict_schema(self) -> str:
+        model_names = self.models.keys()
+        models_schema = ",".join(f"{model_name}:double" for model_name in model_names)
+        schema = f"{self.id_col}:string,{self.time_col}:datetime," + models_schema
+        return schema
 
     def predict(
         self,
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
-        new_data: Optional[pd.DataFrame] = None,
-        level: Optional[List[Union[int, float]]] = None,
-    ) -> pd.DataFrame:
+        new_data: Optional[fugue.AnyDataFrame] = None,
+    ) -> fugue.AnyDataFrame:
         """Compute the predictions for the next `horizon` steps.
 
         Parameters
         ----------
         horizon : int
             Number of periods to predict.
         dynamic_dfs : list of pandas DataFrame, optional (default=None)
@@ -373,254 +479,158 @@
             Function to call on the features before computing the predictions.
                 This function will take the input dataframe that will be passed to the model for predicting and should return a dataframe with the same structure.
                 The series identifier is on the index.
         after_predict_callback : callable, optional (default=None)
             Function to call on the predictions before updating the targets.
                 This function will take a pandas Series with the predictions and should return another one with the same structure.
                 The series identifier is on the index.
-        new_data : pandas DataFrame, optional (default=None)
+        new_data : dask or spark DataFrame, optional (default=None)
             Series data of new observations for which forecasts are to be generated.
                 This dataframe should have the same structure as the one used to fit the model, including any features and time series data.
                 If `new_data` is not None, the method will generate forecasts for the new observations.
-        level : list of ints or floats, optional (default=None)
-            Confidence levels between 0 and 100 for prediction intervals.
 
         Returns
         -------
-        result : pandas DataFrame
+        result : dask, spark or ray DataFrame
             Predictions for each serie and timestep, with one column per model.
         """
-        if not hasattr(self, "models_"):
-            raise ValueError(
-                "No fitted models found. You have to call fit or preprocess + fit_models."
-            )
-
         if new_data is not None:
-            new_ts = TimeSeries(
-                self.ts.freq,
-                self.ts.lags,
-                self.ts.lag_transforms,
-                self.ts.date_features,
-                self.ts.differences,
-                self.ts.num_threads,
+            partition_results = self._preprocess_partitions(
+                data=new_data,
+                id_col=self.id_col,
+                time_col=self.time_col,
+                target_col=self.target_col,
+                static_features=self.static_features,
+                dropna=self.dropna,
+                keep_last_n=self.keep_last_n,
+                fit_ts_only=True,
             )
-            new_ts._fit(
-                new_data,
-                self.ts.id_col,
-                self.ts.time_col,
-                self.ts.target_col,
-                self.ts.static_features.columns,
-                self.ts.keep_last_n,
-            )
-            new_ts.max_horizon = self.ts.max_horizon
-            ts = new_ts
         else:
-            ts = self.ts
-
-        forecasts = ts.predict(
-            self.models_,
-            horizon,
-            dynamic_dfs,
-            before_predict_callback,
-            after_predict_callback,
+            partition_results = self.partition_results
+        schema = self._get_predict_schema()
+        res = fa.transform(
+            partition_results,
+            DistributedMLForecast._predict,
+            params={
+                "models": self.models_,
+                "horizon": horizon,
+                "dynamic_dfs": dynamic_dfs,
+                "before_predict_callback": before_predict_callback,
+                "after_predict_callback": after_predict_callback,
+            },
+            schema=schema,
+            engine=self.engine,
         )
-        if level is not None:
-            if self._cs_df is None:
-                warn_msg = (
-                    "Please rerun the `fit` method passing a proper value "
-                    "to prediction intervals to compute them."
-                )
-                warnings.warn(warn_msg, UserWarning)
-            else:
-                if self.prediction_intervals.window_size not in [1, horizon]:
-                    raise ValueError(
-                        "The `window_size` argument of PredictionIntervals "
-                        "should be equal to one or `horizon`. "
-                        "Please rerun the `fit` method passing a proper value "
-                        "to prediction intervals."
-                    )
-                if self.prediction_intervals.window_size != horizon:
-                    warn_msg = (
-                        "Prediction intervals are calculated using 1-step ahead cross-validation, "
-                        "with a constant width for all horizons. To vary the error by horizon, "
-                        "pass PredictionIntervals(window_size=horizon) to the `prediction_intervals` "
-                        "argument when refitting the model."
-                    )
-                    warnings.warn(warn_msg, UserWarning)
-                level_ = sorted(level)
-                model_names = self.models.keys()
-                if ts.id_col == "index":
-                    forecasts = forecasts.reset_index()
-                dtypes = forecasts.dtypes
-                schema, id_col = _schema_conformal_intervals(
-                    model_names=model_names,
-                    level=level_,
-                    id_col=ts.id_col,
-                    time_col=ts.time_col,
-                    dtypes=dtypes,
-                    fcst_df_columns=forecasts.columns,
-                )
-                forecasts = _cotransform(
-                    forecasts,
-                    self._cs_df,
-                    using=_add_conformal_intervals,
-                    params=dict(
-                        model_names=list(model_names),
-                        level=level_,
-                        cs_window_size=self.prediction_intervals.window_size,
-                        cs_n_windows=self.prediction_intervals.n_windows,
-                    ),
-                    schema=schema,
-                    partition=id_col,
-                )
-                if ts.id_col == "index":
-                    forecasts = forecasts.set_index(forecasts.columns[0])
-        return forecasts
+        return fa.get_native_as_df(res)
 
     def cross_validation(
         self,
-        data: pd.DataFrame,
+        data: fugue.AnyDataFrame,
         n_windows: int,
         window_size: int,
-        id_col: str,
-        time_col: str,
-        target_col: str,
+        id_col: str = "unique_id",
+        time_col: str = "ds",
+        target_col: str = "y",
         step_size: Optional[int] = None,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
         refit: bool = True,
-        max_horizon: Optional[int] = None,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
-        prediction_intervals: Optional[PredictionIntervals] = None,
-        level: Optional[List[Union[int, float]]] = None,
-    ):
+        input_size: Optional[int] = None,
+    ) -> fugue.AnyDataFrame:
         """Perform time series cross validation.
         Creates `n_windows` splits where each window has `window_size` test periods,
         trains the models, computes the predictions and merges the actuals.
 
         Parameters
         ----------
-        data : pandas DataFrame
+        data : dask, spark or ray DataFrame
             Series data in long format.
         n_windows : int
             Number of windows to evaluate.
         window_size : int
             Number of test periods in each window.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         step_size : int, optional (default=None)
             Step size between each cross validation window. If None it will be equal to `window_size`.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
         dropna : bool (default=True)
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
-        max_horizon: int, optional (default=None)
-            Train this many models, where each model will predict a specific horizon.
         refit : bool (default=True)
             Retrain model for each cross validation window.
             If False, the models are trained at the beginning and then used to predict each window.
         before_predict_callback : callable, optional (default=None)
             Function to call on the features before computing the predictions.
                 This function will take the input dataframe that will be passed to the model for predicting and should return a dataframe with the same structure.
                 The series identifier is on the index.
         after_predict_callback : callable, optional (default=None)
             Function to call on the predictions before updating the targets.
                 This function will take a pandas Series with the predictions and should return another one with the same structure.
                 The series identifier is on the index.
-        prediction_intervals : PredictionIntervals, optional (default=None)
-            Configuration to calibrate prediction intervals (Conformal Prediction).
-        level : list of ints or floats, optional (default=None)
-            Confidence levels between 0 and 100 for prediction intervals.
+        input_size : int, optional (default=None)
+            Maximum training samples per serie in each window. If None, will use an expanding window.
 
         Returns
         -------
-        result : pandas DataFrame
-            Predictions for each window with the series id, timestamp, last train date, target value and predictions from each model.
+        result : dask, spark or ray DataFrame
+            Predictions for each window with the series id, timestamp, target value and predictions from each model.
         """
-        if hasattr(self, "models_"):
-            warnings.warn(
-                "Excuting `cross_validation` after `fit` can produce unexpected errors"
-            )
-        results = []
         self.cv_models_ = []
-        if id_col != "index":
-            data = data.set_index(id_col)
-
-        if np.issubdtype(data[time_col].dtype.type, np.integer):
-            freq = 1
-        else:
-            freq = self.freq
-
-        splits = backtest_splits(
-            data, n_windows, window_size, freq, step_size, time_col
-        )
-        ex_cols_to_drop = [target_col]
-        if static_features is not None:
-            ex_cols_to_drop.extend(static_features)
-        has_ex = data.shape[1] > len(ex_cols_to_drop) + 1  # +1 due to time_col
-        for i_window, (train_end, train, valid) in enumerate(splits):
-            if refit or i_window == 0:
-                self.fit(
-                    train,
-                    id_col="index",
+        results = []
+        for i in range(n_windows):
+            window_info = WindowInfo(n_windows, window_size, step_size, i, input_size)
+            if refit or i == 0:
+                self._fit(
+                    data,
+                    id_col=id_col,
+                    time_col=time_col,
+                    target_col=target_col,
+                    static_features=static_features,
+                    dropna=dropna,
+                    keep_last_n=keep_last_n,
+                    window_info=window_info,
+                )
+                self.cv_models_.append(self.models_)
+                partition_results = self.partition_results
+            elif not refit:
+                partition_results = self._preprocess_partitions(
+                    data=data,
+                    id_col=id_col,
                     time_col=time_col,
                     target_col=target_col,
                     static_features=static_features,
                     dropna=dropna,
                     keep_last_n=keep_last_n,
-                    max_horizon=max_horizon,
-                    prediction_intervals=prediction_intervals,
+                    window_info=window_info,
                 )
-            self.cv_models_.append(self.models_)
-            # reset index of valid to be compatible
-            # with _get_features_for_next_step
-            dynamic_dfs = (
-                [valid.drop(columns=ex_cols_to_drop).reset_index()] if has_ex else None
+            schema = (
+                self._get_predict_schema()
+                + f",cutoff:datetime,{self.target_col}:double"
             )
-            y_pred = self.predict(
-                window_size,
-                dynamic_dfs,
-                before_predict_callback,
-                after_predict_callback,
-                new_data=train if not refit else None,
-                level=level,
+            preds = fa.transform(
+                partition_results,
+                DistributedMLForecast._predict,
+                params={
+                    "models": self.models_,
+                    "horizon": window_size,
+                    "before_predict_callback": before_predict_callback,
+                    "after_predict_callback": after_predict_callback,
+                },
+                schema=schema,
+                engine=self.engine,
             )
-            y_pred = y_pred.set_index(time_col, append=True)
-            result = valid.set_index(time_col, append=True)[[target_col]].copy()
-            result = result.join(y_pred).reset_index(time_col)
-            result["cutoff"] = train_end
-            results.append(result)
-
-        out = pd.concat(results)
-        out = out[[time_col, "cutoff", target_col, *y_pred.columns]]
-        if id_col != "index":
-            out = out.reset_index()
-        return out
-
-# %% ../nbs/forecast.ipynb 15
-class Forecast(MLForecast):
-    def __init__(
-        self,
-        models: Models,
-        freq: Optional[Freq] = None,
-        lags: Optional[Lags] = None,
-        lag_transforms: Optional[LagTransforms] = None,
-        date_features: Optional[Iterable[DateFeature]] = None,
-        differences: Optional[Differences] = None,
-        num_threads: int = 1,
-    ):
-        warning_msg = (
-            "The Forecast class is deprecated and will be removed in a future version, "
-            "please use the MLForecast class instead."
-        )
-        warnings.warn(warning_msg, DeprecationWarning)
-        super().__init__(
-            models, freq, lags, lag_transforms, date_features, differences, num_threads
-        )
+            results.append(fa.get_native_as_df(preds))
+        if len(results) == 1:
+            return results[0]
+        if len(results) == 2:
+            return fa.union(results[0], results[1])
+        return fa.union(results[0], results[1], results[2:])
```

### Comparing `mlforecast-0.6.0/mlforecast/lgb_cv.py` & `mlforecast-0.7.0/mlforecast/lgb_cv.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 import lightgbm as lgb
 import numpy as np
 import pandas as pd
 
 from mlforecast.core import (
     DateFeature,
-    Differences,
     Freq,
     LagTransforms,
     Lags,
     TimeSeries,
 )
 from .utils import backtest_splits
+from .target_transforms import BaseTargetTransform
 
 # %% ../nbs/lgb_cv.ipynb 5
 def _mape(y_true, y_pred):
     abs_pct_err = abs(y_true - y_pred) / y_true
     return (
         abs_pct_err.groupby(y_true.index.get_level_values(0), observed=True)
         .mean()
@@ -53,46 +53,49 @@
 
 
 def _predict(
     ts,
     bst,
     valid,
     h,
+    id_col,
     time_col,
     dynamic_dfs,
     before_predict_callback,
     after_predict_callback,
 ):
     preds = ts.predict(
         {"Booster": bst},
         h,
         dynamic_dfs,
         before_predict_callback,
         after_predict_callback,
-    ).set_index(time_col, append=True)
-    return valid.join(preds)
+    )
+    return valid.merge(preds, on=[id_col, time_col], how="left")
 
 
 def _update_and_predict(
     ts,
     bst,
     valid,
     n,
     h,
+    id_col,
     time_col,
     dynamic_dfs,
     before_predict_callback,
     after_predict_callback,
 ):
     _update(bst, n)
     return _predict(
         ts,
         bst,
         valid,
         h,
+        id_col,
         time_col,
         dynamic_dfs,
         before_predict_callback,
         after_predict_callback,
     )
 
 # %% ../nbs/lgb_cv.ipynb 6
@@ -102,16 +105,17 @@
 class LightGBMCV:
     def __init__(
         self,
         freq: Optional[Freq] = None,
         lags: Optional[Lags] = None,
         lag_transforms: Optional[LagTransforms] = None,
         date_features: Optional[Iterable[DateFeature]] = None,
-        differences: Optional[Differences] = None,
+        differences: Optional[Iterable[int]] = None,
         num_threads: int = 1,
+        target_transforms: Optional[List[BaseTargetTransform]] = None,
     ):
         """Create LightGBM CV object.
 
         Parameters
         ----------
         freq : str or int, optional (default=None)
             Pandas offset alias, e.g. 'D', 'W-THU' or integer denoting the frequency of the series.
@@ -121,24 +125,32 @@
             Mapping of target lags to their transformations.
         date_features : list of str or callable, optional (default=None)
             Features computed from the dates. Can be pandas date attributes or functions that will take the dates as input.
         differences : list of int, optional (default=None)
             Differences to take of the target before computing the features. These are restored at the forecasting step.
         num_threads : int (default=1)
             Number of threads to use when computing the features.
+        target_transforms : list of transformers, optional(default=None)
+            Transformations that will be applied to the target before computing the features and restored after the forecasting step.
         """
         self.num_threads = num_threads
         cpu_count = os.cpu_count()
         if cpu_count is None:
             num_cpus = 1
         else:
             num_cpus = cpu_count
         self.bst_threads = max(num_cpus // num_threads, 1)
         self.ts = TimeSeries(
-            freq, lags, lag_transforms, date_features, differences, self.bst_threads
+            freq=freq,
+            lags=lags,
+            lag_transforms=lag_transforms,
+            date_features=date_features,
+            differences=differences,
+            num_threads=self.bst_threads,
+            target_transforms=target_transforms,
         )
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}("
             f"freq={self.ts.freq}, "
             f"lag_features={list(self.ts.transforms.keys())}, "
@@ -148,40 +160,41 @@
         )
 
     def setup(
         self,
         data: pd.DataFrame,
         n_windows: int,
         window_size: int,
-        id_col: str,
-        time_col: str,
-        target_col: str,
+        id_col: str = "unique_id",
+        time_col: str = "ds",
+        target_col: str = "y",
         step_size: Optional[int] = None,
         params: Optional[Dict[str, Any]] = None,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
         weights: Optional[Sequence[float]] = None,
         metric: Union[str, Callable] = "mape",
+        input_size: Optional[int] = None,
     ):
         """Initialize internal data structures to iteratively train the boosters. Use this before calling partial_fit.
 
         Parameters
         ----------
         data : pandas DataFrame
             Series data in long format.
         n_windows : int
             Number of windows to evaluate.
         window_size : int
             Number of test periods in each window.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         step_size : int, optional (default=None)
             Step size between each cross validation window. If None it will be equal to `window_size`.
         params : dict, optional(default=None)
             Parameters to be passed to the LightGBM Boosters.
         static_features : list of str, optional (default=None)
             Names of the features that are static and will be repeated when forecasting.
@@ -189,14 +202,16 @@
             Drop rows with missing values produced by the transformations.
         keep_last_n : int, optional (default=None)
             Keep only these many records from each serie for the forecasting step. Can save time and memory if your features allow it.
         weights : sequence of float, optional (default=None)
             Weights to multiply the metric of each window. If None, all windows have the same weight.
         metric : str or callable, default='mape'
             Metric used to assess the performance of the models and perform early stopping.
+        input_size : int, optional (default=None)
+            Maximum training samples per serie in each window. If None, will use an expanding window.
 
         Returns
         -------
         self : LightGBMCV
             CV object with internal data structures for partial_fit.
         """
         if weights is None:
@@ -211,42 +226,47 @@
         else:
             if metric not in _metric2fn:
                 raise ValueError(
                     f'{metric} is not one of the implemented metrics: ({", ".join(_metric2fn.keys())})'
                 )
             self.metric_fn = _metric2fn[metric]
             self.metric_name = metric
-
-        if id_col != "index":
-            data = data.set_index(id_col)
-
         if np.issubdtype(data[time_col].dtype.type, np.integer):
             freq = 1
         else:
             freq = self.ts.freq
         self.items = []
         self.window_size = window_size
+        self.id_col = id_col
         self.time_col = time_col
         self.target_col = target_col
         self.params = {} if params is None else params
-        for _, train, valid in backtest_splits(
-            data, n_windows, window_size, freq, step_size, time_col
-        ):
+        splits = backtest_splits(
+            data,
+            n_windows=n_windows,
+            window_size=window_size,
+            id_col=id_col,
+            time_col=time_col,
+            freq=freq,
+            step_size=step_size,
+            input_size=input_size,
+        )
+        for _, train, valid in splits:
             ts = copy.deepcopy(self.ts)
             prep = ts.fit_transform(
                 train,
-                "index",
+                id_col,
                 time_col,
                 target_col,
                 static_features,
                 dropna,
                 keep_last_n,
             )
             ds = lgb.Dataset(
-                prep.drop(columns=[time_col, target_col]), prep[target_col]
+                prep.drop(columns=[id_col, time_col, target_col]), prep[target_col]
             ).construct()
             bst = lgb.Booster({**self.params, "num_threads": self.bst_threads}, ds)
             bst.predict = partial(bst.predict, num_threads=self.bst_threads)
             valid = valid.set_index(time_col, append=True)
             self.items.append((ts, bst, valid))
         return self
 
@@ -256,23 +276,24 @@
         num_iterations,
         dynamic_dfs,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
     ):
         for j, (ts, bst, valid) in enumerate(self.items):
             preds = _update_and_predict(
-                ts,
-                bst,
-                valid,
-                num_iterations,
-                self.window_size,
-                self.time_col,
-                dynamic_dfs,
-                before_predict_callback,
-                after_predict_callback,
+                ts=ts,
+                bst=bst,
+                valid=valid,
+                n=num_iterations,
+                h=self.window_size,
+                id_col=self.id_col,
+                time_col=self.time_col,
+                dynamic_dfs=dynamic_dfs,
+                before_predict_callback=before_predict_callback,
+                after_predict_callback=after_predict_callback,
             )
             metric_values[j] = self.metric_fn(preds[self.target_col], preds["Booster"])
 
     def _multithreaded_partial_fit(
         self,
         metric_values,
         num_iterations,
@@ -282,22 +303,23 @@
     ):
         with ThreadPoolExecutor(self.num_threads) as executor:
             futures = []
             for ts, bst, valid in self.items:
                 _update(bst, num_iterations)
                 future = executor.submit(
                     _predict,
-                    ts,
-                    bst,
-                    valid,
-                    self.window_size,
-                    self.time_col,
-                    dynamic_dfs,
-                    before_predict_callback,
-                    after_predict_callback,
+                    ts=ts,
+                    bst=bst,
+                    valid=valid,
+                    h=self.window_size,
+                    id_col=self.id_col,
+                    time_col=self.time_col,
+                    dynamic_dfs=dynamic_dfs,
+                    before_predict_callback=before_predict_callback,
+                    after_predict_callback=after_predict_callback,
                 )
                 futures.append(future)
             cv_preds = [f.result() for f in futures]
         metric_values[:] = [
             self.metric_fn(preds[self.target_col], preds["Booster"])
             for preds in cv_preds
         ]
@@ -365,17 +387,17 @@
         return best_iter
 
     def fit(
         self,
         data: pd.DataFrame,
         n_windows: int,
         window_size: int,
-        id_col: str,
-        time_col: str,
-        target_col: str,
+        id_col: str = "unique_id",
+        time_col: str = "ds",
+        target_col: str = "y",
         step_size: Optional[int] = None,
         num_iterations: int = 100,
         params: Optional[Dict[str, Any]] = None,
         static_features: Optional[List[str]] = None,
         dropna: bool = True,
         keep_last_n: Optional[int] = None,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
@@ -384,30 +406,31 @@
         metric: Union[str, Callable] = "mape",
         verbose_eval: bool = True,
         early_stopping_evals: int = 2,
         early_stopping_pct: float = 0.01,
         compute_cv_preds: bool = False,
         before_predict_callback: Optional[Callable] = None,
         after_predict_callback: Optional[Callable] = None,
+        input_size: Optional[int] = None,
     ) -> List[CVResult]:
         """Train boosters simultaneously and assess their performance on the complete forecasting window.
 
         Parameters
         ----------
         data : pandas DataFrame
             Series data in long format.
         n_windows : int
             Number of windows to evaluate.
         window_size : int
             Number of test periods in each window.
-        id_col : str
-            Column that identifies each serie. If 'index' then the index is used.
-        time_col : str
+        id_col : str (default='unique_id')
+            Column that identifies each serie.
+        time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
-        target_col : str
+        target_col : str (default='y')
             Column that contains the target.
         step_size : int, optional (default=None)
             Step size between each cross validation window. If None it will be equal to `window_size`.
         num_iterations : int (default=100)
             Maximum number of boosting iterations to run.
         params : dict, optional(default=None)
             Parameters to be passed to the LightGBM Boosters.
@@ -437,28 +460,31 @@
             Function to call on the features before computing the predictions.
                 This function will take the input dataframe that will be passed to the model for predicting and should return a dataframe with the same structure.
                 The series identifier is on the index.
         after_predict_callback : callable, optional (default=None)
             Function to call on the predictions before updating the targets.
                 This function will take a pandas Series with the predictions and should return another one with the same structure.
                 The series identifier is on the index.
+        input_size : int, optional (default=None)
+            Maximum training samples per serie in each window. If None, will use an expanding window.
 
         Returns
         -------
         cv_result : list of tuple.
             List of (boosting rounds, metric value) tuples.
         """
         self.setup(
             data=data,
             n_windows=n_windows,
             window_size=window_size,
             params=params,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
+            input_size=input_size,
             step_size=step_size,
             static_features=static_features,
             dropna=dropna,
             keep_last_n=keep_last_n,
             weights=weights,
             metric=metric,
         )
@@ -483,32 +509,28 @@
         self.cv_models_ = {f"Booster{i}": item[1] for i, item in enumerate(self.items)}
         if compute_cv_preds:
             with ThreadPoolExecutor(self.num_threads) as executor:
                 futures = []
                 for ts, bst, valid in self.items:
                     future = executor.submit(
                         _predict,
-                        ts,
-                        bst,
-                        valid,
-                        window_size,
-                        time_col,
-                        dynamic_dfs,
-                        before_predict_callback,
-                        after_predict_callback,
+                        ts=ts,
+                        bst=bst,
+                        valid=valid,
+                        h=self.window_size,
+                        id_col=self.id_col,
+                        time_col=self.time_col,
+                        dynamic_dfs=dynamic_dfs,
+                        before_predict_callback=before_predict_callback,
+                        after_predict_callback=after_predict_callback,
                     )
                     futures.append(future)
-                cv_preds = pd.concat(
+                self.cv_preds_ = pd.concat(
                     [f.result().assign(window=i) for i, f in enumerate(futures)]
                 )
-                if id_col != "index":
-                    idxs = [id_col, time_col]
-                else:
-                    idxs = [time_col]
-                self.cv_preds_ = cv_preds.reset_index(idxs)
         self.ts._fit(data, id_col, time_col, target_col, static_features, keep_last_n)
         return hist
 
     def predict(
         self,
         horizon: int,
         dynamic_dfs: Optional[List[pd.DataFrame]] = None,
```

### Comparing `mlforecast-0.6.0/mlforecast.egg-info/PKG-INFO` & `mlforecast-0.7.0/mlforecast.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforecast
-Version: 0.6.0
+Version: 0.7.0
 Summary: Scalable machine learning based time series forecasting
 Home-page: https://github.com/Nixtla/mlforecast
 Author: José Morales
 Author-email: jmoralz92@gmail.com
 License: Apache Software License 2.0
 Keywords: python forecast forecasting machine-learning dask
 Classifier: Development Status :: 4 - Beta
@@ -18,25 +18,45 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: distributed
 Provides-Extra: dev
 License-File: LICENSE
 
-mlforecast
+Nixtla  
+[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting)
+ ![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+<div align="center">
+
+<center>
+<img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
+</center>
+<h1 align="center">
+Machine Learning 🤖 Forecast
+</h1>
+<h3 align="center">
+Scalable machine learning for time series forecasting
+</h3>
+
 [![CI](https://github.com/Nixtla/mlforecast/actions/workflows/ci.yaml/badge.svg)](https://github.com/Nixtla/mlforecast/actions/workflows/ci.yaml)
 [![Python](https://img.shields.io/pypi/pyversions/mlforecast.png)](https://pypi.org/project/mlforecast/)
 [![PyPi](https://img.shields.io/pypi/v/mlforecast?color=blue.png)](https://pypi.org/project/mlforecast/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/mlforecast?color=blue.png)](https://anaconda.org/conda-forge/mlforecast)
 [![License](https://img.shields.io/github/license/Nixtla/mlforecast.png)](https://github.com/Nixtla/mlforecast/blob/main/LICENSE)
 
+**mlforecast** is a framework to perform time series forecasting using
+machine learning models, with the option to scale to massive amounts of
+data using remote clusters.
+
+</div>
+
 ## Install
 
 ### PyPI
 
 `pip install mlforecast`
 
 If you want to perform distributed training, you can instead use
@@ -53,14 +73,90 @@
 Note that this installation comes with the required dependencies for the
 local interface. If you want to perform distributed training, you must
 install dask (`conda install -c conda-forge dask`) and either
 [LightGBM](https://github.com/microsoft/LightGBM/tree/master/python-package)
 or
 [XGBoost](https://xgboost.readthedocs.io/en/latest/install.html#python).
 
+## Quick Start
+
+**Minimal Example**
+
+``` python
+import lightgbm as lgb
+
+from mlforecast import MLForecast
+from sklearn.linear_model import LinearRegression
+
+mlf = MLForecast(
+    models = [LinearRegression(), lgb.LGBMRegressor()],
+    lags=[1, 12],
+    freq = 'M'
+)
+mlf.fit(df)
+mlf.predict(12)
+```
+
+**Get Started with this [quick
+guide](https://nixtla.github.io/mlforecast/docs/quick_start_local.html).**
+
+**Follow this [end-to-end
+walkthrough](https://nixtla.github.io/mlforecast/docs/end_to_end_walkthrough.html)
+for best practices.**
+
+## Why?
+
+Current Python alternatives for machine learning models are slow,
+inaccurate and don’t scale well. So we created a library that can be
+used to forecast in production environments. `MLForecast` includes
+efficient feature engineering to train any machine learning model (with
+`fit` and `predict` methods such as
+[`sklearn`](https://scikit-learn.org/stable/)) to fit millions of time
+series.
+
+## Features
+
+- Fastest implementations of feature engineering for time series
+  forecasting in Python.
+- Out-of-the-box compatibility with Spark, Dask, and Ray.
+- Probabilistic Forecasting with Conformal Prediction.
+- Support for exogenous variables and static covariates.
+- Familiar `sklearn` syntax: `.fit` and `.predict`.
+
+Missing something? Please open an issue or write us in
+[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white.png)](https://join.slack.com/t/nixtlaworkspace/shared_invite/zt-135dssye9-fWTzMpv2WBthq8NK0Yvu6A)
+
+## Examples and Guides
+
+📚 [End to End
+Walkthrough](https://nixtla.github.io/mlforecast/docs/end_to_end_walkthrough.html):
+model training, evaluation and selection for multiple time series.
+
+🔎 [Probabilistic
+Forecasting](https://nixtla.github.io/mlforecast/docs/prediction_intervals.html):
+use Conformal Prediction to produce prediciton intervals.
+
+👩‍🔬 [Cross
+Validation](https://nixtla.github.io/mlforecast/docs/cross_validation.html):
+robust model’s performance evaluation.
+
+🔌 [Predict Demand
+Peaks](https://nixtla.github.io/mlforecast/docs/electricity_peak_forecasting.html):
+electricity load forecasting for detecting daily peaks and reducing
+electric bills.
+
+📈 [Transfer
+Learning](https://nixtla.github.io/mlforecast/docs/transfer_learning.html):
+pretrain a model using a set of time series and then predict another one
+using that pretrained model.
+
+🌡️ [Distributed
+Training](https://nixtla.github.io/mlforecast/docs/quick_start_distributed.html):
+use a Dask cluster to train models at scale.
+
 ## How to use
 
 The following provides a very basic overview, for a more detailed
 description see the
 [documentation](https://nixtla.github.io/mlforecast/).
 
 ### Data setup
@@ -82,52 +178,52 @@
 ```
 
 <div>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
+      <th>unique_id</th>
       <th>ds</th>
       <th>y</th>
       <th>static_0</th>
     </tr>
-    <tr>
-      <th>unique_id</th>
-      <th></th>
-      <th></th>
-      <th></th>
-    </tr>
   </thead>
   <tbody>
     <tr>
-      <th>id_00</th>
+      <th>0</th>
+      <td>id_00</td>
       <td>2000-01-01</td>
       <td>1.751917</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>1</th>
+      <td>id_00</td>
       <td>2000-01-02</td>
       <td>9.196715</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>2</th>
+      <td>id_00</td>
       <td>2000-01-03</td>
       <td>18.577788</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>3</th>
+      <td>id_00</td>
       <td>2000-01-04</td>
       <td>24.520646</td>
       <td>72</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>4</th>
+      <td>id_00</td>
       <td>2000-01-05</td>
       <td>33.418028</td>
       <td>72</td>
     </tr>
   </tbody>
 </table>
 </div>
@@ -159,14 +255,15 @@
 array, if they have additional arguments you can either supply a tuple
 (`transform_func`, `arg1`, `arg2`, …) or define new functions fixing the
 arguments. You can also define differences to apply to the series before
 fitting that will be restored when predicting.
 
 ``` python
 from mlforecast import MLForecast
+from mlforecast.target_transforms import Differences
 from numba import njit
 from window_ops.expanding import expanding_mean
 from window_ops.rolling import rolling_mean
 
 
 @njit
 def rolling_mean_28(x):
@@ -178,36 +275,28 @@
     freq='D',
     lags=[7, 14],
     lag_transforms={
         1: [expanding_mean],
         7: [rolling_mean_28]
     },
     date_features=['dayofweek'],
-    differences=[1],
+    target_transforms=[Differences([1])],
 )
 ```
 
 ### Training
 
 To compute the features and train the models call `fit` on your
-`Forecast` object. Here you have to specify the columns that:
-
-- Identify each serie (`id_col`). If the series identifier is the index
-  you can specify `id_col='index'`
-- Contain the timestamps (`time_col`). Can also be integers if your data
-  doesn’t have timestamps.
-- Are the series values (`target_col`)
-- Are static (`static_features`). These are features that don’t change
-  over time and can be repeated when predicting.
+`Forecast` object.
 
 ``` python
-fcst.fit(series, id_col='index', time_col='ds', target_col='y', static_features=['static_0'])
+fcst.fit(series)
 ```
 
-    MLForecast(models=[LGBMRegressor, XGBRegressor, RandomForestRegressor], freq=<Day>, lag_features=['lag-7', 'lag-14', 'expanding_mean_lag-1', 'rolling_mean_28_lag-7'], date_features=['dayofweek'], num_threads=1)
+    MLForecast(models=[LGBMRegressor, XGBRegressor, RandomForestRegressor], freq=<Day>, lag_features=['lag7', 'lag14', 'expanding_mean_lag1', 'rolling_mean_28_lag7'], date_features=['dayofweek'], num_threads=1)
 
 ### Predicting
 
 To get the forecasts for the next `n` days call `predict(n)` on the
 forecast object. This will automatically handle the updates required by
 the features using a recursive strategy.
 
@@ -217,120 +306,126 @@
 ```
 
 <div>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
+      <th>unique_id</th>
       <th>ds</th>
       <th>LGBMRegressor</th>
       <th>XGBRegressor</th>
       <th>RandomForestRegressor</th>
     </tr>
-    <tr>
-      <th>unique_id</th>
-      <th></th>
-      <th></th>
-      <th></th>
-      <th></th>
-    </tr>
   </thead>
   <tbody>
     <tr>
-      <th>id_00</th>
+      <th>0</th>
+      <td>id_00</td>
       <td>2000-04-04</td>
       <td>69.082830</td>
       <td>67.761337</td>
-      <td>68.184016</td>
+      <td>68.226556</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>1</th>
+      <td>id_00</td>
       <td>2000-04-05</td>
       <td>75.706024</td>
       <td>74.588699</td>
-      <td>75.470680</td>
+      <td>75.484774</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>2</th>
+      <td>id_00</td>
       <td>2000-04-06</td>
       <td>82.222473</td>
       <td>81.058289</td>
-      <td>82.846249</td>
+      <td>82.853684</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>3</th>
+      <td>id_00</td>
       <td>2000-04-07</td>
       <td>89.577638</td>
       <td>88.735947</td>
-      <td>90.201271</td>
+      <td>90.351212</td>
     </tr>
     <tr>
-      <th>id_00</th>
+      <th>4</th>
+      <td>id_00</td>
       <td>2000-04-08</td>
       <td>44.149095</td>
       <td>44.981384</td>
-      <td>46.096322</td>
+      <td>46.291173</td>
     </tr>
     <tr>
       <th>...</th>
       <td>...</td>
       <td>...</td>
       <td>...</td>
       <td>...</td>
+      <td>...</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>275</th>
+      <td>id_19</td>
       <td>2000-03-23</td>
-      <td>30.236012</td>
-      <td>31.949095</td>
-      <td>32.656369</td>
+      <td>30.151270</td>
+      <td>31.814825</td>
+      <td>32.592799</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>276</th>
+      <td>id_19</td>
       <td>2000-03-24</td>
-      <td>31.308269</td>
-      <td>32.765919</td>
-      <td>33.624488</td>
+      <td>31.418104</td>
+      <td>32.653374</td>
+      <td>33.563294</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>277</th>
+      <td>id_19</td>
       <td>2000-03-25</td>
-      <td>32.788550</td>
-      <td>33.628864</td>
-      <td>34.581486</td>
+      <td>32.843567</td>
+      <td>33.586033</td>
+      <td>34.530912</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>278</th>
+      <td>id_19</td>
       <td>2000-03-26</td>
-      <td>34.086976</td>
-      <td>34.508457</td>
-      <td>35.553173</td>
+      <td>34.127210</td>
+      <td>34.541473</td>
+      <td>35.507559</td>
     </tr>
     <tr>
-      <th>id_19</th>
+      <th>279</th>
+      <td>id_19</td>
       <td>2000-03-27</td>
-      <td>34.288968</td>
-      <td>35.411613</td>
-      <td>36.526505</td>
+      <td>34.329202</td>
+      <td>35.450943</td>
+      <td>36.425001</td>
     </tr>
   </tbody>
 </table>
-<p>280 rows × 4 columns</p>
+<p>280 rows × 5 columns</p>
 </div>
 
 ### Visualize results
 
 ``` python
 import matplotlib.pyplot as plt
 import pandas as pd
 
 fig, ax = plt.subplots(nrows=2, ncols=2, figsize=(12, 6), gridspec_kw=dict(hspace=0.3))
-for i, (cat, axi) in enumerate(zip(series.index.categories, ax.flat)):
-    pd.concat([series.loc[cat, ['ds', 'y']], predictions.loc[cat]]).set_index('ds').plot(ax=axi)
-    axi.set(title=cat, xlabel=None)
+for i, (uid, axi) in enumerate(zip(series['unique_id'].unique(), ax.flat)):
+    fltr = lambda df: df['unique_id'].eq(uid)
+    pd.concat([series.loc[fltr, ['ds', 'y']], predictions.loc[fltr]]).set_index('ds').plot(ax=axi)
+    axi.set(title=uid, xlabel=None)
     if i % 2 == 0:
         axi.legend().remove()
     else:
         axi.legend(bbox_to_anchor=(1.01, 1.0))
 fig.savefig('figs/index.png', bbox_inches='tight')
 plt.close()
 ```
@@ -338,7 +433,12 @@
 ![](https://raw.githubusercontent.com/Nixtla/mlforecast/main/figs/index.png)
 
 ## Sample notebooks
 
 - [m5](https://www.kaggle.com/code/lemuz90/m5-mlforecast-eval)
 - [m4](https://www.kaggle.com/code/lemuz90/m4-competition)
 - [m4-cv](https://www.kaggle.com/code/lemuz90/m4-competition-cv)
+
+## How to contribute
+
+See
+[CONTRIBUTING.md](https://github.com/Nixtla/mlforecast/blob/main/CONTRIBUTING.md).
```

### Comparing `mlforecast-0.6.0/mlforecast.egg-info/SOURCES.txt` & `mlforecast-0.7.0/mlforecast.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,31 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 mlforecast/__init__.py
 mlforecast/_modidx.py
-mlforecast/_nbdev.py
 mlforecast/core.py
 mlforecast/forecast.py
+mlforecast/grouped_array.py
 mlforecast/lgb_cv.py
+mlforecast/target_transforms.py
 mlforecast/utils.py
 mlforecast.egg-info/PKG-INFO
 mlforecast.egg-info/SOURCES.txt
 mlforecast.egg-info/dependency_links.txt
 mlforecast.egg-info/not-zip-safe
 mlforecast.egg-info/requires.txt
 mlforecast.egg-info/top_level.txt
 mlforecast/distributed/__init__.py
-mlforecast/distributed/core.py
 mlforecast/distributed/forecast.py
 mlforecast/distributed/models/__init__.py
-mlforecast/distributed/models/lgb.py
-mlforecast/distributed/models/xgb.py
+mlforecast/distributed/models/dask/__init__.py
+mlforecast/distributed/models/dask/lgb.py
+mlforecast/distributed/models/dask/xgb.py
+mlforecast/distributed/models/ray/__init__.py
+mlforecast/distributed/models/ray/lgb.py
+mlforecast/distributed/models/ray/xgb.py
+mlforecast/distributed/models/spark/__init__.py
+mlforecast/distributed/models/spark/lgb.py
+mlforecast/distributed/models/spark/xgb.py
```

### Comparing `mlforecast-0.6.0/settings.ini` & `mlforecast-0.7.0/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 user = Nixtla
 description = Scalable machine learning based time series forecasting
 keywords = python forecast forecasting machine-learning dask
 author = José Morales
 author_email = jmoralz92@gmail.com
 copyright = Nixtla
 branch = main
-version = 0.6.0
+version = 0.7.0
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 3
-requirements = fugue numba pandas scikit-learn window-ops
-distributed_requirements = dask[complete]
-dev_requirements = black datasetsforecast flake8 lightgbm matplotlib mypy nbdev pylint xgboost
+requirements = numba pandas scikit-learn window-ops
+distributed_requirements = dask[complete] fugue[ray]  pyspark lightgbm_ray xgboost_ray
+dev_requirements = black datasetsforecast flake8 lightgbm matplotlib mypy nbdev pylint statsforecast xgboost
 nbs_path = nbs
 doc_path = _docs
 recursive = True
 doc_host = https://Nixtla.github.io
 doc_baseurl = /
 git_url = https://github.com/Nixtla/mlforecast
 lib_path = mlforecast
```

### Comparing `mlforecast-0.6.0/setup.py` & `mlforecast-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,13 +44,13 @@
     install_requires = requirements,
     extras_require = {
         'distributed': distributed_requirements,
         'dev': dev_requirements,
     },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
+    long_description = open('README.md', encoding='utf-8').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
     **setup_cfg)
```

