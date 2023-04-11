# Comparing `tmp/DeepSlice-1.0.6.tar.gz` & `tmp/DeepSlice-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DeepSlice-1.0.6.tar", last modified: Wed Feb 22 13:33:48 2023, max compression
+gzip compressed data, was "DeepSlice-1.1.0.tar", last modified: Tue Apr 11 08:22:56 2023, max compression
```

## Comparing `DeepSlice-1.0.6.tar` & `DeepSlice-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       27 2023-02-21 12:44:35.000000 DeepSlice-1.0.6/DeepSlice/__init__.py
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       17 2023-02-21 13:54:23.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/__init__.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     5530 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/angle_methods.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     1197 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/depth_estimation.py
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/plane_alignment_functions/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       17 2023-02-21 13:54:23.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)    12255 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     8888 2023-02-21 08:30:40.000000 DeepSlice-1.0.6/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     7544 2023-02-21 08:39:02.000000 DeepSlice-1.0.6/DeepSlice/main.py
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/metadata/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       17 2023-02-21 13:54:23.000000 DeepSlice-1.0.6/DeepSlice/metadata/__init__.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     1984 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/metadata/config.json
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     1326 2023-02-21 08:30:40.000000 DeepSlice-1.0.6/DeepSlice/metadata/metadata_loader.py
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/metadata/volumes/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/metadata/volumes/placeholder.txt
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/metadata/weights/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/metadata/weights/placeholder.txt
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/neural_network/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       17 2023-02-21 13:54:23.000000 DeepSlice-1.0.6/DeepSlice/neural_network/__init__.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/neural_network/network_architecture.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     6468 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/neural_network/neural_network.py
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice/read_and_write/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     5009 2023-02-20 16:39:10.000000 DeepSlice-1.0.6/DeepSlice/read_and_write/QuickNII_functions.py
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       17 2023-02-21 13:54:23.000000 DeepSlice-1.0.6/DeepSlice/read_and_write/__init__.py
-drwxrwxrwx   0 harryc   (357689) harryc   (342363)        0 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice.egg-info/
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     7832 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice.egg-info/PKG-INFO
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)      987 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice.egg-info/SOURCES.txt
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)        1 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice.egg-info/dependency_links.txt
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)      109 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice.egg-info/requires.txt
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       10 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/DeepSlice.egg-info/top_level.txt
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)    35149 2023-02-06 16:54:07.000000 DeepSlice-1.0.6/LICENSE
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     7832 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/PKG-INFO
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     7105 2023-02-22 13:32:19.000000 DeepSlice-1.0.6/README.md
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)       79 2023-02-22 13:33:48.000000 DeepSlice-1.0.6/setup.cfg
--rwxrwxrwx   0 harryc   (357689) harryc   (342363)     1444 2023-02-22 13:33:42.000000 DeepSlice-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 08:22:56.000000 DeepSlice-1.1.0/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-11 08:22:36.000000 DeepSlice-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 08:22:56.905439 DeepSlice-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-11 08:22:37.000000 DeepSlice-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `DeepSlice-1.0.6/DeepSlice/coord_post_processing/angle_methods.py` & `DeepSlice-1.1.0/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 def calculate_brain_center_coordinate(section, atlas_shape, axis):
     """
     Calculates the coordinate closest to the middle of the section as defined by the two 
     dimensions not orthogonal to the dimension along which the series is being aligned.
     for example, if the series is being aligned coronally then this will return the midpoint
     in X and Z as coronal series are spaced along the Y coordinate in the CCF.
+
     :param section: The section to calculate the center for
     :param atlas_shape: The shape of the atlas
     :param axis: The axis along which the series is being aligned ('sagittal', 'coronal', 'horizontal')
     :return: The coordinate closest to the middle of the section
     """
     if axis not in ["sagittal", "coronal", "horizontal"]:
         raise ValueError("axis must be one of sagittal, coronal, or horizontal")
@@ -34,14 +35,15 @@
         center_point_value = -(center_point / cross[2])
     return center_point_value
 
 
 def calculate_angles(df):
     """
     Calculates the Mediolateral and Dorsoventral angles for a series of predictions
+    
     :param df: The dataframe containing the predictions
     :type df: pandas.DataFrame
     :return: a list of calculated ML and DV angles
     :rtype: list[float], list[float]
     """
     DV_list, ML_list = [], []
     for alignment in df.iterrows():
@@ -75,16 +77,20 @@
         ML_angle = np.mean(ML_list)
     elif method == "weighted_mean":
         df_center = depths
         if species == "mouse":
             min, max = 0, 528
         elif species == "rat":
             min, max = 0, 1024
-        weighted_accuracy = plane_alignment.make_gaussian_weights(min, max)
+        if len(df_center) > 2:
+            weighted_accuracy = plane_alignment.make_gaussian_weights(max)
+        else:
+            weighted_accuracy = [1.0] * len(df_center)
         weighted_accuracy = [weighted_accuracy[int(y)] for y in df_center]
+        print(weighted_accuracy)
         DV_angle = np.average(DV_list, weights=weighted_accuracy)
         ML_angle = np.average(ML_list, weights=weighted_accuracy)
     else:
         raise ValueError("method must be one of 'mean' or 'weighted_mean'")
     return DV_angle, ML_angle
```

