# Comparing `tmp/alphastats-0.4.4.tar.gz` & `tmp/alphastats-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphastats-0.4.4.tar", last modified: Wed Mar 15 06:48:23 2023, max compression
+gzip compressed data, was "alphastats-0.5.0.tar", last modified: Tue Apr 11 14:29:27 2023, max compression
```

## Comparing `alphastats-0.4.4.tar` & `alphastats-0.5.0.tar`

### file list

```diff
@@ -1,69 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.962519 alphastats-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-03-15 06:47:52.000000 alphastats-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-15 06:47:52.000000 alphastats-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-15 06:48:23.962519 alphastats-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-03-15 06:47:52.000000 alphastats-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.942519 alphastats-0.4.4/alphastats/
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/DataSet_Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/DataSet_Preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/DataSet_Statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.942519 alphastats-0.4.4/alphastats/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/data/contaminations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.942519 alphastats-0.4.4/alphastats/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.942519 alphastats-0.4.4/alphastats/gui/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/AlphaPeptStats.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/alphapeptstats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/alphastats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/alphastats_logo_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.946519 alphastats-0.4.4/alphastats/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/pages/02_Import Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/pages/03_Data Overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/pages/03_Preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/pages/04_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/pages/06_Results.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.946519 alphastats-0.4.4/alphastats/gui/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/sample_data/metadata.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/sample_data/proteinGroups.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.958519 alphastats-0.4.4/alphastats/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/utils/analysis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/utils/software_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/gui/utils/ui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.958519 alphastats-0.4.4/alphastats/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/loader/AlphaPeptLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/loader/BaseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/loader/DIANNLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/loader/FragPipeLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/loader/MaxQuantLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/loader/SpectronautLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/loader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.958519 alphastats-0.4.4/alphastats/multicova/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/multicova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/multicova/multicova.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.962519 alphastats-0.4.4/alphastats/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/plots/ClusterMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/plots/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/plots/IntensityPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/plots/PlotUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/plots/VolcanoPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-15 06:47:52.000000 alphastats-0.4.4/alphastats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 06:48:23.942519 alphastats-0.4.4/alphastats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-15 06:48:23.000000 alphastats-0.4.4/alphastats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-15 06:48:23.000000 alphastats-0.4.4/alphastats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 06:48:23.000000 alphastats-0.4.4/alphastats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-15 06:48:23.000000 alphastats-0.4.4/alphastats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-15 06:48:23.000000 alphastats-0.4.4/alphastats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-15 06:48:23.000000 alphastats-0.4.4/alphastats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 06:48:23.962519 alphastats-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-15 06:47:52.000000 alphastats-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.063468 alphastats-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-04-11 14:29:01.000000 alphastats-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-11 14:29:01.000000 alphastats-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-11 14:29:27.063468 alphastats-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-11 14:29:01.000000 alphastats-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.043468 alphastats-0.5.0/alphastats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/DataSet_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/DataSet_Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/DataSet_Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.047468 alphastats-0.5.0/alphastats/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/data/contaminations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.047468 alphastats-0.5.0/alphastats/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.047468 alphastats-0.5.0/alphastats/gui/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/AlphaPeptStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/alphapeptstats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/alphastats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/alphastats_logo_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.051468 alphastats-0.5.0/alphastats/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/pages/02_Import Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/pages/03_Data Overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/pages/03_Preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/pages/04_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/pages/06_Results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.051468 alphastats-0.5.0/alphastats/gui/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/sample_data/metadata.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/sample_data/proteinGroups.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.059467 alphastats-0.5.0/alphastats/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/utils/analysis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/utils/software_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/gui/utils/ui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.059467 alphastats-0.5.0/alphastats/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/loader/AlphaPeptLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/loader/BaseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/loader/DIANNLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/loader/FragPipeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/loader/MaxQuantLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/loader/SpectronautLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/loader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.059467 alphastats-0.5.0/alphastats/multicova/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/multicova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/multicova/multicova.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.059467 alphastats-0.5.0/alphastats/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/plots/ClusterMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/plots/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/plots/IntensityPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/plots/PlotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/plots/SampleHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/plots/VolcanoPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.063468 alphastats-0.5.0/alphastats/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/statistics/Anova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/statistics/DifferentialExpressionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/statistics/MultiCovaAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/statistics/StatisticUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-11 14:29:01.000000 alphastats-0.5.0/alphastats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:29:27.043468 alphastats-0.5.0/alphastats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-11 14:29:27.000000 alphastats-0.5.0/alphastats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-11 14:29:27.000000 alphastats-0.5.0/alphastats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:29:27.000000 alphastats-0.5.0/alphastats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-11 14:29:27.000000 alphastats-0.5.0/alphastats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-11 14:29:27.000000 alphastats-0.5.0/alphastats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 14:29:27.000000 alphastats-0.5.0/alphastats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:29:27.063468 alphastats-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-11 14:29:01.000000 alphastats-0.5.0/setup.py
```

### Comparing `alphastats-0.4.4/LICENSE.txt` & `alphastats-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/PKG-INFO` & `alphastats-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.4.4
+Version: 0.5.0
 Summary: An open-source Python package for Mass Spectrometry Analysis
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@hotmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
@@ -43,84 +43,77 @@
 </div>
 
 <br>
 <br>
 
 [link]:https://alphapeptstats.readthedocs.io/en/main/
 
