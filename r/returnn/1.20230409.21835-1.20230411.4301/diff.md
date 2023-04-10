# Comparing `tmp/returnn-1.20230409.21835.tar.gz` & `tmp/returnn-1.20230411.4301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230409.21835.tar", last modified: Sun Apr  9 00:34:28 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230411.4301.tar", last modified: Mon Apr 10 23:03:27 2023, max compression
```

## Comparing `returnn-1.20230409.21835.tar` & `returnn-1.20230411.4301.tar`

### file list

```diff
@@ -1,410 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63018 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-09 00:34:02.000000 returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36530 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93069 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   155711 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   150268 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   148678 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   582337 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292822 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144495 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/py-to-pickle.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187447 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:34:28.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-09 00:33:59.000000 returnn-1.20230409.21835/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63018 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 23:03:06.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-10 23:03:10.000000 returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25787 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36530 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94908 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154928 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150268 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148678 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   584733 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18948 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144495 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/py-to-pickle.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187447 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:03:27.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-10 23:03:04.000000 returnn-1.20230411.4301/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230409.21835/.gitignore` & `returnn-1.20230411.4301/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/.gitmodules` & `returnn-1.20230411.4301/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/CHANGELOG.md` & `returnn-1.20230411.4301/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/CODEOWNERS` & `returnn-1.20230411.4301/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/CONTRIBUTING.md` & `returnn-1.20230411.4301/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/LICENSE` & `returnn-1.20230411.4301/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/MANIFEST.in` & `returnn-1.20230411.4301/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/PKG-INFO` & `returnn-1.20230411.4301/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230409.21835
+Version: 1.20230411.4301
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230409.21835/README.rst` & `returnn-1.20230411.4301/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/__init__.py` & `returnn-1.20230411.4301/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/12AX.cluster_map` & `returnn-1.20230411.4301/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-fwd.config` & `returnn-1.20230411.4301/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-horovod-mpi.py` & `returnn-1.20230411.4301/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230411.4301/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-hyper-param-tuning.config` & `returnn-1.20230411.4301/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-iter-dataset.py` & `returnn-1.20230411.4301/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-list-devices.py` & `returnn-1.20230411.4301/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-lua-torch-layer.config` & `returnn-1.20230411.4301/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230411.4301/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-returnn-as-framework.py` & `returnn-1.20230411.4301/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-rf.config` & `returnn-1.20230411.4301/demos/demo-rf.config`

 * *Files 7% similar despite different names*

```diff
@@ -45,17 +45,18 @@
 
 def get_model(**_kwargs):
     return Model()
 
 def train_step(*, model: Model, extern_data, **_kwargs):
     data = extern_data["data"]
     logits = model(data)
+    logits_packed, pack_dim = rf.pack(logits, dims=(batch_dim, time_dim), enforce_sorted=False)
     targets = extern_data["classes"]
-    # TODO: use flattening on logits/targets
-    loss = rf.cross_entropy(estimated=logits, estimated_type="logits", target=targets, axis=out_dim)
+    targets_packed, _ = rf.pack(targets, dims=(batch_dim, time_dim), enforce_sorted=False, out_dim=pack_dim)
+    loss = rf.cross_entropy(estimated=logits_packed, estimated_type="logits", target=targets_packed, axis=out_dim)
     loss.mark_as_loss(name="ce")
 
 
 # training
 optimizer = {"class": "adam"}
 
 learning_rate = 0.01
```

### Comparing `returnn-1.20230409.21835/demos/demo-rhn-enwik8.config` & `returnn-1.20230411.4301/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-sprint-interface.py` & `returnn-1.20230411.4301/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-att-copy.config` & `returnn-1.20230411.4301/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-attention.config` & `returnn-1.20230411.4301/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-enc-dec.config` & `returnn-1.20230411.4301/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230411.4301/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230411.4301/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230411.4301/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230411.4301/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-rec-self-att.config` & `returnn-1.20230411.4301/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230411.4301/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230411.4301/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-torch.config` & `returnn-1.20230411.4301/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/demo.sh` & `returnn-1.20230411.4301/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/README.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/config_demo` & `returnn-1.20230411.4301/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230411.4301/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/config_real` & `returnn-1.20230411.4301/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230411.4301/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/decode.py` & `returnn-1.20230411.4301/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230411.4301/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230411.4301/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/__init__.py` & `returnn-1.20230411.4301/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/__main__.py` & `returnn-1.20230411.4301/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/__old_mod_loader__.py` & `returnn-1.20230411.4301/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/__setup__.py` & `returnn-1.20230411.4301/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/config.py` & `returnn-1.20230411.4301/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/audio.py` & `returnn-1.20230411.4301/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/basic.py` & `returnn-1.20230411.4301/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/bundle_file.py` & `returnn-1.20230411.4301/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/cached.py` & `returnn-1.20230411.4301/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/cached2.py` & `returnn-1.20230411.4301/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/generating.py` & `returnn-1.20230411.4301/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/hdf.py` & `returnn-1.20230411.4301/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/lm.py` & `returnn-1.20230411.4301/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/map.py` & `returnn-1.20230411.4301/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/meta.py` & `returnn-1.20230411.4301/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/multi_proc.py` & `returnn-1.20230411.4301/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/normalization_data.py` & `returnn-1.20230411.4301/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/numpy_dump.py` & `returnn-1.20230411.4301/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/raw_wav.py` & `returnn-1.20230411.4301/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/sprint.py` & `returnn-1.20230411.4301/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/stereo.py` & `returnn-1.20230411.4301/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230411.4301/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/datasets/util/vocabulary.py` & `returnn-1.20230411.4301/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/engine/base.py` & `returnn-1.20230411.4301/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/engine/batch.py` & `returnn-1.20230411.4301/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/graph_editor/edit.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/graph_editor/select.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/graph_editor/transform.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/extern/graph_editor/util.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/__init__.py` & `returnn-1.20230411.4301/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/_backend.py` & `returnn-1.20230411.4301/returnn/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,24 @@
         backend = get_backend_by_raw_tensor_type(type(raw_tensor))
         existing_shape = backend.get_known_shape_raw(raw_tensor)
         assert all(dim is not None for dim in existing_shape)
         assert len(shape) == len(existing_shape)
         assert all(dim is None or dim == existing_shape[i] for i, dim in enumerate(shape))
 
     @staticmethod
+    def get_new_dim_raw(raw_tensor: T, axis: int, *, name: str) -> Dim:
+        """
+        :param raw_tensor:
+        :param axis:
+        :param name:
+        :return: dim tag of axis
+        """
+        raise NotImplementedError
+
+    @staticmethod
     def fill_raw(shape: Union[Sequence[Union[int, T]], T], value: Union[Any, T]) -> T:
         """
         :param shape: shape
         :param value: scalar value to fill
         :return: raw tensor filled with value everywhere
         """
         raise NotImplementedError
@@ -227,14 +237,33 @@
         # Default implementation using cast_raw.
         res = tensor.copy_template()
         res.dtype = dtype
         # noinspection PyProtectedMember
         res.raw_tensor = tensor._raw_backend.cast_raw(tensor.raw_tensor, dtype)
         return res
 
