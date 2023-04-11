# Comparing `tmp/DeepSlice-1.1.0.tar.gz` & `tmp/DeepSlice-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSlice-1.1.0.tar", last modified: Tue Apr 11 08:22:56 2023, max compression
+gzip compressed data, was "DeepSlice-1.1.1.tar", last modified: Tue Apr 11 11:18:03 2023, max compression
```

## Comparing `DeepSlice-1.1.0.tar` & `DeepSlice-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/coord_post_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/angle_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/depth_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/metadata/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/volumes/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/metadata/weights/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/weights/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/neural_network/network_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/neural_network/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/read_and_write/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/read_and_write/QuickNII_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/read_and_write/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-11 08:22:37.000000 DeepSlice-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:18:03.684570 DeepSlice-1.1.1/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 11:18:03.000000 DeepSlice-1.1.1/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 11:18:03.688571 DeepSlice-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-11 11:17:50.000000 DeepSlice-1.1.1/setup.py
```

### Comparing `DeepSlice-1.1.0/DeepSlice/coord_post_processing/angle_methods.py` & `DeepSlice-1.1.1/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/DeepSlice/coord_post_processing/depth_estimation.py` & `DeepSlice-1.1.1/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `DeepSlice-1.1.1/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `DeepSlice-1.1.1/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/DeepSlice/main.py` & `DeepSlice-1.1.1/DeepSlice/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,16 @@
         :type species: str
         """
         self.species = species
 
         self.config, self.metadata_path = metadata_loader.load_config()
         xception_weights =   metadata_loader.get_data_path(self.config["weight_file_paths"]["xception_imagenet"], self.metadata_path)
         weights =    metadata_loader.get_data_path(self.config["weight_file_paths"][self.species]["primary"], self.metadata_path)
-        try:
-          self.model = neural_network.initialise_network(xception_weights, weights)
-        except:
-            self.model = neural_network.initialise_network(xception_weights, weights)
-        self.weights = weights
+        self.model = neural_network.initialise_network(xception_weights, weights, self.species)
+        
 
 
     def predict(
         self,
         image_directory: str,
         ensemble: bool = None,
         section_numbers: bool = True,
@@ -151,14 +148,18 @@
                 self.species = 'rat'
                 print("switching to a rat model")
         elif filename.lower().endswith('.xml'):
             predictions = QuickNII_functions.read_QuickNII_XML(filename)
         else:
             raise ValueError('File must be a JSON or XML')
         self.predictions = predictions
+        xception_weights =   metadata_loader.get_data_path(self.config["weight_file_paths"]["xception_imagenet"], self.metadata_path)
+        weights =    metadata_loader.get_data_path(self.config["weight_file_paths"][self.species]["primary"], self.metadata_path)
+        self.model = neural_network.initialise_network(xception_weights, weights, self.species) 
+
         
 
     def save_predictions(self, filename):
         """
         Save the predictions to a QuickNII compatible JSON file.
 
         :param filename: the name of the file to save to
```

### Comparing `DeepSlice-1.1.0/DeepSlice/metadata/config.json` & `DeepSlice-1.1.1/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/DeepSlice/metadata/metadata_loader.py` & `DeepSlice-1.1.1/DeepSlice/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/DeepSlice/neural_network/neural_network.py` & `DeepSlice-1.1.1/DeepSlice/neural_network/neural_network.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,41 @@
     :return: The converted image
     :rtype: numpy.ndarray
     """
     img = rgb2gray(img).reshape(299, 299, 1)
     return img
 
 
-def initialise_network(xception_weights: str, weights: str) -> Sequential:
+def initialise_network(xception_weights: str, weights: str, species: str) -> Sequential:
     """
     Initialise a neural network with the given weights
 
     :param weights: The weights for the network
     :type weights: list
+    :param species: The species of the animal, this is necessary because of a previous error where the models are slightly different for different species
     :return: The initialised neural network
     :rtype: keras.models.Sequential
     """
     base_model = Xception(include_top=True, weights=xception_weights)
     base_model._layers.pop()
     base_model._layers.pop()
-    model = Sequential()
-    model.add(base_model)
-    model.add(Dense(256, activation="relu"))
-    model.add(Dense(256, activation="relu"))
-    model.add(Dense(9, activation="linear"))
+    if species == "rat":
+        inputs = Input(shape=(299, 299, 3))
+        base_model_layer = base_model(inputs, training=True)
+        dense1_layer = Dense(256, activation="relu")(base_model_layer)
+        dense2_layer = Dense(256, activation="relu")(dense1_layer)
+        output_layer = Dense(9, activation="linear")(dense2_layer)
+        model = Model(inputs=inputs, outputs=output_layer)
+    else:
+        model = Sequential()
+        model.add(base_model)
+        model.add(Dense(256, activation="relu"))
+        model.add(Dense(256, activation="relu"))
+        model.add(Dense(9, activation="linear"))
+
     if weights != None:
         model.load_weights(weights)
     return model
 
 
 
 def load_images(image_path: str) -> np.ndarray:
```

### Comparing `DeepSlice-1.1.0/DeepSlice/read_and_write/QuickNII_functions.py` & `DeepSlice-1.1.1/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/DeepSlice.egg-info/PKG-INFO` & `DeepSlice-1.1.1/DeepSlice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.0.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.1.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.0 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.1 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.0.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.1.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.0/DeepSlice.egg-info/SOURCES.txt` & `DeepSlice-1.1.1/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/LICENSE` & `DeepSlice-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/PKG-INFO` & `DeepSlice-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.0.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.1.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.0 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.1 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.0.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.1.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.0/README.md` & `DeepSlice-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.0/setup.py` & `DeepSlice-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.1.0',
+    version='1.1.1',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.0.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.1.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
         'tensorflow==1.15.0',
         'h5py==2.10.0',
```

