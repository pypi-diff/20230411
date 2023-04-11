# Comparing `tmp/iloscar-0.1.2a0.tar.gz` & `tmp/iloscar-0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar-0.1.2a0.tar", last modified: Tue Apr 11 20:37:54 2023, max compression
+gzip compressed data, was "iloscar-0.1a0.tar", last modified: Tue Apr 11 20:32:17 2023, max compression
```

## Comparing `iloscar-0.1.2a0.tar` & `iloscar-0.1a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:37:54.935968 iloscar-0.1.2a0/
--rw-r--r--   0 shihan     (504) staff       (20)      730 2023-04-11 20:37:54.935711 iloscar-0.1.2a0/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-04 17:29:12.000000 iloscar-0.1.2a0/README.md
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:37:54.933002 iloscar-0.1.2a0/iloscar/
--rw-r--r--   0 shihan     (504) staff       (20)      341 2023-04-05 02:45:38.000000 iloscar-0.1.2a0/iloscar/__init__.py
--rw-rw-r--   0 shihan     (504) staff       (20)     2006 2023-04-11 20:27:13.000000 iloscar-0.1.2a0/iloscar/app.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:37:54.934290 iloscar-0.1.2a0/iloscar/dat_y0/
--rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.1.2a0/iloscar/dat_y0/petm_steady.dat
--rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.1.2a0/iloscar/dat_y0/preind_steady.dat
--rw-rw-r--   0 shihan     (504) staff       (20)   106008 2023-04-11 20:37:31.000000 iloscar-0.1.2a0/iloscar/iLOSCAR_backend.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:37:54.935260 iloscar-0.1.2a0/iloscar/pages/
--rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-11 20:28:53.000000 iloscar-0.1.2a0/iloscar/pages/Function.py
--rw-rw-r--   0 shihan     (504) staff       (20)    26082 2023-04-11 20:28:43.000000 iloscar-0.1.2a0/iloscar/pages/forward.py
--rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-11 20:29:07.000000 iloscar-0.1.2a0/iloscar/pages/home.py
--rw-rw-r--   0 shihan     (504) staff       (20)    45707 2023-04-11 20:29:17.000000 iloscar-0.1.2a0/iloscar/pages/inverse.py
--rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.1.2a0/iloscar/style.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:37:54.933765 iloscar-0.1.2a0/iloscar.egg-info/
--rw-r--r--   0 shihan     (504) staff       (20)      730 2023-04-11 20:37:54.000000 iloscar-0.1.2a0/iloscar.egg-info/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-11 20:37:54.000000 iloscar-0.1.2a0/iloscar.egg-info/SOURCES.txt
--rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-11 20:37:54.000000 iloscar-0.1.2a0/iloscar.egg-info/dependency_links.txt
--rw-r--r--   0 shihan     (504) staff       (20)      117 2023-04-11 20:37:54.000000 iloscar-0.1.2a0/iloscar.egg-info/requires.txt
--rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-11 20:37:54.000000 iloscar-0.1.2a0/iloscar.egg-info/top_level.txt
--rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-11 20:37:54.936065 iloscar-0.1.2a0/setup.cfg
--rw-r--r--   0 shihan     (504) staff       (20)     1434 2023-04-11 20:37:36.000000 iloscar-0.1.2a0/setup.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.592731 iloscar-0.1a0/
+-rw-r--r--   0 shihan     (504) staff       (20)      728 2023-04-11 20:32:17.592362 iloscar-0.1a0/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-04 17:29:12.000000 iloscar-0.1a0/README.md
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.589587 iloscar-0.1a0/iloscar/
+-rw-r--r--   0 shihan     (504) staff       (20)      341 2023-04-05 02:45:38.000000 iloscar-0.1a0/iloscar/__init__.py
+-rw-rw-r--   0 shihan     (504) staff       (20)     2006 2023-04-11 20:27:13.000000 iloscar-0.1a0/iloscar/app.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.590968 iloscar-0.1a0/iloscar/dat_y0/
+-rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.1a0/iloscar/dat_y0/petm_steady.dat
+-rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.1a0/iloscar/dat_y0/preind_steady.dat
+-rw-rw-r--   0 shihan     (504) staff       (20)   106011 2023-04-09 03:50:44.000000 iloscar-0.1a0/iloscar/iLOSCAR_backend.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.591893 iloscar-0.1a0/iloscar/pages/
+-rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-11 20:28:53.000000 iloscar-0.1a0/iloscar/pages/Function.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    26082 2023-04-11 20:28:43.000000 iloscar-0.1a0/iloscar/pages/forward.py
+-rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-11 20:29:07.000000 iloscar-0.1a0/iloscar/pages/home.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    45707 2023-04-11 20:29:17.000000 iloscar-0.1a0/iloscar/pages/inverse.py
+-rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.1a0/iloscar/style.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.590374 iloscar-0.1a0/iloscar.egg-info/
+-rw-r--r--   0 shihan     (504) staff       (20)      728 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/SOURCES.txt
+-rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/dependency_links.txt
+-rw-r--r--   0 shihan     (504) staff       (20)      117 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/requires.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/top_level.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-11 20:32:17.592818 iloscar-0.1a0/setup.cfg
+-rw-r--r--   0 shihan     (504) staff       (20)     1432 2023-04-11 20:31:11.000000 iloscar-0.1a0/setup.py
```

### Comparing `iloscar-0.1.2a0/PKG-INFO` & `iloscar-0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar
-Version: 0.1.2a0
+Version: 0.1a0
 Summary: iLOSCAR
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-0.1.2a0/iloscar/app.py` & `iloscar-0.1a0/iloscar/app.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar/dat_y0/petm_steady.dat` & `iloscar-0.1a0/iloscar/dat_y0/petm_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar/dat_y0/preind_steady.dat` & `iloscar-0.1a0/iloscar/dat_y0/preind_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar/iLOSCAR_backend.py` & `iloscar-0.1a0/iloscar/iLOSCAR_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,30 +32,29 @@
 import pandas as pd
 import numpy as np
 from numba import jit
 import sys
 
 import dash
 from dash import html, dcc