+    @staticmethod
+    def merge_dims(
+        source: Tensor,
+        *,
+        dims: Sequence[Dim],
+        out_dim: Optional[Dim] = None,
+    ) -> Tuple[Tensor, Dim]:
+        """
+        Merges a list of axes into a single one. (Flatten the dims.)
+        E.g. input is (batch, width, height, dim) and dims=(width,height), then we get (batch, width*height, dim).
+        Or input is (batch, time, height, dim) and axes=(height,dim), then we get (batch, time, height*dim).
+
+        :param nn.Tensor source:
+        :param dims:
+        :param out_dim:
+        :return: tensor, out_dim
+        """
+        raise NotImplementedError
+
     # Restrict the possible activation function names,
     # to not get unexpected behavior,
     # or unwanted incompatibilities.
     _AllowedActivationFuncs = {
         "exp",
         "expm1",
         "log",
@@ -424,20 +453,22 @@
     @staticmethod
     def convert_to_tensor(
         value: Union[Tensor, T, RawTensorTypes],
         *,
         dims: Sequence[Dim],
         dtype: str,
         sparse_dim: Optional[Dim] = None,
+        name: Optional[str] = None,
     ) -> Tensor[T]:
         """
         :param value: tensor, or scalar raw tensor or some other scalar value
         :param dims:
         :param dtype:
         :param sparse_dim:
+        :param name:
         :return: tensor
         """
         raise NotImplementedError
 
     @staticmethod
     def full(
         dims: Sequence[Dim], fill_value: RawTensorTypes, *, dtype: str, sparse_dim: Optional[Dim] = None
@@ -607,14 +638,29 @@
         out: Optional[Tensor] = None,
     ) -> Tensor:
         """
         random. See `rf.random` for details.
         """
         raise NotImplementedError
 
+    @staticmethod
+    def masked_select(
+        tensor: Tensor, *, mask: Tensor, dims: Sequence[Dim], out_dim: Optional[Dim] = None
+    ) -> Tuple[Tensor, Dim]:
+        """
+        :param tensor:
+        :param mask:
+        :param dims: the order of the dims defines the format. those dims should be exactly the dims of the mask.
+        :param out_dim:
+        :return: tensor where all dims in mask/dims are removed and replaced by a new dim.
+            the new dim is also returned.
+            if mask==True for all elements, the returned tensor would be simply the flattened input tensor.
+        """
+        raise NotImplementedError
+
 
 # We use a global instance, and we modify __class__ inplace,
 # such that any reference to this can be updated.
 # This is exposed to the user as `returnn.frontend`.
 # The __class__ assignment is done in `select_engine`.
 # Use object.__new__ because we disallow creating instances of Frontend.
 global_backend = object.__new__(Backend)
```

### Comparing `returnn-1.20230409.21835/returnn/frontend/_numpy_backend.py` & `returnn-1.20230411.4301/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/_utils.py` & `returnn-1.20230411.4301/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/const.py` & `returnn-1.20230411.4301/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/dims.py` & `returnn-1.20230411.4301/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/dtype.py` & `returnn-1.20230411.4301/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/init.py` & `returnn-1.20230411.4301/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/linear.py` & `returnn-1.20230411.4301/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/loss.py` & `returnn-1.20230411.4301/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/math_.py` & `returnn-1.20230411.4301/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/matmul.py` & `returnn-1.20230411.4301/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/module.py` & `returnn-1.20230411.4301/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/parameter.py` & `returnn-1.20230411.4301/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/rand.py` & `returnn-1.20230411.4301/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/reduce.py` & `returnn-1.20230411.4301/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/run_ctx.py` & `returnn-1.20230411.4301/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/state.py` & `returnn-1.20230411.4301/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/frontend/types.py` & `returnn-1.20230411.4301/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/import_/common.py` & `returnn-1.20230411.4301/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/import_/git.py` & `returnn-1.20230411.4301/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/import_/import_.py` & `returnn-1.20230411.4301/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/learning_rate_control.py` & `returnn-1.20230411.4301/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/log.py` & `returnn-1.20230411.4301/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/native_op.cpp` & `returnn-1.20230411.4301/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/native_op.py` & `returnn-1.20230411.4301/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/pretrain.py` & `returnn-1.20230411.4301/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/sprint/cache.py` & `returnn-1.20230411.4301/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/sprint/control.py` & `returnn-1.20230411.4301/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/sprint/error_signals.py` & `returnn-1.20230411.4301/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/sprint/extern_interface.py` & `returnn-1.20230411.4301/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/sprint/interface.py` & `returnn-1.20230411.4301/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tensor/_dim_extra.py` & `returnn-1.20230411.4301/returnn/tensor/_dim_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Backwards-compatible functions and attribs for the old ``Dim`` class,
 or just rarely used attribs, such that we can save memory for the common case.
 """
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Union, Tuple, Dict, List
+from typing import TYPE_CHECKING, Optional, Union, Tuple, Sequence, Dict, List
 
 from returnn.util.basic import Entity
 from returnn.util import basic as util
 
 if TYPE_CHECKING:
     # Those are only used for TensorFlow, or they are deprecated.
     from returnn.tf.util.data import BatchInfo, ControlFlowContext
@@ -686,14 +686,49 @@
                 batch_dim_axis=0,
                 batch=self.batch,
                 beam=beam,
                 control_flow_ctx=self.control_flow_ctx,
             )
         self.dyn_size_ext.placeholder = dyn_size
 
+    def get_mask(self: Dim, *, dim_order: Optional[Sequence[Dim]] = None) -> _t.Tensor:
+        """
+        :param dim_order: if given, the dims of the mask will be in this order.
+            This can be useful if the mask is broadcasted against some other tensor.
+        :return: if need_masking(), the corresponding mask.
+            If this is e.g. the time-dim T of shape [B], then the mask will be of shape [B,T].
+            The mask could be used with :func:`masked_select` (``boolean_mask``) or ``where``.
+        """
+        import returnn.frontend as rf
+
+        assert self.dyn_size_ext and self.dyn_size_ext.raw_tensor is not None
+        # noinspection PyProtectedMember
+        backend = self.dyn_size_ext._raw_backend
+
+        max_idx = rf.reduce(
+            self.dyn_size_ext,
+            axis=self.dyn_size_ext.dims,
+            mode="max",
+            # Masking here is not always possible, e.g. if we have
+            # tag = Dim{'self-att-keys'['time:var:extern_data:classes'[B]]}
+            use_time_mask=False,
+        )
+        # We use the assumption that self.placeholder.shape[axis] == max_idx.
+        # size_ext might have invalid (zero) sizes
+        # when it itself has some padding, e.g. when its own shape is dynamic.
+        # A zero size can lead to problems in some cases, e.g. in SoftmaxOverSpatialLayer,
+        # when everything is masked to -inf, it results in nan,
+        # and this likely produces nan in backprop or elsewhere.
+        # Thus, mask size_ext itself, and set the padded values to 1.
+        # This assumes that max_idx >= 1.
+        size_ext = self.dyn_size_ext.copy_masked(max_idx)
+        idx_range = backend.range_over_dim(self)
+        seq_mask = rf.compare(idx_range, "<", size_ext, allow_broadcast_all_sources=True, dim_order=dim_order)
+        return seq_mask
+
     def is_batch_dim(self):
         """
         :return: whether this dim tag is of kind batch
         :rtype: bool
         """
         return self.kind == DimTypes.Batch
```

### Comparing `returnn-1.20230409.21835/returnn/tensor/_tensor_extra.py` & `returnn-1.20230411.4301/returnn/tensor/_tensor_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -2657,16 +2657,14 @@
         :param int|None axis:
         :return: seq mask of shape ((batch,time) or (time,batch)) + (1,)s for remaining dims
           if BT or TB major, and axis is T or None.
           In general compatible to placeholder, i.e. same ndim, with broadcast dims.
           We assert here that the axis is dynamic (:func:`is_axis_dynamic`), i.e. we have the size.
         :rtype: tf.Tensor
         """
-        import returnn.frontend as rf
-
         if axis is None:
             assert self.time_dim_axis is not None
             axis = self.time_dim_axis
         if axis < 0:
             assert axis + self.batch_ndim > 0
             axis += self.batch_ndim
         assert 0 <= axis < self.batch_ndim
@@ -2688,39 +2686,34 @@
                 seq_mask = backend.sequence_mask_raw(size, batch_major=axis >= self.batch_dim_axis)  # (B,T) or (T,B)
                 shape = [1] * self.batch_ndim  # type: List[Union[int,_t.RawTensorType]]
                 shape[self.batch_dim_axis] = self.get_batch_dim()
                 shape[axis] = tag.get_dim_value()
                 seq_mask = backend.reshape_raw(seq_mask, shape)
                 assert seq_mask.get_shape().ndims == self.batch_ndim
             else:  # size is something unusual, not just [B], but e.g. [B,S] or so
-                max_idx = rf.reduce(
-                    tag.dyn_size_ext,
-                    axis=tag.dyn_size_ext.dims,
-                    mode="max",
-                    # Masking here is not always possible, e.g. if we have
-                    # tag = Dim{'self-att-keys'['time:var:extern_data:classes'[B]]}
-                    use_time_mask=False,
-                ).raw_tensor
-                # We use the assumption that self.placeholder.shape[axis] == max_idx.
-                # size_ext might have invalid (zero) sizes
-                # when it itself has some padding, e.g. when its own shape is dynamic.
-                # A zero size can lead to problems in some cases, e.g. in SoftmaxOverSpatialLayer,
-                # when everything is masked to -inf, it results in nan,
-                # and this likely produces nan in backprop or elsewhere.
-                # Thus, mask size_ext itself, and set the padded values to 1.
-                # This assumes that max_idx >= 1.
-                size_ext = tag.dyn_size_ext.copy_masked(max_idx)
-                idx_range = backend.range_over_dim(tag)
                 seq_mask = (
-                    rf.compare(idx_range, "<", size_ext, allow_broadcast_all_sources=True, dim_order=self.dims)
+                    self.get_sequence_mask_tensor(axis)
                     .copy_compatible_to(self, check_dtype=False, check_sparse=False)
                     .raw_tensor
                 )
         return seq_mask
 
+    def get_sequence_mask_tensor(self: Tensor, axis: int) -> Tensor:
+        """
+        :param axis:
+        :return: mask
+        """
+        if axis < 0:
+            assert axis + self.batch_ndim > 0
+            axis += self.batch_ndim
+        assert 0 <= axis < self.batch_ndim
+        assert axis != self.batch_dim_axis
+        tag: Dim = self.dim_tags[axis]
+        return tag.get_mask(dim_order=self.dims)
+
     def get_sequence_lengths_broadcast(self, axis=None):
         """
         :param int|None axis:
         :return: seq len of some shape which is broadcastable to self.placeholder.
           Note that this is not always possible, e.g. when the seq len has shape [B]
           but the tensor has just shape [T]. We currently throw an error then.
         :rtype: tf.Tensor
@@ -2767,15 +2760,15 @@
                 dims.remove(dim_)
             n_ = rf.reduce_sum(dim.dyn_size_ext, axis=dim.dyn_size_ext.dims)
             n *= n_
         return n
 
     def copy_masked(self: Tensor, mask_value) -> Tensor:
         """
-        :param float|int|tf.Tensor mask_value:
+        :param float|int|tf.Tensor|Tensor mask_value:
         """
         assert self.placeholder is not None
         if not any(dim.need_masking() for dim in self.dims):
             return self.copy()
         assert self._raw_backend.is_tensorflow  # not implemented otherwise for now
         from returnn.tf.util.basic import mask_dyn_seq_len_nd
```

### Comparing `returnn-1.20230409.21835/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230411.4301/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230411.4301/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230411.4301/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tensor/dim.py` & `returnn-1.20230411.4301/returnn/tensor/dim.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
             self.capacity = capacity or dimension
             self.size = dimension
             self.dyn_size_ext = None
         elif isinstance(dimension, _t.Tensor):
             self.capacity = capacity
             self.size = None
             self.dyn_size_ext = dimension.copy()
+        else:
+            raise TypeError(f"unexpected dimension type: {type(dimension)}")
         if not name and not description and self.dyn_size_ext:
             name = self.dyn_size_ext.name
         self.name = name or description
         self._extra = None
 
         if kwargs:
             self._handle_extra_kwargs(**kwargs)
```

### Comparing `returnn-1.20230409.21835/returnn/tensor/marked_dim.py` & `returnn-1.20230411.4301/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tensor/tensor.py` & `returnn-1.20230411.4301/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tensor/tensor_dict.py` & `returnn-1.20230411.4301/returnn/tensor/tensor_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,29 +54,34 @@
     def __getitem__(self, item: str) -> Tensor:
         return self.data[item]
 
     def copy_template(self) -> TensorDict:
         """copy template"""
         return TensorDict({k: v.copy_template() for k, v in self.data.items()})
 
-    def as_raw_tensor_dict(self) -> Dict[str, Any]:
+    def as_raw_tensor_dict(self, *, include_const_sizes: bool = False) -> Dict[str, Any]:
         """
         :return: dict of raw tensors, including any sequence lengths / dynamic sizes
         """
         out = {}
         for key, value in self.data.items():
             assert key not in out
             out[key] = value.raw_tensor
             for i, dim in enumerate(value.dims):
                 key_ = f"{key}:size{i}"
                 assert key_ not in out
                 if dim.is_batch_dim() and (not dim.dyn_size_ext or dim.dyn_size_ext.raw_tensor is None):
                     out[key_] = dim.get_dim_value()
                 elif dim.dyn_size_ext:
                     out[key_] = dim.dyn_size_ext.raw_tensor
+                elif dim.size is not None:
+                    if include_const_sizes:
+                        out[key_] = dim.size
+                else:
+                    raise Exception(f"cannot handle dim: {dim}")
         return out
 
     def assign_from_raw_tensor_dict_(self, raw_tensor_dict: Dict[str, Any]):
         """
         :param raw_tensor_dict: dict of raw tensors, including any sequence lengths / dynamic sizes
         """
         for key, value in self.data.items():
@@ -85,14 +90,17 @@
             for i, dim in enumerate(value.dims):
                 key_ = f"{key}:size{i}"
                 if dim.is_batch_dim() and not dim.dyn_size_ext:
                     dim.dyn_size_ext = Tensor("batch", [], dtype="int32")
                 if dim.dyn_size_ext:
                     assert key_ in raw_tensor_dict
                     dim.dyn_size_ext.raw_tensor = raw_tensor_dict[key_]
+                else:
+                    if key_ in raw_tensor_dict:
+                        assert dim.size == raw_tensor_dict[key_]
 
 
 def _convert_to_tensor(opts: _TensorT, *, name: Optional[str] = None) -> Tensor:
     """
     :param opts:
     """
     if isinstance(opts, Tensor):
```

### Comparing `returnn-1.20230409.21835/returnn/tf/compat.py` & `returnn-1.20230411.4301/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/data_pipeline.py` & `returnn-1.20230411.4301/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/distributed.py` & `returnn-1.20230411.4301/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/engine.py` & `returnn-1.20230411.4301/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/_backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -124,14 +124,42 @@
 
     @staticmethod
     def cast(tensor: Tensor, dtype: str) -> Tensor:
         """cast"""
         return rfl.make_layer({"class": "cast", "from": tensor, "dtype": dtype}, name="cast")
 
     @staticmethod
+    def merge_dims(
+        source: Tensor,
+        *,
+        dims: Sequence[Dim],
+        out_dim: Optional[Dim] = None,
+    ) -> Tuple[Tensor, Dim]:
+        """
+        Merges a list of axes into a single one. (Flatten the dims.)
+        E.g. input is (batch, width, height, dim) and dims=(width,height), then we get (batch, width*height, dim).
+        Or input is (batch, time, height, dim) and axes=(height,dim), then we get (batch, time, height*dim).
+
+        :param nn.Tensor source:
+        :param dims:
+        :param out_dim:
+        :return: tensor, out_dim
+        """
+        if not isinstance(source, Tensor):
+            raise TypeError(f"merge_dims: unexpected type for source {source!r}, need tensor")
+        if out_dim is None:
+            out_dim = dims[0]
+            for d in dims[1:]:
+                out_dim = out_dim * d
+        layer = rfl.make_layer(
+            {"class": "merge_dims", "from": source, "axes": dims, "out_dim": out_dim}, name="merge_dims"
+        )
+        return layer, out_dim
+
+    @staticmethod
     def activation(tensor: Tensor, func: str) -> Tensor:
         """activation"""
         return rfl.make_layer({"class": "activation", "activation": func, "from": tensor}, name=func)
 
     @staticmethod
     def activation_raw(raw_tensor: Layer, func: str) -> Layer:
         """activation"""
@@ -177,15 +205,15 @@
             log_probs = rf.log_softmax(logits, axis=axis)
             return -rf.matmul(targets, log_probs, reduce=axis)
 
     @staticmethod
     def create_parameter_raw(tensor: rf.Parameter) -> Layer:
         """create parameter"""
         return rfl.make_layer(
-            {"class": "variable", "shape": tensor.dims, "dtype": tensor.dtype}, name=tensor.name, existing_tensor=tensor
+            {"class": "variable", "shape": tensor.dims, "dtype": tensor.dtype}, name=tensor.name, out=tensor
         ).raw_tensor
 
     @staticmethod
     def set_parameter_initial_value(param: rf.Parameter[Layer], value: Union[None, Tensor, rf.RawTensorTypes]) -> None:
         """set parameter initial value"""
         if value is None:
             param.raw_tensor.layer_dict.pop("init", None)
@@ -225,26 +253,27 @@
     @staticmethod
     def convert_to_tensor(
         value: Union[Tensor, Layer, RawTensorTypes],
         *,
         dims: Sequence[Dim],
         dtype: str,
         sparse_dim: Optional[Dim] = None,
+        name: Optional[str] = None,
     ) -> Tensor[Layer]:
         """convert to tensor"""
         if isinstance(value, Tensor):
             return value
         kwargs = {}
         if sparse_dim:
             kwargs["sparse_dim"] = sparse_dim
         dim_deps = _dims.get_dim_deps(dims)
         if dim_deps:
             kwargs["shape_deps"] = dim_deps
         return rfl.make_layer(
-            {"class": "constant", "value": value, "shape": dims, "dtype": dtype, **kwargs}, name="constant"
+            {"class": "constant", "value": value, "shape": dims, "dtype": dtype, **kwargs}, name=name or "constant"
         )
 
     @classmethod
     def compare(
         cls,
         a: Union[Tensor, RawTensorTypes],
         kind: str,
@@ -405,14 +434,40 @@
                 "distribution": distribution,
                 "stop_grad": True,
                 **kwargs,
             },
             name="random",
         )
 
+    @staticmethod
+    def masked_select(
+        tensor: Tensor, *, mask: Tensor, dims: Sequence[Dim], out_dim: Optional[Dim] = None
+    ) -> Tuple[Tensor, Dim]:
+        """
+        :param tensor:
+        :param mask:
+        :param dims: the order of the dims defines the format. those dims should be exactly the dims of the mask.
+        :param out_dim:
+        :return: tensor where all dims in mask/dims are removed and replaced by a new dim.
+            the new dim is also returned.
+            if mask==True for all elements, the returned tensor would be simply the flattened input tensor.
+        """
+        assert mask.dtype == "bool"
+        assert set(mask.dims) == set(dims)
+        assert set(mask.dims).issubset(set(tensor.dims))
+        if not out_dim:
+            out_dim = Dim(None, name="mask")
+        return (
+            rfl.make_layer(
+                {"class": "boolean_mask", "from": tensor, "mask": mask, "dims": dims, "out_dim": out_dim},
+                name="boolean_mask",
+            ),
+            out_dim,
+        )
+
 
 def _random_replay_eval(idx, **_kwargs):
     # noinspection PyProtectedMember
     elem = ReturnnLayersBackend._random_journal[idx]
     assert isinstance(elem, dict)
     out = elem["out"]
     assert isinstance(out, Tensor)
```

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/dims.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,14 +63,31 @@
             and all(dep.available_for_inference for dep in deps)
         ):
             _dim_deps.pop(dim)  # go on, replace, use the new list
         else:
             return  # discard new list, keep old
     if _register_dim_via_dyn_layer(dim):
         return
+    if dim.dyn_size_ext and not isinstance(dim.dyn_size_ext.raw_tensor, rfl.Layer):
+        # In the TF net dict backend, the dims dyn_size_ext are usually just templates.
+        # The raw_tensor would not be set.
+        # Once the net dict is created, and then only when the actual TFNetwork is created,
+        # those dim dyn_size_ext.raw_tensor would be set to the TF tensors.
+        # However, we want that the user can directly use the dyn_size_ext in the RF.
+        # In other RF backends (esp eager mode backends), this is usually not a problem.
+        # So we now create a `length` layer getting the tensor from the dim tag,
+        # and then set the dyn_size_ext.raw_tensor to that layer.
+        # Then using dyn_size_ext directly is possible also in the TF net dict backend.
+        assert dim.dyn_size_ext.raw_tensor is None
+        rfl.make_layer(
+            {"class": "length", "from": deps, "axis": dim, "dtype": dim.dyn_size_ext.dtype},
+            name=dim.dyn_size_ext.name,
+            out=dim.dyn_size_ext,
+        )
+        assert isinstance(dim.dyn_size_ext.raw_tensor, rfl.Layer)
     _dim_deps[dim] = deps
 
 
 def _deps_valid_in_cur_name_ctx(deps: List[Tensor]) -> bool:
     cur_root = rfl.Layer.top().root
     for dep in deps:
         assert isinstance(dep, Tensor)
@@ -78,14 +95,18 @@
         if dep.raw_tensor.root != cur_root:
             return False
     return True
 
 
 def _register_dim_via_dyn_layer(dim: Dim) -> bool:
     """
+    Given is any custom length tensor (dyn layer),
+    and we make a dim from that.
+    We do that via the range_from_length layer.
+
     :param dim:
     :return: whether we registered the dim
     """
     if dim.is_static():
         return False
     if dim in _dim_deps:
         return False
```

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/make_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from . import dims as _dims
 
 
 def make_layer(
     layer_dict: rfl.LayerDictRaw,
     *,
     name: Optional[Union[str, rfl.Layer]] = None,
-    existing_tensor: Optional[Tensor] = None,
+    out: Optional[Tensor] = None,
     predefined_out_data: Optional[Tensor] = None,
     name_ctx_ignore_top_stack_frames: int = 0,
 ) -> Tensor[rfl.Layer]:
     """
     Creates the layer. This also registers the layer instance in the top name ctx.
     When no name is given, this assumes that the top name ctx corresponds to this module.
 
@@ -32,15 +32,15 @@
     using that.
     (If this is not the case, please report an issue.)
 
     :param layer_dict: can contain :class:`Tensor` instances
     :param name:
       if str: (suggested) layer name. if given, will create a new :class:`NameCtx`
       if NameCtx, will use this.
-    :param existing_tensor:
+    :param out:
     :param predefined_out_data: normally we can derive the out data automatically.
       If this should be skipped, you can pass this explicitly.
     :param name_ctx_ignore_top_stack_frames: for :func:`Layer.current_ctx`.
       If your calling function creates exactly one single layer, you might want to ignore its stack frame
       and set ignore_top_stack_frames=1 and also set a name for the layer.
       If you are potentially creating multiple layers in your calling function,
       leave the default ignore_top_stack_frames=0.
@@ -59,16 +59,16 @@
     else:
         raise TypeError(f"name must be str or Layer, not {type(name)}; or you should pass a module")
     assert not name_ctx.tensor and not name_ctx.layer_dict  # not yet assigned
     layer_dict = layer_dict.copy()
 
     try:
 
-        if existing_tensor is not None:
-            layer = existing_tensor
+        if out is not None:
+            layer = out
         elif predefined_out_data is not None:
             layer = predefined_out_data.copy_template()
         else:
             layer = _tensor_from_layer_dict(layer_dict, layer=name_ctx)
 
         # Do not assign name_ctx.tensor yet because we potentially could raise exceptions later.
         assert name_ctx.tensor is None
```

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230411.4301/returnn/tf/frontend_low_level/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,27 +359,29 @@
     @staticmethod
     def convert_to_tensor(
         value: Union[_TT, tf.Tensor, RawTensorTypes],
         *,
         dims: Sequence[Dim],
         dtype: str,
         sparse_dim: Optional[Dim] = None,
+        name: Optional[str] = None,
     ) -> _TT:
         """
         :param value:
         :param dims:
         :param dtype:
         :param sparse_dim:
+        :param name:
         :return: tensor
         """
         if isinstance(value, Tensor):
             return value
         value = tf.convert_to_tensor(value, dtype=dtype)
         assert isinstance(value, tf.Tensor)
-        return Tensor("const", raw_tensor=value, dims=dims, dtype=dtype, sparse_dim=sparse_dim)
+        return Tensor(name or "const", raw_tensor=value, dims=dims, dtype=dtype, sparse_dim=sparse_dim)
 
     @staticmethod
     def range_over_dim(dim: Dim) -> _TT:
         """
         :param dim:
         :return: range over dim
         """
```

### Comparing `returnn-1.20230409.21835/returnn/tf/horovod.py` & `returnn-1.20230411.4301/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230411.4301/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/layers/base.py` & `returnn-1.20230411.4301/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/layers/basic.py` & `returnn-1.20230411.4301/returnn/tf/layers/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Many canonical basic layers.
 """
 
 from __future__ import annotations
 
-from typing import Union
+from typing import Optional, Union, Sequence, List
 import typing
 import tensorflow as tf
 import contextlib
 import returnn.tf.compat as tf_compat
 import returnn.tf.util.basic as tf_util
 from returnn.util.basic import unicode, NotSpecified
 from returnn.tf.util.data import Data, SearchBeam, Dim, FeatureDim, SpatialDim
@@ -2667,14 +2667,76 @@
         if isinstance(window_start, LayerBase):
             out.beam = SearchBeam.get_combined_beam(out.beam, window_start.output.beam)
         if isinstance(window_size, LayerBase):
             out.beam = SearchBeam.get_combined_beam(out.beam, window_size.output.beam)
         return out
 
 
+class BooleanMaskLayer(LayerBase):
+    """
+    Wrapper around tf.boolean_mask.
+    """
+
+    layer_class = "boolean_mask"
+
+    def __init__(self, *, mask: LayerBase, dims: Sequence[Dim], out_dim: Optional[Dim] = None, **kwargs):
+        """
+        :param mask:
+        :param dims:
+        :param out_dim:
+        """
+        out_dim  # noqa  # via get_out_data_from_opts
+        super().__init__(**kwargs)
+        assert set(mask.output.dims) == set(dims)
+        self.mask = mask
+        tensor = self.sources[0].output
+        remaining_dims = [d for d in tensor.dims if d not in dims]
+        tensor_templ = tensor.copy_template_new_dim_tags(tuple(dims) + tuple(remaining_dims))
+        tensor = tensor.copy_compatible_to(tensor_templ, add_dims=False)
+        mask_templ = mask.output.copy_template_new_dim_tags(new_dim_tags=tuple(dims))
+        mask_ = mask.output.copy_compatible_to(mask_templ, add_dims=False)
+        self.output.raw_tensor = tf.boolean_mask(tensor.raw_tensor, mask=mask_.raw_tensor)
+        if self.output.dims[0].dyn_size_ext.raw_tensor is None:
+            self.output.dims[0].dyn_size_ext.raw_tensor = tf.shape(self.output.raw_tensor)[0]
+
+    def get_dep_layers(self) -> List[LayerBase]:
+        """dep layers"""
+        return super().get_dep_layers() + [self.mask]
+
+    @classmethod
+    def transform_config_dict(cls, d, network, get_layer):
+        """
+        :param dict[str] d:
+        :param returnn.tf.network.TFNetwork network:
+        :param get_layer:
+        """
+        super().transform_config_dict(d, network=network, get_layer=get_layer)
+        d["mask"] = get_layer(d["mask"])
+
+    @classmethod
+    def get_out_data_from_opts(
+        cls, *, name: str, sources: Sequence[LayerBase], mask: LayerBase, out_dim: Optional[Dim] = None, **kwargs
+    ) -> Data:
+        """
+        :param name:
+        :param sources:
+        :param mask:
+        :param out_dim:
+        """
+        assert len(sources) == 1
+        assert mask.output.dims
+        _out_dim = Dim(Data(name=f"{name}:mask", dims=(), dtype=Data.size_dtype))
+        if out_dim:
+            _out_dim.declare_same_as(out_dim)
+        else:
+            out_dim = _out_dim
+        dims = [out_dim] + [d for d in sources[0].output.dims if d not in mask.output.dims]
+        return sources[0].output.copy_template_new_dim_tags(name=f"{name}_output", new_dim_tags=dims)
+
+
 class RandomStateInitLayer(LayerBase):
     """
     This calculates the initial state value for the state var
     of :class:`RandomLayer`.
     This depends on the algorithm and seed.
     """
```

### Comparing `returnn-1.20230409.21835/returnn/tf/layers/rec.py` & `returnn-1.20230411.4301/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/layers/segmental_model.py` & `returnn-1.20230411.4301/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/layers/signal_processing.py` & `returnn-1.20230411.4301/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/native_op.py` & `returnn-1.20230411.4301/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/network.py` & `returnn-1.20230411.4301/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/sprint.py` & `returnn-1.20230411.4301/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/updater.py` & `returnn-1.20230411.4301/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/util/basic.py` & `returnn-1.20230411.4301/returnn/tf/util/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import threading
 import numpy
 import tensorflow as tf
 from tensorflow.python.client import device_lib
 from tensorflow.python.ops import init_ops
 from returnn.util import basic as util
 from returnn.util.basic import NotSpecified, NativeCodeCompiler
+from returnn.tensor import Tensor
 import returnn.tf.compat as tf_compat
 
 # noinspection PyUnresolvedReferences
 from .data import Data, SearchBeam, Dim, DimensionTag
 
 try:
     from tensorflow.python.ops.control_flow_v2_func_graphs import ControlFlowFuncGraph
@@ -256,20 +257,23 @@
         if v != pad_value:
             del d[k]
     d[dim] = pad_value
 
 
 def mask_dyn_seq_len_nd(x, pad_value, axes):
     """
-    :param Data x:
-    :param float|int|tf.Tensor pad_value:
+    :param Tensor x:
+    :param float|int|tf.Tensor|Tensor pad_value:
     :param list[int]|tuple[int] axes:
     :return: masked x
     :rtype: tf.Tensor
     """
+    if isinstance(pad_value, Tensor):
+        assert pad_value.dims == ()
+        pad_value = pad_value.placeholder
     # Filter out some axes which should not be used for masking.
     axes_ = []
     for axis in axes:
         tag = x.dim_tags[axis]
         assert tag.dyn_size_ext
         # It only makes sense to apply for this axis if the dyn size dims are all existing in x itself.
         # E.g. if the dyn_size_ext shape is [B] but the shape of x is just [T] (without B),
```

### Comparing `returnn-1.20230409.21835/returnn/tf/util/data.py` & `returnn-1.20230411.4301/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/util/ken_lm.py` & `returnn-1.20230411.4301/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/tf/util/open_fst.py` & `returnn-1.20230411.4301/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/torch/data/pipeline.py` & `returnn-1.20230411.4301/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230411.4301/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/torch/data/tensor_utils.py` & `returnn-1.20230411.4301/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/torch/engine.py` & `returnn-1.20230411.4301/returnn/torch/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,15 @@
         if isinstance(model, rf.Module):
             self._pt_model = rf_module_to_pt_module(model)
         elif isinstance(model, torch.nn.Module):
             self._pt_model = model
         else:
             raise TypeError(f"get_model returned {model} of type {type(model)}, expected rf.Module or torch.nn.Module")
         assert isinstance(self._pt_model, torch.nn.Module)
+        print("Model:", self._pt_model, file=log.v4)
 
         if checkpoint_state is not None:
             self._pt_model.load_state_dict(checkpoint_state["model"])
         preload_from_files = self.config.typed_value("preload_from_files", {})
         if preload_from_files:
             # see `preload_from_files` in tf engine and `returnn.tf.network.CustomCheckpointLoader`
             is_training = self.config.value("task", "train") == "train"
```

### Comparing `returnn-1.20230409.21835/returnn/torch/frontend/_backend.py` & `returnn-1.20230411.4301/returnn/torch/frontend/_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,28 +104,76 @@
     def get_known_shape_raw(raw_tensor: torch.Tensor) -> Tuple[Optional[int]]:
         """
         :return: shape of raw tensor; here for PyTorch the full shape is always known
         """
         return tuple(raw_tensor.size())
 
     @staticmethod
+    def get_new_dim_raw(raw_tensor: torch.Tensor, axis: int, *, name: str) -> Dim:
+        """
+        :param raw_tensor:
+        :param axis:
+        :param name:
+        :return: new Dim object
+        """
+        return Dim(raw_tensor.size(axis), name=name)
+
+    @staticmethod
     def expand_dims_raw(raw_tensor: torch.Tensor, axis: int) -> torch.Tensor:
         """
         :param raw_tensor:
         :param axis: e.g. 1
         :return: raw tensor with new axis
         """
         return raw_tensor.unsqueeze(axis)
 
     @staticmethod
     def cast_raw(raw_tensor: torch.Tensor, dtype: str) -> torch.Tensor:
         """cast"""
         return raw_tensor.to(dtype=TorchBackend.as_dtype_raw(dtype))
 
     @staticmethod
+    def merge_dims(
+        source: Tensor,
+        *,
+        dims: Sequence[Dim],
+        out_dim: Optional[Dim] = None,
+    ) -> Tuple[Tensor, Dim]:
+        """
+        Merges a list of axes into a single one. (Flatten the dims.)
+        E.g. input is (batch, width, height, dim) and dims=(width,height), then we get (batch, width*height, dim).
+        Or input is (batch, time, height, dim) and axes=(height,dim), then we get (batch, time, height*dim).
+
+        :param nn.Tensor source:
+        :param dims:
+        :param out_dim:
+        :return: tensor, out_dim
+        """
+        assert dims
+        if len(dims) == 1:
+            return source, dims[0]
+        first_axis = min(source.dims.index(d) for d in dims)
+        pre_dims = source.dims[:first_axis]
+        post_dims = [d for d in source.dims if d not in dims]
+        if out_dim is None:
+            out_dim = dims[0]
+            for d in dims[1:]:
+                out_dim = out_dim * d
+        source = source.copy_transpose(tuple(pre_dims) + tuple(dims) + tuple(post_dims), allow_int=False)
+        out = Tensor(
+            "merge_dims",
+            dims=pre_dims + (out_dim,) + tuple(post_dims),
+            dtype=source.dtype,
+            sparse_dim=source.sparse_dim,
+        )
+        out_shape = [d.get_dim_value() for d in out.dims]
+        out.raw_tensor = torch.reshape(source.raw_tensor, out_shape)
+        return out, out_dim
+
+    @staticmethod
     def activation_raw(raw_tensor: torch.Tensor, func: str) -> torch.Tensor:
         """
         :param raw_tensor:
         :param func: e.g. "tanh"
         :return: raw tensor after activation
         """
         assert func in Backend._AllowedActivationFuncs
@@ -287,28 +335,30 @@
     @staticmethod
     def convert_to_tensor(
         value: Union[Tensor, torch.Tensor, RawTensorTypes],
         *,
         dims: Sequence[Dim],
         dtype: str,
         sparse_dim: Optional[Dim] = None,
+        name: Optional[str] = None,
     ) -> Tensor[torch.Tensor]:
         """
         :param value:
         :param dims:
         :param dtype:
         :param sparse_dim:
+        :param name:
         :return: tensor
         """
         if isinstance(value, Tensor):
             return value
         if isinstance(value, torch.Tensor):
-            name = "raw_tensor"
+            name = name or "raw_tensor"
         else:
-            name = "const"
+            name = name or "const"
             value = torch.tensor(value, dtype=TorchBackend.as_dtype_raw(dtype))
         assert isinstance(value, torch.Tensor)
         return Tensor(name, dims=dims, dtype=dtype, sparse_dim=sparse_dim, raw_tensor=value)
 
     @staticmethod
     def full(
         dims: Sequence[Dim], fill_value: RawTensorTypes, *, dtype: str, sparse_dim: Optional[Dim] = None
@@ -424,15 +474,15 @@
         """
         out = Tensor(
             "range",
             dims=[dim],
             sparse_dim=dim,
             dtype=dim.dyn_size_ext.dtype if dim.dyn_size_ext else rf.get_default_array_index_dtype(),
         )
-        out.raw_tensor = torch.arange(dim.get_dim_value())
+        out.raw_tensor = torch.arange(dim.get_dim_value(), dtype=TorchBackend.as_dtype_raw(out.dtype))
         return out
 
     @staticmethod
     def reduce(
         source: Tensor[torch.Tensor],
         *,
         mode: str,
@@ -607,7 +657,44 @@
                     "maxval": maxval,
                     "seed": seed,
                     "static": static,
                     "out": out_,
                 }
             )
         return out
