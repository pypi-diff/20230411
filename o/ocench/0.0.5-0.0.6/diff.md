# Comparing `tmp/ocench-0.0.5.tar.gz` & `tmp/ocench-0.0.6.tar.gz`

## Comparing `ocench-0.0.5.tar` & `ocench-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.5/readme.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ocench-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   209449 2020-02-02 00:00:00.000000 ocench-0.0.5/figures/figure1.png
--rw-r--r--   0        0        0   341152 2020-02-02 00:00:00.000000 ocench-0.0.5/figures/figure2.jpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/__init__.py
--rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/aux_functions.py
--rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/calcular_NCH.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/example.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/ocench.py
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.5/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 ocench-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 ocench-0.0.6/readme.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ocench-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   209449 2020-02-02 00:00:00.000000 ocench-0.0.6/figures/figure1.png
+-rw-r--r--   0        0        0   341152 2020-02-02 00:00:00.000000 ocench-0.0.6/figures/figure2.jpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.6/src/OCENCH/__init__.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.6/src/OCENCH/aux_functions.py
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 ocench-0.0.6/src/OCENCH/calcular_NCH.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ocench-0.0.6/src/OCENCH/example.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 ocench-0.0.6/src/OCENCH/ocench.py
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 ocench-0.0.6/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 ocench-0.0.6/PKG-INFO
```

### Comparing `ocench-0.0.5/readme.md` & `ocench-0.0.6/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
        - **labels**: 1-D numpy array containing the predicted labels for the input dataset, where 0 = Normal and 1 = Anomaly.
 
 ------------
 
 ## Example
 
 ```python
-from NCH import *
+from ocench import *
 from sklearn.datasets import make_blobs  
 
 # Create a toy dataset using two isotropic Gaussian blobs (one for each class)
 num_normal_samples = 1000 # Training dataset size (only normal data)
 num_abnormal_samples = 10 # Number of anomalies to classify in test
 X_train, _ = make_blobs(n_samples=num_normal_samples, centers= [(1,1)], n_features=10, cluster_std=1, random_state=0)
 X_test_abnormal, _ = make_blobs(n_samples=num_abnormal_samples, centers=[(20,20)], n_features=10, cluster_std=1, random_state=0)
@@ -62,17 +62,17 @@
 Y_train = [0] * num_normal_samples
 Y_test_abnormal = [1] * num_abnormal_samples
 Y_test_normal = [0] * num_abnormal_samples
 X_test = np.concatenate((X_test_normal, X_test_abnormal), axis=0)
 Y_test = np.concatenate((Y_test_normal, Y_test_abnormal), axis=0)
 
 # Train the model with only normal data
-model = NCH_train(X=X_train, n_projections=20, l=2, extend=0.3) 
+model = OCENCH_train(X=X_train, n_projections=20, l=2, extend=0.3) 
 # Predict new (normal and abnormal) data
-prediction = NCH_classify(X=X_test, model=model) 
+prediction = OCENCH_classify(X=X_test, model=model) 
 
 # [0 = Normal | 1 = Anomaly]
 print("Real classes: ", Y_test)
 print("Predictions: ", prediction)
 ```
 
 ## Citations
