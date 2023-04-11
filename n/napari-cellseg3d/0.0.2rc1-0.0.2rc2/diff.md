# Comparing `tmp/napari-cellseg3d-0.0.2rc1.tar.gz` & `tmp/napari_cellseg3d-0.0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-cellseg3d-0.0.2rc1.tar", last modified: Wed Mar 29 08:30:34 2023, max compression
+gzip compressed data, was "napari_cellseg3d-0.0.2rc2.tar", last modified: Tue Apr 11 10:53:10 2023, max compression
```

## Comparing `napari-cellseg3d-0.0.2rc1.tar` & `napari_cellseg3d-0.0.2rc2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.790843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.790843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_model_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_plugin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_weight_download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.790843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/model_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/model_instance_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)    53334 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/model_workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_SegResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_SwinUNetR.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_TRAILMAP.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_VNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/pretrained/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19762 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/unet/buildingblocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/unet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28064 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_model_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    40652 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_model_training.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_review_dock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/thread_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/view_brain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/view_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/weight_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    44457 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-03-29 08:30:34.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-29 08:30:34.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:30:34.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-29 08:30:34.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-29 08:30:34.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-29 08:30:34.000000 napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-29 08:30:13.000000 napari-cellseg3d-0.0.2rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-29 08:30:34.794843 napari-cellseg3d-0.0.2rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.992435 napari_cellseg3d-0.0.2rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-11 10:53:10.992435 napari_cellseg3d-0.0.2rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.984434 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.984434 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_model_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_plugin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_weight_download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.984434 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/model_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/model_instance_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53334 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/model_workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.988434 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_SegResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_SwinUNetR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_TRAILMAP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_VNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.988434 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/pretrained/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.988434 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19762 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/unet/buildingblocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/unet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.988434 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28064 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_model_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40652 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_model_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_review_dock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.992435 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/thread_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/view_brain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/view_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/weight_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44462 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.992435 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:53:10.992435 napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-11 10:53:10.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-11 10:53:10.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:53:10.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 10:53:10.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 10:53:10.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 10:53:10.000000 napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 10:52:52.000000 napari_cellseg3d-0.0.2rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-11 10:53:10.992435 napari_cellseg3d-0.0.2rc2/setup.cfg
```

### Comparing `napari-cellseg3d-0.0.2rc1/LICENSE` & `napari_cellseg3d-0.0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/PKG-INFO` & `napari_cellseg3d-0.0.2rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: napari-cellseg3d
-Version: 0.0.2rc1
+Name: napari_cellseg3d
+Version: 0.0.2rc2
 Summary: plugin for cell segmentation
 Home-page: https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
-Author-email: cyril.achard@epfl.ch, maxime.vidal@epfl.ch, mackenzie@post.harvard.edu
+Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
 Project-URL: Source Code, https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: napari
@@ -21,14 +21,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: test
 License-File: LICENSE
 
 # napari-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep learning
 
 
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/838605d0-9723-4e43-83cd-6dbfe4adf36b/cellseg-logo.png?format=1500w" title="cellseg3d" alt="cellseg3d logo" width="350" align="right" vspace = "80"/>
```

#### html2text {}

```diff
@@ -1,56 +1,58 @@
-Metadata-Version: 2.1 Name: napari-cellseg3d Version: 0.0.2rc1 Summary: plugin
+Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.0.2rc2 Summary: plugin
 for cell segmentation Home-page: https://github.com/AdaptiveMotorControlLab/
 CellSeg3d Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
