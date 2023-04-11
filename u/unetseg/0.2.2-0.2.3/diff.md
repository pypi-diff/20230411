# Comparing `tmp/unetseg-0.2.2.tar.gz` & `tmp/unetseg-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unetseg-0.2.2.tar", last modified: Mon Feb  7 19:32:25 2022, max compression
+gzip compressed data, was "unetseg-0.2.3.tar", max compression
```

## Comparing `unetseg-0.2.2.tar` & `unetseg-0.2.3.tar`

### file list

```diff
@@ -1,49 +1,11 @@
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.696624 unetseg-0.2.2/
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      590 2021-04-20 19:24:57.000000 unetseg-0.2.2/.coveragerc
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      550 2021-04-20 19:24:57.000000 unetseg-0.2.2/.gitignore
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)       55 2021-04-20 19:24:57.000000 unetseg-0.2.2/.isort.cfg
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     1330 2021-11-10 13:00:14.000000 unetseg-0.2.2/.pre-commit-config.yaml
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      461 2021-04-20 19:24:57.000000 unetseg-0.2.2/.readthedocs.yml
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      217 2021-04-20 19:28:32.000000 unetseg-0.2.2/AUTHORS.md
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      831 2022-02-02 12:29:36.000000 unetseg-0.2.2/CHANGELOG.md
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)    11357 2021-04-20 19:28:11.000000 unetseg-0.2.2/LICENSE.txt
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     3209 2022-02-07 19:32:25.696624 unetseg-0.2.2/PKG-INFO
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     2444 2021-08-18 16:44:16.000000 unetseg-0.2.2/README-ES.md
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     2186 2021-08-18 16:44:16.000000 unetseg-0.2.2/README.md
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.692624 unetseg-0.2.2/docs/
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     1153 2021-04-20 19:24:57.000000 unetseg-0.2.2/docs/Makefile
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.692624 unetseg-0.2.2/docs/_static/
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)       18 2021-04-20 19:24:57.000000 unetseg-0.2.2/docs/_static/.gitignore
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      217 2021-04-20 19:28:32.000000 unetseg-0.2.2/docs/authors.md
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      831 2022-02-02 12:29:36.000000 unetseg-0.2.2/docs/changelog.md
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)    10031 2022-01-11 12:53:14.000000 unetseg-0.2.2/docs/conf.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     1052 2021-04-20 19:24:57.000000 unetseg-0.2.2/docs/index.md
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)       67 2021-04-20 19:24:57.000000 unetseg-0.2.2/docs/license.rst
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     2186 2021-08-18 16:44:16.000000 unetseg-0.2.2/docs/readme.md
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      277 2022-01-11 12:35:37.000000 unetseg-0.2.2/docs/requirements.txt
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      311 2021-04-20 19:24:57.000000 unetseg-0.2.2/pyproject.toml
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     1506 2022-02-07 19:32:25.696624 unetseg-0.2.2/setup.cfg
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      704 2021-04-20 19:24:57.000000 unetseg-0.2.2/setup.py
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.688624 unetseg-0.2.2/src/
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.696624 unetseg-0.2.2/src/unetseg/
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      363 2021-07-05 11:54:52.000000 unetseg-0.2.2/src/unetseg/__init__.py
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.696624 unetseg-0.2.2/src/unetseg/console/
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     3537 2021-07-05 11:54:58.000000 unetseg-0.2.2/src/unetseg/console/predict.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     4998 2021-07-05 11:55:00.000000 unetseg-0.2.2/src/unetseg/console/train.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     4060 2022-02-07 19:31:58.000000 unetseg-0.2.2/src/unetseg/evaluate.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     3662 2022-01-11 12:24:26.000000 unetseg-0.2.2/src/unetseg/postprocess.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     3876 2022-01-11 12:33:28.000000 unetseg-0.2.2/src/unetseg/predict.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     4227 2021-07-05 11:54:47.000000 unetseg-0.2.2/src/unetseg/skeleton.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)    21703 2022-01-13 16:10:09.000000 unetseg-0.2.2/src/unetseg/train.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      842 2022-01-13 16:10:09.000000 unetseg-0.2.2/src/unetseg/utils.py
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.696624 unetseg-0.2.2/src/unetseg.egg-info/
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     3209 2022-02-07 19:32:25.000000 unetseg-0.2.2/src/unetseg.egg-info/PKG-INFO
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      801 2022-02-07 19:32:25.000000 unetseg-0.2.2/src/unetseg.egg-info/SOURCES.txt
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)        1 2022-02-07 19:32:25.000000 unetseg-0.2.2/src/unetseg.egg-info/dependency_links.txt
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)        1 2021-05-10 13:34:46.000000 unetseg-0.2.2/src/unetseg.egg-info/not-zip-safe
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      295 2022-02-07 19:32:25.000000 unetseg-0.2.2/src/unetseg.egg-info/requires.txt
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)        8 2022-02-07 19:32:25.000000 unetseg-0.2.2/src/unetseg.egg-info/top_level.txt
-drwxrwxr-x   0 munshkr   (1000) munshkr   (1000)        0 2022-02-07 19:32:25.696624 unetseg-0.2.2/tests/
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      275 2021-04-20 19:24:57.000000 unetseg-0.2.2/tests/conftest.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)      594 2021-04-29 18:21:26.000000 unetseg-0.2.2/tests/test_skeleton.py
--rw-rw-r--   0 munshkr   (1000) munshkr   (1000)     2010 2021-04-20 19:24:57.000000 unetseg-0.2.2/tox.ini
+-rw-r--r--   0        0        0    11357 2023-04-11 14:43:39.872672 unetseg-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0      876 2023-04-11 14:50:20.255825 unetseg-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-04-11 14:43:39.885340 unetseg-0.2.3/unetseg/__init__.py
+-rw-r--r--   0        0        0     3537 2023-04-11 14:43:39.885514 unetseg-0.2.3/unetseg/console/predict.py
+-rw-r--r--   0        0        0     4998 2023-04-11 14:43:39.885650 unetseg-0.2.3/unetseg/console/train.py
+-rw-r--r--   0        0        0     3861 2023-04-11 14:43:39.885769 unetseg-0.2.3/unetseg/evaluate.py
+-rw-r--r--   0        0        0     3662 2023-04-11 14:43:39.885918 unetseg-0.2.3/unetseg/postprocess.py
+-rw-r--r--   0        0        0     3810 2023-04-11 14:43:39.886056 unetseg-0.2.3/unetseg/predict.py
+-rw-r--r--   0        0        0    22083 2023-04-11 14:43:39.886268 unetseg-0.2.3/unetseg/train.py
+-rw-r--r--   0        0        0      842 2023-04-11 14:43:39.886391 unetseg-0.2.3/unetseg/utils.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 unetseg-0.2.3/PKG-INFO
```

### Comparing `unetseg-0.2.2/LICENSE.txt` & `unetseg-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.2/src/unetseg/console/predict.py` & `unetseg-0.2.3/unetseg/console/predict.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.2/src/unetseg/console/train.py` & `unetseg-0.2.3/unetseg/console/train.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.2/src/unetseg/evaluate.py` & `unetseg-0.2.3/unetseg/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import random
 from glob import glob
 
 import matplotlib.pyplot as plt
 import numpy as np
 import tifffile as tiff
 from skimage.transform import resize