```

### Comparing `ocench-0.0.5/.github/workflows/python-publish.yml` & `ocench-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/figures/figure1.png` & `ocench-0.0.6/figures/figure1.png`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/figures/figure2.jpg` & `ocench-0.0.6/figures/figure2.jpg`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/src/OCENCH/aux_functions.py` & `ocench-0.0.6/src/OCENCH/aux_functions.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/src/OCENCH/calcular_NCH.py` & `ocench-0.0.6/src/OCENCH/calcular_NCH.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/src/OCENCH/example.py` & `ocench-0.0.6/src/OCENCH/example.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/src/OCENCH/ocench.py` & `ocench-0.0.6/src/OCENCH/ocench.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/LICENSE.txt` & `ocench-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ocench-0.0.5/README.md` & `ocench-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
        - **labels**: 1-D numpy array containing the predicted labels for the input dataset, where 0 = Normal and 1 = Anomaly.
 
 ------------
 
 ## Example
 
 ```python
-from NCH import *
+from ocench import *
 from sklearn.datasets import make_blobs  
 
 # Create a toy dataset using two isotropic Gaussian blobs (one for each class)
 num_normal_samples = 1000 # Training dataset size (only normal data)
 num_abnormal_samples = 10 # Number of anomalies to classify in test
 X_train, _ = make_blobs(n_samples=num_normal_samples, centers= [(1,1)], n_features=10, cluster_std=1, random_state=0)
 X_test_abnormal, _ = make_blobs(n_samples=num_abnormal_samples, centers=[(20,20)], n_features=10, cluster_std=1, random_state=0)
@@ -62,17 +62,17 @@
 Y_train = [0] * num_normal_samples
 Y_test_abnormal = [1] * num_abnormal_samples
 Y_test_normal = [0] * num_abnormal_samples
 X_test = np.concatenate((X_test_normal, X_test_abnormal), axis=0)
 Y_test = np.concatenate((Y_test_normal, Y_test_abnormal), axis=0)
 
 # Train the model with only normal data
-model = NCH_train(X=X_train, n_projections=20, l=2, extend=0.3) 
+model = OCENCH_train(X=X_train, n_projections=20, l=2, extend=0.3) 
 # Predict new (normal and abnormal) data
-prediction = NCH_classify(X=X_test, model=model) 
+prediction = OCENCH_classify(X=X_test, model=model) 
 
 # [0 = Normal | 1 = Anomaly]
 print("Real classes: ", Y_test)
 print("Predictions: ", prediction)
 ```
 
 ## Citations
```

### Comparing `ocench-0.0.5/pyproject.toml` & `ocench-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ocench"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="David Novoa-Paradela", email="david.novoa@udc.es" },
   { name="Oscar Fontenla-Romero", email="oscar.fontenla@udc.es" },
   { name="Bertha Guijarro-Berdiñas", email="berta.guijarro@udc.es" },
 ]
 description = "OCENCH: A One-Class Classification method based on Expanded Non-Convex Hulls"
 readme = "README.md"
```

### Comparing `ocench-0.0.5/PKG-INFO` & `ocench-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocench
-Version: 0.0.5
+Version: 0.0.6
 Summary: OCENCH: A One-Class Classification method based on Expanded Non-Convex Hulls
 Project-URL: Homepage, https://github.com/DavidNovoaP/OCENCH
 Project-URL: Bug Tracker, https://github.com/DavidNovoaP/OCENCH/issues
 Author-email: David Novoa-Paradela <david.novoa@udc.es>, Oscar Fontenla-Romero <oscar.fontenla@udc.es>, Bertha Guijarro-Berdiñas <berta.guijarro@udc.es>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -60,15 +60,15 @@
        - **labels**: 1-D numpy array containing the predicted labels for the input dataset, where 0 = Normal and 1 = Anomaly.
 
 ------------
 
 ## Example
 
 ```python
-from NCH import *
+from ocench import *
 from sklearn.datasets import make_blobs  
 
 # Create a toy dataset using two isotropic Gaussian blobs (one for each class)
 num_normal_samples = 1000 # Training dataset size (only normal data)
 num_abnormal_samples = 10 # Number of anomalies to classify in test
 X_train, _ = make_blobs(n_samples=num_normal_samples, centers= [(1,1)], n_features=10, cluster_std=1, random_state=0)
 X_test_abnormal, _ = make_blobs(n_samples=num_abnormal_samples, centers=[(20,20)], n_features=10, cluster_std=1, random_state=0)
@@ -76,17 +76,17 @@
 Y_train = [0] * num_normal_samples
 Y_test_abnormal = [1] * num_abnormal_samples
 Y_test_normal = [0] * num_abnormal_samples
 X_test = np.concatenate((X_test_normal, X_test_abnormal), axis=0)
 Y_test = np.concatenate((Y_test_normal, Y_test_abnormal), axis=0)
 
 # Train the model with only normal data
-model = NCH_train(X=X_train, n_projections=20, l=2, extend=0.3) 
+model = OCENCH_train(X=X_train, n_projections=20, l=2, extend=0.3) 
 # Predict new (normal and abnormal) data
-prediction = NCH_classify(X=X_test, model=model) 
+prediction = OCENCH_classify(X=X_test, model=model) 
 
 # [0 = Normal | 1 = Anomaly]
 print("Real classes: ", Y_test)
 print("Predictions: ", prediction)
 ```
 
 ## Citations
```

