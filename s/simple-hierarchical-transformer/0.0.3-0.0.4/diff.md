# Comparing `tmp/simple-hierarchical-transformer-0.0.3.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.3.tar", last modified: Tue Apr 11 15:29:15 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.4.tar", last modified: Tue Apr 11 15:54:14 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.3.tar` & `simple-hierarchical-transformer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:29:15.905244 simple-hierarchical-transformer-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:29:15.901244 simple-hierarchical-transformer-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:29:15.905244 simple-hierarchical-transformer-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:29:15.901244 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:29:15.901244 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-11 15:54:03.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:54:14.816915 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 15:54:14.000000 simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.3/LICENSE` & `simple-hierarchical-transformer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.3/PKG-INFO` & `simple-hierarchical-transformer-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.3/setup.py` & `simple-hierarchical-transformer-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
```

### Comparing `simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
         ce = partial(F.cross_entropy, ignore_index = self.ignore_index)
 
         # reconstruction losses for hierarchy tokens -> may remove if see no benefit, which seems to be leaning that way
 
         recon_loss = torch.zeros((), device = self.device)
         if should_compress:
-            recon_logits = self.to_recon(x)
+            recon_logits = self.to_recon(h)
             recon_logits = rearrange(recon_logits, 'b n (c d) -> (b c) d n', c = c)
 
             recon_ids = F.pad(ids, (c - 1, 0), value = 0)
             recon_ids = tuple(recon_ids[:, i:(orig_seq_len + i)] for i in range(c))
             recon_ids = torch.stack(recon_ids, dim = 1)
             recon_ids = rearrange(recon_ids, 'b c n -> (b c) n')
             recon_loss = ce(recon_logits, recon_ids)
```

### Comparing `simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.4/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

