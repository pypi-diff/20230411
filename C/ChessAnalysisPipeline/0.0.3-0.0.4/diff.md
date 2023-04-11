# Comparing `tmp/ChessAnalysisPipeline-0.0.3.tar.gz` & `tmp/ChessAnalysisPipeline-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChessAnalysisPipeline-0.0.3.tar", last modified: Tue Apr  4 16:09:36 2023, max compression
+gzip compressed data, was "ChessAnalysisPipeline-0.0.4.tar", last modified: Tue Apr 11 18:25:25 2023, max compression
```

## Comparing `ChessAnalysisPipeline-0.0.3.tar` & `ChessAnalysisPipeline-0.0.4.tar`

### file list

```diff
@@ -1,60 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.571785 ChessAnalysisPipeline-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.551785 ChessAnalysisPipeline-0.0.3/CHAP/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.551785 ChessAnalysisPipeline-0.0.3/CHAP/common/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.555785 ChessAnalysisPipeline-0.0.3/CHAP/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/models/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24961 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/models/map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24425 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3547 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.555785 ChessAnalysisPipeline-0.0.3/CHAP/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   125798 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/utils/fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/utils/material.py
--rw-r--r--   0 runner    (1001) docker     (123)    33421 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/utils/scanparsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/common/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.559785 ChessAnalysisPipeline-0.0.3/CHAP/edd/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/edd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/edd/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13599 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/edd/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/edd/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/edd/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.563785 ChessAnalysisPipeline-0.0.3/CHAP/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/inference/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/inference/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/inference/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3577 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2412 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.563785 ChessAnalysisPipeline-0.0.3/CHAP/saxswaxs/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/saxswaxs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/saxswaxs/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/saxswaxs/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/saxswaxs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.567785 ChessAnalysisPipeline-0.0.3/CHAP/sin2psi/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/sin2psi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/sin2psi/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/sin2psi/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/sin2psi/writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2759 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/CHAP/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.571785 ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-04 16:09:36.000000 ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-04 16:09:36.000000 ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:09:36.000000 ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-04 16:09:36.000000 ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 16:09:36.000000 ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 16:09:36.000000 ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:36.571785 ChessAnalysisPipeline-0.0.3/MLaaS/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/MLaaS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/MLaaS/ktrain.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/MLaaS/mnist_img.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/MLaaS/tfaas_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-04 16:09:36.571785 ChessAnalysisPipeline-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 16:09:36.571785 ChessAnalysisPipeline-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-04 16:09:20.000000 ChessAnalysisPipeline-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.084753 ChessAnalysisPipeline-0.0.4/CHAP/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/models/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/models/map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24425 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3547 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   127303 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48178 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/general.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/material.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34386 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/scanparsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/edd/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13557 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3577 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2412 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/CHAP/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97527 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2759 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/MLaaS/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/ktrain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/mnist_img.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/tfaas_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-11 18:25:18.000000 ChessAnalysisPipeline-0.0.4/setup.py
```

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/__init__.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/models/integration.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/models/integration.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/models/map.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/models/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,19 +217,19 @@
         for scans in spec_scans:
             for scan_number in scans.scan_numbers:
                 scanparser = scans.get_scanparser(scan_number)
                 if scan_step_index == 'all':
                     scan_step_index_range = range(scanparser.spec_scan_npts)
                 else:
                     scan_step_index_range = range(scan_step_index,scan_step_index+1)
-                for scan_step_index in scan_step_index_range:
+                for index in scan_step_index_range:
                     try:
-                        self.get_value(scans, scan_number, scan_step_index)
+                        self.get_value(scans, scan_number, index)
                     except:
-                        raise(RuntimeError(f'Could not find data for {self.name} (data_type "{self.data_type}") on scan number {scan_number} in spec file {scans.spec_file}'))
+                        raise(RuntimeError(f'Could not find data for {self.name} (data_type "{self.data_type}") on scan number {scan_number} for index {index} in spec file {scans.spec_file}'))
     def get_value(self, spec_scans:SpecScans, scan_number:int, scan_step_index:int):
         """Return the value recorded for this instance of `PointByPointScanData`
         at a specific scan step.
         
         :param spec_scans: An instance of `SpecScans` in which the requested scan step occurs.
         :type spec_scans: SpecScans
         :param scan_number: The number of the scan in which the requested scan step occurs.
@@ -304,17 +304,18 @@
     :type par_name: str
     :return: The value of the .par file value for  the scan requested.
     :rtype: float
     """
     scanparser = get_scanparser(spec_file, scan_number)
     return(scanparser.pars[par_name])
 def validate_data_source_for_map_config(data_source, values):
-    import_scanparser(values.get('station'), values.get('experiment_type'))
-    data_source.validate_for_station(values.get('station'))
-    data_source.validate_for_spec_scans(values.get('spec_scans'))
+    if data_source is not None:
+        import_scanparser(values.get('station'), values.get('experiment_type'))
+        data_source.validate_for_station(values.get('station'))
+        data_source.validate_for_spec_scans(values.get('spec_scans'))
     return(data_source)
 
 class CorrectionsData(PointByPointScanData):
     """Class representing the special instances of `PointByPointScanData` that
     are used by certain kinds of `CorrectionConfig` tools.
 
     :ivar label: One of the reserved values required by `CorrectionConfig`, 
@@ -420,15 +421,15 @@
     :ivar scalar_data: A list of the sources of data representing other scalar
         raw data values collected at each point ion the map. In the NeXus file
         representation of the map, datasets for these values will be included.
     :type scalar_values: Optional[list[PointByPointScanData]]
     """
     title: constr(strip_whitespace=True, min_length=1)
     station: Literal['id1a3','id3a','id3b']
-    experiment_type: Literal['SAXSWAXS', 'EDD', 'XRF']
+    experiment_type: Literal['SAXSWAXS', 'EDD', 'XRF', 'TOMO']
     sample: Sample
     spec_scans: conlist(item_type=SpecScans, min_items=1)
     independent_dimensions: conlist(item_type=PointByPointScanData, min_items=1)
     presample_intensity: Optional[PresampleIntensity]
     dwell_time_actual: Optional[DwellTimeActual]
     postsample_intensity: Optional[PostsampleIntensity]
     scalar_data: Optional[list[PointByPointScanData]] = []
@@ -439,19 +440,19 @@
     _validate_postsample_intensity = validator('postsample_intensity', allow_reuse=True)(validate_data_source_for_map_config)
     _validate_scalar_data = validator('scalar_data', each_item=True, allow_reuse=True)(validate_data_source_for_map_config)
     @validator('experiment_type')
     def validate_experiment_type(cls, value, values):
         '''Ensure values for the station and experiment_type fields are compatible'''
         station = values.get('station')
         if station == 'id1a3':
-            allowed_experiment_types = ['SAXSWAXS', 'EDD']
+            allowed_experiment_types = ['SAXSWAXS', 'EDD', 'TOMO']
         elif station == 'id3a':
-            allowed_experiment_types = ['EDD']
+            allowed_experiment_types = ['EDD', 'TOMO']
         elif station == 'id3b':
-            allowed_experiment_types = ['SAXSWAXS', 'XRF']
+            allowed_experiment_types = ['SAXSWAXS', 'XRF', 'TOMO']
         else:
             allowed_experiment_types = []
         if value not in allowed_experiment_types:
             raise(ValueError(f'For station {station}, allowed experiment types are {allowed_experiment_types} (suuplied experiment type {value} is not allowed)'))
         return(value)
     @property
     def coords(self):
```

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/processor.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/reader.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/reader.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/utils/__init__.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/utils/fit.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 Created on Mon Dec  6 15:36:22 2021
 
 @author: rv43
 """
 
 import logging
 
-from asteval import Interpreter, get_ast_names
+try:
+    from asteval import Interpreter, get_ast_names
+except:
+    pass
 from copy import deepcopy
-from lmfit import Model, Parameters
-from lmfit.model import ModelResult
-from lmfit.models import ConstantModel, LinearModel, QuadraticModel, PolynomialModel,\
-        ExponentialModel, StepModel, RectangleModel, ExpressionModel, GaussianModel,\
-        LorentzianModel
+try:
+    from lmfit import Model, Parameters
+    from lmfit.model import ModelResult
+    from lmfit.models import ConstantModel, LinearModel, QuadraticModel, PolynomialModel,\
+            ExponentialModel, StepModel, RectangleModel, ExpressionModel, GaussianModel,\
+            LorentzianModel
+except:
+    pass
 import numpy as np
 from os import cpu_count, getpid, listdir, mkdir, path
 from re import compile, sub
 from shutil import rmtree
 try:
     from sympy import diff, simplify
 except:
@@ -92,23 +98,24 @@
             try_linear_fit = kwargs.pop('try_linear_fit')
             if not isinstance(try_linear_fit, bool):
                 illegal_value(try_linear_fit, 'try_linear_fit', 'Fit.fit', raise_error=True)
             self._try_linear_fit = try_linear_fit
         if y is not None:
             if isinstance(y, (tuple, list, np.ndarray)):
                 self._x = np.asarray(x)
+                self._y = np.asarray(y)
             elif have_xarray and isinstance(y, xr.DataArray):
                 if x is not None:
                     logging.warning('Ignoring superfluous input x ({x}) in Fit.__init__')
                 if y.ndim != 1:
                     illegal_value(y.ndim, 'DataArray dimensions', 'Fit:__init__', raise_error=True)
                 self._x = np.asarray(y[y.dims[0]])
+                self._y = y
             else:
                 illegal_value(y, 'y', 'Fit:__init__', raise_error=True)
-            self._y = y
             if self._x.ndim != 1:
                 raise ValueError(f'Invalid dimension for input x ({self._x.ndim})')
             if self._x.size != self._y.size:
                 raise ValueError(f'Inconsistent x and y dimensions ({self._x.size} vs '+
                         f'{self._y.size})')
             if 'mask' in kwargs:
                 self._mask = kwargs.pop('mask')
@@ -168,14 +175,17 @@
 
     @property
     def best_results(self):
         """Convert the input data array to a data set and add the fit results.
         """
         if self._result is None:
             return(None)
+        if not have_xarray:
+            logging.warning('fit.best_results requires xarray in the conda environment')
+            return(None)
         if isinstance(self._y, xr.DataArray):
             best_results = self._y.to_dataset()
             dims = self._y.dims
             fit_name = f'{self._y.name}_fit'
         else:
             coords = {'x': (['x'], self._x)}
             dims = ('x')
@@ -268,17 +278,17 @@
     def normalization_offset(self):
         if self._result is None:
             return(None)
         if self._norm is None:
             return(0.0)
         else:
             if self._result.init_params is not None:
-                normalization_offset = self._result.init_params['tmp_normalization_offset_c']
+                normalization_offset = float(self._result.init_params['tmp_normalization_offset_c'])
             else:
-                normalization_offset = self._result.params['tmp_normalization_offset_c']
+                normalization_offset = float(self._result.params['tmp_normalization_offset_c'])
             return(normalization_offset)
 
     @property
     def num_func_eval(self):
         if self._result is None:
             return(None)
         return(self._result.nfev)
@@ -342,34 +352,34 @@
         if result is not None:
             print(result.fit_report(show_correl=show_correl))
 
     def add_parameter(self, **parameter):
         if not isinstance(parameter, dict):
             raise ValueError(f'Invalid parameter ({parameter})')
         if parameter.get('expr') is not None:
-            raise KeyError(f'Illegal "expr" key in parameter {parameter}')
+            raise KeyError(f'Invalid "expr" key in parameter {parameter}')
         name = parameter['name']
         if not isinstance(name, str):
-            raise ValueError(f'Illegal "name" value ({name}) in parameter {parameter}')
+            raise ValueError(f'Invalid "name" value ({name}) in parameter {parameter}')
         if parameter.get('norm') is None:
             self._parameter_norms[name] = False
         else:
             norm = parameter.pop('norm')
             if self._norm is None:
                 logging.warning(f'Ignoring norm in parameter {name} in '+
                             f'Fit.add_parameter (normalization is turned off)')
                 self._parameter_norms[name] = False
             else:
                 if not isinstance(norm, bool):
-                    raise ValueError(f'Illegal "norm" value ({norm}) in parameter {parameter}')
+                    raise ValueError(f'Invalid "norm" value ({norm}) in parameter {parameter}')
                 self._parameter_norms[name] = norm
         vary = parameter.get('vary')
         if vary is not None:
             if not isinstance(vary, bool):
-                raise ValueError(f'Illegal "vary" value ({vary}) in parameter {parameter}')
+                raise ValueError(f'Invalid "vary" value ({vary}) in parameter {parameter}')
             if not vary:
                 if 'min' in parameter:
                     logging.warning(f'Ignoring min in parameter {name} in '+
                             f'Fit.add_parameter (vary = {vary})')
                     parameter.pop('min')
                 if 'max' in parameter:
                     logging.warning(f'Ignoring max in parameter {name} in '+
@@ -414,37 +424,37 @@
             if parameter_norms is None:
                 if parameters is None:
                     raise ValueError('Either "parameters" or "parameter_norms" is required in '+
                             f'{model}')
                 for par in parameters:
                     name = par['name']
                     if not isinstance(name, str):
-                        raise ValueError(f'Illegal "name" value ({name}) in input parameters')
+                        raise ValueError(f'Invalid "name" value ({name}) in input parameters')
                     if par.get('norm') is not None:
                         norm = par.pop('norm')
                         if not isinstance(norm, bool):
-                            raise ValueError(f'Illegal "norm" value ({norm}) in input parameters')
+                            raise ValueError(f'Invalid "norm" value ({norm}) in input parameters')
                         new_parameter_norms[f'{pprefix}{name}'] = norm
             else:
                 for par in parameter_norms:
                     name = par['name']
                     if not isinstance(name, str):
-                        raise ValueError(f'Illegal "name" value ({name}) in input parameters')
+                        raise ValueError(f'Invalid "name" value ({name}) in input parameters')
                     norm = par.get('norm')
                     if norm is None or not isinstance(norm, bool):
-                        raise ValueError(f'Illegal "norm" value ({norm}) in input parameters')
+                        raise ValueError(f'Invalid "norm" value ({norm}) in input parameters')
                     new_parameter_norms[f'{pprefix}{name}'] = norm
             if parameters is not None:
                 for par in parameters:
                     if par.get('expr') is not None:
-                        raise KeyError(f'Illegal "expr" key ({par.get("expr")}) in parameter '+
+                        raise KeyError(f'Invalid "expr" key ({par.get("expr")}) in parameter '+
                                 f'{name} for a callable model {model}')
                     name = par['name']
                     if not isinstance(name, str):
-                        raise ValueError(f'Illegal "name" value ({name}) in input parameters')
+                        raise ValueError(f'Invalid "name" value ({name}) in input parameters')
 # RV FIX callable model will need partial deriv functions for any linear pars to get the linearized matrix, so for now skip linear solution option
             newmodel = Model(model, prefix=prefix)
         elif isinstance(model, str):
             if model == 'constant':      # Par: c
                 newmodel = ConstantModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}c'] = True
                 self._linear_parameters.append(f'{pprefix}c')
@@ -458,14 +468,24 @@
                 newmodel = QuadraticModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}a'] = True
                 new_parameter_norms[f'{pprefix}b'] = True
                 new_parameter_norms[f'{pprefix}c'] = True
                 self._linear_parameters.append(f'{pprefix}a')
                 self._linear_parameters.append(f'{pprefix}b')
                 self._linear_parameters.append(f'{pprefix}c')
+            elif model == 'polynomial': # Par: c0, c1,..., c7
+                degree = kwargs.get('degree')
+                if degree is not None:
+                    kwargs.pop('degree')
+                if degree is None or not is_int(degree, ge=0, le=7):
+                    raise ValueError(f'Invalid parameter degree for build-in step model ({degree})')
+                newmodel = PolynomialModel(degree=degree, prefix=prefix)
+                for i in range(degree+1):
+                    new_parameter_norms[f'{pprefix}c{i}'] = True
+                    self._linear_parameters.append(f'{pprefix}c{i}')
             elif model == 'gaussian':    # Par: amplitude, center, sigma (fwhm, height)
                 newmodel = GaussianModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}amplitude'] = True
                 new_parameter_norms[f'{pprefix}center'] = False
                 new_parameter_norms[f'{pprefix}sigma'] = False
                 self._linear_parameters.append(f'{pprefix}amplitude')
                 self._nonlinear_parameters.append(f'{pprefix}center')
@@ -520,31 +540,31 @@
                 self._nonlinear_parameters.append(f'{pprefix}center1')
                 self._nonlinear_parameters.append(f'{pprefix}center2')
                 self._nonlinear_parameters.append(f'{pprefix}sigma1')
                 self._nonlinear_parameters.append(f'{pprefix}sigma2')
             elif model == 'expression':  # Par: by expression
                 expr = kwargs['expr']
                 if not isinstance(expr, str):
-                    raise ValueError(f'Illegal "expr" value ({expr}) in {model}')
+                    raise ValueError(f'Invalid "expr" value ({expr}) in {model}')
                 kwargs.pop('expr')
                 if parameter_norms is not None:
                         logging.warning('Ignoring parameter_norms (normalization determined from '+
                                 'linearity)}')
                 if parameters is not None:
                     for par in parameters:
                         if par.get('expr') is not None:
-                            raise KeyError(f'Illegal "expr" key ({par.get("expr")}) in parameter '+
+                            raise KeyError(f'Invalid "expr" key ({par.get("expr")}) in parameter '+
                                     f'({par}) for an expression model')
                         if par.get('norm') is not None:
                             logging.warning(f'Ignoring "norm" key in parameter ({par}) '+
                                 '(normalization determined from linearity)}')
                             par.pop('norm')
                         name = par['name']
                         if not isinstance(name, str):
-                            raise ValueError(f'Illegal "name" value ({name}) in input parameters')
+                            raise ValueError(f'Invalid "name" value ({name}) in input parameters')
                 ast = Interpreter()
                 expr_parameters = [name for name in get_ast_names(ast.parse(expr))
                         if name != 'x' and name not in self._parameters
                         and name not in ast.symtable]
 #                print(f'\nexpr_parameters: {expr_parameters}')
 #                print(f'expr = {expr}')
                 if prefix is None:
@@ -628,15 +648,15 @@
         # Initialize the model parameters from parameters
         if prefix is None:
             prefix = ""
         if parameters is not None:
             for parameter in parameters:
                 name = parameter['name']
                 if not isinstance(name, str):
-                    raise ValueError(f'Illegal "name" value ({name}) in input parameters')
+                    raise ValueError(f'Invalid "name" value ({name}) in input parameters')
                 if name not in new_parameters:
                     name = prefix+name
                     parameter['name'] = name
                 if name not in new_parameters:
                     logging.warning(f'Ignoring superfluous parameter info for {name}')
                     continue
                 if name in self._parameters:
@@ -717,14 +737,21 @@
                 raise ValueError
 
 #        print(f'at end add_model:\nself._parameters:\n{list(self.parameters)}')
 #        print(f'at end add_model: kwargs = {kwargs}')
 #        print(f'\nat end add_model: newmodel:\n{newmodel.__dict__}\n')
         return(kwargs)
 
+    def eval(self, x, result=None):
+        if result is None:
+            result = self._result
+        if result is None:
+            return
+        return(result.eval(x=np.asarray(x))-self.normalization_offset)
+
     def fit(self, interactive=False, guess=False, **kwargs):
         # Check inputs
         if self._model is None:
             logging.error('Undefined fit model')
             return
         if not isinstance(interactive, bool):
             illegal_value(interactive, 'interactive', 'Fit.fit', raise_error=True)
@@ -793,15 +820,15 @@
                 name = par['name']
                 if name not in self._parameters:
                     raise ValueError(f'Unable to match {name} parameter {par} to an existing one')
                 if self._parameters[name].expr is not None:
                     raise ValueError(f'Unable to modify {name} parameter {par} (currently an '+
                             'expression)')
                 if par.get('expr') is not None:
-                    raise KeyError(f'Illegal "expr" key in {name} parameter {par}')
+                    raise KeyError(f'Invalid "expr" key in {name} parameter {par}')
                 self._parameters[name].set(vary=par.get('vary'))
                 self._parameters[name].set(min=par.get('min'))
                 self._parameters[name].set(max=par.get('max'))
                 self._parameters[name].set(value=par.get('value'))
 #RV            print('\nAfter adjust:')
 #RV            self._parameters.pretty_print()
 
@@ -897,16 +924,16 @@
 
         # Renormalize the data and results
         self._renormalize()
 #RV        print('\nAfter renormalization:')
 #RV        self._parameters.pretty_print()
 #        self.print_fit_report()
 
-    def plot(self, y=None, y_title=None, result=None, skip_init=False, plot_comp_legends=False,
-            plot_residual=False, plot_masked_data=True, **kwargs):
+    def plot(self, y=None, y_title=None, result=None, skip_init=False, plot_comp=True,
+            plot_comp_legends=False, plot_residual=False, plot_masked_data=True, **kwargs):
         if result is None:
             result = self._result
         if result is None:
             return
         plots = []
         legend = []
         if self._mask is None:
@@ -928,42 +955,43 @@
         if self._y is not None:
             plots += [(self._x, np.asarray(self._y), 'b.')]
             legend += ['data']
             if plot_masked_data:
                 plots += [(self._x[mask], np.asarray(self._y)[mask], 'bx')]
                 legend += ['masked data']
         if isinstance(plot_residual, bool) and plot_residual:
-            plots += [(self._x[~mask], result.residual, 'k-')]
+            plots += [(self._x[~mask], result.residual, 'r-')]
             legend += ['residual']
         plots += [(self._x[~mask], result.best_fit, 'k-')]
         legend += ['best fit']
         if not skip_init and hasattr(result, 'init_fit'):
             plots += [(self._x[~mask], result.init_fit, 'g-')]
             legend += ['init']
-        components = result.eval_components(x=self._x[~mask])
-        num_components = len(components)
-        if 'tmp_normalization_offset_' in components:
-            num_components -= 1
-        if num_components > 1:
-            eval_index = 0
-            for modelname, y in components.items():
-                if modelname == 'tmp_normalization_offset_':
-                    continue
-                if modelname == '_eval':
-                    modelname = f'eval{eval_index}'
-                if len(modelname) > 20:
-                    modelname = f'{modelname[0:16]} ...'
-                if isinstance(y, (int, float)):
-                    y *= np.ones(self._x[~mask].size)
-                plots += [(self._x[~mask], y, '--')]
-                if plot_comp_legends:
-                    if modelname[-1] == '_':
-                        legend.append(modelname[:-1])
-                    else:
-                        legend.append(modelname)
+        if plot_comp:
+            components = result.eval_components(x=self._x[~mask])
+            num_components = len(components)
+            if 'tmp_normalization_offset_' in components:
+                num_components -= 1
+            if num_components > 1:
+                eval_index = 0
+                for modelname, y in components.items():
+                    if modelname == 'tmp_normalization_offset_':
+                        continue
+                    if modelname == '_eval':
+                        modelname = f'eval{eval_index}'
+                    if len(modelname) > 20:
+                        modelname = f'{modelname[0:16]} ...'
+                    if isinstance(y, (int, float)):
+                        y *= np.ones(self._x[~mask].size)
+                    plots += [(self._x[~mask], y, '--')]
+                    if plot_comp_legends:
+                        if modelname[-1] == '_':
+                            legend.append(modelname[:-1])
+                        else:
+                            legend.append(modelname)
         title = kwargs.get('title')
         if title is not None:
             kwargs.pop('title')
         quick_plot(tuple(plots), legend=legend, title=title, block=True, **kwargs)
 
     @staticmethod
     def guess_init_peak(x, y, *args, center_guess=None, use_max_for_center=True):
@@ -1483,36 +1511,41 @@
     def __init__(self, y, x=None, normalize=True):
         super().__init__(y, x=x, normalize=normalize)
         self._fwhm_max = None
         self._sigma_max = None
 
     @classmethod
     def fit_multipeak(cls, y, centers, x=None, normalize=True, peak_models='gaussian',
-            center_exprs=None, fit_type=None, background_order=None, background_exp=False,
-            fwhm_max=None, plot_components=False):
+            center_exprs=None, fit_type=None, background=None, fwhm_max=None,
+            print_report=False, plot=False, x_eval=None):
         """Make sure that centers and fwhm_max are in the correct units and consistent with expr
            for a uniform fit (fit_type == 'uniform')
         """
+        if x_eval is not None and not isinstance(x_eval, (tuple, list, np.ndarray)):
+            raise ValueError(f'Invalid parameter x_eval ({x_eval})')
         fit = cls(y, x=x, normalize=normalize)
         success = fit.fit(centers, fit_type=fit_type, peak_models=peak_models, fwhm_max=fwhm_max,
-                center_exprs=center_exprs, background_order=background_order,
-                background_exp=background_exp, plot_components=plot_components)
+                center_exprs=center_exprs, background=background, print_report=print_report,
+                plot=plot)
+        if x_eval is None:
+            best_fit = fit.best_fit
+        else:
+            best_fit = fit.eval(x_eval)
         if success:
-            return(fit.best_fit, fit.residual, fit.best_values, fit.best_errors, fit.redchi, \
+            return(best_fit, fit.residual, fit.best_values, fit.best_errors, fit.redchi, \
                     fit.success)
         else:
             return(np.array([]), np.array([]), {}, {}, float_max, False)
 
     def fit(self, centers, fit_type=None, peak_models=None, center_exprs=None, fwhm_max=None,
-                background_order=None, background_exp=False, plot_components=False,
-                param_constraint=False):
+                background=None, print_report=False, plot=True, param_constraint=False):
         self._fwhm_max = fwhm_max
         # Create the multipeak model
-        self._create_model(centers, fit_type, peak_models, center_exprs, background_order,
-                background_exp, param_constraint)
+        self._create_model(centers, fit_type, peak_models, center_exprs, background,
+                param_constraint)
 
         # RV: Obsolete Normalize the data and results
 #        print('\nBefore fit before normalization in FitMultipeak:')
 #        self._parameters.pretty_print()
 #        self._normalize()
 #        print('\nBefore fit after normalization in FitMultipeak:')
 #        self._parameters.pretty_print()
@@ -1532,44 +1565,48 @@
         if fit_failure:
             if param_constraint:
                 logging.warning('  -> Should not happen with param_constraint set, fail the fit')
                 success = False
             else:
                 logging.info('  -> Retry fitting with constraints')
                 self.fit(centers, fit_type, peak_models, center_exprs, fwhm_max=fwhm_max,
-                        background_order=background_order, background_exp=background_exp,
-                        plot_components=plot_components, param_constraint=True)
+                        background=background, print_report=print_report, plot=plot,
+                        param_constraint=True)
         else:
             # RV: Obsolete Renormalize the data and results
 #            print('\nAfter fit before renormalization in FitMultipeak:')
 #            self._parameters.pretty_print()
 #            self.print_fit_report()
 #            self._renormalize()
 #            print('\nAfter fit after renormalization in FitMultipeak:')
 #            self._parameters.pretty_print()
 #            self.print_fit_report()
 
             # Print report and plot components if requested
-            if plot_components:
+            if print_report:
                 self.print_fit_report()
-                self.plot()
+            if plot:
+                self.plot(skip_init=True, plot_comp=True, plot_comp_legends=True,
+                        plot_residual=True)
 
         return(success)
 
     def _create_model(self, centers, fit_type=None, peak_models=None, center_exprs=None,
-                background_order=None, background_exp=False, param_constraint=False):
+                background=None, param_constraint=False):
         """Create the multipeak model
         """
         if isinstance(centers, (int, float)):
             centers = [centers]
         num_peaks = len(centers)
         if peak_models is None:
             peak_models = num_peaks*['gaussian']
-        elif isinstance(peak_models, str):
+        elif isinstance(peak_models, str) and peak_models in ('gaussian', 'lorentzian'):
             peak_models = num_peaks*[peak_models]
+        else:
+            raise ValueError(f'Invalid peak model parameter ({peak_models})')
         if len(peak_models) != num_peaks:
             raise ValueError(f'Inconsistent number of peaks in peak_models ({len(peak_models)} vs '+
                     f'{num_peaks})')
         if num_peaks == 1:
             if fit_type is not None:
                 logging.debug('Ignoring fit_type input for fitting one peak')
             fit_type = None
@@ -1598,29 +1635,29 @@
             min_value = None
 
         # Reset the fit
         self._model = None
         self._parameters = Parameters()
         self._result = None
 
-        # Add background model
-        if background_order is not None:
-            if background_order == 0:
-                self.add_model('constant', prefix='background', parameters=
-                        {'name': 'c', 'value': float_min, 'min': min_value})
-            elif background_order == 1:
-                self.add_model('linear', prefix='background', slope=0.0, intercept=0.0)
-            elif background_order == 2:
-                self.add_model('quadratic', prefix='background', a=0.0, b=0.0, c=0.0)
-            else:
-                raise ValueError(f'Invalid parameter background_order ({background_order})')
-        if background_exp:
-            self.add_model('exponential', prefix='background', parameters=(
-                        {'name': 'amplitude', 'value': float_min, 'min': min_value},
-                        {'name': 'decay', 'value': float_min, 'min': min_value}))
+        # Add background model(s)
+        if background is not None:
+            if isinstance(background, dict):
+                background = [background]
+            if isinstance(background, str):
+                self.add_model(background, prefix='bkgd_')
+            elif is_dict_series(background):
+                for model in deepcopy(background):
+                    if 'model' not in model:
+                        raise KeyError(f'Missing keyword "model" in model in background ({model})')
+                    name = model.pop('model')
+                    parameters=model.pop('parameters', None)
+                    self.add_model(name, prefix=f'bkgd_{name}_', parameters=parameters, **model)
+            else:
+                raise ValueError(f'Invalid parameter background ({background})')
 
         # Add peaks and guess initial fit parameters
         ast = Interpreter()
         if num_peaks == 1:
             height_init, cen_init, fwhm_init = self.guess_init_peak(self._x, self._y)
             if self._fwhm_max is not None and fwhm_init > self._fwhm_max:
                 fwhm_init = self._fwhm_max
@@ -1669,39 +1706,39 @@
 
     def _check_validity(self):
         """Check for valid fit parameter results
         """
         fit_failure = False
         index = compile(r'\d+')
         for name, par in self.best_parameters.items():
-            if 'background' in name:
-#                if ((name == 'backgroundc' and par['value'] <= 0.0) or
+            if 'bkgd' in name:
+#                if ((name == 'bkgd_c' and par['value'] <= 0.0) or
 #                        (name.endswith('amplitude') and par['value'] <= 0.0) or
                  if ((name.endswith('amplitude') and par['value'] <= 0.0) or
                         (name.endswith('decay') and par['value'] <= 0.0)):
                     logging.info(f'Invalid fit result for {name} ({par["value"]})')
                     fit_failure = True
             elif (((name.endswith('amplitude') or name.endswith('height')) and
                     par['value'] <= 0.0) or
                     ((name.endswith('sigma') or name.endswith('fwhm')) and par['value'] <= 0.0) or
                     (name.endswith('center') and par['value'] <= 0.0) or
                     (name == 'scale_factor' and par['value'] <= 0.0)):
                 logging.info(f'Invalid fit result for {name} ({par["value"]})')
                 fit_failure = True
-            if name.endswith('sigma') and self._sigma_max is not None:
+            if 'bkgd' not in name and name.endswith('sigma') and self._sigma_max is not None:
                 if name == 'sigma':
                     sigma_max = self._sigma_max[0]
                 else:
                     sigma_max = self._sigma_max[int(index.search(name).group())-1]
                 if par['value'] > sigma_max:
                     logging.info(f'Invalid fit result for {name} ({par["value"]})')
                     fit_failure = True
                 elif par['value'] == sigma_max:
                     logging.warning(f'Edge result on for {name} ({par["value"]})')
-            if name.endswith('fwhm') and self._fwhm_max is not None:
+            if 'bkgd' not in name and name.endswith('fwhm') and self._fwhm_max is not None:
                 if par['value'] > self._fwhm_max:
                     logging.info(f'Invalid fit result for {name} ({par["value"]})')
                     fit_failure = True
                 elif par['value'] == self._fwhm_max:
                     logging.warning(f'Edge result on for {name} ({par["value"]})')
         return(fit_failure)
 
@@ -2012,15 +2049,15 @@
         legend = [y_title]
         if plot_masked_data:
             plots += [(self._x[mask], np.asarray(self._ymap)[(*dims,mask)], 'bx')]
             legend += ['masked data']
         plots += [(self._x[~mask], self.best_fit[dims], 'k-')]
         legend += ['best fit']
         if plot_residual:
-            plots += [(self._x[~mask], self.residual[dims], 'k--')]
+            plots += [(self._x[~mask], self.residual[dims], 'r--')]
             legend += ['residual']
         # Create current parameters
         parameters = deepcopy(self._parameters)
         for name in self._best_parameters:
             if self._parameters[name].vary:
                 parameters[name].set(value=
                         self.best_values[self._best_parameters.index(name)][dims])
@@ -2124,15 +2161,15 @@
                     raise ValueError(f'Unable to match {name} parameter {par} to an existing one')
                 if self._parameters[name].expr is not None:
                     raise ValueError(f'Unable to modify {name} parameter {par} (currently an '+
                             'expression)')
                 value =  par.get('value')
                 vary =  par.get('vary')
                 if par.get('expr') is not None:
-                    raise KeyError(f'Illegal "expr" key in {name} parameter {par}')
+                    raise KeyError(f'Invalid "expr" key in {name} parameter {par}')
                 self._parameters[name].set(value=value, vary=vary, min=par.get('min'),
                         max=par.get('max'))
                 # Overwrite existing best values for fixed parameters when a value is specified
 #                print(f'best values befored resetting:\n{self._best_values}')
                 if isinstance(value, (int, float)) and vary is False:
                     for i, nname in enumerate(self._best_parameters):
                         if nname == name:
```

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/utils/material.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/material.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/utils/scanparsers.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/scanparsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,27 +509,40 @@
     def get_num_image(self, detector_prefix):
         raise(NotImplementedError)
 
 
 class FMBRotationScanParser(RotationScanParser, FMBScanParser):
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
+    def get_spec_scan_npts(self):
+        if self.spec_macro == 'flyscan':
+            if len(self.spec_args) == 2:
+                # Flat field (dark or bright)
+                return(int(self.spec_args[0])+1)
+            elif len(self.spec_args) == 5:
+                return(int(self.spec_args[3])+1)
+            else:
+                raise(RuntimeError(f'{self.scan_title}: cannot obtain number of points from '+
+                        f'{self.spec_macro} with arguments {self.spec_args}'))
+        else:
+            raise(RuntimeError(f'{self.scan_title}: cannot determine number of points for scans '+
+                    f'of type {self.spec_macro}'))
     def get_theta_vals(self):
         if self.spec_macro == 'flyscan':
             if len(self.spec_args) == 2:
                 # Flat field (dark or bright)
                 return({'num': int(self.spec_args[0])})
             elif len(self.spec_args) == 5:
                 return({'start': float(self.spec_args[1]), 'end': float(self.spec_args[2]),
                         'num': int(self.spec_args[3])+1})
             else:
                 raise(RuntimeError(f'{self.scan_title}: cannot obtain theta values from '+
                         f'{self.spec_macro} with arguments {self.spec_args}'))
         else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine scan motors for scans '+
+            raise(RuntimeError(f'{self.scan_title}: cannot determine theta values for scans '+
                     f'of type {self.spec_macro}'))
     def get_horizontal_shift(self):
         return(0.0)
     def get_vertical_shift(self):
         return(float(self.get_spec_positioner_value('4C_samz')))
     def get_starting_image_index(self):
         return(0)
@@ -574,14 +587,19 @@
         return(self.get_all_detector_data_in_file(detector_prefix, scan_step_index))
 
 
 class SMBRotationScanParser(RotationScanParser, SMBScanParser):
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
         self.par_file_pattern = f'id*-*tomo*-{self.scan_name}'
+    def get_spec_scan_npts(self):
+        if self.spec_macro == 'slew_ome' or self.spec_macro == 'rams4_slew_ome':
+            return(int(self.pars['nframes_real']))
+        else:
+            raise(RuntimeError(f'{self.scan_title}: cannot determine number of points for scans of type {self.spec_macro}'))
     def get_scan_type(self):
         try:
             return(self.pars['tomo_type'])
         except:
             try:
                 return(self.pars['tomotype'])
             except:
```

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/common/writer.py` & `ChessAnalysisPipeline-0.0.4/CHAP/common/writer.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/edd/models.py` & `ChessAnalysisPipeline-0.0.4/CHAP/edd/models.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/edd/processor.py` & `ChessAnalysisPipeline-0.0.4/CHAP/edd/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 '''
 File       : processor.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: Module for Processors used only by EDD experiments
 '''
 
 # system modules
-import argparse
 import json
-import logging
-import sys
 
 # local modules
 from CHAP.processor import Processor
 from CHAP.common import StrainAnalysisProcessor
 
 class MCACeriaCalibrationProcessor(Processor):
     '''A Processor using a CeO2 scan to obtain tuned values for the bragg
```

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/inference/processor.py` & `ChessAnalysisPipeline-0.0.4/CHAP/inference/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/pipeline.py` & `ChessAnalysisPipeline-0.0.4/CHAP/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             if hasattr(item, 'process'):
                 self.logger.info(f'Calling "process" on {item}')
                 data = item.process(data, **kwargs)
             if hasattr(item, 'write'):
                 self.logger.info(f'Calling "write" on {item}')
                 data = item.write(data, **kwargs)
 
-        self.logger.info(f'Exectuted "exectute" in {time()-t0:.3f} seconds')
+        self.logger.info(f'Executed "execute" in {time()-t0:.3f} seconds')
 
 class PipelineObject():
     """
     PipelineObject represent generic Pipeline class
     """
     def __init__(self, reader, writer, processor, fitter):
         """
