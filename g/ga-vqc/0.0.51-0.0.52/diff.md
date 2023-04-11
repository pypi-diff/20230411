# Comparing `tmp/ga_vqc-0.0.51.tar.gz` & `tmp/ga_vqc-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga_vqc-0.0.51.tar", last modified: Sun Apr  9 08:41:32 2023, max compression
+gzip compressed data, was "ga_vqc-0.0.52.tar", last modified: Tue Apr 11 04:40:45 2023, max compression
```

## Comparing `ga_vqc-0.0.51.tar` & `ga_vqc-0.0.52.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 08:41:32.989402 ga_vqc-0.0.51/
--rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.51/LICENSE
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 08:41:32.989009 ga_vqc-0.0.51/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.51/README.md
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 08:41:32.986683 ga_vqc-0.0.51/ga_vqc/
--rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.51/ga_vqc/Distance.py
--rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.51/ga_vqc/GA_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.51/ga_vqc/GA_Manager.py
--rw-r--r--   0 tsievert   (502) staff       (20)     1007 2023-04-09 08:12:19.000000 ga_vqc-0.0.51/ga_vqc/GA_Support.py
--rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.51/ga_vqc/Genes.py
--rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.51/ga_vqc/VQC_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)       69 2023-04-07 16:50:57.000000 ga_vqc-0.0.51/ga_vqc/__init__.py
--rw-r--r--   0 tsievert   (502) staff       (20)    11015 2023-04-09 08:26:52.000000 ga_vqc-0.0.51/ga_vqc/simple_Individual.py
--rw-r--r--   0 tsievert   (502) staff       (20)    17922 2023-04-09 08:39:45.000000 ga_vqc-0.0.51/ga_vqc/simple_Model.py
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-09 08:41:32.988536 ga_vqc-0.0.51/ga_vqc.egg-info/
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/SOURCES.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/dependency_links.txt
--rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/requires.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-09 08:41:32.000000 ga_vqc-0.0.51/ga_vqc.egg-info/top_level.txt
--rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-09 08:41:32.989501 ga_vqc-0.0.51/setup.cfg
--rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-09 08:05:39.000000 ga_vqc-0.0.51/setup.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 04:40:45.678962 ga_vqc-0.0.52/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.52/LICENSE
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 04:40:45.678480 ga_vqc-0.0.52/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.52/README.md
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 04:40:45.675744 ga_vqc-0.0.52/ga_vqc/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.52/ga_vqc/Distance.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.52/ga_vqc/GA_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.52/ga_vqc/GA_Manager.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     1007 2023-04-09 08:12:19.000000 ga_vqc-0.0.52/ga_vqc/GA_Support.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.52/ga_vqc/Genes.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.52/ga_vqc/VQC_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      159 2023-04-10 20:43:29.000000 ga_vqc-0.0.52/ga_vqc/__init__.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    11033 2023-04-10 20:42:42.000000 ga_vqc-0.0.52/ga_vqc/simple_Individual.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    17973 2023-04-11 01:30:41.000000 ga_vqc-0.0.52/ga_vqc/simple_Model.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 04:40:45.677829 ga_vqc-0.0.52/ga_vqc.egg-info/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/SOURCES.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/dependency_links.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/requires.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/top_level.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-11 04:40:45.679100 ga_vqc-0.0.52/setup.cfg
+-rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-11 04:40:02.000000 ga_vqc-0.0.52/setup.py
```

### Comparing `ga_vqc-0.0.51/LICENSE` & `ga_vqc-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.51/PKG-INFO` & `ga_vqc-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga_vqc
-Version: 0.0.51
+Version: 0.0.52
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.51/README.md` & `ga_vqc-0.0.52/README.md`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.51/ga_vqc/Distance.py` & `ga_vqc-0.0.52/ga_vqc/Distance.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.51/ga_vqc/GA_Manager.py` & `ga_vqc-0.0.52/ga_vqc/GA_Manager.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.51/ga_vqc/GA_Support.py` & `ga_vqc-0.0.52/ga_vqc/GA_Support.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.51/ga_vqc/Genes.py` & `ga_vqc-0.0.52/ga_vqc/Genes.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.51/ga_vqc/simple_Individual.py` & `ga_vqc-0.0.52/ga_vqc/simple_Individual.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class Individual(GA_Individual):
     """
     Data structure for the ansatz.
     """
 
-    def __init__(self, n_qubits, n_moments, genepool, rng_seed, ansatz=None):
+    def __init__(self, n_qubits, n_moments, genepool, rng_seed, ansatz_dicts=None):
         """
         Initializes the inidivual object, all individuals (ansatz) are members of this class.
             - n_qubits: Number of qubits in the ansatz.
             - n_moments: Number of moments in the ansatz.
             - genepool: All the allowed gates for the ansatz, as well as meta-data 
                             about those gates.
 
@@ -29,18 +29,18 @@
         self.pennylane_rng = pnp.random.default_rng(seed=rng_seed)
 
         self.ansatz_dicts = []
         self.ansatz_qml = []
         self.ansatz_draw = []
         self.params = []
 
-        if ansatz is None:
+        if ansatz_dicts is None:
             self.generate()
         else:
-            self.generate_from(ansatz)
+            self.generate_from(ansatz_dicts)
         self.convert_to_qml()
         self.draw_ansatz()
 
     def __len__(self):
         return len(self.ansatz_dicts[0])
 
     def __getitem__(self, key):
@@ -97,15 +97,15 @@
                         self.ansatz_dicts[moment][qubit] = gate.name
                 else:
                     raise Exception("Gates with more than 2 qubits haven't been implemented yet.")
 
     def generate_from(self, ansatz):
         self.ansatz_dicts = copy.deepcopy(ansatz)
         self.convert_to_qml()
-        self.ansatz_draw()
+        self.draw_ansatz()
 
     def convert_to_qml(self):
         """
         Converts the ansatz into a general format for the QML.
 
             moment_dict example: _C (_T) means current qubit is control (target) qubit of 2-qubit gate
                 {'I': [],
```

