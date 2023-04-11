# Comparing `tmp/lightly-1.4.0.tar.gz` & `tmp/lightly-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightly-1.4.0.tar", last modified: Wed Apr  5 14:47:10 2023, max compression
+gzip compressed data, was "lightly-1.4.1.tar", last modified: Tue Apr 11 13:09:29 2023, max compression
```

## Comparing `lightly-1.4.0.tar` & `lightly-1.4.1.tar`

### file list

```diff
@@ -1,405 +1,407 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.172237 lightly-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-05 14:47:00.000000 lightly-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-05 14:47:00.000000 lightly-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-05 14:47:10.172237 lightly-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-04-05 14:47:00.000000 lightly-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.136236 lightly-1.4.0/lightly/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.136236 lightly-1.4.0/lightly/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.136236 lightly-1.4.0/lightly/active_learning/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/agents/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.140236 lightly-1.4.0/lightly/active_learning/config/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/config/selection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.140236 lightly-1.4.0/lightly/active_learning/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/scorers/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/scorers/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/scorers/keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/scorers/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.140236 lightly-1.4.0/lightly/active_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/utils/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/utils/keypoint_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/active_learning/utils/object_detection_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.140236 lightly-1.4.0/lightly/api/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_compute_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_upload_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/api_workflow_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/bitmask.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/swagger_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/swagger_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/api/version_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.144236 lightly-1.4.0/lightly/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/_cli_simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.144236 lightly-1.4.0/lightly/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/config/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/crop_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/embed_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/lightly_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/train_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/upload_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/cli/version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.144236 lightly-1.4.0/lightly/data/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/_image_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/_video.py
--rw-r--r--   0 runner    (1001) docker     (123)    49756 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/lightly_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/data/multi_view_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.144236 lightly-1.4.0/lightly/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/embedding/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/embedding/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/embedding/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.144236 lightly-1.4.0/lightly/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/dcl_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/dino_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/hypersphere_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/msn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/negative_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/ntx_ent_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/pmsn_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.144236 lightly-1.4.0/lightly/loss/regularizer/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/regularizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/regularizer/co2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/swav_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/sym_neg_cos_sim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/tico_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/vicreg_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/loss/vicregl_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.148237 lightly-1.4.0/lightly/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/byol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/moco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.148237 lightly-1.4.0/lightly/models/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/modules/heads.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/modules/masked_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/modules/nn_memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/nnclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)    17107 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.136236 lightly-1.4.0/lightly/openapi_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.148237 lightly-1.4.0/lightly/openapi_generated/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    24726 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.148237 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/collaboration_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    76297 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/datasources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/docker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/embeddings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/predictions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/quota_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47328 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/samples_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/samplings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/scores_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api/versioning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.172237 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    23095 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/access_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/api_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/api_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/async_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/category_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/category_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/create_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_license_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/file_name_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/file_output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/general_job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/jobs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_studio_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/path_safe_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/s3_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sama_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sama_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sama_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_input_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/shared_access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/task_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/team_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/team_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/version_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/video_frame_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/openapi_generated/swagger_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.172237 lightly-1.4.0/lightly/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/dino_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/image_grid_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/mae_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/moco_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/msn_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/multi_crop_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/multi_view_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/pirl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/random_crop_and_flip_with_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/simclr_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/smog_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/swav_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/vicreg_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/transforms/vicregl_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.172237 lightly-1.4.0/lightly/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/benchmarking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.172237 lightly-1.4.0/lightly/utils/cropping/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/cropping/crop_image_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/cropping/read_yolo_label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/embeddings_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/hipify.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/reordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-05 14:47:00.000000 lightly-1.4.0/lightly/utils/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:47:10.136236 lightly-1.4.0/lightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-05 14:47:10.000000 lightly-1.4.0/lightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22052 2023-04-05 14:47:10.000000 lightly-1.4.0/lightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:47:10.000000 lightly-1.4.0/lightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-05 14:47:10.000000 lightly-1.4.0/lightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-05 14:47:10.000000 lightly-1.4.0/lightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 14:47:10.000000 lightly-1.4.0/lightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-05 14:47:00.000000 lightly-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-05 14:47:10.176237 lightly-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-05 14:47:00.000000 lightly-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.758879 lightly-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 13:09:18.000000 lightly-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 13:09:18.000000 lightly-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-11 13:09:29.762879 lightly-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-04-11 13:09:18.000000 lightly-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.722879 lightly-1.4.1/lightly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.726879 lightly-1.4.1/lightly/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.726879 lightly-1.4.1/lightly/active_learning/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/agents/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.726879 lightly-1.4.1/lightly/active_learning/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/config/selection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.726879 lightly-1.4.1/lightly/active_learning/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/scorers/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/scorers/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/scorers/keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/scorers/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/scorers/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.726879 lightly-1.4.1/lightly/active_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/utils/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/utils/keypoint_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/active_learning/utils/object_detection_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.730879 lightly-1.4.1/lightly/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19386 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_compute_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_upload_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/api_workflow_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/swagger_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/swagger_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/api/version_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.730879 lightly-1.4.1/lightly/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/_cli_simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.730879 lightly-1.4.1/lightly/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/config/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/crop_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/download_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/embed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/lightly_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/train_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/upload_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/cli/version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.730879 lightly-1.4.1/lightly/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/_image_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49756 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/lightly_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/data/multi_view_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.730879 lightly-1.4.1/lightly/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/embedding/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/embedding/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/embedding/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.734879 lightly-1.4.1/lightly/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/dcl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/dino_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/hypersphere_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/msn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/negative_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/ntx_ent_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/pmsn_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.734879 lightly-1.4.1/lightly/loss/regularizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/regularizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/regularizer/co2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/swav_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/sym_neg_cos_sim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/tico_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/vicreg_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/loss/vicregl_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.734879 lightly-1.4.1/lightly/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/byol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/moco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.734879 lightly-1.4.1/lightly/models/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/modules/heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/modules/masked_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/modules/nn_memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/nnclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17107 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.722879 lightly-1.4.1/lightly/openapi_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.734879 lightly-1.4.1/lightly/openapi_generated/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    24726 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.738879 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/collaboration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76297 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/datasources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/docker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/embeddings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/mappings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/predictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/quota_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47328 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/samples_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/samplings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/scores_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api/versioning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.758879 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    23095 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/access_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/api_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/api_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/async_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/category_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/category_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/create_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_license_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/file_name_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/file_output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/general_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/jobs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_studio_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/path_safe_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/s3_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sama_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sama_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sama_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/shared_access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/task_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/team_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/team_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/version_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/video_frame_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/openapi_generated/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.758879 lightly-1.4.1/lightly/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/dino_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/fast_siam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/image_grid_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/mae_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/moco_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/msn_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/multi_crop_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/multi_view_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/pirl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/random_crop_and_flip_with_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/simclr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/simsiam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/smog_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/swav_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/vicreg_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/transforms/vicregl_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.758879 lightly-1.4.1/lightly/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/benchmarking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.758879 lightly-1.4.1/lightly/utils/cropping/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/cropping/crop_image_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/cropping/read_yolo_label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/embeddings_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/hipify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/reordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-11 13:09:18.000000 lightly-1.4.1/lightly/utils/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:09:29.726879 lightly-1.4.1/lightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-11 13:09:29.000000 lightly-1.4.1/lightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22134 2023-04-11 13:09:29.000000 lightly-1.4.1/lightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:09:29.000000 lightly-1.4.1/lightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 13:09:29.000000 lightly-1.4.1/lightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-11 13:09:29.000000 lightly-1.4.1/lightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 13:09:29.000000 lightly-1.4.1/lightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 13:09:18.000000 lightly-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 13:09:29.762879 lightly-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-11 13:09:18.000000 lightly-1.4.1/setup.py
```

### Comparing `lightly-1.4.0/LICENSE.txt` & `lightly-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/PKG-INFO` & `lightly-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.0
+Version: 1.4.1
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.0/README.md` & `lightly-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -228,22 +228,23 @@
 | Model            | Epochs | Batch Size | Test Accuracy |
 |------------------|--------|------------|---------------|
 | BarlowTwins      |    800 |        256 |         0.850 |
 | BYOL             |    800 |        256 |         0.887 |
 | DCL              |    800 |        256 |         0.864 |
 | DCLW             |    800 |        256 |         0.861 |
 | DINO (Res18)     |    800 |        256 |         0.887 |