+
+    @staticmethod
+    def masked_select(
+        tensor: Tensor, *, mask: Tensor, dims: Sequence[Dim], out_dim: Optional[Dim] = None
+    ) -> Tuple[Tensor, Dim]:
+        """
+        :param tensor:
+        :param mask:
+        :param dims: the order of the dims defines the format. those dims should be exactly the dims of the mask.
+        :param out_dim:
+        :return: tensor where all dims in mask/dims are removed and replaced by a new dim.
+            the new dim is also returned.
+            if mask==True for all elements, the returned tensor would be simply the flattened input tensor.
+        """
+        assert mask.dtype == "bool"
+        assert set(mask.dims) == set(dims)
+        assert set(mask.dims).issubset(set(tensor.dims))
+        remaining_dims = [d for d in tensor.dims if d not in mask.dims]
+        tensor_templ = tensor.copy_template_new_dim_tags(tuple(dims) + tuple(remaining_dims))
+        tensor = tensor.copy_compatible_to(tensor_templ, add_dims=False)
+        mask = mask.copy_compatible_to(tensor_templ, check_dtype=False, check_sparse=False)
+        out_raw = torch.masked_select(tensor.raw_tensor, mask.raw_tensor)
+        remaining_shape = [d.get_dim_value() for d in remaining_dims]
+        remaining_num_elements = numpy.prod(remaining_shape) if remaining_shape else 1
+        assert out_raw.numel() % remaining_num_elements == 0
+        flattened_num_elements = out_raw.numel() // remaining_num_elements
+        out_raw = out_raw.resize(flattened_num_elements, *remaining_shape)
+        if not out_dim:
+            out_dim = TorchBackend.get_new_dim_raw(out_raw, 0, name="masked_select")
+        out = Tensor(
+            "masked_select",
+            dims=(out_dim,) + tuple(remaining_dims),
+            dtype=tensor.dtype,
+            sparse_dim=tensor.sparse_dim,
+            raw_tensor=out_raw,
+        )
+        return out, out_dim
```

### Comparing `returnn-1.20230409.21835/returnn/torch/frontend/_rand.py` & `returnn-1.20230411.4301/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/torch/frontend/bridge.py` & `returnn-1.20230411.4301/returnn/torch/frontend/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
             assert isinstance(pt_param, torch.nn.Parameter)
             self.register_parameter(name, pt_param)
 
         for name, rf_mod in rf_module.named_children():
             pt_mod = rf_module_to_pt_module(rf_mod)
             self.add_module(name, pt_mod)
 
