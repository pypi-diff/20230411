# Comparing `tmp/napari_cellseg3d-0.0.2rc5.tar.gz` & `tmp/napari_cellseg3d-0.0.2rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_cellseg3d-0.0.2rc5.tar", last modified: Tue Apr 11 15:04:53 2023, max compression
+gzip compressed data, was "napari_cellseg3d-0.0.2rc6.tar", last modified: Tue Apr 11 18:25:21 2023, max compression
```

## Comparing `napari_cellseg3d-0.0.2rc5.tar` & `napari_cellseg3d-0.0.2rc6.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.996733 napari_cellseg3d-0.0.2rc5/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-11 15:04:53.996733 napari_cellseg3d-0.0.2rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.988733 napari_cellseg3d-0.0.2rc5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.988733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.992733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_model_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_plugin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_weight_download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.992733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/model_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/model_instance_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)    53334 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/model_workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.992733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_SegResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_SwinUNetR.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_TRAILMAP.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_VNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.996733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.992733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19762 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/unet/buildingblocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/unet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.992733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28064 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_model_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    40652 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_model_training.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_review_dock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.996733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/thread_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/view_brain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/view_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/weight_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    44462 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.996733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   495510 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/res/logo_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:04:53.996733 napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-11 15:04:53.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-11 15:04:53.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:04:53.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 15:04:53.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 15:04:53.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 15:04:53.000000 napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 15:04:37.000000 napari_cellseg3d-0.0.2rc5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-11 15:04:53.996733 napari_cellseg3d-0.0.2rc5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.166453 napari_cellseg3d-0.0.2rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-11 18:25:21.166453 napari_cellseg3d-0.0.2rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.154452 napari_cellseg3d-0.0.2rc6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.154452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.158452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.158452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/res/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/res/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_model_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_plugin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_weight_download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.158452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/model_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/model_instance_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53334 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/model_workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.158452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_SegResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_SwinUNetR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_TRAILMAP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_VNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.162452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.162452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19762 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/unet/buildingblocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/unet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.162452 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28064 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_model_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40652 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_model_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_review_dock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.166453 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/thread_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/view_brain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/view_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/weight_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44462 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.166453 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   495510 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/res/logo_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:21.166453 napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-11 18:25:21.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-11 18:25:21.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:25:21.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 18:25:21.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 18:25:21.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 18:25:21.000000 napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 18:24:58.000000 napari_cellseg3d-0.0.2rc6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-11 18:25:21.166453 napari_cellseg3d-0.0.2rc6/setup.cfg
```

### Comparing `napari_cellseg3d-0.0.2rc5/LICENSE` & `napari_cellseg3d-0.0.2rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/PKG-INFO` & `napari_cellseg3d-0.0.2rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_cellseg3d
-Version: 0.0.2rc5
+Version: 0.0.2rc6
 Summary: plugin for cell segmentation
 Home-page: https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
 Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.0.2rc5 Summary: plugin
+Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.0.2rc6 Summary: plugin
 for cell segmentation Home-page: https://github.com/AdaptiveMotorControlLab/
 CellSeg3d Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
 Author-email: Cyril Achard
 achard@epfl.ch>, Maxime Vidal
 vidal@epfl.ch>, Mackenzie Mathis
 post.harvard.edu> License: MIT Project-URL: Bug Tracker, https://github.com/
 AdaptiveMotorControlLab/CellSeg3d/issues Project-URL: Documentation, https://