-Author-email: cyril.achard@epfl.ch, maxime.vidal@epfl.ch,
-mackenzie@post.harvard.edu License: MIT Project-URL: Bug Tracker, https://
-github.com/AdaptiveMotorControlLab/CellSeg3d/issues Project-URL: Documentation,
-https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
-Project-URL: Source Code, https://github.com/AdaptiveMotorControlLab/CellSeg3d
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Science/Research Classifier: Framework :: napari Classifier: Topic ::
-Software Development :: Testing Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
-:: OS Independent Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Processing Classifier:
-Topic :: Scientific/Engineering :: Visualization Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # napari-
-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep learning
-[cellseg3d logo] [Code_style:_black] [![License: MIT](https://img.shields.io/
-badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/
-CellSeg3d/raw/main/LICENSE) [![PyPI](https://img.shields.io/pypi/v/napari-
-cellseg3d.svg?color=green)](https://pypi.org/project/napari-cellseg3d) [!
-[Python Version](https://img.shields.io/pypi/pyversions/napari-cellseg-
-annotator.svg?color=green)](https://python.org) [![codecov](https://codecov.io/
-gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/graph/
-badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/
-CellSeg3d) [![napari hub](https://img.shields.io/endpoint?url=https://
-api.napari-hub.org/shields/napari-cellseg3d)](https://www.napari-hub.org/
-plugins/napari-cellseg3d) A napari plugin for 3D cell segmentation: training,
-inference, and data review. In particular, this project was developed for
-analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets. ---------
-------------------------- ## News **June 2022: This is an alpha version, please
-expect bugs and issues, and help us make the code better by reporting them as
-an issue!** ## Installation Note : we recommend using conda to create a new
-environment for the plugin. conda create --name python=3.8 napari-cellseg3d
-conda activate napari-cellseg3d You can install `napari-cellseg3d` via [pip]:
-pip install napari-cellseg3d OR directly via [napari-hub]: - Install napari
-from pip with `pip install "napari[all]"`, then from the âPluginsâ menu
-within the napari application, select âInstall/Uninstall Package(s)...â -
-Copy `napari-cellseg3d` and paste it where it says âInstall by name/urlâ¦â
-- Click âInstallâ ## Documentation Available at https://
-AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
-running ``make html`` in the docs folder. ## Usage To use the plugin, please
-run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
-tool to use. - **Review**: This module allows you to review your labels, from
-predictions or manual labeling, and correct them if needed. It then saves the
-status of each file in a csv, for easier monitoring. - **Inference**: This
+Author-email: Cyril Achard
+achard@epfl.ch>, Maxime Vidal
+vidal@epfl.ch>, Mackenzie Mathis
+post.harvard.edu> License: MIT Project-URL: Bug Tracker, https://github.com/
+AdaptiveMotorControlLab/CellSeg3d/issues Project-URL: Documentation, https://
+adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html Project-URL:
+Source Code, https://github.com/AdaptiveMotorControlLab/CellSeg3d Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Science/
+Research Classifier: Framework :: napari Classifier: Topic :: Software
+Development :: Testing Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Operating System :: OS
+Independent Classifier: License :: OSI Approved :: MIT License Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
+Engineering :: Visualization Requires-Python: >=3.8 Description-Content-Type:
+text/markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: test
+License-File: LICENSE # napari-cellseg3D: a napari plug-in for direct 3D cell
+segmentation with deep learning [cellseg3d logo] [Code_style:_black] [!
+[License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://
+github.com/AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE) [![PyPI](https:/
+/img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/
+project/napari-cellseg3d) [![Python Version](https://img.shields.io/pypi/
+pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org) [!
+[codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/
+graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/
+AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
+endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
+www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
+segmentation: training, inference, and data review. In particular, this project
+was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
+datasets. ---------------------------------- ## News **June 2022: This is an
+alpha version, please expect bugs and issues, and help us make the code better
+by reporting them as an issue!** ## Installation Note : we recommend using
+conda to create a new environment for the plugin. conda create --name
+python=3.8 napari-cellseg3d conda activate napari-cellseg3d You can install
+`napari-cellseg3d` via [pip]: pip install napari-cellseg3d OR directly via
+[napari-hub]: - Install napari from pip with `pip install "napari[all]"`, then
+from the âPluginsâ menu within the napari application, select âInstall/
+Uninstall Package(s)...â - Copy `napari-cellseg3d` and paste it where it says
+âInstall by name/urlâ¦â - Click âInstallâ ## Documentation Available
+at https://AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate
+docs by running ``make html`` in the docs folder. ## Usage To use the plugin,
+please run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose
+which tool to use. - **Review**: This module allows you to review your labels,
+from predictions or manual labeling, and correct them if needed. It then saves
+the status of each file in a csv, for easier monitoring. - **Inference**: This
 module allows you to use pre-trained segmentation algorithms on volumes to
 automatically label cells and compute statistics. - **Train**: This module
 allows you to train segmentation algorithms from labeled volumes. -
 **Utilities**: This module allows you to perform several actions like cropping
 your volumes and labels dynamically, by selecting a fixed size volume and
 moving it around the image; computing prediction scores from ground truth and
 predicition labels; or converting labels from instance to segmentation and the
```

### Comparing `napari-cellseg3d-0.0.2rc1/README.md` & `napari_cellseg3d-0.0.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_dock_widget.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_model_framework.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_model_framework.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_plugin_inference.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_plugin_inference.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_review.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_review.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_training.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_training.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/_tests/test_utils.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/model_framework.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/model_framework.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/model_instance_seg.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/model_instance_seg.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/model_workers.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/model_workers.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_TRAILMAP.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_TRAILMAP.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_VNet.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_VNet.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/model_test.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/model_test.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/unet/buildingblocks.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/unet/buildingblocks.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_models/models/unet/model.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_models/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_base.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_convert.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_convert.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_crop.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_crop.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_helper.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.logo_label.setIconSize(QSize(200, 200))
         self.logo_label.setStyleSheet(
             "QPushButton { background-color: transparent }"
         )
         self.logo_label.setToolTip("Open Github page")
 
         self.info_label = ui.make_label(
-            f"You are using napari-cellseg3d v.{'0.0.2rc1'}\n\n"
+            f"You are using napari-cellseg3d v.{'0.0.2rc2'}\n\n"
             f"Plugin for cell segmentation developed\n"
             f"by the Mathis Lab of Adaptive Motor Control\n\n"
             f"Code by :\nCyril Achard\nMaxime Vidal\nJessy Lauer\nMackenzie Mathis\n"
             f"\nReleased under the MIT license",
             self,
         )
```

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_metrics.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_metrics.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_model_inference.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_model_inference.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_model_training.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_model_training.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_review.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_review.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_review_dock.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_review_dock.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/code_plugins/plugin_utilities.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/code_plugins/plugin_utilities.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/config.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/config.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/convert.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/convert.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/thread_test.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/thread_test.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/view_sample.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/view_sample.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/dev_scripts/weight_conversion.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/dev_scripts/weight_conversion.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/interface.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,15 +577,15 @@
     def slider_value(self, value: int):
         """Set a value (int) divided by self._divide_factor"""
         if value < self.minimum() or value > self.maximum():
             raise ValueError(
                 f"The value for the slider ({value}) cannot be out of ({self.minimum()};{self.maximum()}) "
             )
 
-        self.setValue(value)
+        self.setValue(int(value))
 
         divided = value / self._divide_factor
         if self._divide_factor == 1.0:
             divided = int(divided)
         self._value_label.setText(str(divided))
```

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/napari.yaml` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/plugins.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/plugins.py`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d/utils.py` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from skimage import io
 from skimage.filters import gaussian
 from tifffile import imread as tfl_imread
 
 LOGGER = logging.getLogger(__name__)
 ###############
 # Global logging level setting
-LOGGER.setLevel(logging.DEBUG)
-# LOGGER.setLevel(logging.INFO)
+# LOGGER.setLevel(logging.DEBUG)
+LOGGER.setLevel(logging.INFO)
 ###############
 
 """
 utils.py
 ====================================
 Definitions of utility functions, classes, and variables
 """
@@ -157,15 +157,15 @@
         origins.append(diffs["origin"])
         targets.append(diffs["target"])
 
     reverse_mapping = {0: (-3), 1: (-2), 2: (-1)}
     for i in range(len(targets)):
         targets[i] = reverse_mapping[targets[i]]
     infos = np.unique(origins, return_index=True, return_counts=True)
-    info_dict = {"origins": infos[0], "index": infos[1], "counts": infos[2]}
+    {"origins": infos[0], "index": infos[1], "counts": infos[2]}
     # print(info_dict)
 
     final_orig = []
     final_targ = []
     for i in range(len(infos[0])):
         if infos[2][i] == 1:
             final_orig.append(infos[0][i])
```

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/PKG-INFO` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: napari-cellseg3d
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: plugin for cell segmentation
 Home-page: https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
-Author-email: cyril.achard@epfl.ch, maxime.vidal@epfl.ch, mackenzie@post.harvard.edu
+Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
 Project-URL: Source Code, https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: napari
@@ -21,14 +21,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: test
 License-File: LICENSE
 
 # napari-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep learning
 
 
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/838605d0-9723-4e43-83cd-6dbfe4adf36b/cellseg-logo.png?format=1500w" title="cellseg3d" alt="cellseg3d logo" width="350" align="right" vspace = "80"/>
```

#### html2text {}

```diff
@@ -1,56 +1,58 @@
-Metadata-Version: 2.1 Name: napari-cellseg3d Version: 0.0.2rc1 Summary: plugin
+Metadata-Version: 2.1 Name: napari-cellseg3d Version: 0.0.2rc2 Summary: plugin
 for cell segmentation Home-page: https://github.com/AdaptiveMotorControlLab/
 CellSeg3d Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
-Author-email: cyril.achard@epfl.ch, maxime.vidal@epfl.ch,
-mackenzie@post.harvard.edu License: MIT Project-URL: Bug Tracker, https://
-github.com/AdaptiveMotorControlLab/CellSeg3d/issues Project-URL: Documentation,
-https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
-Project-URL: Source Code, https://github.com/AdaptiveMotorControlLab/CellSeg3d
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Science/Research Classifier: Framework :: napari Classifier: Topic ::
-Software Development :: Testing Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
-:: OS Independent Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Processing Classifier:
-Topic :: Scientific/Engineering :: Visualization Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # napari-
-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep learning
-[cellseg3d logo] [Code_style:_black] [![License: MIT](https://img.shields.io/
-badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/
-CellSeg3d/raw/main/LICENSE) [![PyPI](https://img.shields.io/pypi/v/napari-
-cellseg3d.svg?color=green)](https://pypi.org/project/napari-cellseg3d) [!
-[Python Version](https://img.shields.io/pypi/pyversions/napari-cellseg-
-annotator.svg?color=green)](https://python.org) [![codecov](https://codecov.io/
-gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/graph/
-badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/
-CellSeg3d) [![napari hub](https://img.shields.io/endpoint?url=https://
-api.napari-hub.org/shields/napari-cellseg3d)](https://www.napari-hub.org/
-plugins/napari-cellseg3d) A napari plugin for 3D cell segmentation: training,
-inference, and data review. In particular, this project was developed for
-analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets. ---------
-------------------------- ## News **June 2022: This is an alpha version, please
-expect bugs and issues, and help us make the code better by reporting them as
-an issue!** ## Installation Note : we recommend using conda to create a new
-environment for the plugin. conda create --name python=3.8 napari-cellseg3d
-conda activate napari-cellseg3d You can install `napari-cellseg3d` via [pip]:
-pip install napari-cellseg3d OR directly via [napari-hub]: - Install napari
-from pip with `pip install "napari[all]"`, then from the âPluginsâ menu
-within the napari application, select âInstall/Uninstall Package(s)...â -
-Copy `napari-cellseg3d` and paste it where it says âInstall by name/urlâ¦â
-- Click âInstallâ ## Documentation Available at https://
-AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
-running ``make html`` in the docs folder. ## Usage To use the plugin, please
-run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
-tool to use. - **Review**: This module allows you to review your labels, from
-predictions or manual labeling, and correct them if needed. It then saves the
-status of each file in a csv, for easier monitoring. - **Inference**: This
+Author-email: Cyril Achard
+achard@epfl.ch>, Maxime Vidal
+vidal@epfl.ch>, Mackenzie Mathis
+post.harvard.edu> License: MIT Project-URL: Bug Tracker, https://github.com/
+AdaptiveMotorControlLab/CellSeg3d/issues Project-URL: Documentation, https://
+adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html Project-URL:
+Source Code, https://github.com/AdaptiveMotorControlLab/CellSeg3d Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Science/
+Research Classifier: Framework :: napari Classifier: Topic :: Software
+Development :: Testing Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Operating System :: OS
+Independent Classifier: License :: OSI Approved :: MIT License Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
+Engineering :: Visualization Requires-Python: >=3.8 Description-Content-Type:
+text/markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: test
+License-File: LICENSE # napari-cellseg3D: a napari plug-in for direct 3D cell
+segmentation with deep learning [cellseg3d logo] [Code_style:_black] [!
+[License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://
+github.com/AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE) [![PyPI](https:/
+/img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/
+project/napari-cellseg3d) [![Python Version](https://img.shields.io/pypi/
+pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org) [!
+[codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/
+graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/
+AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
+endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
+www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
+segmentation: training, inference, and data review. In particular, this project
+was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
+datasets. ---------------------------------- ## News **June 2022: This is an
+alpha version, please expect bugs and issues, and help us make the code better
+by reporting them as an issue!** ## Installation Note : we recommend using
+conda to create a new environment for the plugin. conda create --name
+python=3.8 napari-cellseg3d conda activate napari-cellseg3d You can install
+`napari-cellseg3d` via [pip]: pip install napari-cellseg3d OR directly via
+[napari-hub]: - Install napari from pip with `pip install "napari[all]"`, then
+from the âPluginsâ menu within the napari application, select âInstall/
+Uninstall Package(s)...â - Copy `napari-cellseg3d` and paste it where it says
+âInstall by name/urlâ¦â - Click âInstallâ ## Documentation Available
+at https://AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate
+docs by running ``make html`` in the docs folder. ## Usage To use the plugin,
+please run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose
+which tool to use. - **Review**: This module allows you to review your labels,
+from predictions or manual labeling, and correct them if needed. It then saves
+the status of each file in a csv, for easier monitoring. - **Inference**: This
 module allows you to use pre-trained segmentation algorithms on volumes to
 automatically label cells and compute statistics. - **Train**: This module
 allows you to train segmentation algorithms from labeled volumes. -
 **Utilities**: This module allows you to perform several actions like cropping
 your volumes and labels dynamically, by selecting a fixed size volume and
 moving it around the image; computing prediction scores from ground truth and
 predicition labels; or converting labels from instance to segmentation and the
```

### Comparing `napari-cellseg3d-0.0.2rc1/napari_cellseg3d.egg-info/SOURCES.txt` & `napari_cellseg3d-0.0.2rc2/napari_cellseg3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-cellseg3d-0.0.2rc1/setup.cfg` & `napari_cellseg3d-0.0.2rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-cellseg3d
-version = 0.0.2rc1
+version = 0.0.2rc2
 author = Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
 author_email = cyril.achard@epfl.ch, maxime.vidal@epfl.ch, mackenzie@post.harvard.edu
 license = MIT
 description = plugin for cell segmentation
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