+    def _get_name(self):
+        return self._rf_module.__class__.__name__ + "[RF→PT]"
+
     @property
     def rf_module(self) -> rf.Module:
         """RF module"""
         return self._rf_module
 
     def forward(self, *args, **kwargs):
         """forward"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `returnn-1.20230409.21835/returnn/torch/updater.py` & `returnn-1.20230411.4301/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/basic.py` & `returnn-1.20230411.4301/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/better_exchook.py` & `returnn-1.20230411.4301/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/bpe.py` & `returnn-1.20230411.4301/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/debug.py` & `returnn-1.20230411.4301/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/debug_helpers.py` & `returnn-1.20230411.4301/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/fsa.py` & `returnn-1.20230411.4301/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230411.4301/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/pprint.py` & `returnn-1.20230411.4301/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/py-to-pickle.cpp` & `returnn-1.20230411.4301/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/sig_proc.py` & `returnn-1.20230411.4301/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn/util/task_system.py` & `returnn-1.20230411.4301/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/returnn.egg-info/PKG-INFO` & `returnn-1.20230411.4301/returnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230409.21835
+Version: 1.20230411.4301
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230409.21835/returnn.egg-info/SOURCES.txt` & `returnn-1.20230411.4301/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/setup.py` & `returnn-1.20230411.4301/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/DummySprintExec.py` & `returnn-1.20230411.4301/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230411.4301/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230411.4301/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230411.4301/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/_set_num_threads1.py` & `returnn-1.20230411.4301/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/_setup_test_env.py` & `returnn-1.20230411.4301/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/bpe-unicode-demo.codes` & `returnn-1.20230411.4301/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/bpe-unicode-demo.vocab` & `returnn-1.20230411.4301/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/lexicon_opt.isyms` & `returnn-1.20230411.4301/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/lexicon_opt.jpg` & `returnn-1.20230411.4301/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/lint_common.py` & `returnn-1.20230411.4301/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/pycharm-inspect.py` & `returnn-1.20230411.4301/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/pylint.py` & `returnn-1.20230411.4301/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/returnn-as-framework.py` & `returnn-1.20230411.4301/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/rf_utils.py` & `returnn-1.20230411.4301/tests/rf_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 RETURNN frontend (returnn.frontend) utils
 """
 
 from __future__ import annotations
 import contextlib
 import numpy
