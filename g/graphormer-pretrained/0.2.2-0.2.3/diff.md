# Comparing `tmp/graphormer-pretrained-0.2.2.tar.gz` & `tmp/graphormer-pretrained-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphormer-pretrained-0.2.2.tar", last modified: Sun Mar 26 16:28:10 2023, max compression
+gzip compressed data, was "graphormer-pretrained-0.2.3.tar", last modified: Tue Apr 11 18:33:13 2023, max compression
```

## Comparing `graphormer-pretrained-0.2.2.tar` & `graphormer-pretrained-0.2.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.367822 graphormer-pretrained-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.359822 graphormer-pretrained-0.2.2/graphormer_pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.359822 graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/binary_logloss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/mae_deltapos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/multiclass_cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/data/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   349339 2023-03-26 16:28:09.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/algos.c
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/algos.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/data/ogb_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/ogb_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/ogb_datasets/ogb_dataset_lookup_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/data/pyg_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/pyg_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/pyg_datasets/pyg_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/pyg_datasets/pyg_dataset_lookup_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/data/smiles_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/smiles_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/smiles_dataset/smiles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/data/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/evaluate/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/models/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/models/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/models/graphormer_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/modules/graphormer_graph_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/modules/graphormer_graph_encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/modules/graphormer_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/modules/multihead_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/tasks/graph_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/tasks/is2re.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/graphormer_pretrained/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/utils/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/graphormer_pretrained/utils/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.359822 graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-03-26 16:28:10.000000 graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-26 16:28:10.000000 graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 16:28:10.000000 graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 16:27:57.000000 graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-26 16:28:10.000000 graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 16:28:10.000000 graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 16:28:10.367822 graphormer-pretrained-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 16:28:10.363822 graphormer-pretrained-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-26 16:26:08.000000 graphormer-pretrained-0.2.2/tests/test_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.831048 graphormer-pretrained-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-11 18:33:13.831048 graphormer-pretrained-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.823047 graphormer-pretrained-0.2.3/graphormer_pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/binary_logloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/mae_deltapos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/multiclass_cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   350993 2023-04-11 18:33:13.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/algos.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/algos.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/data/ogb_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/ogb_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/ogb_datasets/ogb_dataset_lookup_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/data/pyg_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/pyg_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/pyg_datasets/pyg_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/pyg_datasets/pyg_dataset_lookup_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/data/smiles_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/smiles_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/smiles_dataset/smiles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/data/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/evaluate/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/models/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/models/graphormer_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/modules/graphormer_graph_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/modules/graphormer_graph_encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/modules/graphormer_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/modules/multihead_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.831048 graphormer-pretrained-0.2.3/graphormer_pretrained/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/tasks/graph_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/tasks/is2re.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.831048 graphormer-pretrained-0.2.3/graphormer_pretrained/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/utils/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/graphormer_pretrained/utils/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.827048 graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-11 18:33:13.000000 graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-11 18:33:13.000000 graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:33:13.000000 graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:32:58.000000 graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 18:33:13.000000 graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 18:33:13.000000 graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:33:13.831048 graphormer-pretrained-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:33:13.831048 graphormer-pretrained-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-11 18:30:59.000000 graphormer-pretrained-0.2.3/tests/test_embeddings.py
```

### Comparing `graphormer-pretrained-0.2.2/LICENSE` & `graphormer-pretrained-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/PKG-INFO` & `graphormer-pretrained-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphormer-pretrained
-Version: 0.2.2
+Version: 0.2.3
 Summary: Packaging of Graphormer is a deep learning package by Microsoft that allows researchers and developers to train custom models for molecule modeling tasks.
 Author-email: Emmanuel Noutahi <emmanuel@valencediscovery.com>
 License: MIT
 Project-URL: Source Code, https://github.com/maclandrol/graphormer-pretrained
 Project-URL: Bug Tracker, https://github.com/maclandrol/graphormer-pretrained/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: graphormer-pretrained Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: graphormer-pretrained Version: 0.2.3 Summary:
 Packaging of Graphormer is a deep learning package by Microsoft that allows
 researchers and developers to train custom models for molecule modeling tasks.
 Author-email: Emmanuel Noutahi
 valencediscovery.com> License: MIT Project-URL: Source Code, https://
 github.com/maclandrol/graphormer-pretrained Project-URL: Bug Tracker, https://
 github.com/maclandrol/graphormer-pretrained/issues Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [assets/logo-
```

### Comparing `graphormer-pretrained-0.2.2/README.md` & `graphormer-pretrained-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/binary_logloss.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/binary_logloss.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/l1_loss.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/l1_loss.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/mae_deltapos.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/mae_deltapos.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/criterions/multiclass_cross_entropy.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/criterions/multiclass_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/algos.c` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/algos.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "graphormer_pretrained.data.algos",
         "sources": [
             "graphormer_pretrained/data/algos.pyx"
         ]
     },
     "module_name": "graphormer_pretrained.data.algos"
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -221,15 +221,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -260,15 +260,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1041,195 +1041,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1256,42 +1256,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1637,20 +1637,28 @@
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -3706,15 +3714,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_edge_fea_all);
   __Pyx_XDECREF(__pyx_v_path);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3723,29 +3731,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3756,15 +3764,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3773,29 +3781,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3806,15 +3814,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3823,29 +3831,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3856,15 +3864,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3873,29 +3881,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3906,15 +3914,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3923,29 +3931,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3956,212 +3964,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4177,15 +4185,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4193,53 +4201,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4247,30 +4255,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4285,15 +4293,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4309,15 +4317,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4325,53 +4333,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4379,30 +4387,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4417,15 +4425,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4441,15 +4449,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4457,53 +4465,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4511,30 +4519,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4549,176 +4557,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4846,26 +4854,26 @@
  * 
  *     return edge_fea_all
  */
   __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -4979,52 +4987,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -5301,15 +5324,15 @@
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../tmp/build-env-0hxx17ve/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-4rss8vcs/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6953,70 +6976,88 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/algos.pyx` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/algos.pyx`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/collator.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/collator.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/dataset.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/dataset.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/ogb_datasets/ogb_dataset_lookup_table.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/ogb_datasets/ogb_dataset_lookup_table.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/pyg_datasets/pyg_dataset.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/pyg_datasets/pyg_dataset.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/pyg_datasets/pyg_dataset_lookup_table.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/pyg_datasets/pyg_dataset_lookup_table.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/smiles_dataset/smiles_dataset.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/smiles_dataset/smiles_dataset.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/data/wrapper.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/data/wrapper.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/evaluate/evaluate.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/models/graphormer.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/models/graphormer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Licensed under the MIT License.
 
 # Copyright (c) Facebook, Inc. and its affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-import logging
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from fairseq import utils
 from fairseq.models import (
     FairseqEncoder,
@@ -21,16 +20,15 @@
 from fairseq.modules import (
     LayerNorm,
 )
 
 from graphormer_pretrained.utils.loader import load_pretrained_model
 from graphormer_pretrained.utils.common import safe_hasattr
 from graphormer_pretrained.modules import init_graphormer_params, GraphormerGraphEncoder
-
-logger = logging.getLogger(__name__)
+from loguru import logger
 
 
 @register_model("graphormer")
 class GraphormerModel(FairseqEncoderModel):
     def __init__(self, args, encoder):
         super().__init__(encoder)
         self.args = args
@@ -179,14 +177,15 @@
 
         self.lm_head_transform_weight = nn.Linear(args.encoder_embed_dim, args.encoder_embed_dim)
         self.activation_fn = utils.get_activation_fn(args.activation_fn)
         self.layer_norm = LayerNorm(args.encoder_embed_dim)
 
         self.lm_output_learned_bias = None
         if self.load_softmax:
+            print("WHY are we loading softmax ?")
             self.lm_output_learned_bias = nn.Parameter(torch.zeros(1))
 
             if not self.share_input_output_embed:
                 self.embed_out = nn.Linear(args.encoder_embed_dim, args.num_classes, bias=False)
             else:
                 raise NotImplementedError
 
@@ -204,23 +203,23 @@
         x = inner_states[-1].transpose(0, 1)
 
         # project masked tokens only
         if masked_tokens is not None:
             raise NotImplementedError
 
         x = self.layer_norm(self.activation_fn(self.lm_head_transform_weight(x)))
-
         # project back to size of vocabulary
         if self.share_input_output_embed and hasattr(self.graph_encoder.embed_tokens, "weight"):
+            # EN: we should never reach this
             x = F.linear(x, self.graph_encoder.embed_tokens.weight)
         elif self.embed_out is not None:
+            # EN: we should never reach this
             x = self.embed_out(x)
         if self.lm_output_learned_bias is not None:
             x = x + self.lm_output_learned_bias
-
         return x
 
     def max_nodes(self):
         """Maximum output length supported by the encoder."""
         return self.max_nodes
 
     def upgrade_state_dict_named(self, state_dict, name):
```

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/models/graphormer_3d.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/models/graphormer_3d.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/modules/graphormer_graph_encoder.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/modules/graphormer_graph_encoder.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/modules/graphormer_graph_encoder_layer.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/modules/graphormer_graph_encoder_layer.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/modules/graphormer_layers.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/modules/graphormer_layers.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/modules/multihead_attention.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/modules/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/tasks/graph_prediction.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/tasks/graph_prediction.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/tasks/is2re.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/tasks/is2re.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/utils/amp_optimizer.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/utils/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained/utils/loader.py` & `graphormer-pretrained-0.2.3/graphormer_pretrained/utils/loader.py`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/PKG-INFO` & `graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphormer-pretrained
-Version: 0.2.2
+Version: 0.2.3
 Summary: Packaging of Graphormer is a deep learning package by Microsoft that allows researchers and developers to train custom models for molecule modeling tasks.
 Author-email: Emmanuel Noutahi <emmanuel@valencediscovery.com>
 License: MIT
 Project-URL: Source Code, https://github.com/maclandrol/graphormer-pretrained
 Project-URL: Bug Tracker, https://github.com/maclandrol/graphormer-pretrained/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: graphormer-pretrained Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: graphormer-pretrained Version: 0.2.3 Summary:
 Packaging of Graphormer is a deep learning package by Microsoft that allows
 researchers and developers to train custom models for molecule modeling tasks.
 Author-email: Emmanuel Noutahi
 valencediscovery.com> License: MIT Project-URL: Source Code, https://
 github.com/maclandrol/graphormer-pretrained Project-URL: Bug Tracker, https://
 github.com/maclandrol/graphormer-pretrained/issues Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [assets/logo-
```

### Comparing `graphormer-pretrained-0.2.2/graphormer_pretrained.egg-info/SOURCES.txt` & `graphormer-pretrained-0.2.3/graphormer_pretrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphormer-pretrained-0.2.2/pyproject.toml` & `graphormer-pretrained-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel", "cython", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "graphormer-pretrained"
 description = "Packaging of Graphormer is a deep learning package by Microsoft that allows researchers and developers to train custom models for molecule modeling tasks."
-version = "0.2.2" # project
+version = "0.2.3" # project
 authors = [
     { name = "Emmanuel Noutahi", email = "emmanuel@valencediscovery.com" },
 ]
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.8"
 dependencies = [
```