### Comparing `ga_vqc-0.0.51/ga_vqc/simple_Model.py` & `ga_vqc-0.0.52/ga_vqc/simple_Model.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,16 @@
                     )
                 )
         for i in range(len(output_arr)):
             # Both the fitness metrics and eval_metrics must be JSON serializable -> (ie. 
             #  default python classes or have custom serialization)
             self.fitness_arr[i] = output_arr[i]["fitness_metric"]
             self.metrics_arr[i] = output_arr[i]["eval_metrics"]
+
+        print(len(self.fitness_arr))
         end_time = time.time()
         exec_time = end_time - start_time
         print(f"QML Optimization in {exec_time:.2f} seconds")
 
         if self.best_perf["fitness"] < np.amax(self.fitness_arr):
             print("!! IMPROVED PERFORMANCE !!")
             self.best_perf["fitness"] = np.amax(self.fitness_arr).item()
@@ -268,15 +270,15 @@
         plt.title("tSNE of Current Population")
         plt.savefig(filepath_tsne, format="png")
         plt.close(1)
 
         results = {
             "full_population": [i.ansatz_dicts for i in self.population],
             "full_drawn_population": [i.ansatz_draw for i in self.population],
-            "full_fitness": self.fitness_arr,
+            "full_fitness": [i for i in self.fitness_arr],
             "fitness_stats": f"Avg fitness: {np.mean(self.fitness_arr)}, Std. Dev: {np.std(self.fitness_arr)}",
             "full_eval_metrics": self.metrics_arr,
             "eval_metrics_stats": [
                 f"Avg {k}: {np.mean([i[k] for i in self.metrics_arr])}, "
                 + f"Std. Dev: {np.std([i[k] for i in self.metrics_arr])}"
                 for k in self.metrics_arr[0].keys()
             ],
```

### Comparing `ga_vqc-0.0.51/ga_vqc.egg-info/PKG-INFO` & `ga_vqc-0.0.52/ga_vqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-vqc
-Version: 0.0.51
+Version: 0.0.52
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.51/setup.py` & `ga_vqc-0.0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ga_vqc",
-    version="0.0.51",
+    version="0.0.52",
     description="Genetic Algorithm for VQC ansatz search.",
     packages=find_packages(include=["ga_vqc"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

