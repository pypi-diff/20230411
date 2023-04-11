# Comparing `tmp/simple-hierarchical-transformer-0.0.4.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.4.tar", last modified: Tue Apr 11 15:54:14 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.5.tar", last modified: Tue Apr 11 18:21:31 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.4.tar` & `simple-hierarchical-transformer-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.4/LICENSE` & `simple-hierarchical-transformer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.4/PKG-INFO` & `simple-hierarchical-transformer-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.4/README.md` & `simple-hierarchical-transformer-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,26 @@
 
 <a href="https://api.wandb.ai/links/lucidrains/w8vdkz75">Ongoing experiments</a>
 
 Update: I think it is working 🤞 
 
 ## Todo
 
-- [ ] branch out to two parallel paths, one for hierarchical tokens, other for plain fine tokens.
-- [ ] build out simple local attention block, for use across all hierarchies
-- [ ] show that local attention in fine + hierarchical tokens can come close to full attention baseline
+- [x] branch out to two parallel paths, one for hierarchical tokens, other for plain fine tokens.
+- [x] show that local attention in fine + hierarchical tokens can come close to full attention baseline
+
 - [ ] try naive projection + GLU for extracting information from hierarchical tokens to fine
 - [ ] try a few types of attention across hierarchies. full self attention, directional, or even token shift and feedforward
 - [ ] fully customizable dimensions across hierarchies, as higher hierarchies require greater model dimensions
 - [ ] play around with an autoregressive loss on the hierarchy tokens, using a sigmoid contrastive loss from recent brain paper - can also try random projections + vq, as was done in universal speech model paper, also from brain
+- [ ] allow for repeating hierarchy tokens for fine tokens in the future, as position may matter less as one goes up the hierarchy. but not a priority, get things working first
+- [ ] make feedforward efficient too with <a href="https://github.com/lucidrains/CoLT5-attention">routing</a>
+- [ ] auto-set window size to be half of max sequence length for fine and all hierarchies
+- [ ] build out simple local attention block, for use across all hierarchies
+- [ ] add flash attention to local attention library
 
 ## Appreciation
 
 - <a href="https://stability.ai/">StabilityAI</a> for the sponsorship to carry out this independent research
 
 - <a href="https://huggingface.co/">🤗 Huggingface</a> for their accelerate library
```

#### html2text {}

```diff
@@ -1,34 +1,39 @@
 ## Simple Hierarchical Transformer (wip) Experiments around a simple idea for
 inducing multiple hierarchical predictive coding models within a GPT. It is so
 simple, it may not work. But then again, deep learning progress is built on the
 bedrocks of simple ideas. Worth a shot. So far, the idea has passed the litmus
 test from a research friend. Will bring it to completion in the next week or
 so. If it does not work out, I'll leave the negative experimental results as
 well as the repository around, and maybe some PhD student can build upon it.
-Ongoing_experiments Update: I think it is working ð¤ ## Todo - [ ] branch out
+Ongoing_experiments Update: I think it is working ð¤ ## Todo - [x] branch out
 to two parallel paths, one for hierarchical tokens, other for plain fine
-tokens. - [ ] build out simple local attention block, for use across all
-hierarchies - [ ] show that local attention in fine + hierarchical tokens can
-come close to full attention baseline - [ ] try naive projection + GLU for
+tokens. - [x] show that local attention in fine + hierarchical tokens can come
+close to full attention baseline - [ ] try naive projection + GLU for
 extracting information from hierarchical tokens to fine - [ ] try a few types
 of attention across hierarchies. full self attention, directional, or even
 token shift and feedforward - [ ] fully customizable dimensions across
 hierarchies, as higher hierarchies require greater model dimensions - [ ] play
 around with an autoregressive loss on the hierarchy tokens, using a sigmoid
 contrastive loss from recent brain paper - can also try random projections +