### Comparing `DeepSlice-1.0.6/DeepSlice/coord_post_processing/depth_estimation.py` & `DeepSlice-1.1.0/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from .plane_alignment_functions import plane_alignment
 
 
 def calculate_brain_center_depth(section):
     """
     Calculates the depth of the brain center for a given section
+
     :param section: the section coordinates as an array consisting of Oxyz,Uxyz,Vxyz 
     :type section: np.array
     :return: the depth of the brain center
     :rtype: float
     """
     cross, k = plane_alignment.find_plane_equation(section)
     translated_volume = np.array((456, 0, 320))
@@ -19,14 +20,15 @@
     depth = -(linear_point / cross[1])
     return depth
 
 
 def calculate_brain_center_depths(predictions):
     """
     Calculates the depths of the brain center for a series of predictions
+    
     :param predictions: dataframe of predictions
     :type predictions: pandas.DataFrame
     :return: a list of depths
     :rtype: list[float]
     """
     depths = []
     for prediction in predictions[
```

### Comparing `DeepSlice-1.0.6/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `DeepSlice-1.1.0/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import random
 from statistics import mean
 import numpy as np
+from scipy.stats import norm
+
 import math
 
 
 def find_plane_equation(plane):
     """
     Finds the plane equation of a plane
     :param plane: the plane to find the equation of
@@ -90,36 +91,19 @@
             [aa + bb - cc - dd, 2 * (bc - ad), 2 * (bd + ac)],
             [2 * (bc + ad), aa + cc - bb - dd, 2 * (cd - ab)],
             [2 * (bd - ac), 2 * (cd + ab), aa + dd - bb - cc],
         ]
     )
 
 
-def make_gaussian_weights(mini, maxi):
-    """
-    Generates a list of weights for a gaussian distribution
-    :param mini: the minimum value of the distribution
-    :type mini: float
-    :param maxi: the maximum value of the distribution
-    :type maxi: float
-    :returns: a list of weights
-    :rtype: list
-    """
-    weights = []
-    center = mean((mini, maxi))
-    quartile = (maxi - mini) / 4
-    while len(weights) < ((maxi - mini) / 2):
-        weights.append(random.gauss(center, quartile))
-    weights = [max(x, mini) for x in weights]
-    weights = [min(x, maxi) for x in weights]
-    weights = [x - center if x > center else x for x in weights]
-    weights = sorted(weights)
-    weights_rev = sorted(weights, reverse=True)
-    weights.extend(weights_rev)
-    return [x / max(weights) for x in weights]
+
+def make_gaussian_weights(size):
+    x = np.linspace(-np.pi, np.pi, size)
+    weights = np.exp(-(x ** 2) / 2) / np.sqrt(2 * np.pi)
+    return weights
 
 
 def get_axis(m, translation_vector, direction, plane_of_section=None, atlas="AMBA"):
     """
     :param m: the matrix to rotate
     :type m: 3x3 :any:`numpy.ndarray`
     :param translation_vector: the translation vector to apply
```

### Comparing `DeepSlice-1.0.6/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `DeepSlice-1.1.0/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,84 +5,110 @@
 from .depth_estimation import calculate_brain_center_depths
 from .plane_alignment_functions import plane_alignment
 
 def trim_mean(arr: np.array, percent: int) -> float:
     """"
     Calculates the trimmed mean of an array, sourced from:
     https://gist.github.com/StuffbyYuki/6f25f9f2f302cb5c1e82e4481016ccde
+
     :param arr: the array to calculate the trimmed mean of
     :type arr: np.array
     :param percent: the percentage of values to trim
     :type percent: int
     :return: the trimmed mean
     :rtype: float
     """
     n = len(arr)
     k = int(round(n * (float(percent) / 100) / 2))
     return np.mean(arr[k + 1 : n - k])
 
 
 def calculate_average_section_thickness(
-    section_numbers: List[Union[int, float]], section_depth: List[Union[int, float]]
+    section_numbers: List[Union[int, float]], section_depth: List[Union[int, float]], method="weighted",
+    species="mouse"
 ) -> float:
     """
     Calculates the average section thickness for a series of predictions
+
     :param section_numbers: List of section numbers
     :param section_depth: List of section depths
     :type section_numbers: List[int, float]
     :type section_depth: List[int, float]
     :return: the average section thickness
     :rtype: float
     """
     # inter section number differences
     number_spacing = section_numbers[:-1].values - section_numbers[1:].values
     # inter section depth differences
     depth_spacing = section_depth[:-1] - section_depth[1:]
     # dividing depth spacing by number spacing allows us to control for missing sections
     min = 0
     max = np.max(section_numbers)
-    weighted_accuracy = plane_alignment.make_gaussian_weights(min, max + 1)
-    weighted_accuracy = [weighted_accuracy[int(y)] for y in section_numbers]
+    if species == "mouse":
+        min, max = 0, 528
+    elif species == "rat":
+        min, max = 0, 1024
+    if method == "weighted":
+        weighted_accuracy = plane_alignment.make_gaussian_weights(max + 1)
+        weighted_accuracy = [weighted_accuracy[int(y)] for y in section_numbers]
+    elif method == None:
+        weighted_accuracy = [1 for y in section_numbers]
+
     section_thicknesses = depth_spacing / number_spacing
+    if len(section_numbers) <= 2:
+      weighted_accuracy = [1, 1]
     average_thickness = np.average(section_thicknesses, weights = weighted_accuracy[1:])
     return average_thickness
 
 
 def ideal_spacing(
     section_numbers: List[Union[int, float]],
     section_depth: List[Union[int, float]],
     average_thickness: Union[int, float],
+    method = "weighted",
+    species = "mouse"
 ) -> float:
     """
     Calculates the ideal spacing for a series of predictions
+
     :param section_numbers: List of section numbers
     :param section_depth: List of section depths
     :param average_thickness: The average section thickness
     :type section_numbers: List[int, float]
     :type section_depth: List[int, float]
     :type average_thickness: int, float
     :return: the ideal spacing
     :rtype: float
     """
     # unaligned voxel position of section numbers (evenly spaced depths)
     index_spaced_depth = section_numbers * average_thickness
     # average distance between the depths and the evenly spaced depths
     min = 0
     max = np.max(section_numbers)
-    weighted_accuracy = plane_alignment.make_gaussian_weights(min, max + 1)
-    weighted_accuracy = [weighted_accuracy[int(y)] for y in section_numbers]
+    if species == "mouse":
+        min, max = 0, 528
+    elif species == "rat":
+        min, max = 0, 1024
+    if method == "weighted":
+        weighted_accuracy = plane_alignment.make_gaussian_weights(max + 1)
+        weighted_accuracy = [weighted_accuracy[int(y)] for y in section_numbers]
+    elif method == None:
+        weighted_accuracy = [1 for y in section_numbers]
+    if len(section_numbers) <= 2:
+        weighted_accuracy = [0.5, 0.5]
     distance_to_ideal = np.average(section_depth - index_spaced_depth, weights = weighted_accuracy)
     # adjust the evenly spaced depths to minimise their distance to the predicted depths
     ideal_index_spaced_depth = index_spaced_depth + distance_to_ideal
     return ideal_index_spaced_depth
 
 
 def determine_direction_of_indexing(depth: List[Union[int, float]]) -> str:
     """
     Determines the direction of indexing for a series of predictions
+
     :param depth: List of depths sorted by section index
     :type depth: List[int, float]
     :return: the direction of indexing
     :rtype: str
     """
 
     if trim_mean(depth[1:] - depth[:-1], 10) > 0:
@@ -91,14 +117,15 @@
         direction = "caudal-rostro"
     return direction
 
 
 def enforce_section_ordering(predictions):
     """
     Ensures that the predictions are ordered by section number
+
     :param predictions: dataframe of predictions
     :type predictions: pandas.DataFrame
     :return: the input dataframe ordered by section number
     :rtype: pandas.DataFrame
     """
     predictions = predictions.sort_values(by=["nr"], ascending=True).reset_index(drop=True)
     if len(predictions) == 1:
@@ -122,19 +149,20 @@
         temp = temp.sort_values(by=["depths"], ascending=ascending).reset_index(
             drop=True
         )
         predictions["oy"] = temp["oy"]
     return predictions
 
 
-def space_according_to_index(predictions, section_thickness = None, voxel_size = None):
+def space_according_to_index(predictions, section_thickness = None, voxel_size = None, suppress = False, species = "mouse"):
     """
     Space evenly according to the section indexes, if these indexes do not represent the precise order in which the sections were
     cut, this will lead to less accurate predictions. Section indexes must account for missing sections (ie, if section 3 is missing
     indexes must be 1, 2, 4).
+
     :param predictions: dataframe of predictions
     :type predictions: pandas.DataFrame
     :return: the input dataframe with evenly spaced sections
     :rtype: pandas.DataFrame
     """
     if voxel_size == None:
         raise ValueError("voxel_size must be specified")
@@ -149,29 +177,32 @@
         )
     else:
         predictions = enforce_section_ordering(predictions)
         depths = calculate_brain_center_depths(predictions)
         depths = np.array(depths)
         if not section_thickness:
             section_thickness = calculate_average_section_thickness(
-                predictions["nr"], depths
+                predictions["nr"], section_depth = depths, species=species
             )
