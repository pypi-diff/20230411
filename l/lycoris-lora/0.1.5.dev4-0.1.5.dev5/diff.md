# Comparing `tmp/lycoris_lora-0.1.5.dev4.tar.gz` & `tmp/lycoris_lora-0.1.5.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.5.dev4.tar", last modified: Mon Apr 10 10:29:49 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.5.dev5.tar", last modified: Tue Apr 11 14:47:33 2023, max compression
```

## Comparing `lycoris_lora-0.1.5.dev4.tar` & `lycoris_lora-0.1.5.dev5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:29:49.246759 lycoris_lora-0.1.5.dev4/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev4/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.5.dev4/Algo.md
--rw-rw-rw-   0        0        0      552 2023-03-29 07:12:55.000000 lycoris_lora-0.1.5.dev4/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.5.dev4/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev4/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-04-10 10:29:49.246259 lycoris_lora-0.1.5.dev4/PKG-INFO
--rw-rw-rw-   0        0        0     6498 2023-04-10 10:28:19.000000 lycoris_lora-0.1.5.dev4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 10:29:49.229256 lycoris_lora-0.1.5.dev4/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.5.dev4/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.5.dev4/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.5.dev4/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.5.dev4/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.5.dev4/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev4/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.5.dev4/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.5.dev4/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:29:49.233256 lycoris_lora-0.1.5.dev4/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev4/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.5.dev4/lycoris/ia3.py
--rw-rw-rw-   0        0        0    21293 2023-04-10 10:28:50.000000 lycoris_lora-0.1.5.dev4/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.5.dev4/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev4/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3178 2023-04-07 16:38:33.000000 lycoris_lora-0.1.5.dev4/lycoris/locon.py
--rw-rw-rw-   0        0        0     7657 2023-04-07 16:38:27.000000 lycoris_lora-0.1.5.dev4/lycoris/loha.py
--rw-rw-rw-   0        0        0     8974 2023-04-08 05:53:19.000000 lycoris_lora-0.1.5.dev4/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20461 2023-04-09 14:56:53.000000 lycoris_lora-0.1.5.dev4/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:29:49.245259 lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-04-10 10:29:49.000000 lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-04-10 10:29:49.000000 lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:29:49.000000 lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-10 10:29:49.000000 lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-10 10:29:49.000000 lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 10:29:49.246759 lycoris_lora-0.1.5.dev4/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-04-10 10:29:37.000000 lycoris_lora-0.1.5.dev4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:29:49.245759 lycoris_lora-0.1.5.dev4/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.5.dev4/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2807 2023-03-11 01:44:13.000000 lycoris_lora-0.1.5.dev4/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.751890 lycoris_lora-0.1.5.dev5/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.5.dev5/Algo.md
+-rw-rw-rw-   0        0        0      552 2023-03-29 07:12:55.000000 lycoris_lora-0.1.5.dev5/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.5.dev5/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-04-11 14:47:33.751387 lycoris_lora-0.1.5.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0     6498 2023-04-10 10:28:19.000000 lycoris_lora-0.1.5.dev5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.720668 lycoris_lora-0.1.5.dev5/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.5.dev5/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.5.dev5/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.5.dev5/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.5.dev5/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.5.dev5/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.5.dev5/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.5.dev5/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.727698 lycoris_lora-0.1.5.dev5/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     5731 2023-04-11 14:46:32.000000 lycoris_lora-0.1.5.dev5/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.5.dev5/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    21360 2023-04-11 04:27:42.000000 lycoris_lora-0.1.5.dev5/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.5.dev5/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     3178 2023-04-07 16:38:33.000000 lycoris_lora-0.1.5.dev5/lycoris/locon.py
+-rw-rw-rw-   0        0        0     7657 2023-04-07 16:38:27.000000 lycoris_lora-0.1.5.dev5/lycoris/loha.py
+-rw-rw-rw-   0        0        0     8974 2023-04-08 05:53:19.000000 lycoris_lora-0.1.5.dev5/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-04-10 16:04:23.000000 lycoris_lora-0.1.5.dev5/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.749383 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 14:47:33.752392 lycoris_lora-0.1.5.dev5/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-04-11 14:46:58.000000 lycoris_lora-0.1.5.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.750383 lycoris_lora-0.1.5.dev5/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.5.dev5/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-04-10 15:31:09.000000 lycoris_lora-0.1.5.dev5/tools/merge.py
```

### Comparing `lycoris_lora-0.1.5.dev4/.gitignore` & `lycoris_lora-0.1.5.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/Algo.md` & `lycoris_lora-0.1.5.dev5/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/Change.md` & `lycoris_lora-0.1.5.dev5/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/Demo.md` & `lycoris_lora-0.1.5.dev5/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/LICENSE.md` & `lycoris_lora-0.1.5.dev5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/README.md` & `lycoris_lora-0.1.5.dev5/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/better_conv.py` & `lycoris_lora-0.1.5.dev5/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/better_conv_extract.py` & `lycoris_lora-0.1.5.dev5/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/concept_neuron.py` & `lycoris_lora-0.1.5.dev5/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/locon_extract_test.py` & `lycoris_lora-0.1.5.dev5/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/locon_merge_test.py` & `lycoris_lora-0.1.5.dev5/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/singular_value_test.py` & `lycoris_lora-0.1.5.dev5/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.5.dev5/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/experiments/time_test.py` & `lycoris_lora-0.1.5.dev5/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/ia3.py` & `lycoris_lora-0.1.5.dev5/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/kohya.py` & `lycoris_lora-0.1.5.dev5/lycoris/kohya.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import torch
 
 from .kohya_utils import *
 from .locon import LoConModule
 from .loha import LohaModule
 from .ia3 import IA3Module
 from .lokr import LokrModule
