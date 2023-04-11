# Comparing `tmp/SeanFunctions-0.4.3.tar.gz` & `tmp/SeanFunctions-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeanFunctions-0.4.3.tar", last modified: Tue Apr 11 18:04:13 2023, max compression
+gzip compressed data, was "SeanFunctions-0.4.4.tar", last modified: Tue Apr 11 18:13:05 2023, max compression
```

## Comparing `SeanFunctions-0.4.3.tar` & `SeanFunctions-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.122202 SeanFunctions-0.4.3/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/.gitignore
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.4.3/LICENSE
--rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/MANIFEST.in
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-11 18:04:13.121946 SeanFunctions-0.4.3/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.4.3/README.md
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-04-11 18:00:46.000000 SeanFunctions-0.4.3/pyproject.toml
--rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-04-11 18:04:13.122260 SeanFunctions-0.4.3/setup.cfg
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.117347 SeanFunctions-0.4.3/src/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.120213 SeanFunctions-0.4.3/src/SeanFunctions/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.121605 SeanFunctions-0.4.3/src/SeanFunctions/Data/
--rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/__init__.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     3680 2023-04-11 18:03:36.000000 SeanFunctions-0.4.3/src/SeanFunctions/fitting.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     8986 2023-04-10 21:00:12.000000 SeanFunctions-0.4.3/src/SeanFunctions/math.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     4166 2023-01-14 21:57:03.000000 SeanFunctions-0.4.3/src/SeanFunctions/scattering.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)      196 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions/version.py
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:04:13.120913 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/SOURCES.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/dependency_links.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-04-11 18:04:13.000000 SeanFunctions-0.4.3/src/SeanFunctions.egg-info/top_level.txt
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:13:05.642865 SeanFunctions-0.4.4/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.4.4/.gitignore
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.4.4/LICENSE
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.4.4/MANIFEST.in
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-11 18:13:05.642609 SeanFunctions-0.4.4/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.4.4/README.md
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-04-11 18:12:30.000000 SeanFunctions-0.4.4/pyproject.toml
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-04-11 18:13:05.642929 SeanFunctions-0.4.4/setup.cfg
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:13:05.638486 SeanFunctions-0.4.4/src/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:13:05.640598 SeanFunctions-0.4.4/src/SeanFunctions/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:13:05.642255 SeanFunctions-0.4.4/src/SeanFunctions/Data/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.4.4/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.4.4/src/SeanFunctions/Data/NeutronScatteringLengths.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.4.4/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.4.4/src/SeanFunctions/__init__.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     3849 2023-04-11 18:12:24.000000 SeanFunctions-0.4.4/src/SeanFunctions/fitting.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     8986 2023-04-10 21:00:12.000000 SeanFunctions-0.4.4/src/SeanFunctions/math.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     4166 2023-01-14 21:57:03.000000 SeanFunctions-0.4.4/src/SeanFunctions/scattering.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      196 2023-04-11 18:13:05.000000 SeanFunctions-0.4.4/src/SeanFunctions/version.py
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-11 18:13:05.641239 SeanFunctions-0.4.4/src/SeanFunctions.egg-info/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-11 18:13:05.000000 SeanFunctions-0.4.4/src/SeanFunctions.egg-info/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-04-11 18:13:05.000000 SeanFunctions-0.4.4/src/SeanFunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-04-11 18:13:05.000000 SeanFunctions-0.4.4/src/SeanFunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-04-11 18:13:05.000000 SeanFunctions-0.4.4/src/SeanFunctions.egg-info/top_level.txt
```

### Comparing `SeanFunctions-0.4.3/LICENSE` & `SeanFunctions-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.3/PKG-INFO` & `SeanFunctions-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.4.3
+Version: 0.4.4
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.4.3/pyproject.toml` & `SeanFunctions-0.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SeanFunctions"
-version = "0.4.3"
+version = "0.4.4"
 # dynamic = ["version"]
 authors = [
   { name="Sean Fayfar", email="sfayfar@gmail.com" },
 ]
 description = "Collection of useful python functions"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv` & `SeanFunctions-0.4.4/src/SeanFunctions/Data/AtomicFormFactorConstants.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv` & `SeanFunctions-0.4.4/src/SeanFunctions/Data/NeutronScatteringLengths.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv` & `SeanFunctions-0.4.4/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions/fitting.py` & `SeanFunctions-0.4.4/src/SeanFunctions/fitting.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,41 +69,50 @@
         params['center'].set(**centParams)
     
     fitResult = modCombined.fit(fity,params,x=fitx)
     
     return fitResult
 
 
-def find_max(fitfunction,bounds):
+def find_max(fitfunction,bounds,min=False):
     '''
     Finds the maximum value of a Gaussian shaped function determined through a fit
 
     Parameters
     ---------
     fitfunction : lmfit fitted class
         Fitting result from lmfit
     
     bounds : array_like
         A list of the bounds where the peak is located.
 
+    min : bool, optional
+        Optional keyword for finding minimum rather than maximum
+
     Return
     --------
     out : array with xvalue, maxvalue, maxvalueunc
 
 
     Example
     --------
     modGaus = lmfit.models.Gaussian()
     result = modGaus.fit(y,params,x=x)
     maximum = find_max(result,[1,2])
         '''
     from scipy.optimize import minimize_scalar
     
+    if min:
+        scale = 1
+    else:
+        scale = -1
+
+
     def function(xvalue):
-        return -fitfunction.eval(x=xvalue)
+        return scale * fitfunction.eval(x=xvalue)
     xvalue = minimize_scalar(function,bounds=bounds,method='bounded').x
     maxvalue = fitfunction.eval(x=xvalue)
     maxvalueunc = fitfunction.eval_uncertainty(x=xvalue)[0]
     out = np.array([xvalue, maxvalue, maxvalueunc])
     return out
```

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions/math.py` & `SeanFunctions-0.4.4/src/SeanFunctions/math.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions/scattering.py` & `SeanFunctions-0.4.4/src/SeanFunctions/scattering.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions.egg-info/PKG-INFO` & `SeanFunctions-0.4.4/src/SeanFunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.4.3
+Version: 0.4.4
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.4.3/src/SeanFunctions.egg-info/SOURCES.txt` & `SeanFunctions-0.4.4/src/SeanFunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

