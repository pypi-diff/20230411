# Comparing `tmp/ocench-0.0.4.tar.gz` & `tmp/ocench-0.0.5.tar.gz`

## Comparing `ocench-0.0.4.tar` & `ocench-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.4/readme.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ocench-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   209449 2020-02-02 00:00:00.000000 ocench-0.0.4/figures/figure1.png
--rw-r--r--   0        0        0   341152 2020-02-02 00:00:00.000000 ocench-0.0.4/figures/figure2.jpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/__init__.py
--rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/aux_functions.py
--rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/calcular_NCH.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/example.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 ocench-0.0.4/src/OCENCH/ocench.py
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.4/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 ocench-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.5/readme.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ocench-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   209449 2020-02-02 00:00:00.000000 ocench-0.0.5/figures/figure1.png
+-rw-r--r--   0        0        0   341152 2020-02-02 00:00:00.000000 ocench-0.0.5/figures/figure2.jpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/__init__.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/aux_functions.py
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/calcular_NCH.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/example.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 ocench-0.0.5/src/OCENCH/ocench.py
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.5/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 ocench-0.0.5/PKG-INFO
```

### Comparing `ocench-0.0.4/readme.md` & `ocench-0.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/.github/workflows/python-publish.yml` & `ocench-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/figures/figure1.png` & `ocench-0.0.5/figures/figure1.png`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/figures/figure2.jpg` & `ocench-0.0.5/figures/figure2.jpg`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/src/OCENCH/aux_functions.py` & `ocench-0.0.5/src/OCENCH/aux_functions.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/src/OCENCH/calcular_NCH.py` & `ocench-0.0.5/src/OCENCH/calcular_NCH.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/src/OCENCH/example.py` & `ocench-0.0.5/src/OCENCH/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 X_test_normal, _ = make_blobs(n_samples=num_abnormal_samples, centers=[(1,1)], n_features=10, cluster_std=1, random_state=0)
 Y_train = [0] * num_normal_samples
 Y_test_abnormal = [1] * num_abnormal_samples
 Y_test_normal = [0] * num_abnormal_samples
 X_test = np.concatenate((X_test_normal, X_test_abnormal), axis=0)
 Y_test = np.concatenate((Y_test_normal, Y_test_abnormal), axis=0)
 
-model = NCH_train(X=X_train, n_projections=20, l=2, extend=0.3) # Train the model with only normal data
-prediction = NCH_classify(X=X_test, model=model) # Predict new (normal and abnormal) data
+model = OCENCH_train(X=X_train, n_projections=20, l=2, extend=0.3) # Train the model with only normal data
+prediction = OCENCH_classify(X=X_test, model=model) # Predict new (normal and abnormal) data
 
 print("[0 = Normal | 1 = Anomaly]")
 print("Real classes: ", Y_test)
 print("Predictions: ", prediction)
```

### Comparing `ocench-0.0.4/src/OCENCH/ocench.py` & `ocench-0.0.5/src/OCENCH/ocench.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from calcular_NCH import *
 from aux_functions import *
 import numpy as np
 from shapely.geometry import Point
 from shapely.geometry.polygon import Polygon
 import random
 
-def NCH_train (X, n_projections, l, extend):
+def OCENCH_train (X, n_projections, l, extend):
     contraer_SCH = False
     plot = False
     subdividir = True
     # Generamos las proyecciones bidimensionales
     random.seed(10)
     projections = generate_Projections(n_projections, X.shape[1])
     # Proyectamos los datos en estos espacios 2D
@@ -60,15 +60,15 @@
     toc1 = time.perf_counter()
     # Chekear si todos los factores de expansion son el mismo para emplear el NCH o el SNCH
     if (all(v == 0 for v in l_factor_expansion)):
         l_vertices_expandidos = [False] * len(l_factor_expansion)
 
     return l_cierres_separados, projections, l_vertices, l_aristas, l_vertices_expandidos, l_orden_vertices, l_normalizadores, l_asociacion_vertices_e_indices
 
-def NCH_classify (X, model):        
+def OCENCH_classify (X, model):        
     plot = False
     n_projections = len(model[0])
     l_cierres_separados, projections, l_vertices, l_aristas, l_vertices_expandidos, l_orden_vertices, l_normalizadores, l_asociacion_vertices_e_indices = model
     # Proyectamos los datos a clasificar
     tic = time.perf_counter() 
     # Proyectamos los datos a clasificar
     dataset_projected = project_Dataset(X, projections)
```

### Comparing `ocench-0.0.4/LICENSE.txt` & `ocench-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/README.md` & `ocench-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ocench-0.0.4/pyproject.toml` & `ocench-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ocench"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="David Novoa-Paradela", email="david.novoa@udc.es" },
   { name="Oscar Fontenla-Romero", email="oscar.fontenla@udc.es" },
   { name="Bertha Guijarro-Berdiñas", email="berta.guijarro@udc.es" },
 ]
 description = "OCENCH: A One-Class Classification method based on Expanded Non-Convex Hulls"
 readme = "README.md"
```

### Comparing `ocench-0.0.4/PKG-INFO` & `ocench-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocench
-Version: 0.0.4
+Version: 0.0.5
 Summary: OCENCH: A One-Class Classification method based on Expanded Non-Convex Hulls
 Project-URL: Homepage, https://github.com/DavidNovoaP/OCENCH
 Project-URL: Bug Tracker, https://github.com/DavidNovoaP/OCENCH/issues
 Author-email: David Novoa-Paradela <david.novoa@udc.es>, Oscar Fontenla-Romero <oscar.fontenla@udc.es>, Bertha Guijarro-Berdiñas <berta.guijarro@udc.es>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

