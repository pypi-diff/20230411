# Comparing `tmp/cloud_diffusion-0.4.0.tar.gz` & `tmp/cloud_diffusion-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_diffusion-0.4.0.tar", last modified: Thu Mar 23 09:07:58 2023, max compression
+gzip compressed data, was "cloud_diffusion-0.5.1.tar", last modified: Tue Apr 11 07:23:18 2023, max compression
```

## Comparing `cloud_diffusion-0.4.0.tar` & `cloud_diffusion-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:07:58.341584 cloud_diffusion-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-23 09:07:58.341584 cloud_diffusion-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:07:58.341584 cloud_diffusion-0.4.0/cloud_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/cloud_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/cloud_diffusion/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/cloud_diffusion/ddpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/cloud_diffusion/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/cloud_diffusion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/cloud_diffusion/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/cloud_diffusion/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:07:58.341584 cloud_diffusion-0.4.0/cloud_diffusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-23 09:07:58.000000 cloud_diffusion-0.4.0/cloud_diffusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-23 09:07:58.000000 cloud_diffusion-0.4.0/cloud_diffusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 09:07:58.000000 cloud_diffusion-0.4.0/cloud_diffusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 09:07:58.000000 cloud_diffusion-0.4.0/cloud_diffusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-23 09:07:58.000000 cloud_diffusion-0.4.0/cloud_diffusion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 09:07:58.341584 cloud_diffusion-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-23 09:07:46.000000 cloud_diffusion-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:18.438861 cloud_diffusion-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 07:23:18.438861 cloud_diffusion-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:18.438861 cloud_diffusion-0.5.1/cloud_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/ddpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/cloud_diffusion/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:18.438861 cloud_diffusion-0.5.1/cloud_diffusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 07:23:18.000000 cloud_diffusion-0.5.1/cloud_diffusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-11 07:23:18.000000 cloud_diffusion-0.5.1/cloud_diffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:23:18.000000 cloud_diffusion-0.5.1/cloud_diffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-11 07:23:18.000000 cloud_diffusion-0.5.1/cloud_diffusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 07:23:18.000000 cloud_diffusion-0.5.1/cloud_diffusion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:23:18.438861 cloud_diffusion-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 07:22:56.000000 cloud_diffusion-0.5.1/setup.py
```

### Comparing `cloud_diffusion-0.4.0/PKG-INFO` & `cloud_diffusion-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud_diffusion
-Version: 0.4.0
+Version: 0.5.1
 Summary: Diffusion on the Clouds: Short-term solar energy forecasting with Diffusion Models
 Home-page: https://github.com/tcapelle/cloud_diffusion
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,pytorch,stable diffusion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cloud_diffusion-0.4.0/README.md` & `cloud_diffusion-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 [![](https://raw.githubusercontent.com/wandb/assets/main/wandb-github-badge-gradient.svg)](https://wandb.ai/capecape/ddpm_clouds/reports/Diffusion-on-the-Clouds-Short-term-solar-energy-forecasting-with-Diffusion-Models--VmlldzozNDMxNTg5)
 [![PyPI version](https://badge.fury.io/py/cloud_diffusion.svg)](https://badge.fury.io/py/cloud_diffusion)
 
 
 # Cloud Diffusion Experiment
 
-This codebase contains an implementation of a deep diffusion model applied to cloud images. It was developed as part of a research project exploring the potential of diffusion models
-for image generation and forecasting.
+This codebase contains an implementation of a deep diffusion model applied to cloud images. It was developed as part of a research project exploring the potential of diffusion models for image generation and forecasting.
 
 ## Setup
 
 1. Clone this repository and run `pip install -e .` or `pip install cloud_diffusion`
 2. Set up your WandB account by signing up at [wandb.ai](https://wandb.ai/site).
 3. Set up your WandB API key by running `wandb login` and following the prompts.
 
 ## Usage
 
 To train the model, run `python train.py`. You can play with the parameters on top of the file to change the model architecture, training parameters, etc.
 
 You can also override the configuration parameters by passing them as command-line arguments, e.g.
+
 ```bash
 > python train.py --epochs=10 --batch_size=32
 ```
 
 ## Training a Simple Diffusion Model
 
 This training is based on a Transformer based Unet (UViT), you can train the default model by running:
 
 ```bash
-
 > python train_uvit.py
 ```
 
 ## Running Inference
 If you are only interested on using the trained models, you can run inference by running:
 
 ```bash
```

### Comparing `cloud_diffusion-0.4.0/cloud_diffusion/dataset.py` & `cloud_diffusion-0.5.1/cloud_diffusion/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,28 @@
 from fastprogress import progress_bar
 
 from cloud_diffusion.utils import ls
 
 PROJECT_NAME = "ddpm_clouds"
 DATASET_ARTIFACT = 'capecape/gtc/np_dataset:v0'
 
+class DummyNextFrameDataset:
+    "Dataset that returns random images"
+    def __init__(self, num_frames=4, img_size=64, N=1000):
+        self.img_size = img_size
+        self.num_frames = num_frames
+        self.N = N
+
+    def __getitem__(self, idx):
+        return torch.randn(self.num_frames, self.img_size, self.img_size)
+    
+    def __len__(self):
+        return self.N
+
+
 class CloudDataset:
     """Dataset for cloud images
     It loads numpy files from wandb artifact and stacks them into a single array
     It also applies some transformations to the images
     """
     def __init__(self, 
                  files, # list of numpy files to load (they come from the artifact)
```

### Comparing `cloud_diffusion-0.4.0/cloud_diffusion/simple_diffusion.py` & `cloud_diffusion-0.5.1/cloud_diffusion/simple_diffusion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,49 @@
 from functools import partial
 
-import torch, math
-from torch import nn, sqrt
+import torch
+from torch import sqrt
 from torch.special import expm1
-from torch.utils.data import DataLoader
-from torch.utils.data.dataloader import default_collate
 
 from fastprogress import progress_bar
 
 from einops import repeat
 
 try:
-    from denoising_diffusion_pytorch.simple_diffusion import (
-        UViT, right_pad_dims_to, logsnr_schedule_cosine
-    )
+    from denoising_diffusion_pytorch.simple_diffusion import right_pad_dims_to, logsnr_schedule_cosine
 except:
     raise ImportError("Please install denoising_diffusion_pytorch with `pip install denoising_diffusion_pytorch`")
 
 def q_sample(x_start, times, noise):
     log_snr = logsnr_schedule_cosine(times)
 
     log_snr_padded = right_pad_dims_to(x_start, log_snr)
     alpha, sigma = torch.sqrt(log_snr_padded.sigmoid()), torch.sqrt((-log_snr_padded).sigmoid())
     x_noised =  x_start * alpha + noise * sigma
 
     return x_noised, log_snr
 
-def noisify(frames, pred_objective="v"):
-    past_frames = frames[:,:-1]
-    last_frame  = frames[:,-1:]
-    device = frames.device
+def noisify_uvit(x0, pred_objective="v"):
+    device = x0.device
     
-    noise =  torch.randn_like(last_frame)
-    times = torch.zeros((last_frame.shape[0],), device = device).float().uniform_(0, 1)
-    x, log_snr = q_sample(last_frame, times, noise)
+    noise =  torch.randn_like(x0)
+    times = torch.zeros((x0.shape[0],), device = device).float().uniform_(0, 1)
+    x, log_snr = q_sample(x0, times, noise)
     
     if pred_objective == 'v':
         padded_log_snr = right_pad_dims_to(x, log_snr)
         alpha, sigma = padded_log_snr.sigmoid().sqrt(), (-padded_log_snr).sigmoid().sqrt()
-        target = alpha * noise - sigma * last_frame
+        target = alpha * noise - sigma * x0
 
     elif pred_objective == 'eps':
         target = noise
         
-    return torch.cat([past_frames, x], dim=1), log_snr, target
+    return x, log_snr, target
+
 
-def collate_simple_diffusion(b): 
-    "Collate function that noisifies the last frame"
-    return noisify(default_collate(b))
-
-def get_uvit_params(model_name="uvit_small", num_frames=4):
-    "Return the parameters for the diffusers UViT model"
-    if model_name == "uvit_small":
-        return dict(
-            dim=512,
-            ff_mult=2,
-            vit_depth=4,
-            channels=4, 
-            patch_size=4,
-            final_img_itransform=nn.Conv2d(num_frames,1,1)
-            )
-    elif model_name == "uvit_big":
-        return dict(
-            dim=1024,
-            ff_mult=4,
-            vit_depth=8,
-            channels=4, 
-            patch_size=4,
-            final_img_itransform=nn.Conv2d(num_frames,1,1)
-            )
-    else:
-        raise(f"Model name not found: {model_name}, choose between 'uvit_small' or 'uvit_big'")
     
 # Sampling functions
 
 @torch.no_grad()
 def forward(model, past_frames, x, t):
     return model(torch.cat([past_frames, x], dim=1), t)
 
@@ -134,8 +103,8 @@
     new_frame.clamp_(-1., 1.)
     return new_frame
 
 
 def simple_diffusion_sampler(steps=500):
     """Returns a function that samples from the diffusion model using
     the simple diffusion sampling scheme"""
-    return partial(p_sample_loop, steps=500)
+    return partial(p_sample_loop, steps=steps)
```

### Comparing `cloud_diffusion-0.4.0/cloud_diffusion/wandb.py` & `cloud_diffusion-0.5.1/cloud_diffusion/wandb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 import torch
 import wandb
 import numpy as np
 
 ## For Training
 
 def to_wandb_image(img):
```

### Comparing `cloud_diffusion-0.4.0/cloud_diffusion.egg-info/PKG-INFO` & `cloud_diffusion-0.5.1/cloud_diffusion.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-diffusion
-Version: 0.4.0
+Version: 0.5.1
 Summary: Diffusion on the Clouds: Short-term solar energy forecasting with Diffusion Models
 Home-page: https://github.com/tcapelle/cloud_diffusion
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,pytorch,stable diffusion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cloud_diffusion-0.4.0/setup.py` & `cloud_diffusion-0.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         "torch",
         "fastprogress",
         "fastcore",
         "wandb",
         "numpy",
         "matplotlib",
         "diffusers",
+        "denoising_diffusion_pytorch",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
```