-            print(f'predicted thickness is {section_thickness * voxel_size}µm')
+            if not suppress:
+                print(f'predicted thickness is {section_thickness * voxel_size}µm')
         else:
-            print(f'specified thickness is {section_thickness * voxel_size}µm')
+            if not suppress:
+                print(f'specified thickness is {section_thickness * voxel_size}µm')
 
-        calculated_spacing = ideal_spacing(predictions["nr"], depths, section_thickness)
+        calculated_spacing = ideal_spacing(predictions["nr"], depths, section_thickness, None, species)
         distance_to_ideal = calculated_spacing - depths
         predictions["oy"] = predictions["oy"] + distance_to_ideal
     return predictions
 
 
 def number_sections(filenames: List[str], legacy=False) -> List[int]:
     """
     returns the section numbers of filenames
+
     :param filenames: list of filenames
     :type filenames: list[str]
     :return: list of section numbers
     :rtype: list[int]
     """
     filenames = [filename.split("\\")[-1] for filename in filenames]
     section_numbers = []
@@ -193,14 +224,15 @@
         raise ValueError("No section numbers found in filenames")
     return section_numbers
 
 
 def set_bad_sections_util(df: pd.DataFrame, bad_sections: List[str]) -> pd.DataFrame:
     """
     Sets the damaged sections and sections which deepslice may not perform well on for a series of predictions
+    
     :param bad_sections: List of bad sections
     :param df: dataframe of predictions
     :type bad_sections: List[int]
     :type df: pandas.DataFrame
     :return: the input dataframe with bad sections labeled as such
     :rtype: pandas.DataFrame
     """