```

### Comparing `napari_cellseg3d-0.0.2rc5/README.md` & `napari_cellseg3d-0.0.2rc6/README.md`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/docs/conf.py` & `napari_cellseg3d-0.0.2rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_dock_widget.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_model_framework.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_model_framework.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_plugin_inference.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_plugin_inference.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_review.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_review.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_training.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_training.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/_tests/test_utils.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/model_framework.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/model_framework.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/model_instance_seg.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/model_instance_seg.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/model_workers.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/model_workers.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_TRAILMAP.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_TRAILMAP.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_VNet.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_VNet.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/model_test.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/model_test.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/unet/buildingblocks.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/unet/buildingblocks.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_models/models/unet/model.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_models/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_base.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_convert.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_convert.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_crop.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_crop.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_helper.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,29 +19,31 @@
 
         self.help_url = "https://adaptivemotorcontrollab.github.io/CellSeg3d/"
 
         self.about_url = "https://wysscenter.ch/advances/3d-computer-vision-for-brain-analysis"
         self.repo_url = "https://github.com/AdaptiveMotorControlLab/CellSeg3d"
         self._viewer = viewer
 
-        path = pathlib.Path(__file__).parent.resolve()
-        url = str(path) + "../res/logo_alpha.png"
-        image = QPixmap(url)
+        logo_path = str(
+            pathlib.Path(__file__).parent.resolve() / "../res/logo_alpha.png"
+        )
+        print(logo_path)
+        image = QPixmap(logo_path)
 
         self.logo_label = ui.Button(func=lambda: ui.open_url(self.repo_url))
         self.logo_label.setIcon(QIcon(image))
         self.logo_label.setMinimumSize(200, 200)
         self.logo_label.setIconSize(QSize(200, 200))
         self.logo_label.setStyleSheet(
             "QPushButton { background-color: transparent }"
         )
         self.logo_label.setToolTip("Open Github page")
 
         self.info_label = ui.make_label(
-            f"You are using napari-cellseg3d v.{'0.0.2rc5'}\n\n"
+            f"You are using napari-cellseg3d v.{'0.0.2rc6'}\n\n"
             f"Plugin for cell segmentation developed\n"
             f"by the Mathis Lab of Adaptive Motor Control\n\n"
             f"Code by :\nCyril Achard\nMaxime Vidal\nJessy Lauer\nMackenzie Mathis\n"
             f"\nReleased under the MIT license",
             self,
         )
```

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_metrics.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_metrics.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_model_inference.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_model_inference.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_model_training.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_model_training.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_review.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_review.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_review_dock.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_review_dock.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/code_plugins/plugin_utilities.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/code_plugins/plugin_utilities.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/config.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/config.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/convert.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/convert.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/thread_test.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/thread_test.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/view_sample.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/view_sample.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/dev_scripts/weight_conversion.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/dev_scripts/weight_conversion.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/interface.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/interface.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/napari.yaml` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/plugins.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/plugins.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/res/logo_alpha.png` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/res/logo_alpha.png`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d/utils.py` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d/utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/PKG-INFO` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-cellseg3d
-Version: 0.0.2rc5
+Version: 0.0.2rc6
 Summary: plugin for cell segmentation
 Home-page: https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
 Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-cellseg3d Version: 0.0.2rc5 Summary: plugin
+Metadata-Version: 2.1 Name: napari-cellseg3d Version: 0.0.2rc6 Summary: plugin
 for cell segmentation Home-page: https://github.com/AdaptiveMotorControlLab/
 CellSeg3d Author: Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
 Author-email: Cyril Achard
 achard@epfl.ch>, Maxime Vidal
 vidal@epfl.ch>, Mackenzie Mathis
 post.harvard.edu> License: MIT Project-URL: Bug Tracker, https://github.com/
 AdaptiveMotorControlLab/CellSeg3d/issues Project-URL: Documentation, https://
```

### Comparing `napari_cellseg3d-0.0.2rc5/napari_cellseg3d.egg-info/SOURCES.txt` & `napari_cellseg3d-0.0.2rc6/napari_cellseg3d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,28 @@
 ./napari_cellseg3d/_tests/test_model_framework.py
 ./napari_cellseg3d/_tests/test_plugin_inference.py
 ./napari_cellseg3d/_tests/test_plugin_utils.py
 ./napari_cellseg3d/_tests/test_review.py
 ./napari_cellseg3d/_tests/test_training.py
 ./napari_cellseg3d/_tests/test_utils.py
 ./napari_cellseg3d/_tests/test_weight_download.py
