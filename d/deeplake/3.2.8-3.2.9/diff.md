# Comparing `tmp/deeplake-3.2.8.tar.gz` & `tmp/deeplake-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.2.8.tar", last modified: Thu Feb 16 12:44:01 2023, max compression
+gzip compressed data, was "deeplake-3.2.9.tar", last modified: Mon Feb 20 14:49:33 2023, max compression
```

## Comparing `deeplake-3.2.8.tar` & `deeplake-3.2.9.tar`

### file list

```diff
@@ -1,352 +1,351 @@
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.453156 deeplake-3.2.8/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       36 2023-02-16 12:43:15.000000 deeplake-3.2.8/MANIFEST.in
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    24618 2023-02-16 12:44:01.453777 deeplake-3.2.8/PKG-INFO
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    20858 2023-02-16 12:43:15.000000 deeplake-3.2.8/README.md
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.275561 deeplake-3.2.8/deeplake/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2657 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.281675 deeplake-3.2.8/deeplake/api/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    77042 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4701 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/info.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1203 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1698 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/link_tiled.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2703 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/read.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.296499 deeplake-3.2.8/deeplake/api/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3038 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2098 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    77701 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_api.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6439 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    11715 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2654 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1797 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2997 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1500 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6192 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      953 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_events.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5218 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      247 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6514 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_info.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6911 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6823 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_json.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    21293 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3223 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1789 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_linking.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1024 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1235 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_meta.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3951 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6352 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_none.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      952 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1605 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5750 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3308 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    10121 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_pop.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1228 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    16842 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4578 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2331 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_text.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    14194 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7289 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_video.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3499 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tests/test_views.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1368 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/api/tiled.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.296781 deeplake-3.2.8/deeplake/auto/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.297346 deeplake-3.2.8/deeplake/auto/structured/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/structured/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      635 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/structured/base.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2229 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.298695 deeplake-3.2.8/deeplake/auto/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6951 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6135 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5371 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5117 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.302353 deeplake-3.2.8/deeplake/auto/unstructured/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      537 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.303782 deeplake-3.2.8/deeplake/auto/unstructured/coco/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6963 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      669 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1709 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5184 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6575 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3533 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4514 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.305109 deeplake-3.2.8/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      278 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7346 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    12793 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.306466 deeplake-3.2.8/deeplake/cli/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/cli/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5027 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/cli/auth.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      498 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/cli/commands.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      435 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/cli/list_datasets.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1482 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/cli/test_cli.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.308389 deeplake-3.2.8/deeplake/client/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/client/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    17771 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/client/client.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1280 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/client/config.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      690 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/client/log.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1736 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/client/test_client.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3293 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/client/utils.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3872 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5350 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/constants.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.322901 deeplake-3.2.8/deeplake/core/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       23 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.326511 deeplake-3.2.8/deeplake/core/chunk/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    23752 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    25277 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6168 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4926 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4494 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5446 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     9598 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)   100107 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/chunk_engine.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    38985 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/compression.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.328409 deeplake-3.2.8/deeplake/core/compute/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/compute/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      911 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/compute/process.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2243 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/compute/provider.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      640 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/compute/ray.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      742 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/compute/serial.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      576 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/compute/thread.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.333510 deeplake-3.2.8/deeplake/core/dataset/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/dataset/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)   160789 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/dataset/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13657 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      760 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4031 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4242 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.334798 deeplake-3.2.8/deeplake/core/index/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      138 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/index/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    17507 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/index/index.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18555 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/io.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4121 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/ipc.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     9825 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/link_creds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    16161 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1971 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/linked_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2677 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     9763 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/lock.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.336429 deeplake-3.2.8/deeplake/core/meta/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       97 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3595 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.339377 deeplake-3.2.8/deeplake/core/meta/encode/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    25591 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3915 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13495 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1551 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      941 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      683 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.341401 deeplake-3.2.8/deeplake/core/meta/encode/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      226 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2237 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1452 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2114 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3673 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2810 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7515 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      503 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/meta.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13358 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      906 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/partial_reader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      961 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/partial_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5003 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/polygon.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.342698 deeplake-3.2.8/deeplake/core/query/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       82 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/query/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    12021 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/query/autocomplete.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    14324 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/query/filter.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     8905 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/query/query.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    19656 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    22548 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.346519 deeplake-3.2.8/deeplake/core/storage/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      382 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      929 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18306 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/gcs.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    12815 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/google_drive.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     8273 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/local.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18687 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3526 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/memory.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6549 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/provider.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    22659 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/storage/s3.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    47714 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tensor.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7191 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tensor_link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5152 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/test_serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.349380 deeplake-3.2.8/deeplake/core/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7544 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tests/test_compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      691 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tests/test_compute.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      913 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tests/test_io.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4209 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tests/test_locking.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      654 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1425 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.351889 deeplake-3.2.8/deeplake/core/tiling/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tiling/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4547 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1701 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4731 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2893 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tiling/serialize.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1950 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2367 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.361077 deeplake-3.2.8/deeplake/core/transform/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      111 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/transform/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    38044 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/transform/test_transform.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    24687 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/transform/transform.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1560 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6267 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.367184 deeplake-3.2.8/deeplake/core/version_control/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/version_control/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1954 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5774 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2068 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4828 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    18757 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    82757 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.377757 deeplake-3.2.8/deeplake/enterprise/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      257 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5698 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    27064 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/dataloader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3892 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    21065 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1664 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/test_query.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    22446 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1595 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/enterprise/util.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1590 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/hooks.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4617 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/htype.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.379716 deeplake-3.2.8/deeplake/integrations/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       99 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/__init__.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.381510 deeplake-3.2.8/deeplake/integrations/huggingface/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       44 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4100 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.384078 deeplake-3.2.8/deeplake/integrations/mmdet/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      118 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    59631 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    19171 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.386276 deeplake-3.2.8/deeplake/integrations/pytorch/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       40 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4937 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    16740 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4994 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5010 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.387602 deeplake-3.2.8/deeplake/integrations/tf/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      135 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1224 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/tf/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2423 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5330 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.388253 deeplake-3.2.8/deeplake/integrations/wandb/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       21 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    11856 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.389313 deeplake-3.2.8/deeplake/requirements/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      294 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/requirements/common.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       71 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/requirements/docs.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      357 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/requirements/plugins.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      179 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/requirements/tests.txt
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.391214 deeplake-3.2.8/deeplake/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1404 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2547 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/tests/client_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3931 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/tests/common.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3357 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    14022 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/tests/path_fixtures.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2248 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.442598 deeplake-3.2.8/deeplake/util/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       86 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3499 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/access_method.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      971 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/agreement.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1567 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/array_list.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      619 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2961 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/auto.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5329 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/bugout_reporter.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       54 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/bugout_token.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3606 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/cache_chain.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4435 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/casting.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      310 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/check_installation.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1197 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/check_latest_version.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3172 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/chunk_engine.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4534 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/class_label.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      231 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/compression.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1197 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/compute.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     5381 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/connect_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      351 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/creds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      775 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      443 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/delete_entry.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    15912 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/diff.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4638 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/downsample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       84 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/empty_sample.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    13964 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/encoder.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    28248 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/exceptions.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2026 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/exif.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1813 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/from_tfds.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      136 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/generate_id.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      306 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/hash.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2799 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/htype.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1517 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/image.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      873 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/invalid_view_op.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      154 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1001 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/iteration_warning.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      507 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/join_chunks.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6422 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/json.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6644 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/keys.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2949 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/link.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1646 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/logging.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    35704 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/merge.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2426 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/modified.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/notebook.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.447892 deeplake-3.2.8/deeplake/util/object_3d/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3374 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      185 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      185 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1021 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      695 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1323 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6188 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1663 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3221 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    10213 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     7187 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1160 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3669 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/path.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3337 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/pretty_print.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2638 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/remove_cache.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     4007 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/scheduling.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2892 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/shape_interval.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      182 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/shuffle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1153 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/split.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6762 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/storage.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1131 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tag.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      354 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/testing.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.451522 deeplake-3.2.8/deeplake/util/tests/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1476 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_auto.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1757 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1239 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      892 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_read.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     1071 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      407 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      698 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_split.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      266 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_token.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     2428 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      276 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/threading.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      381 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/token.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    19448 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/transform.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    23486 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/version_control.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      927 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/video.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      167 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/util/warnings.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.452750 deeplake-3.2.8/deeplake/visualizer/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       34 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/visualizer/__init__.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6466 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     6680 2023-02-16 12:43:15.000000 deeplake-3.2.8/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-16 12:44:01.278256 deeplake-3.2.8/deeplake.egg-info/
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    24618 2023-02-16 12:44:01.000000 deeplake-3.2.8/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 abhinavtuli   (501) admin       (80)    10572 2023-02-16 12:44:01.000000 deeplake-3.2.8/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-16 12:44:01.000000 deeplake-3.2.8/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)       58 2023-02-16 12:44:01.000000 deeplake-3.2.8/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-16 12:44:01.000000 deeplake-3.2.8/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-16 12:44:01.000000 deeplake-3.2.8/deeplake.egg-info/requires.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)        9 2023-02-16 12:44:01.000000 deeplake-3.2.8/deeplake.egg-info/top_level.txt
--rw-r--r--   0 abhinavtuli   (501) admin       (80)      311 2023-02-16 12:44:01.454664 deeplake-3.2.8/setup.cfg
--rw-r--r--   0 abhinavtuli   (501) admin       (80)     3329 2023-02-16 12:43:15.000000 deeplake-3.2.8/setup.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.205627 deeplake-3.2.9/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       36 2023-02-20 14:48:58.000000 deeplake-3.2.9/MANIFEST.in
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    24618 2023-02-20 14:49:33.206317 deeplake-3.2.9/PKG-INFO
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    20858 2023-02-20 14:48:58.000000 deeplake-3.2.9/README.md
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.078952 deeplake-3.2.9/deeplake/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2632 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/__init__.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.083572 deeplake-3.2.9/deeplake/api/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    76117 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4701 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/info.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1203 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/link.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1698 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/link_tiled.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2703 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/read.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.096909 deeplake-3.2.9/deeplake/api/tests/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3038 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2098 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    78746 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_api.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6439 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    11715 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2654 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1797 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2997 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1500 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6192 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      953 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_events.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5218 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      247 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6514 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_info.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6911 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6823 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_json.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    21293 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_link.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3223 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1789 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1024 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1235 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3951 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6352 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_none.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      952 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1605 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5750 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3308 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    10121 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1228 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    17553 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4578 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2331 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_text.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    14194 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     7289 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_video.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3068 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tests/test_views.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1368 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/api/tiled.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.097162 deeplake-3.2.9/deeplake/auto/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/__init__.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.097829 deeplake-3.2.9/deeplake/auto/structured/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      635 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/structured/base.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2229 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.099290 deeplake-3.2.9/deeplake/auto/tests/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6951 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6135 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5371 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5117 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.101429 deeplake-3.2.9/deeplake/auto/unstructured/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      537 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.103091 deeplake-3.2.9/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6963 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      669 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1709 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5184 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6575 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3533 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4514 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.105469 deeplake-3.2.9/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      278 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     7346 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    12793 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.108383 deeplake-3.2.9/deeplake/cli/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5741 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/auth.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      410 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/commands.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      931 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/cli/test_cli.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.110464 deeplake-3.2.9/deeplake/client/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    17015 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/client.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1245 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/config.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      690 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/log.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1536 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/test_client.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3293 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/client/utils.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3872 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/compression.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5350 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/constants.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.121952 deeplake-3.2.9/deeplake/core/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       23 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/__init__.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.126452 deeplake-3.2.9/deeplake/core/chunk/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    23752 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    25277 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6168 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4926 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4494 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5446 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     9598 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)   100393 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/chunk_engine.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    38985 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compression.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.128979 deeplake-3.2.9/deeplake/core/compute/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      911 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/process.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2243 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/provider.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      640 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/ray.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      742 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/serial.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      576 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/compute/thread.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.134867 deeplake-3.2.9/deeplake/core/dataset/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)   160825 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    13657 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      760 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4031 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4242 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.135595 deeplake-3.2.9/deeplake/core/index/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      138 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/index/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    17507 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/index/index.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    18555 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/io.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4121 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/ipc.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     9825 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/link_creds.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    16161 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1971 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/linked_sample.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2677 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     9763 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/lock.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.137228 deeplake-3.2.9/deeplake/core/meta/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       97 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3595 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.139880 deeplake-3.2.9/deeplake/core/meta/encode/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    25591 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3915 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    13495 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1551 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      941 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      683 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.142207 deeplake-3.2.9/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      226 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2237 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1452 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2114 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3673 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2810 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     7515 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      503 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/meta.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    13358 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      906 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/partial_reader.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      961 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/partial_sample.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5003 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/polygon.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.143676 deeplake-3.2.9/deeplake/core/query/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       82 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    12021 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    14324 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/filter.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     8905 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/query/query.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    19656 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/sample.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    22548 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/serialize.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.148200 deeplake-3.2.9/deeplake/core/storage/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      382 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      929 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    18306 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/gcs.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    12815 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     8273 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/local.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    18687 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3526 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/memory.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6549 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/provider.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    22659 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/storage/s3.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    47714 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tensor.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     7191 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tensor_link.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5152 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/test_serialize.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.151251 deeplake-3.2.9/deeplake/core/tests/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     7544 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      691 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      913 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_io.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4209 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      654 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1425 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.153305 deeplake-3.2.9/deeplake/core/tiling/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4547 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1701 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4731 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2893 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1950 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2367 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.155973 deeplake-3.2.9/deeplake/core/transform/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      111 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    39500 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    24686 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/transform.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1560 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6267 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.158520 deeplake-3.2.9/deeplake/core/version_control/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1954 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5774 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2068 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4828 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    18757 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    82757 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.164086 deeplake-3.2.9/deeplake/enterprise/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      257 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5698 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    27064 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3892 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    21065 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1664 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/test_query.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    22446 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1595 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/enterprise/util.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1590 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/hooks.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4617 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/htype.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.164441 deeplake-3.2.9/deeplake/integrations/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       99 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/__init__.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.165111 deeplake-3.2.9/deeplake/integrations/huggingface/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       44 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4100 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.166735 deeplake-3.2.9/deeplake/integrations/mmdet/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      118 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    59631 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    19171 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.168899 deeplake-3.2.9/deeplake/integrations/pytorch/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       40 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4937 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    16740 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4994 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5010 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.170319 deeplake-3.2.9/deeplake/integrations/tf/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      135 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1224 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/common.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2423 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5330 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.170924 deeplake-3.2.9/deeplake/integrations/wandb/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       21 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    11856 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.172026 deeplake-3.2.9/deeplake/requirements/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      294 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/common.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       71 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/docs.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      357 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/plugins.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      179 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/requirements/tests.txt
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.174083 deeplake-3.2.9/deeplake/tests/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1404 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2547 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3931 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/common.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3357 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    14022 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2248 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.194915 deeplake-3.2.9/deeplake/util/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       86 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3499 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/access_method.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      971 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/agreement.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1567 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/array_list.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      619 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2961 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/auto.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5329 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       54 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/bugout_token.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3606 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/cache_chain.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4435 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/casting.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      310 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/check_installation.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1197 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/check_latest_version.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3172 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/chunk_engine.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4534 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/class_label.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      231 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/compression.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1197 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/compute.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     5381 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/connect_dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      351 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/creds.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      775 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      443 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/delete_entry.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    15912 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/diff.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4638 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/downsample.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       84 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/empty_sample.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    13964 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/encoder.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    28248 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/exceptions.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2026 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/exif.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1813 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/from_tfds.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      136 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/generate_id.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      306 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/hash.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2799 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/htype.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1517 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/image.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      873 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      154 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1001 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/iteration_warning.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      507 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/join_chunks.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6422 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/json.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6644 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/keys.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2949 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/link.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1646 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/logging.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    35704 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/merge.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2426 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/modified.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/notebook.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.201283 deeplake-3.2.9/deeplake/util/object_3d/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3374 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      185 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      185 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1021 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      695 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1323 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6188 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1663 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3221 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    10213 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     7187 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1160 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3669 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/path.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3337 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/pretty_print.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2682 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/remove_cache.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     4007 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/scheduling.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2892 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/shape_interval.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      182 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/shuffle.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1153 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/split.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6762 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/storage.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1131 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tag.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      354 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/testing.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.204328 deeplake-3.2.9/deeplake/util/tests/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1476 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1757 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1239 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      892 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_read.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     1071 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      407 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      698 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_split.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      266 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_token.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     2428 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      276 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/threading.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      381 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/token.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    19516 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/transform.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    23486 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/version_control.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      927 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/video.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      167 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/util/warnings.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.205289 deeplake-3.2.9/deeplake/visualizer/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       34 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/visualizer/__init__.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6466 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     6680 2023-02-20 14:48:58.000000 deeplake-3.2.9/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 abhinavtuli   (501) admin       (80)        0 2023-02-20 14:49:33.080690 deeplake-3.2.9/deeplake.egg-info/
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    24618 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)    10542 2023-02-20 14:49:33.000000 deeplake-3.2.9/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)       58 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        1 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      903 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/requires.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)        9 2023-02-20 14:49:32.000000 deeplake-3.2.9/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)      311 2023-02-20 14:49:33.207116 deeplake-3.2.9/setup.cfg
+-rw-r--r--   0 abhinavtuli   (501) admin       (80)     3329 2023-02-20 14:48:58.000000 deeplake-3.2.9/setup.py
```

### Comparing `deeplake-3.2.8/PKG-INFO` & `deeplake-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.2.8
+Version: 3.2.9
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.2.8 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.2.9 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Description: [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-
 b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
              ****** Deep Lake: Data Lake for Deep Learning ******
```

### Comparing `deeplake-3.2.8/README.md` & `deeplake-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/__init__.py` & `deeplake-3.2.9/deeplake/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 r"""
-The deeplake package provides a database which stores data as compressed chunked arrays that can be stored anywhere and 
+The deeplake package provides a database which stores data as compressed chunked arrays that can be stored anywhere and
 later streamed to deep learning models.
 """
 
 import threading
 from queue import Queue
 from botocore.config import Config
 import numpy as np
@@ -29,15 +29,14 @@
 from .htype import HTYPE_CONFIGURATIONS
 from .htype import htype
 from .integrations import huggingface
 from .integrations import wandb
 
 compressions = list(SUPPORTED_COMPRESSIONS)
 htypes = sorted(list(HTYPE_CONFIGURATIONS))
-list = api_dataset.list
 exists = api_dataset.exists
 load = api_dataset.load
 empty = api_dataset.empty
 like = api_dataset.like
 delete = api_dataset.delete
 rename = api_dataset.rename
 copy = api_dataset.copy
@@ -76,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.2.8"
+__version__ = "3.2.9"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.2.8/deeplake/api/dataset.py` & `deeplake-3.2.9/deeplake/api/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1519,33 +1519,7 @@
             ds = dest
         else:
             dest = convert_pathlib_to_string_if_needed(dest)
             ds = deeplake.dataset(dest, creds=dest_creds, **dataset_kwargs)
 
         structured.fill_dataset(ds, progressbar)  # type: ignore
         return ds  # type: ignore
-
-    @staticmethod
-    def list(
-        org_id: str = "",
-        token: Optional[str] = None,
-    ) -> None:
-        """List all available Deep Lake cloud datasets.
-
-        Args:
-            org_id (str): Specify organization id. If not given,
-                returns a list of all datasets that can be accessed, regardless of what workspace they are in.
-                Otherwise, lists all datasets in the given organization.
-            token (str, optional): Activeloop token, used for fetching credentials for Deep Lake datasets. This is optional, tokens are normally autogenerated.
-
-        Returns:
-            List: List of dataset names.
-        """
-
-        deeplake_reporter.feature_report(
-            feature_name="list",
-            parameters={"org_id": org_id},
-        )
-
-        client = DeepLakeBackendClient(token=token)
-        datasets = client.get_datasets(workspace=org_id)
-        return datasets
```

### Comparing `deeplake-3.2.8/deeplake/api/info.py` & `deeplake-3.2.9/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/link.py` & `deeplake-3.2.9/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/link_tiled.py` & `deeplake-3.2.9/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/read.py` & `deeplake-3.2.9/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_access_method.py` & `deeplake-3.2.9/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_agreement.py` & `deeplake-3.2.9/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_api.py` & `deeplake-3.2.9/deeplake/api/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2127,14 +2127,15 @@
 ):
     result = runner.invoke(login, f"-u {username} -p {password}")
     with pytest.raises(TokenPermissionError):
         deeplake.empty("hub://activeloop-test/sohas-weapons-train")
 
     with pytest.raises(TokenPermissionError):
         ds = deeplake.load("hub://activeloop/fake-path")
