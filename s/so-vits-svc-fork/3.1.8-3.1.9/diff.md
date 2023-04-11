# Comparing `tmp/so_vits_svc_fork-3.1.8.tar.gz` & `tmp/so_vits_svc_fork-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.1.8.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.1.9.tar", max compression
```

## Comparing `so_vits_svc_fork-3.1.8.tar` & `so_vits_svc_fork-3.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-10 10:50:42.816867 so_vits_svc_fork-3.1.8/LICENSE
--rw-r--r--   0        0        0    17996 2023-04-10 10:50:42.816867 so_vits_svc_fork-3.1.8/README.md
--rw-r--r--   0        0        0     3113 2023-04-10 10:50:43.808863 so_vits_svc_fork-3.1.8/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-10 10:50:43.760863 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22637 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2712 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7259 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    24381 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    22944 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0      731 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1627 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1377 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1438 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    16240 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-10 10:50:42.820867 so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.8/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-10 15:12:13.832778 so_vits_svc_fork-3.1.9/LICENSE
+-rw-r--r--   0        0        0    17996 2023-04-10 15:12:13.832778 so_vits_svc_fork-3.1.9/README.md
+-rw-r--r--   0        0        0     3113 2023-04-10 15:12:15.144885 so_vits_svc_fork-3.1.9/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-10 15:12:15.088879 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22637 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1275 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2712 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2826 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    24381 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    22944 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0      731 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1627 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1377 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1438 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2997 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4614 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4693 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    17588 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13081 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.9/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.1.8/LICENSE` & `so_vits_svc_fork-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/README.md` & `so_vits_svc_fork-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/pyproject.toml` & `so_vits_svc_fork-3.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.1.8"
+version = "3.1.9"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/f0.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         f0_max,
         model,
         batch_size=hop_length * 2,
         device=device,
         pad=True,
     )
 