+from .dylora import DyLoraModule
 
 
 def create_network(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
     if network_dim is None:
         network_dim = 4                     # default
     conv_dim = int(kwargs.get('conv_dim', network_dim))
     conv_alpha = float(kwargs.get('conv_alpha', network_alpha))
@@ -28,14 +29,15 @@
               or kwargs.get('use_conv_cp', False))
     network_module = {
         'lora': LoConModule,
         'locon': LoConModule,
         'loha': LohaModule,
         'ia3':  IA3Module,
         'lokr': LokrModule,
+        'dylora': DyLoraModule,
     }[algo]
     
     print(f'Using rank adaptation algo: {algo}')
     
     if ((algo == 'loha' or algo == 'lokr')
         and not kwargs.get('no_dim_warn', False) 
         and (network_dim>64 or conv_dim>64)):
```

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.5.dev5/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/kohya_utils.py` & `lycoris_lora-0.1.5.dev5/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/locon.py` & `lycoris_lora-0.1.5.dev5/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/loha.py` & `lycoris_lora-0.1.5.dev5/lycoris/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/lokr.py` & `lycoris_lora-0.1.5.dev5/lycoris/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/lycoris/utils.py` & `lycoris_lora-0.1.5.dev5/lycoris/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,36 +60,14 @@
     diff = (weight - (U @ Vh).reshape(out_ch, in_ch, kernel_size, kernel_size)).detach()
     extract_weight_A = Vh.reshape(lora_rank, in_ch, kernel_size, kernel_size).detach()
     extract_weight_B = U.reshape(out_ch, lora_rank, 1, 1).detach()
     del U, S, Vh, weight
     return (extract_weight_A, extract_weight_B, diff), 'low rank'
 
 
-def merge_conv(
-    weight_a: Union[torch.Tensor, nn.Parameter],
-    weight_b: Union[torch.Tensor, nn.Parameter],
-    device = 'cpu'
-):
-    rank, in_ch, kernel_size, k_ = weight_a.shape
-    out_ch, rank_, _, _ = weight_b.shape
-    assert rank == rank_ and kernel_size == k_
-    
-    wa = weight_a.to(device)
-    wb = weight_b.to(device)
-    
-    if device == 'cpu':
-        wa = wa.float()
-        wb = wb.float()
-    
-    merged = wb.reshape(out_ch, -1) @ wa.reshape(rank, -1)
-    weight = merged.reshape(out_ch, in_ch, kernel_size, kernel_size)
-    del wb, wa
-    return weight
-
-
 def extract_linear(
     weight: Union[torch.Tensor, nn.Parameter],
     mode = 'fixed',
     mode_param = 0,
     device = 'cpu',
 ) -> Tuple[nn.Parameter, nn.Parameter]:
     weight = weight.to(device)
@@ -126,35 +104,14 @@
     diff = (weight - U @ Vh).detach()
     extract_weight_A = Vh.reshape(lora_rank, in_ch).detach()
     extract_weight_B = U.reshape(out_ch, lora_rank).detach()
     del U, S, Vh, weight
     return (extract_weight_A, extract_weight_B, diff), 'low rank'
 
 
-def merge_linear(
-    weight_a: Union[torch.Tensor, nn.Parameter],
-    weight_b: Union[torch.Tensor, nn.Parameter],
-    device = 'cpu'
-):
-    rank, in_ch = weight_a.shape
-    out_ch, rank_ = weight_b.shape
-    assert rank == rank_
-    
-    wa = weight_a.to(device)
-    wb = weight_b.to(device)
-    
-    if device == 'cpu':
-        wa = wa.float()
-        wb = wb.float()
-    
-    weight = wb @ wa
-    del wb, wa
-    return weight
-
-
 def extract_diff(
     base_model,
     db_model,
     mode = 'fixed',
     linear_mode_param = 0,
     conv_mode_param = 0,
     extract_device = 'cpu',
@@ -348,159 +305,200 @@
         UNET_TARGET_REPLACE_MODULE,
         UNET_TARGET_REPLACE_NAME
     )
     print(len(text_encoder_loras), len(unet_loras))
     return text_encoder_loras|unet_loras
 
 
-def merge_locon(
-    base_model,
-    locon_state_dict: Dict[str, torch.TensorType],
-    scale: float = 1.0,
-    device = 'cpu'
+def get_module(
+    lyco_state_dict: Dict,
+    lora_name
 ):
-    UNET_TARGET_REPLACE_MODULE = [
-        "Transformer2DModel",
-        "Attention",
-        "ResnetBlock2D",
-        "Downsample2D",
-        "Upsample2D"
-    ]
-    UNET_TARGET_REPLACE_NAME = [
-        "conv_in",
-        "conv_out",
-        "time_embedding.linear_1",
-        "time_embedding.linear_2",
-    ]
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
-    LORA_PREFIX_UNET = 'lora_unet'
-    LORA_PREFIX_TEXT_ENCODER = 'lora_te'
-    def merge(
-        prefix,
-        root_module: torch.nn.Module,
-        target_replace_modules,
-        target_replace_names = []
-    ):
-        temp = {}
-        for name, module in tqdm(list(root_module.named_modules())):
-            if module.__class__.__name__ in target_replace_modules or name in target_replace_names:
-                temp[name] = {}
-                for child_name, child_module in module.named_modules():
-                    layer = child_module.__class__.__name__
-                    if layer not in {'Linear', 'Conv2d'}:
-                        continue
-                    lora_name = prefix + '.' + name
-                    if child_name:
-                        lora_name += '.' + child_name
-                    lora_name = lora_name.replace('.', '_')
-                    lora_diff_name = prefix + '_' + name + ".diff"
+    if f'{lora_name}.lora_up.weight' in lyco_state_dict:
+        up = lyco_state_dict[f'{lora_name}.lora_up.weight']
+        down = lyco_state_dict[f'{lora_name}.lora_down.weight']
+        mid = lyco_state_dict.get(f'{lora_name}.lora_mid.weight', None)
+        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
+        return 'locon', (up, down, mid, alpha)
+    elif f'{lora_name}.hada_w1_a' in lyco_state_dict:
+        w1a = lyco_state_dict[f'{lora_name}.hada_w1_a']
+        w1b = lyco_state_dict[f'{lora_name}.hada_w1_b']
+        w2a = lyco_state_dict[f'{lora_name}.hada_w2_a']
+        w2b = lyco_state_dict[f'{lora_name}.hada_w2_b']
+        t1 = lyco_state_dict.get(f'{lora_name}.hada_t1', None)
+        t2 = lyco_state_dict.get(f'{lora_name}.hada_t2', None)
+        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
+        return 'hada', (w1a, w1b, w2a, w2b, t1, t2, alpha)
+    elif f'{lora_name}.weight' in lyco_state_dict:
+        weight = lyco_state_dict[f'{lora_name}.weight']
+        on_input = lyco_state_dict.get(f'{lora_name}.on_input', False)
+        return 'ia3', (weight, on_input)
+    elif (f'{lora_name}.lokr_w1' in lyco_state_dict
+          or f'{lora_name}.lokr_w1_a' in lyco_state_dict):
+        w1 = lyco_state_dict.get(f'{lora_name}.lokr_w1', None)
+        w1a = lyco_state_dict.get(f'{lora_name}.lokr_w1_a', None)
+        w1b = lyco_state_dict.get(f'{lora_name}.lokr_w1_b', None)
+        w2 = lyco_state_dict.get(f'{lora_name}.lokr_w2', None)
+        w2a = lyco_state_dict.get(f'{lora_name}.lokr_w2_a', None)
+        w2b = lyco_state_dict.get(f'{lora_name}.lokr_w2_b', None)
+        t1 = lyco_state_dict.get(f'{lora_name}.lokr_t1', None)
+        t2 = lyco_state_dict.get(f'{lora_name}.lokr_t2', None)
+        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
+        return 'kron', (w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha)
+    elif f'{lora_name}.diff' in lyco_state_dict:
+        return 'full', lyco_state_dict[f'{lora_name}.diff']
+    else:
+        return 'None', ()
 
-                    if lora_diff_name in locon_state_dict:
-                        child_module.weight.requires_grad_(False)
-                        child_module.weight += locon_state_dict[lora_diff_name].cpu()
-                        continue
 
-                    down_name = f'{lora_name}.lora_down.weight'
-                    up_name = f'{lora_name}.lora_up.weight'
-                    alpha_name = f'{lora_name}.alpha'
-
-                    if (down_name not in locon_state_dict 
-                        or up_name not in locon_state_dict 
-                        or alpha_name not in locon_state_dict):
-                        continue
+def cp_weight_from_conv(
+    up, down, mid
+):
+    up = up.reshape(up.size(0), up.size(1))
+    down = down.reshape(down.size(0), down.size(1))
+    return torch.einsum('m n w h, i m, n j -> i j w h', mid, up, down)
 
-                    down = locon_state_dict[down_name].float()
-                    up = locon_state_dict[up_name].float()
-                    alpha = locon_state_dict[alpha_name].float()
-                    rank = down.shape[0]
-
-                    if layer == 'Conv2d':
-                        if f'{lora_name}.lora_mid.weight' in locon_state_dict:
-                            mid = locon_state_dict[f'{lora_name}.lora_mid.weight'].transpose(0,1).float()
-                            down = merge_conv(mid, down.transpose(0,1), device).transpose(0,1)
-                            delta = merge_conv(down, up, device)
-                        else:
-                            delta = merge_conv(down, up, device)
-                        child_module.weight.requires_grad_(False)
-                        child_module.weight += (alpha.to(device)/rank * scale * delta).cpu()
-                        del delta
-                    elif layer == 'Linear':
-                        delta = merge_linear(down, up, device)
-                        child_module.weight.requires_grad_(False)
-                        child_module.weight += (alpha.to(device)/rank * scale * delta).cpu()
-                        del delta
+def cp_weight(
+    wa, wb, t
+):
+    temp = torch.einsum('i j k l, j r -> i r k l', t, wb)
+    return torch.einsum('i j k l, i r -> r j k l', temp, wa)
 
-    merge(
-        LORA_PREFIX_TEXT_ENCODER,
-        base_model[0], 
-        TEXT_ENCODER_TARGET_REPLACE_MODULE,
-        UNET_TARGET_REPLACE_NAME
-    )
-    merge(
-        LORA_PREFIX_UNET,
-        base_model[2],
-        UNET_TARGET_REPLACE_MODULE,
-        UNET_TARGET_REPLACE_NAME
-    )
+
+@torch.no_grad()
+def rebuild_weight(module_type, params, orig_weight, scale=1):
+    if orig_weight is None:
+        return orig_weight
+    merged = orig_weight
+    if module_type == 'locon':
+        up, down, mid, alpha = params
+        if alpha is not None:
+            scale *= alpha/up.size(1)
+        if mid is not None:
+            rebuild = cp_weight_from_conv(up, down, mid)
+        else:
+            rebuild = up.reshape(up.size(0),-1) @ down.reshape(down.size(0), -1)
+        merged = orig_weight + rebuild.reshape(orig_weight.shape) * scale
+        del up, down, mid, alpha, params, rebuild
+    elif module_type == 'hada':
+        w1a, w1b, w2a, w2b, t1, t2, alpha = params
+        if alpha is not None:
+            scale *= alpha / w1b.size(0)
+        if t1 is not None:
+            rebuild1 = cp_weight(w1a, w1b, t1)
+        else:
+            rebuild1 = w1a @ w1b
+        if t2 is not None:
+            rebuild2 = cp_weight(w2a, w2b, t2)
+        else:
+            rebuild2 = w2a @ w2b
+        rebuild = (rebuild1 * rebuild2).reshape(orig_weight.shape)
+        merged = orig_weight + rebuild * scale
+        del w1a, w1b, w2a, w2b, t1, t2, alpha, params, rebuild, rebuild1, rebuild2
+    elif module_type == 'ia3':
+        weight, on_input = params
+        if not on_input:
+            weight = weight.reshape(-1, 1)
+        merged = orig_weight + weight * orig_weight * scale
+        del weight, on_input, params
+    elif module_type == 'kron':
+        w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha = params
+        if alpha is not None and (w1b is not None or w2b is not None):
+            scale *= alpha / (w1b.size(0) if w1b else w2b.size(0))
+        if w1a is not None and w1b is not None:
+            if t1:
+                w1 = cp_weight(w1a, w1b, t1)
+            else:
+                w1 = w1a @ w1b
+        if w2a is not None and w2b is not None:
+            if t2:
+                w2 = cp_weight(w2a, w2b, t2)
+            else:
+                w2 = w2a @ w2b
+        rebuild = torch.kron(w1, w2).reshape(orig_weight.shape) 
+        merged = orig_weight + rebuild* scale
+        del w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, params, rebuild
+    elif module_type == 'full':
+        rebuild = params.reshape(orig_weight.shape) 
+        merged = orig_weight + rebuild * scale
+        del params, rebuild
+    
+    return merged
 
 
-def merge_loha(
+def merge(
     base_model,
-    loha_state_dict: Dict[str, torch.TensorType],
+    lyco_state_dict,
     scale: float = 1.0,
     device = 'cpu'
 ):
     UNET_TARGET_REPLACE_MODULE = [
         "Transformer2DModel", 
         "Attention", 
         "ResnetBlock2D", 
         "Downsample2D", 
         "Upsample2D"
     ]
+    UNET_TARGET_REPLACE_NAME = [
+        "conv_in",
+        "conv_out",
+        "time_embedding.linear_1",
+        "time_embedding.linear_2",
+    ]
     TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
     LORA_PREFIX_UNET = 'lora_unet'
     LORA_PREFIX_TEXT_ENCODER = 'lora_te'
-    def merge(
+    merged = 0
+    def merge_state_dict(
         prefix, 
         root_module: torch.nn.Module,
-        target_replace_modules
+        lyco_state_dict: Dict[str,torch.Tensor],
+        target_replace_modules,
+        target_replace_names = []
     ):
-        temp = {}
-        
-        for name, module in tqdm(list(root_module.named_modules())):
+        nonlocal merged
+        for name, module in tqdm(list(root_module.named_modules()), desc=f'Merging {prefix}'):
             if module.__class__.__name__ in target_replace_modules:
-                temp[name] = {}
                 for child_name, child_module in module.named_modules():
-                    layer = child_module.__class__.__name__
-                    if layer not in {'Linear', 'Conv2d'}:
+                    if child_module.__class__.__name__ not in {'Linear', 'Conv2d'}:
                         continue
                     lora_name = prefix + '.' + name + '.' + child_name
                     lora_name = lora_name.replace('.', '_')
                     
-                    w1a = loha_state_dict[f'{lora_name}.hada_w1_a'].float().to(device)
-                    w1b = loha_state_dict[f'{lora_name}.hada_w1_b'].float().to(device)
-                    w2a = loha_state_dict[f'{lora_name}.hada_w2_a'].float().to(device)
-                    w2b = loha_state_dict[f'{lora_name}.hada_w2_b'].float().to(device)
-                    alpha = loha_state_dict[f'{lora_name}.alpha'].float().to(device)
-                    dim = w1b.shape[0]
-                    
-                    delta = (w1a @ w1b) * (w2a @ w2b)
-                    delta = delta.reshape(child_module.weight.shape)
+                    result = rebuild_weight(*get_module(
+                        lyco_state_dict, lora_name
+                    ), getattr(child_module, 'weight'), scale)
+                    if result is not None:
+                        merged += 1
+                        child_module.requires_grad_(False)
+                        child_module.weight.copy_(result)
+            elif name in target_replace_names:
+                lora_name = prefix + '.' + name
+                lora_name = lora_name.replace('.', '_')
                     
-                    if layer == 'Conv2d':
-                        child_module.weight.requires_grad_(False)
-                        child_module.weight += (alpha.to(device)/dim * scale * delta).cpu()
-                    elif layer == 'Linear':
-                        child_module.weight.requires_grad_(False)
-                        child_module.weight += (alpha.to(device)/dim * scale * delta).cpu()
-                    del delta
+                result = rebuild_weight(*get_module(
+                    lyco_state_dict, lora_name
+                ), getattr(module, 'weight'), scale)
+                if result is not None:
+                    merged += 1
+                    module.requires_grad_(False)
+                    module.weight.copy_(result)
     
-    merge(
-        LORA_PREFIX_TEXT_ENCODER, 
-        base_model[0], 
-        TEXT_ENCODER_TARGET_REPLACE_MODULE
+    if device == 'cpu':
+        for k, v in tqdm(list(lyco_state_dict.items()), desc='Converting Dtype'):
+            lyco_state_dict[k] = v.float()
+    
+    merge_state_dict(
+        LORA_PREFIX_TEXT_ENCODER,
+        base_model[0],
+        lyco_state_dict,
+        TEXT_ENCODER_TARGET_REPLACE_MODULE,
+        UNET_TARGET_REPLACE_NAME
     )
-    merge(
+    merge_state_dict(
         LORA_PREFIX_UNET,
-        base_model[2], 
-        UNET_TARGET_REPLACE_MODULE
-    )
+        base_model[2],
+        lyco_state_dict,
+        UNET_TARGET_REPLACE_MODULE,
+        UNET_TARGET_REPLACE_NAME
+    )
+    print(f'{merged} Modules been merged')
```

