# Comparing `tmp/capsa-0.1.4.tar.gz` & `tmp/capsa-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/capsa-0.1.4.tar", last modified: Thu Feb 16 17:35:28 2023, max compression
+gzip compressed data, was "dist/capsa-0.1.5.tar", last modified: Tue Apr 11 03:44:33 2023, max compression
```

## Comparing `capsa-0.1.4.tar` & `capsa-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/
--rw-r--r--   0 amini      (501) staff       (20)    34523 2022-12-09 05:37:26.000000 capsa-0.1.4/LICENSE
--rw-r--r--   0 amini      (501) staff       (20)     4973 2023-02-16 17:35:28.000000 capsa-0.1.4/PKG-INFO
--rw-r--r--   0 amini      (501) staff       (20)     4441 2023-01-11 04:49:10.000000 capsa-0.1.4/README.md
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa/
--rw-r--r--   0 amini      (501) staff       (20)      268 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/__init__.py
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa/aleatoric/
--rw-r--r--   0 amini      (501) staff       (20)       27 2022-12-09 05:37:26.000000 capsa-0.1.4/capsa/aleatoric/__init__.py
--rw-r--r--   0 amini      (501) staff       (20)     4619 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/aleatoric/mve.py
--rw-r--r--   0 amini      (501) staff       (20)     7761 2023-02-16 17:34:45.000000 capsa-0.1.4/capsa/base_wrapper.py
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa/bias/
--rw-r--r--   0 amini      (501) staff       (20)       85 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/bias/__init__.py
--rw-r--r--   0 amini      (501) staff       (20)     7553 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/bias/histogram.py
--rw-r--r--   0 amini      (501) staff       (20)    17393 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/bias/histogramvae.py
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa/epistemic/
--rw-r--r--   0 amini      (501) staff       (20)      102 2022-12-09 05:37:26.000000 capsa-0.1.4/capsa/epistemic/__init__.py
--rw-r--r--   0 amini      (501) staff       (20)     5532 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/epistemic/dropout.py
--rw-r--r--   0 amini      (501) staff       (20)     9373 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/epistemic/ensemble.py
--rw-r--r--   0 amini      (501) staff       (20)    10368 2023-01-11 04:49:10.000000 capsa-0.1.4/capsa/epistemic/vae.py
--rw-r--r--   0 amini      (501) staff       (20)    38773 2022-12-09 05:37:26.000000 capsa-0.1.4/capsa/risk_tensor.py
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa/utils/
--rw-r--r--   0 amini      (501) staff       (20)      269 2023-02-16 17:34:45.000000 capsa-0.1.4/capsa/utils/__init__.py
--rw-r--r--   0 amini      (501) staff       (20)     6609 2023-02-16 17:34:45.000000 capsa-0.1.4/capsa/utils/utils.py
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa.egg-info/
--rw-r--r--   0 amini      (501) staff       (20)     4973 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa.egg-info/PKG-INFO
--rw-r--r--   0 amini      (501) staff       (20)      679 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa.egg-info/SOURCES.txt
--rw-r--r--   0 amini      (501) staff       (20)        1 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa.egg-info/dependency_links.txt
--rw-r--r--   0 amini      (501) staff       (20)        1 2022-12-09 05:57:09.000000 capsa-0.1.4/capsa.egg-info/not-zip-safe
--rw-r--r--   0 amini      (501) staff       (20)        6 2023-02-16 17:35:28.000000 capsa-0.1.4/capsa.egg-info/top_level.txt
--rw-r--r--   0 amini      (501) staff       (20)       38 2023-02-16 17:35:28.000000 capsa-0.1.4/setup.cfg
--rw-r--r--   0 amini      (501) staff       (20)     1976 2023-02-16 17:35:03.000000 capsa-0.1.4/setup.py
-drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-02-16 17:35:28.000000 capsa-0.1.4/test/
--rw-r--r--   0 amini      (501) staff       (20)     1598 2023-01-11 04:49:10.000000 capsa-0.1.4/test/test_bias.py
--rw-r--r--   0 amini      (501) staff       (20)     1071 2023-01-11 04:49:10.000000 capsa-0.1.4/test/test_dropout.py
--rw-r--r--   0 amini      (501) staff       (20)     1374 2023-02-16 17:34:45.000000 capsa-0.1.4/test/test_ensemble.py
--rw-r--r--   0 amini      (501) staff       (20)     2083 2023-01-11 04:49:10.000000 capsa-0.1.4/test/test_exceptions.py
--rw-r--r--   0 amini      (501) staff       (20)     1419 2023-02-16 17:34:45.000000 capsa-0.1.4/test/test_mve.py
--rw-r--r--   0 amini      (501) staff       (20)    18351 2022-12-09 05:37:26.000000 capsa-0.1.4/test/test_risk_tensor.py
--rw-r--r--   0 amini      (501) staff       (20)     5122 2023-01-11 04:49:10.000000 capsa-0.1.4/test/test_risk_tensor_nn.py
--rw-r--r--   0 amini      (501) staff       (20)     1230 2023-01-11 04:49:10.000000 capsa-0.1.4/test/test_vae.py
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/
+-rw-r--r--   0 amini      (501) staff       (20)    34523 2022-12-09 05:37:26.000000 capsa-0.1.5/LICENSE
+-rw-r--r--   0 amini      (501) staff       (20)     5256 2023-04-11 03:44:33.000000 capsa-0.1.5/PKG-INFO
+-rw-r--r--   0 amini      (501) staff       (20)     4724 2023-04-11 03:40:00.000000 capsa-0.1.5/README.md
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa/
+-rw-r--r--   0 amini      (501) staff       (20)      268 2023-01-11 04:49:10.000000 capsa-0.1.5/capsa/__init__.py
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa/aleatoric/
+-rw-r--r--   0 amini      (501) staff       (20)       27 2022-12-09 05:37:26.000000 capsa-0.1.5/capsa/aleatoric/__init__.py
+-rw-r--r--   0 amini      (501) staff       (20)     4619 2023-01-11 04:49:10.000000 capsa-0.1.5/capsa/aleatoric/mve.py
+-rw-r--r--   0 amini      (501) staff       (20)     7761 2023-02-16 17:34:45.000000 capsa-0.1.5/capsa/base_wrapper.py
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa/bias/
+-rw-r--r--   0 amini      (501) staff       (20)       85 2023-01-11 04:49:10.000000 capsa-0.1.5/capsa/bias/__init__.py
+-rw-r--r--   0 amini      (501) staff       (20)     8019 2023-04-11 03:40:00.000000 capsa-0.1.5/capsa/bias/histogram.py
+-rw-r--r--   0 amini      (501) staff       (20)    17993 2023-04-11 03:40:00.000000 capsa-0.1.5/capsa/bias/histogramvae.py
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa/epistemic/
+-rw-r--r--   0 amini      (501) staff       (20)      102 2022-12-09 05:37:26.000000 capsa-0.1.5/capsa/epistemic/__init__.py
+-rw-r--r--   0 amini      (501) staff       (20)     5532 2023-01-11 04:49:10.000000 capsa-0.1.5/capsa/epistemic/dropout.py
+-rw-r--r--   0 amini      (501) staff       (20)     9373 2023-01-11 04:49:10.000000 capsa-0.1.5/capsa/epistemic/ensemble.py
+-rw-r--r--   0 amini      (501) staff       (20)    10530 2023-04-11 03:40:00.000000 capsa-0.1.5/capsa/epistemic/vae.py
+-rw-r--r--   0 amini      (501) staff       (20)    38773 2022-12-09 05:37:26.000000 capsa-0.1.5/capsa/risk_tensor.py
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa/utils/
+-rw-r--r--   0 amini      (501) staff       (20)      269 2023-02-16 17:34:45.000000 capsa-0.1.5/capsa/utils/__init__.py
+-rw-r--r--   0 amini      (501) staff       (20)     6609 2023-02-16 17:34:45.000000 capsa-0.1.5/capsa/utils/utils.py
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa.egg-info/
+-rw-r--r--   0 amini      (501) staff       (20)     5256 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa.egg-info/PKG-INFO
+-rw-r--r--   0 amini      (501) staff       (20)      679 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa.egg-info/SOURCES.txt
+-rw-r--r--   0 amini      (501) staff       (20)        1 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa.egg-info/dependency_links.txt
+-rw-r--r--   0 amini      (501) staff       (20)        1 2022-12-09 05:57:09.000000 capsa-0.1.5/capsa.egg-info/not-zip-safe
+-rw-r--r--   0 amini      (501) staff       (20)        6 2023-04-11 03:44:33.000000 capsa-0.1.5/capsa.egg-info/top_level.txt
+-rw-r--r--   0 amini      (501) staff       (20)       38 2023-04-11 03:44:33.000000 capsa-0.1.5/setup.cfg
+-rw-r--r--   0 amini      (501) staff       (20)     1995 2023-04-11 03:42:30.000000 capsa-0.1.5/setup.py
+drwxr-xr-x   0 amini      (501) staff       (20)        0 2023-04-11 03:44:33.000000 capsa-0.1.5/test/
+-rw-r--r--   0 amini      (501) staff       (20)     1598 2023-01-11 04:49:10.000000 capsa-0.1.5/test/test_bias.py
+-rw-r--r--   0 amini      (501) staff       (20)     1071 2023-01-11 04:49:10.000000 capsa-0.1.5/test/test_dropout.py
+-rw-r--r--   0 amini      (501) staff       (20)     1420 2023-04-11 03:40:00.000000 capsa-0.1.5/test/test_ensemble.py
+-rw-r--r--   0 amini      (501) staff       (20)     2083 2023-01-11 04:49:10.000000 capsa-0.1.5/test/test_exceptions.py
+-rw-r--r--   0 amini      (501) staff       (20)     1465 2023-04-11 03:40:00.000000 capsa-0.1.5/test/test_mve.py
+-rw-r--r--   0 amini      (501) staff       (20)    18351 2022-12-09 05:37:26.000000 capsa-0.1.5/test/test_risk_tensor.py
+-rw-r--r--   0 amini      (501) staff       (20)     5122 2023-01-11 04:49:10.000000 capsa-0.1.5/test/test_risk_tensor_nn.py
+-rw-r--r--   0 amini      (501) staff       (20)     1230 2023-01-11 04:49:10.000000 capsa-0.1.5/test/test_vae.py
```

### Comparing `capsa-0.1.4/LICENSE` & `capsa-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/PKG-INFO` & `capsa-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: capsa
-Version: 0.1.4
+Version: 0.1.5
 Summary: A data- and model-agnostic neural network wrapper for risk-aware decision making
 Home-page: https://github.com/themis-ai/capsa
