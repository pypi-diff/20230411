# Comparing `tmp/evalml-0.72.0.tar.gz` & `tmp/evalml-0.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-_ysx6gwl/evalml-0.72.0.tar", last modified: Mon Mar 27 19:05:04 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-dmv6l6xa/evalml-0.73.0.tar", last modified: Tue Apr 11 21:23:11 2023, max compression
```

## Comparing `evalml-0.72.0.tar` & `evalml-0.73.0.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/
--rw-r--r--   0 root         (0) root         (0)     1513 2023-03-27 19:04:50.000000 evalml-0.72.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8233 2023-03-27 19:05:04.000000 evalml-0.72.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4824 2023-03-27 19:04:50.000000 evalml-0.72.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/
--rw-r--r--   0 root         (0) root         (0)      763 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/automl/
--rw-r--r--   0 root         (0) root         (0)      412 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/automl/automl_algorithm/
--rw-r--r--   0 root         (0) root         (0)      318 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/automl_algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11921 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/automl_algorithm/automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    29236 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/automl_algorithm/default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    21384 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/automl_algorithm/iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    79400 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/automl_search.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/automl/engine/
--rw-r--r--   0 root         (0) root         (0)      409 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/engine/cf_engine.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/engine/dask_engine.py
--rw-r--r--   0 root         (0) root         (0)    15405 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/engine/engine_base.py
--rw-r--r--   0 root         (0) root         (0)     5060 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/engine/sequential_engine.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/progress.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/automl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/data_checks/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11989 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_check.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_check_action.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_check_action_code.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     2994 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_check_message.py
--rw-r--r--   0 root         (0) root         (0)     6580 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_check_message_code.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_check_message_type.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/data_checks.py
--rw-r--r--   0 root         (0) root         (0)    25088 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/default_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    19650 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)    11843 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    17159 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9500 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6213 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7119 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8159 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8205 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/data_checks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/demos/
--rw-r--r--   0 root         (0) root         (0)      297 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      605 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/churn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/demos/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     1103 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/diabetes.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/fraud.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/weather.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/demos/wine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/exceptions/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/exceptions/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/model_family/
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_family/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_family/model_family.py
--rw-r--r--   0 root         (0) root         (0)      910 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_family/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/model_understanding/
--rw-r--r--   0 root         (0) root         (0)     1273 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
--rw-r--r--   0 root         (0) root         (0)    18388 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/_partial_dependence_utils.py
--rw-r--r--   0 root         (0) root         (0)     8990 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/force_plots.py
--rw-r--r--   0 root         (0) root         (0)    15125 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/metrics.py
--rw-r--r--   0 root         (0) root         (0)    27420 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/partial_dependence_functions.py
--rw-r--r--   0 root         (0) root         (0)    13556 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/permutation_importance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/model_understanding/prediction_explanations/
--rw-r--r--   0 root         (0) root         (0)      175 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/prediction_explanations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13317 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/prediction_explanations/_algorithms.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
--rw-r--r--   0 root         (0) root         (0)    36936 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/prediction_explanations/_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15630 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/prediction_explanations/explainers.py
--rw-r--r--   0 root         (0) root         (0)    22293 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/model_understanding/visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/objectives/
--rw-r--r--   0 root         (0) root         (0)     1543 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     3392 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/fraud_cost.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/multiclass_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/objective_base.py
--rw-r--r--   0 root         (0) root         (0)      406 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/sensitivity_low_alert.py
--rw-r--r--   0 root         (0) root         (0)    33865 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/standard_metrics.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/time_series_regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     6835 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/objectives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/
--rw-r--r--   0 root         (0) root         (0)     1928 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4893 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/binary_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/binary_classification_pipeline_mixin.py
--rw-r--r--   0 root         (0) root         (0)     7845 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    40232 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/component_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/
--rw-r--r--   0 root         (0) root         (0)     1935 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10149 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/component_base.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/component_base_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/ensemble/
--rw-r--r--   0 root         (0) root         (0)      349 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/ensemble/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/estimators/
--rw-r--r--   0 root         (0) root         (0)      964 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/
--rw-r--r--   0 root         (0) root         (0)     1445 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3656 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8575 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4811 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
--rw-r--r--   0 root         (0) root         (0)     5042 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8530 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/
--rw-r--r--   0 root         (0) root         (0)     1685 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13987 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5080 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7583 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7288 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
--rw-r--r--   0 root         (0) root         (0)     9356 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5128 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/
--rw-r--r--   0 root         (0) root         (0)     1478 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6235 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/column_selectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/dimensionality_reduction/
--rw-r--r--   0 root         (0) root         (0)      273 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/encoders/
--rw-r--r--   0 root         (0) root         (0)      439 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
--rw-r--r--   0 root         (0) root         (0)    13779 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    12206 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/
--rw-r--r--   0 root         (0) root         (0)      599 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     5285 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
--rw-r--r--   0 root         (0) root         (0)     3116 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/
--rw-r--r--   0 root         (0) root         (0)      651 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8698 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/imputer.py
--rw-r--r--   0 root         (0) root         (0)     4022 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5668 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    10138 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5899 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    15544 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
--rw-r--r--   0 root         (0) root         (0)     6461 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)    17526 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     5216 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/samplers/
--rw-r--r--   0 root         (0) root         (0)      200 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/samplers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6456 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
--rw-r--r--   0 root         (0) root         (0)     6341 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/samplers/oversampler.py
--rw-r--r--   0 root         (0) root         (0)     8163 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/samplers/undersampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/pipelines/components/transformers/scalers/
--rw-r--r--   0 root         (0) root         (0)      141 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/scalers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/transformers/transformer.py
--rw-r--r--   0 root         (0) root         (0)    20044 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/components/utils.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/multiclass_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    33022 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/pipeline_meta.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    17176 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/time_series_classification_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    14278 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/time_series_pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    11734 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/time_series_regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    54012 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/preprocessing/
--rw-r--r--   0 root         (0) root         (0)      269 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/preprocessing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/preprocessing/data_splitters/
--rw-r--r--   0 root         (0) root         (0)      367 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/preprocessing/data_splitters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/preprocessing/data_splitters/no_split.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/preprocessing/data_splitters/sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     5599 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/preprocessing/data_splitters/time_series_split.py
--rw-r--r--   0 root         (0) root         (0)     3669 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/preprocessing/data_splitters/training_validation_split.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/preprocessing/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/problem_types/
--rw-r--r--   0 root         (0) root         (0)      306 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/problem_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/problem_types/problem_types.py
--rw-r--r--   0 root         (0) root         (0)     6085 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/problem_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/automl_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/dask_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9622 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
--rw-r--r--   0 root         (0) root         (0)    17604 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
--rw-r--r--   0 root         (0) root         (0)    14529 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
--rw-r--r--   0 root         (0) root         (0)   179131 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38707 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38820 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_classification.py
--rw-r--r--   0 root         (0) root         (0)    15745 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
--rw-r--r--   0 root         (0) root         (0)     8716 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_regression.py
--rw-r--r--   0 root         (0) root         (0)     7055 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
--rw-r--r--   0 root         (0) root         (0)    12934 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_automl_utils.py
--rw-r--r--   0 root         (0) root         (0)    33437 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7793 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_engine_base.py
--rw-r--r--   0 root         (0) root         (0)    36749 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_search_iterative.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/automl_tests/test_time_series_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/component_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24915 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    11644 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    16946 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6678 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8548 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_column_selector_transformers.py
--rw-r--r--   0 root         (0) root         (0)    64838 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_components.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     7573 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_en_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_en_regressor.py
--rw-r--r--   0 root         (0) root         (0)    15118 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_estimators.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7789 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_feature_selectors.py
--rw-r--r--   0 root         (0) root         (0)    14925 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_featuretools.py
--rw-r--r--   0 root         (0) root         (0)     9564 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
--rw-r--r--   0 root         (0) root         (0)    25369 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_imputer.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_knn_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     8017 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_label_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_lda.py
--rw-r--r--   0 root         (0) root         (0)    13317 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_lgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     9686 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_lgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8111 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_lsa.py
--rw-r--r--   0 root         (0) root         (0)    20457 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     9988 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_nullable_types_replacer.py
--rw-r--r--   0 root         (0) root         (0)    26816 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_one_hot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    25966 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)    18683 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_oversampler.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_pca.py
--rw-r--r--   0 root         (0) root         (0)    12025 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5021 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)    21607 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)    18269 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)    10542 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8928 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_target_encoder.py
--rw-r--r--   0 root         (0) root         (0)     8683 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    30311 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    22891 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_time_series_imputer.py
--rw-r--r--   0 root         (0) root         (0)     9937 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     5494 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_undersampler.py
--rw-r--r--   0 root         (0) root         (0)    12231 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2792 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/component_tests/test_xgboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)    79969 2023-03-27 19:04:50.000000 evalml-0.72.0/evalml/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     9729 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data/tips.csv
--rw-r--r--   0 root         (0) root         (0)    61194 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data/titanic.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/data_checks_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24199 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check_action.py
--rw-r--r--   0 root         (0) root         (0)    20667 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check_message.py
--rw-r--r--   0 root         (0) root         (0)    30071 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    19715 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)    12185 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    27859 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    26417 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8238 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5609 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)    16756 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4898 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/data_checks_tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/demo_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/demo_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/demo_tests/test_datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/dependency_update_check/
--rw-r--r--   0 root         (0) root         (0)      636 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
--rw-r--r--   0 root         (0) root         (0)      608 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/dependency_update_check/minimum_requirements.txt
--rw-r--r--   0 root         (0) root         (0)      760 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9843 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
--rw-r--r--   0 root         (0) root         (0)     3095 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/integration_tests/test_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)     7110 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/integration_tests/test_time_series_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/model_family_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_family_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_family_tests/test_model_family.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14158 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
--rw-r--r--   0 root         (0) root         (0)    67430 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
--rw-r--r--   0 root         (0) root         (0)     9790 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
--rw-r--r--   0 root         (0) root         (0)    19357 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)    14744 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)    26774 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    98439 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
--rw-r--r--   0 root         (0) root         (0)    29313 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
--rw-r--r--   0 root         (0) root         (0)    26181 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/model_understanding_tests/test_visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/objective_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/test_binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/test_fraud_detection.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/test_lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/test_objectives.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/test_sla.py
--rw-r--r--   0 root         (0) root         (0)    27155 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/objective_tests/test_standard_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
--rw-r--r--   0 root         (0) root         (0)     4688 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3652 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
--rw-r--r--   0 root         (0) root         (0)    94249 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/test_component_graph.py
--rw-r--r--   0 root         (0) root         (0)     8969 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/test_graphs.py
--rw-r--r--   0 root         (0) root         (0)    50293 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
--rw-r--r--   0 root         (0) root         (0)   101164 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/test_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    65166 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/preprocessing_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/preprocessing_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/preprocessing_tests/test_no_split.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/preprocessing_tests/test_split_data.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/problem_type_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/problem_type_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6537 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/problem_type_tests/test_problem_types.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/test_all_test_dirs_included.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/tuner_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/tuner_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/tuner_tests/test_random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     9170 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/tuner_tests/test_skopt_tuner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tests/utils_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/utils_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/utils_tests/test_cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    30958 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/utils_tests/test_gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     4685 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/utils_tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/utils_tests/test_nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)    13332 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tests/utils_tests/test_woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/tuners/
--rw-r--r--   0 root         (0) root         (0)      316 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tuners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tuners/grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     4675 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tuners/random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tuners/skopt_tuner.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tuners/tuner.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/tuners/tuner_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml/utils/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/base_meta.py
--rw-r--r--   0 root         (0) root         (0)     6540 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    26932 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     4265 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/update_checker.py
--rw-r--r--   0 root         (0) root         (0)     6871 2023-03-27 19:04:51.000000 evalml-0.72.0/evalml/utils/woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8233 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20684 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1245 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-27 19:05:04.000000 evalml-0.72.0/evalml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5037 2023-03-27 19:04:51.000000 evalml-0.72.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 19:05:04.000000 evalml-0.72.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-04-11 21:22:59.000000 evalml-0.73.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-04-11 21:23:11.000000 evalml-0.73.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-04-11 21:22:59.000000 evalml-0.73.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/automl/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/automl/automl_algorithm/
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/automl_algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11921 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/automl_algorithm/automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    29236 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/automl_algorithm/default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    21384 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/automl_algorithm/iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    79400 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/automl_search.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/automl/engine/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/engine/cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/engine/dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)    15405 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/engine/engine_base.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/engine/sequential_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/progress.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/automl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/data_checks/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11989 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_check_action_code.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_check_message_code.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_check_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    25088 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/default_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    20762 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    11843 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    17159 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8124 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/data_checks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/demos/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      605 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/churn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/demos/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/diabetes.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/fraud.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/weather.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/demos/wine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/exceptions/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/model_family/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_family/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_family/model_family.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_family/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/model_understanding/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18388 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/_partial_dependence_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    15125 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    27420 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/partial_dependence_functions.py
+-rw-r--r--   0 root         (0) root         (0)    13556 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/permutation_importance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/model_understanding/prediction_explanations/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/prediction_explanations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/prediction_explanations/_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
+-rw-r--r--   0 root         (0) root         (0)    36936 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/prediction_explanations/_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15630 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/prediction_explanations/explainers.py
+-rw-r--r--   0 root         (0) root         (0)    22293 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/model_understanding/visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/objectives/
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/fraud_cost.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/multiclass_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/objective_base.py
+-rw-r--r--   0 root         (0) root         (0)      406 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/sensitivity_low_alert.py
+-rw-r--r--   0 root         (0) root         (0)    33865 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/standard_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/time_series_regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)     6835 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/objectives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/binary_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/binary_classification_pipeline_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    40232 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/component_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10149 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/component_base.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/component_base_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/ensemble/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/ensemble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/estimators/
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8797 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8530 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13466 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7329 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5128 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/column_selectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/dimensionality_reduction/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/encoders/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    13779 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    12206 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8253 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/imputer.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    11389 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5899 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    15805 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
+-rw-r--r--   0 root         (0) root         (0)     6461 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)    17526 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/samplers/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/samplers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     7283 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/samplers/oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     8265 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/samplers/undersampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/pipelines/components/transformers/scalers/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/scalers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/transformers/transformer.py
+-rw-r--r--   0 root         (0) root         (0)    18498 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/components/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/multiclass_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    33022 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/pipeline_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    17176 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/time_series_classification_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    15153 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/time_series_pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    12779 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/time_series_regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    53231 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/preprocessing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/preprocessing/data_splitters/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/preprocessing/data_splitters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/preprocessing/data_splitters/no_split.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/preprocessing/data_splitters/sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/preprocessing/data_splitters/time_series_split.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/preprocessing/data_splitters/training_validation_split.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/preprocessing/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/problem_types/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/problem_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/problem_types/problem_types.py
+-rw-r--r--   0 root         (0) root         (0)     6085 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/problem_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/automl_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/dask_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9622 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
+-rw-r--r--   0 root         (0) root         (0)    17604 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)    14529 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)   179131 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38707 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38820 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_classification.py
+-rw-r--r--   0 root         (0) root         (0)    15745 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_regression.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
+-rw-r--r--   0 root         (0) root         (0)    12934 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_automl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    33034 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_engine_base.py
+-rw-r--r--   0 root         (0) root         (0)    36749 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_search_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/automl_tests/test_time_series_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/component_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27084 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    11644 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8548 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_column_selector_transformers.py
+-rw-r--r--   0 root         (0) root         (0)    64838 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_components.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_en_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_en_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    15118 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_estimators.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_feature_selectors.py
+-rw-r--r--   0 root         (0) root         (0)    14950 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     9627 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
+-rw-r--r--   0 root         (0) root         (0)    25736 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_knn_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     8017 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_lda.py
+-rw-r--r--   0 root         (0) root         (0)    13414 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_lgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     9754 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_lgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_lsa.py
+-rw-r--r--   0 root         (0) root         (0)    20457 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_nullable_types_replacer.py
+-rw-r--r--   0 root         (0) root         (0)    26816 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_one_hot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    25966 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    19941 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_pca.py
+-rw-r--r--   0 root         (0) root         (0)    12025 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    23430 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    18269 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)    10542 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_target_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    30311 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    24722 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_time_series_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     6246 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_undersampler.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/component_tests/test_xgboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    80070 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     9729 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data/tips.csv
+-rw-r--r--   0 root         (0) root         (0)    61194 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data/titanic.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/data_checks_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24199 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)    29212 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    19715 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    12185 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    30182 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    26417 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8238 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    18212 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/data_checks_tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/demo_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/demo_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/demo_tests/test_datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/dependency_update_check/
+-rw-r--r--   0 root         (0) root         (0)      636 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
+-rw-r--r--   0 root         (0) root         (0)      608 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/dependency_update_check/minimum_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      760 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10709 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/integration_tests/test_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/integration_tests/test_time_series_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/model_family_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_family_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_family_tests/test_model_family.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14158 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)    67430 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    19357 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)    14744 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)    26774 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    98520 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
+-rw-r--r--   0 root         (0) root         (0)    29313 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
+-rw-r--r--   0 root         (0) root         (0)    26181 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/model_understanding_tests/test_visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/objective_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/test_binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/test_fraud_detection.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/test_lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/test_objectives.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/test_sla.py
+-rw-r--r--   0 root         (0) root         (0)    27155 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/objective_tests/test_standard_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
+-rw-r--r--   0 root         (0) root         (0)     4688 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
+-rw-r--r--   0 root         (0) root         (0)    94308 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/test_component_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8969 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/test_graphs.py
+-rw-r--r--   0 root         (0) root         (0)    49957 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
+-rw-r--r--   0 root         (0) root         (0)   101164 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/test_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    68369 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/preprocessing_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/preprocessing_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/preprocessing_tests/test_no_split.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/preprocessing_tests/test_split_data.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/problem_type_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/problem_type_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/problem_type_tests/test_problem_types.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/test_all_test_dirs_included.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/tuner_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/tuner_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/tuner_tests/test_random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     9170 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/tuner_tests/test_skopt_tuner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tests/utils_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/utils_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/utils_tests/test_cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30486 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/utils_tests/test_gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4685 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/utils_tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/utils_tests/test_nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tests/utils_tests/test_woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/tuners/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tuners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tuners/grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     4675 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tuners/random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tuners/skopt_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tuners/tuner.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/tuners/tuner_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml/utils/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/base_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    26270 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7066 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/update_checker.py
+-rw-r--r--   0 root         (0) root         (0)     6346 2023-04-11 21:22:59.000000 evalml-0.73.0/evalml/utils/woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20684 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 21:23:11.000000 evalml-0.73.0/evalml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5037 2023-04-11 21:22:59.000000 evalml-0.73.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 21:23:11.000000 evalml-0.73.0/setup.cfg
```

### Comparing `evalml-0.72.0/LICENSE` & `evalml-0.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/PKG-INFO` & `evalml-0.73.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.72.0
+Version: 0.73.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.72.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.73.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.72.0/README.md` & `evalml-0.73.0/README.md`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/__init__.py` & `evalml-0.73.0/evalml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", FutureWarning)
     warnings.simplefilter("ignore", DeprecationWarning)
     import skopt
 warnings.filterwarnings("ignore", category=FutureWarning)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-__version__ = "0.72.0"
+__version__ = "0.73.0"
```