+from style import *
 
 import timeit
 import plotly.graph_objects as go
 
 
 from scipy import interpolate
 from scipy.optimize import root_scalar, toms748
 
 
 from scipy.integrate import solve_ivp
 
 from os.path import join, exists
 from os import makedirs
 
-from iloscar.style import *
-
 
 
 
 
 
 def init_start(params):
     # input: front-end user input
@@ -916,15 +915,15 @@
                 yfinal = ysol.y[:,-1]
                 yfinal[3*NB:4*NB] *= TSCAL
                 np.savetxt('inv_ystart.dat', yfinal)
 
             elapse = timeit.default_timer() - start_time
             print(f'{elapse: .2f}s used.')
 
-
+            
             RUN_TYPE = 3
             frccinp = interpolate.interp1d(t_target_d13c, (d13c_eval/1e3+1)*RST, bounds_error=False, fill_value=((d13c_eval[0]/1e3+1)*RST,0), kind = 'zero')
             # emi_d13c_scenario = np.vstack([t_target_d13c, d13c_eval]).T
             # np.savetxt('inverse_emission_d13c_results.dat', emi_d13c_scenario)
             t_end = np.minimum(t_target[-1], t_target_d13c[-1])
             t_start = np.minimum(t_target[0], t_target_d13c[0])
             tt = np.linspace(t_target_d13c[0], t_target_d13c[-1]-10, int((t_target[-1]-t_target[0])/100))
```

### Comparing `iloscar-0.1.2a0/iloscar/pages/Function.py` & `iloscar-0.1a0/iloscar/pages/Function.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar/pages/forward.py` & `iloscar-0.1a0/iloscar/pages/forward.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar/pages/home.py` & `iloscar-0.1a0/iloscar/pages/home.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar/pages/inverse.py` & `iloscar-0.1a0/iloscar/pages/inverse.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar/style.py` & `iloscar-0.1a0/iloscar/style.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1.2a0/iloscar.egg-info/PKG-INFO` & `iloscar-0.1a0/iloscar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar
-Version: 0.1.2a0
+Version: 0.1a0
 Summary: iLOSCAR
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-0.1.2a0/setup.py` & `iloscar-0.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2-alpha'
+VERSION = '0.1-alpha'
 DESCRIPTION = 'iLOSCAR'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar",
     version=VERSION,
```

