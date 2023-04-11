# Comparing `tmp/needle-shape-sensing-0.8.2.tar.gz` & `tmp/needle-shape-sensing-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\needle-shape-sensing-0.8.2.tar", last modified: Fri Mar 31 20:14:31 2023, max compression
+gzip compressed data, was "dist\needle-shape-sensing-0.8.3.tar", last modified: Tue Apr 11 02:33:31 2023, max compression
```

## Comparing `needle-shape-sensing-0.8.2.tar` & `needle-shape-sensing-0.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 20:14:31.000000 needle-shape-sensing-0.8.2/
--rw-rw-rw-   0        0        0     1072 2021-08-13 20:31:43.000000 needle-shape-sensing-0.8.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-03-31 20:14:30.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/
--rw-rw-rw-   0        0        0    12846 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/cost_functions.py
--rw-rw-rw-   0        0        0     1452 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/fbg_signal_processing.py
--rw-rw-rw-   0        0        0     9347 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/geometry.py
--rw-rw-rw-   0        0        0    22289 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/intrinsics.py
--rw-rw-rw-   0        0        0    24249 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/numerical.py
-drwxrwxrwx   0        0        0        0 2023-03-31 20:14:31.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/
--rw-rw-rw-   0        0        0      588 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/config.py
--rw-rw-rw-   0        0        0     1278 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/geometry.py
--rw-rw-rw-   0        0        0    13480 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/intrinsics.py
--rw-rw-rw-   0        0        0     8017 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/numerical.py
--rw-rw-rw-   0        0        0      106 2022-12-07 21:25:38.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/__init__.py
--rw-rw-rw-   0        0        0    41393 2023-03-31 20:12:29.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/sensorized_needles.py
--rw-rw-rw-   0        0        0    19564 2023-03-31 17:59:26.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/shape_sensing.py
-drwxrwxrwx   0        0        0        0 2023-03-31 20:14:31.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/
--rw-rw-rw-   0        0        0     1576 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/geometry.py
--rw-rw-rw-   0        0        0    12463 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/intrinsics.py
--rw-rw-rw-   0        0        0     8692 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/numerical.py
--rw-rw-rw-   0        0        0       96 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/__init__.py
--rw-rw-rw-   0        0        0      214 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.2/needle_shape_sensing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 20:14:31.000000 needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-31 20:14:29.000000 needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1678 2023-03-31 20:14:29.000000 needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-03-31 20:14:29.000000 needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/requires.txt
--rw-rw-rw-   0        0        0      935 2023-03-31 20:14:30.000000 needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       21 2023-03-31 20:14:29.000000 needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1678 2023-03-31 20:14:31.000000 needle-shape-sensing-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1089 2021-08-13 16:01:29.000000 needle-shape-sensing-0.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 20:14:31.000000 needle-shape-sensing-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-03-31 20:13:21.000000 needle-shape-sensing-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:33:31.000000 needle-shape-sensing-0.8.3/
+-rw-rw-rw-   0        0        0     1072 2021-08-13 20:31:43.000000 needle-shape-sensing-0.8.3/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 02:33:30.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/
+-rw-rw-rw-   0        0        0    12846 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/cost_functions.py
+-rw-rw-rw-   0        0        0     1452 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/fbg_signal_processing.py
+-rw-rw-rw-   0        0        0     9347 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/geometry.py
+-rw-rw-rw-   0        0        0    22289 2023-03-31 17:18:02.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/intrinsics.py
+-rw-rw-rw-   0        0        0    24248 2023-04-11 02:33:25.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/numerical.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:33:30.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/
+-rw-rw-rw-   0        0        0      588 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/config.py
+-rw-rw-rw-   0        0        0     1278 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/geometry.py
+-rw-rw-rw-   0        0        0    13480 2023-01-03 18:44:04.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/intrinsics.py
+-rw-rw-rw-   0        0        0     8017 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/numerical.py
+-rw-rw-rw-   0        0        0      106 2022-12-07 21:25:38.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/__init__.py
+-rw-rw-rw-   0        0        0    41396 2023-04-11 02:33:25.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/sensorized_needles.py
+-rw-rw-rw-   0        0        0    19677 2023-04-11 02:33:25.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/shape_sensing.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:33:31.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/
+-rw-rw-rw-   0        0        0     1576 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/geometry.py
+-rw-rw-rw-   0        0        0    12463 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/intrinsics.py
+-rw-rw-rw-   0        0        0     8692 2023-03-02 20:35:13.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/numerical.py
+-rw-rw-rw-   0        0        0       96 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0      214 2022-12-01 20:57:10.000000 needle-shape-sensing-0.8.3/needle_shape_sensing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:33:30.000000 needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:33:29.000000 needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1678 2023-04-11 02:33:29.000000 needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-04-11 02:33:29.000000 needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      935 2023-04-11 02:33:29.000000 needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       21 2023-04-11 02:33:29.000000 needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1678 2023-04-11 02:33:31.000000 needle-shape-sensing-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2021-08-13 16:01:29.000000 needle-shape-sensing-0.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:33:31.000000 needle-shape-sensing-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-04-11 02:33:25.000000 needle-shape-sensing-0.8.3/setup.py
```

### Comparing `needle-shape-sensing-0.8.2/LICENSE.txt` & `needle-shape-sensing-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/cost_functions.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/cost_functions.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/fbg_signal_processing.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/fbg_signal_processing.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/geometry.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/geometry.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/intrinsics.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/intrinsics.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/numerical.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/numerical.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         # else
 
         # normalize the weights
         weights = weights / np.sum( weights )
 
         # compute the weighted-mean curvature from the measurements
         data_ins_w = data_ins * weights.reshape( -1, 1 )