+    runner.invoke(logout)
 
 
 def invalid_token_exception_check():
     with pytest.raises(InvalidTokenException):
         ds = deeplake.empty("hub://adilkhan/demo", token="invalid_token")
 
 
@@ -2150,14 +2151,15 @@
         ds = deeplake.empty("hub://adilkhan/demo")
 
 
 def dataset_handler_error_check(runner, username, password):
     result = runner.invoke(login, f"-u {username} -p {password}")
     with pytest.raises(DatasetHandlerError):
         ds = deeplake.load(f"hub://{username}/wrong-path")
+    runner.invoke(logout)
 
 
 def test_hub_related_permission_exceptions(
     hub_cloud_dev_credentials, hub_cloud_dev_token, hub_dev_token
 ):
     username, password = hub_cloud_dev_credentials
     runner = CliRunner()
@@ -2374,14 +2376,54 @@
 
     with pytest.raises(TensorDoesNotExistError):
         ds["__temp_123"].numpy()
 
     assert ds._temp_tensors == []
 
 
+def test_max_view(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc")
+        ds.create_tensor("xyz")
+        ds.create_tensor("pqr")
+
+        ds.abc.extend([1, 2, 3, 4])
+        ds.xyz.extend([1, 2, 3])
+        ds.pqr.extend([1, 2])
+
+    expected = {
+        "abc": [[1], [2], [3], [4]],
+        "xyz": [[1], [2], [3], []],
+        "pqr": [[1], [2], [], []],
+    }
+
+    for i, sample in enumerate(ds.max_view):
+        np.testing.assert_array_equal(sample.abc.numpy(), expected["abc"][i])
+
+
+def test_min_view(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc")
+        ds.create_tensor("xyz")
+        ds.create_tensor("pqr")
+
+        ds.abc.extend([1, 2, 3, 4])
+        ds.xyz.extend([1, 2, 3])
+        ds.pqr.extend([1, 2])
+
+    expected = {
+        "abc": [[1], [2]],
+        "xyz": [[1], [2]],
+        "pqr": [[1], [2]],
+    }
+
+    for i, sample in enumerate(ds.min_view):
+        np.testing.assert_array_equal(sample.abc.numpy(), expected["abc"][i])
+
+
 def test_extend_with_empty_tensor(memory_ds):
     with memory_ds as ds:
         ds.create_tensor("abc")
         ds.abc.extend([None, None, None])
 
         ds.create_tensor("xyz")
         ds.xyz.extend(ds.abc)
```

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.2.9/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.2.9/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.2.9/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.2.9/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_dataset.py` & `deeplake-3.2.9/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_dicom.py` & `deeplake-3.2.9/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_downsample.py` & `deeplake-3.2.9/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_events.py` & `deeplake-3.2.9/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_grayscale.py` & `deeplake-3.2.9/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_info.py` & `deeplake-3.2.9/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.2.9/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_json.py` & `deeplake-3.2.9/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_link.py` & `deeplake-3.2.9/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.2.9/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_linking.py` & `deeplake-3.2.9/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_mesh.py` & `deeplake-3.2.9/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_meta.py` & `deeplake-3.2.9/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_nifti.py` & `deeplake-3.2.9/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_none.py` & `deeplake-3.2.9/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.2.9/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_pickle.py` & `deeplake-3.2.9/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.2.9/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_polygons.py` & `deeplake-3.2.9/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_pop.py` & `deeplake-3.2.9/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_readonly.py` & `deeplake-3.2.9/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_rechunk.py` & `deeplake-3.2.9/deeplake/api/tests/test_rechunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,7 +265,32 @@
     sample_1 = ds.abc[1]._linked_sample()
     assert sample_1.path == s3_path_1, sample_1.creds_key == "my_s3_key_1"
 
     sample_2 = ds.abc[2]._linked_sample()
     assert sample_2.path == s3_path_1, sample_2.creds_key == "my_s3_key_1"
 
     assert ds.abc.chunk_engine.creds_encoder.num_samples == 3
+
+
+@deeplake.compute
+def add_samples(sample_in, samples_out):
+    samples_out.labels.append(np.ones((200,), dtype=np.int64))
+
+
+def test_rechunk_vc_bug(local_ds):
+    ds = local_ds
+    with ds:
+        ds.create_tensor("labels", dtype="int64")
+    add_samples().eval(list(range(200)), ds, num_workers=2)
+    ds.commit()
+    add_samples().eval(list(range(100)), ds, num_workers=2)
+    ds.commit()
+    ds.checkout("alt", True)
+    ds.labels[8] = ds.labels[8].numpy()
+    ds.commit()
+    np.testing.assert_array_equal(
+        ds.labels.numpy(), np.ones((300, 200), dtype=np.int64)
+    )
+    ds.checkout("main")
+    np.testing.assert_array_equal(
+        ds.labels.numpy(), np.ones((300, 200), dtype=np.int64)
+    )
```

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_sample_info.py` & `deeplake-3.2.9/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_text.py` & `deeplake-3.2.9/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_update_samples.py` & `deeplake-3.2.9/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_video.py` & `deeplake-3.2.9/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/api/tests/test_views.py` & `deeplake-3.2.9/deeplake/api/tests/test_views.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,25 +22,18 @@
     )
     ds.commit()
 
 
 def test_view_token_only(
     hub_cloud_path, hub_cloud_dev_token, hub_cloud_dev_credentials
 ):
-    username = get_user_name()
-    if username != "public":
-        state = "logged in"
-    else:
-        state = "logged out"
     runner = CliRunner()
     result = runner.invoke(logout)
     assert result.exit_code == 0
 
-    username, password = hub_cloud_dev_credentials
-
     ds = deeplake.empty(hub_cloud_path, token=hub_cloud_dev_token)
     with ds:
         populate(ds)
 
     ds = deeplake.load(hub_cloud_path, token=hub_cloud_dev_token)
     view = ds[50:100]
     view.save_view(id="50to100")
@@ -60,24 +53,16 @@
     np.testing.assert_array_equal(loaded.images.numpy(), ds[25:100].images.numpy())
     np.testing.assert_array_equal(loaded.labels.numpy(), ds[25:100].labels.numpy())
     assert loaded._vds.path == posixpath.join(hub_cloud_path, ".queries/25to100")
 
     ds.delete_view("25to100")
     deeplake.delete(hub_cloud_path, token=hub_cloud_dev_token)
 
-    if state == "logged in":
-        runner.invoke(login, f"-u {username} -p {password}")
-
 
 def test_view_public(hub_cloud_dev_credentials):
-    username = get_user_name()
-    if username != "public":
-        state = "logged in"
-    else:
-        state = "logged out"
     runner = CliRunner()
     result = runner.invoke(logout)
     assert result.exit_code == 0
 
     username, password = hub_cloud_dev_credentials
 
     ds = deeplake.load("hub://activeloop/mnist-train")
@@ -90,16 +75,15 @@
 
     ds = deeplake.load("hub://activeloop/mnist-train")
     view = ds[100:200]
 
     with pytest.raises(ReadOnlyModeError):
         view.save_view(id="100to200")
 
-    if state == "logged out":
-        runner.invoke(logout)
+    runner.invoke(logout)
 
 
 def test_view_with_empty_tensor(local_ds):
     with local_ds as ds:
         ds.create_tensor("images")
         ds.images.extend([1, 2, 3, 4, 5])
```

### Comparing `deeplake-3.2.8/deeplake/api/tiled.py` & `deeplake-3.2.9/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/structured/base.py` & `deeplake-3.2.9/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/structured/dataframe.py` & `deeplake-3.2.9/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.2.9/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.2.9/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.2.9/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.2.9/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/base.py` & `deeplake-3.2.9/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.2.9/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.2.9/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.2.9/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.2.9/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.2.9/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.2.9/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/util.py` & `deeplake-3.2.9/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.2.9/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.2.9/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/cli/auth.py` & `deeplake-3.2.9/deeplake/cli/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,42 +7,55 @@
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.client.utils import remove_username_from_config, write_token, remove_token
 from deeplake.util.bugout_reporter import (
     save_reporting_config,
     get_reporting_config,
     deeplake_reporter,
 )
-from deeplake.util.exceptions import AuthenticationException
+from deeplake.util.exceptions import AuthenticationException, LoginException
 
 
 @click.command()
 @click.option("--username", "-u", default=None, help="Your Activeloop Username")
 @click.option("--password", "-p", default=None, help="Your Activeloop Password")
-def login(username: str, password: str):
+@click.option("--token", "-t", default=None, help="Your Activeloop API token")
+def login(username: str, password: str, token: str):
     """Log in to Activeloop"""
     chances: int = 3
     while chances:
-        if not username:
-            click.echo("Login to Activeloop using your credentials.")
-            click.echo(
-                "If you don't have an account, register by using the 'activeloop register' command or by going to "
-                f"{HUB_REST_ENDPOINT}/register."
-            )
-            username = click.prompt("Username")
-            password = click.prompt("Password", hide_input=True)
-        if not password:
-            password = click.prompt(
-                f"Please enter password for user {username}", hide_input=True
-            )
-        username = username.strip()
-        password = password.strip()
+        if not (username or password) and token:
+            token = token.strip()
+        else:
+            if not username:
+                click.echo("Login to Activeloop using your credentials.")
+                click.echo(
+                    "If you don't have an account, register by using the 'activeloop register' command or by going to "
+                    f"{HUB_REST_ENDPOINT}/register."
+                )
+                username = click.prompt("Username")
+                password = click.prompt("Password", hide_input=True)
+            if not password:
+                password = click.prompt(
+                    f"Please enter password for user {username}", hide_input=True
+                )
+            username = username.strip()
+            password = password.strip()
         try:
-            client = DeepLakeBackendClient()
-            token = client.request_auth_token(username, password)
-            write_token(token)
+            if token is None:
+                client = DeepLakeBackendClient()
+                token = client.request_auth_token(username, password)
+                write_token(token)
+            else:
+                client = DeepLakeBackendClient(token)
+                orgs = client.get_user_organizations()
+                if orgs == ["public"]:
+                    raise LoginException(
+                        "Invalid API token. Please make sure the token is correct and try again."
+                    )
+                write_token(token)
             click.echo("Successfully logged in to Activeloop.")
             reporting_config = get_reporting_config()
             if reporting_config.get("username") != username:
                 save_reporting_config(True, username=username)
             break
         except AuthenticationException:
             chances -= 1
@@ -50,14 +63,16 @@
                 print("Login failed. Check username and password.")
                 username = ""
                 password = ""
             else:
                 print(
                     "3 unsuccessful attempts. Kindly retry logging in after sometime."
                 )
+        except LoginException:
+            raise
         except Exception as e:
             print(f"Encountered an error {e} Please try again later.")
             break
 
 
 @click.command()
 def logout():
```

### Comparing `deeplake-3.2.8/deeplake/client/client.py` & `deeplake-3.2.9/deeplake/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     GET_TOKEN_SUFFIX,
     HUB_REST_ENDPOINT_STAGING,
     REGISTER_USER_SUFFIX,
     DEFAULT_REQUEST_TIMEOUT,
     GET_DATASET_CREDENTIALS_SUFFIX,
     CREATE_DATASET_SUFFIX,
     DATASET_SUFFIX,
-    LIST_DATASETS,
     GET_USER_PROFILE,
     SEND_EVENT_SUFFIX,
     UPDATE_SUFFIX,
     GET_PRESIGNED_URL_SUFFIX,
     CONNECT_DATASET_SUFFIX,
 )
 from deeplake.client.log import logger
