# Comparing `tmp/richvalues-3.0.3.tar.gz` & `tmp/richvalues-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.0.3.tar", last modified: Tue Apr 11 11:26:08 2023, max compression
+gzip compressed data, was "richvalues-3.0.4.tar", last modified: Tue Apr 11 14:03:36 2023, max compression
```

## Comparing `richvalues-3.0.3.tar` & `richvalues-3.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 11:26:08.983686 richvalues-3.0.3/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 11:26:08.983686 richvalues-3.0.3/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.3/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 11:25:46.000000 richvalues-3.0.3/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 11:26:08.979686 richvalues-3.0.3/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   144484 2023-04-11 11:25:12.000000 richvalues-3.0.3/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 11:26:08.983686 richvalues-3.0.3/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 11:26:08.000000 richvalues-3.0.3/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 11:26:08.000000 richvalues-3.0.3/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 11:26:08.000000 richvalues-3.0.3/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 11:26:08.000000 richvalues-3.0.3/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 11:26:08.000000 richvalues-3.0.3/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 11:26:08.983686 richvalues-3.0.3/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 11:25:40.000000 richvalues-3.0.3/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:03:36.775993 richvalues-3.0.4/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:03:36.775993 richvalues-3.0.4/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.4/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 13:59:18.000000 richvalues-3.0.4/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:03:36.775993 richvalues-3.0.4/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   146009 2023-04-11 13:58:40.000000 richvalues-3.0.4/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 14:03:36.775993 richvalues-3.0.4/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 14:03:36.000000 richvalues-3.0.4/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 14:03:36.775993 richvalues-3.0.4/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 13:59:10.000000 richvalues-3.0.4/setup.py
```

### Comparing `richvalues-3.0.3/PKG-INFO` & `richvalues-3.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.3
+Version: 3.0.4
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.3/README.md` & `richvalues-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `richvalues-3.0.3/pyproject.toml` & `richvalues-3.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.0.3"
+version = "3.0.4"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `richvalues-3.0.3/richvalues/__init__.py` & `richvalues-3.0.4/richvalues/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.0.0'
+__version__ = '3.0.4'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
@@ -61,15 +61,15 @@
     'use 1-sigma combinations to approximate uncertainty propagation': False,
     'fraction of the central value for upper/lower limits': 0.2,
     'number of repetitions to estimate upper/lower limits': 4,
     'decimal exponent to define zero': -90.,
     'decimal exponent to define infinity': 90.,
     'multiplication symbol for scientific notation in LaTeX': '\\cdot',
     'sigmas for overlap': 1.,