+| FastSiam         |    800 |        256 |         0.865 |
 | MAE (ViT-S)      |    800 |        256 |         0.620 |
 | MSN (ViT-S)      |    800 |        256 |         0.833 |
 | Moco             |    800 |        256 |         0.874 |
 | NNCLR            |    800 |        256 |         0.885 |
 | PMSN (ViT-S)     |    800 |        256 |         0.830 |
 | SimCLR           |    800 |        256 |         0.889 |
 | SimMIM (ViT-B32) |    800 |        256 |         0.351 |
-| SimSiam          |    800 |        256 |         0.885 |
+| SimSiam          |    800 |        256 |         0.871 |
 | SwaV             |    800 |        256 |         0.899 |
 | SwaVQueue        |    800 |        256 |         0.898 |
 | SMoG             |    800 |        256 |         0.782 |
 | TiCo             |    800 |        256 |         0.857 |
 | VICReg           |    800 |        256 |         0.843 |
 | VICRegL          |    800 |        256 |         0.781 |
 
@@ -253,18 +254,19 @@
 | Model         | Epochs | Batch Size | Test Accuracy |
 |---------------|--------|------------|---------------|
 | BarlowTwins   |    800 |        512 |         0.857 |
 | BYOL          |    800 |        512 |         0.911 |
 | DCL           |    800 |        512 |         0.873 |
 | DCLW          |    800 |        512 |         0.873 | 
 | DINO          |    800 |        512 |         0.884 |
