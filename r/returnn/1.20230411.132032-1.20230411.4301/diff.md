# Comparing `tmp/returnn-1.20230411.132032.tar.gz` & `tmp/returnn-1.20230411.4301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230411.132032.tar", last modified: Tue Apr 11 11:35:04 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230411.4301.tar", last modified: Mon Apr 10 23:03:27 2023, max compression
```

## Comparing `returnn-1.20230411.132032.tar` & `returnn-1.20230411.4301.tar`

### file list

```diff
@@ -1,410 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 11:35:03.000000 returnn-1.20230411.132032/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63018 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 11:34:33.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-11 11:34:36.000000 returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25787 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36530 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94908 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   155800 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   150268 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   148678 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   584733 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18948 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144495 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/py-to-pickle.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:35:04.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-11 11:34:30.000000 returnn-1.20230411.132032/tools/tf_inspect_summary_log.py
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

### Comparing `returnn-1.20230411.132032/.gitignore` & `returnn-1.20230411.4301/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/.gitmodules` & `returnn-1.20230411.4301/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/CHANGELOG.md` & `returnn-1.20230411.4301/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/CODEOWNERS` & `returnn-1.20230411.4301/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/CONTRIBUTING.md` & `returnn-1.20230411.4301/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/LICENSE` & `returnn-1.20230411.4301/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/MANIFEST.in` & `returnn-1.20230411.4301/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/PKG-INFO` & `returnn-1.20230411.4301/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230411.132032
+Version: 1.20230411.4301
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230411.132032/README.rst` & `returnn-1.20230411.4301/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/__init__.py` & `returnn-1.20230411.4301/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/12AX.cluster_map` & `returnn-1.20230411.4301/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-fwd.config` & `returnn-1.20230411.4301/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-horovod-mpi.py` & `returnn-1.20230411.4301/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230411.4301/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-hyper-param-tuning.config` & `returnn-1.20230411.4301/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-iter-dataset.py` & `returnn-1.20230411.4301/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-list-devices.py` & `returnn-1.20230411.4301/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-lua-torch-layer.config` & `returnn-1.20230411.4301/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230411.4301/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-returnn-as-framework.py` & `returnn-1.20230411.4301/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-rf.config` & `returnn-1.20230411.4301/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-rhn-enwik8.config` & `returnn-1.20230411.4301/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-sprint-interface.py` & `returnn-1.20230411.4301/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-att-copy.config` & `returnn-1.20230411.4301/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-attention.config` & `returnn-1.20230411.4301/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-enc-dec.config` & `returnn-1.20230411.4301/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230411.4301/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230411.4301/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230411.4301/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230411.4301/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230411.4301/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-rec-self-att.config` & `returnn-1.20230411.4301/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230411.4301/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230411.4301/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-torch.config` & `returnn-1.20230411.4301/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230411.4301/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/demo.sh` & `returnn-1.20230411.4301/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230411.4301/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/README.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/config_demo` & `returnn-1.20230411.4301/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230411.4301/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/config_real` & `returnn-1.20230411.4301/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230411.4301/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/decode.py` & `returnn-1.20230411.4301/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230411.4301/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230411.4301/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230411.4301/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230411.4301/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/__init__.py` & `returnn-1.20230411.4301/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/__main__.py` & `returnn-1.20230411.4301/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/__old_mod_loader__.py` & `returnn-1.20230411.4301/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/__setup__.py` & `returnn-1.20230411.4301/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/config.py` & `returnn-1.20230411.4301/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/audio.py` & `returnn-1.20230411.4301/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/basic.py` & `returnn-1.20230411.4301/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/bundle_file.py` & `returnn-1.20230411.4301/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/cached.py` & `returnn-1.20230411.4301/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/cached2.py` & `returnn-1.20230411.4301/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/generating.py` & `returnn-1.20230411.4301/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/hdf.py` & `returnn-1.20230411.4301/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/lm.py` & `returnn-1.20230411.4301/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/map.py` & `returnn-1.20230411.4301/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/meta.py` & `returnn-1.20230411.4301/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/multi_proc.py` & `returnn-1.20230411.4301/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/normalization_data.py` & `returnn-1.20230411.4301/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/numpy_dump.py` & `returnn-1.20230411.4301/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/raw_wav.py` & `returnn-1.20230411.4301/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/sprint.py` & `returnn-1.20230411.4301/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/stereo.py` & `returnn-1.20230411.4301/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230411.4301/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/datasets/util/vocabulary.py` & `returnn-1.20230411.4301/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/engine/base.py` & `returnn-1.20230411.4301/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/engine/batch.py` & `returnn-1.20230411.4301/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230411.4301/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/graph_editor/edit.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/graph_editor/select.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/graph_editor/transform.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/extern/graph_editor/util.py` & `returnn-1.20230411.4301/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/__init__.py` & `returnn-1.20230411.4301/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/_backend.py` & `returnn-1.20230411.4301/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/_numpy_backend.py` & `returnn-1.20230411.4301/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/_utils.py` & `returnn-1.20230411.4301/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/array_.py` & `returnn-1.20230411.4301/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/const.py` & `returnn-1.20230411.4301/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/dims.py` & `returnn-1.20230411.4301/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/dtype.py` & `returnn-1.20230411.4301/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/init.py` & `returnn-1.20230411.4301/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/linear.py` & `returnn-1.20230411.4301/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/loss.py` & `returnn-1.20230411.4301/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/math_.py` & `returnn-1.20230411.4301/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/matmul.py` & `returnn-1.20230411.4301/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/module.py` & `returnn-1.20230411.4301/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/parameter.py` & `returnn-1.20230411.4301/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/rand.py` & `returnn-1.20230411.4301/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/reduce.py` & `returnn-1.20230411.4301/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/run_ctx.py` & `returnn-1.20230411.4301/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/state.py` & `returnn-1.20230411.4301/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/frontend/types.py` & `returnn-1.20230411.4301/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/import_/common.py` & `returnn-1.20230411.4301/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/import_/git.py` & `returnn-1.20230411.4301/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/import_/import_.py` & `returnn-1.20230411.4301/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/learning_rate_control.py` & `returnn-1.20230411.4301/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/log.py` & `returnn-1.20230411.4301/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/native_op.cpp` & `returnn-1.20230411.4301/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/native_op.py` & `returnn-1.20230411.4301/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/pretrain.py` & `returnn-1.20230411.4301/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/sprint/cache.py` & `returnn-1.20230411.4301/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/sprint/control.py` & `returnn-1.20230411.4301/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/sprint/error_signals.py` & `returnn-1.20230411.4301/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/sprint/extern_interface.py` & `returnn-1.20230411.4301/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/sprint/interface.py` & `returnn-1.20230411.4301/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/_dim_extra.py` & `returnn-1.20230411.4301/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/_tensor_extra.py` & `returnn-1.20230411.4301/returnn/tensor/_tensor_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,59 +783,48 @@
         :return: copy of self with feature_dim_axis being the very last axis
         """
         assert self.feature_dim_axis is not None
         return self.copy_with_feature_dim_axis(-1)
 
     def copy_add_batch_dim(self, batch_dim_axis, batch=None, dim_tag=None) -> _t.Tensor:
         """