+from tensorflow.python.util import nest
 
 from returnn.config import Config, global_config_ctx
 from returnn.util.pprint import pprint
 import returnn.frontend as rf
-from returnn.tensor import Tensor, TensorDict
+from returnn.tensor import Tensor, Dim, TensorDict
 import returnn.tf.compat as tf_compat
 import returnn.torch.frontend as rft
 import returnn.tf.frontend_layers as rfl
 from returnn.tf.network import TFNetwork
 from returnn.torch.data.tensor_utils import tensor_numpy_to_torch_, tensor_torch_to_numpy_
 
 
@@ -30,25 +31,43 @@
         _reset_tensor(v)
     rnd = numpy.random.RandomState(42)
     for v in extern_data.data.values():
         _fill_random(v, rnd=rnd)
 
     with rft.TorchBackend.random_journal_record() as random_journal:
         out_pt = run_model_torch(extern_data, get_model, forward_step)
-        out_pt_raw = out_pt.as_raw_tensor_dict()  # get them now because dims might get overwritten
+        # get the values now because dims might get overwritten
+        out_pt_raw = out_pt.as_raw_tensor_dict(include_const_sizes=True)
 
     with rfl.ReturnnLayersBackend.random_journal_replay(random_journal):
         out_tf = run_model_net_dict_tf(extern_data, get_model, forward_step)