-from sklearn.preprocessing import minmax_scale
 
 from unetseg.predict import PredictConfig
 from unetseg.train import TrainConfig, build_data_generator
 
 
 def plot_data_generator(
     num_samples: int = 3,
@@ -33,16 +32,14 @@
     train_config : TrainConfig
         Training configuration object.
 
     """
 
     if train_config.n_channels < 4:
         img_ch = train_config.n_channels
-    else:
-        img_ch = img_ch
 
     images_dir = os.path.join(train_config.images_path, "images")
     mask_dir = train_config.masks_path or os.path.join(
         train_config.images_path, "extent"
     )
 
     images = glob(os.path.join(images_dir, "*.tif"))
@@ -70,14 +67,15 @@
                 j += 1
                 if j >= num:
                     return
 
     plot_samples(plt, data_generator, num_samples)
     plt.show()
 
+
 def plot_data_results(
     num_samples: int = 3,
     fig_size=(20, 10),
     *,
     predict_config: PredictConfig,
     img_ch: int = 3,
     n_bands: int = 3
@@ -102,49 +100,45 @@
     ]
 
     images = random.sample(images, num_samples)
     for img_file in images:
         try:
             if n_bands not in (1, 3):
                 raise RuntimeError("n_bands option must be 1 or 3")
-            
+
             fig, axes = plt.subplots(
                 nrows=1, ncols=predict_config.n_classes + 1, figsize=(20, 40)
             )
-                 
+
             if n_bands == 1:
-          
+
                 img_s2 = tiff.imread(
                     os.path.join(predict_config.images_path, "images", img_file)
                 )[:, :, img_ch]
                 axes[0].imshow(img_s2)
-               
+
             if n_bands == 3:
-             
+
                 img_s2 = tiff.imread(
                     os.path.join(predict_config.images_path, "images", img_file)
                 )[:, :, :3]
                 axes[0].imshow(img_s2)
-            
+
             # Prediccion
             mask_ = (
                 tiff.imread(os.path.join(predict_config.results_path, img_file)) / 255
             )
-   
+
             mask_ = resize(
                 mask_,
                 (predict_config.height, predict_config.width, predict_config.n_classes),
                 mode="constant",
                 preserve_range=True,
             )
 
-          
-           
-            
-
             for c in range(predict_config.n_classes):
                 axes[1 + c].imshow(np.squeeze(mask_[:, :, c]))
 
             plt.show()
 
         except Exception as err:
             print(err)
```

### Comparing `unetseg-0.2.2/src/unetseg/postprocess.py` & `unetseg-0.2.3/unetseg/postprocess.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.2/src/unetseg/predict.py` & `unetseg-0.2.3/unetseg/predict.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 import warnings
+from dataclasses import dataclass
 from glob import glob
+from typing import List
 
-import attr
 import numpy as np
 import rasterio
 from sklearn.preprocessing import minmax_scale
 from tqdm import tqdm
 
 from unetseg.train import build_model_unet, build_model_unetplusplus
 from unetseg.utils import grouper, resize
 
 warnings.filterwarnings("ignore", category=UserWarning, module="skimage")
 
 
-@attr.s
+@dataclass
 class PredictConfig:
-    images_path = attr.ib(default="")
-    results_path = attr.ib(default="")
-    batch_size = attr.ib(default=32)
-    model_architecture = attr.ib(default="unet")
-    model_path = attr.ib(default="unet.h5")
-    height = attr.ib(default=320)
-    width = attr.ib(default=320)
-    n_channels = attr.ib(default=3)
-    n_classes = attr.ib(default=1)
-    class_weights = attr.ib(default=0)
+    images_path: str
+    results_path: str = "."
+    batch_size: int = 32
+    model_architecture: str = "unet"
+    model_path: str = "unet.h5"
+    height: int = 320
+    width: int = 320
+    n_channels: int = 3
+    n_classes: int = 1
+    class_weights: List[float] = []
 
 
 def predict(cfg: PredictConfig):
     """
     Performs inference based on a configuration object
 
     Parameters
```

### Comparing `unetseg-0.2.2/src/unetseg/train.py` & `unetseg-0.2.3/unetseg/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import math
 import os
 import random
 import warnings
+from dataclasses import dataclass
 from glob import glob
 from typing import List, Tuple
-
+from datetime import datetime
 import albumentations as A
-import attr
 import numpy as np
 import rasterio
 import tensorflow as tf
 from sklearn.preprocessing import minmax_scale
 from tensorflow.compat.v1.keras import backend as K
-from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint
+from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, TensorBoard,CSVLogger
 from tensorflow.keras.layers import (
     BatchNormalization,
     Conv2D,
     Conv2DTranspose,
     Dropout,
     Input,
     LeakyReLU,
@@ -26,34 +27,34 @@
 from tensorflow.keras.models import Model
 
 from unetseg.utils import resize
 
 warnings.filterwarnings("ignore", category=UserWarning, module="skimage")
 
 
-@attr.s
+@dataclass
 class TrainConfig:
-    images_path = attr.ib()
-    masks_path = attr.ib(default=None)
-    width = attr.ib(default=200)
-    height = attr.ib(default=200)
-    n_channels = attr.ib(default=3)
-    n_classes = attr.ib(default=1)
-    apply_image_augmentation = attr.ib(default=True)
-    model_path = attr.ib(default="unet.h5")
-    model_architecture = attr.ib(default="unet")
-    validation_split = attr.ib(default=0.1)
-    test_split = attr.ib(default=0.1)
-    epochs = attr.ib(default=15)
-    steps_per_epoch = attr.ib(default=2000)
-    early_stopping_patience = attr.ib(default=3)
-    batch_size = attr.ib(default=32)
-    seed = attr.ib(default=None)
-    evaluate = attr.ib(default=True)
-    class_weights = attr.ib(default=0)
+    images_path: str
+    masks_path: str
+    width: int = 200
+    height: int = 200
+    n_channels: int = 3
+    n_classes: int = 1
+    apply_image_augmentation: bool = True
+    model_path: str = "unet.h5"
+    model_architecture: str = "unet"
+    validation_split: float = 0.1
+    test_split: float = 0.1
+    epochs: int = 15
+    steps_per_epoch: int = 2000
+    early_stopping_patience: int = 3
+    batch_size: int = 32
+    seed: int = None
+    evaluate: bool = True
+    class_weights: List[float] = []
 
 
 def build_model_unetplusplus(cfg: TrainConfig) -> Model:
     """
     Builds a U-Net++ model.
 
     Parameters
@@ -63,16 +64,16 @@
 
     Returns
     -------
     Model
         The U-Net++ model.
 
     """
-    # NOTE: for now, classes are equally balanced
-    if cfg.class_weights == 0:
+    # Classes are equally balanced by default
+    if not cfg.class_weights:
         cfg.class_weights = [0.5 for _ in range(cfg.n_classes)]
 
     # growth_factor = 2
     # droprate = 0.25
     number_of_filters = 2
     # upconv = True
     # batch_size = cfg.batch_size
@@ -263,16 +264,16 @@
 
     Returns
     -------
     Model
         U-Net model class.
 
     """
-    # NOTE: for now, classes are equally balanced
-    if cfg.class_weights == 0:
+    # Classes are equally balanced by default
+    if not cfg.class_weights:
         cfg.class_weights = [0.5 for _ in range(cfg.n_classes)]
 
     growth_factor = 2
     n_filters_start = 32
     droprate = 0.25
     n_filters = n_filters_start
     upconv = True
@@ -577,14 +578,21 @@
 
     Parameters
     ----------
     cfg : TrainConfig
         Configuration object containing all the necessary parameters for training.
 
     """
+    #Save date and time
+    # datetime object containing current date and time
+    now = datetime.now()
+    dt_string = now.strftime("Date_%d-%m-%Y_Time_%H-%M-%S")
+
+    
+    
     if cfg.seed:
         random.seed = cfg.seed
         np.random.seed = cfg.seed
 
     if cfg.model_architecture == "unet":
         model = build_model_unet(cfg)
         print(model.summary())
@@ -627,33 +635,39 @@
 
     # Make sure weights dir exist
     os.makedirs(os.path.dirname(cfg.model_path), exist_ok=True)
 
     print("Compile and fit the UNet model")
     early_stopping = EarlyStopping(patience=cfg.early_stopping_patience, verbose=1)
     checkpoint = ModelCheckpoint(cfg.model_path, verbose=1, save_best_only=True)
+    
+    head, tail = os.path.split(cfg.model_path)
+    log_file = tail[:-3]
+    print(log_file)
+    os.makedirs('./../logs', exist_ok=True)
+    log_csv = CSVLogger ( f'./../logs/my_logs.csv',separator = ',',append=False)
+    tensorboard = TensorBoard(log_dir = f'./../logs/{log_file}_{dt_string}')
     # reduce_lr = ReduceLROnPlateau(monitor='val_loss', factor=0.2,
     #                               patience=5, min_lr=0.001)
 
     results = model.fit(
         train_generator,
         epochs=cfg.epochs,
         steps_per_epoch=cfg.steps_per_epoch,
         validation_data=val_generator,
         validation_steps=round(cfg.steps_per_epoch * cfg.validation_split),
-        callbacks=[early_stopping, checkpoint],
+        callbacks=[early_stopping, checkpoint,tensorboard,log_csv],
     )
 
     # Save model
     model.save(cfg.model_path)
 
     # Evaluate model on test set
     if cfg.evaluate:
-        scores = model.evaluate(
-            test_generator, steps=len(test_images) // cfg.batch_size
-        )
+        steps = math.ceil(len(test_images) / cfg.batch_size)
+        scores = model.evaluate(test_generator, steps=steps)
         loss, mean_iou = scores
         print("*** Final  metrics ***")
         print("Loss:", loss)
         print("Mean IoU:", mean_iou)
 
     return results
```

### Comparing `unetseg-0.2.2/src/unetseg/utils.py` & `unetseg-0.2.3/unetseg/utils.py`

 * *Files identical despite different names*

