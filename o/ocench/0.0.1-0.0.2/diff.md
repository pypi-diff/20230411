# Comparing `tmp/ocench-0.0.1.tar.gz` & `tmp/ocench-0.0.2.tar.gz`

## Comparing `ocench-0.0.1.tar` & `ocench-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ocench-0.0.1/readme.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.1/requirements.txt
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 ocench-0.0.1/src/OCENCH/NCH.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.1/src/OCENCH/__init__.py
--rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.1/src/OCENCH/aux_functions.py
--rw-r--r--   0        0        0    18495 2020-02-02 00:00:00.000000 ocench-0.0.1/src/OCENCH/calcular_NCH.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 ocench-0.0.1/src/OCENCH/example.py
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ocench-0.0.1/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ocench-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.2/readme.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ocench-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ocench-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   209449 2020-02-02 00:00:00.000000 ocench-0.0.2/figures/figure1.png
+-rw-r--r--   0        0        0   341152 2020-02-02 00:00:00.000000 ocench-0.0.2/figures/figure2.jpg
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 ocench-0.0.2/src/OCENCH/NCH.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ocench-0.0.2/src/OCENCH/__init__.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ocench-0.0.2/src/OCENCH/aux_functions.py
+-rw-r--r--   0        0        0    18468 2020-02-02 00:00:00.000000 ocench-0.0.2/src/OCENCH/calcular_NCH.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 ocench-0.0.2/src/OCENCH/example.py
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 ocench-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 ocench-0.0.2/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ocench-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 ocench-0.0.2/PKG-INFO
```

### Comparing `ocench-0.0.1/src/OCENCH/NCH.py` & `ocench-0.0.2/src/OCENCH/NCH.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.1/src/OCENCH/aux_functions.py` & `ocench-0.0.2/src/OCENCH/aux_functions.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.1/src/OCENCH/calcular_NCH.py` & `ocench-0.0.2/src/OCENCH/calcular_NCH.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import math
 import time
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.spatial import Delaunay, ConvexHull
 from IPython import get_ipython
 from bentley_ottmann.planar import contour_self_intersects # Implementacion del algoritmo Bentley Ottmann
-from calcular_NCH import *
-from aux_functions import *
+#from aux_functions import *
 
 # #############################################################################
 
 def etapa_podado (boundary_e, boundary_v, boundary_final, dist_sorted, triangles, X, l):
     lista_aristas_sospechosas_division = []
     lista_triangulos_sospechosas_division = []
     while len(boundary_e)>0:
```

### Comparing `ocench-0.0.1/src/OCENCH/example.py` & `ocench-0.0.2/src/OCENCH/example.py`

 * *Files identical despite different names*

### Comparing `ocench-0.0.1/LICENSE.txt` & `ocench-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ocench-0.0.1/pyproject.toml` & `ocench-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ocench"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="David Novoa-Paradela", email="david.novoa@udc.es" },
   { name="Oscar Fontenla-Romero", email="oscar.fontenla@udc.es" },
   { name="Bertha Guijarro-Berdiñas", email="berta.guijarro@udc.es" },
 ]
 description = "OCENCH: A One-Class Classification method based on Expanded Non-Convex Hulls"
 readme = "README.md"
```

