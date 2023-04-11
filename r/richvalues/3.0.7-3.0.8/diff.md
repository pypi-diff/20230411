# Comparing `tmp/richvalues-3.0.7.tar.gz` & `tmp/richvalues-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.0.7.tar", last modified: Tue Apr 11 14:34:40 2023, max compression
+gzip compressed data, was "richvalues-3.0.8.tar", last modified: Tue Apr 11 15:18:01 2023, max compression
```

## Comparing `richvalues-3.0.7.tar` & `richvalues-3.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:34:40.745544 richvalues-3.0.7/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:34:40.745544 richvalues-3.0.7/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.7/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 14:34:22.000000 richvalues-3.0.7/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:34:40.741545 richvalues-3.0.7/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   146119 2023-04-11 14:34:11.000000 richvalues-3.0.7/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:34:40.745544 richvalues-3.0.7/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 14:34:40.745544 richvalues-3.0.7/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 14:34:18.000000 richvalues-3.0.7/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 15:18:01.312888 richvalues-3.0.8/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 15:18:01.312888 richvalues-3.0.8/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.8/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 15:17:56.000000 richvalues-3.0.8/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 15:18:01.308888 richvalues-3.0.8/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   146269 2023-04-11 15:16:45.000000 richvalues-3.0.8/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 15:18:01.312888 richvalues-3.0.8/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 15:18:01.000000 richvalues-3.0.8/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 15:18:01.312888 richvalues-3.0.8/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 15:17:43.000000 richvalues-3.0.8/setup.py
```

### Comparing `richvalues-3.0.7/PKG-INFO` & `richvalues-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.7
+Version: 3.0.8
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.7/README.md` & `richvalues-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.7/pyproject.toml` & `richvalues-3.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.0.7"
+version = "3.0.8"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `richvalues-3.0.7/richvalues/__init__.py` & `richvalues-3.0.8/richvalues/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.0.7'
+__version__ = '3.0.8'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
@@ -331,14 +331,16 @@
         if 'is_finite_range' in kwargs:
             is_range = kwargs['is_finite_range']
         
         if domain is None:
             domain = defaultparams['domain']
         unc_or = copy.copy(unc)
         main_or = copy.copy(main)
+        if not domain[0] <= domain[1]:
+            raise Exception('Invalid domain {}.'.format(domain))
         
         if type(main) in [list, tuple]:
             is_lolim, is_uplim, is_range = False, False, False
             main = [float(main[0]), float(main[1])]
             if main_or[0] <= domain[0] and main_or[1] < domain[1]:
                 is_uplim = True
                 main = main[1]
@@ -1277,30 +1279,30 @@
         are_lolims = np.array(are_lolims)
         are_uplims = np.array(are_uplims)
         are_ranges = np.array(are_ranges)
         domains = np.array(domains)
         array = np.empty(mains.size, object)
         if uncs.size == 1:
             uncs = uncs * np.ones((*mains.shape, 2))
-        elif len(uncs) == 2:
+        elif len(uncs) == 2 and type(uncs[0]) is not np.ndarray:
             uncs = np.array([uncs[0] * np.ones(mains.shape),
-                             uncs[1] * np.ones(mains.shape)]).transpose()
+                             uncs[1] * np.ones(mains.shape)])
         elif uncs.shape == (*mains.shape, 2):
             uncs = uncs.transpose()
         elif uncs.shape == mains.shape:
             uncs = np.array([[uncs]]*2).reshape((2, *mains.shape))
-        if len(domains) == 2:
+        if len(domains) == 2 and type(domains[0]) is not np.ndarray:
             domains = np.array([domains[0] * np.ones(mains.shape),
-                                domains[1] * np.ones(mains.shape)]).transpose()
+                                domains[1] * np.ones(mains.shape)])
         elif domains.shape == (*mains.shape, 2):
             domains = domains.transpose()
         elif domains.flatten().shape == (2,):
             domains = (np.array([domains for x in mains.flat])
                        .reshape((*mains.shape, 2)).transpose())
-            
+        
         mains_flat = mains.flatten()
         uncs_flat = uncs.flatten()
         are_lolims_flat = are_lolims.flatten()
         are_uplims_flat = are_uplims.flatten()
         are_ranges_flat = are_ranges.flatten()
         domains_flat = domains.flatten()
         offset = len(uncs_flat) // 2
@@ -3635,8 +3637,8 @@
 function = function_with_rich_values
 array_function = function_with_rich_arrays
 distribution = distr_with_rich_values
 evaluate_distribution = evaluate_distr
 center_and_uncertainties = center_and_uncs
 is_not_a_number = is_nan = isnan
 is_infinite = is_inf = isinf
-is_finite = is_finite = isfinite
+is_finite = is_finite = isfinite
```

### Comparing `richvalues-3.0.7/richvalues.egg-info/PKG-INFO` & `richvalues-3.0.8/richvalues.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.7
+Version: 3.0.8
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.7/setup.py` & `richvalues-3.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.0.7',
+    version = '3.0.8',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues',
```

