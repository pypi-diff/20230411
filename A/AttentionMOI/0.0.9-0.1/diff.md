# Comparing `tmp/AttentionMOI-0.0.9.tar.gz` & `tmp/AttentionMOI-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AttentionMOI-0.0.9.tar", last modified: Tue Apr 11 02:14:55 2023, max compression
+gzip compressed data, was "AttentionMOI-0.1.tar", last modified: Tue Apr 11 02:18:19 2023, max compression
```

## Comparing `AttentionMOI-0.0.9.tar` & `AttentionMOI-0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.309631 AttentionMOI-0.0.9/
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.015108 AttentionMOI-0.0.9/AttentionMOI/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/__init__.py
--rw-rw-rw-   0        0        0     2673 2023-03-24 10:35:08.000000 AttentionMOI-0.0.9/AttentionMOI/deepmoi.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.074728 AttentionMOI-0.0.9/AttentionMOI/example/
--rw-rw-rw-   0        0        0     7419 2022-08-26 01:04:12.000000 AttentionMOI-0.0.9/AttentionMOI/example/cnv.csv.gz
--rw-rw-rw-   0        0        0    13651 2022-08-26 01:04:12.000000 AttentionMOI-0.0.9/AttentionMOI/example/label.csv
--rw-rw-rw-   0        0        0    77257 2022-08-26 01:04:12.000000 AttentionMOI-0.0.9/AttentionMOI/example/met.csv.gz
--rw-rw-rw-   0        0        0   118903 2022-08-26 01:04:12.000000 AttentionMOI-0.0.9/AttentionMOI/example/rna.csv.gz
--rw-rw-rw-   0        0        0       72 2023-04-11 02:14:44.000000 AttentionMOI-0.0.9/AttentionMOI/moi.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.152554 AttentionMOI-0.0.9/AttentionMOI/src/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/__init__.py
--rw-rw-rw-   0        0        0      488 2022-11-07 18:45:20.000000 AttentionMOI-0.0.9/AttentionMOI/src/explain.py
--rw-rw-rw-   0        0        0     2944 2022-11-07 18:45:20.000000 AttentionMOI-0.0.9/AttentionMOI/src/feature_selection.py
--rw-rw-rw-   0        0        0     7085 2023-03-24 10:49:51.000000 AttentionMOI-0.0.9/AttentionMOI/src/fsd.py
--rw-rw-rw-   0        0        0     1962 2023-03-24 06:27:29.000000 AttentionMOI-0.0.9/AttentionMOI/src/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.185037 AttentionMOI-0.0.9/AttentionMOI/src/moanna/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/__init__.py
--rw-rw-rw-   0        0        0       22 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/__meta__.py
--rw-rw-rw-   0        0        0     2734 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.225520 AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/
--rw-rw-rw-   0        0        0     3501 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py
--rw-rw-rw-   0        0        0    21017 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py
--rw-rw-rw-   0        0        0     2994 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/__init__.py
--rw-rw-rw-   0        0        0     7542 2023-03-23 07:59:37.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.248917 AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/
--rw-rw-rw-   0        0        0     6780 2023-03-24 08:37:52.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/Autoencoder.py
--rw-rw-rw-   0        0        0     5066 2023-03-23 06:48:20.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/ClassificationModel.py
--rw-rw-rw-   0        0        0     1458 2023-03-23 09:16:06.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/Moanna.py
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/__init__.py
--rw-rw-rw-   0        0        0     3439 2022-11-07 18:45:20.000000 AttentionMOI-0.0.9/AttentionMOI/src/module.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.293110 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/
--rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/__init__.py
--rw-rw-rw-   0        0        0     3753 2021-03-31 20:51:34.000000 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/feat_importance.py
--rw-rw-rw-   0        0        0      675 2021-03-31 20:51:34.000000 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/main_biomarker.py
--rw-rw-rw-   0        0        0     1150 2023-03-24 07:18:32.000000 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/main_mogonet.py
--rw-rw-rw-   0        0        0     3711 2021-03-31 20:51:34.000000 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/models.py
--rw-rw-rw-   0        0        0     9308 2023-03-24 10:46:36.000000 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/train_test.py
--rw-rw-rw-   0        0        0     4594 2023-03-24 05:54:54.000000 AttentionMOI-0.0.9/AttentionMOI/src/mogonet/utils.py
--rw-rw-rw-   0        0        0     7379 2022-11-23 23:48:44.000000 AttentionMOI-0.0.9/AttentionMOI/src/prediction.py
--rw-rw-rw-   0        0        0     2164 2022-11-07 18:45:20.000000 AttentionMOI-0.0.9/AttentionMOI/src/preprocess.py
--rw-rw-rw-   0        0        0    23921 2023-03-24 10:44:22.000000 AttentionMOI-0.0.9/AttentionMOI/src/train.py
--rw-rw-rw-   0        0        0     9205 2022-11-07 18:45:20.000000 AttentionMOI-0.0.9/AttentionMOI/src/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:14:55.051011 AttentionMOI-0.0.9/AttentionMOI.egg-info/
--rw-rw-rw-   0        0        0      391 2023-04-11 02:14:54.000000 AttentionMOI-0.0.9/AttentionMOI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-04-11 02:14:54.000000 AttentionMOI-0.0.9/AttentionMOI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       72 2023-04-11 02:14:54.000000 AttentionMOI-0.0.9/AttentionMOI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-11 02:14:54.000000 AttentionMOI-0.0.9/AttentionMOI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      223 2023-04-11 02:14:54.000000 AttentionMOI-0.0.9/AttentionMOI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 02:14:54.000000 AttentionMOI-0.0.9/AttentionMOI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2023-03-16 08:33:55.000000 AttentionMOI-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      391 2023-04-11 02:14:55.298165 AttentionMOI-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2216 2023-03-24 09:41:22.000000 AttentionMOI-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 02:14:55.310750 AttentionMOI-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1550 2023-04-11 02:14:42.000000 AttentionMOI-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.268339 AttentionMOI-0.1/
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.109140 AttentionMOI-0.1/AttentionMOI/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/__init__.py
+-rw-rw-rw-   0        0        0     2673 2023-03-24 10:35:08.000000 AttentionMOI-0.1/AttentionMOI/deepmoi.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.152083 AttentionMOI-0.1/AttentionMOI/example/
+-rw-rw-rw-   0        0        0     7419 2022-08-26 01:04:12.000000 AttentionMOI-0.1/AttentionMOI/example/cnv.csv.gz
+-rw-rw-rw-   0        0        0    13651 2022-08-26 01:04:12.000000 AttentionMOI-0.1/AttentionMOI/example/label.csv
+-rw-rw-rw-   0        0        0    77257 2022-08-26 01:04:12.000000 AttentionMOI-0.1/AttentionMOI/example/met.csv.gz
+-rw-rw-rw-   0        0        0   118903 2022-08-26 01:04:12.000000 AttentionMOI-0.1/AttentionMOI/example/rna.csv.gz
+-rw-rw-rw-   0        0        0       72 2023-04-11 02:14:44.000000 AttentionMOI-0.1/AttentionMOI/moi.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.189437 AttentionMOI-0.1/AttentionMOI/src/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/__init__.py
+-rw-rw-rw-   0        0        0      488 2022-11-07 18:45:20.000000 AttentionMOI-0.1/AttentionMOI/src/explain.py
+-rw-rw-rw-   0        0        0     2944 2022-11-07 18:45:20.000000 AttentionMOI-0.1/AttentionMOI/src/feature_selection.py
+-rw-rw-rw-   0        0        0     7085 2023-03-24 10:49:51.000000 AttentionMOI-0.1/AttentionMOI/src/fsd.py
+-rw-rw-rw-   0        0        0     1962 2023-03-24 06:27:29.000000 AttentionMOI-0.1/AttentionMOI/src/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.204291 AttentionMOI-0.1/AttentionMOI/src/moanna/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/__init__.py
+-rw-rw-rw-   0        0        0       22 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/__meta__.py
+-rw-rw-rw-   0        0        0     2734 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.221245 AttentionMOI-0.1/AttentionMOI/src/moanna/helper/
+-rw-rw-rw-   0        0        0     3501 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py
+-rw-rw-rw-   0        0        0    21017 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py
+-rw-rw-rw-   0        0        0     2994 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/helper/__init__.py
+-rw-rw-rw-   0        0        0     7542 2023-03-23 07:59:37.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.236901 AttentionMOI-0.1/AttentionMOI/src/moanna/model/
+-rw-rw-rw-   0        0        0     6780 2023-03-24 08:37:52.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/model/Autoencoder.py
+-rw-rw-rw-   0        0        0     5066 2023-03-23 06:48:20.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/model/ClassificationModel.py
+-rw-rw-rw-   0        0        0     1458 2023-03-23 09:16:06.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/model/Moanna.py
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/moanna/model/__init__.py
+-rw-rw-rw-   0        0        0     3439 2022-11-07 18:45:20.000000 AttentionMOI-0.1/AttentionMOI/src/module.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.263354 AttentionMOI-0.1/AttentionMOI/src/mogonet/
+-rw-rw-rw-   0        0        0        0 2020-12-15 02:37:18.000000 AttentionMOI-0.1/AttentionMOI/src/mogonet/__init__.py
+-rw-rw-rw-   0        0        0     3753 2021-03-31 20:51:34.000000 AttentionMOI-0.1/AttentionMOI/src/mogonet/feat_importance.py
+-rw-rw-rw-   0        0        0      675 2021-03-31 20:51:34.000000 AttentionMOI-0.1/AttentionMOI/src/mogonet/main_biomarker.py
+-rw-rw-rw-   0        0        0     1150 2023-03-24 07:18:32.000000 AttentionMOI-0.1/AttentionMOI/src/mogonet/main_mogonet.py
+-rw-rw-rw-   0        0        0     3711 2021-03-31 20:51:34.000000 AttentionMOI-0.1/AttentionMOI/src/mogonet/models.py
+-rw-rw-rw-   0        0        0     9308 2023-03-24 10:46:36.000000 AttentionMOI-0.1/AttentionMOI/src/mogonet/train_test.py
+-rw-rw-rw-   0        0        0     4594 2023-03-24 05:54:54.000000 AttentionMOI-0.1/AttentionMOI/src/mogonet/utils.py
+-rw-rw-rw-   0        0        0     7379 2022-11-23 23:48:44.000000 AttentionMOI-0.1/AttentionMOI/src/prediction.py
+-rw-rw-rw-   0        0        0     2164 2022-11-07 18:45:20.000000 AttentionMOI-0.1/AttentionMOI/src/preprocess.py
+-rw-rw-rw-   0        0        0    23921 2023-03-24 10:44:22.000000 AttentionMOI-0.1/AttentionMOI/src/train.py
+-rw-rw-rw-   0        0        0     9205 2022-11-07 18:45:20.000000 AttentionMOI-0.1/AttentionMOI/src/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:18:19.134067 AttentionMOI-0.1/AttentionMOI.egg-info/
+-rw-rw-rw-   0        0        0      389 2023-04-11 02:18:18.000000 AttentionMOI-0.1/AttentionMOI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-04-11 02:18:18.000000 AttentionMOI-0.1/AttentionMOI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       72 2023-04-11 02:18:18.000000 AttentionMOI-0.1/AttentionMOI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-11 02:18:18.000000 AttentionMOI-0.1/AttentionMOI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      231 2023-04-11 02:18:18.000000 AttentionMOI-0.1/AttentionMOI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 02:18:18.000000 AttentionMOI-0.1/AttentionMOI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2023-03-16 08:33:55.000000 AttentionMOI-0.1/LICENSE
+-rw-rw-rw-   0        0        0      389 2023-04-11 02:18:19.268041 AttentionMOI-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2216 2023-03-24 09:41:22.000000 AttentionMOI-0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:18:19.269337 AttentionMOI-0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-04-11 02:17:46.000000 AttentionMOI-0.1/setup.py
```

### Comparing `AttentionMOI-0.0.9/AttentionMOI/deepmoi.py` & `AttentionMOI-0.1/AttentionMOI/deepmoi.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/example/cnv.csv.gz` & `AttentionMOI-0.1/AttentionMOI/example/cnv.csv.gz`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/example/label.csv` & `AttentionMOI-0.1/AttentionMOI/example/label.csv`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/example/met.csv.gz` & `AttentionMOI-0.1/AttentionMOI/example/met.csv.gz`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/example/rna.csv.gz` & `AttentionMOI-0.1/AttentionMOI/example/rna.csv.gz`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/feature_selection.py` & `AttentionMOI-0.1/AttentionMOI/src/feature_selection.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/fsd.py` & `AttentionMOI-0.1/AttentionMOI/src/fsd.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/main.py` & `AttentionMOI-0.1/AttentionMOI/src/main.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/cli.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/cli.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/helper/ClusteringMetricsHelper.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/helper/DataCleanUpFunctions.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/helper/SurvivalHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/main.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/main.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/Autoencoder.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/model/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/ClassificationModel.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/model/ClassificationModel.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/moanna/model/Moanna.py` & `AttentionMOI-0.1/AttentionMOI/src/moanna/model/Moanna.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/module.py` & `AttentionMOI-0.1/AttentionMOI/src/module.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/mogonet/feat_importance.py` & `AttentionMOI-0.1/AttentionMOI/src/mogonet/feat_importance.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/mogonet/main_biomarker.py` & `AttentionMOI-0.1/AttentionMOI/src/mogonet/main_biomarker.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/mogonet/main_mogonet.py` & `AttentionMOI-0.1/AttentionMOI/src/mogonet/main_mogonet.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/mogonet/models.py` & `AttentionMOI-0.1/AttentionMOI/src/mogonet/models.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/mogonet/train_test.py` & `AttentionMOI-0.1/AttentionMOI/src/mogonet/train_test.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/mogonet/utils.py` & `AttentionMOI-0.1/AttentionMOI/src/mogonet/utils.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/prediction.py` & `AttentionMOI-0.1/AttentionMOI/src/prediction.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/preprocess.py` & `AttentionMOI-0.1/AttentionMOI/src/preprocess.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/train.py` & `AttentionMOI-0.1/AttentionMOI/src/train.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI/src/utils.py` & `AttentionMOI-0.1/AttentionMOI/src/utils.py`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/AttentionMOI.egg-info/SOURCES.txt` & `AttentionMOI-0.1/AttentionMOI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/LICENSE` & `AttentionMOI-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/README.md` & `AttentionMOI-0.1/README.md`

 * *Files identical despite different names*

### Comparing `AttentionMOI-0.0.9/setup.py` & `AttentionMOI-0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,26 +12,27 @@
     'torch==1.13.1',
     'scikit-learn==1.2.2',
     'numpy==1.23.5',
     'matplotlib==3.6.2',
     'xgboost==1.7.4',
     'livelossplot', 
     'tensorboardX',
-    'tqdm'
+    'tqdm',
+    'ipython',
 ]
 
 setup(
     # 应用名
     name='AttentionMOI',
     # 作者名
     author='Billy',
     # 作者邮箱
     author_email='liangbilin0324@163.com',
     # 版本号
-    version='0.0.9',
+    version='0.1',
     # 要求python版本
     python_requires=">=3.9.*",
     # 找到本目录下的所有python包
     packages=find_packages(),
     # 自动安装依赖
     install_requires=install_packages,
     dependency_links=[
```