```

### Comparing `DeepSlice-1.0.6/DeepSlice/main.py` & `DeepSlice-1.1.0/DeepSlice/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from .metadata import metadata_loader
 
 
 
 
 class DSModel:
     def __init__(self, species):
+        """Initialises a DeepSlice model for a given species
+        :param species: the species of the brain to be processed, must be one of "mouse", "rat"
+        :type species: str
+        """
         self.species = species
 
         self.config, self.metadata_path = metadata_loader.load_config()
         xception_weights =   metadata_loader.get_data_path(self.config["weight_file_paths"]["xception_imagenet"], self.metadata_path)
         weights =    metadata_loader.get_data_path(self.config["weight_file_paths"][self.species]["primary"], self.metadata_path)
         try:
           self.model = neural_network.initialise_network(xception_weights, weights)
@@ -75,14 +79,15 @@
 
         self.predictions = predictions
         self.image_directory = image_directory
 
     def set_bad_sections(self, bad_sections: list):
         """
         sets the bad sections for a given brain. Must be run after predict()
+
         :param bad_sections: A list of bad sections to ignore when calculating angles and spacing
         :type bad_sections: list
         """
         self.predictions = spacing_and_indexing.set_bad_sections_util(
             self.predictions, bad_sections
         )
 
@@ -90,30 +95,32 @@
         """
         reorders the section depths (oy) in the predictions such that they align with the section indexes
         """
         self.predictions = spacing_and_indexing.enforce_section_ordering(
             self.predictions
         )
 
