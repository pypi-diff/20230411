# Comparing `tmp/SeanFunctions-0.4.1.tar.gz` & `tmp/SeanFunctions-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeanFunctions-0.4.1.tar", last modified: Mon Apr 10 18:03:40 2023, max compression
+gzip compressed data, was "SeanFunctions-0.4.3.tar", last modified: Tue Apr 11 18:04:13 2023, max compression
```

## Comparing `SeanFunctions-0.4.1.tar` & `SeanFunctions-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-10 18:03:40.860426 SeanFunctions-0.4.1/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/.gitignore
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.4.1/LICENSE
--rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/MANIFEST.in
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-10 18:03:40.860144 SeanFunctions-0.4.1/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.4.1/README.md
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-04-10 18:01:41.000000 SeanFunctions-0.4.1/pyproject.toml
--rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-04-10 18:03:40.860491 SeanFunctions-0.4.1/setup.cfg
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-10 18:03:40.855100 SeanFunctions-0.4.1/src/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-10 18:03:40.858525 SeanFunctions-0.4.1/src/SeanFunctions/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-10 18:03:40.859806 SeanFunctions-0.4.1/src/SeanFunctions/Data/
--rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/src/SeanFunctions/Data/NeutronScatteringLengths.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/src/SeanFunctions/__init__.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     3056 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/src/SeanFunctions/fitting.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     8983 2023-04-10 18:01:34.000000 SeanFunctions-0.4.1/src/SeanFunctions/math.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     4166 2023-01-14 21:57:03.000000 SeanFunctions-0.4.1/src/SeanFunctions/scattering.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)      196 2023-04-10 18:03:40.000000 SeanFunctions-0.4.1/src/SeanFunctions/version.py
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-10 18:03:40.859130 SeanFunctions-0.4.1/src/SeanFunctions.egg-info/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-10 18:03:40.000000 SeanFunctions-0.4.1/src/SeanFunctions.egg-info/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-04-10 18:03:40.000000 SeanFunctions-0.4.1/src/SeanFunctions.egg-info/SOURCES.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-04-10 18:03:40.000000 SeanFunctions-0.4.1/src/SeanFunctions.egg-info/dependency_links.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-04-10 18:03:40.000000 SeanFunctions-0.4.1/src/SeanFunctions.egg-info/top_level.txt
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.122202 SeanFunctions-0.4.3/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/.gitignore
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.4.3/LICENSE
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/MANIFEST.in
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-11 18:04:13.121946 SeanFunctions-0.4.3/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.4.3/README.md
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-04-11 18:00:46.000000 SeanFunctions-0.4.3/pyproject.toml
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-04-11 18:04:13.122260 SeanFunctions-0.4.3/setup.cfg
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.117347 SeanFunctions-0.4.3/src/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.120213 SeanFunctions-0.4.3/src/SeanFunctions/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.121605 SeanFunctions-0.4.3/src/SeanFunctions/Data/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/__init__.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     3680 2023-04-11 18:03:36.000000 SeanFunctions-0.4.3/src/SeanFunctions/fitting.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     8986 2023-04-10 21:00:12.000000 SeanFunctions-0.4.3/src/SeanFunctions/math.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     4166 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/scattering.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      196 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions/version.py
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.120913 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/top_level.txt
```

### Comparing `SeanFunctions-0.4.1/LICENSE` & `SeanFunctions-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.1/PKG-INFO` & `SeanFunctions-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.4.1
+Version: 0.4.3
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.4.1/pyproject.toml` & `SeanFunctions-0.4.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SeanFunctions"
-version = "0.4.1"
+version = "0.4.3"
 # dynamic = ["version"]
 authors = [
   { name="Sean Fayfar", email="sfayfar@gmail.com" },
 ]
 description = "Collection of useful python functions"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions/Data/AtomicFormFactorConstants.csv` & `SeanFunctions-0.4.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions/Data/NeutronScatteringLengths.csv` & `SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv` & `SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions/fitting.py` & `SeanFunctions-0.4.3/src/SeanFunctions/fitting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import lmfit as lm
 
 
-def fitPeak(data,xleft,xright,peakType='Gaussian',constant=False):
+def fitPeak(data,xleft,xright,peakType='Gaussian',constant=False,ampParams=None,centParams=None,constParams=None):
     '''
     Fit data to a peak model with the provided bounds and the addition of a constant background term
     
     Parameters
     --------
     data : array_like
         Input 2D array containing the data to fit.
@@ -15,14 +15,20 @@
     xright : float
         Right boundary of the data to fit.
     peakType : str, optional
         The type of peak to use for the fit. The default choice is a Gaussian model.
         All models are listed below.
     constant : bool, optional
         Whether to add a constant background value to the fit.
+    ampParams : dict, optional
+        Dictionary of optional keyword args for the amplitude param
+    centParams : dict, optional
+        Dictionary of optional keyword args for the center param
+    constParams : dict, optional
+        Dictionary of optional keyword args for the constant param
 
 
     Returns
     --------
     fitResult : lmfit ModelResult object
         The ModelResult contains the fitting results created by lmfit. 
     '''
@@ -44,19 +50,27 @@
         modCombined = modPeak
     
     dataLocations = np.where((datax >= xleft) & (datax <= xright))[0]
     
     fitx = datax[dataLocations]
     fity = datay[dataLocations]
     
-    
-    params = modConst.guess(fity,x=fitx)
-    params+= modPeak.guess(fity,x=fitx)
-    
-    params['c'].set(min=0,max=np.max(fity))
+    params = modPeak.guess(fity,x=fitx)
+    if constant:
+        params += modConst.guess(fity,x=fitx)
+        if constParams is not None:
+            params['c'].set(**constParams)
+        else:
+            params['c'].set(min=0,max=np.max(fity))
+        
+    if ampParams is not None:
+        params['amplitude'].set(**ampParams)
+        
+    if centParams is not None:
+        params['center'].set(**centParams)
     
     fitResult = modCombined.fit(fity,params,x=fitx)
     
     return fitResult
 
 
 def find_max(fitfunction,bounds):
```

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions/math.py` & `SeanFunctions-0.4.3/src/SeanFunctions/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     
     r = np.arange(nq) * np.pi / np.max(q) #Define the values of r
     nr = len(r)
     ft = np.zeros(nr) #Create empty array (detault is float64)
     
     for i in range(nr):
         x = q * r[i]
-        ft[i] = sum(intq2 * np.sinc(x/np.pi)) #np.sinc = sin(pi*x)/(pi*x)
+        ft[i] = np.sum(intq2 * np.sinc(x/np.pi)) #np.sinc = sin(pi*x)/(pi*x)
     
     ft *= dq
     
     if unpack is None:
         return np.column_stack((r, ft))
     else:
         return r, ft
```

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions/scattering.py` & `SeanFunctions-0.4.3/src/SeanFunctions/scattering.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions.egg-info/PKG-INFO` & `SeanFunctions-0.4.3/src/SeanFunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.4.1
+Version: 0.4.3
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.4.1/src/SeanFunctions.egg-info/SOURCES.txt` & `SeanFunctions-0.4.3/src/SeanFunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