-        out_tf_raw = out_tf.as_raw_tensor_dict()
+        out_tf_raw = out_tf.as_raw_tensor_dict(include_const_sizes=True)
 
     print(out_pt, out_tf)
     assert set(out_pt.data.keys()) == set(out_tf.data.keys())
     for k, v_pt in out_pt.data.items():
         v_tf = out_tf[k]
-        assert v_pt.dims == v_tf.dims
+        # We cannot really check the dims directly for equality,
+        # because the model code often creates new dims, which are different in each call.
+        # However, via mark_as_output, the order of dims is well-defined.
+        # So we can check the values.
+        assert len(v_pt.dims) == len(v_tf.dims)
+        for d_pt, d_tf in zip(v_pt.dims, v_tf.dims):
+            assert isinstance(d_pt, Dim) and isinstance(d_tf, Dim)
+            assert _dim_is_scalar_size(d_pt) == _dim_is_scalar_size(d_tf)
+            if _dim_is_scalar_size(d_pt):
+                assert _dim_scalar_size(d_pt) == _dim_scalar_size(d_tf)
+            else:
+                assert d_pt.dyn_size_ext and d_tf.dyn_size_ext
+                # There might be cases where the dims are maybe not equal
+                # (same reasoning as above, or also different order),
+                # although this would be quite exotic.
+                # Let's just assume for now that this does not happen.
+                assert d_pt.dyn_size_ext.dims == d_tf.dyn_size_ext.dims
+                assert (d_pt.dyn_size_ext.raw_tensor == d_tf.dyn_size_ext.raw_tensor).all()
     assert set(out_pt_raw.keys()) == set(out_tf_raw.keys())
     for k, v_pt in out_pt_raw.items():
         v_tf = out_tf_raw[k]
         assert numpy.allclose(v_pt, v_tf, atol=1e-5, rtol=1e-5)
     return out_pt
 
 
