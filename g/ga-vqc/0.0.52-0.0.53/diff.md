# Comparing `tmp/ga_vqc-0.0.52.tar.gz` & `tmp/ga_vqc-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga_vqc-0.0.52.tar", last modified: Tue Apr 11 04:40:45 2023, max compression
+gzip compressed data, was "ga_vqc-0.0.53.tar", last modified: Tue Apr 11 06:33:37 2023, max compression
```

## Comparing `ga_vqc-0.0.52.tar` & `ga_vqc-0.0.53.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 04:40:45.678962 ga_vqc-0.0.52/
--rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.52/LICENSE
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 04:40:45.678480 ga_vqc-0.0.52/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.52/README.md
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 04:40:45.675744 ga_vqc-0.0.52/ga_vqc/
--rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.52/ga_vqc/Distance.py
--rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.52/ga_vqc/GA_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.52/ga_vqc/GA_Manager.py
--rw-r--r--   0 tsievert   (502) staff       (20)     1007 2023-04-09 08:12:19.000000 ga_vqc-0.0.52/ga_vqc/GA_Support.py
--rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.52/ga_vqc/Genes.py
--rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.52/ga_vqc/VQC_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      159 2023-04-10 20:43:29.000000 ga_vqc-0.0.52/ga_vqc/__init__.py
--rw-r--r--   0 tsievert   (502) staff       (20)    11033 2023-04-10 20:42:42.000000 ga_vqc-0.0.52/ga_vqc/simple_Individual.py
--rw-r--r--   0 tsievert   (502) staff       (20)    17973 2023-04-11 01:30:41.000000 ga_vqc-0.0.52/ga_vqc/simple_Model.py
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 04:40:45.677829 ga_vqc-0.0.52/ga_vqc.egg-info/
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/SOURCES.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/dependency_links.txt
--rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/requires.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-11 04:40:45.000000 ga_vqc-0.0.52/ga_vqc.egg-info/top_level.txt
--rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-11 04:40:45.679100 ga_vqc-0.0.52/setup.cfg
--rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-11 04:40:02.000000 ga_vqc-0.0.52/setup.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 06:33:37.255360 ga_vqc-0.0.53/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.53/LICENSE
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 06:33:37.254998 ga_vqc-0.0.53/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.53/README.md
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 06:33:37.251944 ga_vqc-0.0.53/ga_vqc/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1916 2023-04-09 06:07:20.000000 ga_vqc-0.0.53/ga_vqc/Distance.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.53/ga_vqc/GA_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.53/ga_vqc/GA_Manager.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     1007 2023-04-09 08:12:19.000000 ga_vqc-0.0.53/ga_vqc/GA_Support.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.53/ga_vqc/Genes.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.53/ga_vqc/VQC_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      159 2023-04-10 20:43:29.000000 ga_vqc-0.0.53/ga_vqc/__init__.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    11033 2023-04-10 20:42:42.000000 ga_vqc-0.0.53/ga_vqc/simple_Individual.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    17986 2023-04-11 06:32:50.000000 ga_vqc-0.0.53/ga_vqc/simple_Model.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-11 06:33:37.254488 ga_vqc-0.0.53/ga_vqc.egg-info/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/SOURCES.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/dependency_links.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/requires.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-11 06:33:37.000000 ga_vqc-0.0.53/ga_vqc.egg-info/top_level.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-11 06:33:37.255473 ga_vqc-0.0.53/setup.cfg
+-rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-11 04:45:04.000000 ga_vqc-0.0.53/setup.py
```

### Comparing `ga_vqc-0.0.52/LICENSE` & `ga_vqc-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.52/PKG-INFO` & `ga_vqc-0.0.53/ga_vqc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ga_vqc
-Version: 0.0.52
+Name: ga-vqc
+Version: 0.0.53
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.52/README.md` & `ga_vqc-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.52/ga_vqc/Distance.py` & `ga_vqc-0.0.53/ga_vqc/Distance.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.52/ga_vqc/GA_Manager.py` & `ga_vqc-0.0.53/ga_vqc/GA_Manager.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.52/ga_vqc/GA_Support.py` & `ga_vqc-0.0.53/ga_vqc/GA_Support.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.52/ga_vqc/Genes.py` & `ga_vqc-0.0.53/ga_vqc/Genes.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.52/ga_vqc/simple_Individual.py` & `ga_vqc-0.0.53/ga_vqc/simple_Individual.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.52/ga_vqc/simple_Model.py` & `ga_vqc-0.0.53/ga_vqc/simple_Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,16 @@
 
             print(
                 f"Best fitness: {self.best_perf['fitness']}, " + 
                 f"Best metrics: {self.best_perf['eval_metrics']}, " +
                 f"Best ansatz: {self.best_perf['ansatz_dicts']}"
             )
 
-            if gen > 20:
-                if (gen - self.best_perf["generation"]) > self.n_steps_patience:
-                    break
+            if (gen - self.best_perf["generation"]) > self.n_steps_patience:
+                break
             print(
                 "filepath is: ",
                 make_results_json(results, self.start_time, self.ga_output_path, gen)
             )
             gen += 1
         print(
             "filepath is: ",
@@ -206,15 +205,14 @@
                 )
         for i in range(len(output_arr)):
             # Both the fitness metrics and eval_metrics must be JSON serializable -> (ie. 
             #  default python classes or have custom serialization)
             self.fitness_arr[i] = output_arr[i]["fitness_metric"]
             self.metrics_arr[i] = output_arr[i]["eval_metrics"]
 
-        print(len(self.fitness_arr))
         end_time = time.time()
         exec_time = end_time - start_time
         print(f"QML Optimization in {exec_time:.2f} seconds")
 
         if self.best_perf["fitness"] < np.amax(self.fitness_arr):
             print("!! IMPROVED PERFORMANCE !!")
             self.best_perf["fitness"] = np.amax(self.fitness_arr).item()
@@ -242,17 +240,19 @@
         filepath_euclid = os.path.join(
             destdir_curves,
             "%03deuclid_distance_data.png"
             % gen
         )
         plt.figure(0)
         plt.style.use("seaborn")
-        plt.scatter(distances_from_best, [i["auroc"] for i in self.metrics_arr], marker=".", color="g")
+        plt.scatter(distances_from_best, self.fitness_arr, marker=".", c=[i["auroc"] for i in self.metrics_arr], cmap=plt.set_cmap('plasma'))
+        cbar = plt.colorbar()
+        cbar.set_label("AUROC")
         plt.ylabel("AUROC")
-        plt.xlabel("Euclidian distance from best ansatz")
+        plt.xlabel("Euclidian distance")
         plt.title("Euclidean Distances from Best Performing Ansatz")
         plt.savefig(filepath_euclid, format="png")
         plt.close(0)
         ### tSNE clustering ###
         data_tsne = tsne(self.population, rng_seed=self.rng_seed, perplexity=2)
         x, y = data_tsne[0], data_tsne[1]
         filepath_tsne = os.path.join(
```

### Comparing `ga_vqc-0.0.52/ga_vqc.egg-info/PKG-INFO` & `ga_vqc-0.0.53/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ga-vqc
-Version: 0.0.52
+Name: ga_vqc
+Version: 0.0.53
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.52/setup.py` & `ga_vqc-0.0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ga_vqc",
-    version="0.0.52",
+    version="0.0.53",
     description="Genetic Algorithm for VQC ansatz search.",
     packages=find_packages(include=["ga_vqc"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

