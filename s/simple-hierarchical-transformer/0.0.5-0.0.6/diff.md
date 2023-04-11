# Comparing `tmp/simple-hierarchical-transformer-0.0.5.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.5.tar", last modified: Tue Apr 11 18:21:31 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.6.tar", last modified: Tue Apr 11 19:33:34 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.5.tar` & `simple-hierarchical-transformer-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-11 18:21:15.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:21:31.607104 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 18:21:31.000000 simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.5/LICENSE` & `simple-hierarchical-transformer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.5/PKG-INFO` & `simple-hierarchical-transformer-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.5/README.md` & `simple-hierarchical-transformer-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 
 Update: I think it is working 🤞 
 
 ## Todo
 
 - [x] branch out to two parallel paths, one for hierarchical tokens, other for plain fine tokens.
 - [x] show that local attention in fine + hierarchical tokens can come close to full attention baseline
+- [x] simple dsconv seems enough to merge for 1 hierarchy
 
-- [ ] try naive projection + GLU for extracting information from hierarchical tokens to fine
 - [ ] try a few types of attention across hierarchies. full self attention, directional, or even token shift and feedforward
 - [ ] fully customizable dimensions across hierarchies, as higher hierarchies require greater model dimensions
 - [ ] play around with an autoregressive loss on the hierarchy tokens, using a sigmoid contrastive loss from recent brain paper - can also try random projections + vq, as was done in universal speech model paper, also from brain
 - [ ] allow for repeating hierarchy tokens for fine tokens in the future, as position may matter less as one goes up the hierarchy. but not a priority, get things working first
 - [ ] make feedforward efficient too with <a href="https://github.com/lucidrains/CoLT5-attention">routing</a>
 - [ ] auto-set window size to be half of max sequence length for fine and all hierarchies
 - [ ] build out simple local attention block, for use across all hierarchies
 - [ ] add flash attention to local attention library
+- [ ] figure out if attention can be shared across hierarchies
+- [ ] add prophet losses for hierarchical tokens
+- [ ] figure out effects of just pooling all fine + hierarchical tokens before cross entropy loss
 
 ## Appreciation
 
 - <a href="https://stability.ai/">StabilityAI</a> for the sponsorship to carry out this independent research
 
 - <a href="https://huggingface.co/">🤗 Huggingface</a> for their accelerate library
```

#### html2text {}

```diff
@@ -4,28 +4,30 @@
 bedrocks of simple ideas. Worth a shot. So far, the idea has passed the litmus
 test from a research friend. Will bring it to completion in the next week or
 so. If it does not work out, I'll leave the negative experimental results as
 well as the repository around, and maybe some PhD student can build upon it.
 Ongoing_experiments Update: I think it is working ð¤ ## Todo - [x] branch out
 to two parallel paths, one for hierarchical tokens, other for plain fine
 tokens. - [x] show that local attention in fine + hierarchical tokens can come
-close to full attention baseline - [ ] try naive projection + GLU for
-extracting information from hierarchical tokens to fine - [ ] try a few types
-of attention across hierarchies. full self attention, directional, or even
-token shift and feedforward - [ ] fully customizable dimensions across
-hierarchies, as higher hierarchies require greater model dimensions - [ ] play
-around with an autoregressive loss on the hierarchy tokens, using a sigmoid
-contrastive loss from recent brain paper - can also try random projections +
-vq, as was done in universal speech model paper, also from brain - [ ] allow
-for repeating hierarchy tokens for fine tokens in the future, as position may
-matter less as one goes up the hierarchy. but not a priority, get things
-working first - [ ] make feedforward efficient too with routing - [ ] auto-set
-window size to be half of max sequence length for fine and all hierarchies -
-[ ] build out simple local attention block, for use across all hierarchies -
-[ ] add flash attention to local attention library ## Appreciation -
+close to full attention baseline - [x] simple dsconv seems enough to merge for
+1 hierarchy - [ ] try a few types of attention across hierarchies. full self
+attention, directional, or even token shift and feedforward - [ ] fully
+customizable dimensions across hierarchies, as higher hierarchies require
+greater model dimensions - [ ] play around with an autoregressive loss on the
+hierarchy tokens, using a sigmoid contrastive loss from recent brain paper -
+can also try random projections + vq, as was done in universal speech model
+paper, also from brain - [ ] allow for repeating hierarchy tokens for fine
+tokens in the future, as position may matter less as one goes up the hierarchy.
+but not a priority, get things working first - [ ] make feedforward efficient
+too with routing - [ ] auto-set window size to be half of max sequence length
+for fine and all hierarchies - [ ] build out simple local attention block, for
+use across all hierarchies - [ ] add flash attention to local attention library
+- [ ] figure out if attention can be shared across hierarchies - [ ] add
+prophet losses for hierarchical tokens - [ ] figure out effects of just pooling
+all fine + hierarchical tokens before cross entropy loss ## Appreciation -
 StabilityAI for the sponsorship to carry out this independent research - ð¤
 Huggingface for their accelerate library ## Citations Closest idea would be
 hourglass_transformers. And my renewed interest in hierarchical approaches came
 from reading this. ```bibtex @article{Nawrot2021HierarchicalTA, title =
 {Hierarchical Transformers Are More Efficient Language Models}, author = {Piotr
 Nawrot and Szymon Tworkowski and Michal Tyrolski and Lukasz Kaiser and Yuhuai
 Wu and Christian Szegedy and Henryk Michalewski}, journal = {ArXiv}, year =
```