@@ -118,14 +137,24 @@
         fetches = outputs_tf.as_raw_tensor_dict()
         assert set(extern_data.data.keys()) == set(net.extern_data.data.keys())
         extern_data_tf_placeholders = net.extern_data.as_raw_tensor_dict()
         assert set(extern_data_tf_placeholders.keys()) == set(extern_data_raw.keys())
         feed_dict = {extern_data_tf_placeholders[k]: v for k, v in extern_data_raw.items()}
 
         outputs_numpy_raw = session.run(fetches, feed_dict=feed_dict)
+
+        # Scalars are not Numpy arrays, but our code below assumes that we only have Numpy arrays.
+        # So we convert them here.
+        def _make_numpy_array(x):
+            if isinstance(x, numpy.ndarray):
+                return x
+            return numpy.array(x)
+
+        outputs_numpy_raw = nest.map_structure(_make_numpy_array, outputs_numpy_raw)
+
         outputs_numpy = outputs_tf.copy_template()
         for v in outputs_numpy.data.values():
             _reset_tensor(v)
         outputs_numpy.assign_from_raw_tensor_dict_(outputs_numpy_raw)
 
     extern_data.assign_from_raw_tensor_dict_(extern_data_raw)
     return outputs_numpy
@@ -181,7 +210,26 @@
         else:
             raise NotImplementedError(f"not implemented for {x} dtype {x.dtype}")
         filled = True
 
     assert isinstance(x.raw_tensor, numpy.ndarray)
 
     return filled