```

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/processor.py` & `ChessAnalysisPipeline-0.0.4/CHAP/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/reader.py` & `ChessAnalysisPipeline-0.0.4/CHAP/reader.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/runner.py` & `ChessAnalysisPipeline-0.0.4/CHAP/runner.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/CHAP/writer.py` & `ChessAnalysisPipeline-0.0.4/CHAP/writer.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/PKG-INFO` & `ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.3/ChessAnalysisPipeline.egg-info/SOURCES.txt` & `ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 CHAP/common/reader.py
 CHAP/common/writer.py
 CHAP/common/models/__init__.py
 CHAP/common/models/integration.py
 CHAP/common/models/map.py
 CHAP/common/utils/__init__.py
 CHAP/common/utils/fit.py
+CHAP/common/utils/general.py
 CHAP/common/utils/material.py
 CHAP/common/utils/scanparsers.py
 CHAP/edd/__init__.py
 CHAP/edd/models.py
 CHAP/edd/processor.py
 CHAP/edd/reader.py
 CHAP/edd/writer.py
@@ -31,14 +32,19 @@
 CHAP/saxswaxs/processor.py
 CHAP/saxswaxs/reader.py
 CHAP/saxswaxs/writer.py
 CHAP/sin2psi/__init__.py
 CHAP/sin2psi/processor.py
 CHAP/sin2psi/reader.py
 CHAP/sin2psi/writer.py
+CHAP/tomo/__init__.py
+CHAP/tomo/models.py
+CHAP/tomo/processor.py
+CHAP/tomo/reader.py
+CHAP/tomo/writer.py
 ChessAnalysisPipeline.egg-info/PKG-INFO
 ChessAnalysisPipeline.egg-info/SOURCES.txt
 ChessAnalysisPipeline.egg-info/dependency_links.txt
 ChessAnalysisPipeline.egg-info/entry_points.txt
 ChessAnalysisPipeline.egg-info/requires.txt
 ChessAnalysisPipeline.egg-info/top_level.txt
 MLaaS/__init__.py
```