### Comparing `simple-hierarchical-transformer-0.0.5/setup.py` & `simple-hierarchical-transformer-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
```

### Comparing `simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,14 +283,52 @@
             q, k = apply_rotary_pos_emb_qk(rotary_emb, q, k)
 
         out = self.attend(q, k, v)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
+class HierarchicalAttention(nn.Module):
+    def __init__(
+        self,
+        dim,
+        dim_head = 64,
+        heads = 8,
+        window_size = None,
+        compress_factor = 2
+    ):
+        super().__init__()
+        assert compress_factor > 1 and is_power_of_two(compress_factor)
+        self.compress_factor = compress_factor
+
+        attn_klass = Attention
+        if exists(window_size):
+            attn_klass = partial(LocalMHA, window_size = window_size, causal = True, prenorm = True)
+
+        self.attn = attn_klass(dim = dim, dim_head = dim_head, heads = heads)
+
+    def forward(self, x):
+        c = self.compress_factor
+        x, orig_seq_len = pad_seq_to_multiple(x, c)
+
+        # hierarchical attention is performed with a simple axial attention
+
+        # this, and using a convolution for compressing at the beginning
+        # is one of the improvements on top of hourglass transformer
+        # the downside is that the savings are only O(c) instead of O(c ** 2)
+        # but this should provide better learning per-token
+
+        x = rearrange(x, 'b (n c) d -> (b c) n d', c = c)
+
+        x = self.attn(x)
+
+        x = rearrange(x, '(b c) n d -> b (n c) d', c = c)
+
+        return x[:, :orig_seq_len]
+
 class HierarchicalTransformer(nn.Module):
     def __init__(
         self,
         *,
         num_tokens,
         dim,
         depth,
@@ -331,15 +369,15 @@
         self.layers = mlist([])
 
         local_attn = partial(LocalMHA, causal = True, prenorm = True)
 
         for _ in range(depth):
 
             self.layers.append(mlist([
-                local_attn(dim = dim, dim_head = dim_head, heads = heads, window_size = hierarchical_window_size),
+                HierarchicalAttention(dim = dim, dim_head = dim_head, heads = heads, window_size = hierarchical_window_size, compress_factor = compress_factor),
                 FeedForward(dim = dim, mult = ff_mult),
                 local_attn(dim = dim, dim_head = dim_head, heads = heads, window_size = fine_window_size),
                 FeedForward(dim = dim, mult = ff_mult),
                 HierarchicalMerge(dim = dim)
             ]))
 
         self.norm = RMSNorm(dim)
@@ -413,34 +451,22 @@
         if exists(self.compress):
             h, uncompressed = self.compress(x)
 
         # layers
 
         for h_local_attn, h_ff, local_attn, ff, h_merge in self.layers:
 
-            if should_compress:
-                h = rearrange(h, 'b (n c) d -> (b c) n d', c = c)
-
             h = h_local_attn(h) + h
-
-            if should_compress:
-                h = rearrange(h, '(b c) n d -> b (n c) d', c = c)
-
             h = h_ff(token_shift(h)) + h
 
             x = local_attn(x) + x
             x = ff(token_shift(x)) + x
 
             x = h_merge(x, h) + x
 
-        # get back the original sequence length
-
-        x = x[:, :orig_seq_len]
-        h = h[:, :orig_seq_len]
-
         # final norm and logits
 
         x = self.norm(x)
 
         logits = self.to_logits(x)
 
         if not return_loss:
```

### Comparing `simple-hierarchical-transformer-0.0.5/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