-vq, as was done in universal speech model paper, also from brain ##
-Appreciation - StabilityAI for the sponsorship to carry out this independent
-research - ð¤_Huggingface for their accelerate library ## Citations Closest
-idea would be hourglass_transformers. And my renewed interest in hierarchical
-approaches came from reading this. ```bibtex @article{Nawrot2021HierarchicalTA,
-title = {Hierarchical Transformers Are More Efficient Language Models}, author
-= {Piotr Nawrot and Szymon Tworkowski and Michal Tyrolski and Lukasz Kaiser and
-Yuhuai Wu and Christian Szegedy and Henryk Michalewski}, journal = {ArXiv},
-year = {2021}, volume = {abs/2110.13711} } ``` ```bibtex @inproceedings
+vq, as was done in universal speech model paper, also from brain - [ ] allow
+for repeating hierarchy tokens for fine tokens in the future, as position may
+matter less as one goes up the hierarchy. but not a priority, get things
+working first - [ ] make feedforward efficient too with routing - [ ] auto-set
+window size to be half of max sequence length for fine and all hierarchies -
+[ ] build out simple local attention block, for use across all hierarchies -
+[ ] add flash attention to local attention library ## Appreciation -
+StabilityAI for the sponsorship to carry out this independent research - ð¤
+Huggingface for their accelerate library ## Citations Closest idea would be
+hourglass_transformers. And my renewed interest in hierarchical approaches came
+from reading this. ```bibtex @article{Nawrot2021HierarchicalTA, title =
+{Hierarchical Transformers Are More Efficient Language Models}, author = {Piotr
+Nawrot and Szymon Tworkowski and Michal Tyrolski and Lukasz Kaiser and Yuhuai
+Wu and Christian Szegedy and Henryk Michalewski}, journal = {ArXiv}, year =
+{2021}, volume = {abs/2110.13711} } ``` ```bibtex @inproceedings
 {dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
 Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
 Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
 in Neural Information Processing Systems}, year = {2022} } ``` ```bibtex
 @article{Yan2020ProphetNetPF, title = {ProphetNet: Predicting Future N-gram for
 Sequence-to-Sequence Pre-training}, author = {Yu Yan and Weizhen Qi and Yeyun
 Gong and Dayiheng Liu and Nan Duan and Jiusheng Chen and Ruofei Zhang and Ming
```

### Comparing `simple-hierarchical-transformer-0.0.4/setup.py` & `simple-hierarchical-transformer-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
@@ -16,14 +16,15 @@
     'transformers',
     'attention mechanism',
     'hierarchical'
   ],
   install_requires=[
     'accelerate',
     'einops>=0.4',
+    'local-attention',
     'torch>=1.6',
     'vector-quantize-pytorch'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

### Comparing `simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from torch import nn, einsum
 
 from einops import rearrange, repeat
 from einops.layers.torch import Rearrange
 
 from simple_hierarchical_transformer.attention import Attend
 
+from local_attention import LocalMHA
+
 # constants
 
 mlist = nn.ModuleList
 
 Linear = partial(nn.Linear, bias = False)
 
 # helper functions
@@ -98,14 +100,20 @@
         return freqs, scale
 
 def rotate_half(x):
     x1, x2 = x.chunk(2, dim=-1)
     return torch.cat((-x2, x1), dim=-1)
 
 def apply_rotary_pos_emb(pos, t, scale = 1.):
+    seq_len = t.shape[-2]
+
+    pos = pos[..., -seq_len:, :]
+    if not isinstance(scale, (int, float)):
+        scale = scale[..., -seq_len:, :]
+
     return (t * pos.cos() * scale) + (rotate_half(t) * pos.sin() * scale)
 
 def apply_rotary_pos_emb_qk(rotary_emb, q, k):
     freqs, scale = rotary_emb
     q = apply_rotary_pos_emb(freqs, q, scale)
     k = apply_rotary_pos_emb(freqs, k, scale ** -1)
     return q, k
@@ -176,14 +184,48 @@
         x = rearrange(x, 'b n d -> b d n 1')
         x = F.pad(x, (0, 0, factor - 1, 0), value = 0.)
         unfolded = F.unfold(x, (factor, 1))
         unfolded = rearrange(unfolded, 'b (d c) n -> (b n) c d', c = factor)
 
         return pooled, unfolded
 
+class HierarchicalMerge(nn.Module):
+    def __init__(
+        self,
+        dim,
+        num_hierarchies = 2 # 2 for now
+    ):
+        super().__init__()
+        self.norm = RMSNorm(dim)
+        self.h_norm = RMSNorm(dim)
+
+        # simple dsconv for now
+
+        self.num_hierarchies = num_hierarchies
+
+        self.conv = nn.Conv1d(dim, dim, num_hierarchies, stride = num_hierarchies, groups = dim)
+
+    def forward(self, x, h):
+        """
+        einops notations:
+        b - batch
+        h - hierarchies
+        n - sequence length
+        d - dimension
+        """
+        nh = self.num_hierarchies
+
+        x = self.norm(x)
+        h = self.h_norm(h)
+
+        x = rearrange([x, h], 'h b n d -> b d (n h)')
+        x = self.conv(x)
+        x = rearrange(x, 'b d n -> b n d')
+        return x
+
 # classes
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.scale = dim ** 0.5
         self.gamma = nn.Parameter(torch.ones(dim))
@@ -255,24 +297,28 @@
         seq_len = 2048,
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
         use_flash_attn = False,
         ignore_index = 0,
         compress_factor = 1,
-        recon_loss_weight = 0.1
+        recon_loss_weight = 0.1,
+        hierarchical_window_size = 64,
+        fine_window_size = 64
     ):
         super().__init__()
         assert is_power_of_two(compress_factor)
 
         self.seq_len = seq_len
         self.ignore_index = ignore_index
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
+        self.post_token_emb_norm = RMSNorm(dim)
+
         should_compress = compress_factor > 1
 
         self.compress_factor = compress_factor
         self.compress = None
 
         if should_compress:
             self.compress = Compress(
@@ -280,20 +326,24 @@
                 compress_factor = compress_factor
             )
 
         self.recon_loss_weight = recon_loss_weight
 
         self.layers = mlist([])
 
-        self.rotary_emb = RotaryEmbedding(dim_head)
+        local_attn = partial(LocalMHA, causal = True, prenorm = True)
 
         for _ in range(depth):
+
             self.layers.append(mlist([
-                Attention(dim = dim, dim_head = dim_head, heads = heads, use_flash_attn = use_flash_attn),
-                FeedForward(dim = dim, mult = ff_mult)
+                local_attn(dim = dim, dim_head = dim_head, heads = heads, window_size = hierarchical_window_size),
+                FeedForward(dim = dim, mult = ff_mult),
+                local_attn(dim = dim, dim_head = dim_head, heads = heads, window_size = fine_window_size),
+                FeedForward(dim = dim, mult = ff_mult),
+                HierarchicalMerge(dim = dim)
             ]))
 
         self.norm = RMSNorm(dim)
 
         self.to_logits = Linear(dim, num_tokens)
         self.to_recon = Linear(dim, compress_factor * num_tokens) if should_compress else None
 
@@ -349,46 +399,53 @@
             ids, labels = ids[:, :-1], ids[:, 1:]
 
         # get token embeddings, and pad to multiple of compression factor
 
         x = self.token_emb(ids)
         x, orig_seq_len = pad_seq_to_multiple(x, c)
 
+        # post embedding norm
+
+        x = self.post_token_emb_norm(x)
+
         # compress to hierarchical tokens from the beginning
 
         h = x
         if exists(self.compress):
             h, uncompressed = self.compress(x)
 
-        # rotary positional embeddings
-
-        pos_emb = self.rotary_emb(h.shape[-2] // c)
-
         # layers
 
-        for attn, ff in self.layers:
+        for h_local_attn, h_ff, local_attn, ff, h_merge in self.layers:
+
             if should_compress:
                 h = rearrange(h, 'b (n c) d -> (b c) n d', c = c)
 
-            h = attn(h, rotary_emb = pos_emb) + h
+            h = h_local_attn(h) + h
 
             if should_compress:
                 h = rearrange(h, '(b c) n d -> b (n c) d', c = c)
 
-            h = ff(token_shift(h)) + h
+            h = h_ff(token_shift(h)) + h
+
+            x = local_attn(x) + x
+            x = ff(token_shift(x)) + x
+
+            x = h_merge(x, h) + x
 
         # get back the original sequence length
 
+        x = x[:, :orig_seq_len]
         h = h[:, :orig_seq_len]
 
         # final norm and logits
 
-        h = self.norm(h)
+        x = self.norm(x)
 
-        logits = self.to_logits(h)
+        logits = self.to_logits(x)
 
         if not return_loss:
             return logits
 
         ce = partial(F.cross_entropy, ignore_index = self.ignore_index)
 
         # reconstruction losses for hierarchy tokens -> may remove if see no benefit, which seems to be leaning that way
```

### Comparing `simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