@@ -393,35 +392,14 @@
                 "GET",
                 suffix_public,
                 endpoint=self.endpoint(),
                 params={"organization": workspace},
             ).json()
         return response
 
-    def get_datasets(self, workspace: str):
-        suffix_public = LIST_DATASETS.format("public")
-        suffix_user = LIST_DATASETS.format("all")
-        if workspace:
-            res_datasets = self.get_workspace_datasets(
-                workspace, suffix_public, suffix_user
-            )
-        else:
-            public_datasets = self.request(
-                "GET",
-                suffix_public,
-                endpoint=self.endpoint(),
-            ).json()
-            user_datasets = self.request(
-                "GET",
-                suffix_user,
-                endpoint=self.endpoint(),
-            ).json()
-            res_datasets = public_datasets + user_datasets
-        return [ds["_id"] for ds in res_datasets]
-
     def update_privacy(self, username: str, dataset_name: str, public: bool):
         suffix = UPDATE_SUFFIX.format(username, dataset_name)
         self.request("PUT", suffix, endpoint=self.endpoint(), json={"public": public})
 
     def get_presigned_url(self, org_id, ds_id, chunk_path, expiration=3600):
         relative_url = GET_PRESIGNED_URL_SUFFIX.format(org_id, ds_id)
         response = self.request(
```

### Comparing `deeplake-3.2.8/deeplake/client/config.py` & `deeplake-3.2.9/deeplake/client/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,13 @@
 CREATE_DATASET_SUFFIX = "/api/dataset/create"
 SEND_EVENT_SUFFIX = "/api/event"
 DATASET_SUFFIX = "/api/dataset"
 UPDATE_SUFFIX = "/api/org/{}/dataset/{}"
 GET_MANAGED_CREDS_SUFFIX = "/api/org/{}/storage/name"
 ACCEPT_AGREEMENTS_SUFFIX = "/api/organization/{}/dataset/{}/agree"
 REJECT_AGREEMENTS_SUFFIX = "/api/organization/{}/dataset/{}/disagree"
-LIST_DATASETS = "/api/datasets/{}"
 GET_USER_PROFILE = "/api/user/profile"
 CONNECT_DATASET_SUFFIX = "/api/dataset/connect"
 
 DEFAULT_REQUEST_TIMEOUT = 170
 
 HUB_AUTH_TOKEN = "HUB_AUTH_TOKEN"
```

### Comparing `deeplake-3.2.8/deeplake/client/log.py` & `deeplake-3.2.9/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/client/utils.py` & `deeplake-3.2.9/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/compression.py` & `deeplake-3.2.9/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/constants.py` & `deeplake-3.2.9/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk/base_chunk.py` & `deeplake-3.2.9/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.2.9/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.2.9/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.2.9/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.2.9/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.2.9/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.2.9/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/chunk_engine.py` & `deeplake-3.2.9/deeplake/core/chunk_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1398,14 +1398,16 @@
 
         next_chunk_name = ChunkIdEncoder.name_from_id(next_chunk_id)  # type: ignore
         next_chunk_commit_id, tkey = self.get_chunk_commit(next_chunk_name)
         chunk_key = get_chunk_key(tkey, next_chunk_name, next_chunk_commit_id)
         next_chunk_size = self.cache.get_object_size(chunk_key)
         next_chunk = self.get_chunk_from_chunk_id(int(next_chunk_id))
         if next_chunk_size + chunk.num_data_bytes < next_chunk.min_chunk_size:
+            if next_chunk_commit_id != self.commit_id:
+                next_chunk = self.copy_chunk_to_new_commit(next_chunk, next_chunk_name)
             # merge with next chunk
             return self._merge_chunks(
                 from_chunk=next_chunk,
                 from_chunk_row=next_chunk_row,
                 to_chunk=chunk,
                 to_chunk_row=row,
             )
@@ -1422,14 +1424,16 @@
 
         prev_chunk_name = ChunkIdEncoder.name_from_id(prev_chunk_id)  # type: ignore
         prev_chunk_commit_id, tkey = self.get_chunk_commit(prev_chunk_name)
         prev_chunk_key = get_chunk_key(tkey, prev_chunk_name, prev_chunk_commit_id)
         prev_chunk_size = self.cache.get_object_size(prev_chunk_key)
         prev_chunk = self.get_chunk_from_chunk_id(int(prev_chunk_id))
         if prev_chunk_size + chunk.num_data_bytes < prev_chunk.min_chunk_size:
+            if prev_chunk_commit_id != self.commit_id:
+                prev_chunk = self.copy_chunk_to_new_commit(prev_chunk, prev_chunk_name)
             # merge with previous chunk
             return self._merge_chunks(
                 from_chunk=chunk,
                 from_chunk_row=row,
                 to_chunk=prev_chunk,
                 to_chunk_row=prev_chunk_row,
             )
```

### Comparing `deeplake-3.2.8/deeplake/core/compression.py` & `deeplake-3.2.9/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/compute/process.py` & `deeplake-3.2.9/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/compute/provider.py` & `deeplake-3.2.9/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/compute/ray.py` & `deeplake-3.2.9/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/compute/serial.py` & `deeplake-3.2.9/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/compute/thread.py` & `deeplake-3.2.9/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/dataset/__init__.py` & `deeplake-3.2.9/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/dataset/dataset.py` & `deeplake-3.2.9/deeplake/core/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,29 +227,30 @@
         d["_checkout_hooks"] = {}
         d["_parent_dataset"] = None
         d["_pad_tensors"] = pad_tensors
         d["_locking_enabled"] = lock
         d["_temp_tensors"] = []
         dct = self.__dict__
         dct.update(d)
-        dct["enabled_tensors"] = (
-            set(self._resolve_tensor_list(enabled_tensors, root=True))
-            if enabled_tensors
-            else None
-        )
+
         try:
             self._set_derived_attributes()
         except LockedException:
             raise LockedException(
                 "This dataset cannot be open for writing as it is locked by another machine. Try loading the dataset with `read_only=True`."
             )
         except ReadOnlyModeError as e:
             raise ReadOnlyModeError(
                 "This dataset cannot be open for writing as you don't have permissions. Try loading the dataset with `read_only=True."
             )
+        dct["enabled_tensors"] = (
+            set(self._resolve_tensor_list(enabled_tensors, root=True))
+            if enabled_tensors
+            else None
+        )
         self._first_load_init()
         self._initial_autoflush: List[
             bool
         ] = []  # This is a stack to support nested with contexts
         self._indexing_history: List[int] = []
 
         if not self.read_only:
@@ -302,16 +303,18 @@
         """Returns the client of the dataset."""
         return self._client
 
     def __len__(self, warn: bool = True):
         """Returns the length of the smallest tensor."""
         tensor_lengths = [len(tensor) for tensor in self.tensors.values()]
         pad_tensors = self._pad_tensors
-        if not pad_tensors and min(tensor_lengths, default=0) != max(
-            tensor_lengths, default=0
+        if (
+            warn
+            and not pad_tensors
+            and min(tensor_lengths, default=0) != max(tensor_lengths, default=0)
         ):
             warning(
                 "The length of tensors in the dataset is different. The len(ds) returns the length of the "
                 "smallest tensor in the dataset. If you want the length of the longest tensor in the dataset use "
                 "ds.max_len."
             )
         length_fn = max if pad_tensors else min
```

### Comparing `deeplake-3.2.8/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.2.9/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/dataset/invalid_view.py` & `deeplake-3.2.9/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/dataset/view_entry.py` & `deeplake-3.2.9/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/fast_forwarding.py` & `deeplake-3.2.9/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/index/index.py` & `deeplake-3.2.9/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/io.py` & `deeplake-3.2.9/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/ipc.py` & `deeplake-3.2.9/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/link_creds.py` & `deeplake-3.2.9/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/linked_chunk_engine.py` & `deeplake-3.2.9/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/linked_sample.py` & `deeplake-3.2.9/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/linked_tiled_sample.py` & `deeplake-3.2.9/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/lock.py` & `deeplake-3.2.9/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/dataset_meta.py` & `deeplake-3.2.9/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.2.9/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.2.9/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.2.9/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/creds.py` & `deeplake-3.2.9/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/sequence.py` & `deeplake-3.2.9/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/shape.py` & `deeplake-3.2.9/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.2.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/encode/tile.py` & `deeplake-3.2.9/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/meta/tensor_meta.py` & `deeplake-3.2.9/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/partial_reader.py` & `deeplake-3.2.9/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/partial_sample.py` & `deeplake-3.2.9/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/polygon.py` & `deeplake-3.2.9/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/query/autocomplete.py` & `deeplake-3.2.9/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/query/filter.py` & `deeplake-3.2.9/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/query/query.py` & `deeplake-3.2.9/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/sample.py` & `deeplake-3.2.9/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/serialize.py` & `deeplake-3.2.9/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.2.9/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/gcs.py` & `deeplake-3.2.9/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/google_drive.py` & `deeplake-3.2.9/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/local.py` & `deeplake-3.2.9/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/lru_cache.py` & `deeplake-3.2.9/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/memory.py` & `deeplake-3.2.9/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/provider.py` & `deeplake-3.2.9/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/storage/s3.py` & `deeplake-3.2.9/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tensor.py` & `deeplake-3.2.9/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tensor_link.py` & `deeplake-3.2.9/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/test_serialize.py` & `deeplake-3.2.9/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tests/test_compression.py` & `deeplake-3.2.9/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tests/test_compute.py` & `deeplake-3.2.9/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tests/test_io.py` & `deeplake-3.2.9/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tests/test_locking.py` & `deeplake-3.2.9/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tests/test_readonly.py` & `deeplake-3.2.9/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tests/test_serialize.py` & `deeplake-3.2.9/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tiling/deserialize.py` & `deeplake-3.2.9/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tiling/optimizer.py` & `deeplake-3.2.9/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.2.9/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tiling/serialize.py` & `deeplake-3.2.9/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.2.9/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/tiling/test_serialize.py` & `deeplake-3.2.9/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/transform/test_transform.py` & `deeplake-3.2.9/deeplake/core/transform/test_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -800,14 +800,60 @@
     ds.checkout(br)
     assert len(ds) == 20
     for i in range(20):
         target = 2 if i % 2 == 0 else 3
         check_target_array(ds, i, target)
 
 
+def test_inplace_transform_bug(local_ds_generator):
+    @deeplake.compute
+    def construct(sample_in, sample_out):
+        sample_out.append({"positive": [1, 2, 3], "negative": [4, 5, 6]})
+
+    ds = local_ds_generator()
+    with ds:
+        ds.create_tensor("id")
+        ds.id.extend(list(range(10)))
+
+        ds.create_tensor("positive")
+        ds.create_tensor("negative")
+
+    for _ in range(0, ds.max_len):
+        construct().eval(
+            ds,
+            num_workers=2,
+            skip_ok=True,
+            check_lengths=False,
+            pad_data_in=True,
+        )
+
+    np.testing.assert_array_equal(
+        ds.positive.numpy(aslist=True), [np.array([1, 2, 3])] * 10
+    )
+    np.testing.assert_array_equal(
+        ds.negative.numpy(aslist=True), [np.array([4, 5, 6])] * 10
+    )
+
+
+def test_inplace_transform_bug_2(local_ds_generator):
+    @deeplake.compute
+    def tform(sample_in, sample_out):
+        sample_out.text2.append(sample_in.text.text())
+
+    ds = local_ds_generator()
+    with ds:
+        ds.create_tensor("text", htype="text", sample_compression="lz4")
+        ds.text.extend(["abcd", "efgh", "hijk"] * 10)
+        ds.create_tensor("text2", htype="text", sample_compression="lz4")
+        tform().eval(ds[["text"]], ds, num_workers=2, check_lengths=False)
+
+    np.testing.assert_array_equal(ds.text.text(), ["abcd", "efgh", "hijk"] * 10)
+    np.testing.assert_array_equal(ds.text2.text(), ["abcd", "efgh", "hijk"] * 10)
+
+
 def test_inplace_transform_clear_chunks(local_ds_generator):
     ds = local_ds_generator()
 
     with ds:
         ds.create_tensor("img")
         ds.create_tensor("label")
```

### Comparing `deeplake-3.2.8/deeplake/core/transform/transform.py` & `deeplake-3.2.9/deeplake/core/transform/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,14 @@
             self,
             version_state,
             target_ds.link_creds,
             skip_ok,
             extend_only,
         )
         map_inp = zip(slices, storages, repeat(args))
-
         try:
             if progressbar:
                 desc = get_pbar_description(self.functions)
                 result = compute.map_with_progressbar(
                     store_data_slice_with_pbar,
                     map_inp,
                     total_length=len(data_in),
```

### Comparing `deeplake-3.2.8/deeplake/core/transform/transform_dataset.py` & `deeplake-3.2.9/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/transform/transform_tensor.py` & `deeplake-3.2.9/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.2.9/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/version_control/commit_diff.py` & `deeplake-3.2.9/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/version_control/commit_node.py` & `deeplake-3.2.9/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.2.9/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/version_control/test_merge.py` & `deeplake-3.2.9/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/core/version_control/test_version_control.py` & `deeplake-3.2.9/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.2.9/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/enterprise/dataloader.py` & `deeplake-3.2.9/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.2.9/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/enterprise/test_pytorch.py` & `deeplake-3.2.9/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/enterprise/test_query.py` & `deeplake-3.2.9/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.2.9/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/enterprise/util.py` & `deeplake-3.2.9/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/hooks.py` & `deeplake-3.2.9/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/htype.py` & `deeplake-3.2.9/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.2.9/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.2.9/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/pytorch/common.py` & `deeplake-3.2.9/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.2.9/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.2.9/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.2.9/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/tf/common.py` & `deeplake-3.2.9/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.2.9/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.2.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/integrations/wandb/wandb.py` & `deeplake-3.2.9/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/tests/cache_fixtures.py` & `deeplake-3.2.9/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/tests/client_fixtures.py` & `deeplake-3.2.9/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/tests/common.py` & `deeplake-3.2.9/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/tests/dataset_fixtures.py` & `deeplake-3.2.9/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/tests/path_fixtures.py` & `deeplake-3.2.9/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/tests/storage_fixtures.py` & `deeplake-3.2.9/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/access_method.py` & `deeplake-3.2.9/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/agreement.py` & `deeplake-3.2.9/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/array_list.py` & `deeplake-3.2.9/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/assert_byte_indexes.py` & `deeplake-3.2.9/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/auto.py` & `deeplake-3.2.9/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/bugout_reporter.py` & `deeplake-3.2.9/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/cache_chain.py` & `deeplake-3.2.9/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/casting.py` & `deeplake-3.2.9/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/check_latest_version.py` & `deeplake-3.2.9/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/chunk_engine.py` & `deeplake-3.2.9/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/class_label.py` & `deeplake-3.2.9/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/compute.py` & `deeplake-3.2.9/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/connect_dataset.py` & `deeplake-3.2.9/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/dataset.py` & `deeplake-3.2.9/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/diff.py` & `deeplake-3.2.9/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/downsample.py` & `deeplake-3.2.9/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/encoder.py` & `deeplake-3.2.9/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/exceptions.py` & `deeplake-3.2.9/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/exif.py` & `deeplake-3.2.9/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/from_tfds.py` & `deeplake-3.2.9/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/htype.py` & `deeplake-3.2.9/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/image.py` & `deeplake-3.2.9/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/invalid_view_op.py` & `deeplake-3.2.9/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/iteration_warning.py` & `deeplake-3.2.9/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/json.py` & `deeplake-3.2.9/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/keys.py` & `deeplake-3.2.9/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/link.py` & `deeplake-3.2.9/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/logging.py` & `deeplake-3.2.9/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/merge.py` & `deeplake-3.2.9/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/modified.py` & `deeplake-3.2.9/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/notebook.py` & `deeplake-3.2.9/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/mesh.py` & `deeplake-3.2.9/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.2.9/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.2.9/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.2.9/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.2.9/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.2.9/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.2.9/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.2.9/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.2.9/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.2.9/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/path.py` & `deeplake-3.2.9/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/pretty_print.py` & `deeplake-3.2.9/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/remove_cache.py` & `deeplake-3.2.9/deeplake/util/remove_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         storage=zero_cache_storage,
         group_index=ds.group_index,
         read_only=ds.read_only,
         token=ds.token,
         verbose=False,
         link_creds=ds.link_creds,
         pad_tensors=ds._pad_tensors,
+        enabled_tensors=ds.enabled_tensors,
     )
     if ds.pending_commit_id != commit_id:
         ds.checkout(commit_id)
     ds.index = index
     return ds
```

### Comparing `deeplake-3.2.8/deeplake/util/scheduling.py` & `deeplake-3.2.9/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/shape_interval.py` & `deeplake-3.2.9/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/split.py` & `deeplake-3.2.9/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/storage.py` & `deeplake-3.2.9/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tag.py` & `deeplake-3.2.9/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tests/test_auto.py` & `deeplake-3.2.9/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.2.9/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.2.9/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tests/test_read.py` & `deeplake-3.2.9/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.2.9/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tests/test_split.py` & `deeplake-3.2.9/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/tests/test_version_control.py` & `deeplake-3.2.9/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/transform.py` & `deeplake-3.2.9/deeplake/util/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,14 @@
     actual_tensors: Optional[List[str]],
     all_chunk_engines: Dict[str, ChunkEngine],
     group_index: str,
     pg_callback=None,
     skip_ok=False,
 ) -> None:
     """Transforms the data_slice with the pipeline and adds the resultant samples to chunk_engines."""