-    def enforce_index_spacing(self, section_thickness:Union[int, float] = None):
+    def enforce_index_spacing(self, section_thickness:Union[int, float] = None, suppress = False):
         """
         Space evenly according to the section indexes, if these indexes do not represent the precise order in which the sections were
         cut, this will lead to less accurate predictions. Section indexes must account for missing sections (ie, if section 3 is missing
         indexes must be 1, 2, 4).
+
         :param section_thickness: the thickness of the sections in microns, defaults to None
         :type section_thickness: Union[int, float], optional
         """
         voxel_size = self.config["target_volumes"][self.species]["voxel_size_microns"]
         self.predictions = spacing_and_indexing.space_according_to_index(
-            self.predictions, section_thickness = section_thickness, voxel_size = voxel_size
+            self.predictions, section_thickness = section_thickness, voxel_size = voxel_size, suppress = suppress, species=self.species
         )
 
     def adjust_angles(self, ML: Union[int, float], DV: Union[int, float]):
         """
         Adjusts the Mediolateral (ML) and Dorsoventral (DV) angles of all sections to the specified values.
+
         :param ML: the Mediolateral angle to set
         :param DV: the Dorsoventral angle to set
         :type ML: [int, float]
         :type DV: [int, float]
         """
         self.predictions = angle_methods.set_angles(self.predictions, ML, DV)
 
@@ -127,33 +134,37 @@
                 self.predictions, method, self.species
             )
             
 
     def load_QUINT(self, filename):
         """
         Load a QUINT compatible JSON or XML.
+
         :param filename: the name of the file to load
         :type filename: str
         """
         if filename.lower().endswith('.json'):
             predictions, target = QuickNII_functions.read_QUINT_JSON(filename)
             if target == "ABA_Mouse_CCFv3_2017_25um.cutlas" and self.species!='mouse':
                     self.species = 'mouse'
                     print('Switching to a mouse model')
             elif target == "WHS_Rat_v4_39um.cutlas" and self.species!='rat':
                 self.species = 'rat'
                 print("switching to a rat model")
         elif filename.lower().endswith('.xml'):
             predictions = QuickNII_functions.read_QuickNII_XML(filename)
