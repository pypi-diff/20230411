# Comparing `tmp/simple-hierarchical-transformer-0.0.2.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.2.tar", last modified: Mon Apr 10 15:14:51 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.3.tar", last modified: Tue Apr 11 15:29:15 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.2.tar` & `simple-hierarchical-transformer-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:14:51.245723 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-10 15:14:42.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:14:51.249723 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 15:14:51.000000 simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:29:15.905244 simple-hierarchical-transformer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:29:15.901244 simple-hierarchical-transformer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:29:15.905244 simple-hierarchical-transformer-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:29:15.901244 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-11 15:29:05.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:29:15.901244 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 15:29:15.000000 simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.2/LICENSE` & `simple-hierarchical-transformer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.2/PKG-INFO` & `simple-hierarchical-transformer-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.2/README.md` & `simple-hierarchical-transformer-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ## Simple Hierarchical Transformer (wip)
 
 Experiments around a simple idea for inducing multiple hierarchical predictive coding models within a GPT. It is so simple, it may not work. But then again, deep learning progress is built on the bedrocks of simple ideas. Worth a shot.
 
 So far, the idea has passed the litmus test from a research friend. Will bring it to completion in the next week or so. If it does not work out, I'll leave the negative experimental results as well as the repository around, and maybe some PhD student can build upon it.
 
+<a href="https://api.wandb.ai/links/lucidrains/w8vdkz75">Ongoing experiments</a>
+
+Update: I think it is working 🤞 
+
 ## Appreciation
 
 - <a href="https://stability.ai/">StabilityAI</a> for the sponsorship to carry out this independent research
 
 - <a href="https://huggingface.co/">🤗 Huggingface</a> for their accelerate library
 
 ## Citations
@@ -59,7 +63,20 @@
 ```bibtex
 @inproceedings{Sun2022ALT,
     title     = {A Length-Extrapolatable Transformer},
     author    = {Yutao Sun and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary and Xia Song and Furu Wei},
     year      = {2022}
 }
 ```
+
+```bibtex
+@software{peng_bo_2021_5196578,
+    author       = {PENG Bo},
+    title        = {BlinkDL/RWKV-LM: 0.01},
+    month        = {aug},
+    year         = {2021},
+    publisher    = {Zenodo},
+    version      = {0.01},
+    doi          = {10.5281/zenodo.5196578},
+    url          = {https://doi.org/10.5281/zenodo.5196578}
+}
+```
```

#### html2text {}

```diff
@@ -1,30 +1,35 @@
 ## Simple Hierarchical Transformer (wip) Experiments around a simple idea for
 inducing multiple hierarchical predictive coding models within a GPT. It is so
 simple, it may not work. But then again, deep learning progress is built on the
 bedrocks of simple ideas. Worth a shot. So far, the idea has passed the litmus
 test from a research friend. Will bring it to completion in the next week or
 so. If it does not work out, I'll leave the negative experimental results as
-well as the repository around, and maybe some PhD student can build upon it. ##
-Appreciation - StabilityAI for the sponsorship to carry out this independent
-research - ð¤_Huggingface for their accelerate library ## Citations Closest
-idea would be hourglass_transformers. And my renewed interest in hierarchical
-approaches came from reading this. ```bibtex @article{Nawrot2021HierarchicalTA,
-title = {Hierarchical Transformers Are More Efficient Language Models}, author
-= {Piotr Nawrot and Szymon Tworkowski and Michal Tyrolski and Lukasz Kaiser and
-Yuhuai Wu and Christian Szegedy and Henryk Michalewski}, journal = {ArXiv},
-year = {2021}, volume = {abs/2110.13711} } ``` ```bibtex @inproceedings
+well as the repository around, and maybe some PhD student can build upon it.
+Ongoing_experiments Update: I think it is working ð¤ ## Appreciation -
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
 Zhou}, journal = {ArXiv}, year = {2020}, volume = {abs/2001.04063} } ```
 ```bibtex @misc{su2021roformer, title = {RoFormer: Enhanced Transformer with
 Rotary Position Embedding}, author = {Jianlin Su and Yu Lu and Shengfeng Pan
 and Bo Wen and Yunfeng Liu}, year = {2021}, eprint = {2104.09864},
 archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @inproceedings
 {Sun2022ALT, title = {A Length-Extrapolatable Transformer}, author = {Yutao Sun
 and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim
-and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ```
+and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex
+@software{peng_bo_2021_5196578, author = {PENG Bo}, title = {BlinkDL/RWKV-LM:
+0.01}, month = {aug}, year = {2021}, publisher = {Zenodo}, version = {0.01},
+doi = {10.5281/zenodo.5196578}, url = {https://doi.org/10.5281/zenodo.5196578}
+} ```
```

### Comparing `simple-hierarchical-transformer-0.0.2/setup.py` & `simple-hierarchical-transformer-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
```

### Comparing `simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.2/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.3/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