+        Warning: Assumes TensorFlow.
+
         :param int batch_dim_axis:
         :param BatchInfo|None batch:
         :param Dim|None dim_tag:
         :return: copy of myself with added batch-dim
         """
         assert self.batch_dim_axis is None
+        if not batch:
+            from returnn.tf.layers.base import LayerBase
+
+            batch = LayerBase.get_recent_layer().get_batch_info()
         if batch_dim_axis < 0:
             assert batch_dim_axis + self.batch_ndim + 1 >= 0
             batch_dim_axis += self.batch_ndim + 1
         assert 0 <= batch_dim_axis <= self.batch_ndim
         data_opts = self.get_kwargs(include_special_axes=False)
         placeholder = self.placeholder
         if placeholder is not None:
             backend = self._raw_backend
             placeholder = backend.expand_dims_raw(placeholder, batch_dim_axis)
-            if batch:
-                batch_dim_ = batch.dim
-            elif dim_tag:
-                if dim_tag.dyn_size_ext:
-                    assert dim_tag.dyn_size_ext.dims == ()
-                    assert dim_tag.dyn_size_ext.raw_tensor is not None
-                    batch_dim_ = dim_tag.dyn_size_ext.raw_tensor
-                elif dim_tag.dimension:
-                    batch_dim_ = dim_tag.dimension
-                else:
-                    raise Exception(f"{self} copy_add_batch_dim: unknown batch dim for {dim_tag!r}")
-            else:
-                raise Exception(f"{self} copy_add_batch_dim: unknown batch dim ")
-            if not isinstance(batch_dim_, int) or batch_dim_ != 1:
-                placeholder = backend.expand_raw(placeholder, batch_dim_axis, batch_dim_)
+            if not isinstance(batch.dim, int) or batch.dim != 1:
+                placeholder = backend.expand_raw(placeholder, batch_dim_axis, batch.dim)
         dim_tags = list(self.dim_tags)
         if dim_tag:
             assert dim_tag.is_batch_dim()
+            assert dim_tag.dimension == batch.static_dim or dim_tag.dimension is None
             assert dim_tag.batch == batch
-            if batch:
-                assert dim_tag.dimension == batch.static_dim or dim_tag.dimension is None
         else:
-            dim_tag = Dim(
-                kind=Dim.Types.Batch, description="batch", dimension=batch.static_dim if batch else None, batch=batch
-            )
+            dim_tag = Dim(kind=Dim.Types.Batch, description="batch", dimension=batch.static_dim, batch=batch)
         dim_tags.insert(batch_dim_axis, dim_tag)
         data_opts["dims"] = dim_tags
-        if batch:
-            data_opts["batch"] = batch
-            data_opts["beam"] = batch.beam
+        data_opts["batch"] = batch
+        data_opts["beam"] = batch.beam
         other_special_axes = self.get_special_axes_dict(counted_with_batch_dim=True, only_available=True)
         for k, a in other_special_axes.items():
             data_opts[k] = a if (a < batch_dim_axis) else (a + 1)
         return _t.Tensor(placeholder=placeholder, **data_opts)
 
     def copy_add_spatial_dim(self, spatial_dim_axis=None, dim=1, auto_time_dim_axis=True) -> _t.Tensor:
         """