+        else:
+            raise ValueError('File must be a JSON or XML')
         self.predictions = predictions
         
 
     def save_predictions(self, filename):
         """
         Save the predictions to a QuickNII compatible JSON file.
+
         :param filename: the name of the file to save to
         :type filename: str
         """
         target  = self.config["target_volumes"][self.species]["name"]
         aligner = self.config["DeepSlice_version"]["prerelease"]
         self.predictions.to_csv(filename + ".csv", index=False)
         QuickNII_functions.write_QUINT_JSON(
```

### Comparing `DeepSlice-1.0.6/DeepSlice/metadata/config.json` & `DeepSlice-1.1.0/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.0.6/DeepSlice/metadata/metadata_loader.py` & `DeepSlice-1.1.0/DeepSlice/metadata/metadata_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 import requests
 import os
 
 
 def load_config() -> dict:
     """
     Loads the config file
+
     :return: the config file
     :rtype: dict
     """
     path = str(Path(__file__).parent) + os.sep
     with open(path + "config.json", "r") as f:
         config = json.loads(f.read())
     return config, path
 
 
 def download_file(url: str, path: str):
     """
     Downloads a file from a url to a path
+
     :param url: the url of the file to download
     :type url: str
     :param path: the path to save the file to
     :type path: str
     """
     print("Downloading file from " + url + " to " + path)
     r = requests.get(url, allow_redirects=True)
     open(path, "wb").write(r.content)
 
 def get_data_path(url_path_dict, path):
     """
     If the data is not present, download it from the DeepSlice github. Else return the path to the data.
+    
     :param url_path_dict: a dictionary of a url and path to the data
     :type url_path_dict: dict
     :param path: the path to the DeepSlice metadata directory
     :type path: str
     :return: the path to the data
     :rtype: str
     """
```

### Comparing `DeepSlice-1.0.6/DeepSlice/neural_network/neural_network.py` & `DeepSlice-1.1.0/DeepSlice/neural_network/neural_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,49 +13,51 @@
 import imghdr
 import struct
 
 
 def gray_scale(img: np.ndarray) -> np.ndarray:
     """
     Convert the image to grayscale
+
     :param img: The image to convert
     :type img: numpy.ndarray
     :return: The converted image
     :rtype: numpy.ndarray
     """
     img = rgb2gray(img).reshape(299, 299, 1)
     return img
 
 
 def initialise_network(xception_weights: str, weights: str) -> Sequential:
     """
     Initialise a neural network with the given weights
+
     :param weights: The weights for the network
     :type weights: list
     :return: The initialised neural network
     :rtype: keras.models.Sequential
     """
     base_model = Xception(include_top=True, weights=xception_weights)
     base_model._layers.pop()
     base_model._layers.pop()
-    inputs = Input(shape=(299, 299, 3))
-    base_model_layer = base_model(inputs, training=True)
-    dense1_layer = Dense(256, activation="relu")(base_model_layer)
-    dense2_layer = Dense(256, activation="relu")(dense1_layer)
-    output_layer = Dense(9, activation="linear")(dense2_layer)
-    model = Model(inputs=inputs, outputs=output_layer)
+    model = Sequential()
+    model.add(base_model)
+    model.add(Dense(256, activation="relu"))
+    model.add(Dense(256, activation="relu"))
+    model.add(Dense(9, activation="linear"))
     if weights != None:
         model.load_weights(weights)
     return model
 
 
 
 def load_images(image_path: str) -> np.ndarray:
     """
     Load the images from the given path
+
     :param image_path: The path to the images
     :type image_path: str
     :return: an Image generator for the found images
     :rtype: keras.preprocessing.image.ImageDataGenerator
     """
     if not os.path.isdir(image_path):
         raise ValueError("The path provided is not a directory")
@@ -95,14 +97,15 @@
     image_generator: ImageDataGenerator,
     primary_weights: str,
     secondary_weights: str,
     ensemble: bool = False,
 ):
     """
     Predict the image alignments
+    
     :param model: The model to use for prediction
     :param image_generator: The image generator to use for prediction
     :type model: keras.models.Sequential
     :type image_generator: keras.preprocessing.image.ImageDataGenerator
     :return: The predicted alignments
     :rtype: list
     """