### Comparing `lycoris_lora-0.1.5.dev4/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 experiments/concept_neuron.py
 experiments/locon_extract_test.py
 experiments/locon_merge_test.py
 experiments/singular_value_test.py
 experiments/sparse_bias_test.py
 experiments/time_test.py
 lycoris/__init__.py
+lycoris/dylora.py
 lycoris/ia3.py
 lycoris/kohya.py
 lycoris/kohya_model_utils.py
 lycoris/kohya_utils.py
 lycoris/locon.py
 lycoris/loha.py
 lycoris/lokr.py
```

### Comparing `lycoris_lora-0.1.5.dev4/setup.py` & `lycoris_lora-0.1.5.dev5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.5-dev4',
+    version='0.1.5-dev5',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.5.dev4/tools/extract_locon.py` & `lycoris_lora-0.1.5.dev5/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev4/tools/merge.py` & `lycoris_lora-0.1.5.dev5/tools/merge.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "--weight", help='weight for the lyco model to merge',
         default='1.0', type=float
     )
     return parser.parse_args()
 ARGS = get_args()
 
 
-from lycoris.utils import merge_loha, merge_locon
+from lycoris.utils import merge
 from lycoris.kohya_model_utils import (
     load_models_from_stable_diffusion_checkpoint,
     save_stable_diffusion_checkpoint,
     load_file
 )
 
 import torch