@@ -916,25 +905,22 @@
             axis += self.batch_ndim + 1
         assert 0 <= axis <= self.batch_ndim
 
         if dim_tag.is_batch_dim():
             if unbroadcast:
                 return self.copy_add_batch_dim(batch_dim_axis=axis, batch=dim_tag.batch, dim_tag=dim_tag)
             else:
-                if dim_tag.batch or self.batch:
-                    from returnn.tf.util.data import BatchInfo
+                from returnn.tf.util.data import BatchInfo
 
-                    batch_info = BatchInfo.make_global_broadcast_batch_info()
-                else:
-                    batch_info = None
-                if dim_tag and dim_tag.dimension == 1 and dim_tag.batch == batch_info:
-                    pass  # keep it
-                else:
-                    dim_tag = Dim(kind=Dim.Types.Batch, description="batch-broadcast", dimension=1, batch=batch_info)
-                return self.copy_add_batch_dim(batch_dim_axis=axis, batch=batch_info, dim_tag=dim_tag)
+                batch_info = BatchInfo.make_global_broadcast_batch_info()
+                return self.copy_add_batch_dim(
+                    batch_dim_axis=axis,
+                    batch=batch_info,
+                    dim_tag=dim_tag if (dim_tag.dimension == 1 and dim_tag.batch == batch_info) else None,
+                )
 
         data_opts = self.get_kwargs()
         # Note: if dim_tag is feature, but we are sparse, we just make it spatial
         if self.sparse and dim_tag.is_feature_dim():
             dim_tag = dim_tag.copy(same_as_self=True, kind=Dim.Types.Spatial)
         if not unbroadcast and dim_tag.dimension != 1:
             dim_tag = Dim(
@@ -2822,19 +2808,17 @@
         return self.dim_tags[self.batch_dim_axis]
 
     def get_static_batch_dim(self):
         """
         :rtype: int|None
         """
         # Do not fallback to get_batch_dim or get_recent_layer or so. This should be safe.
-        if self.batch:
-            return self.batch.static_dim
-        if self.have_batch_axis():
-            return self.get_batch_dim_tag().dimension
-        return None
+        if not self.batch:
+            return None
+        return self.batch.static_dim
 
     def get_spatial_batch_axes(self):
         """
         :rtype: list[int]
         :return: list of axes which are not batch axes and not feature or which are time axis or dynamic.
           counted with batch-dim.
         """
```

### Comparing `returnn-1.20230411.132032/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230411.4301/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230411.4301/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230411.4301/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/dim.py` & `returnn-1.20230411.4301/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/marked_dim.py` & `returnn-1.20230411.4301/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/tensor.py` & `returnn-1.20230411.4301/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tensor/tensor_dict.py` & `returnn-1.20230411.4301/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/compat.py` & `returnn-1.20230411.4301/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/data_pipeline.py` & `returnn-1.20230411.4301/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/distributed.py` & `returnn-1.20230411.4301/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/engine.py` & `returnn-1.20230411.4301/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230411.4301/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230411.4301/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/horovod.py` & `returnn-1.20230411.4301/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230411.4301/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/layers/base.py` & `returnn-1.20230411.4301/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/layers/basic.py` & `returnn-1.20230411.4301/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/layers/rec.py` & `returnn-1.20230411.4301/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/layers/segmental_model.py` & `returnn-1.20230411.4301/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/layers/signal_processing.py` & `returnn-1.20230411.4301/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/native_op.py` & `returnn-1.20230411.4301/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/network.py` & `returnn-1.20230411.4301/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/sprint.py` & `returnn-1.20230411.4301/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/updater.py` & `returnn-1.20230411.4301/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/util/basic.py` & `returnn-1.20230411.4301/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/util/data.py` & `returnn-1.20230411.4301/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/util/ken_lm.py` & `returnn-1.20230411.4301/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/tf/util/open_fst.py` & `returnn-1.20230411.4301/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/data/pipeline.py` & `returnn-1.20230411.4301/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230411.4301/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/data/tensor_utils.py` & `returnn-1.20230411.4301/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/engine.py` & `returnn-1.20230411.4301/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/frontend/_backend.py` & `returnn-1.20230411.4301/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/frontend/_rand.py` & `returnn-1.20230411.4301/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/frontend/bridge.py` & `returnn-1.20230411.4301/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/torch/updater.py` & `returnn-1.20230411.4301/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/basic.py` & `returnn-1.20230411.4301/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/better_exchook.py` & `returnn-1.20230411.4301/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/bpe.py` & `returnn-1.20230411.4301/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/debug.py` & `returnn-1.20230411.4301/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/debug_helpers.py` & `returnn-1.20230411.4301/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/fsa.py` & `returnn-1.20230411.4301/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230411.4301/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/pprint.py` & `returnn-1.20230411.4301/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/py-to-pickle.cpp` & `returnn-1.20230411.4301/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/sig_proc.py` & `returnn-1.20230411.4301/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn/util/task_system.py` & `returnn-1.20230411.4301/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/returnn.egg-info/PKG-INFO` & `returnn-1.20230411.4301/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230411.132032
+Version: 1.20230411.4301
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230411.132032/returnn.egg-info/SOURCES.txt` & `returnn-1.20230411.4301/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/setup.py` & `returnn-1.20230411.4301/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/DummySprintExec.py` & `returnn-1.20230411.4301/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230411.4301/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230411.4301/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230411.4301/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/_set_num_threads1.py` & `returnn-1.20230411.4301/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/_setup_test_env.py` & `returnn-1.20230411.4301/tests/_setup_test_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,24 +60,21 @@
 
     from returnn.log import log
 
     # No propagate, use stdout directly.
     log.initialize(verbosity=[5], propagate=False)
 
     # TF is optional.
-    if "RETURNN_DISABLE_TF" in os.environ and int(os.environ["RETURNN_DISABLE_TF"]) == 1:
+    # Note that importing TF still has a small side effect:
+    # BackendEngine._get_default_engine() will return TF by default, if TF is already loaded.
+    # For most tests, this does not matter.
+    try:
+        import tensorflow as tf
+    except ImportError:
         tf = None
-    else:
-        # Note that importing TF still has a small side effect:
-        # BackendEngine._get_default_engine() will return TF by default, if TF is already loaded.
-        # For most tests, this does not matter.
-        try:
-            import tensorflow as tf
-        except ImportError:
-            tf = None
 
     if tf:
         import returnn.tf.util.basic as tf_util
 
         tf_util.debug_register_better_repr()
 
     import returnn.util.debug as debug
```

### Comparing `returnn-1.20230411.132032/tests/bpe-unicode-demo.codes` & `returnn-1.20230411.4301/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/bpe-unicode-demo.vocab` & `returnn-1.20230411.4301/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/lexicon_opt.isyms` & `returnn-1.20230411.4301/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/lexicon_opt.jpg` & `returnn-1.20230411.4301/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/lint_common.py` & `returnn-1.20230411.4301/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/pycharm-inspect.py` & `returnn-1.20230411.4301/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/pylint.py` & `returnn-1.20230411.4301/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/returnn-as-framework.py` & `returnn-1.20230411.4301/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/rf_utils.py` & `returnn-1.20230411.4301/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/spelling.dic` & `returnn-1.20230411.4301/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_Config.py` & `returnn-1.20230411.4301/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_Dataset.py` & `returnn-1.20230411.4301/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_Fsa.py` & `returnn-1.20230411.4301/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_GeneratingDataset.py` & `returnn-1.20230411.4301/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_HDFDataset.py` & `returnn-1.20230411.4301/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_LearningRateControl.py` & `returnn-1.20230411.4301/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_Log.py` & `returnn-1.20230411.4301/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_MultiProcDataset.py` & `returnn-1.20230411.4301/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_PTDataset.py` & `returnn-1.20230411.4301/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_Pretrain.py` & `returnn-1.20230411.4301/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_ResNet.py` & `returnn-1.20230411.4301/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_SprintDataset.py` & `returnn-1.20230411.4301/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_SprintInterface.py` & `returnn-1.20230411.4301/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TFEngine.py` & `returnn-1.20230411.4301/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TFNativeOp.py` & `returnn-1.20230411.4301/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TFNetworkLayer.py` & `returnn-1.20230411.4301/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230411.4301/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230411.4301/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TFUpdater.py` & `returnn-1.20230411.4301/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TFUtil.py` & `returnn-1.20230411.4301/tests/test_TFUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     assert_equal(d1.find_matching_dims(d2.get_dim_tag(0), is_equal_opts=is_equal_opts_match), [1])
     assert_equal(d1.find_matching_dims(d2.get_dim_tag(1), is_equal_opts=is_equal_opts_match), [1, 2])
 
     mapping = d1.find_matching_dim_map(d2, list(range(d2.batch_ndim)), is_equal_opts)  # maps d2 -> d1
     assert mapping[0] == 1 and mapping[1] == 2
 
     copied = d2.copy_compatible_to(d1)
-    assert copied.batch_ndim == d1.batch_ndim and copied.get_static_batch_dim() == 1 and copied.batch_shape == (1, 5, 1)
+    assert copied.batch_ndim == d1.batch_ndim and copied.batch.static_dim == 1 and copied.batch_shape == (1, 5, 1)
     print("copied compatible:", copied)
 
 
 def test_Data_get_all_dimension_tags_same_spatial_dim_twice():
     from returnn.tf.util.data import batch_dim, SpatialDim, FeatureDim
 
     time_dim = SpatialDim("time")
@@ -629,22 +629,22 @@
 
 def test_Data_copy_compatible_to_src_no_batch():
     d1 = Data(name="d1", shape=(None, 1), time_dim_axis=None)
     d1.placeholder = tf.zeros([d if (d is not None) else 1 for d in d1.batch_shape])
     d2 = Data(name="d2", shape=(), batch_dim_axis=None, time_dim_axis=None)
     d2.placeholder = tf.zeros([d if (d is not None) else 1 for d in d2.batch_shape])
     d3 = d2.copy_compatible_to(d1)
-    assert d3.get_static_batch_dim() == 1 and d3.batch_shape == (1, 1, 1)
+    assert d3.batch.static_dim == 1 and d3.batch_shape == (1, 1, 1)
 
 
 def test_Data_copy_compatible_to_add_batch_dim():
     common_data = Data(name="accum_att_weights_output", shape=(None, 1))
     d1 = Data(name="att_weights_avg_output", shape=(1,), batch_dim_axis=None)
     d2 = d1.copy_compatible_to(common_data)
-    assert d2.have_batch_axis() and d2.get_static_batch_dim() == 1 and d2.batch_shape == (1, 1, 1)
+    assert d2.have_batch_axis() and d2.batch.static_dim == 1 and d2.batch_shape == (1, 1, 1)
 
 
 def test_Data_copy_compatible_to_add_feature_dim():
     common_data = Data(name="energy", shape=(None, 3), time_dim_axis=0, batch_dim_axis=None)  # [T,F]
     d1 = Data(name="mask", shape=(None,), batch_dim_axis=None, time_dim_axis=0, feature_dim_axis=None)  # [T]
     d2 = d1.copy_compatible_to(common_data)
     assert d2.batch_dim_axis is None and d2.time_dim_axis is not None and d2.batch_shape == (None, 1)
@@ -654,15 +654,15 @@
     common_data = Data(name="energy", shape=(None, 3))  # [B,T,F]
     assert common_data.batch_shape == (None, None, 3)
     d1 = Data(name="mask", shape=(None,), batch_dim_axis=None, time_dim_axis=0, feature_dim_axis=None)  # [T]
     assert d1.batch_shape == (None,)
     d2 = d1.copy_compatible_to(common_data)
     print(d2)
     assert d2.have_batch_axis() and d2.have_time_axis()
-    assert d2.get_static_batch_dim() == 1  # batch-dim is broadcasted
+    assert d2.batch.static_dim == 1  # batch-dim is broadcasted
     assert d2.batch_shape == (1, None, 1)
 
 
 def test_Data_copy_compatible_to_add_time_dim():
     common_data = Data(name="energy", shape=(None, 3))  # [B,T,F]
     d1 = Data(name="mask", shape=(3,))  # [B,F]
     d2 = d1.copy_compatible_to(common_data)
```

### Comparing `returnn-1.20230411.132032/tests/test_TF_determinism.py` & `returnn-1.20230411.4301/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TaskSystem.py` & `returnn-1.20230411.4301/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230411.4301/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_TranslationDataset.py` & `returnn-1.20230411.4301/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_Util.py` & `returnn-1.20230411.4301/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_demos.py` & `returnn-1.20230411.4301/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_fork_exec.py` & `returnn-1.20230411.4301/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_hdf_dump.py` & `returnn-1.20230411.4301/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_rf_base.py` & `returnn-1.20230411.4301/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_tensor.py` & `returnn-1.20230411.4301/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_tools.py` & `returnn-1.20230411.4301/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_torch_frontend.py` & `returnn-1.20230411.4301/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tests/test_torch_internal_frontend.py` & `returnn-1.20230411.4301/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/analyze-dataset-batches.py` & `returnn-1.20230411.4301/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/bliss-collect-seq-lens.py` & `returnn-1.20230411.4301/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/bliss-dump-text.py` & `returnn-1.20230411.4301/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/bliss-get-segment-names.py` & `returnn-1.20230411.4301/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/bliss-to-ogg-zip.py` & `returnn-1.20230411.4301/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/bpe-create-lexicon.py` & `returnn-1.20230411.4301/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/calculate-word-error-rate.py` & `returnn-1.20230411.4301/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/cleanup-old-models.py` & `returnn-1.20230411.4301/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/collect-orth-symbols.py` & `returnn-1.20230411.4301/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/collect-words.py` & `returnn-1.20230411.4301/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/compile_native_op.py` & `returnn-1.20230411.4301/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/compile_tf_graph.py` & `returnn-1.20230411.4301/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/debug-dump-search-scores.py` & `returnn-1.20230411.4301/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/debug-plot-search-scores.py` & `returnn-1.20230411.4301/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/dump-dataset-raw-strings.py` & `returnn-1.20230411.4301/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/dump-dataset.py` & `returnn-1.20230411.4301/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/dump-forward-stats.py` & `returnn-1.20230411.4301/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/dump-forward.py` & `returnn-1.20230411.4301/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/dump-network-json.py` & `returnn-1.20230411.4301/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/dump-pickle.py` & `returnn-1.20230411.4301/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230411.4301/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/get-attention-weights.py` & `returnn-1.20230411.4301/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/get-best-model-epoch.py` & `returnn-1.20230411.4301/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/hdf_dump.py` & `returnn-1.20230411.4301/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230411.4301/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/import-blocks-mt-model.py` & `returnn-1.20230411.4301/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/import-t2t-mt-model.py` & `returnn-1.20230411.4301/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/Makefile` & `returnn-1.20230411.4301/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/README.md` & `returnn-1.20230411.4301/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/example/README.md` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230411.4301/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/file.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230411.4301/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/main.cc` & `returnn-1.20230411.4301/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230411.4301/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230411.4301/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/tf_avg_checkpoints.py` & `returnn-1.20230411.4301/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/tf_inspect_checkpoint.py` & `returnn-1.20230411.4301/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230411.132032/tools/tf_inspect_summary_log.py` & `returnn-1.20230411.4301/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