### Comparing `ChessAnalysisPipeline-0.0.3/LICENSE` & `ChessAnalysisPipeline-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/MLaaS/ktrain.py` & `ChessAnalysisPipeline-0.0.4/MLaaS/ktrain.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/MLaaS/mnist_img.py` & `ChessAnalysisPipeline-0.0.4/MLaaS/mnist_img.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/MLaaS/tfaas_client.py` & `ChessAnalysisPipeline-0.0.4/MLaaS/tfaas_client.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/PKG-INFO` & `ChessAnalysisPipeline-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.3/README.md` & `ChessAnalysisPipeline-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.3/setup.py` & `ChessAnalysisPipeline-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 to build doc : python setup.py doc
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
+version = 'v0.0.4'
+
 def datafiles(idir, pattern=None):
     """Return list of data files in provided relative dir"""
     files = []
     for dirname, dirnames, filenames in os.walk(idir):
         for subdirname in dirnames:
             files.append(os.path.join(dirname, subdirname))
         for filename in filenames:
@@ -28,15 +30,15 @@
 data_files = datafiles('examples')
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ChessAnalysisPipeline",
-    version="0.0.3",
+    version=version,
     author="Keara Soloway, Rolf Verberg, Valentin Kuznetsov",
     author_email="",
     description="CHESS analysis pipeline framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CHESSComputing/ChessAnalysisPipeline",
     packages=[
@@ -44,25 +46,27 @@
         'CHAP.common',
         'CHAP.common.models',
         'CHAP.common.utils',
         'CHAP.edd',
         'CHAP.inference',
         'CHAP.saxswaxs',
         'CHAP.sin2psi',
+        'CHAP.tomo',
         'MLaaS'
     ],
     package_dir={
         'CHAP': 'CHAP',
         'CHAP.common': 'CHAP/common',
         'CHAP.common.models': 'CHAP/common/models',
         'CHAP.common.utils': 'CHAP/common/utils',
         'CHAP.edd': 'CHAP/edd',
         'CHAP.inference': 'CHAP/inference',
         'CHAP.saxswaxs': 'CHAP/saxswaxs',
         'CHAP.sin2psi': 'CHAP/sin2psi',
+        'CHAP.tomo': 'CHAP/tomo',
         'MLaaS': 'MLaaS'
     },
     package_data={
         'examples': data_files
     },
     entry_points={
         'console_scripts': ['CHAP = CHAP.runner:main']
```