+| FastSiam      |    800 |        512 |         0.902 |
 | Moco          |    800 |        512 |         0.900 |
 | NNCLR         |    800 |        512 |         0.896 |
 | SimCLR        |    800 |        512 |         0.875 |
-| SimSiam       |    800 |        512 |         0.906 |
+| SimSiam       |    800 |        512 |         0.902 |
 | SwaV          |    800 |        512 |         0.881 |
 
 ## Terminology
 
 Below you can see a schematic overview of the different concepts present in the lightly Python package. The terms in bold are explained in more detail in our [documentation](https://docs.lightly.ai/self-supervised-learning/).
 
 <img src="/docs/source/getting_started/images/lightly_overview.png" alt="Overview of the lightly pip package"/></a>
```

### Comparing `lightly-1.4.0/lightly/__init__.py` & `lightly-1.4.1/lightly/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 __name__ = "lightly"
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 import os
 
 try:
     # See (https://github.com/PyTorchLightning/pytorch-lightning)
     # This variable is injected in the __builtins__ by the build
     # process. It used to enable importing subpackages of skimage when
```

### Comparing `lightly-1.4.0/lightly/active_learning/agents/agent.py` & `lightly-1.4.1/lightly/active_learning/agents/agent.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/config/selection_config.py` & `lightly-1.4.1/lightly/active_learning/config/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/scorers/classification.py` & `lightly-1.4.1/lightly/active_learning/scorers/classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/scorers/detection.py` & `lightly-1.4.1/lightly/active_learning/scorers/detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/scorers/keypoint_detection.py` & `lightly-1.4.1/lightly/active_learning/scorers/keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/scorers/semantic_segmentation.py` & `lightly-1.4.1/lightly/active_learning/scorers/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/utils/bounding_box.py` & `lightly-1.4.1/lightly/active_learning/utils/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/utils/keypoint_predictions.py` & `lightly-1.4.1/lightly/active_learning/utils/keypoint_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/active_learning/utils/object_detection_output.py` & `lightly-1.4.1/lightly/active_learning/utils/object_detection_output.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/__init__.py` & `lightly-1.4.1/lightly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_artifacts.py` & `lightly-1.4.1/lightly/api/api_workflow_artifacts.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_client.py` & `lightly-1.4.1/lightly/api/api_workflow_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_collaboration.py` & `lightly-1.4.1/lightly/api/api_workflow_collaboration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_compute_worker.py` & `lightly-1.4.1/lightly/api/api_workflow_compute_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     DockerRunScheduledPriority,
     DockerRunScheduledState,
     DockerRunState,
     DockerWorkerConfigV3,
     DockerWorkerConfigV3CreateRequest,
     DockerWorkerConfigV3Docker,
     DockerWorkerConfigV3Lightly,
+    DockerWorkerRegistryEntryData,
     DockerWorkerType,
     SelectionConfig,
     SelectionConfigEntry,
     SelectionConfigEntryInput,
     SelectionConfigEntryStrategy,
     TagData,
 )