-
     n = len(data_slice)
     last_reported_time = time.time()
     last_reported_num_samples = 0
     for i, sample in enumerate(
         (data_slice[i : i + 1] for i in range(n))
         if pd and isinstance(data_slice, pd.DataFrame)
         else data_slice
@@ -394,14 +393,15 @@
         storage=cached_store,
         group_index=dataset_slice.group_index,
         read_only=dataset_slice.read_only,
         token=dataset_slice.token,
         verbose=False,
         link_creds=dataset_slice.link_creds,
         pad_tensors=dataset_slice._pad_tensors,
+        enabled_tensors=dataset_slice.enabled_tensors,
     )
     dataset_slice.checkout(commit_id)
     dataset_slice.index = index
     return dataset_slice
 
 
 def check_transform_data_in(data_in, scheduler: str) -> None:
@@ -462,15 +462,16 @@
 
     names_desc = ", ".join(func_names)
     return f"Evaluating [{names_desc}]"
 
 
 def create_slices(data_in, num_workers):
     size = math.ceil(len(data_in) / num_workers)
-    return [data_in[i * size : (i + 1) * size] for i in range(num_workers)]
+    ret = [data_in[i * size : (i + 1) * size] for i in range(num_workers)]
+    return ret
 
 
 def get_old_chunk_paths(target_ds, generated_tensors, overwrite):
     old_chunk_paths = []
     if overwrite:
         for key in generated_tensors:
             tensor = target_ds[key]
