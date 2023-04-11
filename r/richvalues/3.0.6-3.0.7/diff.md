# Comparing `tmp/richvalues-3.0.6.tar.gz` & `tmp/richvalues-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.0.6.tar", last modified: Tue Apr 11 14:31:30 2023, max compression
+gzip compressed data, was "richvalues-3.0.7.tar", last modified: Tue Apr 11 14:34:40 2023, max compression
```

## Comparing `richvalues-3.0.6.tar` & `richvalues-3.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:31:30.616232 richvalues-3.0.6/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:31:30.612233 richvalues-3.0.6/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.6/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 14:31:14.000000 richvalues-3.0.6/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:31:30.612233 richvalues-3.0.6/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   146009 2023-04-11 13:58:40.000000 richvalues-3.0.6/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:31:30.612233 richvalues-3.0.6/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:31:30.000000 richvalues-3.0.6/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 14:31:30.000000 richvalues-3.0.6/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 14:31:30.000000 richvalues-3.0.6/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 14:31:30.000000 richvalues-3.0.6/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 14:31:30.000000 richvalues-3.0.6/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 14:31:30.616232 richvalues-3.0.6/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 14:31:10.000000 richvalues-3.0.6/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:34:40.745544 richvalues-3.0.7/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:34:40.745544 richvalues-3.0.7/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.7/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 14:34:22.000000 richvalues-3.0.7/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:34:40.741545 richvalues-3.0.7/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   146119 2023-04-11 14:34:11.000000 richvalues-3.0.7/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:34:40.745544 richvalues-3.0.7/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 14:34:40.000000 richvalues-3.0.7/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 14:34:40.745544 richvalues-3.0.7/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 14:34:18.000000 richvalues-3.0.7/setup.py
```

### Comparing `richvalues-3.0.6/PKG-INFO` & `richvalues-3.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.6
+Version: 3.0.7
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.6/README.md` & `richvalues-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.6/pyproject.toml` & `richvalues-3.0.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.0.6"
+version = "3.0.7"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `richvalues-3.0.6/richvalues/__init__.py` & `richvalues-3.0.7/richvalues/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.0.4'
+__version__ = '3.0.7'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
@@ -513,16 +513,18 @@
         isfinite = (True if np.isfinite(self.main)
                     and all(np.isfinite(self.unc)) else False)
         return isfinite
     
     def interval(self, sigmas=defaultparams['sigmas for interval']):
         """Interval of possible values of the rich value."""
         if not self.is_interv:
-            interv = [max(self.domain[0], self.main - sigmas*self.unc[0]),
-                      min(self.domain[1], self.main + sigmas*self.unc[1])]
+            ampl1 = sigmas * self.unc[0] if self.unc[0] != 0 else 0
+            ampl2 = sigmas * self.unc[1] if self.unc[1] != 0 else 0
+            interv = [max(self.domain[0], self.main - ampl1),
+                      min(self.domain[1], self.main + ampl2)]
         else:
             if self.is_uplim and not self.is_lolim:
                 interv = [self.domain[0], self.main]
             elif self.is_lolim and not self.is_uplim:
                 interv = [self.main, self.domain[1]]
             else:
                 interv = [self.main - self.unc[0], self.main + self.unc[1]]
```

### Comparing `richvalues-3.0.6/richvalues.egg-info/PKG-INFO` & `richvalues-3.0.7/richvalues.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.6
+Version: 3.0.7
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.6/setup.py` & `richvalues-3.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.0.6',
+    version = '3.0.7',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues',
```

