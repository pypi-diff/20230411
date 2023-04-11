# Comparing `tmp/ocench-0.0.3.tar.gz` & `tmp/ocench-0.0.4.tar.gz`

## Comparing `ocench-0.0.3.tar` & `ocench-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.3/readme.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ocench-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   209449 2020-02-02 00:00:00.000000 ocench-0.0.3/figures/figure1.png
--rw-r--r--   0        0        0   341152 2020-02-02 00:00:00.000000 ocench-0.0.3/figures/figure2.jpg
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 ocench-0.0.3/src/OCENCH/NCH.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.3/src/OCENCH/__init__.py
--rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.3/src/OCENCH/aux_functions.py
--rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 ocench-0.0.3/src/OCENCH/calcular_NCH.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 ocench-0.0.3/src/OCENCH/example.py
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.3/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 ocench-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.4/readme.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ocench-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   209449 2020-02-02 00:00:00.000000 ocench-0.0.4/figures/figure1.png
+-rw-r--r--   0        0        0   341152 2020-02-02 00:00:00.000000 ocench-0.0.4/figures/figure2.jpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/__init__.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/aux_functions.py
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/calcular_NCH.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/example.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/ocench.py
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.4/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 ocench-0.0.4/PKG-INFO
```

### Comparing `ocench-0.0.3/readme.md` & `ocench-0.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/.github/workflows/python-publish.yml` & `ocench-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/figures/figure1.png` & `ocench-0.0.4/figures/figure1.png`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/figures/figure2.jpg` & `ocench-0.0.4/figures/figure2.jpg`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/src/OCENCH/NCH.py` & `ocench-0.0.4/src/OCENCH/ocench.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/src/OCENCH/aux_functions.py` & `ocench-0.0.4/src/OCENCH/aux_functions.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/src/OCENCH/calcular_NCH.py` & `ocench-0.0.4/src/OCENCH/calcular_NCH.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/src/OCENCH/example.py` & `ocench-0.0.4/src/OCENCH/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.datasets import make_blobs
 import pandas as pd
-from NCH import *
+from ocench import *
 
 num_normal_samples = 1000 # Training dataset size (only normal data)
 num_abnormal_samples = 10 # Number of anomalies to classify in test
 
 # Create a toy dataset using two isotropic Gaussian blobs (one for each class)
 X_train, _ = make_blobs(n_samples=num_normal_samples, centers= [(1,1)], n_features=10, cluster_std=1, random_state=0)
 X_test_abnormal, _ = make_blobs(n_samples=num_abnormal_samples, centers=[(20,20)], n_features=10, cluster_std=1, random_state=0)
```

### Comparing `ocench-0.0.3/LICENSE.txt` & `ocench-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/README.md` & `ocench-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ocench-0.0.3/pyproject.toml` & `ocench-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ocench"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="David Novoa-Paradela", email="david.novoa@udc.es" },
   { name="Oscar Fontenla-Romero", email="oscar.fontenla@udc.es" },
   { name="Bertha Guijarro-Berdiñas", email="berta.guijarro@udc.es" },
 ]
 description = "OCENCH: A One-Class Classification method based on Expanded Non-Convex Hulls"
 readme = "README.md"
```

### Comparing `ocench-0.0.3/PKG-INFO` & `ocench-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocench
-Version: 0.0.3
+Version: 0.0.4
 Summary: OCENCH: A One-Class Classification method based on Expanded Non-Convex Hulls
 Project-URL: Homepage, https://github.com/DavidNovoaP/OCENCH
 Project-URL: Bug Tracker, https://github.com/DavidNovoaP/OCENCH/issues
 Author-email: David Novoa-Paradela <david.novoa@udc.es>, Oscar Fontenla-Romero <oscar.fontenla@udc.es>, Bertha Guijarro-Berdiñas <berta.guijarro@udc.es>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