-        curvature = data_ins_w.mean( axis=0 )
+        curvature = data_ins_w.sum( axis=0 )
 
         return curvature
 
     # constant_curvature
 
     def singlebend_singlelayer_k0(
             self, k_c_0: float, w_init_0: np.ndarray, data: np.ndarray, L: float,
```

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/config.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/config.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/geometry.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/geometry.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/intrinsics.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/intrinsics.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/pytorch/numerical.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/pytorch/numerical.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/sensorized_needles.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/sensorized_needles.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     def num_signals( self ):
         return self.num_channels * self.num_activeAreas
 
     # num_signals
 
     @property
     def sensor_calibrated( self ):
-        return all( self.ref_wavelengths >= 0 )
+        return np.all( self.ref_wavelengths >= 0 )
 
     # sensor_calibrated
 
     @property
     def sensor_location( self ):
         return self._sensor_location
```

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/shape_sensing.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/shape_sensing.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,17 @@
                         self.current_curvatures.T, self.current_depth )
                 curvature = np.append( curvature, 0 )  # ensure 3 vector
                 pmat, Rmat = intrinsics.ConstantCurvature.shape( s, curvature )
 
                 pmat = pmat @ R_init.T
                 Rmat = R_init @ Rmat
 
+                self.current_winit = curvature
+                self.current_kc = [np.linalg.norm(curvature)]
+
             # if
             elif self.current_shapetype == intrinsics.SHAPETYPE.SINGLEBEND_SINGLELAYER:
                 # get parameters
                 kc_i = args[ 0 ]
                 if len( args ) > 1:
                     w_init_i = args[ 1 ]
                     if not isinstance( w_init_i, np.ndarray ) or len( w_init_i ) != 3:
```

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/geometry.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/geometry.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/intrinsics.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/intrinsics.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing/tensorflow/numerical.py` & `needle-shape-sensing-0.8.3/needle_shape_sensing/tensorflow/numerical.py`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/PKG-INFO` & `needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: needle-shape-sensing
-Version: 0.8.2
+Version: 0.8.3
 Summary: Needle Shape Sensing library
 Home-page: http://pypi.python.org/pypi/needle-shape-sensing/
 Author: Dimitri Lezcano
 Author-email: dlezcan1@jhu.edu
 License: LICENSE.txt
 Description: # python-needle-shape-sensing
         Author: Dimitri Lezcano
```

### Comparing `needle-shape-sensing-0.8.2/needle_shape_sensing.egg-info/SOURCES.txt` & `needle-shape-sensing-0.8.3/needle_shape_sensing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/PKG-INFO` & `needle-shape-sensing-0.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: needle-shape-sensing
-Version: 0.8.2
+Version: 0.8.3
 Summary: Needle Shape Sensing library
 Home-page: http://pypi.python.org/pypi/needle-shape-sensing/
 Author: Dimitri Lezcano
 Author-email: dlezcan1@jhu.edu
 License: LICENSE.txt
 Description: # python-needle-shape-sensing
         Author: Dimitri Lezcano
```

### Comparing `needle-shape-sensing-0.8.2/README.md` & `needle-shape-sensing-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `needle-shape-sensing-0.8.2/setup.py` & `needle-shape-sensing-0.8.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
         name='needle-shape-sensing',
-        version='0.8.2',
+        version='0.8.3',
         author='Dimitri Lezcano',
         author_email='dlezcan1@jhu.edu',
         packages=find_packages(),
         url='http://pypi.python.org/pypi/needle-shape-sensing/',
         license='LICENSE.txt',
         description='Needle Shape Sensing library',
         long_description=open( 'README.md' ).read(),
```