@@ -106,14 +107,21 @@
         return response.id
 
     def get_compute_worker_ids(self) -> List[str]:
         """Returns the ids of all registered compute workers."""
         entries = self._compute_worker_api.get_docker_worker_registry_entries()
         return [entry.id for entry in entries]
 
+    def get_compute_workers(self) -> List[DockerWorkerRegistryEntryData]:
+        """Returns the ids of all registered compute workers."""
+        entries: list[
+            DockerWorkerRegistryEntryData
+        ] = self._compute_worker_api.get_docker_worker_registry_entries()
+        return entries
+
     def delete_compute_worker(self, worker_id: str):
         """Removes a compute worker.
 
         Args:
             worker_id:
                 The id of the worker to remove.
```

### Comparing `lightly-1.4.0/lightly/api/api_workflow_datasets.py` & `lightly-1.4.1/lightly/api/api_workflow_datasets.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_datasources.py` & `lightly-1.4.1/lightly/api/api_workflow_datasources.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_download_dataset.py` & `lightly-1.4.1/lightly/api/api_workflow_download_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_export.py` & `lightly-1.4.1/lightly/api/api_workflow_export.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_predictions.py` & `lightly-1.4.1/lightly/api/api_workflow_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_selection.py` & `lightly-1.4.1/lightly/api/api_workflow_selection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_tags.py` & `lightly-1.4.1/lightly/api/api_workflow_tags.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_upload_dataset.py` & `lightly-1.4.1/lightly/api/api_workflow_upload_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_upload_embeddings.py` & `lightly-1.4.1/lightly/api/api_workflow_upload_embeddings.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/api_workflow_upload_metadata.py` & `lightly-1.4.1/lightly/api/api_workflow_upload_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/bitmask.py` & `lightly-1.4.1/lightly/api/bitmask.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/download.py` & `lightly-1.4.1/lightly/api/download.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/patch.py` & `lightly-1.4.1/lightly/api/patch.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/prediction_singletons.py` & `lightly-1.4.1/lightly/api/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/swagger_api_client.py` & `lightly-1.4.1/lightly/api/swagger_api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/swagger_rest_client.py` & `lightly-1.4.1/lightly/api/swagger_rest_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/utils.py` & `lightly-1.4.1/lightly/api/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/api/version_checking.py` & `lightly-1.4.1/lightly/api/version_checking.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/_cli_simclr.py` & `lightly-1.4.1/lightly/cli/_cli_simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/_helpers.py` & `lightly-1.4.1/lightly/cli/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/config/config.yaml` & `lightly-1.4.1/lightly/cli/config/config.yaml`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/crop_cli.py` & `lightly-1.4.1/lightly/cli/crop_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/download_cli.py` & `lightly-1.4.1/lightly/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/embed_cli.py` & `lightly-1.4.1/lightly/cli/embed_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/lightly_cli.py` & `lightly-1.4.1/lightly/cli/lightly_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/train_cli.py` & `lightly-1.4.1/lightly/cli/train_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/upload_cli.py` & `lightly-1.4.1/lightly/cli/upload_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/cli/version_cli.py` & `lightly-1.4.1/lightly/cli/version_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/core.py` & `lightly-1.4.1/lightly/core.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/__init__.py` & `lightly-1.4.1/lightly/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/_helpers.py` & `lightly-1.4.1/lightly/data/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/_image.py` & `lightly-1.4.1/lightly/data/_image.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/_image_loaders.py` & `lightly-1.4.1/lightly/data/_image_loaders.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/_utils.py` & `lightly-1.4.1/lightly/data/_utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/_video.py` & `lightly-1.4.1/lightly/data/_video.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/collate.py` & `lightly-1.4.1/lightly/data/collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/dataset.py` & `lightly-1.4.1/lightly/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/lightly_subset.py` & `lightly-1.4.1/lightly/data/lightly_subset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/data/multi_view_collate.py` & `lightly-1.4.1/lightly/data/multi_view_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/embedding/_base.py` & `lightly-1.4.1/lightly/embedding/_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/embedding/callbacks.py` & `lightly-1.4.1/lightly/embedding/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/embedding/embedding.py` & `lightly-1.4.1/lightly/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/__init__.py` & `lightly-1.4.1/lightly/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/barlow_twins_loss.py` & `lightly-1.4.1/lightly/loss/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/dcl_loss.py` & `lightly-1.4.1/lightly/loss/dcl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/dino_loss.py` & `lightly-1.4.1/lightly/loss/dino_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/hypersphere_loss.py` & `lightly-1.4.1/lightly/loss/hypersphere_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/memory_bank.py` & `lightly-1.4.1/lightly/loss/memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/msn_loss.py` & `lightly-1.4.1/lightly/loss/msn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/negative_cosine_similarity.py` & `lightly-1.4.1/lightly/loss/negative_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/ntx_ent_loss.py` & `lightly-1.4.1/lightly/loss/ntx_ent_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/pmsn_loss.py` & `lightly-1.4.1/lightly/loss/pmsn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/regularizer/co2.py` & `lightly-1.4.1/lightly/loss/regularizer/co2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/swav_loss.py` & `lightly-1.4.1/lightly/loss/swav_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/sym_neg_cos_sim_loss.py` & `lightly-1.4.1/lightly/loss/sym_neg_cos_sim_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/tico_loss.py` & `lightly-1.4.1/lightly/loss/tico_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/vicreg_loss.py` & `lightly-1.4.1/lightly/loss/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/loss/vicregl_loss.py` & `lightly-1.4.1/lightly/loss/vicregl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/__init__.py` & `lightly-1.4.1/lightly/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/_momentum.py` & `lightly-1.4.1/lightly/models/_momentum.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/barlowtwins.py` & `lightly-1.4.1/lightly/models/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/batchnorm.py` & `lightly-1.4.1/lightly/models/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/byol.py` & `lightly-1.4.1/lightly/models/byol.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/moco.py` & `lightly-1.4.1/lightly/models/moco.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/modules/__init__.py` & `lightly-1.4.1/lightly/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/modules/heads.py` & `lightly-1.4.1/lightly/models/modules/heads.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/modules/masked_autoencoder.py` & `lightly-1.4.1/lightly/models/modules/masked_autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/modules/nn_memory_bank.py` & `lightly-1.4.1/lightly/models/modules/nn_memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/nnclr.py` & `lightly-1.4.1/lightly/models/nnclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/resnet.py` & `lightly-1.4.1/lightly/models/resnet.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/simclr.py` & `lightly-1.4.1/lightly/models/simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/simsiam.py` & `lightly-1.4.1/lightly/models/simsiam.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/utils.py` & `lightly-1.4.1/lightly/models/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/models/zoo.py` & `lightly-1.4.1/lightly/models/zoo.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/__init__.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/__init__.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/collaboration_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/collaboration_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/datasets_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/datasources_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/datasources_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/docker_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/docker_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/embeddings_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/jobs_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/mappings_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/mappings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/predictions_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/predictions_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/quota_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/quota_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/samples_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/samples_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/samplings_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/samplings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/scores_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/scores_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/tags_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/teams_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api/versioning_api.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api/versioning_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/api_client.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/configuration.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/__init__.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/access_role.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/access_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/active_learning_scores.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/active_learning_scores.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/api_error_code.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/api_error_code.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/api_error_response.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/async_task_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/async_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/bounding_box.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/category_id.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/category_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/category_name.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/category_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_entry.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_set_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_set_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/create_entity_response.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/create_entity_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/creator.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/crop_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/crop_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_creator.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_name.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_name_query.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_name_query.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dataset_update_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dataset_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_base.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_local.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_local.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_purpose.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_purpose.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_license_information.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_license_information.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_state.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_task_description.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_task_description.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_user_stats.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_user_stats.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_name.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_state.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/docker_worker_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/docker_worker_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding2d_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding2d_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/embedding_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/file_name_format.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/file_name_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/file_output_format.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/file_output_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/general_job_result.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/general_job_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/image_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/image_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_result_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_result_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_state.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_data_result.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_data_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_meta.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_meta.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/jobs_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/jobs_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_data_row.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_studio_task.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_studio_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/mongo_object_id.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/mongo_object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/object_id.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/path_safe_name.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/path_safe_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_singletons.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/probabilities.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/probabilities.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/questionnaire_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/questionnaire_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/read_url.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/redirected_read_url.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/redirected_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/s3_region.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/s3_region.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sama_task.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sama_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sama_task_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sama_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sama_tasks.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sama_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_data_modes.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_data_modes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_meta_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_sort_by.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_sort_by.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_update_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sample_write_urls.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sample_write_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_config.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sampling_method.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sampling_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/score.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/score.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/sector.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/sector.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config_entry.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_input_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_input_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/shared_access_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/shared_access_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_change_entry.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_change_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_create_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_creator.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_name.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_update_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/task_name.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/task_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/task_type.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/task_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/team_basic_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/team_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/team_role.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/team_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/timestamp.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/version_number.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/version_number.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/video_frame_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/video_frame_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/openapi_generated/swagger_client/rest.py` & `lightly-1.4.1/lightly/openapi_generated/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/__init__.py` & `lightly-1.4.1/lightly/transforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 from lightly.transforms.dino_transform import DINOTransform, DINOViewTransform
+from lightly.transforms.fast_siam_transform import FastSiamTransform
 from lightly.transforms.gaussian_blur import GaussianBlur
 from lightly.transforms.jigsaw import Jigsaw
 from lightly.transforms.mae_transform import MAETransform
 from lightly.transforms.moco_transform import MoCoV1Transform, MoCoV2Transform
 from lightly.transforms.msn_transform import MSNTransform, MSNViewTransform
 from lightly.transforms.pirl_transform import PIRLTransform
 from lightly.transforms.rotation import (
     RandomRotate,
     RandomRotateDegrees,
     random_rotation_transform,
 )
 from lightly.transforms.simclr_transform import SimCLRTransform, SimCLRViewTransform
+from lightly.transforms.simsiam_transform import SimSiamTransform, SimSiamViewTransform
 from lightly.transforms.smog_transform import SMoGTransform, SmoGViewTransform
 from lightly.transforms.solarize import RandomSolarization
 from lightly.transforms.swav_transform import SwaVTransform, SwaVViewTransform
 from lightly.transforms.vicreg_transform import VICRegTransform, VICRegViewTransform
 from lightly.transforms.vicregl_transform import VICRegLTransform, VICRegLViewTransform
```

### Comparing `lightly-1.4.0/lightly/transforms/dino_transform.py` & `lightly-1.4.1/lightly/transforms/dino_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/gaussian_blur.py` & `lightly-1.4.1/lightly/transforms/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/image_grid_transform.py` & `lightly-1.4.1/lightly/transforms/image_grid_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/jigsaw.py` & `lightly-1.4.1/lightly/transforms/jigsaw.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/mae_transform.py` & `lightly-1.4.1/lightly/transforms/mae_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/moco_transform.py` & `lightly-1.4.1/lightly/transforms/moco_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/msn_transform.py` & `lightly-1.4.1/lightly/transforms/msn_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/multi_crop_transform.py` & `lightly-1.4.1/lightly/transforms/multi_crop_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/multi_view_transform.py` & `lightly-1.4.1/lightly/transforms/multi_view_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/pirl_transform.py` & `lightly-1.4.1/lightly/transforms/pirl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/random_crop_and_flip_with_grid.py` & `lightly-1.4.1/lightly/transforms/random_crop_and_flip_with_grid.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/rotation.py` & `lightly-1.4.1/lightly/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/simclr_transform.py` & `lightly-1.4.1/lightly/transforms/simclr_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/smog_transform.py` & `lightly-1.4.1/lightly/transforms/smog_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/solarize.py` & `lightly-1.4.1/lightly/transforms/solarize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/swav_transform.py` & `lightly-1.4.1/lightly/transforms/swav_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/vicreg_transform.py` & `lightly-1.4.1/lightly/transforms/vicreg_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/transforms/vicregl_transform.py` & `lightly-1.4.1/lightly/transforms/vicregl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/benchmarking.py` & `lightly-1.4.1/lightly/utils/benchmarking.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/cropping/crop_image_by_bounding_boxes.py` & `lightly-1.4.1/lightly/utils/cropping/crop_image_by_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/cropping/read_yolo_label_file.py` & `lightly-1.4.1/lightly/utils/cropping/read_yolo_label_file.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/debug.py` & `lightly-1.4.1/lightly/utils/debug.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/dist.py` & `lightly-1.4.1/lightly/utils/dist.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/embeddings_2d.py` & `lightly-1.4.1/lightly/utils/embeddings_2d.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/hipify.py` & `lightly-1.4.1/lightly/utils/hipify.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/io.py` & `lightly-1.4.1/lightly/utils/io.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/reordering.py` & `lightly-1.4.1/lightly/utils/reordering.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/scheduler.py` & `lightly-1.4.1/lightly/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly/utils/version_compare.py` & `lightly-1.4.1/lightly/utils/version_compare.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/lightly.egg-info/PKG-INFO` & `lightly-1.4.1/lightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.0
+Version: 1.4.1
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.0/lightly.egg-info/SOURCES.txt` & `lightly-1.4.1/lightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -344,26 +344,28 @@
 lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
 lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
 lightly/openapi_generated/swagger_client/models/version_number.py
 lightly/openapi_generated/swagger_client/models/video_frame_data.py
 lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
 lightly/transforms/__init__.py
 lightly/transforms/dino_transform.py
+lightly/transforms/fast_siam_transform.py
 lightly/transforms/gaussian_blur.py
 lightly/transforms/image_grid_transform.py
 lightly/transforms/jigsaw.py
 lightly/transforms/mae_transform.py
 lightly/transforms/moco_transform.py
 lightly/transforms/msn_transform.py
 lightly/transforms/multi_crop_transform.py
 lightly/transforms/multi_view_transform.py
 lightly/transforms/pirl_transform.py
 lightly/transforms/random_crop_and_flip_with_grid.py
 lightly/transforms/rotation.py
 lightly/transforms/simclr_transform.py
+lightly/transforms/simsiam_transform.py
 lightly/transforms/smog_transform.py
 lightly/transforms/solarize.py
 lightly/transforms/swav_transform.py
 lightly/transforms/utils.py
 lightly/transforms/vicreg_transform.py
 lightly/transforms/vicregl_transform.py
 lightly/utils/__init__.py
```

### Comparing `lightly-1.4.0/lightly.egg-info/requires.txt` & `lightly-1.4.1/lightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.0/setup.py` & `lightly-1.4.1/setup.py`

 * *Files identical despite different names*

