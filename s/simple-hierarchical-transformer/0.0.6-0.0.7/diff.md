# Comparing `tmp/simple-hierarchical-transformer-0.0.6.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.6.tar", last modified: Tue Apr 11 19:33:34 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.7.tar", last modified: Tue Apr 11 19:36:07 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.6.tar` & `simple-hierarchical-transformer-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-11 19:33:21.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:33:34.708804 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 19:33:34.000000 simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:36:07.599089 simple-hierarchical-transformer-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:36:07.595089 simple-hierarchical-transformer-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:36:07.599089 simple-hierarchical-transformer-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:36:07.595089 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:36:07.595089 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.6/LICENSE` & `simple-hierarchical-transformer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.6/PKG-INFO` & `simple-hierarchical-transformer-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.6/README.md` & `simple-hierarchical-transformer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.6/setup.py` & `simple-hierarchical-transformer-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
```

### Comparing `simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,18 +432,19 @@
         should_compress = c > 1
 
         # if training, predict next token in sequence
 
         if return_loss:
             ids, labels = ids[:, :-1], ids[:, 1:]
 
+        seq_len = ids.shape[-1]
+
         # get token embeddings, and pad to multiple of compression factor
 
         x = self.token_emb(ids)
-        x, orig_seq_len = pad_seq_to_multiple(x, c)
 
         # post embedding norm
 
         x = self.post_token_emb_norm(x)
 
         # compress to hierarchical tokens from the beginning
 
@@ -478,15 +479,15 @@
 
         recon_loss = torch.zeros((), device = self.device)
         if should_compress:
             recon_logits = self.to_recon(h)
             recon_logits = rearrange(recon_logits, 'b n (c d) -> (b c) d n', c = c)
 
             recon_ids = F.pad(ids, (c - 1, 0), value = 0)
-            recon_ids = tuple(recon_ids[:, i:(orig_seq_len + i)] for i in range(c))
+            recon_ids = tuple(recon_ids[:, i:(seq_len + i)] for i in range(c))
             recon_ids = torch.stack(recon_ids, dim = 1)
             recon_ids = rearrange(recon_ids, 'b c n -> (b c) n')
             recon_loss = ce(recon_logits, recon_ids)
 
         logits = rearrange(logits, 'b n c -> b c n')
         ce_loss = ce(logits, labels)
```

### Comparing `simple-hierarchical-transformer-0.0.6/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