-    'sigmas for comparison': 3.
+    'sigmas for interval': 3.
     }
 
 variable_count = 1
 variable_dict = {}
 
 def round_sf(x,
         n=defaultparams['number of significant figures'],
@@ -363,15 +363,15 @@
             main = float(main)
         if not hasattr(unc, '__iter__'):
             unc = [unc, unc]
         if any(np.isinf(unc)):
             main = np.nan
             unc = [0, 0]
         unc = np.nan_to_num(unc, nan=0)
-        if np.isfinite(main) and not domain[0] <= main <= domain[1]:
+        if not np.isnan(main) and not domain[0] <= main <= domain[1]:
             raise Exception('Invalid main value {} for domain {}.'
                             .format(main, domain))
         unc = list(unc)
         unc = [float(unc[0]), float(unc[1])]
         unc[0] = abs(unc[0])
         if not (is_lolim or is_uplim) and unc[1] < 0:
             unc_text = ('Superior uncertainty' if hasattr(unc_or, '__iter__')
@@ -510,27 +510,41 @@
     @property
     def is_finite(self):
         """Finite value."""
         isfinite = (True if np.isfinite(self.main)
                     and all(np.isfinite(self.unc)) else False)
         return isfinite
     
-    def interval(self, sigmas=3.):
+    def interval(self, sigmas=defaultparams['sigmas for interval']):
         """Interval of possible values of the rich value."""
         if not self.is_interv:
             interv = [max(self.domain[0], self.main - sigmas*self.unc[0]),
                       min(self.domain[1], self.main + sigmas*self.unc[1])]
         else:
             if self.is_uplim and not self.is_lolim:
                 interv = [self.domain[0], self.main]
             elif self.is_lolim and not self.is_uplim:
                 interv = [self.main, self.domain[1]]
             else:
                 interv = [self.main - self.unc[0], self.main + self.unc[1]]
         return interv
+    
+    def sign(self, sigmas=np.inf):
+        """Sign of the richvalue."""
+        interv = self.interval(sigmas)
+        signs_interv = np.sign(interv)
+        if all(signs_interv == 0):
+            s = 0
+        elif all(signs_interv >= 0):
+            s = 1
+        elif all(signs_interv <= 0):
+            s = -1
+        else:
+            s = np.nan
+        return s
   
     def set_lims_factor(self, factor=4.):
         """Set uncertainties of limits with respect to cetral values."""
         if self.is_lolim or self.is_uplim:
             self.unc = [self.main / factor, self.main / factor]
         
     def _format_as_rich_value(self):
@@ -739,15 +753,15 @@
         domain = copy.copy(self.domain)
         if not self.is_interv:
             x = abs(main)
         else:
             x1, x2 = self.interval()
             x1, x2 = abs(x1), abs(x2)
             x = [min(x1, x2), max(x1, x2)]
-        dx = unc
+        dx = np.abs(unc)
         domain = [abs(domain[0]), abs(domain[1])]
         domain = [min(domain), max(domain)]
         if np.isinf(domain[0]):
             domain[0] = 0
         new_rval = RichValue(x, dx, domain=domain)
         new_rval.vars = self.vars
         new_rval.expression = 'abs({})'.format(self.expression)
@@ -758,15 +772,15 @@
         unc = copy.copy(self.unc)
         domain = copy.copy(self.domain)
         if not self.is_interv:
             x = -main
         else:
             x1, x2 = self.interval()
             x = [-x2, -x1]
-        dx = unc
+        dx = np.abs(unc)
         domain = [-domain[0], -domain[1]]
         domain = [min(domain), max(domain)]
         new_rval = RichValue(x, dx, domain=domain)
         new_rval.vars = self.vars
         new_rval.expression = '-({})'.format(self.expression)
         return new_rval
     
@@ -786,15 +800,15 @@
             other_ = (other.main if type(other) is RichValue
                       and other.unc==[0,0] else other)
             if type(other_) is RichValue:
                 new_rval = add_two_rich_values(self, other_)
             else:
                 if other_ != 0:
                     x = self.main + other_
-                    dx = copy.copy(self.unc)
+                    dx = np.abs(self.unc)
                     new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                          self.is_range, self.domain)
                 else:
                     new_rval = RichValue(0, domain=self.domain)
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
@@ -829,19 +843,19 @@
             other_ = (other.main if type(other) is RichValue
                       and other.unc==[0,0] else other)
             if type(other_) is RichValue:
                 new_rval = multiply_two_rich_values(self, other_)
             else:
                 if other_ != 0:
                     x = self.main * other_
-                    dx = np.array(self.unc) * other_
+                    dx = np.abs(np.array(self.unc) * other_)
                     if type(other_) is not RichValue:
-                        domain = (other.domain if type(other) is RichValue
-                                  else None)
-                        other_ = RichValue(other_, domain=domain)
+                        other_domain = (other.domain if type(other)
+                                        is RichValue else None)
+                        other_ = RichValue(other_, domain=other_domain)
                     domain_combs = [self.domain[i1] * other_.domain[i2]
                                     for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
                     domain1, domain2 = min(domain_combs), max(domain_combs)
                     if not np.isfinite(domain1):
                         domain1 = -np.inf
                     if not np.isfinite(domain2):
                         domain2 = np.inf
@@ -879,33 +893,53 @@
                       and other.unc==[0,0] else other)
             if type(other_) is RichValue:
                 new_rval = divide_two_rich_values(self, other_)
             else:
                 if other_ != 0:
                     with np.errstate(divide='ignore', invalid='ignore'):
                         x = self.main / other_
-                        dx = np.array(self.unc) / other_
+                        dx = np.abs(np.array(self.unc) / other_)
                         if type(other_) is not RichValue:
-                            domain = (other.domain if type(other) is RichValue
-                                      else None)
-                            other_ = RichValue(other_)
+                            other_domain = (other.domain if type(other)
+                                            is RichValue else None)
+                            other_ = RichValue(other_, domain=other_domain)
                         domain_combs = [self.domain[i1] * other_.domain[i2]
                                         for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
                         domain1, domain2 = min(domain_combs), max(domain_combs)
                         if not np.isfinite(domain1):
                             domain1 = -np.inf
                         if not np.isfinite(domain2):
                             domain2 = np.inf
                         domain = [domain1, domain2]
                     new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                          self.is_range, domain)
                     new_rval.num_sf = self.num_sf
                     new_rval.min_exp = self.min_exp
                 else:
-                    new_rval = RichValue(np.nan, domain=self.domain)
+                    if type(other_) is not RichValue:
+                        other_domain = (other.domain if type(other)
+                                        is RichValue else None)
+                        other_ = RichValue(other_, domain=other_domain)
+                    zero = other_
+                    zero_signs = np.sign(zero.domain)
+                    if all(zero_signs == 0):
+                        zero_sign = np.nan
+                    elif all(zero_signs >= 0):
+                        zero_sign = 1
+                    elif all(zero_signs <= 0):
+                        zero_sign = -1
+                    else:
+                        zero_sign = np.nan
+                    sign = self.sign() * zero_sign
+                    value = sign * np.inf
+                    if np.isinf(value):
+                        domain = [0, np.inf] if value > 0 else [-np.inf, 0]
+                    else:
+                        domain = (sign * abs(self)).domain
+                    new_rval = RichValue(value, domain=domain)
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
         new_rval.vars = list(variables)
         new_rval.expression = expression
@@ -926,19 +960,19 @@
                       and other.unc==[0,0] else other)
             if type(other_) is RichValue:
                 new_rval = divide_two_rich_values(other_, self)
             else:
                 if other_ != 0:
                     with np.errstate(divide='ignore'):
                         x = other_ / self.main
