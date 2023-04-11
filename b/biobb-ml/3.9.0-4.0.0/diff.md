# Comparing `tmp/biobb_ml-3.9.0.tar.gz` & `tmp/biobb_ml-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_ml-3.9.0.tar", last modified: Wed Dec 28 09:41:55 2022, max compression
+gzip compressed data, was "dist/biobb_ml-4.0.0.tar", last modified: Tue Apr 11 15:49:36 2023, max compression
```

## Comparing `biobb_ml-3.9.0.tar` & `biobb_ml-4.0.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3974 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3206 2022-12-28 09:40:29.000000 biobb_ml-3.9.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      166 2022-12-28 09:40:22.000000 biobb_ml-3.9.0/biobb_ml/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/classification/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      190 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/classification/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11666 2022-12-28 07:43:14.000000 biobb_ml-3.9.0/biobb_ml/classification/classification_predict.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    10110 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/classification/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17591 2022-12-28 08:50:06.000000 biobb_ml-3.9.0/biobb_ml/classification/decision_tree.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17589 2022-12-28 08:50:18.000000 biobb_ml-3.9.0/biobb_ml/classification/k_neighbors.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    14295 2022-12-28 08:50:12.000000 biobb_ml-3.9.0/biobb_ml/classification/k_neighbors_coefficient.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18155 2022-12-28 08:50:24.000000 biobb_ml-3.9.0/biobb_ml/classification/logistic_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17724 2022-12-28 07:49:34.000000 biobb_ml-3.9.0/biobb_ml/classification/random_forest_classifier.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17881 2022-12-28 08:50:28.000000 biobb_ml-3.9.0/biobb_ml/classification/support_vector_machine.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/clustering/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      193 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/clustering/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11919 2022-12-28 08:00:31.000000 biobb_ml-3.9.0/biobb_ml/clustering/agglomerative_clustering.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12092 2022-12-28 07:58:30.000000 biobb_ml-3.9.0/biobb_ml/clustering/agglomerative_coefficient.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10122 2022-12-28 07:59:11.000000 biobb_ml-3.9.0/biobb_ml/clustering/clustering_predict.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    12906 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/clustering/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12824 2022-12-28 08:01:01.000000 biobb_ml-3.9.0/biobb_ml/clustering/dbscan.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11855 2022-12-28 08:50:56.000000 biobb_ml-3.9.0/biobb_ml/clustering/k_means.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12159 2022-12-28 08:48:14.000000 biobb_ml-3.9.0/biobb_ml/clustering/k_means_coefficient.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11549 2022-12-28 08:51:58.000000 biobb_ml-3.9.0/biobb_ml/clustering/spectral_clustering.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10965 2022-12-28 08:53:19.000000 biobb_ml-3.9.0/biobb_ml/clustering/spectral_coefficient.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      103 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     7900 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15723 2022-12-28 08:54:26.000000 biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/pls_components.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11602 2022-12-28 08:56:11.000000 biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/pls_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12148 2022-12-28 08:56:44.000000 biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/principal_component.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      201 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17704 2022-12-28 08:58:43.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/autoencoder_neural_network.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    23369 2022-12-28 09:05:19.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/classification_neural_network.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    12546 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10156 2022-12-28 09:16:32.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/neural_network_decode.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11621 2022-12-28 09:17:17.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/neural_network_predict.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17930 2022-12-28 09:18:11.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/recurrent_neural_network.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    21904 2022-12-28 09:20:13.000000 biobb_ml-3.9.0/biobb_ml/neural_networks/regression_neural_network.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/regression/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      161 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/regression/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5770 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/regression/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16543 2022-12-28 09:24:20.000000 biobb_ml-3.9.0/biobb_ml/regression/linear_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16491 2022-12-28 09:25:20.000000 biobb_ml-3.9.0/biobb_ml/regression/polynomial_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16489 2022-12-28 09:26:19.000000 biobb_ml-3.9.0/biobb_ml/regression/random_forest_regressor.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10857 2022-12-28 09:27:10.000000 biobb_ml-3.9.0/biobb_ml/regression/regression_predict.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/resampling/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       75 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/resampling/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     7407 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/resampling/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18772 2022-12-28 09:28:40.000000 biobb_ml-3.9.0/biobb_ml/resampling/oversampling.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5133 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/resampling/reg_resampler.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17817 2022-12-28 09:30:15.000000 biobb_ml-3.9.0/biobb_ml/resampling/resampling.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    20788 2022-12-28 09:31:24.000000 biobb_ml-3.9.0/biobb_ml/resampling/undersampling.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml/utils/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      147 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/utils/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4047 2022-05-26 11:34:41.000000 biobb_ml-3.9.0/biobb_ml/utils/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7429 2022-12-28 09:32:49.000000 biobb_ml-3.9.0/biobb_ml/utils/correlation_matrix.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6674 2022-12-28 09:33:54.000000 biobb_ml-3.9.0/biobb_ml/utils/dendrogram.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6802 2022-12-28 09:34:44.000000 biobb_ml-3.9.0/biobb_ml/utils/drop_columns.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7058 2022-12-28 09:35:32.000000 biobb_ml-3.9.0/biobb_ml/utils/dummy_variables.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7295 2022-12-28 09:36:20.000000 biobb_ml-3.9.0/biobb_ml/utils/map_variables.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7334 2022-12-28 09:37:06.000000 biobb_ml-3.9.0/biobb_ml/utils/pairwise_comparison.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7055 2022-12-28 09:38:04.000000 biobb_ml-3.9.0/biobb_ml/utils/scale_columns.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3974 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2431 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2545 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      126 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/biobb_ml.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2022-12-28 09:41:55.000000 biobb_ml-3.9.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4373 2022-12-28 09:40:08.000000 biobb_ml-3.9.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5893 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5125 2023-04-11 15:48:31.000000 biobb_ml-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      166 2023-04-11 15:48:17.000000 biobb_ml-4.0.0/biobb_ml/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/classification/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      190 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/classification/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11666 2022-12-28 07:43:14.000000 biobb_ml-4.0.0/biobb_ml/classification/classification_predict.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10110 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/classification/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17591 2022-12-28 08:50:06.000000 biobb_ml-4.0.0/biobb_ml/classification/decision_tree.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17589 2022-12-28 08:50:18.000000 biobb_ml-4.0.0/biobb_ml/classification/k_neighbors.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    14295 2022-12-28 08:50:12.000000 biobb_ml-4.0.0/biobb_ml/classification/k_neighbors_coefficient.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18155 2022-12-28 08:50:24.000000 biobb_ml-4.0.0/biobb_ml/classification/logistic_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17724 2022-12-28 07:49:34.000000 biobb_ml-4.0.0/biobb_ml/classification/random_forest_classifier.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17881 2022-12-28 08:50:28.000000 biobb_ml-4.0.0/biobb_ml/classification/support_vector_machine.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/clustering/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      193 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/clustering/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11919 2022-12-28 08:00:31.000000 biobb_ml-4.0.0/biobb_ml/clustering/agglomerative_clustering.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12092 2022-12-28 07:58:30.000000 biobb_ml-4.0.0/biobb_ml/clustering/agglomerative_coefficient.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10122 2022-12-28 07:59:11.000000 biobb_ml-4.0.0/biobb_ml/clustering/clustering_predict.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12906 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/clustering/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12824 2022-12-28 08:01:01.000000 biobb_ml-4.0.0/biobb_ml/clustering/dbscan.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11855 2022-12-28 08:50:56.000000 biobb_ml-4.0.0/biobb_ml/clustering/k_means.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12159 2022-12-28 08:48:14.000000 biobb_ml-4.0.0/biobb_ml/clustering/k_means_coefficient.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11549 2022-12-28 08:51:58.000000 biobb_ml-4.0.0/biobb_ml/clustering/spectral_clustering.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10965 2022-12-28 08:53:19.000000 biobb_ml-4.0.0/biobb_ml/clustering/spectral_coefficient.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      103 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7900 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15723 2022-12-28 08:54:26.000000 biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/pls_components.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11602 2022-12-28 08:56:11.000000 biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/pls_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12148 2022-12-28 08:56:44.000000 biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/principal_component.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      201 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17704 2022-12-28 08:58:43.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/autoencoder_neural_network.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    23369 2022-12-28 09:05:19.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/classification_neural_network.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12546 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10156 2022-12-28 09:16:32.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/neural_network_decode.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11621 2022-12-28 09:17:17.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/neural_network_predict.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17930 2022-12-28 09:18:11.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/recurrent_neural_network.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    21904 2022-12-28 09:20:13.000000 biobb_ml-4.0.0/biobb_ml/neural_networks/regression_neural_network.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/regression/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      161 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/regression/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5770 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/regression/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16543 2022-12-28 09:24:20.000000 biobb_ml-4.0.0/biobb_ml/regression/linear_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16491 2022-12-28 09:25:20.000000 biobb_ml-4.0.0/biobb_ml/regression/polynomial_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16489 2022-12-28 09:26:19.000000 biobb_ml-4.0.0/biobb_ml/regression/random_forest_regressor.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10857 2022-12-28 09:27:10.000000 biobb_ml-4.0.0/biobb_ml/regression/regression_predict.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/resampling/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       75 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/resampling/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7407 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/resampling/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18772 2022-12-28 09:28:40.000000 biobb_ml-4.0.0/biobb_ml/resampling/oversampling.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5133 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/resampling/reg_resampler.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17817 2022-12-28 09:30:15.000000 biobb_ml-4.0.0/biobb_ml/resampling/resampling.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    20788 2022-12-28 09:31:24.000000 biobb_ml-4.0.0/biobb_ml/resampling/undersampling.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml/utils/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      147 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/utils/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4047 2022-05-26 11:34:41.000000 biobb_ml-4.0.0/biobb_ml/utils/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7429 2022-12-28 09:32:49.000000 biobb_ml-4.0.0/biobb_ml/utils/correlation_matrix.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6674 2022-12-28 09:33:54.000000 biobb_ml-4.0.0/biobb_ml/utils/dendrogram.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6802 2022-12-28 09:34:44.000000 biobb_ml-4.0.0/biobb_ml/utils/drop_columns.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7058 2022-12-28 09:35:32.000000 biobb_ml-4.0.0/biobb_ml/utils/dummy_variables.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7295 2022-12-28 09:36:20.000000 biobb_ml-4.0.0/biobb_ml/utils/map_variables.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7334 2022-12-28 09:37:06.000000 biobb_ml-4.0.0/biobb_ml/utils/pairwise_comparison.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7055 2022-12-28 09:38:04.000000 biobb_ml-4.0.0/biobb_ml/utils/scale_columns.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5893 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2431 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2545 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      126 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        9 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/biobb_ml.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 15:49:36.000000 biobb_ml-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4373 2023-04-11 15:48:09.000000 biobb_ml-4.0.0/setup.py
```

### Comparing `biobb_ml-3.9.0/LICENSE` & `biobb_ml-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/classification_predict.py` & `biobb_ml-4.0.0/biobb_ml/classification/classification_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/common.py` & `biobb_ml-4.0.0/biobb_ml/classification/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/decision_tree.py` & `biobb_ml-4.0.0/biobb_ml/classification/decision_tree.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/k_neighbors.py` & `biobb_ml-4.0.0/biobb_ml/classification/k_neighbors.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/k_neighbors_coefficient.py` & `biobb_ml-4.0.0/biobb_ml/classification/k_neighbors_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/logistic_regression.py` & `biobb_ml-4.0.0/biobb_ml/classification/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/random_forest_classifier.py` & `biobb_ml-4.0.0/biobb_ml/classification/random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/classification/support_vector_machine.py` & `biobb_ml-4.0.0/biobb_ml/classification/support_vector_machine.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/agglomerative_clustering.py` & `biobb_ml-4.0.0/biobb_ml/clustering/agglomerative_clustering.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/agglomerative_coefficient.py` & `biobb_ml-4.0.0/biobb_ml/clustering/agglomerative_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/clustering_predict.py` & `biobb_ml-4.0.0/biobb_ml/clustering/clustering_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/common.py` & `biobb_ml-4.0.0/biobb_ml/clustering/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/dbscan.py` & `biobb_ml-4.0.0/biobb_ml/clustering/dbscan.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/k_means.py` & `biobb_ml-4.0.0/biobb_ml/clustering/k_means.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/k_means_coefficient.py` & `biobb_ml-4.0.0/biobb_ml/clustering/k_means_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/spectral_clustering.py` & `biobb_ml-4.0.0/biobb_ml/clustering/spectral_clustering.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/clustering/spectral_coefficient.py` & `biobb_ml-4.0.0/biobb_ml/clustering/spectral_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/common.py` & `biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/pls_components.py` & `biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/pls_components.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/pls_regression.py` & `biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/pls_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/dimensionality_reduction/principal_component.py` & `biobb_ml-4.0.0/biobb_ml/dimensionality_reduction/principal_component.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/neural_networks/autoencoder_neural_network.py` & `biobb_ml-4.0.0/biobb_ml/neural_networks/autoencoder_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/neural_networks/classification_neural_network.py` & `biobb_ml-4.0.0/biobb_ml/neural_networks/classification_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/neural_networks/common.py` & `biobb_ml-4.0.0/biobb_ml/neural_networks/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/neural_networks/neural_network_decode.py` & `biobb_ml-4.0.0/biobb_ml/neural_networks/neural_network_decode.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/neural_networks/neural_network_predict.py` & `biobb_ml-4.0.0/biobb_ml/neural_networks/neural_network_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/neural_networks/recurrent_neural_network.py` & `biobb_ml-4.0.0/biobb_ml/neural_networks/recurrent_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/neural_networks/regression_neural_network.py` & `biobb_ml-4.0.0/biobb_ml/neural_networks/regression_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/regression/common.py` & `biobb_ml-4.0.0/biobb_ml/regression/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/regression/linear_regression.py` & `biobb_ml-4.0.0/biobb_ml/regression/linear_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/regression/polynomial_regression.py` & `biobb_ml-4.0.0/biobb_ml/regression/polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/regression/random_forest_regressor.py` & `biobb_ml-4.0.0/biobb_ml/regression/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/regression/regression_predict.py` & `biobb_ml-4.0.0/biobb_ml/regression/regression_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/resampling/common.py` & `biobb_ml-4.0.0/biobb_ml/resampling/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/resampling/oversampling.py` & `biobb_ml-4.0.0/biobb_ml/resampling/oversampling.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/resampling/reg_resampler.py` & `biobb_ml-4.0.0/biobb_ml/resampling/reg_resampler.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/resampling/resampling.py` & `biobb_ml-4.0.0/biobb_ml/resampling/resampling.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/resampling/undersampling.py` & `biobb_ml-4.0.0/biobb_ml/resampling/undersampling.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/common.py` & `biobb_ml-4.0.0/biobb_ml/utils/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/correlation_matrix.py` & `biobb_ml-4.0.0/biobb_ml/utils/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/dendrogram.py` & `biobb_ml-4.0.0/biobb_ml/utils/dendrogram.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/drop_columns.py` & `biobb_ml-4.0.0/biobb_ml/utils/drop_columns.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/dummy_variables.py` & `biobb_ml-4.0.0/biobb_ml/utils/dummy_variables.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/map_variables.py` & `biobb_ml-4.0.0/biobb_ml/utils/map_variables.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/pairwise_comparison.py` & `biobb_ml-4.0.0/biobb_ml/utils/pairwise_comparison.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml/utils/scale_columns.py` & `biobb_ml-4.0.0/biobb_ml/utils/scale_columns.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml.egg-info/SOURCES.txt` & `biobb_ml-4.0.0/biobb_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/biobb_ml.egg-info/entry_points.txt` & `biobb_ml-4.0.0/biobb_ml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_ml-3.9.0/setup.py` & `biobb_ml-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_ml",
-    version="3.9.0",
+    version="4.0.0",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_ml is the Biobb module collection to perform machine learning predictions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_ml",
     project_urls={
         "Documentation": "http://biobb_ml.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==3.9.0', 'scikit-learn ==0.24.2', 'pandas ==1.3.0', 'seaborn ==0.10.1', 'tensorflow>=2.4.2', 'h5py ==2.10.0', 'imbalanced-learn ==0.7.0'],
+    install_requires=['biobb_common==4.0.0', 'scikit-learn ==0.24.2', 'pandas ==1.3.0', 'seaborn ==0.10.1', 'tensorflow>=2.4.2', 'h5py ==2.10.0', 'imbalanced-learn ==0.7.0'],
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "classification_predict = biobb_ml.classification.classification_predict:main",
             "decision_tree = biobb_ml.classification.decision_tree:main",
             "k_neighbors_coefficient = biobb_ml.classification.k_neighbors_coefficient:main",
             "k_neighbors = biobb_ml.classification.k_neighbors:main",
```