-An open-source Python package of the AlphaPept ecosystem from the [Mann Group at the University of Copenhagen](https://www.biochem.mpg.de/mann).
+An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
 
 
-* [**About**](#about)
+* [**Citation**](#citation)
 * [**Installation**](#installation)
- * [Pip Installation](#pip-installation)
- * [One Click Installer](#one-click-installer)
- * [Docker Image](#docker-image)
-* [**Usage**](#usage)
 * [**Troubleshooting**](#troubleshooting)
-* [**Citations**](#citations)
 * [**License**](#license)
 * [**How to contribute**](#how-to-contribute)
 * [**Changelog**](#changelog)
 
 ---
-## About
-An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
+## Citation
+Manuscript: [AlphaPeptStats: an open-source Python package for automated, scalable and industrial-strength statistical analysis of mass spectrometry-based proteomics](https://doi.org/10.1101/2023.03.10.532057)
+> **Citation:** <br>
+> Krismer, E., Strauss M. & Mann M. (2023). AlphaPeptStats: an open-source Python package for automated, scalable and industrial-strength statistical analysis of mass spectrometry-based proteomics. BioRxiv [Preprint] 
+> https://doi.org/10.1101/2023.03.10.532057
 
 ---
-
 ## Installation
 
-AlphaPeptStats can be used as python library (pip-installation), or Graphical User Interface (either pip-installation or one-click installer). Further we provide a Dockerimage for the GUI.
-
----
+AlphaPeptStats can be used as 
+ * python library (pip-installation), or 
+ * Graphical User Interface (either pip-installation or one-click installer). 
+ 
+Further we provide a Dockerimage for the GUI.
 
-## Pip Installation
+### Pip Installation
 
 AlphaStats can be installed in an existing Python 3.8/3.9/3.10 environment with a single `bash` command. 
 
 ```bash
 pip install alphastats
 ```
----
-## Usage
 
-For the Graphical User Interface
+In case you want to use the Graphical User Interface, use following command in the command line:
  
 ```bash
 alphastats gui
 ```
 
 AlphaStats can be imported as a Python package into any Python script or notebook with the command `import alphastats`.
-
 A brief [Jupyter notebook tutorial](nbs/getting_started.ipynb) on how to use the API is also present in the [nbs folder](nbs).
 
----
 
-## One Click Installer
+### One Click Installer
 
-One click Installer for MacOS, Windows and Linux can be found [here](https://github.com/MannLabs/alphapeptstats/releases)
+One click Installer for MacOS, Windows and Linux can be found [here](https://github.com/MannLabs/alphapeptstats/releases).
 
----
 
-## Docker Image
+### Docker Image
 
 We provide two Dockerfiles, one for the library and one for the Graphical User Interface.
 The Image can be pulled from Dockerhub
 
 ```bash
 docker pull elenakrismer/alphapeptstats_streamlit
 ```
 
 ---
-
 ## GUI
 ![](https://github.com/MannLabs/alphapeptstats/blob/main/misc/volcano.gif)
 
-
+---
 ## Troubleshooting
 
 In case of issues, check out the following:
 
 * [Issues](https://github.com/MannLabs/alphapeptstats/issues): Try a few different search terms to find out if a similar problem has been encountered before
 
 ---
@@ -133,7 +126,14 @@
 
 If you like this software, you can give us a [star](https://github.com/MannLabs/alphapeptstats/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/alphapeptstats/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/alphapeptstats/pulls) with a new branch. For an even more interactive participation, check out the [discussions](https://github.com/MannLabs/alphapeptstats/discussions) and the [the Contributors License Agreement](misc/CLA.md).
 
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made in each version.
+
+
+---
+## FAQ
+
+### How can I resolve the Microsoft visual error message when installing: error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools"?
+Please, find a description on how to update required tools [here](https://github.com/MannLabs/alphapeptstats/issues/158).
```

### Comparing `alphastats-0.4.4/README.md` & `alphastats-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,84 +20,77 @@
 </div>
 
 <br>
 <br>
 
 [link]:https://alphapeptstats.readthedocs.io/en/main/
 
-An open-source Python package of the AlphaPept ecosystem from the [Mann Group at the University of Copenhagen](https://www.biochem.mpg.de/mann).
+An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
 
 
-* [**About**](#about)
+* [**Citation**](#citation)
 * [**Installation**](#installation)
- * [Pip Installation](#pip-installation)
- * [One Click Installer](#one-click-installer)
- * [Docker Image](#docker-image)
-* [**Usage**](#usage)
 * [**Troubleshooting**](#troubleshooting)
-* [**Citations**](#citations)
 * [**License**](#license)
 * [**How to contribute**](#how-to-contribute)
 * [**Changelog**](#changelog)
 
 ---
-## About
-An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
+## Citation
+Manuscript: [AlphaPeptStats: an open-source Python package for automated, scalable and industrial-strength statistical analysis of mass spectrometry-based proteomics](https://doi.org/10.1101/2023.03.10.532057)
+> **Citation:** <br>
+> Krismer, E., Strauss M. & Mann M. (2023). AlphaPeptStats: an open-source Python package for automated, scalable and industrial-strength statistical analysis of mass spectrometry-based proteomics. BioRxiv [Preprint] 
+> https://doi.org/10.1101/2023.03.10.532057
 
 ---
-
 ## Installation
 
-AlphaPeptStats can be used as python library (pip-installation), or Graphical User Interface (either pip-installation or one-click installer). Further we provide a Dockerimage for the GUI.
-
----
+AlphaPeptStats can be used as 
+ * python library (pip-installation), or 
+ * Graphical User Interface (either pip-installation or one-click installer). 
+ 
+Further we provide a Dockerimage for the GUI.
 
-## Pip Installation
+### Pip Installation
 
 AlphaStats can be installed in an existing Python 3.8/3.9/3.10 environment with a single `bash` command. 
 
 ```bash
 pip install alphastats
 ```
----
-## Usage
 
-For the Graphical User Interface
+In case you want to use the Graphical User Interface, use following command in the command line:
  
 ```bash
 alphastats gui
 ```
 
 AlphaStats can be imported as a Python package into any Python script or notebook with the command `import alphastats`.
-
 A brief [Jupyter notebook tutorial](nbs/getting_started.ipynb) on how to use the API is also present in the [nbs folder](nbs).
 
----
 
-## One Click Installer
+### One Click Installer
 
-One click Installer for MacOS, Windows and Linux can be found [here](https://github.com/MannLabs/alphapeptstats/releases)
+One click Installer for MacOS, Windows and Linux can be found [here](https://github.com/MannLabs/alphapeptstats/releases).
 
----
 
-## Docker Image
+### Docker Image
 
 We provide two Dockerfiles, one for the library and one for the Graphical User Interface.
 The Image can be pulled from Dockerhub
 
 ```bash
 docker pull elenakrismer/alphapeptstats_streamlit
 ```
 
 ---
-
 ## GUI
 ![](https://github.com/MannLabs/alphapeptstats/blob/main/misc/volcano.gif)
 
-
+---
 ## Troubleshooting
 
 In case of issues, check out the following:
 
 * [Issues](https://github.com/MannLabs/alphapeptstats/issues): Try a few different search terms to find out if a similar problem has been encountered before
 
 ---
@@ -110,7 +103,14 @@
 
 If you like this software, you can give us a [star](https://github.com/MannLabs/alphapeptstats/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/alphapeptstats/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/alphapeptstats/pulls) with a new branch. For an even more interactive participation, check out the [discussions](https://github.com/MannLabs/alphapeptstats/discussions) and the [the Contributors License Agreement](misc/CLA.md).
 
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made in each version.
+
+
+---
+## FAQ
+
+### How can I resolve the Microsoft visual error message when installing: error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools"?
+Please, find a description on how to update required tools [here](https://github.com/MannLabs/alphapeptstats/issues/158).
```

### Comparing `alphastats-0.4.4/alphastats/DataSet.py` & `alphastats-0.5.0/alphastats/DataSet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from random import sample
 import pandas as pd
 import numpy as np
 import logging
 import warnings
+import plotly
 
 from alphastats.loader.AlphaPeptLoader import AlphaPeptLoader
 from alphastats.loader.DIANNLoader import DIANNLoader
 from alphastats.loader.FragPipeLoader import FragPipeLoader
 from alphastats.loader.MaxQuantLoader import MaxQuantLoader
 from alphastats.loader.SpectronautLoader import SpectronautLoader
 
@@ -16,14 +17,34 @@
 from alphastats.DataSet_Statistics import Statistics
 from alphastats.utils import LoaderError
 
 # remove warning from openpyxl
 # only appears on mac
 warnings.filterwarnings("ignore", category=UserWarning, module="openpyxl")
 
+plotly.io.templates["alphastats_colors"] = plotly.graph_objects.layout.Template(
+    layout=plotly.graph_objects.Layout(
+        paper_bgcolor="rgba(0,0,0,0)",
+        plot_bgcolor="rgba(0,0,0,0)",
+        colorway=[
+            "#009599",
+            "#005358",
+            "#772173",
+            "#B65EAF",  # pink
+            "#A73A00",
+            "#6490C1",
+            "#FF894F",
+            "#2B5E8B",
+            "#A87F32",
+        ],
+    )
+)
+
+plotly.io.templates.default = "simple_white+alphastats_colors"
+
 
 class DataSet(Preprocess, Statistics, Plot, Enrichment):
     """Analysis Object"""
 
     def __init__(self, loader, metadata_path=None, sample_column=None):
         """Create DataSet
```

### Comparing `alphastats-0.4.4/alphastats/DataSet_Pathway.py` & `alphastats-0.5.0/alphastats/DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/DataSet_Plot.py` & `alphastats-0.5.0/alphastats/DataSet_Plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import itertools
 import plotly.figure_factory
 
 from alphastats.plots.DimensionalityReduction import DimensionalityReduction
 from alphastats.plots.VolcanoPlot import VolcanoPlot
 from alphastats.plots.IntensityPlot import IntensityPlot
 from alphastats.plots.ClusterMap import ClusterMap
+from alphastats.plots.SampleHistogram import SampleHistogram
 from alphastats.utils import ignore_warning, check_for_missing_values
 
 
 class plotly_object(plotly.graph_objs._figure.Figure):
     plotting_data = None
     preprocessing = None
     method = None
@@ -286,14 +287,22 @@
             label_bar=label_bar,
             only_significant=only_significant,
             group=group,
             subgroups=subgroups
         )
         return  clustermap.plot
 
+    def plot_samplehistograms(self):
+        """Plots the Denisty distribution of each sample
+
+        Returns:
+            plotly: Plotly Graph Object
+        """
+        return SampleHistogram(dataset=self).plot()
+
     @check_for_missing_values
     def plot_dendrogram(
         self, linkagefun=lambda x: scipy.cluster.hierarchy.linkage(x, "complete")
     ):
         """Plot Hierarichical Clustering Dendrogram. This is a wrapper around:
         https://plotly.com/python-api-reference/generated/plotly.figure_factory.create_dendrogram.html
```

### Comparing `alphastats-0.4.4/alphastats/DataSet_Preprocess.py` & `alphastats-0.5.0/alphastats/DataSet_Preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sklearn.ensemble
 import sklearn.impute
 from alphastats.utils import ignore_warning
 from sklearn.experimental import enable_iterative_imputer
 import itertools
 
 
+
 class Preprocess:
     def _remove_sampels(self, sample_list):
         # exclude samples for analysis
         self.mat = self.mat.drop(sample_list)
         self.metadata = self.metadata[~self.metadata[self.sample].isin(sample_list)]
 
     def _subset(self):
@@ -162,15 +163,15 @@
     def reset_preprocessing(self):
         """ Reset all preprocessing steps
         """
         # reset all preprocessing steps
         self.create_matrix()
         print("All preprocessing steps are reset.")
     
-    def _compare_preprocessing_modes(self, func, params_for_func):
+    def _compare_preprocessing_modes(self, func, params_for_func) -> list:
         dataset = self
         imputation_methods = ["mean", "median", "knn"]
         normalization_methods = ["zscore", "quantile", "vst"]
         preprocessing_modes = list(itertools.product(normalization_methods, imputation_methods))
 
         results_list = []
 
@@ -191,26 +192,39 @@
             res = func(**params_for_func)
             results_list.append(res)
         
         return results_list
 
     def _log2_transform(self):
         self.mat = np.log2(self.mat + 0.1)
-        self.preprocessing_info.update({"Log2 Transformed": True})
+        self.preprocessing_info.update({"Log2-transformed": True})
+        print("Data has been log2-transformed.")
+    
+    def batch_correction(self, batch:str):
+        """Correct for technical bias/batch effects
+        Behdenna A, Haziza J, Azencot CA and Nordor A. (2020) pyComBat, a Python tool for batch effects correction in high-throughput molecular data using empirical Bayes methods. bioRxiv doi: 10.1101/2020.03.17.995431
 
+        Args:
+            batch (str): column name in the metadata describing the different batches
+        """
+        import combat
+        from combat.pycombat import pycombat
+        data = self.mat.transpose()
+        series_of_batches = self.metadata.set_index(self.sample).reindex(data.columns.to_list())[batch]
+        self.mat = pycombat(data=data, batch=series_of_batches).transpose()
 
     @ignore_warning(RuntimeWarning)
     def preprocess(
         self,
-        log2_transform=True,
-        remove_contaminations=False,
-        subset=False,
-        normalization=None,
-        imputation=None,
-        remove_samples=None,
+        log2_transform: bool=True,
+        remove_contaminations: bool=False,
+        subset: bool=False,
+        normalization: str=None,
+        imputation: str=None,
+        remove_samples: list=None,
     ):
         """Preprocess Protein data
 
         Removal of contaminations:
 
         Removes all observations, that were identified as contaminations.
 
@@ -247,25 +261,25 @@
             normalization (str, optional): method to normalize data: either "zscore", "quantile", "linear". Defaults to None.
             remove_samples (list, optional): list with sample ids to remove. Defaults to None.
             imputation (str, optional):  method to impute data: either "mean", "median", "knn" or "randomforest". Defaults to None.
             subset (bool, optional): filter matrix so only samples that are described in metadata found in matrix. Defaults to False.
         """
         if remove_contaminations:
             self._filter()
+        
+        if remove_samples is not None:
+            self._remove_sampels(sample_list=remove_samples)
 
         if subset:
             self.mat = self._subset()
         
         if log2_transform:
             self._log2_transform()
 
         if normalization is not None:
             self._normalization(method=normalization)
 
         if imputation is not None:
             self._imputation(method=imputation)
 
-        if remove_samples is not None:
-            self._remove_sampels(sample_list=remove_samples)
-
         self.mat = self.mat.loc[:, (self.mat != 0).any(axis=0)]
         self.preprocessed = True
```

### Comparing `alphastats-0.4.4/alphastats/__init__.py` & `alphastats-0.5.0/alphastats/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "alphastats"
-__version__ = "0.4.4"
+__version__ = "0.5.0"
 __license__ = "Apache"
 __description__ = "An open-source Python package for Mass Spectrometry Analysis"
 __author__ = "Mann Labs"
 __author_email__ = "elena.krismer@hotmail.com"
 __github__ = "https://github.com/MannLabs/alphapeptstats"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphastats-0.4.4/alphastats/data/contaminations.txt` & `alphastats-0.5.0/alphastats/data/contaminations.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/AlphaPeptStats.py` & `alphastats-0.5.0/alphastats/gui/AlphaPeptStats.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/alphapeptstats_logo.png` & `alphastats-0.5.0/alphastats/gui/alphapeptstats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/alphastats_logo.png` & `alphastats-0.5.0/alphastats/gui/alphastats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/alphastats_logo_2.png` & `alphastats-0.5.0/alphastats/gui/alphastats_logo_2.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/gui.py` & `alphastats-0.5.0/alphastats/gui/gui.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/pages/02_Import Data.py` & `alphastats-0.5.0/alphastats/gui/pages/02_Import Data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from curses import meta
 import streamlit as st
-
+import sys
 import os
 
 try:
     from alphastats.gui.utils.ui_helper import sidebar_info
     from alphastats.gui.utils.analysis_helper import *
     from alphastats.gui.utils.software_options import software_options
     from alphastats.loader.MaxQuantLoader import MaxQuantLoader
@@ -18,14 +17,24 @@
     from alphastats import DataSet
 
 
 
 import pandas as pd
 import plotly.express as px
 
+from streamlit.runtime import get_instance
+from streamlit.runtime.scriptrunner.script_run_context import get_script_run_ctx
+
+runtime = get_instance()
+session_id = get_script_run_ctx().session_id
+session_info = runtime._session_mgr.get_session_info(session_id)
+
+user_session_id = session_id
+st.session_state["user_session_id"] = user_session_id
+
 
 def load_options():
 
     from alphastats.gui.utils.options import plotting_options, statistic_options
 
     st.session_state["plotting_options"] = plotting_options
     st.session_state["statistic_options"] = statistic_options
@@ -215,17 +224,21 @@
 
         display_loaded_dataset()
 
 
 def load_sample_data():
     _this_file = os.path.abspath(__file__)
     _this_directory = os.path.dirname(_this_file)
-    filepath = os.path.join(_this_directory, "sample_data/proteinGroups.txt").replace("pages/","")
-    metadatapath =  os.path.join(_this_directory, "sample_data/metadata.xlsx").replace("pages/","")
+    _parent_directory = os.path.dirname(_this_directory)     
+    folder_to_load = os.path.join(_parent_directory, 'sample_data')
     
+    filepath= os.path.join(folder_to_load, "proteinGroups.txt")
+    metadatapath= os.path.join(folder_to_load, "metadata.xlsx")
+
+
     loader = MaxQuantLoader(file=filepath)
     ds = DataSet(
         loader=loader, metadata_path=metadatapath, sample_column="sample"
     )
     
     ds.metadata = ds.metadata[
         [
```

### Comparing `alphastats-0.4.4/alphastats/gui/pages/03_Data Overview.py` & `alphastats-0.5.0/alphastats/gui/pages/03_Data Overview.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 def display_matrix():
 
     text = (
         "Normalization: "
         + str(st.session_state.dataset.preprocessing_info["Normalization"])
         + ", Imputation: "
         + str(st.session_state.dataset.preprocessing_info["Imputation"])
+        + ", Log2-transformed: "
+        + str(st.session_state.dataset.preprocessing_info["Log2-transformed"])
     )
 
     st.markdown("**DataFrame used for analysis** *preview*")
     st.markdown(text)
 
     df = get_display_matrix()
     csv = convert_df(st.session_state.dataset.mat)
@@ -37,14 +39,24 @@
     st.dataframe(df)
 
     st.download_button(
         "Download as .csv", csv, "analysis_matrix.csv", "text/csv", key="download-csv"
     )
 
 
+@st.cache_data
+def get_sample_histogram_matrix(user_session_id = st.session_state.user_session_id):
+    return st.session_state.dataset.plot_samplehistograms()
+
+@st.cache_data
+def get_intensity_distribution_processed(user_session_id = st.session_state.user_session_id):
+    return st.session_state.dataset.plot_sampledistribution()
+
+
+
 if "dataset" in st.session_state:
     st.markdown("## DataSet overview")
 
     c1, c2 = st.columns(2)
     
     with c1:
 
@@ -53,15 +65,22 @@
             st.session_state.distribution_plot.update_layout(plot_bgcolor="white"),
             use_container_width=True
         )
     
     with c2:
 
         st.markdown("**Intensity distribution data per sample used for analysis**")
-        fig_processed = st.session_state.dataset.plot_sampledistribution()
-        st.plotly_chart(fig_processed.update_layout(plot_bgcolor="white"), use_container_width=True)
+        st.plotly_chart(
+            get_intensity_distribution_processed(user_session_id = st.session_state.user_session_id)
+                        .update_layout(plot_bgcolor="white"), use_container_width=True
+        )
+ 
+    st.plotly_chart(
+        get_sample_histogram_matrix(user_session_id = st.session_state.user_session_id)
+                    .update_layout(plot_bgcolor="white"), use_container_width=True
+    )
 
     display_matrix()
 
 
 else:
     st.info("Import Data first")
```

### Comparing `alphastats-0.4.4/alphastats/gui/pages/03_Preprocessing.py` & `alphastats-0.5.0/alphastats/gui/pages/03_Preprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     c1, c2 = st.columns(2)
 
     with c1:
 
         st.markdown(
             "Before analyzing your data, consider normalizing and imputing your data as well as the removal of contaminants. "
-            + "A more detailed description about the preprocessing methods can be found in the AlphaPeptStats" 
+            + "A more detailed description about the preprocessing methods can be found in the AlphaPeptStats " 
             + "[documentation](https://alphapeptstats.readthedocs.io/en/main/data_preprocessing.html)."
         )
 
         with st.form("preprocessing"):
             dataset = st.session_state["dataset"]
 
             remove_contaminations = st.selectbox(
@@ -25,14 +25,19 @@
             )
 
             subset = st.selectbox(
                 "Subset data so it matches with metadata. Remove miscellanous samples in rawinput.",
                 options=[True, False],
             )
 
+            remove_samples = st.multiselect(
+                "Remove samples from analysis", 
+                options=st.session_state.dataset.metadata[st.session_state.dataset.sample].to_list()
+            )
+
             log2_transform = st.selectbox(
                 "Log2-transform dataset",
                 options=[True, False],
             )
 
             normalization = st.selectbox(
                 "Normalization", options=[None, "zscore", "quantile", "vst", "linear"]
@@ -41,40 +46,66 @@
             imputation = st.selectbox(
                 "Imputation", options=[None, "mean", "median", "knn", "randomforest"]
             )
 
             submitted = st.form_submit_button("Submit")
 
         if submitted:
+            if len(remove_samples) == 0:
+                remove_samples = None
+            
             st.session_state.dataset.preprocess(
                 remove_contaminations=remove_contaminations,
                 log2_transform=log2_transform,
+                remove_samples = remove_samples,
                 subset=subset,
                 normalization=normalization,
                 imputation=imputation,
             )
             preprocessing = st.session_state.dataset.preprocessing_info
             st.info(
                 "Data has been processed. "
                 + datetime.datetime.now().strftime("%d/%m/%Y %H:%M:%S")
             )
             st.dataframe(
                 pd.DataFrame.from_dict(preprocessing, orient="index").astype(str),
                 use_container_width=True,
             )
+        
+        st.markdown("#### Batch correction: correct for technical bias")
+
+        with st.form("Batch correction: correct for technical bias"):
+            batch = st.selectbox(
+                "Batch", 
+                options= st.session_state.dataset.metadata.columns.to_list()
+            )
+            submit_batch_correction = st.form_submit_button("Submit")
+        
+        if submit_batch_correction:
+            st.session_state.dataset.batch_correction(
+                batch=batch
+            )
+            st.info(
+                "Data has been processed. "
+                + datetime.datetime.now().strftime("%d/%m/%Y %H:%M:%S")
+            )
+
     
     with c2:
-        st.markdown("**Intensity Distribution per sample**")
-        fig_none_processed = st.session_state.dataset.plot_sampledistribution()
-        st.plotly_chart(fig_none_processed.update_layout(plot_bgcolor="white"), use_container_width=True)
-        
+
         if submitted:
             st.markdown("**Intensity Distribution after preprocessing per sample**")
             fig_processed = st.session_state.dataset.plot_sampledistribution()
             st.plotly_chart(fig_processed.update_layout(plot_bgcolor="white"), use_container_width=True)
+        
+        else:
+            st.markdown("**Intensity Distribution per sample**")
+            fig_none_processed = st.session_state.dataset.plot_sampledistribution()
+            st.plotly_chart(fig_none_processed.update_layout(plot_bgcolor="white"), use_container_width=True)
+        
     
     reset_steps = st.button("Reset all Preprocessing steps")
         
     if reset_steps:
         reset_preprocessing()
```

### Comparing `alphastats-0.4.4/alphastats/gui/pages/04_Analysis.py` & `alphastats-0.5.0/alphastats/gui/pages/04_Analysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/pages/06_Results.py` & `alphastats-0.5.0/alphastats/gui/pages/06_Results.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/sample_data/metadata.xlsx` & `alphastats-0.5.0/alphastats/gui/sample_data/metadata.xlsx`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/sample_data/proteinGroups.txt` & `alphastats-0.5.0/alphastats/gui/sample_data/proteinGroups.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/utils/analysis_helper.py` & `alphastats-0.5.0/alphastats/gui/utils/analysis_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,18 @@
     submitted = st.button("Submit")
 
     if submitted:
         with st.spinner("Calculating..."):
             return method_dict["function"](**chosen_parameter_dict)
 
 
-@st.cache(persist=True, max_entries=10, allow_output_mutation=True)
-def gui_volcano_plot_differential_expression_analysis(chosen_parameter_dict):
+@st.cache_data
+def gui_volcano_plot_differential_expression_analysis(
+        chosen_parameter_dict, user_session_id = st.session_state.user_session_id
+    ):
     """
     initalize volcano plot object with differential expression analysis results
     """
     volcano_plot = VolcanoPlot(
         dataset=st.session_state.dataset, 
         **chosen_parameter_dict, 
         plot = False
@@ -88,15 +90,15 @@
 def gui_volcano_plot():
     """
     Draw Volcano Plot using the VolcanoPlot class
     """
     chosen_parameter_dict = helper_compare_two_groups()
     method = st.selectbox(
         "Differential Analysis using:",
-        options=["ttest", "anova", "wald", "sam"],
+        options=["ttest", "anova", "wald", "sam", "paired-ttest", "welch-ttest"],
     )
     chosen_parameter_dict.update({"method": method})
 
     # TODO streamlit doesnt allow nested columns check for updates
     
     labels = st.checkbox("Add label")
 
@@ -124,15 +126,17 @@
         )
         chosen_parameter_dict.update({"perm": perm, "fdr": fdr})
 
    
     submitted = st.button("Submit")
 
     if submitted:
-        volcano_plot = gui_volcano_plot_differential_expression_analysis(chosen_parameter_dict)
+        volcano_plot = gui_volcano_plot_differential_expression_analysis(
+            chosen_parameter_dict, user_session_id = st.session_state.user_session_id
+        )
         volcano_plot._update(plotting_parameter_dict)
         volcano_plot._annotate_result_df()
         volcano_plot._plot()
         return volcano_plot.plot
 
 
 def get_analysis_options_from_dict(method, options_dict):
@@ -255,52 +259,40 @@
     group = st.selectbox(
         "Grouping variable",
         options=["< None >"] + st.session_state.dataset.metadata.columns.to_list(),
     )
 
     if group != "< None >":
 
-        #col1, col2 = st.columns(2)
-
         unique_values = get_unique_values_from_column(group)
 
-        #with col1:
-
         group1 = st.selectbox("Group 1", options=unique_values)
 
-        #with col2:
-
         group2 = st.selectbox("Group 2", options=list(reversed(unique_values)))
 
         chosen_parameter_dict.update(
             {"column": group, "group1": group1, "group2": group2}
         )
 
         if group1 == group2:
             st.error(
                 "Group 1 and Group 2 can not be the same please select different group."
             )
 
     else:
 
-        #col1, col2 = st.columns(2)
-
-        #with col1:
-
         group1 = st.multiselect(
                 "Group 1 samples:",
-                options=st.session_state.dataset.metadata["sample"].to_list(),
+                options=st.session_state.dataset.metadata[st.session_state.dataset.sample].to_list(),
             )
 
-        #with col2:
-
         group2 = st.multiselect(
                 "Group 2 samples:",
                 options=list(
-                    reversed(st.session_state.dataset.metadata["sample"].to_list())
+                    reversed(st.session_state.dataset.metadata[st.session_state.dataset.sample].to_list())
                 ),
             )
 
         intersection_list = list(set(group1).intersection(set(group2)))
 
         if len(intersection_list) > 0:
             st.warning(
```

### Comparing `alphastats-0.4.4/alphastats/gui/utils/options.py` & `alphastats-0.5.0/alphastats/gui/utils/options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/utils/software_options.py` & `alphastats-0.5.0/alphastats/gui/utils/software_options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/gui/utils/ui_helper.py` & `alphastats-0.5.0/alphastats/gui/utils/ui_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/load_data.py` & `alphastats-0.5.0/alphastats/load_data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/loader/AlphaPeptLoader.py` & `alphastats-0.5.0/alphastats/loader/AlphaPeptLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/loader/BaseLoader.py` & `alphastats-0.5.0/alphastats/loader/BaseLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import logging
 import os
 import numpy as np
-from iteration_utilities import duplicates
+from alphastats.utils import find_duplicates_in_list
 import pkg_resources
 
 
 class BaseLoader:
     """Parent class of Loaders"""
 
     def __init__(self, file, intensity_column, index_column, sep):
@@ -48,15 +48,15 @@
                 "MaxQuant Format: http://www.coxdocs.org/doku.php?id=maxquant:table:proteingrouptable"
             )
     
     def _read_all_columns_as_string(self):
         self.rawinput.columns = self.rawinput.columns.astype(str)
 
     def _check_if_indexcolumn_is_unique(self):
-        duplicated_values = list(duplicates(self.rawinput[self.index_column].to_list()))
+        duplicated_values = find_duplicates_in_list(self.rawinput[self.index_column].to_list())
         if len(duplicated_values) > 0:
             # error or warning, duplicates could be resolved with preprocessing/filtering
             logging.warning(
                 f"Column {self.index_column} contains duplicated values: "
                 + ", ".join(duplicated_values)
             )
```

### Comparing `alphastats-0.4.4/alphastats/loader/DIANNLoader.py` & `alphastats-0.5.0/alphastats/loader/DIANNLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/loader/FragPipeLoader.py` & `alphastats-0.5.0/alphastats/loader/FragPipeLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/loader/MaxQuantLoader.py` & `alphastats-0.5.0/alphastats/loader/MaxQuantLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/loader/SpectronautLoader.py` & `alphastats-0.5.0/alphastats/loader/SpectronautLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/multicova/multicova.py` & `alphastats-0.5.0/alphastats/multicova/multicova.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import math
 import swifter
 from sklearn.preprocessing import StandardScaler
 from statsmodels.stats.multitest import multipletests
 import os
 from pathlib import Path
 
+# code taken from Isabel Bludau - multicova
 
 def get_std(x):
     """
     Function to calculate the sample standard deviation.
     """
     std_x = np.sqrt(np.sum((abs(x - x.mean())**2)/(len(x)-1)))
     return std_x
@@ -305,15 +306,15 @@
 
     s_df = pd.DataFrame(np.array([fc_s, svals, pvals]).T, columns=['fc_s','svals','pvals'])
     s_df = s_df[s_df.pvals != 1]
 
     s_df_neg = s_df.copy()
     s_df_neg.fc_s = -s_df_neg.fc_s
 
-    s_df = s_df.append(s_df_neg)
+    s_df = pd.concat([s_df, s_df_neg])
 
     if (plot):
         fig = px.scatter(x=s_df.fc_s,
                          y=-np.log10(s_df.pvals),
                          template='simple_white')
         fig.show()
 
@@ -465,15 +466,15 @@
     for k in np.arange(0, X.shape[1]):
         s_df = pd.DataFrame(np.array([fc_s,svals[k],pvals[k]]).T, columns=['fc_s','svals','pvals'])
         s_df = s_df[s_df.pvals != 1]
 
         s_df_neg = s_df.copy()
         s_df_neg.fc_s = -s_df_neg.fc_s
 
-        s_df = s_df.append(s_df_neg)
+        s_df = pd.concat([s_df, s_df_neg])
 
         if (plot):
             fig = px.scatter(x=s_df.fc_s,
                              y=-np.log10(s_df.pvals),
                              template='simple_white')
             fig.show()
```

### Comparing `alphastats-0.4.4/alphastats/plots/ClusterMap.py` & `alphastats-0.5.0/alphastats/plots/ClusterMap.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/plots/DimensionalityReduction.py` & `alphastats-0.5.0/alphastats/plots/DimensionalityReduction.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/plots/IntensityPlot.py` & `alphastats-0.5.0/alphastats/plots/IntensityPlot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/plots/PlotUtils.py` & `alphastats-0.5.0/alphastats/plots/PlotUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.4.4/alphastats/plots/VolcanoPlot.py` & `alphastats-0.5.0/alphastats/plots/VolcanoPlot.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 
         elif self.method == "ttest":
             self._ttest()
 
         elif self.method == "anova":
             self._anova()
         
+        elif self.method == "welch-ttest":
+            self._welch_ttest()
+        
+        elif self.method == "paired-ttest":
+            self._pairedttest()
+        
         elif self.method == "sam":
             self._sam()
         
         # elif self.method == "Multi Covariates":
         #    raise NotImplementedError
 
         else:
@@ -148,17 +154,43 @@
             group1=self.group1,
             group2=self.group2,
             method=self.method,
         )
         self.pvalue_column = "qval"
 
     @lru_cache(maxsize=20)
+    def _welch_ttest(self):
+
+        print("Calculating Welchs t-test...")
+
+        self.res = self.dataset.diff_expression_analysis(
+            column=self.column,
+            group1=self.group1,
+            group2=self.group2,
+            method=self.method,
+        )
+        self.pvalue_column = "pval"
+    
+    @lru_cache(maxsize=20)
     def _ttest(self):
 
-        print("Calculating t-test...")
+        print("Calculating Students t-test...")
+
+        self.res = self.dataset.diff_expression_analysis(
+            column=self.column,
+            group1=self.group1,
+            group2=self.group2,
+            method=self.method,
+        )
+        self.pvalue_column = "pval"
+    
+    @lru_cache(maxsize=20)
+    def _pairedttest(self):
+
+        print("Calculating paired t-test...")
 
         self.res = self.dataset.diff_expression_analysis(
             column=self.column,
             group1=self.group1,
             group2=self.group2,
             method=self.method,
         )
```

### Comparing `alphastats-0.4.4/alphastats.egg-info/PKG-INFO` & `alphastats-0.5.0/alphastats.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.4.4
+Version: 0.5.0
 Summary: An open-source Python package for Mass Spectrometry Analysis
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@hotmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
@@ -43,84 +43,77 @@
 </div>
 
 <br>
 <br>
 
 [link]:https://alphapeptstats.readthedocs.io/en/main/
 
-An open-source Python package of the AlphaPept ecosystem from the [Mann Group at the University of Copenhagen](https://www.biochem.mpg.de/mann).
+An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
 
 
-* [**About**](#about)
+* [**Citation**](#citation)
 * [**Installation**](#installation)
- * [Pip Installation](#pip-installation)
- * [One Click Installer](#one-click-installer)
- * [Docker Image](#docker-image)
-* [**Usage**](#usage)
 * [**Troubleshooting**](#troubleshooting)
-* [**Citations**](#citations)
 * [**License**](#license)
 * [**How to contribute**](#how-to-contribute)
 * [**Changelog**](#changelog)
 
 ---
-## About
-An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
+## Citation
+Manuscript: [AlphaPeptStats: an open-source Python package for automated, scalable and industrial-strength statistical analysis of mass spectrometry-based proteomics](https://doi.org/10.1101/2023.03.10.532057)
+> **Citation:** <br>
+> Krismer, E., Strauss M. & Mann M. (2023). AlphaPeptStats: an open-source Python package for automated, scalable and industrial-strength statistical analysis of mass spectrometry-based proteomics. BioRxiv [Preprint] 
+> https://doi.org/10.1101/2023.03.10.532057
 
 ---
-
 ## Installation
 
-AlphaPeptStats can be used as python library (pip-installation), or Graphical User Interface (either pip-installation or one-click installer). Further we provide a Dockerimage for the GUI.
-
----
+AlphaPeptStats can be used as 
+ * python library (pip-installation), or 
+ * Graphical User Interface (either pip-installation or one-click installer). 
+ 
+Further we provide a Dockerimage for the GUI.
 
-## Pip Installation
+### Pip Installation
 
 AlphaStats can be installed in an existing Python 3.8/3.9/3.10 environment with a single `bash` command. 
 
 ```bash
 pip install alphastats
 ```
----
-## Usage
 
-For the Graphical User Interface
+In case you want to use the Graphical User Interface, use following command in the command line:
  
 ```bash
 alphastats gui
 ```
 
 AlphaStats can be imported as a Python package into any Python script or notebook with the command `import alphastats`.
-
 A brief [Jupyter notebook tutorial](nbs/getting_started.ipynb) on how to use the API is also present in the [nbs folder](nbs).
 
----
 
-## One Click Installer
+### One Click Installer
 
-One click Installer for MacOS, Windows and Linux can be found [here](https://github.com/MannLabs/alphapeptstats/releases)
+One click Installer for MacOS, Windows and Linux can be found [here](https://github.com/MannLabs/alphapeptstats/releases).
 
----
 
-## Docker Image
+### Docker Image
 
 We provide two Dockerfiles, one for the library and one for the Graphical User Interface.
 The Image can be pulled from Dockerhub
 
 ```bash
 docker pull elenakrismer/alphapeptstats_streamlit
 ```
 
 ---
-
 ## GUI
 ![](https://github.com/MannLabs/alphapeptstats/blob/main/misc/volcano.gif)
 
-
+---
 ## Troubleshooting
 
 In case of issues, check out the following:
 
 * [Issues](https://github.com/MannLabs/alphapeptstats/issues): Try a few different search terms to find out if a similar problem has been encountered before
 
 ---
@@ -133,7 +126,14 @@
 
 If you like this software, you can give us a [star](https://github.com/MannLabs/alphapeptstats/stargazers) to boost our visibility! All direct contributions are also welcome. Feel free to post a new [issue](https://github.com/MannLabs/alphapeptstats/issues) or clone the repository and create a [pull request](https://github.com/MannLabs/alphapeptstats/pulls) with a new branch. For an even more interactive participation, check out the [discussions](https://github.com/MannLabs/alphapeptstats/discussions) and the [the Contributors License Agreement](misc/CLA.md).
 
 ---
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made in each version.
+
+
+---
+## FAQ
+
+### How can I resolve the Microsoft visual error message when installing: error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools"?
+Please, find a description on how to update required tools [here](https://github.com/MannLabs/alphapeptstats/issues/158).
```

### Comparing `alphastats-0.4.4/alphastats.egg-info/SOURCES.txt` & `alphastats-0.5.0/alphastats.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -47,9 +47,14 @@
 alphastats/loader/__init__.py
 alphastats/multicova/__init__.py
 alphastats/multicova/multicova.py
 alphastats/plots/ClusterMap.py
 alphastats/plots/DimensionalityReduction.py
 alphastats/plots/IntensityPlot.py
 alphastats/plots/PlotUtils.py
+alphastats/plots/SampleHistogram.py
 alphastats/plots/VolcanoPlot.py
-alphastats/plots/__init__.py
+alphastats/plots/__init__.py
+alphastats/statistics/Anova.py
+alphastats/statistics/DifferentialExpressionAnalysis.py
+alphastats/statistics/MultiCovaAnalysis.py
+alphastats/statistics/StatisticUtils.py
```

### Comparing `alphastats-0.4.4/setup.py` & `alphastats-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return required
     
 
 def create_pip_wheel():
     requirements = get_requirements()
     setuptools.setup(
         name="alphastats",
-        version="0.4.4",
+        version="0.5.0",
         license="Apache",
         description="An open-source Python package for Mass Spectrometry Analysis",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         author="Mann Labs",
         author_email="elena.krismer@hotmail.com",
         url="https://github.com/MannLabs/alphastats",
```