+
+
+def _dim_is_scalar_size(dim: Dim) -> bool:
+    """dim is scalar size"""
+    if dim.size is not None:
+        return True
+    if dim.dyn_size_ext:
+        return dim.dyn_size_ext.dims == ()
+    return False
+
+
+def _dim_scalar_size(dim: Dim) -> int:
+    """dim scalar size"""
+    if dim.size is not None:
+        return dim.size
+    if dim.dyn_size_ext:
+        assert dim.dyn_size_ext.dims == ()
+        return dim.dyn_size_ext.raw_tensor
+    raise Exception(f"dim {dim} has no known size")
```

### Comparing `returnn-1.20230409.21835/tests/spelling.dic` & `returnn-1.20230411.4301/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_Config.py` & `returnn-1.20230411.4301/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_Dataset.py` & `returnn-1.20230411.4301/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_Fsa.py` & `returnn-1.20230411.4301/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_GeneratingDataset.py` & `returnn-1.20230411.4301/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_HDFDataset.py` & `returnn-1.20230411.4301/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_LearningRateControl.py` & `returnn-1.20230411.4301/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_Log.py` & `returnn-1.20230411.4301/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_MultiProcDataset.py` & `returnn-1.20230411.4301/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_PTDataset.py` & `returnn-1.20230411.4301/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_Pretrain.py` & `returnn-1.20230411.4301/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_ResNet.py` & `returnn-1.20230411.4301/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_SprintDataset.py` & `returnn-1.20230411.4301/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_SprintInterface.py` & `returnn-1.20230411.4301/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TFEngine.py` & `returnn-1.20230411.4301/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TFNativeOp.py` & `returnn-1.20230411.4301/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TFNetworkLayer.py` & `returnn-1.20230411.4301/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230411.4301/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230411.4301/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TFUpdater.py` & `returnn-1.20230411.4301/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TFUtil.py` & `returnn-1.20230411.4301/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TF_determinism.py` & `returnn-1.20230411.4301/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TaskSystem.py` & `returnn-1.20230411.4301/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230411.4301/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_TranslationDataset.py` & `returnn-1.20230411.4301/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_Util.py` & `returnn-1.20230411.4301/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_demos.py` & `returnn-1.20230411.4301/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_fork_exec.py` & `returnn-1.20230411.4301/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_hdf_dump.py` & `returnn-1.20230411.4301/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_rf_base.py` & `returnn-1.20230411.4301/tests/test_rf_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 RETURNN frontend (returnn.frontend) tests
 """
 
 from __future__ import annotations
+from typing import Tuple
 import _setup_test_env  # noqa
 import returnn.frontend as rf
 from returnn.tensor import Tensor, Dim, TensorDict, batch_dim
 from rf_utils import run_model
 
 
 def test_linear_direct():
@@ -136,7 +137,29 @@
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         logits = model(extern_data["data"])
         targets = extern_data["classes"]
         loss = rf.cross_entropy(estimated=logits, estimated_type="logits", target=targets, axis=out_dim)
         loss.mark_as_default_output()
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
+
+
+def test_pack():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __call__(self, x: Tensor) -> Tuple[Tensor, Dim]:
+            pack, pack_dim = rf.pack(x, dims=[batch_dim, time_dim], enforce_sorted=False)
+            return pack, pack_dim
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out, pack_dim = model(extern_data["data"])
+        out.mark_as_default_output(shape=(pack_dim, in_dim))
+
+    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
```

### Comparing `returnn-1.20230409.21835/tests/test_tensor.py` & `returnn-1.20230411.4301/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_tools.py` & `returnn-1.20230411.4301/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_torch_frontend.py` & `returnn-1.20230411.4301/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tests/test_torch_internal_frontend.py` & `returnn-1.20230411.4301/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/analyze-dataset-batches.py` & `returnn-1.20230411.4301/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/bliss-collect-seq-lens.py` & `returnn-1.20230411.4301/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/bliss-dump-text.py` & `returnn-1.20230411.4301/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/bliss-get-segment-names.py` & `returnn-1.20230411.4301/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/bliss-to-ogg-zip.py` & `returnn-1.20230411.4301/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/bpe-create-lexicon.py` & `returnn-1.20230411.4301/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/calculate-word-error-rate.py` & `returnn-1.20230411.4301/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/cleanup-old-models.py` & `returnn-1.20230411.4301/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/collect-orth-symbols.py` & `returnn-1.20230411.4301/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/collect-words.py` & `returnn-1.20230411.4301/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/compile_native_op.py` & `returnn-1.20230411.4301/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/compile_tf_graph.py` & `returnn-1.20230411.4301/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/debug-dump-search-scores.py` & `returnn-1.20230411.4301/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/debug-plot-search-scores.py` & `returnn-1.20230411.4301/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/dump-dataset-raw-strings.py` & `returnn-1.20230411.4301/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/dump-dataset.py` & `returnn-1.20230411.4301/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/dump-forward-stats.py` & `returnn-1.20230411.4301/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/dump-forward.py` & `returnn-1.20230411.4301/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/dump-network-json.py` & `returnn-1.20230411.4301/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/dump-pickle.py` & `returnn-1.20230411.4301/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230411.4301/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/get-attention-weights.py` & `returnn-1.20230411.4301/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/get-best-model-epoch.py` & `returnn-1.20230411.4301/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/hdf_dump.py` & `returnn-1.20230411.4301/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230411.4301/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/import-blocks-mt-model.py` & `returnn-1.20230411.4301/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/import-t2t-mt-model.py` & `returnn-1.20230411.4301/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/Makefile` & `returnn-1.20230411.4301/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/README.md` & `returnn-1.20230411.4301/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/example/README.md` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/file.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230411.4301/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/main.cc` & `returnn-1.20230411.4301/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230411.4301/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/tf_avg_checkpoints.py` & `returnn-1.20230411.4301/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/tf_inspect_checkpoint.py` & `returnn-1.20230411.4301/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230409.21835/tools/tf_inspect_summary_log.py` & `returnn-1.20230411.4301/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