```

### Comparing `DeepSlice-1.0.6/DeepSlice/read_and_write/QuickNII_functions.py` & `DeepSlice-1.1.0/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         },
     )
 
 
 def read_QuickNII_XML(filename: str) -> pd.DataFrame:
     """
     Converts a QuickNII XML to a pandas dataframe
+
     :param xml: The path to the QuickNII XML
     :type xml: str
     :return: A pandas dataframe
     :rtype: pd.DataFrame
     """
     df = pd.read_xml(filename)
     # split the anchoring string into separate columns
@@ -120,14 +121,15 @@
     with open(filename + ".json", "w") as outfile:
         json.dump(QUINT_json, outfile)
 
 
 def read_QUINT_JSON(filename: str) -> pd.DataFrame:
     """
     Converts a QUINT JSON to a pandas dataframe
+    
     :param json: The path to the QUINT JSON
     :type json: str
     :return: A pandas dataframe
     :rtype: pd.DataFrame
     """
     with open(filename, "r") as f:
         data = json.load(f)
```

### Comparing `DeepSlice-1.0.6/DeepSlice.egg-info/PKG-INFO` & `DeepSlice-1.1.0/DeepSlice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.0.6
+Version: 1.1.0
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.0.6.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.0.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -41,20 +41,20 @@
 
 
 <a name='Installation'></a> 
 <h1> Installation </h1>
 <!-- This h2 must be bold  -->
 
 <h2 style="font-weight: bold; text-decoration: underline"> From PIP  </h2>
-This is the easy and recommended way to install DeepSlice. 
+This is the easy and recommended way to install DeepSlice. Make sure your env has Python 3.7 installed and then simply:
 
 ```bash
 pip install DeepSlice
 ```
-And you're ready to go! 🚀
+And you're ready to go! 🚀 Check out the PyPi package [here](https://pypi.org/project/DeepSlice/)
 
 <h2 style="font-weight: bold; text-decoration: underline"> From Source </h2>
 
 **First** To use DeepSlice you must have python3.7 installed. In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
 
 
 **Second** Once anaconda is installed, cd into your cloned DeepSlice directory, then cd into the 'conda_environments' directory, and use our premade environment files to setup your system.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.0.6 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.0 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.0.6.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.0.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