### Comparing `evalml-0.72.0/evalml/automl/automl_algorithm/automl_algorithm.py` & `evalml-0.73.0/evalml/automl/automl_algorithm/automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/automl_algorithm/default_algorithm.py` & `evalml-0.73.0/evalml/automl/automl_algorithm/default_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/automl_algorithm/iterative_algorithm.py` & `evalml-0.73.0/evalml/automl/automl_algorithm/iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/automl_search.py` & `evalml-0.73.0/evalml/automl/automl_search.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/callbacks.py` & `evalml-0.73.0/evalml/automl/callbacks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/engine/cf_engine.py` & `evalml-0.73.0/evalml/automl/engine/cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/engine/dask_engine.py` & `evalml-0.73.0/evalml/automl/engine/dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/engine/engine_base.py` & `evalml-0.73.0/evalml/automl/engine/engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/engine/sequential_engine.py` & `evalml-0.73.0/evalml/automl/engine/sequential_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/pipeline_search_plots.py` & `evalml-0.73.0/evalml/automl/pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/progress.py` & `evalml-0.73.0/evalml/automl/progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/automl/utils.py` & `evalml-0.73.0/evalml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/__init__.py` & `evalml-0.73.0/evalml/data_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/class_imbalance_data_check.py` & `evalml-0.73.0/evalml/data_checks/class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/data_check.py` & `evalml-0.73.0/evalml/data_checks/data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/data_check_action.py` & `evalml-0.73.0/evalml/data_checks/data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/data_check_action_code.py` & `evalml-0.73.0/evalml/data_checks/data_check_action_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/data_check_action_option.py` & `evalml-0.73.0/evalml/data_checks/data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/data_check_message.py` & `evalml-0.73.0/evalml/data_checks/data_check_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 
 class DataCheckMessage:
     """Base class for a message returned by a DataCheck, tagged by name.
 
     Args:
         message (str): Message string.
-        data_check_name (str): Name of data check.
-        message_code (DataCheckMessageCode): Message code associated with message. Defaults to None.
-        details (dict): Additional useful information associated with the message. Defaults to None.
+        data_check_name (str): Name of the associated data check.
+        message_code (DataCheckMessageCode, optional): Message code associated with the message. Defaults to None.
+        details (dict, optional): Additional useful information associated with the message. Defaults to None.
+        action_options (list, optional): A list of `DataCheckActionOption`s associated with the message. Defaults to None.
     """
 
     message_type = None
 
     def __init__(
         self,
         message,
```

### Comparing `evalml-0.72.0/evalml/data_checks/data_check_message_code.py` & `evalml-0.73.0/evalml/data_checks/data_check_message_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/data_checks.py` & `evalml-0.73.0/evalml/data_checks/data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/datetime_format_data_check.py` & `evalml-0.73.0/evalml/data_checks/datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/default_data_checks.py` & `evalml-0.73.0/evalml/data_checks/default_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/id_columns_data_check.py` & `evalml-0.73.0/evalml/data_checks/id_columns_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/invalid_target_data_check.py` & `evalml-0.73.0/evalml/data_checks/invalid_target_data_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,33 @@
 
     Args:
         problem_type (str or ProblemTypes): The specific problem type to data check for.
             e.g. 'binary', 'multiclass', 'regression, 'time series regression'
         objective (str or ObjectiveBase): Name or instance of the objective class.
         n_unique (int): Number of unique target values to store when problem type is binary and target
             incorrectly has more than 2 unique values. Non-negative integer. If None, stores all unique values. Defaults to 100.
+        null_strategy (str): The type of action option that should be returned if the target is partially null.
+            The options are `impute` and `drop` (default).
+            `impute` - Will return a `DataCheckActionOption` for imputing the target column.
+            `drop` - Will return a `DataCheckActionOption` for dropping the null rows in the target column.
     """
 
     multiclass_continuous_threshold = 0.05
 
-    def __init__(self, problem_type, objective, n_unique=100):
+    def __init__(self, problem_type, objective, n_unique=100, null_strategy="drop"):
         self.problem_type = handle_problem_types(problem_type)
         self.objective = get_objective(objective)
         if n_unique is not None and n_unique <= 0:
             raise ValueError("`n_unique` must be a non-negative integer value.")
         self.n_unique = n_unique
+        if null_strategy is None or null_strategy.lower() not in ["impute", "drop"]:
+            raise ValueError(
+                "The acceptable values for 'null_strategy' are 'impute' and 'drop'.",
+            )
+        self.null_strategy = null_strategy
 
     def validate(self, X, y):
         """Check if the target data is considered invalid. If the input features argument is not None, it will be used to check that the target and features have the same dimensions and indices.
 
         Target data is considered invalid if:
             - Target is None.
             - Target has NaN or None values.
@@ -69,18 +78,18 @@
         Examples:
             >>> import pandas as pd
 
             Target values must be integers, doubles, or booleans.
 
             >>> X = pd.DataFrame({"col": [1, 2, 3, 1]})
             >>> y = pd.Series(["cat_1", "cat_2", "cat_1", "cat_2"])
-            >>> target_check = InvalidTargetDataCheck("regression", "R2")
+            >>> target_check = InvalidTargetDataCheck("regression", "R2", null_strategy="impute")
             >>> assert target_check.validate(X, y) == [
             ...     {
-            ...         "message": "Target is unsupported Unknown type. Valid Woodwork logical types include: integer, double, boolean, integer_nullable, boolean_nullable, age_nullable",
+            ...         "message": "Target is unsupported Unknown type. Valid Woodwork logical types include: integer, double, boolean, age, age_fractional, integer_nullable, boolean_nullable, age_nullable",
             ...         "data_check_name": "InvalidTargetDataCheck",
             ...         "level": "error",
             ...         "details": {"columns": None, "rows": None, "unsupported_type": "unknown"},
             ...         "code": "TARGET_UNSUPPORTED_TYPE",
             ...         "action_options": []
             ...     },
             ...     {
@@ -112,15 +121,15 @@
             >>> assert target_check.validate(None, y) == [
             ...     {
             ...         "message": "2 row(s) (50.0%) of target values are null",
             ...         "data_check_name": "InvalidTargetDataCheck",
             ...         "level": "error",
             ...         "details": {
             ...             "columns": None,
-            ...             "rows": None,
+            ...             "rows": [1, 3],
             ...             "num_null_rows": 2,
             ...             "pct_null_rows": 50.0
             ...         },
             ...         "code": "TARGET_HAS_NULL",
             ...         "action_options": [
             ...            {
             ...                 "code": "IMPUTE_COL",
@@ -239,45 +248,59 @@
                     details={},
                 ).to_dict(),
             )
             return messages
         elif null_rows.any():
             num_null_rows = null_rows.sum()
             pct_null_rows = null_rows.mean() * 100
+            rows_to_drop = null_rows.loc[null_rows].index.tolist()
+
+            action_options = []
+            impute_action_option = DataCheckActionOption(
+                DataCheckActionCode.IMPUTE_COL,
+                data_check_name=self.name,
+                parameters={
+                    "impute_strategy": {
+                        "parameter_type": DCAOParameterType.GLOBAL,
+                        "type": "category",
+                        "categories": ["mean", "most_frequent"]
+                        if is_regression(self.problem_type)
+                        else ["most_frequent"],
+                        "default_value": "mean"
+                        if is_regression(self.problem_type)
+                        else "most_frequent",
+                    },
+                },
+                metadata={"is_target": True},
+            )
+            drop_action_option = DataCheckActionOption(
+                DataCheckActionCode.DROP_ROWS,
+                data_check_name=self.name,
+                metadata={"is_target": True, "rows": rows_to_drop},
+            )
+
+            if self.null_strategy.lower() == "impute":
+                action_options.append(impute_action_option)
+            elif self.null_strategy.lower() == "drop":
+                action_options.append(drop_action_option)
+
             messages.append(
                 DataCheckError(
                     message="{} row(s) ({}%) of target values are null".format(
                         num_null_rows,
                         pct_null_rows,
                     ),
                     data_check_name=self.name,
                     message_code=DataCheckMessageCode.TARGET_HAS_NULL,
                     details={
                         "num_null_rows": num_null_rows,
                         "pct_null_rows": pct_null_rows,
+                        "rows": rows_to_drop,
                     },
-                    action_options=[
-                        DataCheckActionOption(
-                            DataCheckActionCode.IMPUTE_COL,
-                            data_check_name=self.name,
-                            parameters={
-                                "impute_strategy": {
-                                    "parameter_type": DCAOParameterType.GLOBAL,
-                                    "type": "category",
-                                    "categories": ["mean", "most_frequent"]
-                                    if is_regression(self.problem_type)
-                                    else ["most_frequent"],
-                                    "default_value": "mean"
-                                    if is_regression(self.problem_type)
-                                    else "most_frequent",
-                                },
-                            },
-                            metadata={"is_target": True},
-                        ),
-                    ],
+                    action_options=action_options,
                 ).to_dict(),
             )
 
         return messages
 
     def _check_target_and_features_compatible(self, X, y, messages):
         if X is not None:
```

### Comparing `evalml-0.72.0/evalml/data_checks/multicollinearity_data_check.py` & `evalml-0.73.0/evalml/data_checks/multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/no_variance_data_check.py` & `evalml-0.73.0/evalml/data_checks/no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/null_data_check.py` & `evalml-0.73.0/evalml/data_checks/null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/outliers_data_check.py` & `evalml-0.73.0/evalml/data_checks/outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/sparsity_data_check.py` & `evalml-0.73.0/evalml/data_checks/sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/target_distribution_data_check.py` & `evalml-0.73.0/evalml/data_checks/target_distribution_data_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             >>> y = pd.Series([1, 1, 1, 2, 2, 3, 4, 4, 5, 5, 5])
             >>> assert target_check.validate(None, y) == []
             ...
             ...
             >>> y = pd.Series(pd.date_range("1/1/21", periods=10))
             >>> assert target_check.validate(None, y) == [
             ...     {
-            ...         "message": "Target is unsupported datetime type. Valid Woodwork logical types include: integer, double",
+            ...         "message": "Target is unsupported datetime type. Valid Woodwork logical types include: integer, double, age, age_fractional",
             ...         "data_check_name": "TargetDistributionDataCheck",
             ...         "level": "error",
             ...         "details": {"columns": None, "rows": None, "unsupported_type": "datetime"},
             ...         "code": "TARGET_UNSUPPORTED_TYPE",
             ...         "action_options": []
             ...     }
             ... ]
@@ -86,14 +86,16 @@
             )
             return messages
 
         y = infer_feature_types(y)
         allowed_types = [
             ww.logical_types.Integer.type_string,
             ww.logical_types.Double.type_string,
+            ww.logical_types.Age.type_string,
+            ww.logical_types.AgeFractional.type_string,
         ]
         is_supported_type = y.ww.logical_type.type_string in allowed_types
 
         if not is_supported_type:
             messages.append(
                 DataCheckError(
                     message="Target is unsupported {} type. Valid Woodwork logical types include: {}".format(
```

### Comparing `evalml-0.72.0/evalml/data_checks/target_leakage_data_check.py` & `evalml-0.73.0/evalml/data_checks/target_leakage_data_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,33 +17,32 @@
     If method='mutual_info', this data check uses mutual information and supports all target and feature types.
     Other correlation metrics only support binary with numeric and boolean dtypes. This method will return a value in [-1, 1] if other correlation metrics are selected
     and will returns a value in [0, 1] if mutual information is selected. Correlation metrics available can be found in Woodwork's
     `dependence_dict method <https://woodwork.alteryx.com/en/stable/generated/woodwork.table_accessor.WoodworkTableAccessor.dependence_dict.html#woodwork.table_accessor.WoodworkTableAccessor.dependence_dict>`_.
 
     Args:
         pct_corr_threshold (float): The correlation threshold to be considered leakage. Defaults to 0.95.
-        method (string): The method to determine correlation. Use 'max' for the maximum correlation, or for specific correlation metrics, use their name (ie 'mutual_info' for mutual information, 'pearson' for Pearson correlation, etc).
+        method (string): The method to determine correlation. Use 'all' or 'max' for the maximum correlation, or for specific correlation metrics, use their name (ie 'mutual_info' for mutual information, 'pearson' for Pearson correlation, etc).
             possible methods can be found in Woodwork's `config <https://woodwork.alteryx.com/en/stable/guides/setting_config_options.html?highlight=config#Viewing-Config-Settings>`_, under `correlation_metrics`.
-            Excludes 'all'. Defaults to 'mutual_info'.
+            Defaults to 'all'.
     """
 
-    def __init__(self, pct_corr_threshold=0.95, method="mutual_info"):
+    def __init__(self, pct_corr_threshold=0.95, method="all"):
         if pct_corr_threshold < 0 or pct_corr_threshold > 1:
             raise ValueError(
                 "pct_corr_threshold must be a float between 0 and 1, inclusive.",
             )
         methods = CONFIG_DEFAULTS["correlation_metrics"]
         if method not in methods:
             raise ValueError(
                 f"Method '{method}' not in available correlation methods. Available methods include {methods}",
             )
-        if method == "all":
-            raise ValueError("Cannot use 'all' as the method")
         self.pct_corr_threshold = pct_corr_threshold
         self.method = method
+        self._method_to_check = "max" if method == "all" else method
 
     def _calculate_dependence(self, X, y):
         highly_corr_cols = []
         X2 = X.ww.copy()
         target_str = "target_y"
         while target_str in list(X2.columns):
             target_str += "_y"
@@ -56,15 +55,15 @@
         except KeyError:
             # keyError raised when the target does not appear due to incompatibility with the metric, return []
             return []
         highly_corr_cols = sorted(
             [
                 corr_info["column_1"]
                 for corr_info in dep_corr
-                if abs(corr_info[self.method]) >= self.pct_corr_threshold
+                if abs(corr_info[self._method_to_check]) >= self.pct_corr_threshold
             ],
             key=lambda x: X2.columns.tolist().index(x),
         )
         return highly_corr_cols
 
     def validate(self, X, y):
         """Check if any of the features are highly correlated with the target by using mutual information, Pearson correlation, and/or Spearman correlation.
```

### Comparing `evalml-0.72.0/evalml/data_checks/ts_parameters_data_check.py` & `evalml-0.73.0/evalml/data_checks/ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/ts_splitting_data_check.py` & `evalml-0.73.0/evalml/data_checks/ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/uniqueness_data_check.py` & `evalml-0.73.0/evalml/data_checks/uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/data_checks/utils.py` & `evalml-0.73.0/evalml/data_checks/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/breast_cancer.py` & `evalml-0.73.0/evalml/demos/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/churn.py` & `evalml-0.73.0/evalml/demos/churn.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/data/churn.csv` & `evalml-0.73.0/evalml/demos/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/data/daily-min-temperatures.csv` & `evalml-0.73.0/evalml/demos/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/data/fraud_transactions.csv.gz` & `evalml-0.73.0/evalml/demos/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/diabetes.py` & `evalml-0.73.0/evalml/demos/diabetes.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/fraud.py` & `evalml-0.73.0/evalml/demos/fraud.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/weather.py` & `evalml-0.73.0/evalml/demos/weather.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/demos/wine.py` & `evalml-0.73.0/evalml/demos/wine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/exceptions/__init__.py` & `evalml-0.73.0/evalml/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/exceptions/exceptions.py` & `evalml-0.73.0/evalml/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_family/model_family.py` & `evalml-0.73.0/evalml/model_family/model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_family/utils.py` & `evalml-0.73.0/evalml/model_family/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/__init__.py` & `evalml-0.73.0/evalml/model_understanding/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py` & `evalml-0.73.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/_partial_dependence_utils.py` & `evalml-0.73.0/evalml/model_understanding/_partial_dependence_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/decision_boundary.py` & `evalml-0.73.0/evalml/model_understanding/decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/feature_explanations.py` & `evalml-0.73.0/evalml/model_understanding/feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/force_plots.py` & `evalml-0.73.0/evalml/model_understanding/force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/metrics.py` & `evalml-0.73.0/evalml/model_understanding/metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/partial_dependence_functions.py` & `evalml-0.73.0/evalml/model_understanding/partial_dependence_functions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/permutation_importance.py` & `evalml-0.73.0/evalml/model_understanding/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/prediction_explanations/_algorithms.py` & `evalml-0.73.0/evalml/model_understanding/prediction_explanations/_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py` & `evalml-0.73.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/prediction_explanations/_user_interface.py` & `evalml-0.73.0/evalml/model_understanding/prediction_explanations/_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/prediction_explanations/explainers.py` & `evalml-0.73.0/evalml/model_understanding/prediction_explanations/explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/model_understanding/visualizations.py` & `evalml-0.73.0/evalml/model_understanding/visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/__init__.py` & `evalml-0.73.0/evalml/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/binary_classification_objective.py` & `evalml-0.73.0/evalml/objectives/binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/cost_benefit_matrix.py` & `evalml-0.73.0/evalml/objectives/cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/fraud_cost.py` & `evalml-0.73.0/evalml/objectives/fraud_cost.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/lead_scoring.py` & `evalml-0.73.0/evalml/objectives/lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/objective_base.py` & `evalml-0.73.0/evalml/objectives/objective_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/sensitivity_low_alert.py` & `evalml-0.73.0/evalml/objectives/sensitivity_low_alert.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/standard_metrics.py` & `evalml-0.73.0/evalml/objectives/standard_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/objectives/utils.py` & `evalml-0.73.0/evalml/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/__init__.py` & `evalml-0.73.0/evalml/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/binary_classification_pipeline.py` & `evalml-0.73.0/evalml/pipelines/binary_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/binary_classification_pipeline_mixin.py` & `evalml-0.73.0/evalml/pipelines/binary_classification_pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/classification_pipeline.py` & `evalml-0.73.0/evalml/pipelines/classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/component_graph.py` & `evalml-0.73.0/evalml/pipelines/component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/component_base.py` & `evalml-0.73.0/evalml/pipelines/components/component_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/component_base_meta.py` & `evalml-0.73.0/evalml/pipelines/components/component_base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py` & `evalml-0.73.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,30 +185,34 @@
             X (pd.DataFrame): The input training data of shape [n_samples, n_features].
             y (pd.Series): The target training data of length [n_samples].
 
         Returns:
             self
         """
         X = infer_feature_types(X)
-        X_encoded = self._encode_categories(X, fit=True)
-        y_encoded = self._encode_labels(y)
+        if y is not None:
+            y = infer_feature_types(y)
+        X_d, y_d = self._handle_nullable_types(X, y)
+        X_encoded = self._encode_categories(X_d, fit=True)
+        y_encoded = self._encode_labels(y_d)
         self._component_obj.fit(X_encoded, y_encoded)
         return self
 
     def predict(self, X):
         """Make predictions using the fitted LightGBM classifier.
 
         Args:
             X (pd.DataFrame): Data of shape [n_samples, n_features].
 
         Returns:
             pd.DataFrame: Predicted values.
         """
         X_encoded = self._encode_categories(X)
-        predictions = super().predict(X_encoded)
+        X_d, _ = self._handle_nullable_types(X_encoded)
+        predictions = super().predict(X_d)
         if not self._label_encoder:
             return predictions
         predictions = self._label_encoder.inverse_transform(
             predictions.astype(np.int64),
         )
         return predictions
 
@@ -218,8 +222,9 @@
         Args:
             X (pd.DataFrame): Data of shape [n_samples, n_features].
 
         Returns:
             pd.DataFrame: Predicted probability values.
         """
         X_encoded = self._encode_categories(X)
-        return super().predict_proba(X_encoded)
+        X_d, _ = self._handle_nullable_types(X_encoded)
+        return super().predict_proba(X_d)
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/estimator.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import pandas as pd
 from skopt.space import Integer
 
 from evalml.model_family import ModelFamily
 from evalml.pipelines.components.estimators import Estimator
 from evalml.problem_types import ProblemTypes
 from evalml.utils import (
-    downcast_int_nullable_to_double,
     import_or_raise,
     infer_feature_types,
 )
 
 
 class ARIMARegressor(Estimator):
     """Autoregressive Integrated Moving Average Model. The three parameters (p, d, q) are the AR order, the degree of differencing, and the MA order. More information here: https://www.statsmodels.org/devel/generated/statsmodels.tsa.arima.model.ARIMA.html.
@@ -62,21 +61,14 @@
     """ModelFamily.ARIMA"""
     supported_problem_types = [ProblemTypes.TIME_SERIES_REGRESSION]
     """[ProblemTypes.TIME_SERIES_REGRESSION]"""
 
     max_rows = 1000
     max_cols = 7
 
-    # ARIMARegressor doesn't support BooleanNullable not because of nullable type
-    # incompatibilities but because we do not handle their null values correctly
-    # https://github.com/alteryx/evalml/issues/4009
-    # IntegerNullable incompatibility: https://github.com/alteryx/evalml/issues/4015
-    # TODO: Remove when support is added https://github.com/alteryx/evalml/issues/4016
-    _integer_nullable_incompatibilities = ["X"]
-
     def __init__(
         self,
         time_index: Optional[Hashable] = None,
         trend: Optional[str] = None,
         start_p: int = 2,
         d: int = 0,
         start_q: int = 2,
@@ -209,18 +201,17 @@
 
         Returns:
             self
 
         Raises:
             ValueError: If y was not passed in.
         """
-        if X is not None:
-            X = downcast_int_nullable_to_double(X)
-            X = X.fillna(X.mean())
         X, y = self._manage_woodwork(X, y)
+        if X is not None:
+            X = X.ww.fillna(X.mean())
         if y is None:
             raise ValueError("ARIMA Regressor requires y as input.")
 
         sp = self._get_sp(X)
         self._component_obj.sp = sp
         self.last_X_index = X.index[-1] if X is not None else y.index
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from skopt.space import Integer, Real
 
 from evalml.model_family import ModelFamily
 from evalml.pipelines.components.estimators import Estimator
 from evalml.pipelines.components.utils import handle_float_categories_for_catboost
 from evalml.problem_types import ProblemTypes
 from evalml.utils import (
-    downcast_int_nullable_to_double,
     import_or_raise,
     infer_feature_types,
 )
 
 
 class CatBoostRegressor(Estimator):
     """CatBoost Regressor, a regressor that uses gradient-boosting on decision trees. CatBoost is an open-source library and natively supports categorical features.
@@ -109,15 +108,14 @@
         Returns:
             self
         """
         X = infer_feature_types(X)
         cat_cols = list(X.ww.select("category", return_schema=True).columns)
         self.input_feature_names = list(X.columns)
         X, y = super()._manage_woodwork(X, y)
-        X = downcast_int_nullable_to_double(X)
 
         X = handle_float_categories_for_catboost(X)
         self._component_obj.fit(X, y, silent=True, cat_features=cat_cols)
         return self
 
     def predict(self, X):
         """Make predictions using the fitted CatBoost regressor.
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/et_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,14 @@
         "sp": Integer(2, 8),
     }"""
     model_family = ModelFamily.EXPONENTIAL_SMOOTHING
     """ModelFamily.EXPONENTIAL_SMOOTHING"""
     supported_problem_types = [ProblemTypes.TIME_SERIES_REGRESSION]
     """[ProblemTypes.TIME_SERIES_REGRESSION]"""
 
-    # Incompatibility: https://github.com/alteryx/evalml/issues/3926
-    # TODO: Remove when support is added https://github.com/alteryx/evalml/issues/4016
-    _integer_nullable_incompatibilities = ["y"]
-    _boolean_nullable_incompatibilities = ["y"]
-
     def __init__(
         self,
         trend: Optional[str] = None,
         damped_trend: bool = False,
         seasonal: Optional[str] = None,
         sp: int = 2,
         n_jobs: int = -1,
@@ -162,15 +157,14 @@
 
         Returns:
             dict: Prediction intervals, keys are in the format {coverage}_lower or {coverage}_upper.
         """
         if coverage is None:
             coverage = [0.95]
         X, y = self._manage_woodwork(X, y)
-
         # Accesses the fitted statsmodels model within sktime
         # nsimulations represents how many steps should be simulated
         # repetitions represents the number of simulations that should be run (confusing, I know)
         # anchor represents where the simulations should start from (forecasting is done from the "end")
         y_pred = self._component_obj._fitted_forecaster.simulate(
             nsimulations=X.shape[0],
             repetitions=400,
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from evalml.model_family import ModelFamily
 from evalml.pipelines.components.estimators import Estimator
 from evalml.problem_types import ProblemTypes
 from evalml.utils import (
     SEED_BOUNDS,
     _rename_column_names_to_numeric,
-    downcast_int_nullable_to_double,
     import_or_raise,
     infer_feature_types,
 )
 
 
 class LightGBMRegressor(Estimator):
     """LightGBM Regressor.
@@ -166,22 +165,23 @@
 
         Returns:
             self
         """
         X_encoded = self._encode_categories(X, fit=True)
         if y is not None:
             y = infer_feature_types(y)
-        X_encoded = downcast_int_nullable_to_double(X_encoded)
-        self._component_obj.fit(X_encoded, y)
+        X_d, y_d = self._handle_nullable_types(X_encoded, y)
+        self._component_obj.fit(X_d, y_d)
         return self
 
     def predict(self, X):
         """Make predictions using fitted LightGBM regressor.
 
         Args:
             X (pd.DataFrame): Data of shape [n_samples, n_features].
 
         Returns:
             pd.Series: Predicted values.
         """
         X_encoded = self._encode_categories(X)
-        return super().predict(X_encoded)
+        X_d, _ = self._handle_nullable_types(X_encoded)
+        return super().predict(X_d)
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py` & `evalml-0.73.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/column_selectors.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/column_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/encoders/label_encoder.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/encoders/label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/encoders/target_encoder.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/imputers/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/imputers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/imputers/imputer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/imputers/imputer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Component that imputes missing data according to a specified imputation strategy."""
 import pandas as pd
-from woodwork import init_series
 
 from evalml.pipelines.components.transformers import Transformer
 from evalml.pipelines.components.transformers.imputers import KNNImputer, SimpleImputer
-from evalml.utils import downcast_nullable_types, infer_feature_types
-from evalml.utils.gen_utils import is_categorical_actually_boolean
+from evalml.utils import infer_feature_types
 
 
 class Imputer(Transformer):
     """Imputes missing data according to a specified imputation strategy.
 
     Args:
         categorical_impute_strategy (string): Impute strategy to use for string, object, boolean, categorical dtypes. Valid values include "most_frequent" and "constant".
@@ -115,37 +113,32 @@
         X = infer_feature_types(X)
         cat_cols = list(X.ww.select(["category"], return_schema=True).columns)
         bool_cols = list(
             X.ww.select(["BooleanNullable", "Boolean"], return_schema=True).columns,
         )
         numeric_cols = list(X.ww.select(["numeric"], return_schema=True).columns)
 
-        # TODO: Remove this when columns with True/False/NaN are inferred properly as BooleanNullable.
-        # If columns with boolean values and NaN are included with normal categorical columns, columns
-        # with object dtypes are attempted to be cast to float64 with scikit-learn 1.1.  So we separate
-        # boolean and categorical into separate imputers.
-        for col in cat_cols:
-            if is_categorical_actually_boolean(X, col):
-                cat_cols.remove(col)
-                bool_cols.append(col)
-
         nan_ratio = X.isna().sum() / X.shape[0]
         self._all_null_cols = nan_ratio[nan_ratio == 1].index.tolist()
 
-        X_numerics = X[[col for col in numeric_cols if col not in self._all_null_cols]]
+        X_numerics = X.ww[
+            [col for col in numeric_cols if col not in self._all_null_cols]
+        ]
         if len(X_numerics.columns) > 0:
             self._numeric_imputer.fit(X_numerics, y)
             self._numeric_cols = X_numerics.columns
 
-        X_categorical = X[[col for col in cat_cols if col not in self._all_null_cols]]
+        X_categorical = X.ww[
+            [col for col in cat_cols if col not in self._all_null_cols]
+        ]
         if len(X_categorical.columns) > 0:
             self._categorical_imputer.fit(X_categorical, y)
             self._categorical_cols = X_categorical.columns
 
-        X_boolean = X[[col for col in bool_cols if col not in self._all_null_cols]]
+        X_boolean = X.ww[[col for col in bool_cols if col not in self._all_null_cols]]
         if len(X_boolean.columns) > 0:
             self._boolean_imputer.fit(X_boolean, y)
             self._boolean_cols = X_boolean.columns
         return self
 
     def transform(self, X, y=None):
         """Transforms data X by imputing missing values.
@@ -160,29 +153,31 @@
         X = infer_feature_types(X)
         if len(self._all_null_cols) == X.shape[1]:
             df = pd.DataFrame(index=X.index)
             df.ww.init()
             return df
 
         X_no_all_null = X.ww.drop(self._all_null_cols)
+        original_schema = X_no_all_null.ww.schema
+        new_ltypes = None
 
         if self._numeric_cols is not None and len(self._numeric_cols) > 0:
             X_numeric = X.ww[self._numeric_cols.tolist()]
             imputed = self._numeric_imputer.transform(X_numeric)
-            for numeric_col in X_numeric.columns:
-                X_no_all_null.ww[numeric_col] = init_series(
-                    imputed[numeric_col],
-                    logical_type="Double",
-                )
+            X_no_all_null[X_numeric.columns] = imputed
+            # Numeric imputing may have changed logical types because of use of _get_new_logical_types_for_imputed_data
+            if imputed.ww.schema is None:
+                imputed.ww.init()
+            new_ltypes = imputed.ww.logical_types
 
         if self._categorical_cols is not None and len(self._categorical_cols) > 0:
             X_categorical = X.ww[self._categorical_cols.tolist()]
             imputed = self._categorical_imputer.transform(X_categorical)
             X_no_all_null[X_categorical.columns] = imputed
 
         if self._boolean_cols is not None and len(self._boolean_cols) > 0:
             X_boolean = X.ww[self._boolean_cols.tolist()]
             imputed = self._boolean_imputer.transform(X_boolean)
             X_no_all_null[X_boolean.columns] = imputed
 
-        X_no_all_null = downcast_nullable_types(X_no_all_null, ignore_null_cols=False)
+        X_no_all_null.ww.init(schema=original_schema, logical_types=new_ltypes)
         return X_no_all_null
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 """Component that imputes missing data according to a specified imputation strategy."""
 import pandas as pd
 import woodwork
 from sklearn.impute import SimpleImputer as SkImputer
-from woodwork.logical_types import Double
 
 from evalml.pipelines.components.transformers import Transformer
-from evalml.pipelines.components.utils import (
-    drop_natural_language_columns,
-    set_boolean_columns_to_integer,
-)
 from evalml.utils import infer_feature_types
-from evalml.utils.gen_utils import is_categorical_actually_boolean
+from evalml.utils.nullable_type_utils import _get_new_logical_types_for_imputed_data
 
 
 class SimpleImputer(Transformer):
     """Imputes missing data according to a specified imputation strategy.  Natural language columns are ignored.
 
     Args:
         impute_strategy (string): Impute strategy to use. Valid values include "mean", "median", "most_frequent", "constant" for
@@ -65,99 +60,95 @@
 
         """
         X = infer_feature_types(X)
 
         if set([lt.type_string for lt in X.ww.logical_types.values()]) == {
             "boolean",
             "categorical",
-        } and not all(
-            [
-                is_categorical_actually_boolean(X, col)
-                for col in X.ww.select("Categorical")
-            ],
-        ):
+        }:
             raise ValueError(
                 "SimpleImputer cannot handle dataframes with both boolean and categorical features.  Use Imputer instead.",
             )
 
         nan_ratio = X.isna().sum() / X.shape[0]
-        self._all_null_cols = nan_ratio[nan_ratio == 1].index.tolist()
-
-        X, _ = drop_natural_language_columns(X)
 
-        # Convert any boolean columns to IntegerNullable, but keep track of the columns so they can be converted back
-        self._boolean_cols = list(
+        # Keep track of the different types of data in X
+        self._all_null_cols = nan_ratio[nan_ratio == 1].index.tolist()
+        self._natural_language_cols = list(
             X.ww.select(
-                include=["Boolean", "BooleanNullable"],
+                "NaturalLanguage",
                 return_schema=True,
-            ).columns,
+            ).columns.keys(),
         )
-        # Make sure we're tracking Categorical columns that should be boolean as well
-        self._boolean_cols.extend(
-            [
-                col
-                for col in X.ww.select("Categorical")
-                if is_categorical_actually_boolean(X, col)
-            ],
-        )
-        X = set_boolean_columns_to_integer(X)
 
-        # If the Dataframe only had natural language columns, do nothing.
-        if X.shape[1] == 0:
+        # Only impute data that is not natural language columns or fully null
+        self._cols_to_impute = [
+            col
+            for col in X.columns
+            if col not in self._natural_language_cols and col not in self._all_null_cols
+        ]
+
+        # If there are no columns to impute, return early
+        if not self._cols_to_impute:
             return self
+
+        X = X[self._cols_to_impute]
+        if (X.dtypes == bool).all():
+            # Ensure that _component_obj still gets fit so that if any of the dtypes are different
+            # at transform, we've fit the component. This is needed because sklearn doesn't allow
+            # data with only bool dtype to be passed in.
+            X = X.astype("boolean")
+
         self._component_obj.fit(X, y)
         return self
 
     def transform(self, X, y=None):
         """Transforms input by imputing missing values. 'None' and np.nan values are treated as the same.
 
         Args:
             X (pd.DataFrame): Data to transform.
             y (pd.Series, optional): Ignored.
 
         Returns:
             pd.DataFrame: Transformed X
         """
+        # Record original data
         X = infer_feature_types(X)
         original_schema = X.ww.schema
-        X = set_boolean_columns_to_integer(X)
-
-        not_all_null_cols = [col for col in X.columns if col not in self._all_null_cols]
         original_index = X.index
 
-        # Drop natural language columns and transform the other columns
-        X_t, natural_language_cols = drop_natural_language_columns(X)
-        if X_t.shape[1] == 0:
-            return X
-        not_all_null_or_natural_language_cols = [
-            col for col in not_all_null_cols if col not in natural_language_cols
-        ]
+        # separate out just the columns we are imputing
+        X_t = X[self._cols_to_impute]
+        if not self._cols_to_impute or (X_t.dtypes == bool).all():
+            # If there are no columns to impute or all columns to impute are bool dtype,
+            # which will never have null values, return the original data without any fully null columns
+            not_all_null_cols = [
+                col for col in X.columns if col not in self._all_null_cols
+            ]
+            return X.ww[not_all_null_cols]
 
+        # Transform the data
         X_t = self._component_obj.transform(X_t)
-        X_t = pd.DataFrame(X_t, columns=not_all_null_or_natural_language_cols)
+        X_t = pd.DataFrame(X_t, columns=self._cols_to_impute)
 
-        new_schema = original_schema.get_subset_schema(X_t.columns)
+        # Reinit woodwork, maintaining original types where possible
+        imputed_schema = original_schema.get_subset_schema(self._cols_to_impute)
+        new_logical_types = _get_new_logical_types_for_imputed_data(
+            impute_strategy=self.impute_strategy,
+            original_schema=imputed_schema,
+        )
+        X_t.ww.init(schema=imputed_schema, logical_types=new_logical_types)
 
-        # Iterate through previously saved boolean columns and convert them back to boolean
-        for col in self._boolean_cols:
-            X_t[col] = X_t[col].astype(bool)
-
-        # Convert Nullable Integers to Doubles for the "mean" and "median" strategies
-        if self.impute_strategy in ["mean", "median"]:
-            nullable_int_cols = X.ww.select(["IntegerNullable"], return_schema=True)
-            nullable_int_cols = [x for x in nullable_int_cols.columns.keys()]
-            for col in nullable_int_cols:
-                new_schema.set_types({col: Double})
-        X_t.ww.init(schema=new_schema)
-
-        # Add back in natural language columns, unchanged
-        if len(natural_language_cols) > 0:
-            X_t = woodwork.concat_columns([X_t, X[natural_language_cols]])
+        # Add back in the unchanged original natural language columns that we want to keep
+        if len(self._natural_language_cols) > 0:
+            X_t = woodwork.concat_columns([X_t, X.ww[self._natural_language_cols]])
+            # reorder columns to match original
+            X_t = X_t.ww[[col for col in original_schema.columns if col in X_t.columns]]
 
-        if not_all_null_or_natural_language_cols:
+        if self._cols_to_impute:
             X_t.index = original_index
         return X_t
 
     def fit_transform(self, X, y=None):
         """Fits on X and transforms X.
 
         Args:
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/imputers/target_imputer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/imputers/target_imputer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Component that imputes missing target data according to a specified imputation strategy."""
 from functools import wraps
 
 import pandas as pd
 import woodwork as ww
 from sklearn.impute import SimpleImputer as SkImputer
-from woodwork.logical_types import Categorical, Integer, IntegerNullable
 
 from evalml.exceptions import ComponentNotYetFittedError
 from evalml.pipelines.components import ComponentBaseMeta
 from evalml.pipelines.components.transformers import Transformer
 from evalml.utils import infer_feature_types
+from evalml.utils.nullable_type_utils import _get_new_logical_types_for_imputed_data
 
 
 class TargetImputerMeta(ComponentBaseMeta):
     """A version of the ComponentBaseMeta class which handles when input features is None."""
 
     @classmethod
     def check_for_fit(cls, method):
@@ -89,17 +89,17 @@
         if y is None:
             return self
         y = infer_feature_types(y)
         if all(y.isnull()):
             raise TypeError("Provided target full of nulls.")
         y = y.to_frame()
 
-        # Convert all bool dtypes to category for fitting
+        # Return early if all the columns are bool dtype, which will never have null values
         if (y.dtypes == bool).all():
-            y = y.astype("category")
+            return y
 
         self._component_obj.fit(y)
         return self
 
     def transform(self, X, y):
         """Transforms input target data by imputing missing values. 'None' and np.nan values are treated as the same.
 
@@ -113,41 +113,29 @@
         if X is not None:
             X = infer_feature_types(X)
         if y is None:
             return X, None
         y_ww = infer_feature_types(y)
         y_df = y_ww.ww.to_frame()
 
-        # Return early since bool dtype doesn't support nans and sklearn errors if all cols are bool
+        # Return early if all the columns are bool dtype, which will never have null values
         if (y_df.dtypes == bool).all():
             return X, y_ww
 
         transformed = self._component_obj.transform(y_df)
         y_t = pd.Series(transformed[:, 0], index=y_ww.index)
 
-        # TODO: Fix this after WW adds inference of object type booleans to BooleanNullable
-        # Iterate through categorical columns that might have been boolean and convert them back to boolean
-        if {True, False}.issubset(set(y_t.unique())) and isinstance(
-            y_ww.ww.logical_type,
-            Categorical,
-        ):
-            y_t = y_t.astype(bool)
-
-        new_logical_type = (
-            Integer
-            if isinstance(y_ww.ww.logical_type, IntegerNullable)
-            else y_ww.ww.logical_type
+        # Determine logical type to use - should match input data where possible
+        new_logical_type_dict = _get_new_logical_types_for_imputed_data(
+            self.parameters["impute_strategy"],
+            y_df.ww.schema,
         )
+        new_logical_type = list(new_logical_type_dict.values())[0]
 
-        y_t = ww.init_series(
-            y_t,
-            logical_type=new_logical_type,
-            semantic_tags=y_ww.ww.semantic_tags,
-        )
-        return X, y_t
+        return X, ww.init_series(y_t, logical_type=new_logical_type)
 
     def fit_transform(self, X, y):
         """Fits on and transforms the input target data.
 
         Args:
             X (pd.DataFrame): Features. Ignored.
             y (pd.Series): Target data to impute.
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """Component that imputes missing data according to a specified timeseries-specific imputation strategy."""
 import pandas as pd
 import woodwork as ww
-from woodwork.logical_types import BooleanNullable, Double
+from woodwork.logical_types import (
+    BooleanNullable,
+    Double,
+)
 
 from evalml.pipelines.components.transformers import Transformer
 from evalml.utils import infer_feature_types
+from evalml.utils.nullable_type_utils import (
+    _determine_fractional_type,
+    _determine_non_nullable_equivalent,
+)
 
 
 class TimeSeriesImputer(Transformer):
     """Imputes missing data according to a specified timeseries-specific imputation strategy.
 
     This Transformer should be used after the `TimeSeriesRegularizer` in order to impute the missing values that were
     added to X and y (if passed).
@@ -48,15 +55,15 @@
     _valid_target_impute_strategies = set(
         ["backwards_fill", "forwards_fill", "interpolate"],
     )
 
     # Incompatibility: https://github.com/alteryx/evalml/issues/4001
     # TODO: Remove when support is added https://github.com/alteryx/evalml/issues/4014
     _integer_nullable_incompatibilities = ["X", "y"]
-    _boolean_nullable_incompatibilities = ["X", "y"]
+    _boolean_nullable_incompatibilities = ["y"]
 
     def __init__(
         self,
         categorical_impute_strategy="forwards_fill",
         numeric_impute_strategy="interpolate",
         target_impute_strategy="forwards_fill",
         random_seed=0,
@@ -104,15 +111,15 @@
             y (pd.Series, optional): The target training data of length [n_samples]
 
         Returns:
             self
         """
         X = infer_feature_types(X)
 
-        nan_ratio = X.ww.describe().loc["nan_count"] / X.shape[0]
+        nan_ratio = X.isna().sum() / X.shape[0]
         self._all_null_cols = nan_ratio[nan_ratio == 1].index.tolist()
 
         def _filter_cols(impute_strat, X):
             """Function to return which columns of the dataset to impute given the impute strategy."""
             cols = []
             if self.parameters["categorical_impute_strategy"] == impute_strat:
                 if self.parameters["numeric_impute_strategy"] == impute_strat:
@@ -151,57 +158,77 @@
             df = pd.DataFrame(index=X.index)
             df.ww.init()
             return df, y
         X = infer_feature_types(X)
         if y is not None:
             y = infer_feature_types(y)
 
+        # This will change the logical type of BooleanNullable/IntegerNullable/AgeNullable columns with nans
+        # so we save the original schema to recreate it where possible after imputation
+        original_schema = X.ww.schema
+        X, y = self._handle_nullable_types(X, y)
+
         X_not_all_null = X.ww.drop(self._all_null_cols)
-        X_schema = X_not_all_null.ww.schema
-        X_schema = X_schema.get_subset_schema(
-            subset_cols=X_schema._filter_cols(
-                exclude=["IntegerNullable", "BooleanNullable", "AgeNullable"],
-            ),
+
+        # Because the TimeSeriesImputer is always used with the TimeSeriesRegularizer,
+        # many of the columns containing nans may have originally been non nullable logical types.
+        # We will use the non nullable equivalents where possible
+        original_schema = original_schema.get_subset_schema(
+            list(X_not_all_null.columns),
         )
+        new_ltypes = {
+            col: _determine_non_nullable_equivalent(ltype)
+            for col, ltype in original_schema.logical_types.items()
+        }
 
         if self._forwards_cols is not None:
-            X_forward = X.ww[self._forwards_cols]
+            X_forward = X[self._forwards_cols]
             imputed = X_forward.pad()
             imputed.bfill(inplace=True)  # Fill in the first value, if missing
             X_not_all_null[X_forward.columns] = imputed
 
         if self._backwards_cols is not None:
-            X_backward = X.ww[self._backwards_cols]
+            X_backward = X[self._backwards_cols]
             imputed = X_backward.bfill()
             imputed.pad(inplace=True)  # Fill in the last value, if missing
             X_not_all_null[X_backward.columns] = imputed
 
         if self._interpolate_cols is not None:
-            X_interpolate = X.ww[self._interpolate_cols]
-            # TODO: Revert when pandas introduces Float64 dtype
-            imputed = X_interpolate.astype(
-                float,
-            ).interpolate()  # Cast to float because Int64 not handled
+            X_interpolate = X_not_all_null[self._interpolate_cols]
+            imputed = X_interpolate.interpolate()
             imputed.bfill(inplace=True)  # Fill in the first value, if missing
             X_not_all_null[X_interpolate.columns] = imputed
-        X_not_all_null.ww.init(schema=X_schema)
+
+            # Interpolate may add floating point values to integer data, so we
+            # have to update those logical types from the ones passed in to a fractional type
+            # Note we ignore all other types of columns to maintain the types specified above
+            int_cols_to_update = original_schema._filter_cols(
+                include=["IntegerNullable", "AgeNullable"],
+            )
+            new_int_ltypes = {
+                col: _determine_fractional_type(ltype)
+                for col, ltype in original_schema.logical_types.items()
+                if col in int_cols_to_update
+            }
+            new_ltypes.update(new_int_ltypes)
+        X_not_all_null.ww.init(schema=original_schema, logical_types=new_ltypes)
 
         y_imputed = pd.Series(y)
         if y is not None and len(y) > 0:
             if self._impute_target == "forwards_fill":
                 y_imputed = y.pad()
                 y_imputed.bfill(inplace=True)
             elif self._impute_target == "backwards_fill":
                 y_imputed = y.bfill()
                 y_imputed.pad(inplace=True)
             elif self._impute_target == "interpolate":
-                # TODO: Revert when pandas introduces Float64 dtype
-                y_imputed = y.astype(float).interpolate()
+                y_imputed = y.interpolate()
                 y_imputed.bfill(inplace=True)
-            y_imputed = ww.init_series(y_imputed)
+            # Re-initialize woodwork with the downcast logical type
+            y_imputed = ww.init_series(y_imputed, logical_type=y.ww.logical_type)
 
         return X_not_all_null, y_imputed
 
     def _handle_nullable_types(self, X=None, y=None):
         """Transforms X and y to remove any incompatible nullable types for the time series imputer when the interpolate method is used.
 
         Args:
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/__init__.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
     name = "Decomposer"
     hyperparameter_ranges = None
     modifies_features = False
     modifies_target = True
     needs_fitting = True
     invalid_frequencies = []
+    # Incompatibility: https://github.com/alteryx/evalml/issues/4103
+    # TODO: Remove when support is added https://github.com/pandas-dev/pandas/issues/52127
+    _integer_nullable_incompatibilities = ["y"]
 
     def __init__(
         self,
         component_obj=None,
         random_seed: int = 0,
         degree: int = 1,
         period: int = -1,
@@ -144,14 +147,15 @@
                 repeats.  If the time series data is in days, then this is the number of days that it takes the target's
                 seasonal signal to repeat. Note: the target data can contain multiple seasonal signals.  This function
                 will only return the stronger.  E.g. if the target has both weekly and yearly seasonality, the function
                 may return either "7" or "365", depending on which seasonality is more strongly autocorrelated.  If no
                 period is detected, returns None.
 
         """
+        X, y = cls._handle_nullable_types(cls, X, y)
 
         def _get_rel_max_from_acf(y):
             """Determines the relative maxima of the target's autocorrelation."""
             acf = sm.tsa.acf(y, nlags=np.maximum(400, len(y)))
             # Filter out small values to avoid picking up noise
             filter_acf = [
                 acf[i] if (acf[i] > acf_threshold) else 0 for i in range(len(acf))
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/lsa.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,24 +69,21 @@
         X_ww = infer_feature_types(X)
         if self._features is None or len(self._features) == 0:
             return X_ww
 
         es = self._make_entity_set(X_ww)
         features = ft.calculate_feature_matrix(features=self._features, entityset=es)
 
-        # Convert to object dtype so that pd.NA is converted to np.nan
-        # until sklearn imputer can handle pd.NA in release 1.1
-        # FT returns these as string types, currently there isn't much difference
-        # in terms of performance between object and string
-        # see https://pandas.pydata.org/docs/user_guide/text.html#text-data-types
-        # "Currently, the performance of object dtype arrays of strings
-        # "and arrays.StringArray are about the same."
+        ltypes = features.ww.logical_types
+        # CatBoost has an issue with categoricals with string categories:
+        # https://github.com/catboost/catboost/issues/1965
+        # Which will pop up if these categorical features are left with string categories,
+        # so convert them to object until the bug is fixed.
         features = features.astype(object, copy=False)
-        features.index = X_ww.index
-        features.ww.init(logical_types={col_: "categorical" for col_ in features})
+        features.ww.init(logical_types=ltypes)
 
         X_ww = X_ww.ww.drop(self._columns)
         X_ww = ww.concat_columns([X_ww, features])
 
         return X_ww
 
     @staticmethod
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/samplers/base_sampler.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/samplers/oversampler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,177 +1,176 @@
-"""Base Sampler component. Used as the base class of all sampler components."""
-import copy
-from abc import abstractmethod
-
-from woodwork.logical_types import IntegerNullable
-
-from evalml.pipelines.components.transformers import Transformer
+"""SMOTE Oversampler component. Will automatically select whether to use SMOTE, SMOTEN, or SMOTENC based on inputs to the component."""
+from evalml.pipelines.components.transformers.samplers.base_sampler import BaseSampler
+from evalml.pipelines.components.utils import make_balancing_dictionary
+from evalml.utils import import_or_raise
 from evalml.utils.woodwork_utils import infer_feature_types
 
 
-class BaseSampler(Transformer):
-    """Base Sampler component. Used as the base class of all sampler components.
+class Oversampler(BaseSampler):
+    """SMOTE Oversampler component. Will automatically select whether to use SMOTE, SMOTEN, or SMOTENC based on inputs to the component.
 
     Args:
-        parameters (dict): Dictionary of parameters for the component. Defaults to None.
-        component_obj (obj): Third-party objects useful in component implementation. Defaults to None.
-        random_seed (int): Seed for the random number generator. Defaults to 0.
+        sampling_ratio (float): This is the goal ratio of the minority to majority class, with range (0, 1]. A value of 0.25 means we want a 1:4 ratio
+            of the minority to majority class after oversampling. We will create the a sampling dictionary using this ratio, with the keys corresponding to the class
+            and the values responding to the number of samples. Defaults to 0.25.
+        sampling_ratio_dict (dict): A dictionary specifying the desired balanced ratio for each target value. For instance, in a binary case where class 1 is the minority, we could specify:
+            `sampling_ratio_dict={0: 0.5, 1: 1}`, which means we would undersample class 0 to have twice the number of samples as class 1 (minority:majority ratio = 0.5), and don't sample class 1.
+            Overrides sampling_ratio if provided. Defaults to None.
+        k_neighbors_default (int): The number of nearest neighbors used to construct synthetic samples. This is the default value used, but the actual k_neighbors value might be smaller
+            if there are less samples. Defaults to 5.
+        n_jobs (int): The number of CPU cores to use. Defaults to -1.
+        random_seed (int): The seed to use for random sampling. Defaults to 0.
     """
 
-    modifies_features = True
-    modifies_target = True
-    training_only = True
+    name = "Oversampler"
+    hyperparameter_ranges = {}
+    _can_be_used_for_fast_partial_dependence = False
+
+    # Incompatibility https://github.com/alteryx/evalml/issues/3974
+    # TODO: Remove when support is added https://github.com/alteryx/evalml/issues/4067
+    _boolean_nullable_incompatibilities = ["X"]
+    _integer_nullable_incompatibilities = ["X"]
+
+    """{}"""
+
+    def __init__(
+        self,
+        sampling_ratio=0.25,
+        sampling_ratio_dict=None,
+        k_neighbors_default=5,
+        n_jobs=-1,
+        random_seed=0,
+        **kwargs,
+    ):
+        error_msg = "imbalanced-learn is not installed. Please install using 'pip install imbalanced-learn'"
+        im = import_or_raise("imblearn.over_sampling", error_msg=error_msg)
+        self.sampler = None
+        self.sampler_options = {
+            "SMOTE": im.SMOTE,
+            "SMOTENC": im.SMOTENC,
+            "SMOTEN": im.SMOTEN,
+        }
+        parameters = {
+            "sampling_ratio": sampling_ratio,
+            "k_neighbors_default": k_neighbors_default,
+            "n_jobs": n_jobs,
+            "sampling_ratio_dict": sampling_ratio_dict,
+        }
+        parameters.update(kwargs)
+        super().__init__(
+            parameters=parameters,
+            component_obj=None,
+            random_seed=random_seed,
+        )
 
     def fit(self, X, y):
-        """Fits the sampler to the data.
+        """Fits oversampler to data.
 
         Args:
-            X (pd.DataFrame): Input features.
-            y (pd.Series): Target.
+            X (pd.DataFrame): The input training data of shape [n_samples, n_features].
+            y (pd.Series, optional): The target training data of length [n_samples].
 
         Returns:
             self
-
-        Raises:
-            ValueError: If y is None.
         """
+        X_ww = infer_feature_types(X)
         if y is None:
             raise ValueError("y cannot be None")
-        X_ww, y_ww = self._prepare_data(X, y)
-        self._initialize_sampler(X_ww, y_ww)
-        return self
-
-    @abstractmethod
-    def _initialize_sampler(self, X, y):
-        """Helper function to initialize the sampler component object.
-
-        Args:
-            X (pd.DataFrame): Features.
-            y (pd.Series): The target data.
-        """
+        y_ww = infer_feature_types(y)
 
-    def _prepare_data(self, X, y):
-        """Transforms the input data to pandas data structure that our sampler can ingest.
+        sampler_name = self._get_best_oversampler(X_ww)
+        self.sampler = self.sampler_options[sampler_name]
 
-        Args:
-            X (pd.DataFrame): Training features.
-            y (pd.Series): Target.
-
-        Returns:
-            pd.DataFrame, pd.Series: Prepared X and y data as pandas types
-        """
-        X = infer_feature_types(X)
-        int_nullable_cols = X.ww.select(IntegerNullable).columns
-        if len(int_nullable_cols) > 0:
-            try:
-                X = X.astype(
-                    {
-                        null_col: int
-                        for null_col in X.ww.select(IntegerNullable).columns
-                    },
-                )
-            except ValueError:
-                X = X.astype(
-                    {
-                        null_col: float
-                        for null_col in X.ww.select(IntegerNullable).columns
-                    },
-                )
-            X.ww.init(schema=X.ww.schema)
-
-        if y is None:
-            raise ValueError("y cannot be None")
-        y = infer_feature_types(y)
-        return X, y
+        # get categorical features first, if necessary
+        if sampler_name == "SMOTENC":
+            self._get_categorical(X_ww)
+        super().fit(X_ww, y_ww)
+        return self
 
     def transform(self, X, y=None):
-        """Transforms the input data by sampling the data.
+        """Transforms the input data by Oversampling the data.
 
         Args:
             X (pd.DataFrame): Training features.
             y (pd.Series): Target.
 
         Returns:
             pd.DataFrame, pd.Series: Transformed features and target.
         """
-        X, y = self._prepare_data(X, y)
-
-        categorical_columns = X.ww.select("Categorical", return_schema=True).columns
-        for col in categorical_columns:
-            X[col] = X[col].astype("object")
-
-        X_new, y_new = self._component_obj.fit_resample(X, y)
-
-        for col in categorical_columns:
-            X[col] = X[col].astype("category")
+        X_ww = infer_feature_types(X)
+        original_schema = X_ww.ww.schema
+        if y is None:
+            raise ValueError("y cannot be None")
+        y_ww = infer_feature_types(y)
+        X_d, _ = self._handle_nullable_types(X_ww)
+        X_t, y_t = super().transform(X_d, y_ww)
+
+        # X_t will have the downcasted types, so convert back to the original schema
+        X_t.ww.init(schema=original_schema)
+
+        return X_t, y_t
+
+    def _get_best_oversampler(self, X):
+        cat_cols = X.ww.select(
+            ["category", "boolean", "BooleanNullable"],
+            return_schema=True,
+        ).columns
+        if len(cat_cols) == X.shape[1]:
+            return "SMOTEN"
+        elif not len(cat_cols):
+            return "SMOTE"
+        else:
+            return "SMOTENC"
 
-        X_new.ww.init(schema=X.ww.schema)
-        y_new.ww.init(schema=y.ww.schema)
-        return X_new, y_new
+    def _get_categorical(self, X):
+        X = infer_feature_types(X)
+        # Grab categorical columns
+        self.categorical_features = [
+            i
+            for i, val in enumerate(X.ww.semantic_tags.items())
+            if "category" in val[1]
+        ]
+        # Grab boolean columns, since SMOTE considers these categorical as well
+        for i, val in enumerate(X.ww.types["Logical Type"].items()):
+            if str(val[1]) in {"Boolean", "BooleanNullable"}:
+                self.categorical_features.append(i)
+        self._parameters["categorical_features"] = self.categorical_features
 
-    def _convert_dictionary(self, sampling_dict, y):
-        """Converts the provided sampling dictionary from a dictionary of ratios to a dictionary of number of samples.
+    def _initialize_sampler(self, X, y):
+        """Initializes the oversampler with the given sampler_ratio or sampler_ratio_dict.
 
-        Expects the provided dictionary keys to be the target values y, and the associated values to be the min:max ratios.
-        Converts and returns a dictionary with the same keys, but changes the values to be the number of samples rather than ratio.
+        If a sampler_ratio_dict is provided, we will opt to use that. Otherwise, we use will create the sampler_ratio_dict dictionary.
 
         Args:
-            sampling_dict (dict): The input sampling dictionary passed in from user.
-            y (pd.Series): The target values.
-
-        Returns:
-            dict: A dictionary with target values as keys and the number of samples as values.
+            X (pd.DataFrame): Input features.
+            y (pd.Series): Target.
         """
-        # check that the lengths of the dict and y are equal
-        y_unique = y.unique()
-        if len(sampling_dict) != len(y_unique):
+        sampler_class = self.sampler
+        y_pd = infer_feature_types(y)
+        sampler_params = {
+            k: v
+            for k, v in self.parameters.items()
+            if k not in ["sampling_ratio", "sampling_ratio_dict", "k_neighbors_default"]
+        }
+        if self.parameters["sampling_ratio_dict"] is not None:
+            # make the dictionary
+            dic = self._convert_dictionary(self.parameters["sampling_ratio_dict"], y_pd)
+        else:
+            # create the sampling dictionary
+            sampling_ratio = self.parameters["sampling_ratio"]
+            dic = make_balancing_dictionary(y_pd, sampling_ratio)
+        sampler_params["sampling_strategy"] = dic
+
+        # check for k_neighbors value
+        neighbors = self.parameters["k_neighbors_default"]
+        min_counts = y_pd.value_counts().values[-1]
+        if min_counts == 1:
             raise ValueError(
-                "Sampling dictionary contains a different number of targets than are provided in the data.",
+                f"Minority class needs more than 1 sample to use SMOTE!, received {min_counts} sample",
             )
+        if min_counts <= neighbors:
+            neighbors = min_counts - 1
 
-        if len(set(sampling_dict.keys()).intersection(set(y_unique))) != len(y_unique):
-            raise ValueError("Dictionary keys are different from target values!")
-
-        new_dic = {}
-        y_counts = y.value_counts()
-        for k, v in sampling_dict.items():
-            # turn the ratios into sampler values
-            if self.__class__.__name__ == "Undersampler":
-                # for undersampling, we make sure we never sample more than the
-                # total samples for that class
-                new_dic[k] = int(min(y_counts.values[-1] / v, y_counts[k]))
-            else:
-                # for oversampling, we need to make sure we never sample less than
-                # the total samples for that class
-                new_dic[k] = int(max(y_counts.values[0] * v, y_counts[k]))
-        return new_dic
-
-    def _dictionary_to_params(self, sampling_dict, y):
-        """If a sampling ratio dictionary is provided, add the updated sampling dictionary to the parameters and return the updated parameter dictionary. Otherwise, simply return the current parameters.
-
-        Args:
-            sampling_dict (dict): The input sampling dictionary passed in from user.
-            y (pd.Series): The target values.
-
-        Returns:
-            dict: The parameters dictionary with the sampling_ratio_dict value replaced as necessary.
-        """
-        param_copy = copy.copy(self.parameters)
-        if self.parameters["sampling_ratio_dict"]:
-            new_dic = self._convert_dictionary(
-                self.parameters["sampling_ratio_dict"],
-                y,
-            )
-            param_copy["sampling_ratio_dict"] = new_dic
-        return param_copy
-
-    def fit_transform(self, X, y):
-        """Fit and transform data using the sampler component.
-
-        Args:
-            X (pd.DataFrame): The input training data of shape [n_samples, n_features].
-            y (pd.Series, optional): The target training data of length [n_samples].
-
-        Returns:
-            (pd.DataFrame, pd.Series): Transformed data.
-        """
-        return self.fit(X, y).transform(X, y)
+        sampler_params["k_neighbors"] = neighbors
+        self._parameters["k_neighbors"] = neighbors
+        sampler = sampler_class(**sampler_params, random_state=self.random_seed)
+        self._component_obj = sampler
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/samplers/oversampler.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/samplers/undersampler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,146 +1,191 @@
-"""SMOTE Oversampler component. Will automatically select whether to use SMOTE, SMOTEN, or SMOTENC based on inputs to the component."""
+"""An undersampling transformer to downsample the majority classes in the dataset."""
+import numpy as np
+import pandas as pd
+
 from evalml.pipelines.components.transformers.samplers.base_sampler import BaseSampler
-from evalml.pipelines.components.utils import make_balancing_dictionary
-from evalml.utils import import_or_raise
 from evalml.utils.woodwork_utils import infer_feature_types
 
 
-class Oversampler(BaseSampler):
-    """SMOTE Oversampler component. Will automatically select whether to use SMOTE, SMOTEN, or SMOTENC based on inputs to the component.
+class Undersampler(BaseSampler):
+    """Initializes an undersampling transformer to downsample the majority classes in the dataset.
+
+    This component is only run during training and not during predict.
 
     Args:
-        sampling_ratio (float): This is the goal ratio of the minority to majority class, with range (0, 1]. A value of 0.25 means we want a 1:4 ratio
-            of the minority to majority class after oversampling. We will create the a sampling dictionary using this ratio, with the keys corresponding to the class
-            and the values responding to the number of samples. Defaults to 0.25.
+        sampling_ratio (float): The smallest minority:majority ratio that is accepted as 'balanced'. For instance, a 1:4 ratio would be
+            represented as 0.25, while a 1:1 ratio is 1.0. Must be between 0 and 1, inclusive. Defaults to 0.25.
         sampling_ratio_dict (dict): A dictionary specifying the desired balanced ratio for each target value. For instance, in a binary case where class 1 is the minority, we could specify:
             `sampling_ratio_dict={0: 0.5, 1: 1}`, which means we would undersample class 0 to have twice the number of samples as class 1 (minority:majority ratio = 0.5), and don't sample class 1.
             Overrides sampling_ratio if provided. Defaults to None.
-        k_neighbors_default (int): The number of nearest neighbors used to construct synthetic samples. This is the default value used, but the actual k_neighbors value might be smaller
-            if there are less samples. Defaults to 5.
-        n_jobs (int): The number of CPU cores to use. Defaults to -1.
+        min_samples (int): The minimum number of samples that we must have for any class, pre or post sampling. If a class must be downsampled, it will not be downsampled past this value.
+            To determine severe imbalance, the minority class must occur less often than this and must have a class ratio below min_percentage.
+            Must be greater than 0. Defaults to 100.
+        min_percentage (float): The minimum percentage of the minimum class to total dataset that we tolerate, as long as it is above min_samples.
+            If min_percentage and min_samples are not met, treat this as severely imbalanced, and we will not resample the data.
+            Must be between 0 and 0.5, inclusive. Defaults to 0.1.
         random_seed (int): The seed to use for random sampling. Defaults to 0.
+
+    Raises:
+        ValueError: If sampling_ratio is not in the range (0, 1].
+        ValueError: If min_sample is not greater than 0.
+        ValueError: If min_percentage is not between 0 and 0.5, inclusive.
     """
 
-    name = "Oversampler"
+    name = "Undersampler"
     hyperparameter_ranges = {}
-    _can_be_used_for_fast_partial_dependence = False
-
-    # Incompatibility https://github.com/alteryx/evalml/issues/3974
-    # TODO: Remove when support is added https://github.com/alteryx/evalml/issues/4067
-    _boolean_nullable_incompatibilities = ["X"]
-    _integer_nullable_incompatibilities = ["X"]
-
     """{}"""
 
     def __init__(
         self,
         sampling_ratio=0.25,
         sampling_ratio_dict=None,
-        k_neighbors_default=5,
-        n_jobs=-1,
+        min_samples=100,
+        min_percentage=0.1,
         random_seed=0,
         **kwargs,
     ):
-        error_msg = "imbalanced-learn is not installed. Please install using 'pip install imbalanced-learn'"
-        im = import_or_raise("imblearn.over_sampling", error_msg=error_msg)
-        self.sampler = None
-        self.sampler_options = {
-            "SMOTE": im.SMOTE,
-            "SMOTENC": im.SMOTENC,
-            "SMOTEN": im.SMOTEN,
-        }
+        if sampling_ratio <= 0 or sampling_ratio > 1:
+            raise ValueError(
+                f"sampling_ratio must be within (0, 1], but received {sampling_ratio}",
+            )
+        if min_samples <= 0:
+            raise ValueError(
+                f"min_sample must be greater than 0, but received {min_samples}",
+            )
+        if min_percentage <= 0 or min_percentage > 0.5:
+            raise ValueError(
+                f"min_percentage must be between 0 and 0.5, inclusive, but received {min_percentage}",
+            )
+
         parameters = {
             "sampling_ratio": sampling_ratio,
-            "k_neighbors_default": k_neighbors_default,
-            "n_jobs": n_jobs,
+            "min_samples": min_samples,
+            "min_percentage": min_percentage,
             "sampling_ratio_dict": sampling_ratio_dict,
         }
+        self.sampling_ratio = sampling_ratio
+        self.min_samples = min_samples
+        self.min_percentage = min_percentage
+        self.random_seed = random_seed
+        self.sampling_ratio_dict = sampling_ratio_dict or {}
+
         parameters.update(kwargs)
         super().__init__(
             parameters=parameters,
             component_obj=None,
             random_seed=random_seed,
         )
 
-    def fit(self, X, y):
-        """Fits oversampler to data.
+    def _initialize_sampler(self, X, y):
+        """Helper function to initialize the undersampler component object.
+
+        Args:
+            X (pd.DataFrame): Ignored.
+            y (pd.Series): The target data.
+        """
+        pass
+
+    def transform(self, X, y=None):
+        """Transforms the input data by sampling the data.
 
         Args:
-            X (pd.DataFrame): The input training data of shape [n_samples, n_features].
-            y (pd.Series, optional): The target training data of length [n_samples].
+            X (pd.DataFrame): Training features.
+            y (pd.Series): Target.
 
         Returns:
-            self
+            pd.DataFrame, pd.Series: Transformed features and target.
         """
-        X_ww, y_ww = self._prepare_data(X, y)
-        sampler_name = self._get_best_oversampler(X_ww)
-        self.sampler = self.sampler_options[sampler_name]
-
-        # get categorical features first, if necessary
-        if sampler_name == "SMOTENC":
-            self._get_categorical(X)
-        super().fit(X, y)
-        return self
-
-    def _get_best_oversampler(self, X):
-        cat_cols = X.ww.select(["category", "boolean"]).columns
-        if len(cat_cols) == X.shape[1]:
-            return "SMOTEN"
-        elif not len(cat_cols):
-            return "SMOTE"
-        else:
-            return "SMOTENC"
+        X_ww = infer_feature_types(X)
+        if y is None:
+            raise ValueError("y cannot be None")
+        y_ww = infer_feature_types(y)
+
+        index_df = pd.Series(y_ww.index)
+        indices = self.fit_resample(X_ww, y_ww)
 
-    def _get_categorical(self, X):
-        X = infer_feature_types(X)
-        # Grab categorical columns
-        self.categorical_features = [
-            i
-            for i, val in enumerate(X.ww.semantic_tags.items())
-            if "category" in val[1]
-        ]
-        # Grab boolean columns, since SMOTE considers these categorical as well
-        for i, val in enumerate(X.ww.types["Logical Type"].items()):
-            if str(val[1]) == "Boolean":
-                self.categorical_features.append(i)
-        self._parameters["categorical_features"] = self.categorical_features
+        train_indices = index_df[index_df.isin(indices)].index.values.tolist()
+        return X_ww.ww.iloc[train_indices], y_ww.ww.iloc[train_indices]
 
-    def _initialize_sampler(self, X, y):
-        """Initializes the oversampler with the given sampler_ratio or sampler_ratio_dict.
+    def _find_ideal_samples(self, y):
+        """Returns dictionary of examples to drop for each class if we need to resample.
 
-        If a sampler_ratio_dict is provided, we will opt to use that. Otherwise, we use will create the sampler_ratio_dict dictionary.
+        Arguments:
+            y (pd.Series): Target data passed in.
 
-        Args:
-            X (pd.DataFrame): Input features.
-            y (pd.Series): Target.
+        Returns:
+            dict: Dictionary with undersample target class as key, and number of samples to remove as the value.
+                If we don't need to resample, returns empty dictionary.
         """
-        sampler_class = self.sampler
-        _, y_pd = self._prepare_data(X, y)
-        sampler_params = {
-            k: v
-            for k, v in self.parameters.items()
-            if k not in ["sampling_ratio", "sampling_ratio_dict", "k_neighbors_default"]
-        }
-        if self.parameters["sampling_ratio_dict"] is not None:
-            # make the dictionary
-            dic = self._convert_dictionary(self.parameters["sampling_ratio_dict"], y_pd)
-        else:
-            # create the sampling dictionary
-            sampling_ratio = self.parameters["sampling_ratio"]
-            dic = make_balancing_dictionary(y_pd, sampling_ratio)
-        sampler_params["sampling_strategy"] = dic
-
-        # check for k_neighbors value
-        neighbors = self.parameters["k_neighbors_default"]
-        min_counts = y_pd.value_counts().values[-1]
-        if min_counts == 1:
-            raise ValueError(
-                f"Minority class needs more than 1 sample to use SMOTE!, received {min_counts} sample",
+        counts = y.value_counts()
+        normalized_counts = y.value_counts(normalize=True)
+        minority_class_count = min(normalized_counts)
+        class_ratios = minority_class_count / normalized_counts
+        # if no class ratios are larger than what we consider balanced, then the target is balanced
+        if all(class_ratios >= self.sampling_ratio):
+            return {}
+        # if any classes have less than min_samples counts and are less than min_percentage of the total data,
+        # then it's severely imbalanced
+        if any(counts < self.min_samples) and any(
+            normalized_counts < self.min_percentage,
+        ):
+            return {}
+        # otherwise, we are imbalanced enough to perform on this
+        undersample_classes = counts[class_ratios <= self.sampling_ratio].index.values
+        # find goal size, round it down if it's a float
+        minority_class = min(counts.values)
+        goal_value = max(
+            int((minority_class / self.sampling_ratio) // 1),
+            self.min_samples,
+        )
+        # we don't want to drop less than 0 rows
+        drop_values = {k: max(0, counts[k] - goal_value) for k in undersample_classes}
+        return {k: v for k, v in drop_values.items() if v > 0}
+
+    def _sampling_dict_to_remove_dict(self, y):
+        """Turns the sampling dict input into a dict of samples to remove for each target, similar to the return of _find_ideal_samples.
+
+        Arguments:
+            y (pd.Series): Training data targets.
+
+        Returns:
+            (dict): dictionary with undersample target class as key, and number of samples to remove as the value.
+                If we don't need to resample, returns empty dictionary.
+        """
+        y_dict = y.value_counts().to_dict()
+        new_dic = {}
+        for k, v in self.sampling_ratio_dict.items():
+            new_dic[k] = max(y_dict[k] - v, 0)
+        return new_dic
+
+    def fit_resample(self, X, y):
+        """Resampling technique for this sampler.
+
+        Arguments:
+            X (pd.DataFrame): Training data to fit and resample.
+            y (pd.Series): Training data targets to fit and resample.
+
+        Returns:
+            list: Indices to keep for training data.
+        """
+        if self.parameters["sampling_ratio_dict"]:
+            self.sampling_ratio_dict = self._convert_dictionary(
+                self.parameters["sampling_ratio_dict"],
+                y,
             )
-        if min_counts <= neighbors:
-            neighbors = min_counts - 1
 
-        sampler_params["k_neighbors"] = neighbors
-        self._parameters["k_neighbors"] = neighbors
-        sampler = sampler_class(**sampler_params, random_state=self.random_seed)
-        self._component_obj = sampler
+        y = infer_feature_types(y)
+        random_state = np.random.RandomState(self.random_seed)
+        if len(self.sampling_ratio_dict):
+            result = self._sampling_dict_to_remove_dict(y)
+        else:
+            result = self._find_ideal_samples(y)
+        indices_to_drop = []
+        if len(result):
+            # iterate through the classes we need to undersample and remove the number of samples we need to remove
+            for key, value in result.items():
+                indices = y.index[y == key].values
+                indices_to_remove = random_state.choice(indices, value, replace=False)
+                indices_to_drop.extend(indices_to_remove)
+        # indices of the y series
+        original_indices = list(set(y.index.values).difference(set(indices_to_drop)))
+        return original_indices
```

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/transformers/transformer.py` & `evalml-0.73.0/evalml/pipelines/components/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/components/utils.py` & `evalml-0.73.0/evalml/pipelines/components/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,62 +163,14 @@
         raise MissingComponentError(
             'Component "{}" was not found'.format(component_class),
         )
     component_class = component_classes[component_class]
     return component_class
 
 
-def drop_natural_language_columns(X):
-    """Drops natural language columns from dataframes for the imputers.
-
-    Args:
-        X (pd.Dataframe): The dataframe that we want to impute on.
-
-    Returns:
-        pd.Dataframe: the dataframe with any natural language columns dropped.
-        list: list of all the columns that are considered natural language.
-    """
-    natural_language_columns = list(
-        X.ww.select(["NaturalLanguage"], return_schema=True).columns.keys(),
-    )
-    if natural_language_columns:
-        X = X.ww.copy()
-        X = X.ww.drop(columns=natural_language_columns)
-    return X, natural_language_columns
-
-
-def set_boolean_columns_to_integer(X):
-    """Sets boolean columns to integer nullable for the imputer.
-
-    Args:
-        X (pd.Dataframe): The dataframe that we want to impute on.
-
-    Returns:
-        pd.Dataframe: the dataframe with any of its ww columns that are boolean set to integer nullable.
-    """
-    X = X.ww.copy()
-    original_X_schema = X.ww.schema.get_subset_schema(
-        subset_cols=list(
-            X.ww.select(
-                exclude=["Boolean", "BooleanNullable"],
-                return_schema=True,
-            ).columns,
-        ),
-    )
-    X_boolean_cols = list(
-        X.ww.select(
-            include=["Boolean", "BooleanNullable"],
-            return_schema=True,
-        ).columns,
-    )
-    new_ltypes_for_boolean_cols = {col: "IntegerNullable" for col in X_boolean_cols}
-    X.ww.init(schema=original_X_schema, logical_types=new_ltypes_for_boolean_cols)
-    return X
-
-
 def get_prediction_intevals_for_tree_regressors(
     X: pd.DataFrame,
     predictions: pd.Series,
     coverage: List[float],
     estimators: List[Estimator],
 ) -> Dict[str, pd.Series]:
     """Find the prediction intervals for tree-based regressors.
```

### Comparing `evalml-0.72.0/evalml/pipelines/multiclass_classification_pipeline.py` & `evalml-0.73.0/evalml/pipelines/multiclass_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/pipeline_base.py` & `evalml-0.73.0/evalml/pipelines/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/pipeline_meta.py` & `evalml-0.73.0/evalml/pipelines/pipeline_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/regression_pipeline.py` & `evalml-0.73.0/evalml/pipelines/regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/time_series_classification_pipelines.py` & `evalml-0.73.0/evalml/pipelines/time_series_classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/pipelines/time_series_pipeline_base.py` & `evalml-0.73.0/evalml/pipelines/time_series_pipeline_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,78 +163,109 @@
             y.ww.init(schema=y_schema)
 
             if X.ww.schema is not None:
                 X = X.ww.copy()
                 X.ww.set_time_index(None)
                 X.ww.set_index(self.time_index)
                 X = X.ww.drop(self.time_index)
+                X.index.freq = time_index.freq
             else:
                 X.set_index(time_index)
                 X = X.drop(self.time_index, axis=1)
             X.index.name = index_name
             y.index.name = index_name
         return X, y
 
-    def transform_all_but_final(self, X, y=None, X_train=None, y_train=None):
+    def transform_all_but_final(
+        self,
+        X,
+        y=None,
+        X_train=None,
+        y_train=None,
+        calculating_residuals=False,
+    ):
         """Transforms the data by applying all pre-processing components.
 
         Args:
             X (pd.DataFrame): Input data to the pipeline to transform.
             y (pd.Series): Targets corresponding to the pipeline targets.
             X_train (pd.DataFrame): Training data used to generate generates from past observations.
             y_train (pd.Series): Training targets used to generate features from past observations.
+            calculating_residuals (bool): Whether we're calling predict_in_sample to calculate the residuals.  This means
+                the X and y arguments are not future data, but actually the train data.
 
         Returns:
             pd.DataFrame: New transformed features.
         """
         if y_train is None:
             y_train = pd.Series()
         X_train, y_train = self._convert_to_woodwork(X_train, y_train)
         X, y = self._convert_to_woodwork(X, y)
 
         empty_training_data = X_train.empty or y_train.empty
-        if empty_training_data or self.should_skip_featurization:
+        if (
+            empty_training_data
+            or self.should_skip_featurization
+            or calculating_residuals
+        ):
             features_holdout = super().transform_all_but_final(X, y)
         else:
             padded_features, padded_target = self._add_training_data_to_X_Y(
                 X,
                 y,
                 X_train,
                 y_train,
             )
             features = super().transform_all_but_final(padded_features, padded_target)
             features_holdout = features.ww.iloc[-len(y) :]
         return features_holdout
 
-    def predict_in_sample(self, X, y, X_train, y_train, objective=None):
+    def predict_in_sample(
+        self,
+        X,
+        y,
+        X_train,
+        y_train,
+        objective=None,
+        calculating_residuals=False,
+    ):
         """Predict on future data where the target is known, e.g. cross validation.
 
         Args:
             X (pd.DataFrame or np.ndarray): Future data of shape [n_samples, n_features]
             y (pd.Series, np.ndarray): Future target of shape [n_samples]
             X_train (pd.DataFrame, np.ndarray): Data the pipeline was trained on of shape [n_samples_train, n_feautures]
             y_train (pd.Series, np.ndarray): Targets used to train the pipeline of shape [n_samples_train]
             objective (ObjectiveBase, str, None): Objective used to threshold predicted probabilities, optional.
+            calculating_residuals (bool): Whether we're calling predict_in_sample to calculate the residuals.  This means
+                the X and y arguments are not future data, but actually the train data.
 
         Returns:
             pd.Series: Estimated labels.
 
         Raises:
             ValueError: If final component is not an Estimator.
         """
         if self.estimator is None:
             raise ValueError(
                 "Cannot call predict_in_sample() on a component graph because the final component is not an Estimator.",
             )
         X, y = self._drop_time_index(X, y)
         X_train, y_train = self._drop_time_index(X_train, y_train)
         target = infer_feature_types(y)
-        features = self.transform_all_but_final(X, target, X_train, y_train)
+        features = self.transform_all_but_final(
+            X,
+            target,
+            X_train,
+            y_train,
+            calculating_residuals=calculating_residuals,
+        )
         predictions = self._estimator_predict(features)
-        predictions.index = y.index
+        if len(predictions) == len(y):
+            predictions.index = y.index
         predictions = self.inverse_transform(predictions)
         predictions = predictions.rename(self.input_target_name)
         return infer_feature_types(predictions)
 
     def _create_empty_series(self, y_train, size):
         return ww.init_series(
             pd.Series([y_train.iloc[0]] * size),
```

### Comparing `evalml-0.72.0/evalml/pipelines/time_series_regression_pipeline.py` & `evalml-0.73.0/evalml/pipelines/time_series_regression_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pipeline base class for time series regression problems."""
+import numpy as np
 import pandas as pd
 from woodwork.statistics_utils import infer_frequency
 
 from evalml.model_family import ModelFamily
 from evalml.pipelines.components import STLDecomposer
 from evalml.pipelines.time_series_pipeline_base import TimeSeriesPipelineBase
 from evalml.problem_types import ProblemTypes
@@ -199,18 +200,18 @@
 
         Returns:
             dict: Prediction intervals, keys are in the format {coverage}_lower or {coverage}_upper.
 
         Raises:
             MethodPropertyNotFoundError: If the estimator does not support Time Series Regression as a problem type.
         """
-        X, y = self._drop_time_index(X, y)
+        X_no_datetime, y_no_datetime = self._drop_time_index(X, y)
         estimator_input = self.transform_all_but_final(
-            X,
-            y,
+            X_no_datetime,
+            y_no_datetime,
             X_train=X_train,
             y_train=y_train,
         )
         has_stl = STLDecomposer.name in list(
             self.component_graph.component_instances.keys(),
         )
         if coverage is None:
@@ -234,19 +235,45 @@
                     (orig_pi_values.values - residuals.values)
                     + trend_pred_intervals[key].values
                     + y.values,
                     index=orig_pi_values.index,
                 )
             return trans_pred_intervals
         else:
-            predictions = self.predict_in_sample(
+            future_vals = self.predict(
                 X=X,
-                y=y,
                 X_train=X_train,
                 y_train=y_train,
             )
-            return self.estimator.get_prediction_intervals(
-                X=estimator_input,
-                y=y,
-                coverage=coverage,
-                predictions=predictions,
+
+            predictions_train = self.predict_in_sample(
+                X=X_train,
+                y=y_train,
+                X_train=X_train,
+                y_train=y_train,
+                calculating_residuals=True,
             )
+            residuals = y_train - predictions_train
+            std_residual = np.sqrt(np.sum(residuals**2) / len(residuals))
+
+            res_dict = {}
+            cov_to_mult = {0.75: 1.15, 0.85: 1.44, 0.95: 1.96}
+            for cov in coverage:
+                lower = []
+                upper = []
+                multiplier = cov_to_mult[cov]
+                for counter, val in enumerate(future_vals):
+                    factor = multiplier * std_residual * np.sqrt(counter + 1)
+                    lower.append(val - factor)
+                    upper.append(val + factor)
+
+                res_dict[f"{cov}_lower"] = pd.Series(
+                    lower,
+                    name=f"{cov}_lower",
+                    index=future_vals.index,
+                )
+                res_dict[f"{cov}_upper"] = pd.Series(
+                    upper,
+                    name=f"{cov}_upper",
+                    index=future_vals.index,
+                )
+            return res_dict
```

### Comparing `evalml-0.72.0/evalml/pipelines/utils.py` & `evalml-0.73.0/evalml/pipelines/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,36 +85,14 @@
     non_index_unknown = X.ww.select(exclude=["index", "unknown"])
     all_null_cols = non_index_unknown.columns[non_index_unknown.isnull().all()]
     if len(all_null_cols) > 0:
         component.append(DropNullColumns)
     return component
 
 
-def _get_replace_null(X, y, problem_type, estimator_class, sampler_name=None):
-    component = []
-    input_logical_types = {type(lt) for lt in X.ww.logical_types.values()}
-    types_replace_null_handles = [
-        logical_types.AgeNullable,
-        logical_types.Boolean,
-        logical_types.BooleanNullable,
-        logical_types.Double,
-        logical_types.Integer,
-        logical_types.IntegerNullable,
-    ]
-
-    nullable_target = isinstance(y.ww.logical_type, tuple(types_replace_null_handles))
-
-    if (
-        len(input_logical_types.intersection(set(types_replace_null_handles)))
-        or nullable_target
-    ):
-        component.append(ReplaceNullableTypes)
-    return component
-
-
 def _get_drop_index_unknown(X, y, problem_type, estimator_class, sampler_name=None):
     component = []
     index_and_unknown_columns = list(
         X.ww.select(["index", "unknown"], return_schema=True).columns,
     )
     if len(index_and_unknown_columns) > 0:
         component.append(DropColumns)
@@ -190,15 +168,15 @@
 
 def _get_ohe(X, y, problem_type, estimator_class, sampler_name=None):
     components = []
 
     # The URL and EmailAddress Featurizers will create categorical columns
     categorical_cols = list(
         X.ww.select(
-            ["category", "URL", "EmailAddress", "BooleanNullable"],
+            ["category", "URL", "EmailAddress"],
             return_schema=True,
         ).columns,
     )
     if len(categorical_cols) > 0 and estimator_class not in {
         CatBoostClassifier,
         CatBoostRegressor,
     }:
@@ -308,15 +286,14 @@
     Returns:
         list[Transformer]: A list of applicable preprocessing components to use with the estimator.
     """
     if is_time_series(problem_type):
         components_functions = [
             _get_label_encoder,
             _get_drop_all_null,
-            _get_replace_null,
             _get_drop_index_unknown,
             _get_url,
             _get_email,
             _get_natural_language,
             _get_imputer,
             _get_time_series_featurizer,
         ]
@@ -330,15 +307,14 @@
             _get_sampler,
             _get_standard_scaler,
         ]
     else:
         components_functions = [
             _get_label_encoder,
             _get_drop_all_null,
-            _get_replace_null,
             _get_drop_index_unknown,
             _get_url,
             _get_email,
             _get_datetime,
             _get_natural_language,
             _get_imputer,
             _get_ordinal_encoder,
```

### Comparing `evalml-0.72.0/evalml/preprocessing/data_splitters/no_split.py` & `evalml-0.73.0/evalml/preprocessing/data_splitters/no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/preprocessing/data_splitters/sk_splitters.py` & `evalml-0.73.0/evalml/preprocessing/data_splitters/sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/preprocessing/data_splitters/time_series_split.py` & `evalml-0.73.0/evalml/preprocessing/data_splitters/time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/preprocessing/data_splitters/training_validation_split.py` & `evalml-0.73.0/evalml/preprocessing/data_splitters/training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/preprocessing/utils.py` & `evalml-0.73.0/evalml/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/problem_types/problem_types.py` & `evalml-0.73.0/evalml/problem_types/problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/problem_types/utils.py` & `evalml-0.73.0/evalml/problem_types/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/dask_test_utils.py` & `evalml-0.73.0/evalml/tests/automl_tests/dask_test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py` & `evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py` & `evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py` & `evalml-0.73.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl_algorithm.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_classification.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_regression.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_automl_utils.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_automl_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_default_algorithm.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_default_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,21 +391,14 @@
     pipeline = algo._make_split_pipeline(RandomForestClassifier, "test_pipeline")
 
     order = pipeline.component_graph.compute_order
     assert order[0] == "Label Encoder" if not features else "DFS Transformer"
     if sampler:
         assert order[-2] == sampler
     assert order[-1] == "Random Forest Classifier"
-    for dtype in ["Categorical", "Numeric"]:
-        assert order.index(f"{dtype} Pipeline - Label Encoder") < order.index(
-            f"{dtype} Pipeline - Replace Nullable Types Transformer",
-        )
-        assert order.index(
-            f"{dtype} Pipeline - Replace Nullable Types Transformer",
-        ) < order.index(f"{dtype} Pipeline - Imputer")
 
     assert pipeline.name == "test_pipeline"
     assert pipeline.parameters["Numeric Pipeline - Select Columns By Type Transformer"][
         "column_types"
     ] == ["category", "EmailAddress", "URL"]
     assert pipeline.parameters["Numeric Pipeline - Select Columns By Type Transformer"][
         "exclude"
@@ -429,15 +422,14 @@
 
     algo = DefaultAlgorithm(X, y, ProblemTypes.BINARY, sampler_name=None)
     algo._selected_cat_cols = ["A", "B", "C"]
     pipeline = algo._make_split_pipeline(RandomForestClassifier)
     compute_order = [
         "Select Columns Transformer",
         "Label Encoder",
-        "Replace Nullable Types Transformer",
         "Imputer",
         "One Hot Encoder",
         "Random Forest Classifier",
     ]
     assert pipeline.component_graph.compute_order == compute_order
     assert pipeline.parameters["Select Columns Transformer"]["columns"] == [
         "A",
```

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_engine_base.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_iterative_algorithm.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_pipeline_search_plots.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_progress.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_search.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_search_iterative.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_search_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/automl_tests/test_time_series_split.py` & `evalml-0.73.0/evalml/tests/automl_tests/test_time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py` & `evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import itertools
 from datetime import datetime, timedelta
 
 import matplotlib
 import numpy as np
 import pandas as pd
 import pytest
+import woodwork as ww
 
 import evalml.exceptions
 from evalml.pipelines.components.transformers.preprocessing import (
     PolynomialDecomposer,
     STLDecomposer,
 )
 
@@ -435,37 +436,43 @@
     dec.set_period(X, y)
 
     assert 0.95 * period <= dec.period <= 1.05 * period
     assert dec.parameters["period"] == dec.period
 
 
 @pytest.mark.parametrize(
+    "y_logical_type",
+    ["Double", "Integer", "Age", "IntegerNullable", "AgeNullable"],
+)
+@pytest.mark.parametrize(
     "decomposer_child_class",
     decomposer_list,
 )
 @pytest.mark.parametrize("decomposer_picked_correct_degree", [True, False])
 @pytest.mark.parametrize(
     "synthetic_data,trend_degree,period",
     [
         *itertools.product(["synthetic"], [1, 2, 3], [None, 7, 30, 365]),
         ("real", 1, 365),
     ],
 )
 def test_decomposer_determine_periodicity(
+    y_logical_type,
     decomposer_child_class,
     period,
     trend_degree,
     decomposer_picked_correct_degree,
     synthetic_data,
     generate_seasonal_data,
 ):
     X, y = generate_seasonal_data(real_or_synthetic=synthetic_data)(
         period,
         trend_degree=trend_degree,
     )
+    y = ww.init_series(y.astype(int), logical_type=y_logical_type)
 
     # Test that the seasonality can be determined if trend guess isn't spot on.
     if not decomposer_picked_correct_degree:
         trend_degree = 1 if trend_degree in [2, 3] else 2
 
     dec = decomposer_child_class(degree=trend_degree, period=period)
     ac = dec.determine_periodicity(X, y)
@@ -476,14 +483,69 @@
         assert 0.95 * period <= ac <= 1.05 * period
 
 
 @pytest.mark.parametrize(
     "decomposer_child_class",
     decomposer_list,
 )
+@pytest.mark.parametrize(
+    "nullable_ltype",
+    ["IntegerNullable", "AgeNullable"],
+)
+@pytest.mark.parametrize(
+    "handle_incompatibility",
+    [
+        True,
+        pytest.param(
+            False,
+            marks=pytest.mark.xfail(strict=True, raises=AssertionError),
+        ),
+    ],
+)
+def test_decomposer_determine_periodicity_nullable_type_incompatibility(
+    decomposer_child_class,
+    handle_incompatibility,
+    nullable_ltype,
+    generate_seasonal_data,
+):
+    """Testing that the nullable type incompatibility that caused us to add handling for the Decomposer
+    is still present in pandas. If this test is causing the test suite to fail
+    because the code below no longer raises the expected AssertionError, we should confirm that the nullable
+    types now work for our use case and remove the nullable type handling logic from Decomposer.determine_periodicity.
+    """
+    trend_degree = 2
+    period = 7
+    X, y = generate_seasonal_data(real_or_synthetic="synthetic")(
+        period,
+        trend_degree=trend_degree,
+    )
+
+    # Convert to Integer, truncating the rest of the value
+    y = ww.init_series(y.astype(int), logical_type=nullable_ltype)
+
+    if handle_incompatibility:
+        dec = decomposer_child_class(degree=trend_degree, period=period)
+        X, y = dec._handle_nullable_types(X, y)
+
+    # Introduce nans like we do in _detrend_on_fly by rolling y
+    moving_avg = 10
+    y_trend_estimate = y.rolling(moving_avg).mean().dropna()
+    subtracted_floats = y - y_trend_estimate
+
+    # Pandas will not recognize the np.NaN value in a Float64 subtracted_floats
+    # and will not drop those null values, so calling _handle_nullable_types ensures
+    # that we stay in float64 and properly drop the null values
+    dropped_nans = subtracted_floats.dropna()
+    assert len(dropped_nans) == len(y) - moving_avg + 1
+
+
+@pytest.mark.parametrize(
+    "decomposer_child_class",
+    decomposer_list,
+)
 @pytest.mark.parametrize("fit_before_decompose", [True, False])
 def test_decomposer_get_trend_dataframe_error_not_fit(
     decomposer_child_class,
     ts_data,
     fit_before_decompose,
 ):
     X, _, y = ts_data()
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py` & `evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py` & `evalml-0.73.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_arima_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_arima_regressor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import math
 from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
 import pytest
-from sktime.forecasting.arima import AutoARIMA as SKArima
-from sktime.forecasting.base import ForecastingHorizon
+import woodwork as ww
 
 from evalml.model_family import ModelFamily
 from evalml.pipelines.components import ARIMARegressor
 from evalml.preprocessing import split_data
 from evalml.problem_types import ProblemTypes
 
 pytestmark = [
@@ -472,27 +471,32 @@
     arima.fit(X_train, y_train)
 
     assert (
         arima.predict(X_test).tail(5).tolist() == arima.predict(X_test_last_5).tolist()
     )
 
 
-def test_arima_regressor_nullable_handling():
+@pytest.mark.parametrize(
+    "nullable_ltype",
+    ["IntegerNullable", "AgeNullable"],
+)
+def test_arima_regressor_with_nullable_types(nullable_ltype):
     X = pd.DataFrame()
     X["nums"] = pd.Series([i for i in range(100)], dtype="Int64")
     X.index = pd.date_range("1/1/21", periods=100)
-    X.ww.init(logical_types={"nums": "IntegerNullable"})
+    X.ww.init(logical_types={"nums": nullable_ltype})
 
     y = pd.Series([i for i in range(100)], dtype="Int64")
     y.index = pd.date_range("1/1/21", periods=100)
 
     X_train = X.ww.iloc[:80, :]
     X_test = X.ww.iloc[80:, :]
 
     y_train = y[:80]
+    y_train = ww.init_series(y_train, logical_type=nullable_ltype)
 
     arima_params = {
         "trend": None,
         "start_p": 2,
         "d": 0,
         "start_q": 2,
         "max_p": 5,
@@ -501,71 +505,11 @@
         "seasonal": True,
         "maxiter": 10,
         "n_jobs": -1,
     }
 
     evalml_arima = ARIMARegressor(**arima_params)
     evalml_arima.fit(X_train, y_train)
-    preds = evalml_arima.predict(X=X_test)
+    preds = evalml_arima.predict(X=X_test.ww.copy())
     assert not preds.isnull().any().any()
-
-
-@pytest.mark.parametrize(
-    "nullable_ltype",
-    ["IntegerNullable", "AgeNullable"],
-)
-@pytest.mark.parametrize(
-    "handle_incompatibility",
-    [
-        True,
-        pytest.param(
-            False,
-            marks=pytest.mark.xfail(strict=True, raises=ValueError),
-        ),
-    ],
-)
-def test_arima_nullable_type_incompatibility(
-    handle_incompatibility,
-    nullable_ltype,
-):
-    """Testing that the nullable type incompatibility that caused us to add handling for ARIMARegressor
-    is still present in sktime's AutoARIMA component. If this test is causing the test suite to fail
-    because the code below no longer raises the expected ValueError, we should confirm that the nullable
-    types now work for our use case and remove the nullable type handling logic from ARIMARegressor.
-    """
-    X = pd.DataFrame()
-    X["nums"] = pd.Series([i for i in range(100)], dtype="Int64")
-    X.index = pd.date_range("1/1/21", periods=100)
-    X.ww.init(logical_types={"nums": nullable_ltype})
-
-    y = pd.Series([i for i in range(100)], dtype="Int64")
-    y.index = pd.date_range("1/1/21", periods=100)
-
-    arima_params = {
-        "trend": None,
-        "start_p": 2,
-        "d": 0,
-        "start_q": 2,
-        "max_p": 5,
-        "max_d": 2,
-        "max_q": 5,
-        "seasonal": True,
-        "maxiter": 10,
-        "n_jobs": -1,
-    }
-
-    if handle_incompatibility:
-        evalml_arima = ARIMARegressor(**arima_params)
-        X, y = evalml_arima._handle_nullable_types(X, y)
-
-    X_train = X.ww.iloc[:80, :]
-    X_test = X.ww.iloc[80:, :]
-    y_train = y[:80]
-
-    # SKTime's AutoARIMA regressor cannot handle IntegerNullable type
-    sk_arima = SKArima(**arima_params)
-    fh_ = ForecastingHorizon(
-        [i + 1 for i in range(len(X_test))],
-        is_relative=True,
-    )
-    sk_arima.fit(y=y_train, X=X_train)
-    sk_arima.predict(fh=fh_, X=X_test)
+    results_coverage = evalml_arima.get_prediction_intervals(X=X_test.ww.copy())
+    assert results_coverage
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_baseline_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_baseline_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_catboost_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_catboost_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_column_selector_transformers.py` & `evalml-0.73.0/evalml/tests/component_tests/test_column_selector_transformers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_components.py` & `evalml-0.73.0/evalml/tests/component_tests/test_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_datetime_featurizer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_decision_tree_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_decision_tree_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_drop_rows_transformer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_en_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_en_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_en_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_en_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_estimators.py` & `evalml-0.73.0/evalml/tests/component_tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_et_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_et_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py`

 * *Files 17% similar despite different names*

```diff
@@ -198,68 +198,22 @@
     assert (y_pred_sk.values == y_pred.values).all()
 
 
 @pytest.mark.parametrize(
     "nullable_y_ltype",
     ["IntegerNullable", "AgeNullable", "BooleanNullable"],
 )
-def test_handle_nullable_types(
+def test_estimator_with_nullable_types(
     nullable_type_test_data,
     nullable_type_target,
     nullable_y_ltype,
 ):
     y = nullable_type_target(ltype=nullable_y_ltype, has_nans=False)
     X = nullable_type_test_data(has_nans=False)
     X = X.ww.select(include=["numeric", "Boolean", "BooleanNullable"])
 
     comp = ExponentialSmoothingRegressor()
 
-    X_d, y_d = comp._handle_nullable_types(X, y)
-    comp.fit(X_d, y_d)
-    comp.predict(X_d)
-
-
-@pytest.mark.parametrize(
-    "nullable_y_ltype",
-    ["IntegerNullable", "AgeNullable", "BooleanNullable"],
-)
-@pytest.mark.parametrize(
-    "handle_incompatibility",
-    [
-        True,
-        pytest.param(
-            False,
-            marks=pytest.mark.xfail(strict=True, raises=ValueError),
-        ),
-    ],
-)
-def test_exponential_smoothing_regressor_nullable_type_incompatibility(
-    nullable_type_target,
-    nullable_type_test_data,
-    handle_incompatibility,
-    nullable_y_ltype,
-):
-    """Testing that the nullable type incompatibility that caused us to add handling for ExponentialSmoothingRegressor
-    is still present in sktime's ForecastingHorizon component. If this test is causing the test suite to fail
-    because the code below no longer raises the expected ValueError, we should confirm that the nullable
-    types now work for our use case and remove the nullable type handling logic from ExponentialSmoothingRegressor.
-    """
-    from sktime.forecasting.base import ForecastingHorizon
-    from sktime.forecasting.exp_smoothing import ExponentialSmoothing
-
-    y = nullable_type_target(ltype=nullable_y_ltype, has_nans=False)
-    X = nullable_type_test_data(has_nans=False)
-    X = X.ww.select(include=["numeric", "Boolean", "BooleanNullable"])
-
-    if handle_incompatibility:
-        comp = ExponentialSmoothingRegressor()
-        X, y = comp._handle_nullable_types(X, y)
-
-    X_train = X.ww.iloc[:10, :]
-    X_test = X.ww.iloc[10:, :]
-    y_train = y[:10]
-
-    fh_ = ForecastingHorizon([i + 1 for i in range(len(X_test))], is_relative=True)
-
-    sk_comp = ExponentialSmoothing()
-    sk_comp.fit(X=X_train, y=y_train)
-    sk_comp.predict(fh=fh_)
+    # Copy X to avoid X taking on any mutations from the internal _handle_nullable_types call
+    comp.fit(X.ww.copy(), y)
+    comp.predict(X.ww.copy())
+    comp.get_prediction_intervals(X.ww.copy())
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_feature_selectors.py` & `evalml-0.73.0/evalml/tests/component_tests/test_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_featuretools.py` & `evalml-0.73.0/evalml/tests/component_tests/test_featuretools.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 import featuretools as ft
 import pandas as pd
 import pytest
 import woodwork as ww
 from featuretools.feature_base import IdentityFeature
 from pandas.testing import assert_frame_equal
-from woodwork.logical_types import Boolean, Categorical, Datetime, Double, Integer
+from woodwork.logical_types import (
+    Boolean,
+    Categorical,
+    Datetime,
+    Double,
+    Integer,
+)
 
 from evalml.demos import load_diabetes
 from evalml.pipelines.components import DFSTransformer
 
 
 def test_index_errors(X_y_binary):
     with pytest.raises(TypeError, match="Index provided must be string"):
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py` & `evalml-0.73.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 
 def make_answer_email_fit_transform(df_with_url_and_email):
     expected = df_with_url_and_email.ww.copy()
     expected.ww["EMAIL_ADDRESS_TO_DOMAIN(email)"] = pd.Series(
         ["gmail.com", "yahoo.com", "abalone.com", "hotmail.com", "email.org"],
         dtype="category",
     )
-    expected.ww["IS_FREE_EMAIL_DOMAIN(email)"] = pd.Series(
-        [True, True, False, True, True],
-        dtype="category",
+    expected.ww["IS_FREE_EMAIL_DOMAIN(email)"] = ww.init_series(
+        pd.Series(
+            [True, True, False, True, True],
+        ),
+        logical_type="BooleanNullable",
     )
     expected.ww.drop(["email"], inplace=True)
     return expected
 
 
 def make_answer_url_fit_transform(df_with_url_and_email):
     expected = df_with_url_and_email.ww.copy()
@@ -89,19 +91,19 @@
     )
     expected.ww["EMAIL_ADDRESS_TO_DOMAIN(email_2)"] = pd.Series(
         [None, None, "abalone.com", "hotmail.com", None],
         dtype="category",
     )
     expected.ww["IS_FREE_EMAIL_DOMAIN(email)"] = pd.Series(
         [None, None, False, True, True],
-        dtype="category",
+        dtype="boolean",
     )
     expected.ww["IS_FREE_EMAIL_DOMAIN(email_2)"] = pd.Series(
         [None, None, False, True, None],
-        dtype="category",
+        dtype="boolean",
     )
     return expected
 
 
 def make_answer_url_fit_transform_missing_values(df_with_url_and_email):
     df_with_missing_values = make_data_url_fit_transform_missing_values(
         df_with_url_and_email,
@@ -137,15 +139,15 @@
     return expected
 
 
 def make_expected_logical_types_email_fit_transform():
     return {
         "categorical": ww.logical_types.Categorical(),
         "numeric": ww.logical_types.Double(),
-        "IS_FREE_EMAIL_DOMAIN(email)": ww.logical_types.Categorical(),
+        "IS_FREE_EMAIL_DOMAIN(email)": ww.logical_types.BooleanNullable(),
         "EMAIL_ADDRESS_TO_DOMAIN(email)": ww.logical_types.Categorical(),
         "integer": ww.logical_types.Integer(),
         "boolean": ww.logical_types.Boolean(),
         "nat_lang": ww.logical_types.NaturalLanguage(),
         "url": ww.logical_types.URL(),
     }
 
@@ -166,16 +168,16 @@
 
 def make_expected_logical_types_email_fit_transform_missing_values():
     return {
         "categorical": ww.logical_types.Categorical(),
         "numeric": ww.logical_types.Double(),
         "EMAIL_ADDRESS_TO_DOMAIN(email)": ww.logical_types.Categorical(),
         "EMAIL_ADDRESS_TO_DOMAIN(email_2)": ww.logical_types.Categorical(),
-        "IS_FREE_EMAIL_DOMAIN(email)": ww.logical_types.Categorical(),
-        "IS_FREE_EMAIL_DOMAIN(email_2)": ww.logical_types.Categorical(),
+        "IS_FREE_EMAIL_DOMAIN(email)": ww.logical_types.BooleanNullable(),
+        "IS_FREE_EMAIL_DOMAIN(email_2)": ww.logical_types.BooleanNullable(),
         "integer": ww.logical_types.Integer(),
         "boolean": ww.logical_types.Boolean(),
         "nat_lang": ww.logical_types.NaturalLanguage(),
         "url": ww.logical_types.URL(),
     }
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_imputer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_imputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,24 @@
 import woodwork as ww
 from pandas.testing import assert_frame_equal
 from woodwork.logical_types import (
     Boolean,
     BooleanNullable,
     Categorical,
     Double,
+    Integer,
+    IntegerNullable,
     NaturalLanguage,
 )
 
 from evalml.pipelines.components import Imputer
-from evalml.pipelines.components.transformers.imputers import KNNImputer, SimpleImputer
+from evalml.pipelines.components.transformers.imputers import (
+    KNNImputer,
+    SimpleImputer,
+)
 
 
 def test_invalid_strategy_parameters():
     with pytest.raises(ValueError, match="Valid numeric imputation strategies are"):
         Imputer(numeric_impute_strategy="not a valid strategy")
     with pytest.raises(ValueError, match="Valid categorical imputation strategies are"):
         Imputer(categorical_impute_strategy="mean")
@@ -175,14 +180,15 @@
                 ["zero", "one", "two", "zero", "two"] * 4,
                 dtype="category",
             ),
             "int col": [0, 1, 2, 0, 3] * 4,
             "object col": pd.Series(["b", "b", "a", "c", "d"] * 4, dtype="category"),
             "float col": [0.1, 1.0, 0.0, -2.0, 5.0] * 4,
             "bool col": [True, False, False, True, True] * 4,
+            "bool col 2": [True, False, False, True, True] * 4,
             "natural language col": pd.Series(
                 ["cats are really great", "don't", "believe", "me?", "well..."] * 4,
                 dtype="string",
             ),
             "categorical with nan": pd.Series(
                 ["0", "1", "0", "0", "3"] * 4,
                 dtype="category",
@@ -526,15 +532,15 @@
 
 
 @pytest.mark.parametrize("data_type", ["pd", "ww"])
 def test_imputer_bool_dtype_object(data_type, make_data_type):
     X = pd.DataFrame([True, np.nan, False, np.nan, True] * 4)
     X.ww.init(logical_types={0: BooleanNullable})
     y = pd.Series([1, 0, 0, 1, 0] * 4)
-    X_expected_arr = pd.DataFrame([True, True, False, True, True] * 4, dtype="bool")
+    X_expected_arr = pd.DataFrame([True, True, False, True, True] * 4, dtype="boolean")
     X = make_data_type(data_type, X)
     y = make_data_type(data_type, y)
     imputer = Imputer()
     imputer.fit(X, y)
     X_t = imputer.transform(X)
     assert_frame_equal(X_expected_arr, X_t)
 
@@ -554,15 +560,15 @@
         logical_types={"bool with nan": BooleanNullable, "bool no nan": Boolean},
     )
     y = pd.Series([1, 0, 0, 1, 0] * 4)
     X_multi_expected_arr = pd.DataFrame(
         {
             "bool with nan": pd.Series(
                 [True, False, False, False, False] * 4,
-                dtype="bool",
+                dtype="boolean",
             ),
             "bool no nan": pd.Series(
                 [False, False, False, False, True] * 4,
             ),
         },
     )
 
@@ -572,71 +578,77 @@
     imputer = Imputer()
     imputer.fit(X_multi, y)
     X_multi_t = imputer.transform(X_multi)
     assert_frame_equal(X_multi_expected_arr, X_multi_t)
 
 
 def test_imputer_int_preserved():
+    # With mean impute strategy, the integer nullable column should become Double
     X = pd.DataFrame(pd.Series([1, 2, 11, np.nan]))
     imputer = Imputer(numeric_impute_strategy="mean")
     transformed = imputer.fit_transform(X)
     pd.testing.assert_frame_equal(
         transformed,
         pd.DataFrame(pd.Series([1, 2, 11, 14 / 3])),
     )
     assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {
         0: Double,
     }
 
+    # With mean impute strategy, the integer nullable column should become Double even if mean is an integer
     X = pd.DataFrame(pd.Series([1, 2, 3, np.nan]))
     imputer = Imputer(numeric_impute_strategy="mean")
     transformed = imputer.fit_transform(X)
     pd.testing.assert_frame_equal(
         transformed,
         pd.DataFrame(pd.Series([1, 2, 3, 2])),
         check_dtype=False,
     )
     assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {
         0: Double,
     }
 
+    # If no null values need to be imputed, integer column should be maintained
+    # even with mean impute strategy.
     X = pd.DataFrame(pd.Series([1, 2, 3, 4], dtype="int"))
     imputer = Imputer(numeric_impute_strategy="mean")
     transformed = imputer.fit_transform(X)
     pd.testing.assert_frame_equal(
         transformed,
         pd.DataFrame(pd.Series([1, 2, 3, 4])),
         check_dtype=False,
     )
-    assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {0: Double}
+    assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {0: Integer}
 
 
 @pytest.mark.parametrize("null_type", ["pandas_na", "numpy_nan", "python_none"])
 @pytest.mark.parametrize("test_case", ["boolean_with_null", "boolean_without_null"])
 def test_imputer_bool_preserved(test_case, null_type):
     if test_case == "boolean_with_null":
         null_type = {"pandas_na": pd.NA, "numpy_nan": np.nan, "python_none": None}[
             null_type
         ]
         X = pd.DataFrame(pd.Series([True, False, True, null_type] * 4))
         X.ww.init(logical_types={0: BooleanNullable})
         expected = pd.DataFrame(
-            pd.Series([True, False, True, True] * 4, dtype="bool"),
+            pd.Series([True, False, True, True] * 4, dtype="boolean"),
         )
+        expected_ltype = BooleanNullable
     elif test_case == "boolean_without_null":
         X = pd.DataFrame(pd.Series([True, False, True, False] * 4))
         expected = pd.DataFrame(pd.Series([True, False, True, False] * 4))
+        expected_ltype = Boolean
     imputer = Imputer(categorical_impute_strategy="most_frequent")
     transformed = imputer.fit_transform(X)
     pd.testing.assert_frame_equal(
         transformed,
         expected,
     )
     assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {
-        0: Boolean,
+        0: expected_ltype,
     }
 
 
 def test_imputer_does_not_erase_ww_info():
     df_train = pd.DataFrame({"a": [1, 2, 3, 2], "b": ["a", "b", "b", "c"]})
     df_holdout = pd.DataFrame({"a": [2], "b": [None]})
     df_train.ww.init(logical_types={"a": "Double", "b": "Categorical"})
@@ -678,22 +690,24 @@
     X_df = {
         "int col": imputer_test_data[["int col"]],
         "float col": imputer_test_data[["float col"]],
         "categorical col": imputer_test_data[["categorical col"]],
         "bool col": imputer_test_data[["bool col"]],
     }[data]
     logical_type = {
-        "Integer": Double,
+        "Integer": Integer,
         "Double": Double,
         "Categorical": Categorical,
         "NaturalLanguage": NaturalLanguage,
         "Boolean": Boolean,
     }[logical_type]
     if has_nan == "has_nan" and logical_type == Boolean:
         logical_type = BooleanNullable
+    elif has_nan == "has_nan" and logical_type == Integer:
+        logical_type = IntegerNullable
     y = pd.Series([1, 2, 1])
     try:
         X = X_df.copy()
         if has_nan == "has_nan" and logical_type == BooleanNullable:
             X.iloc[len(X_df) - 1, 0] = None
         elif has_nan == "has_nan":
             X.iloc[len(X_df) - 1, 0] = np.nan
@@ -701,23 +715,19 @@
     except ww.exceptions.TypeConversionError:
         return
 
     imputer = Imputer(numeric_impute_strategy=numeric_impute_strategy)
     imputer.fit(X, y)
     transformed = imputer.transform(X, y)
     assert isinstance(transformed, pd.DataFrame)
-    if logical_type == BooleanNullable:
-        assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {
-            data: Boolean,
-        }
-    elif numeric_impute_strategy == "most_frequent":
-        assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {
-            data: logical_type,
-        }
-    elif logical_type in [Categorical, NaturalLanguage] or has_nan == "no_nans":
+    if (
+        logical_type in [Categorical, NaturalLanguage, BooleanNullable]
+        or has_nan == "no_nans"
+        or numeric_impute_strategy == "most_frequent"
+    ):
         assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {
             data: logical_type,
         }
     else:
         assert {k: type(v) for k, v in transformed.ww.logical_types.items()} == {
             data: Double,
         }
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_knn_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_knn_imputer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_knn_imputer.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 @pytest.mark.parametrize("df_composition", ["full_df", "single_column"])
 @pytest.mark.parametrize("has_nan", ["has_nan", "no_nans"])
 def test_knn_imputer_ignores_natural_language(
     has_nan,
     imputer_test_data,
     df_composition,
 ):
-    """Test to ensure that the simple imputer just passes through
+    """Test to ensure that the knn imputer just passes through
     natural language columns, unchanged.
     """
     if df_composition == "single_column":
         X_df = imputer_test_data[["natural language col"]]
         X_df.ww.init()
     elif df_composition == "full_df":
         X_df = imputer_test_data[["int col", "float col", "natural language col"]]
@@ -52,20 +52,16 @@
     imputer = KNNImputer(number_neighbors=3)
 
     imputer.fit(X_df, y)
 
     result = imputer.transform(X_df, y)
 
     if df_composition == "full_df":
-        X_df = X_df.astype(
-            {"int col": float},
-        )  # Convert to float as the imputer will do this as we're requesting KNN
-        result = result.astype(
-            {"int col": float},
-        )
+        # Update the other columns in result so that we can confirm the natural language column
+        # is unchanged
         X_df["float col"] = result["float col"]
         X_df["int col"] = result["int col"]
         assert_frame_equal(result, X_df)
     elif df_composition == "single_column":
         assert_frame_equal(result, X_df)
 
 
@@ -81,7 +77,20 @@
     result = imputer.transform(X, y)
     assert unchanged_schema == result.ww.drop(int_nullable_cols).ww.schema
     assert {
         str(ltype)
         for col, ltype in result.ww.logical_types.items()
         if col in int_nullable_cols
     } == {"Double"}
+
+
+def test_knn_imputer_with_all_null_and_nl_cols(
+    imputer_test_data,
+):
+    X = imputer_test_data.ww[["all nan", "natural language col", "int col"]]
+    X_copy = X.ww.copy()
+
+    imp = KNNImputer(number_neighbors=3)
+    imp.fit(X)
+
+    X_imputed = imp.transform(X)
+    pd.testing.assert_frame_equal(X_copy.ww.drop("all nan"), X_imputed)
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_label_encoder.py` & `evalml-0.73.0/evalml/tests/component_tests/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_lda.py` & `evalml-0.73.0/evalml/tests/component_tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_lgbm_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_lgbm_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,31 +328,31 @@
     assert mock_predict.call_args[0][0].ww.schema == original_schema
     lgb.predict_proba(X)
     assert mock_predict_proba.call_args[0][0].ww.schema == original_schema
 
 
 @pytest.mark.parametrize(
     "nullable_y_ltype",
-    ["IntegerNullable", "AgeNullable"],
+    ["IntegerNullable", "AgeNullable", "BooleanNullable"],
 )
-def test_lgbm_handle_nullable_types(
+def test_lgbm_with_nullable_types(
     nullable_type_test_data,
     nullable_type_target,
     nullable_y_ltype,
 ):
     y = nullable_type_target(ltype=nullable_y_ltype, has_nans=False)
     X = nullable_type_test_data(has_nans=False)
     X = X.ww.select(include=["numeric", "Boolean", "BooleanNullable"])
 
     lgb = LightGBMClassifier()
 
-    X, y = lgb._handle_nullable_types(X, y)
-    lgb.fit(X, y)
-    preds = lgb.predict(X)
-    pred_probs = lgb.predict_proba(X)
+    # Copy X to avoid X taking on any mutations from the internal _handle_nullable_types call
+    lgb.fit(X.ww.copy(), y)
+    preds = lgb.predict(X.ww.copy())
+    pred_probs = lgb.predict_proba(X.ww.copy())
 
     assert not preds.isnull().any().any()
     assert not pred_probs.isnull().any().any()
 
 
 @pytest.mark.parametrize(
     "nullable_y_ltype",
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_lgbm_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_lgbm_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,28 +230,28 @@
     assert mock_predict.call_args[0][0].ww.schema == original_schema
 
 
 @pytest.mark.parametrize(
     "nullable_y_ltype",
     ["IntegerNullable", "AgeNullable", "BooleanNullable"],
 )
-def test_lgbm_handle_nullable_types(
+def test_lgbm_with_nullable_types(
     nullable_type_test_data,
     nullable_type_target,
     nullable_y_ltype,
 ):
     y = nullable_type_target(ltype=nullable_y_ltype, has_nans=False)
     X = nullable_type_test_data(has_nans=False)
     X = X.ww.select(include=["numeric", "Boolean", "BooleanNullable"])
 
     lgb = LightGBMRegressor()
 
-    X, y = lgb._handle_nullable_types(X, y)
-    lgb.fit(X, y)
-    preds = lgb.predict(X)
+    # Copy X to avoid X taking on any mutations from the internal _handle_nullable_types call
+    lgb.fit(X.ww.copy(), y)
+    preds = lgb.predict(X.ww.copy())
 
     assert not preds.isnull().any().any()
 
 
 @pytest.mark.parametrize(
     "nullable_y_ltype",
     ["IntegerNullable", "AgeNullable", "BooleanNullable"],
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_log_transformer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_lsa.py` & `evalml-0.73.0/evalml/tests/component_tests/test_lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_natural_language_featurizer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_nullable_types_replacer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_nullable_types_replacer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_one_hot_encoder.py` & `evalml-0.73.0/evalml/tests/component_tests/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_ordinal_encoder.py` & `evalml-0.73.0/evalml/tests/component_tests/test_ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_oversampler.py` & `evalml-0.73.0/evalml/tests/component_tests/test_oversampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,26 +258,47 @@
     X_im, y_im = imb_sampler.fit_resample(X, y)
 
     np.testing.assert_equal(X_com.values, X_im)
     np.testing.assert_equal(y_com.values, y_im)
     np.testing.assert_equal(sorted(y_im), expected_y)
 
 
-def test_smoten_categorical_boolean(X_y_binary, im):
+@pytest.mark.parametrize("use_nullable", [True, False])
+def test_smoten_categorical_boolean(X_y_binary, im, use_nullable):
     X, y = X_y_binary
-    X.ww.set_types({0: "Categorical", 1: "Boolean"})
-    X = X.drop(range(2, len(X.columns)), axis=1)
+    bool_ltype = "BooleanNullable" if use_nullable else "Boolean"
+    # Set the 0 column of float values to be Categorical type
+    X.ww.set_types({0: "Categorical"})
+    # Add a Boolean column into X
+    X.ww[len(X.columns)] = ww.init_series(
+        pd.Series([True, False] * 50),
+        logical_type=bool_ltype,
+    )
+    X = X.ww.select(["Boolean", "BooleanNullable", "Categorical"])
+
     sn = Oversampler()
     _ = sn.fit_transform(X, y)
     assert sn.sampler == im.SMOTEN
 
 
-def test_smotenc_boolean_numeric(X_y_binary, im):
-    X, y = X_y_binary
-    X.ww.set_types({5: "Boolean", 12: "Boolean"})
+@pytest.mark.parametrize("use_nullable_1", [True, False])
+@pytest.mark.parametrize("use_nullable_2", [True, False])
+def test_smotenc_boolean_numeric(X_y_binary, im, use_nullable_1, use_nullable_2):
+    bool_ltype_1 = "BooleanNullable" if use_nullable_1 else "Boolean"
+    bool_ltype_2 = "BooleanNullable" if use_nullable_2 else "Boolean"
+    X, y = X_y_binary
+    # Add two boolean columns into X
+    X.ww[len(X.columns)] = ww.init_series(
+        pd.Series([True, False] * 50),
+        logical_type=bool_ltype_1,
+    )
+    X.ww[len(X.columns)] = ww.init_series(
+        pd.Series([True, False] * 50),
+        logical_type=bool_ltype_2,
+    )
     snc = Oversampler()
     _, _ = snc.fit_transform(X, y)
     assert snc.sampler == im.SMOTENC
 
 
 def test_smotenc_categorical_features(X_y_binary):
     X, y = X_y_binary
@@ -299,25 +320,30 @@
     X = pd.DataFrame(X).rename({0: "postal", 1: "country"}, axis="columns")
     X["2"] = [i % 2 for i in range(X.shape[0])]
 
     # Replace postal and country features with plausible postal/country codes
     X["postal"] = np.arange(10001, 10001 + X.shape[0])
     X["country"] = np.arange(20001, 20001 + X.shape[0])
 
+    # Add different types of categorical data - boolean values, string categories, and postal codes
     X_ww = infer_feature_types(
         X,
         feature_types={
             "postal": "PostalCode",
             "country": "CountryCode",
             "2": "Boolean",
         },
     )
+    X_ww.ww[str(len(X.columns))] = ww.init_series(
+        pd.Series([True, False] * 50),
+        logical_type="BooleanNullable",
+    )
     snc = Oversampler()
     _ = snc.fit_transform(X_ww, y)
-    assert snc.categorical_features == [20, 21, 2]
+    assert snc.categorical_features == [20, 21, 2, len(X.columns)]
 
 
 def test_smotenc_output_shape(X_y_binary):
     X, y = X_y_binary
     y_imbalanced = pd.Series([0] * 90 + [1] * 10)
     X_ww = infer_feature_types(X, feature_types={0: "Categorical", 1: "Categorical"})
     snc = Oversampler()
@@ -446,24 +472,28 @@
     nullable_type_test_data,
     nullable_type_target,
     nullable_y_ltype,
 ):
     X = nullable_type_test_data(has_nans=False)
     # Oversampler can only handle numeric and boolean columns
     X = X.ww.select(include=["numeric", "Boolean", "BooleanNullable", "category"])
+    original_schema = X.ww.schema
     y = nullable_type_target(ltype=nullable_y_ltype, has_nans=False)
 
     oversampler = Oversampler(sampling_ratio=0.5)
     oversampler.fit(X.ww.copy(), y)
     X_t, y_t = oversampler.transform(X.ww.copy(), y)
 
     # Confirm oversampling happened by checking the length increased
     assert len(X_t) > len(X)
     assert len(y_t) > len(y)
 
+    # Confirm the original types are maintained
+    assert original_schema == X_t.ww.schema
+
 
 @pytest.mark.parametrize(
     "nullable_y_ltype",
     ["IntegerNullable", "AgeNullable", "BooleanNullable"],
 )
 @pytest.mark.parametrize(
     "im_oversampler",
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_pca.py` & `evalml-0.73.0/evalml/tests/component_tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_per_column_imputer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_prophet_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_simple_imputer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_simple_imputer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import pandas
 import pandas as pd
 import pytest
 import woodwork as ww
-import woodwork.exceptions
 from pandas.testing import assert_frame_equal
 from woodwork.logical_types import (
     Boolean,
     BooleanNullable,
     Categorical,
     Double,
     Integer,
@@ -622,7 +621,60 @@
 
     imp = SimpleImputer()
     imp.fit(X_train, y)
 
     X_t = imp.transform(X_test)
     assert not X_t["a"].isna().any()
     assert isinstance(X_t.ww.logical_types["a"], BooleanNullable)
+
+
+def test_simple_imputer_all_bools_at_fit_and_transform(imputer_test_data):
+    """Confirms that the simple imputer can handle data with only the bool dtype
+    which sklearn would error on."""
+    X = imputer_test_data.ww.select("boolean")
+
+    imp = SimpleImputer(impute_strategy="most_frequent")
+    imp.fit(X)
+
+    X_imputed = imp.transform(X)
+    pd.testing.assert_frame_equal(X, X_imputed)
+
+
+def test_simple_imputer_all_bools_at_fit_and_transform_with_all_null_and_nl_cols(
+    imputer_test_data,
+):
+    """Confirm that the simple imputer, which doesn't pass all null or natural language columns
+    to sklearn works when the remaining columns are all teh bool dtype, which sklearn would error on.
+    """
+    X = imputer_test_data.ww[
+        ["all nan", "bool col", "bool col 2", "natural language col"]
+    ]
+    X_copy = X.ww.copy()
+
+    imp = SimpleImputer(impute_strategy="most_frequent")
+    imp.fit(X)
+
+    X_imputed = imp.transform(X)
+    pd.testing.assert_frame_equal(X_copy.ww.drop("all nan"), X_imputed)
+
+
+def test_simple_imputer_all_bools_at_fit_with_nans_at_transform(imputer_test_data):
+    """Confirm that the simple imputer can handle data whose dtype is different at transform
+    when originally the data only had bool dtype columns."""
+    # X_train will be only bool dtypes so the _component_obj won't be fit
+    X_train = imputer_test_data.ww.select("boolean")
+
+    imp = SimpleImputer(impute_strategy="most_frequent")
+    imp.fit(X_train)
+
+    # X_test will be BooleanNullable which will be a problem when _component_obj isn't fit
+    X_test = X_train.copy()
+    X_test.iloc[-1] = np.nan
+    X_test.ww.init(
+        logical_types={
+            "bool col": "BooleanNullable",
+            "bool col 2": "BooleanNullable",
+        },
+    )
+
+    X_imputed = imp.transform(X_test)
+    assert not X_imputed.isna().any().any()
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_standard_scaler.py` & `evalml-0.73.0/evalml/tests/component_tests/test_standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_svm_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_svm_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_target_encoder.py` & `evalml-0.73.0/evalml/tests/component_tests/test_target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_target_imputer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_target_imputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,16 +123,16 @@
     imputer.fit(None, y)
     _, y_t = imputer.transform(None, y)
     assert_series_equal(y_expected, y_t)
 
 
 @pytest.mark.parametrize("data_type", ["pd", "ww"])
 def test_target_imputer_boolean_dtype(data_type, make_data_type):
-    y = pd.Series([True, np.nan, False, np.nan, True], dtype="category")
-    y_expected = pd.Series([True, True, False, True, True], dtype="category")
+    y = pd.Series([True, np.nan, False, np.nan, True], dtype="boolean")
+    y_expected = pd.Series([True, True, False, True, True], dtype="boolean")
     y = make_data_type(data_type, y)
     imputer = TargetImputer()
     imputer.fit(None, y)
     _, y_t = imputer.transform(None, y)
     assert_series_equal(y_expected, y_t)
 
 
@@ -149,15 +149,15 @@
     with pytest.raises(TypeError, match="Provided target full of nulls."):
         imputer.fit_transform(None, y)
 
 
 def test_target_imputer_numpy_input():
     y = np.array([np.nan, 0, 2])
     imputer = TargetImputer(impute_strategy="mean")
-    y_expected = pd.Series([1, 0, 2], dtype="int64")
+    y_expected = pd.Series([1, 0, 2], dtype="float64")
     _, y_t = imputer.fit_transform(None, y)
     assert y_expected.equals(y_t)
     np.testing.assert_almost_equal(y, np.array([np.nan, 0, 2]))
 
 
 def test_target_imputer_does_not_reset_index():
     y = pd.Series(np.arange(10))
@@ -205,16 +205,16 @@
     "y, y_expected",
     [
         (
             pd.Series(["b", "a", "a", None] * 4, dtype="category"),
             pd.Series(["b", "a", "a", "a"] * 4, dtype="category"),
         ),
         (
-            pd.Series([True, None, False, True], dtype="category"),
-            pd.Series([True, True, False, True], dtype="category"),
+            pd.Series([True, None, False, True], dtype="boolean"),
+            pd.Series([True, True, False, True], dtype="bool"),
         ),
         (
             pd.Series(["b", "a", "a", None] * 4),
             pd.Series(["b", "a", "a", "a"] * 4, dtype="category"),
         ),
     ],
 )
@@ -261,7 +261,28 @@
         imputer.fit(None, y)
         _, y_t = imputer.transform(None, y)
 
         if impute_strategy_to_use == "most_frequent" or not has_nan:
             assert type(y_t.ww.logical_type) == logical_type
         else:
             assert type(y_t.ww.logical_type) == Double
+
+
+@pytest.mark.parametrize("impute_strategy", ["mean", "median", "most_frequent"])
+def test_target_imputer_doesnt_truncate_imputed_ints(impute_strategy):
+    y = pd.Series([1, 2, 3, 3, pd.NA], dtype="Int64")
+    y = ww.init_series(y, logical_type="IntegerNullable")
+
+    imputer = TargetImputer(impute_strategy=impute_strategy)
+    imputer.fit(None, y)
+
+    _, y_t = imputer.transform(None, y)
+    expected_y_t = pd.Series(
+        imputer._component_obj.transform(y.ww.to_frame())[:, 0],
+        index=y.index,
+    )
+
+    if impute_strategy != "most_frequent":
+        # Confirm floating points are present
+        assert not (expected_y_t % 1 == 0).all()
+
+    assert_series_equal(y_t, expected_y_t, check_dtype=False)
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_time_series_featurizer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_time_series_imputer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_time_series_imputer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.testing import assert_frame_equal, assert_series_equal
-from woodwork.logical_types import Boolean, BooleanNullable, IntegerNullable
+from woodwork.logical_types import (
+    AgeFractional,
+    Boolean,
+    BooleanNullable,
+    Double,
+    IntegerNullable,
+)
 
 from evalml.pipelines.components import TimeSeriesImputer
 
 
 def test_invalid_strategy_parameters():
     with pytest.raises(ValueError, match="Valid numeric impute strategies are"):
         TimeSeriesImputer(numeric_impute_strategy="mean")
@@ -125,14 +131,15 @@
             ),
             "object with nan": pd.Series(
                 ["b", "b", "b", "c", "c"] * 4,
                 dtype="category",
             ),
             "bool col with nan": pd.Series(
                 [True, True, False, False, True] * 4,
+                dtype="bool",
             ),
         },
     )
     imputer = TimeSeriesImputer()
     transformed, _ = imputer.fit_transform(X, y)
     assert_frame_equal(transformed, expected, check_dtype=True)
     assert "all nan cat" not in transformed.columns
@@ -143,38 +150,41 @@
     )
     expected["object with nan"] = pd.Series(
         ["b", "b", "c", "c", "b"] * 3 + ["b", "b", "c", "c", "c"],
         dtype="category",
     )
     expected["bool col with nan"] = pd.Series(
         [True, False, False, True, True] * 4,
+        dtype="bool",
     )
 
     imputer = TimeSeriesImputer(categorical_impute_strategy="backwards_fill")
     transformed, _ = imputer.fit_transform(X, y)
     assert_frame_equal(transformed, expected, check_dtype=True)
 
 
 def test_categorical_and_numeric_input(imputer_test_data):
     X = imputer_test_data
     y = pd.Series([0, 0, 1, 0, 1])
     imputer = TimeSeriesImputer()
     imputer.fit(X, y)
-    transformed, _ = imputer.transform(X, y)
+    # Copy X to avoid X taking on any mutations from the internal _handle_nullable_types call
+    transformed, _ = imputer.transform(X.ww.copy(), y)
     expected = pd.DataFrame(
         {
             "dates": pd.date_range("01-01-2022", periods=20),
             "categorical col": pd.Series(
                 ["zero", "one", "two", "zero", "two"] * 4,
                 dtype="category",
             ),
             "int col": [0, 1, 2, 0, 3] * 4,
             "object col": pd.Series(["b", "b", "a", "c", "d"] * 4, dtype="category"),
             "float col": [0.1, 1.0, 0.0, -2.0, 5.0] * 4,
             "bool col": [True, False, False, True, True] * 4,
+            "bool col 2": [True, False, False, True, True] * 4,
             "natural language col": pd.Series(
                 ["cats are really great", "don't", "believe", "me?", "well..."] * 4,
                 dtype="string",
             ),
             "categorical with nan": pd.Series(
                 ["1", "1", "0", "0", "3"] + ["3", "1", "0", "0", "3"] * 3,
                 dtype="category",
@@ -192,15 +202,16 @@
     )
     assert_frame_equal(transformed, expected, check_dtype=False)
 
     imputer = TimeSeriesImputer(
         numeric_impute_strategy="forwards_fill",
         categorical_impute_strategy="forwards_fill",
     )
-    transformed, _ = imputer.fit_transform(X, y)
+    # Copy X to avoid X taking on any mutations from the internal _handle_nullable_types call
+    transformed, _ = imputer.fit_transform(X.ww.copy(), y)
     expected["float with nan"] = [0.3, 1.0, 1.0, -1.0, 0.0] * 4
     assert_frame_equal(transformed, expected, check_dtype=False)
 
 
 def test_impute_target():
     X = pd.DataFrame({"dates": pd.date_range("01-01-2022", periods=20)})
     y = pd.Series([0, 1, 0, 1, np.nan] * 4)
@@ -557,34 +568,72 @@
     assert (
         transformed.ww.logical_types["categorical with nan"]
         == X.ww.logical_types["categorical with nan"]
     )
 
 
 @pytest.mark.parametrize(
-    "nullable_ltype",
-    ["BooleanNullable", "IntegerNullable", "AgeNullable"],
+    "nullable_y_ltype, expected_imputed_y_ltype",
+    [
+        ("BooleanNullable", Double),
+        ("IntegerNullable", Double),
+        ("AgeNullable", AgeFractional),
+    ],
+)
+@pytest.mark.parametrize(
+    "numeric_impute_strategy",
+    ["forwards_fill", "backwards_fill", "interpolate"],
 )
 def test_imputer_can_take_in_nullable_types(
     nullable_type_test_data,
     nullable_type_target,
-    nullable_ltype,
+    numeric_impute_strategy,
+    nullable_y_ltype,
+    expected_imputed_y_ltype,
 ):
-    y = nullable_type_target(ltype=nullable_ltype, has_nans=True)
+    y = nullable_type_target(ltype=nullable_y_ltype, has_nans=True)
     X = nullable_type_test_data(has_nans=True)
-    # Only numeric imputing has interpolate as an option
-    X = X.ww.select("numeric")
+    # Drop the fully null columns since aren't relevant to the handle nullable types checks
+    X = X.ww.drop(["all nan", "all nan cat"])
 
-    imputer = TimeSeriesImputer(numeric_impute_strategy="interpolate")
-    imputer.fit(X, y)
-    X_imputed, y_imputed = imputer.transform(X, y)
+    cols_expected_to_change = X.ww.schema._filter_cols(
+        include=["IntegerNullable", "AgeNullable", "BooleanNullable"],
+    )
+    cols_expected_to_stay_the_same = X.ww.schema._filter_cols(
+        exclude=["IntegerNullable", "AgeNullable", "BooleanNullable"],
+    )
+
+    imputer = TimeSeriesImputer(
+        numeric_impute_strategy=numeric_impute_strategy,
+        target_impute_strategy="interpolate",
+    )
+    # Copy X to avoid X taking on any mutations from the internal _handle_nullable_types call
+    imputer.fit(X.ww.copy(), y)
+    X_imputed, y_imputed = imputer.transform(X.ww.copy(), y)
 
     assert not X_imputed.isnull().any().any()
     assert not y_imputed.isnull().any()
 
+    # Check that the types are as expected - when interpolate is used, we need fractional numeric ltypes
+    if numeric_impute_strategy == "interpolate":
+        expected_X_ltypes = {"AgeFractional", "Double", "Boolean"}
+    else:
+        expected_X_ltypes = {"Age", "Integer", "Boolean"}
+
+    assert X.ww.get_subset_schema(
+        cols_expected_to_stay_the_same,
+    ) == X_imputed.ww.get_subset_schema(cols_expected_to_stay_the_same)
+    assert {
+        str(ltype)
+        for col, ltype in X_imputed.ww.logical_types.items()
+        if col in cols_expected_to_change
+    } == expected_X_ltypes
+
+    assert isinstance(y_imputed.ww.logical_type, expected_imputed_y_ltype)
+
 
 @pytest.mark.parametrize(
     "categorical_impute_strategy",
     ["forwards_fill", "backwards_fill"],
 )
 @pytest.mark.parametrize(
     "numeric_impute_strategy",
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_time_series_regularizer.py` & `evalml-0.73.0/evalml/tests/component_tests/test_time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_undersampler.py` & `evalml-0.73.0/evalml/tests/component_tests/test_undersampler.py`

 * *Files 15% similar despite different names*

```diff
@@ -147,7 +147,30 @@
     dictionary = {"minority": 1, "majority": 0.5}
     expected_result = {"minority": 150, "majority": 300}
     undersampler = Undersampler(sampling_ratio_dict=dictionary)
     new_X, new_y = undersampler.fit_transform(X, y)
 
     assert len(new_X) == sum(expected_result.values())
     assert new_y.value_counts().to_dict() == expected_result
+
+
+@pytest.mark.parametrize(
+    "nullable_y_ltype",
+    ["IntegerNullable", "AgeNullable", "BooleanNullable"],
+)
+def test_undersampler_with_nullable_types(
+    nullable_type_test_data,
+    nullable_type_target,
+    nullable_y_ltype,
+):
+    X = nullable_type_test_data(has_nans=False)
+    # Undersampler can only handle numeric and boolean columns
+    X = X.ww.select(include=["numeric", "Boolean", "BooleanNullable"])
+    y = nullable_type_target(ltype=nullable_y_ltype, has_nans=False)
+
+    oversampler = Undersampler(sampling_ratio_dict={0: 1, 1: 0.5})
+    oversampler.fit(X, y)
+    X_t, y_t = oversampler.transform(X, y)
+
+    # Confirm oversampling happened by checking the length increased
+    assert len(X_t) < len(X)
+    assert len(y_t) < len(y)
```

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_xgboost_classifier.py` & `evalml-0.73.0/evalml/tests/component_tests/test_xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/component_tests/test_xgboost_regressor.py` & `evalml-0.73.0/evalml/tests/component_tests/test_xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/conftest.py` & `evalml-0.73.0/evalml/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2201,28 +2201,30 @@
                 ["zero", "one", "two", "zero", "two"] * 4,
                 dtype="category",
             ),
             "int col": [0, 1, 2, 0, 3] * 4,
             "object col": ["b", "b", "a", "c", "d"] * 4,
             "float col": [0.1, 1.0, 0.0, -2.0, 5.0] * 4,
             "bool col": [True, False, False, True, True] * 4,
+            "bool col 2": [True, False, False, True, True] * 4,
             "natural language col": pd.Series(
                 ["cats are really great", "don't", "believe", "me?", "well..."] * 4,
                 dtype="string",
             ),
         },
     )
     X.ww.init(
         logical_types={
             "dates": "datetime",
             "categorical col": "categorical",
             "int col": "integer",
             "object col": "categorical",
             "float col": "double",
             "bool col": "boolean",
+            "bool col 2": "boolean",
             "natural language col": "NaturalLanguage",
         },
     )
     return X
 
 
 @pytest.fixture
```

### Comparing `evalml-0.72.0/evalml/tests/data/churn.csv` & `evalml-0.73.0/evalml/tests/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data/daily-min-temperatures.csv` & `evalml-0.73.0/evalml/tests/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data/fraud_transactions.csv.gz` & `evalml-0.73.0/evalml/tests/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data/tips.csv` & `evalml-0.73.0/evalml/tests/data/tips.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data/titanic.csv` & `evalml-0.73.0/evalml/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check_action.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check_action_option.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_data_check_message.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_data_checks.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_data_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,24 @@
     DataCheckActionCode,
     DataCheckActionOption,
     DataCheckError,
     DataCheckMessageCode,
     DataChecks,
     DataCheckWarning,
     DateTimeFormatDataCheck,
-    DCAOParameterType,
     DefaultDataChecks,
     InvalidTargetDataCheck,
     TargetDistributionDataCheck,
     TimeSeriesParametersDataCheck,
     TimeSeriesSplittingDataCheck,
 )
 from evalml.exceptions import DataCheckInitError
 from evalml.problem_types import (
     ProblemTypes,
     is_classification,
-    is_regression,
     is_time_series,
 )
 
 
 @pytest.fixture
 def data_checks_input_dataframe():
     X = pd.DataFrame(
@@ -225,32 +223,21 @@
                 ),
             ],
         ).to_dict(),
         DataCheckError(
             message="1 row(s) (20.0%) of target values are null",
             data_check_name="InvalidTargetDataCheck",
             message_code=DataCheckMessageCode.TARGET_HAS_NULL,
-            details={"num_null_rows": 1, "pct_null_rows": 20.0},
+            details={"num_null_rows": 1, "pct_null_rows": 20.0, "rows": [2]},
             action_options=[
                 DataCheckActionOption(
-                    DataCheckActionCode.IMPUTE_COL,
+                    DataCheckActionCode.DROP_ROWS,
                     data_check_name="InvalidTargetDataCheck",
-                    parameters={
-                        "impute_strategy": {
-                            "parameter_type": DCAOParameterType.GLOBAL,
-                            "type": "category",
-                            "categories": ["mean", "most_frequent"]
-                            if is_regression(problem_type)
-                            else ["most_frequent"],
-                            "default_value": "mean"
-                            if is_regression(problem_type)
-                            else "most_frequent",
-                        },
-                    },
-                    metadata={"is_target": True},
+                    parameters={},
+                    metadata={"is_target": True, "rows": [2]},
                 ),
             ],
         ).to_dict(),
         DataCheckWarning(
             message="'all_null', 'also_all_null' has 0 unique values.",
             data_check_name="NoVarianceDataCheck",
             message_code=DataCheckMessageCode.NO_VARIANCE_ZERO_UNIQUE,
@@ -471,28 +458,21 @@
                 ),
             ],
         ).to_dict(),
         DataCheckError(
             message="1 row(s) (20.0%) of target values are null",
             data_check_name="InvalidTargetDataCheck",
             message_code=DataCheckMessageCode.TARGET_HAS_NULL,
-            details={"num_null_rows": 1, "pct_null_rows": 20.0},
+            details={"num_null_rows": 1, "pct_null_rows": 20.0, "rows": [2]},
             action_options=[
                 DataCheckActionOption(
-                    DataCheckActionCode.IMPUTE_COL,
+                    DataCheckActionCode.DROP_ROWS,
                     data_check_name="InvalidTargetDataCheck",
-                    parameters={
-                        "impute_strategy": {
-                            "parameter_type": DCAOParameterType.GLOBAL,
-                            "type": "category",
-                            "categories": ["mean", "most_frequent"],
-                            "default_value": "mean",
-                        },
-                    },
-                    metadata={"is_target": True},
+                    parameters={},
+                    metadata={"is_target": True, "rows": [2]},
                 ),
             ],
         ).to_dict(),
         DataCheckWarning(
             message="'all_null', 'also_all_null' has 0 unique values.",
             data_check_name="NoVarianceDataCheck",
             message_code=DataCheckMessageCode.NO_VARIANCE_ZERO_UNIQUE,
@@ -503,15 +483,15 @@
                     data_check_name="NoVarianceDataCheck",
                     metadata={"columns": ["all_null", "also_all_null"]},
                 ),
             ],
         ).to_dict(),
         DataCheckError(
             message="Target is unsupported integer_nullable type. Valid Woodwork "
-            "logical types include: integer, double",
+            "logical types include: integer, double, age, age_fractional",
             data_check_name="TargetDistributionDataCheck",
             message_code=DataCheckMessageCode.TARGET_UNSUPPORTED_TYPE,
             details={"unsupported_type": "integer_nullable"},
             action_options=[],
         ).to_dict(),
     ]
     validation_messages = data_checks.validate(X, y)
```

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,27 @@
         InvalidTargetDataCheck(
             "regression",
             get_default_primary_search_objective("regression"),
             n_unique=-1,
         )
 
 
+@pytest.mark.parametrize("null_strategy", ["invalid", None])
+def test_invalid_target_data_check_invalid_null_strategy(null_strategy):
+    with pytest.raises(
+        ValueError,
+        match="The acceptable values for 'null_strategy' are 'impute' and 'drop'.",
+    ):
+        InvalidTargetDataCheck(
+            "regression",
+            get_default_primary_search_objective("regression"),
+            null_strategy=null_strategy,
+        )
+
+
 def test_invalid_target_data_check_nan_error():
     X = pd.DataFrame({"col": [1, 2, 3]})
     invalid_targets_check = InvalidTargetDataCheck(
         "regression",
         get_default_primary_search_objective("regression"),
     )
 
@@ -144,18 +157,68 @@
             data_check_name=invalid_targets_data_check_name,
             message_code=DataCheckMessageCode.TARGET_IS_NONE,
             details={},
         ).to_dict(),
     ]
 
 
+@pytest.mark.parametrize("null_strategy", ["Impute", "DROP"])
+def test_invalid_target_data_null_strategies(null_strategy):
+    invalid_targets_check = InvalidTargetDataCheck(
+        "regression",
+        get_default_primary_search_objective("regression"),
+        null_strategy=null_strategy,
+    )
+
+    expected_action_options = []
+    impute_action_option = DataCheckActionOption(
+        DataCheckActionCode.IMPUTE_COL,
+        data_check_name=invalid_targets_data_check_name,
+        parameters={
+            "impute_strategy": {
+                "parameter_type": DCAOParameterType.GLOBAL,
+                "type": "category",
+                "categories": ["mean", "most_frequent"],
+                "default_value": "mean",
+            },
+        },
+        metadata={"is_target": True},
+    )
+    drop_action_option = DataCheckActionOption(
+        DataCheckActionCode.DROP_ROWS,
+        data_check_name=invalid_targets_data_check_name,
+        metadata={"is_target": True, "rows": [0, 3]},
+    )
+    if null_strategy.lower() == "impute":
+        expected_action_options.append(impute_action_option)
+    elif null_strategy.lower() == "drop":
+        expected_action_options.append(drop_action_option)
+
+    expected = [
+        DataCheckError(
+            message="2 row(s) (40.0%) of target values are null",
+            data_check_name=invalid_targets_data_check_name,
+            message_code=DataCheckMessageCode.TARGET_HAS_NULL,
+            details={"num_null_rows": 2, "pct_null_rows": 40.0, "rows": [0, 3]},
+            action_options=expected_action_options,
+        ).to_dict(),
+    ]
+
+    y = pd.Series([None, 3.5, 2.8, None, 0])
+    X = pd.DataFrame({"col": range(len(y))})
+
+    messages = invalid_targets_check.validate(X, y)
+    assert messages == expected
+
+
 def test_invalid_target_data_input_formats():
     invalid_targets_check = InvalidTargetDataCheck(
         "binary",
         get_default_primary_search_objective("binary"),
+        null_strategy="impute",
     )
 
     # test empty pd.Series
     X = pd.DataFrame()
     messages = invalid_targets_check.validate(X, pd.Series())
     assert messages == [
         DataCheckError(
@@ -167,15 +230,15 @@
     ]
 
     expected = [
         DataCheckError(
             message="3 row(s) (75.0%) of target values are null",
             data_check_name=invalid_targets_data_check_name,
             message_code=DataCheckMessageCode.TARGET_HAS_NULL,
-            details={"num_null_rows": 3, "pct_null_rows": 75},
+            details={"num_null_rows": 3, "pct_null_rows": 75, "rows": [0, 1, 2]},
             action_options=[
                 DataCheckActionOption(
                     DataCheckActionCode.IMPUTE_COL,
                     data_check_name=invalid_targets_data_check_name,
                     parameters={
                         "impute_strategy": {
                             "parameter_type": DCAOParameterType.GLOBAL,
@@ -670,21 +733,22 @@
     if use_nullable_types:
         y = ww.init_series(y, logical_type="IntegerNullable")
 
     X = pd.DataFrame({"col": range(len(y))})
     invalid_targets_check = InvalidTargetDataCheck(
         problem_type,
         get_default_primary_search_objective(problem_type),
+        null_strategy="impute",
     )
     expected = [
         DataCheckError(
             message="3 row(s) (30.0%) of target values are null",
             data_check_name=invalid_targets_data_check_name,
             message_code=DataCheckMessageCode.TARGET_HAS_NULL,
-            details={"num_null_rows": 3, "pct_null_rows": 30.0},
+            details={"num_null_rows": 3, "pct_null_rows": 30.0, "rows": [0, 1, 2]},
             action_options=[
                 DataCheckActionOption(
                     DataCheckActionCode.IMPUTE_COL,
                     data_check_name=invalid_targets_data_check_name,
                     parameters={
                         "impute_strategy": {
                             "parameter_type": DCAOParameterType.GLOBAL,
```

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_null_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_outliers_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     target_dist_check = TargetDistributionDataCheck()
 
     if target_type in ["integer", "double"]:
         assert target_dist_check.validate(X, y) == []
     else:
         assert target_dist_check.validate(X, y) == [
             DataCheckError(
-                message=f"Target is unsupported {y.ww.logical_type.type_string} type. Valid Woodwork logical types include: integer, double",
+                message=f"Target is unsupported {y.ww.logical_type.type_string} type. Valid Woodwork logical types include: integer, double, age, age_fractional",
                 data_check_name=target_dist_check_name,
                 message_code=DataCheckMessageCode.TARGET_UNSUPPORTED_TYPE,
                 details={"unsupported_type": y.ww.logical_type.type_string},
             ).to_dict(),
         ]
```

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     X["a"] = y * 3
     X["b"] = y - 1
     X["c"] = y / 10
     X["d"] = y % 2
     X["e"] = [0] * 30
     X.ww.init(logical_types={"d": "Boolean"})
 
-    leakage_check = TargetLeakageDataCheck(pct_corr_threshold=0.5)
+    leakage_check = TargetLeakageDataCheck(method="mutual_info", pct_corr_threshold=0.5)
     assert leakage_check.validate(X, y) == [
         DataCheckWarning(
             message="Columns 'a', 'b', 'c' are 50.0% or more correlated with the target",
             data_check_name=target_leakage_data_check_name,
             message_code=DataCheckMessageCode.TARGET_LEAKAGE,
             details={"columns": ["a", "b", "c"]},
             action_options=[
@@ -78,15 +78,15 @@
 
 def test_target_leakage_data_check_singular_warning():
     y = pd.Series(range(30))
     X = pd.DataFrame()
     X["a"] = y * 3
     X["b"] = [0] * 30
 
-    leakage_check = TargetLeakageDataCheck(pct_corr_threshold=0.5)
+    leakage_check = TargetLeakageDataCheck(method="mutual_info", pct_corr_threshold=0.5)
     assert leakage_check.validate(X, y) == [
         DataCheckWarning(
             message="Column 'a' is 50.0% or more correlated with the target",
             data_check_name=target_leakage_data_check_name,
             message_code=DataCheckMessageCode.TARGET_LEAKAGE,
             details={"columns": ["a"]},
             action_options=[
@@ -447,15 +447,18 @@
     y_ww = ww.init_series(y)
     assert leakage_check.validate(X_ww, y_ww) == expected
 
     #  test y as list
     assert leakage_check.validate(X, y.values) == expected
 
 
-@pytest.mark.parametrize("measures", ["pearson", "spearman", "mutual_info", "max"])
+@pytest.mark.parametrize(
+    "measures",
+    ["pearson", "spearman", "mutual_info", "max", "all"],
+)
 def test_target_leakage_none_measures(measures):
     leakage_check = TargetLeakageDataCheck(pct_corr_threshold=0.5, method=measures)
     y = pd.Series([1, 0, 1, 1] * 6 + [1])
     X = pd.DataFrame()
     X["a"] = ["a", "b", "a", "a"] * 6 + ["a"]
     X["b"] = y
     y = y.astype(bool)
@@ -494,14 +497,42 @@
     y = pd.Series([1, 0, 1, 1] * 10)
     X = pd.DataFrame()
     X["target_y"] = y * 3
     X["target_y_y"] = y - 1
     X["target"] = y / 10
     X["d"] = ~y
     X["e"] = [0, 1, 2, 3] * 10
+    leakage_check = TargetLeakageDataCheck(method="mutual_info", pct_corr_threshold=0.8)
+
+    expected = [
+        DataCheckWarning(
+            message="Columns 'target_y', 'target_y_y', 'target', 'd' are 80.0% or more correlated with the target",
+            data_check_name=target_leakage_data_check_name,
+            message_code=DataCheckMessageCode.TARGET_LEAKAGE,
+            details={"columns": ["target_y", "target_y_y", "target", "d"]},
+            action_options=[
+                DataCheckActionOption(
+                    DataCheckActionCode.DROP_COL,
+                    data_check_name=target_leakage_data_check_name,
+                    metadata={"columns": ["target_y", "target_y_y", "target", "d"]},
+                ),
+            ],
+        ).to_dict(),
+    ]
+    assert leakage_check.validate(X, y) == expected
+
+
+def test_target_leakage_target_string_all():
+    y = pd.Series([1, 0, 1, 1] * 10)
+    X = pd.DataFrame()
+    X["target_y"] = y * 3
+    X["target_y_y"] = y - 1
+    X["target"] = y / 10
+    X["d"] = ~y
+    X["e"] = [0, 1, 2, 3] * 10
     leakage_check = TargetLeakageDataCheck(pct_corr_threshold=0.8)
 
     expected = [
         DataCheckWarning(
             message="Columns 'target_y', 'target_y_y', 'target', 'd' are 80.0% or more correlated with the target",
             data_check_name=target_leakage_data_check_name,
             message_code=DataCheckMessageCode.TARGET_LEAKAGE,
@@ -514,10 +545,18 @@
                 ),
             ],
         ).to_dict(),
     ]
     assert leakage_check.validate(X, y) == expected
 
 
-def test_target_leakage_use_all():
-    with pytest.raises(ValueError, match="Cannot use 'all' as the method"):
-        TargetLeakageDataCheck(method="all")
+def test_target_leakage_target_all_matches_max():
+    y = pd.Series([1, 0, 1, 1] * 10)
+    X = pd.DataFrame()
+    X["target_y"] = y * 3
+    X["target_y_y"] = y - 1
+    X["target"] = y / 10
+    X["d"] = ~y
+    X["e"] = [0, 1, 2, 3] * 10
+    leakage_check_all = TargetLeakageDataCheck(pct_corr_threshold=0.8, method="all")
+    leakage_check_max = TargetLeakageDataCheck(pct_corr_threshold=0.8, method="max")
+    assert leakage_check_all.validate(X, y) == leakage_check_max.validate(X, y)
```

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/data_checks_tests/test_utils.py` & `evalml-0.73.0/evalml/tests/data_checks_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/demo_tests/test_datasets.py` & `evalml-0.73.0/evalml/tests/demo_tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt` & `evalml-0.73.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-black==23.1.0
+black==23.3.0
 catboost==1.1.1
 category-encoders==2.5.1.post0
 click==8.1.3
 cloudpickle==2.2.1
 colorama==0.4.6
 dask==2023.3.2
-featuretools==1.23.0
+featuretools==1.24.0
 graphviz==0.20.1
 holidays==0.20
 imbalanced-learn==0.10.1
 ipywidgets==8.0.4
 kaleido==0.2.1
 lightgbm==3.3.5
 lime==0.2.0.1
 matplotlib==3.7.1
 matplotlib-inline==0.1.6
-networkx==3.0
+networkx==3.1
 nlp-primitives==2.10.0
 numpy==1.23.5
 packaging==23.0
 pandas==1.5.3
-plotly==5.13.1
+plotly==5.14.1
 pmdarima==2.0.3
 pyzmq==25.0.2
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
 scipy==1.9.1
 seaborn==0.12.2
 shap==0.41.0
-sktime==0.16.1
+sktime==0.17.0
 statsmodels==0.13.5
 texttable==1.6.7
 tomli==2.0.1
 vowpalwabbit==9.8.0
 woodwork==0.22.0
-xgboost==1.7.4
+xgboost==1.7.5
```

### Comparing `evalml-0.72.0/evalml/tests/dependency_update_check/minimum_requirements.txt` & `evalml-0.73.0/evalml/tests/dependency_update_check/minimum_requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 pmdarima==1.8.5
 pyzmq==20.0.0
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
 scipy==1.5.0
 seaborn==0.11.1
 shap==0.40.0
-sktime==0.15.0
+sktime==0.17.0
 statsmodels==0.12.2
 texttable==1.6.2
 tomli==2.0.1
 vowpalwabbit==8.11.0
 woodwork==0.22.0
 xgboost==1.7.0
```

### Comparing `evalml-0.72.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt` & `evalml-0.73.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,14 @@
 pytest==7.1.2
 pyzmq==20.0.0
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
 scipy==1.5.0
 seaborn==0.11.1
 shap==0.40.0
-sktime==0.15.0
+sktime==0.17.0
 statsmodels==0.12.2
 texttable==1.6.2
 tomli==2.0.1
 vowpalwabbit==8.11.0
 woodwork==0.22.0
 xgboost==1.7.0
```

### Comparing `evalml-0.72.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py` & `evalml-0.73.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from evalml.data_checks.null_data_check import NullDataCheck
 from evalml.pipelines import (
     BinaryClassificationPipeline,
     TimeSeriesImputer,
     TimeSeriesRegressionPipeline,
     TimeSeriesRegularizer,
 )
-from evalml.pipelines.components import DropColumns, DropRowsTransformer, TargetImputer
+from evalml.pipelines.components import (
+    DropColumns,
+    DropRowsTransformer,
+    TargetImputer,
+)
 from evalml.pipelines.components.transformers.imputers.per_column_imputer import (
     PerColumnImputer,
 )
 from evalml.pipelines.multiclass_classification_pipeline import (
     MulticlassClassificationPipeline,
 )
 from evalml.pipelines.regression_pipeline import RegressionPipeline
@@ -214,35 +218,35 @@
     X = pd.DataFrame()
     if problem_type == "binary":
         y = ww.init_series(pd.Series([0, 1, 1, None, None]))
         objective = "Log Loss Binary"
         expected_pipeline_class = BinaryClassificationPipeline
         y_expected = ww.init_series(
             pd.Series([0, 1, 1, 1, 1]),
-            logical_type="Integer",
+            logical_type="IntegerNullable",
         )
 
     elif problem_type == "multiclass":
         y = ww.init_series(pd.Series([0, 1, 2, 2, None]))
         objective = "Log Loss Multiclass"
         expected_pipeline_class = MulticlassClassificationPipeline
         y_expected = ww.init_series(
             pd.Series([0, 1, 2, 2, 2]),
-            logical_type="Integer",
+            logical_type="IntegerNullable",
         )
 
     else:
         y = ww.init_series(pd.Series([0, 0.1, 0.2, None, None]))
         objective = "R2"
         expected_pipeline_class = RegressionPipeline
         y_expected = ww.init_series(
             pd.Series([0, 0.1, 0.2, 0.1, 0.1]),
             logical_type="double",
         )
-    data_check = InvalidTargetDataCheck(problem_type, objective)
+    data_check = InvalidTargetDataCheck(problem_type, objective, null_strategy="impute")
     data_checks_output = data_check.validate(None, y)
 
     action_pipeline = make_pipeline_from_data_check_output(
         problem_type,
         data_checks_output,
     )
     expected_parameters = (
@@ -289,7 +293,28 @@
     X_expected.ww.init()
     y_expected = y.drop([0, 3, 5, 10])
 
     action_pipeline.fit(X, y)
     X_t, y_t = action_pipeline.transform(X, y)
     assert_frame_equal(X_expected, X_t)
     assert_series_equal(y_expected, y_t)
+
+    y = pd.Series(np.concatenate([np.tile([0, 1], 49), [np.nan, np.nan]]))
+
+    data_check = InvalidTargetDataCheck("binary", "Log Loss Binary")
+    data_checks_output = data_check.validate(None, y)
+
+    action_pipeline = make_pipeline_from_data_check_output("binary", data_checks_output)
+    assert action_pipeline == BinaryClassificationPipeline(
+        component_graph={"Drop Rows Transformer": [DropRowsTransformer, "X", "y"]},
+        parameters={"Drop Rows Transformer": {"indices_to_drop": [98, 99]}},
+        random_seed=0,
+    )
+
+    X_expected = X.drop([98, 99])
+    X_expected.ww.init()
+    y_expected = y.drop([98, 99]).astype("Int64")
+
+    action_pipeline.fit(X, y)
+    X_t, y_t = action_pipeline.transform(X, y)
+    assert_frame_equal(X_expected, X_t)
+    assert_series_equal(y_expected, y_t)
```

### Comparing `evalml-0.72.0/evalml/tests/integration_tests/test_time_series_integration.py` & `evalml-0.73.0/evalml/tests/integration_tests/test_time_series_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_family_tests/test_model_family.py` & `evalml-0.73.0/evalml/tests/model_family_tests/test_model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/test_decision_boundary.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/test_decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/test_feature_explanations.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/test_feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/test_metrics.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/test_partial_dependence.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/test_partial_dependence.py`

 * *Files 0% similar despite different names*

```diff
@@ -3018,22 +3018,27 @@
     "grid_resolution",
     [2, 10, 50],
 )
 @pytest.mark.parametrize(
     "use_int_null_many_values",
     [True, False],
 )
+@pytest.mark.parametrize(
+    "X_has_nans",
+    [True, False],
+)
 def test_partial_dependence_with_nullable_types(
     nullable_type_test_data,
     nullable_type_target,
     linear_regression_pipeline,
     logistic_regression_binary_pipeline,
     nullable_y_ltype,
     grid_resolution,
     use_int_null_many_values,
+    X_has_nans,
 ):
     y = nullable_type_target(ltype=nullable_y_ltype, has_nans=False)
     X = nullable_type_test_data(has_nans=False)
     X = X.ww.select(["numeric", "Boolean", "BooleanNullable"])
 
     int_col = "int col nullable"
     if use_int_null_many_values:
```

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/test_permutation_importance.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/model_understanding_tests/test_visualizations.py` & `evalml-0.73.0/evalml/tests/model_understanding_tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/objective_tests/test_binary_classification_objective.py` & `evalml-0.73.0/evalml/tests/objective_tests/test_binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py` & `evalml-0.73.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/objective_tests/test_fraud_detection.py` & `evalml-0.73.0/evalml/tests/objective_tests/test_fraud_detection.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/objective_tests/test_lead_scoring.py` & `evalml-0.73.0/evalml/tests/objective_tests/test_lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/objective_tests/test_objectives.py` & `evalml-0.73.0/evalml/tests/objective_tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/objective_tests/test_sla.py` & `evalml-0.73.0/evalml/tests/objective_tests/test_sla.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/objective_tests/test_standard_metrics.py` & `evalml-0.73.0/evalml/tests/objective_tests/test_standard_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/test_component_graph.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/test_component_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 from unittest.mock import patch
 
 import featuretools as ft
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.testing import assert_frame_equal, assert_index_equal, assert_series_equal
-from woodwork.logical_types import Boolean, Categorical, Double, EmailAddress, Integer
+from woodwork.logical_types import (
+    Boolean,
+    BooleanNullable,
+    Categorical,
+    Double,
+    EmailAddress,
+    Integer,
+)
 
 from evalml.demos import load_diabetes
 from evalml.exceptions import (
     MethodPropertyNotFoundError,
     MissingComponentError,
     ParameterNotUsedWarning,
     PipelineError,
@@ -2673,23 +2680,23 @@
     )
     graph1.instantiate()
     graph1.fit(X, y)
     assert graph1.get_component_input_logical_types("OHE") == {
         "numeric": Integer(),
         "cat": Categorical(),
         "EMAIL_ADDRESS_TO_DOMAIN(email)": Categorical(),
-        "IS_FREE_EMAIL_DOMAIN(email)": Categorical(),
+        "IS_FREE_EMAIL_DOMAIN(email)": BooleanNullable(),
     }
     assert graph1.last_component_input_logical_types == {
         "numeric": Integer(),
         "cat_a": Boolean(),
         "cat_b": Boolean(),
         "cat_c": Boolean(),
         "EMAIL_ADDRESS_TO_DOMAIN(email)_gmail.com": Boolean(),
-        "IS_FREE_EMAIL_DOMAIN(email)_1.0": Boolean(),
+        "IS_FREE_EMAIL_DOMAIN(email)": BooleanNullable(),
     }
 
     ensemble = ComponentGraph(
         component_dict={
             "Email": ["Email Featurizer", "X", "y"],
             "OHE": ["One Hot Encoder", "Email.x", "y"],
             "RF": [
@@ -2713,15 +2720,15 @@
         "Catboost.x": Double(),
         "RF.x": Double(),
     }
     assert ensemble.get_component_input_logical_types("Catboost") == {
         "cat": Categorical(),
         "numeric": Integer(),
         "EMAIL_ADDRESS_TO_DOMAIN(email)": Categorical(),
-        "IS_FREE_EMAIL_DOMAIN(email)": Categorical(),
+        "IS_FREE_EMAIL_DOMAIN(email)": BooleanNullable(),
     }
 
     no_estimator = ComponentGraph(
         {
             "Imputer": ["Imputer", "X", "y"],
             "OHE": ["One Hot Encoder", "Imputer.x", "y"],
         },
@@ -2735,10 +2742,10 @@
 
     with pytest.raises(ValueError, match="not in the graph"):
         _ = no_estimator.get_component_input_logical_types("Catboost")
 
     no_estimator.fit(X, y)
     assert no_estimator.last_component_input_logical_types == {
         "cat": Categorical(),
-        "numeric": Double(),
+        "numeric": Integer(),
         "email": EmailAddress(),
     }
```

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/test_graphs.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/test_pipeline_utils.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/test_pipeline_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     EmailFeaturizer,
     Estimator,
     Imputer,
     LinearRegressor,
     LogisticRegressionClassifier,
     NaturalLanguageFeaturizer,
     OneHotEncoder,
-    ReplaceNullableTypes,
     StackedEnsembleBase,
     StandardScaler,
     STLDecomposer,
     TargetImputer,
     TimeSeriesFeaturizer,
     Transformer,
     URLFeaturizer,
@@ -124,15 +123,15 @@
             assert isinstance(pipeline, pipeline_class)
             label_encoder = [LabelEncoder] if is_classification(problem_type) else []
             delayed_features = (
                 [TimeSeriesFeaturizer] if is_time_series(problem_type) else []
             )
 
             if estimator_class.model_family != ModelFamily.CATBOOST and any(
-                column_name in ["url", "email", "categorical", "bool_null"]
+                column_name in ["url", "email", "categorical"]
                 for column_name in column_names
             ):
                 ohe = [OneHotEncoder]
             else:
                 ohe = []
             dfs = [DFSTransformer] if features else []
             decomposer = [STLDecomposer] if is_regression(problem_type) else []
@@ -145,17 +144,14 @@
             )
             standard_scaler = (
                 [StandardScaler]
                 if estimator_class.model_family == ModelFamily.LINEAR_MODEL
                 else []
             )
             drop_null = [DropColumns] if "all_null" in column_names else []
-            replace_null = (
-                [] if (column_names in [["email"], ["url"]]) else [ReplaceNullableTypes]
-            )
             natural_language_featurizer = (
                 [NaturalLanguageFeaturizer] if "text" in column_names else []
             )
             email_featurizer = [EmailFeaturizer] if "email" in column_names else []
             url_featurizer = [URLFeaturizer] if "url" in column_names else []
             imputer = [] if (column_names in [["ip"], ["all_null"]]) else [Imputer]
             drop_nan_rows_transformer = (
@@ -165,15 +161,14 @@
                 else []
             )
 
             if is_time_series(problem_type):
                 expected_components = (
                     dfs
                     + label_encoder
-                    + replace_null
                     + email_featurizer
                     + url_featurizer
                     + drop_null
                     + natural_language_featurizer
                     + imputer
                     + delayed_features
                     + decomposer
@@ -183,15 +178,14 @@
                     + standard_scaler
                     + [estimator_class]
                 )
             else:
                 expected_components = (
                     dfs
                     + label_encoder
-                    + replace_null
                     + email_featurizer
                     + url_featurizer
                     + drop_null
                     + delayed_features
                     + datetime
                     + natural_language_featurizer
                     + imputer
@@ -1299,15 +1293,17 @@
     input_pipelines = [pipeline_1, pipeline_2]
 
     combined_pipeline = _make_pipeline_from_multiple_graphs(
         input_pipelines=input_pipelines,
         estimator=estimator,
         problem_type=ProblemTypes.BINARY,
     )
-    second_pipeline_sampler = "Pipeline w/ Label Encoder + Replace Nullable Types Transformer + Imputer + Undersampler Pipeline 2 - Undersampler.y"
+    second_pipeline_sampler = (
+        "Pipeline w/ Label Encoder + Imputer + Undersampler Pipeline 2 - Undersampler.y"
+    )
     assert (
         combined_pipeline.component_graph.get_inputs("Random Forest Classifier")[2]
         == second_pipeline_sampler
     )
 
 
 def test_make_pipeline_from_multiple_graphs_pre_pipeline_components(X_y_binary):
@@ -1341,22 +1337,21 @@
     combined_pipeline = _make_pipeline_from_multiple_graphs(
         input_pipelines=input_pipelines,
         estimator=estimator,
         problem_type=ProblemTypes.BINARY,
         pre_pipeline_components=pre_pipeline_components,
         sub_pipeline_names=sub_pipeline_names,
     )
-
     assert (
         combined_pipeline.component_graph.get_inputs("First Pipeline - Imputer")[0]
-        == "First Pipeline - Replace Nullable Types Transformer.x"
+        == "DFS Transformer.x"
     )
     assert (
         combined_pipeline.component_graph.get_inputs("Second Pipeline - Imputer")[0]
-        == "Second Pipeline - Replace Nullable Types Transformer.x"
+        == "DFS Transformer.x"
     )
 
 
 def test_make_pipeline_features_and_dfs(X_y_binary):
     X, y = X_y_binary
     estimator = handle_component_class("Random Forest Classifier")
     features = True
```

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/test_pipelines.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py` & `evalml-0.73.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from unittest.mock import patch
 
+import featuretools as ft
 import numpy as np
 import pandas as pd
 import pytest
 import woodwork as ww
 from pandas.testing import assert_frame_equal, assert_series_equal
 
 from evalml.exceptions import PipelineNotYetFittedError
@@ -1864,72 +1865,135 @@
             prediction_start,
             prediction_end,
         )
 
 
 @pytest.mark.parametrize("set_coverage", [True, False])
 @pytest.mark.parametrize("add_decomposer", [True, False])
-@pytest.mark.parametrize("no_preds_pi_estimator", [True, False])
+@pytest.mark.parametrize("ts_native_estimator", [True, False])
+@pytest.mark.parametrize("featuretools_first", [True, False])
 def test_time_series_pipeline_get_prediction_intervals(
-    no_preds_pi_estimator,
+    featuretools_first,
+    ts_native_estimator,
     add_decomposer,
     set_coverage,
     ts_data_long,
+    ts_data_quadratic_trend,
 ):
-    X, _, y = ts_data_long
-    component_graph = {
-        "Time Series Featurizer": ["Time Series Featurizer", "X", "y"],
-        "DateTime Featurizer": ["DateTime Featurizer", "Time Series Featurizer.x", "y"],
-        "Drop NaN Rows Transformer": [
-            "Drop NaN Rows Transformer",
-            "DateTime Featurizer.x",
-            "y",
-        ],
-        "Regressor": [
-            "Exponential Smoothing Regressor"
-            if no_preds_pi_estimator
-            else "Linear Regressor",
-            "Drop NaN Rows Transformer.x",
-            "Drop NaN Rows Transformer.y",
-        ],
+    X, y = ts_data_quadratic_trend
+
+    # Test the case where we featurize via featuretools instead of our
+    # native transformers
+    if featuretools_first:
+        component_graph = {
+            "DFS Transformer": ["DFS Transformer", "X", "y"],
+            "Drop NaN Rows Transformer": [
+                "Drop NaN Rows Transformer",
+                "DFS Transformer.x",
+                "y",
+            ],
+            "Regressor": [
+                "Exponential Smoothing Regressor"
+                if ts_native_estimator
+                else "Linear Regressor",
+                "Drop NaN Rows Transformer.x",
+                "Drop NaN Rows Transformer.y",
+            ],
+        }
+        if add_decomposer:
+            component_graph.update(
+                {
+                    "STL Decomposer": [
+                        "STL Decomposer",
+                        "DFS Transformer.x",
+                        "y",
+                    ],
+                    "Drop NaN Rows Transformer": [
+                        "Drop NaN Rows Transformer",
+                        "STL Decomposer.x",
+                        "STL Decomposer.y",
+                    ],
+                },
+            )
+    else:
+        component_graph = {
+            "Time Series Featurizer": ["Time Series Featurizer", "X", "y"],
+            "DateTime Featurizer": [
+                "DateTime Featurizer",
+                "Time Series Featurizer.x",
+                "y",
+            ],
+            "Drop NaN Rows Transformer": [
+                "Drop NaN Rows Transformer",
+                "DateTime Featurizer.x",
+                "y",
+            ],
+            "Regressor": [
+                "Exponential Smoothing Regressor"
+                if ts_native_estimator
+                else "Linear Regressor",
+                "Drop NaN Rows Transformer.x",
+                "Drop NaN Rows Transformer.y",
+            ],
+        }
+        if add_decomposer:
+            component_graph.update(
+                {
+                    "STL Decomposer": [
+                        "STL Decomposer",
+                        "Time Series Featurizer.x",
+                        "y",
+                    ],
+                    "DateTime Featurizer": [
+                        "DateTime Featurizer",
+                        "STL Decomposer.x",
+                        "STL Decomposer.y",
+                    ],
+                    "Drop NaN Rows Transformer": [
+                        "Drop NaN Rows Transformer",
+                        "DateTime Featurizer.x",
+                        "STL Decomposer.y",
+                    ],
+                },
+            )
+
+    pipeline_parameters = {
+        "pipeline": {
+            "gap": 1,
+            "max_delay": 10,
+            "time_index": "date",
+            "forecast_horizon": 7,
+            "random_seed": 0,
+        },
+        "Time Series Featurizer": {
+            "max_delay": 2,
+            "gap": 1,
+            "forecast_horizon": 10,
+            "time_index": "date",
+        },
     }
-    if add_decomposer:
-        component_graph.update(
-            {
-                "STL Decomposer": ["STL Decomposer", "Time Series Featurizer.x", "y"],
-                "DateTime Featurizer": [
-                    "DateTime Featurizer",
-                    "STL Decomposer.x",
-                    "STL Decomposer.y",
-                ],
-                "Drop NaN Rows Transformer": [
-                    "Drop NaN Rows Transformer",
-                    "DateTime Featurizer.x",
-                    "STL Decomposer.y",
-                ],
-            },
+    if featuretools_first:
+        es = ft.EntitySet()
+        es.add_dataframe(
+            dataframe_name="X",
+            dataframe=X.copy(),
+            index="id",
+            make_index=True,
+        )
+        features = ft.dfs(
+            entityset=es,
+            target_dataframe_name="X",
+            max_depth=1,
+            features_only=True,
         )
+        pipeline_parameters["DFS Transformer"] = {"features": features}
 
     pipeline = TimeSeriesRegressionPipeline(
         component_graph=component_graph,
-        parameters={
-            "pipeline": {
-                "gap": 1,
-                "max_delay": 10,
-                "time_index": "date",
-                "forecast_horizon": 7,
-                "random_seed": 0,
-            },
-            "Time Series Featurizer": {
-                "max_delay": 2,
-                "gap": 1,
-                "forecast_horizon": 10,
-                "time_index": "date",
-            },
-        },
+        parameters=pipeline_parameters,
     )
     limit = int(np.floor(0.66 * len(X)))
     X_train, y_train = X[:limit], y[:limit]
     X_validation, y_validation = X[limit + 1 :], y[limit + 1 :]
     pipeline.fit(X_train, y_train)
 
     coverage = [0.75, 0.85, 0.95] if set_coverage else None
@@ -1938,49 +2002,84 @@
         X=X_validation,
         y=y_validation,
         X_train=X_train,
         y_train=y_train,
         coverage=coverage,
     )
 
-    predictions = pipeline.predict_in_sample(
-        X_validation,
-        y_validation,
-        X_train,
-        y_train,
-    )
-    features = pipeline.transform_all_but_final(
-        X_validation,
-        y_validation,
-        X_train,
-        y_train,
-    )
-    est_intervals = pipeline.estimator.get_prediction_intervals(
-        X=features,
-        y=y_validation,
-        predictions=predictions,
-        coverage=coverage,
-    )
+    if set_coverage is False:
+        coverage = [0.95]
+
+    # The time series native estimators are handled separately when they have
+    # a decomposer in the pipeline
+    if ts_native_estimator and add_decomposer:
+        predictions = pipeline.predict_in_sample(
+            X_validation,
+            y_validation,
+            X_train,
+            y_train,
+        )
+        X_validation, y_validation = pipeline._drop_time_index(
+            X_validation,
+            y_validation,
+        )
+        features = pipeline.transform_all_but_final(
+            X_validation,
+            y_validation,
+            X_train,
+            y_train,
+        )
+        est_intervals = pipeline.estimator.get_prediction_intervals(
+            X=features,
+            y=y_validation,
+            predictions=predictions,
+            coverage=coverage,
+        )
 
-    if no_preds_pi_estimator and add_decomposer:
         trend_pred_intervals = pipeline.get_component(
             "STL Decomposer",
         ).get_trend_prediction_intervals(y_validation, coverage=coverage)
         residuals = pipeline.estimator.predict(features)
 
-    if set_coverage is False:
-        coverage = [0.95]
-
-    for cover_value in coverage:
-        for key in [f"{cover_value}_lower", f"{cover_value}_upper"]:
-            pl_interval = pl_intervals[key]
-            if no_preds_pi_estimator and add_decomposer:
+        for cover_value in coverage:
+            for key in [f"{cover_value}_lower", f"{cover_value}_upper"]:
+                pl_interval = pl_intervals[key]
                 residual_pi = est_intervals[key] - residuals
                 expected_res = pd.Series(
                     residual_pi.values
                     + trend_pred_intervals[key].values
                     + y_validation.values,
                     index=est_intervals[key].index,
                 )
                 assert_series_equal(expected_res, pl_interval)
-            else:
-                assert_series_equal(est_intervals[key], pl_interval)
+
+    if set_coverage:
+        pairs = [(0.75, 0.85), (0.85, 0.95)]
+        for pair in pairs:
+            assert all(
+                [
+                    narrower >= broader
+                    for narrower, broader in zip(
+                        pl_intervals[f"{pair[0]}_lower"],
+                        pl_intervals[f"{pair[1]}_lower"],
+                    )
+                ],
+            )
+            assert all(
+                [
+                    narrower <= broader
+                    for narrower, broader in zip(
+                        pl_intervals[f"{pair[0]}_upper"],
+                        pl_intervals[f"{pair[1]}_upper"],
+                    )
+                ],
+            )
+    for cover_value in coverage:
+        assert all(
+            [
+                lower < upper
+                for lower, upper in zip(
+                    pl_intervals[f"{cover_value}_lower"],
+                    pl_intervals[f"{cover_value}_upper"],
+                )
+            ],
+        )
```

### Comparing `evalml-0.72.0/evalml/tests/preprocessing_tests/test_no_split.py` & `evalml-0.73.0/evalml/tests/preprocessing_tests/test_no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/preprocessing_tests/test_sk_splitters.py` & `evalml-0.73.0/evalml/tests/preprocessing_tests/test_sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/preprocessing_tests/test_split_data.py` & `evalml-0.73.0/evalml/tests/preprocessing_tests/test_split_data.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/preprocessing_tests/test_training_validation_split.py` & `evalml-0.73.0/evalml/tests/preprocessing_tests/test_training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/problem_type_tests/test_problem_types.py` & `evalml-0.73.0/evalml/tests/problem_type_tests/test_problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/test_all_test_dirs_included.py` & `evalml-0.73.0/evalml/tests/test_all_test_dirs_included.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/tuner_tests/test_grid_search_tuner.py` & `evalml-0.73.0/evalml/tests/tuner_tests/test_grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/tuner_tests/test_random_search_tuner.py` & `evalml-0.73.0/evalml/tests/tuner_tests/test_random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/tuner_tests/test_skopt_tuner.py` & `evalml-0.73.0/evalml/tests/tuner_tests/test_skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/utils_tests/test_cli_utils.py` & `evalml-0.73.0/evalml/tests/utils_tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/utils_tests/test_gen_utils.py` & `evalml-0.73.0/evalml/tests/utils_tests/test_gen_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     contains_all_ts_parameters,
     convert_to_seconds,
     deprecate_arg,
     get_importable_subclasses,
     get_random_seed,
     get_time_index,
     import_or_raise,
-    is_categorical_actually_boolean,
     jupyter_check,
     pad_with_nans,
     save_plot,
     validate_holdout_datasets,
 )
 
 
@@ -874,28 +873,14 @@
     assert are_datasets_separated_by_gap_time_index(
         train,
         test,
         {"time_index": "time_index", "gap": 2},
     )
 
 
-def test_is_categorical_actually_boolean():
-    X = pd.DataFrame(
-        {
-            "categorical": ["a", "b", "c"],
-            "boolean_categorical": [True, False, None],
-            "boolean": [True, False, True],
-        },
-    )
-
-    assert not is_categorical_actually_boolean(X, "categorical")
-    assert is_categorical_actually_boolean(X, "boolean_categorical")
-    assert not is_categorical_actually_boolean(X, "boolean")
-
-
 @pytest.mark.parametrize("X_num_time_columns", [0, 1, 2, 3])
 @pytest.mark.parametrize(
     "X_has_time_index",
     ["X_has_time_index", "X_doesnt_have_time_index"],
 )
 @pytest.mark.parametrize(
     "y_has_time_index",
```

### Comparing `evalml-0.72.0/evalml/tests/utils_tests/test_logger.py` & `evalml-0.73.0/evalml/tests/utils_tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tests/utils_tests/test_nullable_type_utils.py` & `evalml-0.73.0/evalml/tests/utils_tests/test_nullable_type_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
-from woodwork.logical_types import AgeNullable, BooleanNullable, IntegerNullable
+from woodwork.logical_types import (
+    AgeNullable,
+    BooleanNullable,
+    IntegerNullable,
+)
 
 from evalml.utils import (
     _determine_downcast_type,
     _downcast_nullable_X,
     _downcast_nullable_y,
     _get_incompatible_nullable_types,
 )
```

### Comparing `evalml-0.72.0/evalml/tests/utils_tests/test_woodwork_utils.py` & `evalml-0.73.0/evalml/tests/utils_tests/test_woodwork_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     IntegerNullable,
     Unknown,
 )
 
 from evalml.utils import (
     _convert_numeric_dataset_pandas,
     _schema_is_equal,
-    downcast_int_nullable_to_double,
     downcast_nullable_types,
     infer_feature_types,
 )
 
 
 def test_infer_feature_types_no_type_change():
     X_dt = pd.DataFrame([[1, 2], [3, 4]])
@@ -376,29 +375,7 @@
 
     df.ww.init(logical_types=forced_ltypes)
 
     df_dc = downcast_nullable_types(df, ignore_null_cols=ignore_null_cols)
 
     for col, ltype in df_dc.ww.logical_types.items():
         assert str(ltype) == str(expected_ltypes[col])
-
-
-def test_downcast_int_nullable_to_double():
-    df = pd.DataFrame()
-    df["ints"] = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 5
-    df["ints_nullable"] = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 5
-    df["ints_nullable_with_nulls"] = [1, 2, 3, 4, 5, 6, 7, 8, 9, pd.NA] * 5
-
-    expected_ltypes = {
-        "ints": Integer,
-        "ints_nullable": Double,
-        "ints_nullable_with_nulls": Double,
-    }
-
-    forced_ltypes = {
-        "ints_nullable": IntegerNullable,
-    }
-    df.ww.init(logical_types=forced_ltypes)
-    df_dc = downcast_int_nullable_to_double(df)
-
-    for col, ltype in df_dc.ww.logical_types.items():
-        assert str(ltype) == str(expected_ltypes[col])
```

### Comparing `evalml-0.72.0/evalml/tuners/grid_search_tuner.py` & `evalml-0.73.0/evalml/tuners/grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tuners/random_search_tuner.py` & `evalml-0.73.0/evalml/tuners/random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tuners/skopt_tuner.py` & `evalml-0.73.0/evalml/tuners/skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/tuners/tuner.py` & `evalml-0.73.0/evalml/tuners/tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/utils/__init__.py` & `evalml-0.73.0/evalml/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     print_sys_info,
     standardize_format,
 )
 from evalml.utils.woodwork_utils import (
     infer_feature_types,
     _convert_numeric_dataset_pandas,
     _schema_is_equal,
-    downcast_int_nullable_to_double,
     downcast_nullable_types,
 )
 from evalml.utils.nullable_type_utils import (
     _downcast_nullable_X,
     _downcast_nullable_y,
     _determine_downcast_type,
     _get_incompatible_nullable_types,
```

### Comparing `evalml-0.72.0/evalml/utils/base_meta.py` & `evalml-0.73.0/evalml/utils/base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/utils/cli_utils.py` & `evalml-0.73.0/evalml/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/utils/gen_utils.py` & `evalml-0.73.0/evalml/utils/gen_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,34 +45,14 @@
         msg = f"An exception occurred while trying to import `{library}`: {str(ex)}"
         if warning:
             warnings.warn(msg)
         else:
             raise Exception(msg)
 
 
-def is_categorical_actually_boolean(df, df_col):
-    """Function to identify columns of a dataframe that contain True, False and null type.
-
-    The function is intended to be applied to columns that are identified as Categorical
-    by the Imputer/SimpleImputer.
-
-    Args:
-        df (pandas.DataFrame): Pandas dataframe with data.
-        df_col (str): The column to identify as basically a nullable Boolean.
-
-    Returns:
-        bool: Whether the column contains True, False and a null type.
-
-    """
-    unique_vals = df[df_col].unique()
-    return {True, False}.issubset(set(unique_vals)) and any(
-        isinstance(x, bool) for x in unique_vals
-    )
-
-
 def convert_to_seconds(input_str):
     """Converts a string describing a length of time to its length in seconds.
 
     Args:
         input_str (str): The string to be parsed and converted to seconds.
 
     Returns:
```

### Comparing `evalml-0.72.0/evalml/utils/logger.py` & `evalml-0.73.0/evalml/utils/logger.py`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml/utils/woodwork_utils.py` & `evalml-0.73.0/evalml/utils/woodwork_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from evalml.utils.gen_utils import is_all_numeric
 
 numeric_and_boolean_ww = [
     ww.logical_types.Integer.type_string,
     ww.logical_types.Double.type_string,
     ww.logical_types.Boolean.type_string,
+    ww.logical_types.Age.type_string,
+    ww.logical_types.AgeFractional.type_string,
     ww.logical_types.IntegerNullable.type_string,
     ww.logical_types.BooleanNullable.type_string,
     ww.logical_types.AgeNullable.type_string,
 ]
 
 
 def _numpy_to_pandas(array):
@@ -156,26 +158,7 @@
     new_ltypes.update(
         {col: "Double" for col in int_nullable_cols if col in non_null_columns},
     )
 
     if new_ltypes:
         data.ww.set_types(logical_types=new_ltypes)
     return data
-
-
-def downcast_int_nullable_to_double(X):
-    """Downcasts IntegerNullable type to Double in order to support certain estimators like ARIMA, CatBoost, and LightGBM.
-
-    Args:
-        X (pd.DataFrame): Feature data.
-
-    Returns:
-        X: DataFrame initialized with logical type information where IntegerNullable are cast as Double.
-    """
-    if X.ww.schema is None:
-        X.ww.init()
-
-    X_int_nullable_cols = X.ww.select(["IntegerNullable", "AgeNullable"])
-    new_ltypes = {col: "Double" for col in X_int_nullable_cols}
-    if new_ltypes:
-        X.ww.set_types(logical_types=new_ltypes)
-    return X
```

### Comparing `evalml-0.72.0/evalml.egg-info/PKG-INFO` & `evalml-0.73.0/evalml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.72.0
+Version: 0.73.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.72.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.73.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.72.0/evalml.egg-info/SOURCES.txt` & `evalml-0.73.0/evalml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.72.0/evalml.egg-info/requires.txt` & `evalml-0.73.0/evalml.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 catboost>=1.1.1
 lightgbm>=2.3.1
 matplotlib>=3.3.3
 seaborn>=0.11.1
 category-encoders<=2.5.1.post0,>=2.2.2
 imbalanced-learn>=0.9.1
 pmdarima>=1.8.5
-sktime>=0.15.0
+sktime==0.17.0
 lime>=0.2.0.1
 vowpalwabbit>=8.11.0
 tomli>=2.0.1
 packaging>=23.0
 black[jupyter]>=22.3.0
 holidays<0.21,>=0.13
```

### Comparing `evalml-0.72.0/pyproject.toml` & `evalml-0.73.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     "lightgbm >= 2.3.1",
     "matplotlib >= 3.3.3",
     "graphviz >= 0.13; platform_system!='Windows'",
     "seaborn >= 0.11.1",
     "category-encoders >= 2.2.2, <= 2.5.1.post0",
     "imbalanced-learn >= 0.9.1",
     "pmdarima >= 1.8.5",
-    "sktime >= 0.15.0",
+    "sktime == 0.17.0",
     "lime >= 0.2.0.1",
     "vowpalwabbit >= 8.11.0",
     "tomli >= 2.0.1",
     "packaging >= 23.0",
     "black[jupyter] >= 22.3.0",
     "holidays >= 0.13, < 0.21"
 ]
```