-Download-URL: https://github.com/themis-ai/capsa/archive/refs/tags/0.1.4.tar.gz
+Download-URL: https://github.com/themis-ai/capsa/archive/refs/tags/0.1.5.tar.gz
 Author: Themis AI
 Author-email: info@themisai.io
 License: GNU Affero General Public License v3.0
 Keywords: capsa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -31,14 +31,15 @@
 <h2><p align="center">A Library for Risk-Aware and Trustworthy Machine Learning</p></h2>
 
 <h4><p align='center'>
 <a href="https://themisai.io/capsa/getting_started/basic_usage.html">[🚀 Getting Started]</a>
 - <a href="https://themisai.io/capsa/">[📄 Docs]</a>
 - <a href="https://www.themisai.io">[🌐 Website]</a>
 - <a href="https://themisai.io/company.html">[🧠 We're Hiring!]</a>
+- <a href="https://themisai.io/capsa/tutorials/index.html">[💡 Tutorials!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/capsa/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/capsa">
     </a>
     <a href="https://pypi.org/project/capsa/">
@@ -112,7 +113,11 @@
 
 
 # 💪 Contribution
 
 Capsa is being actively maintained and advanced. It has been built with research, extensibility, and community development as a priority. We greatly appreciate contributions to the capsa repository and codebase, including issues, enhancements, and pull requests.
 
 For more details please see <a href="https://themisai.io/capsa/contribute/">here</a>.
+
+# 💡 Support
+
+Capsa currently supports Keras Sequential models, although we are looking at possible solutions for supporting wider range of models. We can't wait to share you some new details soon!
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: capsa Version: 0.1.4 Summary: A data- and model-
+Metadata-Version: 2.1 Name: capsa Version: 0.1.5 Summary: A data- and model-
 agnostic neural network wrapper for risk-aware decision making Home-page:
 https://github.com/themis-ai/capsa Download-URL: https://github.com/themis-ai/
-capsa/archive/refs/tags/0.1.4.tar.gz Author: Themis AI Author-email:
+capsa/archive/refs/tags/0.1.5.tar.gz Author: Themis AI Author-email:
 info@themisai.io License: GNU Affero General Public License v3.0 Keywords:
 capsa Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE
   [https://raw.githubusercontent.com/themis-ai/capsa/main/docs/source/assets/
                                header-light.svg]
 ***** A Library for Risk-Aware and Trustworthy Machine Learning *****
 *** [ð_Getting_Started] - [ð_Docs] - [ð_Website] - [ð§ _We're
-Hiring!] ***
+Hiring!] - [ð¡_Tutorials!] ***
        [PyPi_Version] [PyPi_Package_Version] [PyPi_Downloads]  [License]
 
 # ð Welcome We know deploying machine learning models can be tough. Today's
 models are notoriously bad at understanding their own risks -- they are biased
 on underrepresented data, brittle on challenging out-of-distribution scenarios,
 and can fail without warning when insufficiently trained. Ensuring awareness of
 not one, but all of these risks, requires a tedious process involving changes
@@ -46,8 +46,10 @@
 capsa including other forms of risk, composing wrappers together, high-
 dimensional datasets, and more! All tutorials can be opened directly in Google
 Collab so you can play around without needing access to GPUs. # ðª
 Contribution Capsa is being actively maintained and advanced. It has been built
 with research, extensibility, and community development as a priority. We
 greatly appreciate contributions to the capsa repository and codebase,
 including issues, enhancements, and pull requests. For more details please see
-here.
+here. # ð¡ Support Capsa currently supports Keras Sequential models, although
+we are looking at possible solutions for supporting wider range of models. We
+can't wait to share you some new details soon!
```

### Comparing `capsa-0.1.4/README.md` & `capsa-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 <h2><p align="center">A Library for Risk-Aware and Trustworthy Machine Learning</p></h2>
 
 <h4><p align='center'>
 <a href="https://themisai.io/capsa/getting_started/basic_usage.html">[🚀 Getting Started]</a>
 - <a href="https://themisai.io/capsa/">[📄 Docs]</a>
 - <a href="https://www.themisai.io">[🌐 Website]</a>
 - <a href="https://themisai.io/company.html">[🧠 We're Hiring!]</a>
+- <a href="https://themisai.io/capsa/tutorials/index.html">[💡 Tutorials!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/capsa/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/capsa">
     </a>
     <a href="https://pypi.org/project/capsa/">
@@ -94,7 +95,11 @@
 
 
 # 💪 Contribution
 
 Capsa is being actively maintained and advanced. It has been built with research, extensibility, and community development as a priority. We greatly appreciate contributions to the capsa repository and codebase, including issues, enhancements, and pull requests.
 
 For more details please see <a href="https://themisai.io/capsa/contribute/">here</a>.
+
+# 💡 Support
+
+Capsa currently supports Keras Sequential models, although we are looking at possible solutions for supporting wider range of models. We can't wait to share you some new details soon!
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
   [https://raw.githubusercontent.com/themis-ai/capsa/main/docs/source/assets/
   header-light.svg]  [https://raw.githubusercontent.com/themis-ai/capsa/main/
                      docs/source/assets/header-dark.svg]
 ***** A Library for Risk-Aware and Trustworthy Machine Learning *****
 *** [ð_Getting_Started] - [ð_Docs] - [ð_Website] - [ð§ _We're
-Hiring!] ***
+Hiring!] - [ð¡_Tutorials!] ***
        [PyPi_Version] [PyPi_Package_Version] [PyPi_Downloads]  [License]
 
 # ð Welcome We know deploying machine learning models can be tough. Today's
 models are notoriously bad at understanding their own risks -- they are biased
 on underrepresented data, brittle on challenging out-of-distribution scenarios,
 and can fail without warning when insufficiently trained. Ensuring awareness of
 not one, but all of these risks, requires a tedious process involving changes
@@ -36,8 +36,10 @@
 capsa including other forms of risk, composing wrappers together, high-
 dimensional datasets, and more! All tutorials can be opened directly in Google
 Collab so you can play around without needing access to GPUs. # ðª
 Contribution Capsa is being actively maintained and advanced. It has been built
 with research, extensibility, and community development as a priority. We
 greatly appreciate contributions to the capsa repository and codebase,
 including issues, enhancements, and pull requests. For more details please see
-here.
+here. # ð¡ Support Capsa currently supports Keras Sequential models, although
+we are looking at possible solutions for supporting wider range of models. We
+can't wait to share you some new details soon!
```

### Comparing `capsa-0.1.4/capsa/aleatoric/mve.py` & `capsa-0.1.5/capsa/aleatoric/mve.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/capsa/base_wrapper.py` & `capsa-0.1.5/capsa/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/capsa/bias/histogram.py` & `capsa-0.1.5/capsa/bias/histogram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from numpy import histogram
 import tensorflow as tf
 import tensorflow_probability as tfp
 
 from ..base_wrapper import BaseWrapper
 from ..utils import copy_layer
+from ..risk_tensor import RiskTensor
+
 
 
 class HistogramWrapper(BaseWrapper):
     def __init__(self, base_model, queue_size, num_bins=5, target_hidden_layer=True):
         """
         A wrapper that generates feature histograms for a given model.
 
@@ -119,43 +121,54 @@
             self.add_queue(target_features)
             bias = None
         else:
             bias = self.get_histogram_probability(target_features)
 
         predictor_y = self.output_layer(features)
 
-        return predictor_y, bias
+        if training:
+            return predictor_y, bias
+        else:
+            bias = tf.repeat(input=tf.expand_dims(bias,axis=-1),repeats=predictor_y.shape[-1],axis=-1)
+            return RiskTensor(predictor_y, bias=bias)
+
+    def get_histogram_probability(self,features):
 
-    def get_histogram_probability(self, features):
         """
         Get the probability of each feature in the histogram. This utilizes the internal queue data-structure to calculate the probability.
 
         Parameters
         ----------
         features : tf.Tensor
             Features to calculate probability for.
 
         Returns
         -------
         logits : tf.Tensor
             Calculated probabilities for each feature.
         """
+        
+        # DON'T NEED TO CALCULATE EVERY TIME!---------------------
 
         edges = self.get_histogram_edges()
 
         frequencies = tfp.stats.histogram(
             self.queue.value(),
             edges,
             axis=0,
             extend_lower_interval=True,
             extend_upper_interval=True,
         )
 
+        epsilon = 1e-8
+
         # Normalize histograms
-        hist_probs = tf.divide(frequencies, tf.reduce_sum(frequencies, axis=0))
+        hist_probs = tf.divide(frequencies, tf.reduce_sum(frequencies, axis=0)) + epsilon
+
+        # DON'T NEED TO CALCULATE EVERY TIME!---------------------
 
         # Get the corresponding bins of the features
         bin_indices = tf.cast(
             tfp.stats.find_bins(
                 features,
                 edges,
                 extend_lower_interval=True,
@@ -167,19 +180,24 @@
         # Multiply probabilities together to compute bias
         second_element = tf.repeat(
             [tf.range(tf.shape(features)[1])], repeats=[tf.shape(features)[0]], axis=0
         )
         indices = tf.stack([bin_indices, second_element], axis=2)
 
         probabilities = tf.gather_nd(hist_probs, indices)
+
         logits = tf.reduce_sum(tf.math.log(probabilities), axis=1)
-        logits = logits - tf.math.reduce_mean(
-            logits
-        )  # log probabilities are the wrong sign if we don't subtract the mean
-        return tf.math.softmax(logits)
+
+        # logits = logits - tf.math.reduce_mean(
+        #     logits
+        # )  # log probabilities are the wrong sign if we don't subtract the mean
+
+        #return tf.math.softmax(logits)
+        
+        return tf.math.exp(logits)
 
     # Defining a Tensor Queue that saves the last ``queue_size`` values
     def build_queue(self, features):
         # Get the shape of the features
         feature_shape = tf.shape(features)
 
         # Create a queue with the shape of the features and an index to keep track of how many values are in the queue
```

### Comparing `capsa-0.1.4/capsa/bias/histogramvae.py` & `capsa-0.1.5/capsa/bias/histogramvae.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import tensorflow as tf
 from tensorflow.keras import layers
 
 from ..utils import copy_layer, _get_out_dim
 from ..base_wrapper import BaseWrapper
 import tensorflow_probability as tfp
+from ..risk_tensor import RiskTensor
 
 
 
 def kl(mu, log_std):
     return -0.5 * tf.reduce_mean(
         1 + log_std - tf.math.square(mu) - tf.math.square(tf.math.exp(log_std)),
         axis=-1,
@@ -18,15 +19,15 @@
 def mse(y, y_hat, reduce=True):
     ax = list(range(1, len(y.shape)))
     mse = tf.reduce_sum(
         (y - y_hat) ** 2,
         axis=ax,
         keepdims=(False if reduce else True),
     )
-    return tf.reduce_mean(mse) if reduce else mse
+    return tf.expand_dims(mse,axis=-1) if reduce else mse
 
 class HistogramVAEWrapper(BaseWrapper):
     """
     Combines the functionalities of both HistogramWrapper and VAEWrapper. This is done by converting a given base_model into Variational AutoEncoder architecture, with latent dimension defined by the given parameter ``latent_dim``.
 
     VAEs are typically used to learn a robust, low-dimensional representation
     of the latent space. They can be used as a method of estimating epistemic
@@ -36,15 +37,15 @@
     mapping to the latent space will be less accurate. Conversely, when the model
     is very familiar with the features being fed in, or the data is in distribution,
     we expect the latent space mapping to be robust and the reconstruction loss to be low.
 
     A histogram distribution is constructed from the mean layer of the VAE architecture. This histogram is used to estimate a    
     """
 
-    def __init__(self, base_model, latent_dim,queue_size,num_bins,decoder=None):
+    def __init__(self, base_model, latent_dim,queue_size,num_bins=5,decoder=None):
         """
         Parameters
         ----------
         base_model : tf.keras.Model
             A model to be transformed into a risk-aware variant.
         decoder : tf.keras.Model, default None
             To construct the VAE for any given model in capsa, we use the feature extractor as the encoder,
@@ -126,16 +127,22 @@
                 self.queue_built = True
 
             bias = self.get_histogram_probability(mu)
 
             # deterministic
             if T == 1:
                 rec = self.decoder(mu, training)
-                epistemic = mse(x, rec, reduce=False)
-                return y_hat,epistemic,bias
+                epistemic = mse(x, rec, reduce=True)
+
+                epistemic = tf.repeat(input=epistemic,repeats=y_hat.shape[-1],axis=-1)
+                bias = tf.repeat(input=tf.expand_dims(bias,axis=-1),repeats=y_hat.shape[-1],axis=-1)
+                if training:
+                    return y_hat, epistemic, bias
+                else:
+                    return RiskTensor(y_hat,epistemic=epistemic,bias=bias)
 
             # stochastic
             else:
                 recs = []
                 for _ in T:
                     sampled_latent = self.sampling(mu, log_std)
                     recs.append(self.decoder(sampled_latent))
@@ -179,15 +186,15 @@
 
         sampled_latent = self.sampling(mu, log_std)
         rec = self.decoder(sampled_latent)
         loss = kl(mu, log_std) + mse(x, rec)
         return loss, y_hat, bias
     
 
-    @tf.function
+    #@tf.function
     def train_step(self, data, prefix=None):
         """
         The logic for one training step.
 
         Adds the compiled loss such that the models that subclass this class don't need to explicitly add it.
         Thus the ``metric_loss`` returned from such a model is not expected to reflect the compiled
         (user specified) loss -- because it is added here.
@@ -283,41 +290,48 @@
     #     # Create a queue with the shape of the features and an index to keep track of how many values are in the queue
     #     self.queue = tf.Variable(
     #         tf.zeros([self.queue_size, feature_shape[-1]]), trainable=False
     #     )
     #     self.queue_index = tf.Variable(0, trainable=False)
 
 
-    def get_histogram_probability(self, features):
+    def get_histogram_probability(self,features):
+
         """
         Get the probability of each feature in the histogram. This utilizes the internal queue data-structure to calculate the probability.
 
         Parameters
         ----------
         features : tf.Tensor
             Features to calculate probability for.
 
         Returns
         -------
         logits : tf.Tensor
             Calculated probabilities for each feature.
         """
+        
+        # DON'T NEED TO CALCULATE EVERY TIME!---------------------
 
         edges = self.get_histogram_edges()
 
         frequencies = tfp.stats.histogram(
             self.queue.value(),
             edges,
             axis=0,
             extend_lower_interval=True,
             extend_upper_interval=True,
         )
 
+        epsilon = 1e-8
+
         # Normalize histograms
-        hist_probs = tf.divide(frequencies, tf.reduce_sum(frequencies, axis=0))
+        hist_probs = tf.divide(frequencies, tf.reduce_sum(frequencies, axis=0)) + epsilon
+
+        # DON'T NEED TO CALCULATE EVERY TIME!---------------------
 
         # Get the corresponding bins of the features
         bin_indices = tf.cast(
             tfp.stats.find_bins(
                 features,
                 edges,
                 extend_lower_interval=True,
@@ -329,19 +343,24 @@
         # Multiply probabilities together to compute bias
         second_element = tf.repeat(
             [tf.range(tf.shape(features)[1])], repeats=[tf.shape(features)[0]], axis=0
         )
         indices = tf.stack([bin_indices, second_element], axis=2)
 
         probabilities = tf.gather_nd(hist_probs, indices)
+
         logits = tf.reduce_sum(tf.math.log(probabilities), axis=1)
-        logits = logits - tf.math.reduce_mean(
-            logits
-        )  # log probabilities are the wrong sign if we don't subtract the mean
-        return tf.math.softmax(logits)
+
+        # logits = logits - tf.math.reduce_mean(
+        #     logits
+        # )  # log probabilities are the wrong sign if we don't subtract the mean
+
+        #return tf.math.softmax(logits)
+        
+        return tf.math.exp(logits)
 
 
     def add_queue(self, features):
 
         # Get the index of the queue
         index = self.get_queue_index(features)
```

### Comparing `capsa-0.1.4/capsa/epistemic/dropout.py` & `capsa-0.1.5/capsa/epistemic/dropout.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/capsa/epistemic/ensemble.py` & `capsa-0.1.5/capsa/epistemic/ensemble.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/capsa/epistemic/vae.py` & `capsa-0.1.5/capsa/epistemic/vae.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,23 +182,25 @@
             mu = self.mean_layer(features)
             log_std = self.log_std_layer(features)
 
             # deterministic
             if T == 1:
                 rec = self.decoder(mu, training)
                 epistemic = mse(x, rec, reduce=False)
+                epistemic = tf.repeat(input=epistemic,repeats=y_hat.shape[-1],axis=-1)
                 return RiskTensor(y_hat, epistemic=epistemic)
 
             # stochastic
             else:
                 recs = []
                 for _ in T:
                     sampled_latent = self.sampling(mu, log_std)
                     recs.append(self.decoder(sampled_latent))
                 std = tf.reduce_std(recs)
+                std = tf.repeat(input=std,repeats=y_hat.shape[-1],axis=-1)
                 return RiskTensor(y_hat, epistemic=std)
 
     def input_to_histogram(self, x, training=False, features=None):
         # needed to interface with the Histogram metric
         features = self.feature_extractor(x, training)
         mu = self.mean_layer(features)
         return mu
```

### Comparing `capsa-0.1.4/capsa/risk_tensor.py` & `capsa-0.1.5/capsa/risk_tensor.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/capsa/utils/utils.py` & `capsa-0.1.5/capsa/utils/utils.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/capsa.egg-info/PKG-INFO` & `capsa-0.1.5/capsa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: capsa
-Version: 0.1.4
+Version: 0.1.5
 Summary: A data- and model-agnostic neural network wrapper for risk-aware decision making
 Home-page: https://github.com/themis-ai/capsa
-Download-URL: https://github.com/themis-ai/capsa/archive/refs/tags/0.1.4.tar.gz
+Download-URL: https://github.com/themis-ai/capsa/archive/refs/tags/0.1.5.tar.gz
 Author: Themis AI
 Author-email: info@themisai.io
 License: GNU Affero General Public License v3.0
 Keywords: capsa
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -31,14 +31,15 @@
 <h2><p align="center">A Library for Risk-Aware and Trustworthy Machine Learning</p></h2>
 
 <h4><p align='center'>
 <a href="https://themisai.io/capsa/getting_started/basic_usage.html">[🚀 Getting Started]</a>
 - <a href="https://themisai.io/capsa/">[📄 Docs]</a>
 - <a href="https://www.themisai.io">[🌐 Website]</a>
 - <a href="https://themisai.io/company.html">[🧠 We're Hiring!]</a>
+- <a href="https://themisai.io/capsa/tutorials/index.html">[💡 Tutorials!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/capsa/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/capsa">
     </a>
     <a href="https://pypi.org/project/capsa/">
@@ -112,7 +113,11 @@
 
 
 # 💪 Contribution
 
 Capsa is being actively maintained and advanced. It has been built with research, extensibility, and community development as a priority. We greatly appreciate contributions to the capsa repository and codebase, including issues, enhancements, and pull requests.
 
 For more details please see <a href="https://themisai.io/capsa/contribute/">here</a>.
+
+# 💡 Support
+
+Capsa currently supports Keras Sequential models, although we are looking at possible solutions for supporting wider range of models. We can't wait to share you some new details soon!
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: capsa Version: 0.1.4 Summary: A data- and model-
+Metadata-Version: 2.1 Name: capsa Version: 0.1.5 Summary: A data- and model-
 agnostic neural network wrapper for risk-aware decision making Home-page:
 https://github.com/themis-ai/capsa Download-URL: https://github.com/themis-ai/
-capsa/archive/refs/tags/0.1.4.tar.gz Author: Themis AI Author-email:
+capsa/archive/refs/tags/0.1.5.tar.gz Author: Themis AI Author-email:
 info@themisai.io License: GNU Affero General Public License v3.0 Keywords:
 capsa Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE
   [https://raw.githubusercontent.com/themis-ai/capsa/main/docs/source/assets/
                                header-light.svg]
 ***** A Library for Risk-Aware and Trustworthy Machine Learning *****
 *** [ð_Getting_Started] - [ð_Docs] - [ð_Website] - [ð§ _We're
-Hiring!] ***
+Hiring!] - [ð¡_Tutorials!] ***
        [PyPi_Version] [PyPi_Package_Version] [PyPi_Downloads]  [License]
 
 # ð Welcome We know deploying machine learning models can be tough. Today's
 models are notoriously bad at understanding their own risks -- they are biased
 on underrepresented data, brittle on challenging out-of-distribution scenarios,
 and can fail without warning when insufficiently trained. Ensuring awareness of
 not one, but all of these risks, requires a tedious process involving changes
@@ -46,8 +46,10 @@
 capsa including other forms of risk, composing wrappers together, high-
 dimensional datasets, and more! All tutorials can be opened directly in Google
 Collab so you can play around without needing access to GPUs. # ðª
 Contribution Capsa is being actively maintained and advanced. It has been built
 with research, extensibility, and community development as a priority. We
 greatly appreciate contributions to the capsa repository and codebase,
 including issues, enhancements, and pull requests. For more details please see
-here.
+here. # ð¡ Support Capsa currently supports Keras Sequential models, although
+we are looking at possible solutions for supporting wider range of models. We
+can't wait to share you some new details soon!
```

### Comparing `capsa-0.1.4/capsa.egg-info/SOURCES.txt` & `capsa-0.1.5/capsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/setup.py` & `capsa-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.md') as readme_file:
+
+with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 # Hide the content between <!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_BEGIN --> and
 # <!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_END --> tags in the README
 while True:
     start_tag = '<!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_BEGIN -->'
     end_tag = '<!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_END -->'
@@ -46,11 +47,11 @@
     license="GNU Affero General Public License v3.0", #TODO: update
     include_package_data=True,
     keywords='capsa',
     name='capsa',
     packages=find_packages(include=['capsa', 'capsa.*']),
     setup_requires=setup_requirements,
     url='https://github.com/themis-ai/capsa',
-    download_url = 'https://github.com/themis-ai/capsa/archive/refs/tags/0.1.4.tar.gz',
-    version='0.1.4',
+    download_url = 'https://github.com/themis-ai/capsa/archive/refs/tags/0.1.5.tar.gz',
+    version='0.1.5',
     zip_safe=False,
 )
```

### Comparing `capsa-0.1.4/test/test_bias.py` & `capsa-0.1.5/test/test_bias.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/test/test_dropout.py` & `capsa-0.1.5/test/test_dropout.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/test/test_ensemble.py` & `capsa-0.1.5/test/test_mve.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,47 +2,51 @@
 import numpy as np
 import tensorflow as tf
 
 from tensorflow import keras
 import tensorflow_probability as tfp
 
 from capsa.utils import generate_moon_data_classification
-from capsa import EnsembleWrapper
 
-class test_ensemble(unittest.TestCase):
+from capsa import MVEWrapper
+
+
+class test_mve(unittest.TestCase):
 
     def test_points(self):
         
         (x_train, y_train) = generate_moon_data_classification()
 
-        max_points = np.load("data/ensemble_max_points.npy")
-        min_points = np.load("data/ensemble_min_points.npy")
+        max_points = np.load("data/mve_max_points.npy")
+        min_points = np.load("data/mve_min_points.npy")
 
         model = tf.keras.Sequential(
         [
-            tf.keras.Input(shape=(None,2)),
+            tf.keras.Input(shape=(2,)),
             tf.keras.layers.Dense(8, "relu"),
             tf.keras.layers.Dense(8, "relu"),
             tf.keras.layers.Dense(8, "relu"),
             tf.keras.layers.Dense(8, "relu"),
-            tf.keras.layers.Dense(1,"sigmoid"),
+            tf.keras.layers.Dense(2,"softmax"),
         ]
         )
 
-        wrapped_model = EnsembleWrapper(model,num_members=5)
+        wrapped_model = MVEWrapper(model,is_classification=True)
+
 
         wrapped_model.compile(
             optimizer=tf.keras.optimizers.Adam(learning_rate=2e-3),
-            loss=tf.keras.losses.BinaryCrossentropy(),
-            metrics=[tf.keras.metrics.BinaryAccuracy()],
+            loss=tf.keras.losses.CategoricalCrossentropy(),
+            metrics=[tf.keras.metrics.Accuracy()],
         )
 
-        wrapped_model.fit(x_train, y_train, epochs=2)
+        wrapped_model.fit(x_train, tf.one_hot(y_train,2), epochs=20)
 
 
-        max_results = wrapped_model(max_points).epistemic
-        min_results = wrapped_model(min_points).epistemic
+        max_results = tf.reduce_mean(wrapped_model(max_points).aleatoric,axis=-1)
+        min_results = tf.reduce_mean(wrapped_model(min_points).aleatoric,axis=-1)
 
         self.assertGreater(tf.reduce_mean(max_results),tf.reduce_mean(min_results))
 
 
-
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `capsa-0.1.4/test/test_exceptions.py` & `capsa-0.1.5/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/test/test_mve.py` & `capsa-0.1.5/test/test_ensemble.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,50 +2,48 @@
 import numpy as np
 import tensorflow as tf
 
 from tensorflow import keras
 import tensorflow_probability as tfp
 
 from capsa.utils import generate_moon_data_classification
+from capsa import EnsembleWrapper
 
-from capsa import MVEWrapper
-
-
-class test_mve(unittest.TestCase):
+class test_ensemble(unittest.TestCase):
 
     def test_points(self):
         
         (x_train, y_train) = generate_moon_data_classification()
 
-        max_points = np.load("data/mve_max_points.npy")
-        min_points = np.load("data/mve_min_points.npy")
+        max_points = np.load("data/ensemble_max_points.npy")
+        min_points = np.load("data/ensemble_min_points.npy")
 
         model = tf.keras.Sequential(
         [
-            tf.keras.Input(shape=(2,)),
+            tf.keras.Input(shape=(None,2)),
             tf.keras.layers.Dense(8, "relu"),
             tf.keras.layers.Dense(8, "relu"),
             tf.keras.layers.Dense(8, "relu"),
             tf.keras.layers.Dense(8, "relu"),
-            tf.keras.layers.Dense(2,"softmax"),
+            tf.keras.layers.Dense(1,"sigmoid"),
         ]
         )
 
-        wrapped_model = MVEWrapper(model,is_classification=True)
-
+        wrapped_model = EnsembleWrapper(model,num_members=5)
 
         wrapped_model.compile(
             optimizer=tf.keras.optimizers.Adam(learning_rate=2e-3),
-            loss=tf.keras.losses.CategoricalCrossentropy(),
-            metrics=[tf.keras.metrics.Accuracy()],
+            loss=tf.keras.losses.BinaryCrossentropy(),
+            metrics=[tf.keras.metrics.BinaryAccuracy()],
         )
 
-        wrapped_model.fit(x_train, tf.one_hot(y_train,2), epochs=20)
+        wrapped_model.fit(x_train, y_train, epochs=2)
 
 
-        max_results = tf.reduce_mean(wrapped_model(max_points).aleatoric,axis=-1)
-        min_results = tf.reduce_mean(wrapped_model(min_points).aleatoric,axis=-1)
+        max_results = wrapped_model(max_points).epistemic
+        min_results = wrapped_model(min_points).epistemic
 
         self.assertGreater(tf.reduce_mean(max_results),tf.reduce_mean(min_results))
 
 
-
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `capsa-0.1.4/test/test_risk_tensor.py` & `capsa-0.1.5/test/test_risk_tensor.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/test/test_risk_tensor_nn.py` & `capsa-0.1.5/test/test_risk_tensor_nn.py`

 * *Files identical despite different names*

### Comparing `capsa-0.1.4/test/test_vae.py` & `capsa-0.1.5/test/test_vae.py`

 * *Files identical despite different names*