@@ -27,16 +27,18 @@
 allow you to upload your dataset and download the aligned results. The web
 interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
 [Installation: How to install DeepSlice](#installation) ## [Usage: How to align
 using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
 (examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ****** Installation ******
 ***** From PIP *****
-This is the easy and recommended way to install DeepSlice. ```bash pip install
-DeepSlice ``` And you're ready to go! ð
+This is the easy and recommended way to install DeepSlice. Make sure your env
+has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
+you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
+project/DeepSlice/)
 ***** From Source *****
 **First** To use DeepSlice you must have python3.7 installed. In order to
 easily install all the dependancies we recommend using [Anaconda](https://
 www.anaconda.com/products/individual "Anaconda Installation Files"). **Second**
 Once anaconda is installed, cd into your cloned DeepSlice directory, then cd
 into the 'conda_environments' directory, and use our premade environment files
 to setup your system. ``` cd DeepSlice/conda_environments ``` * **CPU
```

### Comparing `DeepSlice-1.0.6/DeepSlice.egg-info/SOURCES.txt` & `DeepSlice-1.1.0/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.0.6/LICENSE` & `DeepSlice-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.0.6/PKG-INFO` & `DeepSlice-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.0.6
+Version: 1.1.0
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.0.6.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.0.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -41,20 +41,20 @@
 
 
 <a name='Installation'></a> 
 <h1> Installation </h1>
 <!-- This h2 must be bold  -->
 
 <h2 style="font-weight: bold; text-decoration: underline"> From PIP  </h2>
-This is the easy and recommended way to install DeepSlice. 
+This is the easy and recommended way to install DeepSlice. Make sure your env has Python 3.7 installed and then simply:
 
 ```bash
 pip install DeepSlice
 ```
-And you're ready to go! 🚀
+And you're ready to go! 🚀 Check out the PyPi package [here](https://pypi.org/project/DeepSlice/)
 
 <h2 style="font-weight: bold; text-decoration: underline"> From Source </h2>
 
 **First** To use DeepSlice you must have python3.7 installed. In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
 
 
 **Second** Once anaconda is installed, cd into your cloned DeepSlice directory, then cd into the 'conda_environments' directory, and use our premade environment files to setup your system.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.0.6 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.0 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.0.6.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.0.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
@@ -27,16 +27,18 @@
 allow you to upload your dataset and download the aligned results. The web
 interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
 [Installation: How to install DeepSlice](#installation) ## [Usage: How to align
 using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
 (examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ****** Installation ******
 ***** From PIP *****
-This is the easy and recommended way to install DeepSlice. ```bash pip install
-DeepSlice ``` And you're ready to go! ð
+This is the easy and recommended way to install DeepSlice. Make sure your env
+has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
+you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
+project/DeepSlice/)
 ***** From Source *****
 **First** To use DeepSlice you must have python3.7 installed. In order to
 easily install all the dependancies we recommend using [Anaconda](https://
 www.anaconda.com/products/individual "Anaconda Installation Files"). **Second**
 Once anaconda is installed, cd into your cloned DeepSlice directory, then cd
 into the 'conda_environments' directory, and use our premade environment files
 to setup your system. ``` cd DeepSlice/conda_environments ``` * **CPU
```

### Comparing `DeepSlice-1.0.6/README.md` & `DeepSlice-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
 
 <a name='Installation'></a> 
 <h1> Installation </h1>
 <!-- This h2 must be bold  -->
 
 <h2 style="font-weight: bold; text-decoration: underline"> From PIP  </h2>
-This is the easy and recommended way to install DeepSlice. 
+This is the easy and recommended way to install DeepSlice. Make sure your env has Python 3.7 installed and then simply:
 
 ```bash
 pip install DeepSlice
 ```
-And you're ready to go! 🚀
+And you're ready to go! 🚀 Check out the PyPi package [here](https://pypi.org/project/DeepSlice/)
 
 <h2 style="font-weight: bold; text-decoration: underline"> From Source </h2>
 
 **First** To use DeepSlice you must have python3.7 installed. In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
 
 
 **Second** Once anaconda is installed, cd into your cloned DeepSlice directory, then cd into the 'conda_environments' directory, and use our premade environment files to setup your system.
```

#### html2text {}

```diff
@@ -17,16 +17,18 @@
 allow you to upload your dataset and download the aligned results. The web
 interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
 [Installation: How to install DeepSlice](#installation) ## [Usage: How to align
 using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
 (examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ****** Installation ******
 ***** From PIP *****
-This is the easy and recommended way to install DeepSlice. ```bash pip install
-DeepSlice ``` And you're ready to go! ð
+This is the easy and recommended way to install DeepSlice. Make sure your env
+has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
+you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
+project/DeepSlice/)
 ***** From Source *****
 **First** To use DeepSlice you must have python3.7 installed. In order to
 easily install all the dependancies we recommend using [Anaconda](https://
 www.anaconda.com/products/individual "Anaconda Installation Files"). **Second**
 Once anaconda is installed, cd into your cloned DeepSlice directory, then cd
 into the 'conda_environments' directory, and use our premade environment files
 to setup your system. ``` cd DeepSlice/conda_environments ``` * **CPU
```

### Comparing `DeepSlice-1.0.6/setup.py` & `DeepSlice-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.0.6',
+    version='1.1.0',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.0.6.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.0.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
         'tensorflow==1.15.0',
         'h5py==2.10.0',
```