```

### Comparing `deeplake-3.2.8/deeplake/util/version_control.py` & `deeplake-3.2.9/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/util/video.py` & `deeplake-3.2.9/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/visualizer/video_streaming.py` & `deeplake-3.2.9/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake/visualizer/visualizer.py` & `deeplake-3.2.9/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.2.8/deeplake.egg-info/PKG-INFO` & `deeplake-3.2.9/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.2.8
+Version: 3.2.9
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.2.8 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.2.9 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Description: [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-
 b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
              ****** Deep Lake: Data Lake for Deep Learning ******
```

### Comparing `deeplake-3.2.8/deeplake.egg-info/SOURCES.txt` & `deeplake-3.2.9/deeplake.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 deeplake/auto/unstructured/yolo/__init__.py
 deeplake/auto/unstructured/yolo/constants.py
 deeplake/auto/unstructured/yolo/utils.py
 deeplake/auto/unstructured/yolo/yolo.py
 deeplake/cli/__init__.py
 deeplake/cli/auth.py
 deeplake/cli/commands.py
-deeplake/cli/list_datasets.py
 deeplake/cli/test_cli.py
 deeplake/client/__init__.py
 deeplake/client/client.py
 deeplake/client/config.py
 deeplake/client/log.py
 deeplake/client/test_client.py
 deeplake/client/utils.py
```

### Comparing `deeplake-3.2.8/deeplake.egg-info/requires.txt` & `deeplake-3.2.9/deeplake.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 humbug>=0.2.6
 tqdm
 numcodecs
 pyjwt
 hub>=2.8.7
 
 [all]
-oauth2client~=4.1.3
-google-cloud-storage~=1.42.0
-flask
-google-api-python-client~=2.31.0
+nibabel
 google-auth-oauthlib~=0.4.5
+google-api-python-client~=2.31.0
 laspy
-nibabel
-IPython
-pydicom
+google-cloud-storage~=1.42.0
 google-auth~=2.0.1
+oauth2client~=4.1.3
+flask
+pydicom
+IPython
 libdeeplake==0.0.37
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [audio]
```

### Comparing `deeplake-3.2.8/setup.py` & `deeplake-3.2.9/setup.py`

 * *Files identical despite different names*