-    f0 = pitch.squeeze(0).cpu().numpy()
+    f0 = pitch.squeeze(0).cpu().float().numpy()
     p_len = p_len or wav_numpy.shape[0] // hop_length
     f0 = _resize_f0(f0, p_len)
     return f0
 
 
 def compute_f0(
     wav_numpy: ndarray[Any, dtype[float32]],
```

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .modules.descriminators import MultiPeriodDiscriminator
 from .modules.losses import discriminator_loss, feature_loss, generator_loss, kl_loss
 from .modules.mel_processing import mel_spectrogram_torch
 from .modules.synthesizers import SynthesizerTrn
 
 LOG = getLogger(__name__)
 torch.backends.cudnn.benchmark = True
+torch.set_float32_matmul_precision("high")
 
 
 class VCDataModule(pl.LightningDataModule):
     def __init__(self, hparams: Any):
         super().__init__()
         self.__hparams = hparams
         self.collate_fn = TextAudioCollate()
@@ -67,17 +68,17 @@
     datamodule = VCDataModule(hparams)
     trainer = pl.Trainer(
         logger=TensorBoardLogger(model_path),
         # profiler="simple",
         val_check_interval=hparams.train.eval_interval,
         max_epochs=hparams.train.epochs,
         check_val_every_n_epoch=None,
-        precision=16
+        precision="16-mixed"
         if hparams.train.fp16_run
-        else "bf16"
+        else "bf16-mixed"
         if hparams.train.get("bf16_run", False)
         else 32,
     )
     model = VitsLightning(reset_optimizer=reset_optimizer, **hparams)
     trainer.fit(model, datamodule=datamodule)
 
 
@@ -155,14 +156,48 @@
                     normalized,
                     onesided,
                     return_complex,
                 ).to(device)
 
             torch.stft = stft
 
+        elif "bf" in self.trainer.precision:
+            LOG.warning("Using bf. Patching torch.stft to use fp32.")
+
+            def stft(
+                input: torch.Tensor,
+                n_fft: int,
+                hop_length: int | None = None,
+                win_length: int | None = None,
+                window: torch.Tensor | None = None,
+                center: bool = True,
+                pad_mode: str = "reflect",
+                normalized: bool = False,
+                onesided: bool | None = None,
+                return_complex: bool | None = None,
+            ) -> torch.Tensor:
+                dtype = input.dtype
+                input = input.float()
+                if window is not None:
+                    window = window.float()
+                return torch.functional.stft(
+                    input,
+                    n_fft,
+                    hop_length,
+                    win_length,
+                    window,
+                    center,
+                    pad_mode,
+                    normalized,
+                    onesided,
+                    return_complex,
+                ).to(dtype)
+
+            torch.stft = stft
+
     def set_current_epoch(self, epoch: int):
         LOG.info(f"Setting current epoch to {epoch}")
         self.trainer.fit_loop.epoch_progress.current.completed = epoch
         assert self.current_epoch == epoch, f"{self.current_epoch} != {epoch}"
 
     def set_global_step(self, global_step: int):
         LOG.info(f"Setting global step to {global_step}")
@@ -235,15 +270,15 @@
         if not isinstance(self.logger, TensorBoardLogger):
             warnings.warn("Audio logging is only supported with TensorBoardLogger.")
             return
         writer: SummaryWriter = self.logger.experiment
         for k, v in audio_dict.items():
             writer.add_audio(
                 k,
-                v,
+                v.float(),
                 self.total_batch_idx,
                 sample_rate=self.hparams.data.sampling_rate,
             )
 
     def log_dict_(self, log_dict: dict[str, Any], **kwargs) -> None:
         if not isinstance(self.logger, TensorBoardLogger):
             warnings.warn("Logging is only supported with TensorBoardLogger.")
@@ -330,29 +365,29 @@
         )
         if self.hparams.model.get("type_") == "mb-istft":
             self.log_("loss/g/subband", loss_subband)
         if self.total_batch_idx % self.hparams.train.log_interval == 0:
             self.log_image_dict(
                 {
                     "slice/mel_org": utils.plot_spectrogram_to_numpy(
-                        y_mel[0].data.cpu().numpy()
+                        y_mel[0].data.cpu().float().numpy()
                     ),
                     "slice/mel_gen": utils.plot_spectrogram_to_numpy(
-                        y_hat_mel[0].data.cpu().numpy()
+                        y_hat_mel[0].data.cpu().float().numpy()
                     ),
                     "all/mel": utils.plot_spectrogram_to_numpy(
-                        mel[0].data.cpu().numpy()
+                        mel[0].data.cpu().float().numpy()
                     ),
                     "all/lf0": so_vits_svc_fork.utils.plot_data_to_numpy(
-                        lf0[0, 0, :].cpu().numpy(),
-                        pred_lf0[0, 0, :].detach().cpu().numpy(),
+                        lf0[0, 0, :].cpu().float().numpy(),
+                        pred_lf0[0, 0, :].detach().cpu().float().numpy(),
                     ),
                     "all/norm_lf0": so_vits_svc_fork.utils.plot_data_to_numpy(
-                        lf0[0, 0, :].cpu().numpy(),
-                        norm_lf0[0, 0, :].detach().cpu().numpy(),
+                        lf0[0, 0, :].cpu().float().numpy(),
+                        norm_lf0[0, 0, :].detach().cpu().float().numpy(),
                     ),
                 }
             )
 
         # optimizer
         optim_g.zero_grad()
         self.manual_backward(loss_gen_all)
@@ -391,17 +426,19 @@
             y_hat_mel = mel_spectrogram_torch(y_hat.squeeze(1).float(), self.hparams)
             self.log_audio_dict(
                 {f"gen/audio_{batch_idx}": y_hat[0], f"gt/audio_{batch_idx}": y[0]}
             )
             self.log_image_dict(
                 {
                     "gen/mel": utils.plot_spectrogram_to_numpy(
-                        y_hat_mel[0].cpu().numpy()
+                        y_hat_mel[0].cpu().float().numpy()
+                    ),
+                    "gt/mel": utils.plot_spectrogram_to_numpy(
+                        mel[0].cpu().float().numpy()
                     ),
-                    "gt/mel": utils.plot_spectrogram_to_numpy(mel[0].cpu().numpy()),
                 }
             )
             if self.current_epoch == 0 or batch_idx != 0:
                 return
             utils.save_checkpoint(
                 self.net_g,
                 self.optim_g,
```

### Comparing `so_vits_svc_fork-3.1.8/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.8/PKG-INFO` & `so_vits_svc_fork-3.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.1.8
+Version: 3.1.9
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.8 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.9 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