-                        dx = x * np.array(self.unc) / self.main
+                        dx = np.abs(x * np.array(self.unc) / self.main)
                         if type(other_) is not RichValue:
-                            domain = (other.domain if type(other) is RichValue
-                                      else None)
-                            other_ = RichValue(other_)
+                            other_domain = (other.domain if type(other)
+                                            is RichValue else None)
+                            other_ = RichValue(other_, domain=other_domain)
                         domain_combs = [self.domain[i1] * other_.domain[i2]
                                         for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
                         domain1, domain2 = min(domain_combs), max(domain_combs)
                         if not np.isfinite(domain1):
                             domain1 = -np.inf
                         if not np.isfinite(domain2):
                             domain2 = np.inf
@@ -988,15 +1022,15 @@
                     new_rval = function_with_rich_values(lambda a,b: a**b,
                                                 [self, other_], domain=domain)
                 else:
                     new_rval = RichValue(0)
                     new_rval.num_sf = self.num_sf
             elif (type(other) is not RichValue and self.prop_score > sigmas):
                 x = main ** other
-                dx = abs(x * other * np.array(unc) / main)
+                dx = np.abs(x * other * np.array(unc) / main)
                 if domain != [-np.inf, np.inf]:
                     if domain[0] != 0 or (domain[0] == 0 and other>0):
                         x1 = domain[0] ** other
                     else:
                         x1 = np.inf
                     if domain[1] != 0 or (domain[0] == 0 and other>0):
                         x2 = domain[1] ** other
@@ -1341,15 +1375,15 @@
     def prop_scores(self):
         return (np.array([x.prop_score for x in self.flat])
                 .reshape(self.shape))
     @property
     def uncs_eb(self):
         return self.uncs.transpose()
     
-    def intervals(self, sigmas=3.):
+    def intervals(self, sigmas=None):
         return (np.array([x.interval() for x in self.flat])
                 .reshape((*self.shape,2)))
     
     def set_params(self, params):
         """Set the rich value parameters of each entry of the rich array."""
         for x in self.flat:
             if 'domain' in params:
@@ -1781,15 +1815,15 @@
         return [pd.Series(rich_array(self.values).norm_uncs.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def prop_scores(self):
         return [pd.Series(rich_array(self.values).prop_scores.T[i].T,
                           self.index) for i in (0,1)]
     
-    def intervals(self, sigmas=3.):
+    def intervals(self, sigmas=defaultparams['sigmas for interval']):
         return [pd.Series(rich_array(self.values).intervals(sigmas).T[i].T,
                           self.index) for i in (0,1)]
     
     def set_params(self, params):
         data = self.values.view(RichArray)
         data.set_params(params)
         self.update(pd.Series(data, self.index))
@@ -1860,15 +1894,15 @@
         domain2 = np.inf
     domain = [domain1, domain2]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
     if (not (x.is_interv or y.is_interv)
          and x.prop_score > sigmas and y.prop_score > sigmas):
         z = x.main * y.main
         dx, dy = np.array(x.unc), np.array(y.unc)
-        dz = z * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
+        dz = abs(z) * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a*b, [x, y], domain=domain,
                                       is_vectorizable=True)
     z.num_sf = num_sf
     z.min_exp = min_exp
     return z
@@ -1887,24 +1921,24 @@
         domain2 = np.inf
     domain = [domain1, domain2]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
     if (not (x.is_interv or y.is_interv) and 0 not in [x.main, y.main]
          and x.prop_score > sigmas and y.prop_score > sigmas):
         z = x.main / y.main
         dx, dy = np.array(x.unc), np.array(y.unc)
-        dz = z * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
+        dz = abs(z) * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a/b, [x, y], domain=domain,
                                   is_vectorizable=True, sigmas=sigmas)
     z.num_sf = num_sf
     z.min_exp = min_exp
     return z
 
-def greater(x, y, sigmas=defaultparams['sigmas for comparison']):
+def greater(x, y, sigmas=defaultparams['sigmas for interval']):
     """Determine if a rich value/array (x) is greater than another one (y)."""
     are_single_values = all([type(var) is str
                              or not hasattr(var, '__iter__') for var in (x,y)])
     if are_single_values:
         x = x if type(x) is RichValue else rich_value(x)
         y = y if type(y) is RichValue else rich_value(y)
         x1, x2 = x.interval(sigmas=sigmas)
@@ -1973,23 +2007,23 @@
         output = np.empty(0, bool)
         for xi,yi in zip(x.flat, y.flat):
             output = np.append(output, equiv(xi,yi))
         output = output.reshape(x.shape)
     return output
 
 def greater_equiv(x, y,
-                  sigmas_comparison=defaultparams['sigmas for comparison'],
+                  sigmas_interval=defaultparams['sigmas for interval'],
                   sigmas_overlap=defaultparams['sigmas for overlap']):
     """Check if a rich value/array is greater or equivalent than another one."""
     are_single_values = all([type(var) is str
                              or not hasattr(var, '__iter__') for var in (x,y)])
     if are_single_values:
         x = x if type(x) is RichValue else rich_value(x)
         y = y if type(y) is RichValue else rich_value(y)
-        output = greater(x, y, sigmas_comparison) or equiv(x, y, sigmas_overlap)
+        output = greater(x, y, sigmas_interval) or equiv(x, y, sigmas_overlap)
     else:
         x = x if type(x) is RichArray else rich_array(x)
         y = y if type(y) is RichValue else rich_array(y)
         if x.size == 1 and x.shape != y.shape:
             x = x.flatten()[0] * np.ones(y.shape)
         if y.size == 1 and x.shape != y.shape:
             y = y.flatten()[0] * np.ones(x.shape)
@@ -1998,23 +2032,23 @@
         output = np.empty(0, bool)
         for xi,yi in zip(x.flat, y.flat):
             output = np.append(output, greater_equiv(xi,yi))
         output = output.reshape(x.shape)
     return output
 
 def less_equiv(x, y,
-               sigmas_comparison=defaultparams['sigmas for comparison'],
+               sigmas_interval=defaultparams['sigmas for interval'],
                sigmas_overlap=defaultparams['sigmas for overlap']):
     """Check if a rich value/array is less or equivalent than another one."""
     are_single_values = all([type(var) is str
                              or not hasattr(var, '__iter__') for var in (x,y)])
     if are_single_values:
         x = x if type(x) is RichValue else rich_value(x)
         y = y if type(y) is RichValue else rich_value(y)
-        output = less(x, y, sigmas_comparison) or equiv(x, y, sigmas_overlap)
+        output = less(x, y, sigmas_interval) or equiv(x, y, sigmas_overlap)
     else:
         x = x if type(x) is RichArray else rich_array(x)
         y = y if type(y) is RichValue else rich_array(y)
         if x.size == 1 and x.shape != y.shape:
             x = x.flatten()[0] * np.ones(y.shape)
         if y.size == 1 and x.shape != y.shape:
             y = y.flatten()[0] * np.ones(x.shape)
@@ -3599,8 +3633,8 @@
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

### Comparing `richvalues-3.0.3/richvalues.egg-info/PKG-INFO` & `richvalues-3.0.4/richvalues.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.3
+Version: 3.0.4
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
         Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
```

### Comparing `richvalues-3.0.3/setup.py` & `richvalues-3.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.0.3',
+    version = '3.0.4',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues',
```