@@ -50,51 +50,32 @@
 def main():
     base = load_models_from_stable_diffusion_checkpoint(ARGS.is_v2, ARGS.base_model)
     if ARGS.lycoris_model.rsplit('.', 1)[-1] == 'safetensors':
         lyco = load_file(ARGS.lycoris_model)
     else:
         lyco = torch.load(ARGS.lycoris_model)
     
-    algo = None
-    for key in lyco:
-        if 'hada' in key:
-            algo = 'loha'
-            break
-        elif 'lora_up' in key:
-            algo = 'lora'
-            break
-    else:
-        raise NotImplementedError('Cannot find the algo for this lycoris model file.')
-    
     dtype_str = ARGS.dtype.replace('fp', 'float').replace('bf', 'bfloat')
     dtype = {
         'float': torch.float,
         'float16': torch.float16,
         'float32': torch.float32,
         'float64': torch.float64,
         'bfloat': torch.bfloat16,
         'bfloat16': torch.bfloat16,
     }.get(dtype_str, None)
     if dtype is None:
         raise ValueError(f'Cannot Find the dtype "{dtype}"')
     
-    if algo == 'loha':
-        merge_loha(
-            base,
-            lyco,
-            ARGS.weight,
-            ARGS.device
-        )
-    elif algo == 'lora':
-        merge_locon(
-            base,
-            lyco,
-            ARGS.weight,
-            ARGS.device
-        )
+    merge(
+        base,
+        lyco,
+        ARGS.weight,
+        ARGS.device
+    )
     
     save_stable_diffusion_checkpoint(
         ARGS.is_v2, ARGS.output_name, 
         base[0], base[2], 
         None, 0, 0, dtype, 
         base[1]
     )
```