+./napari_cellseg3d/_tests/res/test.png
 ./napari_cellseg3d/code_models/__init__.py
 ./napari_cellseg3d/code_models/model_framework.py
 ./napari_cellseg3d/code_models/model_instance_seg.py
 ./napari_cellseg3d/code_models/model_workers.py
 ./napari_cellseg3d/code_models/models/__init__.py
 ./napari_cellseg3d/code_models/models/model_SegResNet.py
 ./napari_cellseg3d/code_models/models/model_SwinUNetR.py
 ./napari_cellseg3d/code_models/models/model_TRAILMAP.py
 ./napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
 ./napari_cellseg3d/code_models/models/model_VNet.py
 ./napari_cellseg3d/code_models/models/model_test.py
 ./napari_cellseg3d/code_models/models/pretrained/__init__.py
+./napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
 ./napari_cellseg3d/code_models/models/unet/__init__.py
 ./napari_cellseg3d/code_models/models/unet/buildingblocks.py
 ./napari_cellseg3d/code_models/models/unet/model.py
 ./napari_cellseg3d/code_plugins/__init__.py
 ./napari_cellseg3d/code_plugins/plugin_base.py
 ./napari_cellseg3d/code_plugins/plugin_convert.py
 ./napari_cellseg3d/code_plugins/plugin_crop.py
@@ -55,15 +57,14 @@
 ./napari_cellseg3d/dev_scripts/convert.py
 ./napari_cellseg3d/dev_scripts/drafts.py
 ./napari_cellseg3d/dev_scripts/thread_test.py
 ./napari_cellseg3d/dev_scripts/view_brain.py
 ./napari_cellseg3d/dev_scripts/view_sample.py
 ./napari_cellseg3d/dev_scripts/weight_conversion.py
 ./napari_cellseg3d/res/__init__.py
+./napari_cellseg3d/res/logo_alpha.png
 napari_cellseg3d.egg-info/PKG-INFO
 napari_cellseg3d.egg-info/SOURCES.txt
 napari_cellseg3d.egg-info/dependency_links.txt
 napari_cellseg3d.egg-info/entry_points.txt
 napari_cellseg3d.egg-info/requires.txt
-napari_cellseg3d.egg-info/top_level.txt
-napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
-napari_cellseg3d/res/logo_alpha.png
+napari_cellseg3d.egg-info/top_level.txt
```

### Comparing `napari_cellseg3d-0.0.2rc5/pyproject.toml` & `napari_cellseg3d-0.0.2rc6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "napari_cellseg3d"
-version = "0.0.2rc5"
+version = "0.0.2rc6"
 authors = [
     {name = "Cyril Achard", email = "cyril.achard@epfl.ch"},
     {name = "Maxime Vidal", email = "maxime.vidal@epfl.ch"},
     {name = "Mackenzie Mathis", email = "mackenzie@post.harvard.edu"},
 ]
 requires-python = ">=3.8"
 dependencies = [
@@ -29,19 +29,22 @@
     "vispy>=0.9.6",
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = true
+
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.package-data]
-"*" = ["napari_cellseg3d/res/*.png", "napari_cellseg3d/code_models/models/pretrained/*.json", "*.yaml"]
+"*" = ["res/*.png", "code_models/models/pretrained/*.json", "*.yaml"]
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
 ignore = ["E501", "E741"]
 
 [tool.black]
 line-length = 79
```

### Comparing `napari_cellseg3d-0.0.2rc5/setup.cfg` & `napari_cellseg3d-0.0.2rc6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-cellseg3d
-version = 0.0.2rc5
+version = 0.0.2rc6
 author = Cyril Achard, Maxime Vidal, Jessy Lauer, Mackenzie Mathis
 author_email = cyril.achard@epfl.ch, maxime.vidal@epfl.ch, mackenzie@post.harvard.edu
 license = MIT
 description = plugin for cell segmentation
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -55,19 +55,18 @@
 	matplotlib
 	vispy>=0.9.6
 
 [options.packages.find]
 where = .
 
 [options.package_data]
-* = 
-	napari_cellseg3d/res/*.png
-	napari_cellseg3d/code_models/models/pretrained/*.json
+napari-cellseg3d = 
+	res/*.png
+	code_models/models/pretrained/*.json
 	napari.yaml
-napari-cellseg3d = napari.yaml
 
 [options.entry_points]
 napari.manifest = 
 	napari-cellseg3d = napari_cellseg3d:napari.yaml
 
 [egg_info]
 tag_build =
```

