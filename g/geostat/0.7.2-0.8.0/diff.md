# Comparing `tmp/geostat-0.7.2.tar.gz` & `tmp/geostat-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-dtq111dn/geostat-0.7.2.tar", last modified: Mon Feb 27 23:47:58 2023, max compression
+gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-i1jhopsr/geostat-0.8.0.tar", last modified: Mon Apr 10 23:28:57 2023, max compression
```

## Comparing `geostat-0.7.2.tar` & `geostat-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-02-27 23:47:58.804520 geostat-0.7.2/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.7.2/LICENSE
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-02-27 23:47:58.804520 geostat-0.7.2/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.7.2/README.md
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      653 2023-02-27 23:01:46.000000 geostat-0.7.2/pyproject.toml
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      950 2023-02-27 23:47:58.804520 geostat-0.7.2/setup.cfg
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-02-27 23:47:58.804520 geostat-0.7.2/src/
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-02-27 23:47:58.804520 geostat-0.7.2/src/geostat/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      246 2023-02-27 23:01:35.000000 geostat-0.7.2/src/geostat/__init__.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    10951 2023-02-27 22:20:36.000000 geostat-0.7.2/src/geostat/gp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-02-03 03:28:12.000000 geostat-0.7.2/src/geostat/krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.7.2/src/geostat/mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-02-20 16:39:42.000000 geostat-0.7.2/src/geostat/metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    24115 2023-02-27 22:20:50.000000 geostat-0.7.2/src/geostat/model.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3257 2023-02-16 05:49:27.000000 geostat-0.7.2/src/geostat/op.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2972 2023-01-21 05:40:47.000000 geostat-0.7.2/src/geostat/param.py
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-02-27 23:47:58.804520 geostat-0.7.2/src/geostat.egg-info/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-02-27 23:47:58.000000 geostat-0.7.2/src/geostat.egg-info/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      568 2023-02-27 23:47:58.000000 geostat-0.7.2/src/geostat.egg-info/SOURCES.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-02-27 23:47:58.000000 geostat-0.7.2/src/geostat.egg-info/dependency_links.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-02-27 23:47:58.000000 geostat-0.7.2/src/geostat.egg-info/requires.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-02-27 23:47:58.000000 geostat-0.7.2/src/geostat.egg-info/top_level.txt
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-02-27 23:47:58.804520 geostat-0.7.2/tests/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     4410 2023-02-27 23:43:37.000000 geostat-0.7.2/tests/test_antiderivative.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3902 2023-02-03 03:49:08.000000 geostat-0.7.2/tests/test_delta.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3780 2023-02-03 03:49:34.000000 geostat-0.7.2/tests/test_gp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.7.2/tests/test_krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3569 2023-02-07 05:44:41.000000 geostat-0.7.2/tests/test_mcmc.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.7.2/tests/test_mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2641 2023-02-03 03:50:53.000000 geostat-0.7.2/tests/test_metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2072 2023-02-03 03:51:01.000000 geostat-0.7.2/tests/test_multigp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3870 2023-02-05 00:36:21.000000 geostat-0.7.2/tests/test_trend.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.117009 geostat-0.8.0/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.0/LICENSE
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-10 23:28:57.117009 geostat-0.8.0/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.0/README.md
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-10 23:28:45.000000 geostat-0.8.0/pyproject.toml
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-10 23:28:57.117009 geostat-0.8.0/setup.cfg
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.113009 geostat-0.8.0/src/
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.113009 geostat-0.8.0/src/geostat/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-10 23:06:48.000000 geostat-0.8.0/src/geostat/__init__.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    13134 2023-04-10 22:40:44.000000 geostat-0.8.0/src/geostat/kernel.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.0/src/geostat/krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.0/src/geostat/mean.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.0/src/geostat/mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.0/src/geostat/metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.0/src/geostat/model.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.0/src/geostat/op.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2972 2023-03-05 02:04:15.000000 geostat-0.8.0/src/geostat/param.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.113009 geostat-0.8.0/src/geostat.egg-info/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/SOURCES.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/dependency_links.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/requires.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/top_level.txt
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.117009 geostat-0.8.0/tests/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.0/tests/test_antiderivative.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.0/tests/test_delta.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.0/tests/test_gp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.0/tests/test_krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.0/tests/test_mcmc.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.0/tests/test_mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.0/tests/test_metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.0/tests/test_multigp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.0/tests/test_trend.py
```

### Comparing `geostat-0.7.2/LICENSE` & `geostat-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/PKG-INFO` & `geostat-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.7.2
+Version: 0.8.0
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.7.2/README.md` & `geostat-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/pyproject.toml` & `geostat-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geostat"
-version = "0.7.2"
+version = "0.8.0"
 description = "Model spatial data with Gaussian processes"
 readme = "README.md"
 authors = [
   {name="Michael J. Stephens", email="mjstephens@usgs.gov"},
   {name="Will Chang", email="will@hypergradient.ai"}
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["geospatial", "spatial", "interpolation", "gaussian process", "krige", "kriging"]
+requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/whdc/geostat"
```

### Comparing `geostat-0.7.2/setup.cfg` & `geostat-0.8.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geostat
-version = 0.7.2
+version = 0.8.0
 author = Michael J. Stephens, Will Chang
 author_email = mjstephens@usgs.gov, will@hypergradient.ai
 description = Python package for performing kriging and Gaussian processes with geoscience-oriented utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://code.usgs.gov/mjstephens/geostat
 project_urls = 
@@ -14,15 +14,14 @@
 	License :: OSI Approved :: Apache2 License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
 install_requires = 
 	matplotlib >= 3.0
 	numpy >= 1.19
 	pandas >= 1.2
 	scipy >= 1.5
 	shapely >= 1.8
 	tensorflow >= 2.5
```

### Comparing `geostat-0.7.2/src/geostat/gp.py` & `geostat-0.8.0/src/geostat/kernel.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,29 +3,40 @@
 import numpy as np
 
 # Tensorflow is extraordinarily noisy. Catch warnings during import.
 import warnings
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     import tensorflow as tf
+    from tensorflow.linalg import LinearOperatorFullMatrix as LOFullMatrix
+    from tensorflow.linalg import LinearOperatorBlockDiag as LOBlockDiag
 
 from .op import Op
-from .metric import Euclidean, ed
+from .metric import Euclidean, PerAxisDist2, ed
 from .param import get_parameter_values, ppp, upp, bpp
+from .mean import get_trend_coefs
 
-@dataclass
-class GP(Op):
+__all__ = ['Kernel']
+
+def block_diag(blocks):
+    """Return a dense block-diagonal matrix."""
+    return LOBlockDiag([LOFullMatrix(b) for b in blocks]).to_dense()
+
+class Kernel(Op):
     def __init__(self, fa, autoinputs):
         if 'offset' not in autoinputs: autoinputs['offset'] = 'offset'
         if 'locs1' not in autoinputs: autoinputs['locs1'] = 'locs1'
         if 'locs2' not in autoinputs: autoinputs['locs2'] = 'locs2'
         super().__init__(fa, autoinputs)
 
     def __add__(self, other):
-        return Stack([self]) + other
+        if other is None:
+            return self
+        else:
+            return Stack([self]) + other
 
     def __mul__(self, other):
         return Product([self]) * other
 
     def call(self, p, e):
         """
         Returns tuple `(mean, covariance)` for locations.
@@ -34,119 +45,90 @@
         pass
 
     def __call__(self, p, e):
         """
         Returns tuple `(mean, covariance)` for locations.
         Return values have correct shapes.
         """
-        M, C = self.call(p, e)
-        if M is None: M = 0.
+        C = self.call(p, e)
         if C is None: C = 0.
         n1 = tf.shape(e['locs1'])[0]
         n2 = tf.shape(e['locs2'])[0]
-        M = tf.broadcast_to(M, [n1])
         C = tf.broadcast_to(C, [n1, n2])
-        return M, C
+        return C
 
     def report(self, p):
         string = ', '.join('%s %4.2f' % (v.name, p[v.name]) for v in self.vars())
         return '[' + string + ']'
 
     def reg(self, p):
         pass
 
-def get_trend_coefs(beta):
-    if isinstance(beta, (list, tuple)):
-        return [p for s in beta for p in upp(s)]
-    elif isinstance(beta, str):
-        return upp(beta)
-    else:
-        return []
-
-class Trend(GP):
-    def __init__(self, featurizer, beta='beta'):
-        fa = dict(beta=beta)
-        self.featurizer = featurizer
-        super().__init__(fa, dict(locs1='locs1'))
-
-    def vars(self):
-        return get_trend_coefs(self.fa['beta'])
-
-    def call(self, p, e):
-        v = get_parameter_values(self.fa, p)
-        x = tf.cast(self.featurizer(e['locs1']), tf.float32)
-        if isinstance(v['beta'], (tuple, list)):
-            v['beta'] = tf.stack(v['beta'])
-        return tf.einsum('ab,b->a', x, v['beta']), None # [locs1]
-
-    def reg(self, p):
-        return 0.
-
-class TrendPrior(GP):
+class TrendPrior(Kernel):
     def __init__(self, featurizer, alpha='alpha'):
         fa = dict(alpha=alpha)
         self.featurizer = featurizer
         super().__init__(fa, dict(locs1='locs1', locs2='locs2'))
 
     def vars(self):
         return ppp(self.fa['alpha'])
 
     def call(self, p, e):
         v = get_parameter_values(self.fa, p)
         F1 = tf.cast(self.featurizer(e['locs1']), tf.float32)
         F2 = tf.cast(self.featurizer(e['locs2']), tf.float32)
-        return None, v['alpha'] * tf.einsum('ba,ca->bc', F1, F2)
+        return v['alpha'] * tf.einsum('ba,ca->bc', F1, F2)
 
     def reg(self, p):
         return 0.
 
 def scale_to_metric(scale, metric):
     assert scale is None or metric is None
     if metric is None:
         if scale is None:
             metric = 'euclidean'
         else:
             metric = Euclidean(scale)
     return metric
 
-class SquaredExponential(GP):
+class SquaredExponential(Kernel):
     def __init__(self, sill='sill', range='range', scale=None, metric=None):
         fa = dict(sill=sill, range=range)
         autoinputs = scale_to_metric(scale, metric)
         super().__init__(fa, dict(d2=autoinputs))
 
     def vars(self):
         return ppp(self.fa['sill']) + ppp(self.fa['range'])
 
     def call(self, p, e):
         v = get_parameter_values(self.fa, p)
-        return None, v['sill'] * tf.exp(-0.5 * e['d2'] / tf.square(v['range']))
+        return v['sill'] * tf.exp(-0.5 * e['d2'] / tf.square(v['range']))
 
     def reg(self, p):
         v = get_parameter_values(self.fa, p)
         return v['range']
 
-class GammaExponential(GP):
+class GammaExponential(Kernel):
     def __init__(self, range='range', sill='sill', gamma='gamma', scale=None, metric=None):
         fa = dict(sill=sill, range=range, gamma=gamma, scale=scale)
         autoinputs = scale_to_metric(scale, metric)
         super().__init__(fa, dict(d2=autoinputs))
 
     def vars(self):
         return ppp(self.fa['sill']) + ppp(self.fa['range']) + bpp(self.fa['gamma'], 0., 2.)
 
     def call(self, p, e):
         v = get_parameter_values(self.fa, p)
-        return None, v['sill'] * gamma_exp(e['d2'] / tf.square(v['range']), v['gamma'])
+        return v['sill'] * gamma_exp(e['d2'] / tf.square(v['range']), v['gamma'])
 
     def reg(self, p):
         v = get_parameter_values(self.fa, p)
         return v['range']
 
-class Wiener(GP):
+class Wiener(Kernel):
     def __init__(self, axis, start):
 
         self.axis = axis
         self.start = start
 
         # Include the element of scale corresponding to the axis of
         # integration as an explicit formal argument.
@@ -158,20 +140,20 @@
         return []
 
     def call(self, p, e):
         v = get_parameter_values(self.fa, p)
         x1 = e['locs1'][..., self.axis]
         x2 = e['locs2'][..., self.axis]
         k = tf.minimum(ed(x1, 1), ed(x2, 0)) - self.start
-        return None, k
+        return k
 
     def reg(self, p):
         return 0.
 
-class IntSquaredExponential(GP):
+class IntSquaredExponential(Kernel):
     def __init__(self, axis, start, range='range'):
 
         self.axis = axis
         self.start = start
 
         # Include the element of scale corresponding to the axis of
         # integration as an explicit formal argument.
@@ -190,20 +172,20 @@
         r = v['range']
         sdiff = (ed(x1, 1) - ed(x2, 0)) / (r * np.sqrt(2.))
         k = -tf.square(r) * (np.sqrt(np.pi) * sdiff * tf.math.erf(sdiff) + tf.exp(-tf.square(sdiff)))
         k -= k[0:1, :]
         k -= k[:, 0:1]
         k = k[1:, 1:]
 
-        return None, k
+        return k
 
     def reg(self, p):
         return 0.
 
-class IntExponential(GP):
+class IntExponential(Kernel):
     def __init__(self, axis, start, range='range'):
 
         self.axis = axis
         self.start = start
 
         # Include the element of scale corresponding to the axis of
         # integration as an explicit formal argument.
@@ -222,39 +204,39 @@
         r = v['range']
         sdiff = tf.abs(ed(x1, 1) - ed(x2, 0)) / r
         k = -tf.square(r) * (sdiff + tf.exp(-sdiff))
         k -= k[0:1, :]
         k -= k[:, 0:1]
         k = k[1:, 1:]
 
-        return None, k
+        return k
 
     def reg(self, p):
         return 0.
 
-class Noise(GP):
+class Noise(Kernel):
     def __init__(self, nugget='nugget'):
         fa = dict(nugget=nugget)
         super().__init__(fa, dict(locs1='locs1', locs2='locs2'))
 
     def vars(self):
         return ppp(self.fa['nugget'])
 
     def call(self, p, e):
         v = get_parameter_values(self.fa, p)
 
         indices1 = tf.range(tf.shape(e['locs1'])[0])
         indices2 = tf.range(tf.shape(e['locs2'])[0]) + e['offset']
         C = tf.where(tf.equal(tf.expand_dims(indices1, -1), indices2), v['nugget'], 0.)
-        return None, C
+        return C
 
     def reg(self, p):
         return 0.
 
-class Delta(GP):
+class Delta(Kernel):
     def __init__(self, dsill='dsill', axes=None):
         fa = dict(dsill=dsill)
         self.axes = axes
         super().__init__(fa, dict(pa_d2='per_axis_dist2'))
 
     def vars(self):
         return ppp(self.fa['dsill'])
@@ -265,64 +247,126 @@
         if self.axes is not None:
             n = tf.shape(e['pa_d2'])[-1]
             mask = tf.math.bincount(self.axes, minlength=n, maxlength=n, dtype=tf.float32)
             d2 = tf.einsum('abc,c->ab', e['pa_d2'], mask)
         else:
             d2 = tf.reduce_sum(e['pa_d2'], axis=-1)
 
-        return None, v['dsill'] * tf.cast(tf.equal(d2, 0.), tf.float32)
+        return v['dsill'] * tf.cast(tf.equal(d2, 0.), tf.float32)
 
     def reg(self, p):
         return 0.
 
-class Stack(GP):
-    def __init__(self, parts: List[GP]):
+class Mix(Kernel):
+    def __init__(self, inputs, weights=None):
+        self.inputs = inputs
+        fa = {}
+        ai = dict(cats1='cats1', cats2='cats2')
+
+        # Special case if weights is not given.
+        if weights is not None:
+            fa['weights'] = weights
+            ai['inputs'] = inputs
+
+        super().__init__(fa, ai)
+
+    def gather_vars(self, cache=None):
+        """Make a special version of gather_vars because
+           we want to gather variables from `inputs`
+           even when it's not in autoinputs"""
+        vv = super().gather_vars(cache)
+        for iput in self.inputs:
+            cache[id(self)] |= iput.gather_vars(cache)
+        return cache[id(self)]
+
+    def vars(self):
+        if 'weights' in self.fa:
+            return [p for row in self.fa['weights']
+                      for p in get_trend_coefs(row)]
+        else:
+            return []
+
+    def call(self, p, e):
+        v = get_parameter_values(self.fa, p)
+        if 'weights' in v:
+            weights = []
+            for row in v['weights']:
+                if isinstance(row, (tuple, list)):
+                    row = tf.stack(row)
+                    weights.append(row)
+            weights = tf.stack(weights)
+            C = tf.stack(e['inputs'], axis=-1) # [locs, locs, numinputs].
+            Aaug1 = tf.gather(weights, e['cats1']) # [locs, numinputs].
+            Aaug2 = tf.gather(weights, e['cats2']) # [locs, numinputs].
+            outer = tf.einsum('ac,bc->abc', Aaug1, Aaug2) # [locs, locs, numinputs].
+            C = tf.einsum('abc,abc->ab', C, outer) # [locs, locs].
+            return C
+        else:
+            # When weights is not given, exploit the fact that we don't have
+            # to compute every element in component covariance matrices.
+            N = len(self.inputs)
+            catcounts1 = tf.math.bincount(e['cats1'], minlength=N, maxlength=N)
+            catcounts2 = tf.math.bincount(e['cats2'], minlength=N, maxlength=N)
+            catindices1 = tf.math.cumsum(catcounts1, exclusive=True)
+            catindices2 = tf.math.cumsum(catcounts2, exclusive=True)
+            catdiffs = tf.unstack(catindices2 - catindices1, num=N)
+            locsegs1 = tf.split(e['locs1'], catcounts1, num=N)
+            locsegs2 = tf.split(e['locs2'], catcounts2, num=N)
+
+            CC = [] # Observation noise submatrices.
+            for sublocs1, sublocs2, catdiff, iput in zip(locsegs1, locsegs2, catdiffs, self.inputs):
+                cache = dict(
+                    offset = e['offset'] + catdiff,
+                    locs1 = sublocs1,
+                    locs2 = sublocs2)
+                cache['per_axis_dist2'] = PerAxisDist2().run(cache, p)
+                cache['euclidean'] = Euclidean().run(cache, p)
+                Csub = iput.run(cache, p)
+                CC.append(Csub)
+
+            return block_diag(CC)
+
+    def reg(self, sp):
+        return tf.reduce_sum([iput.reg(sp) for iput in self.inputs])
+
+class Stack(Kernel):
+    def __init__(self, parts: List[Kernel]):
         self.parts = parts
         super().__init__({}, dict(locs1='locs1', locs2='locs2', parts=parts))
 
     def vars(self):
         return [p for part in self.parts for p in part.vars()]
 
     def __add__(self, other):
-        if isinstance(other, GP):
+        if isinstance(other, Kernel):
             return Stack(self.parts + [other])
     
     def call(self, p, e):
-        MM, CC = zip(*e['parts'])
-        MM = [M for M in MM if M is not None]
-        CC = [C for C in CC if C is not None]
-        M = tf.reduce_sum(MM, axis=0)
-        C = tf.reduce_sum(CC, axis=0)
-        return M, C
+        return tf.reduce_sum(e['parts'], axis=0)
 
     def report(self, p):
         return ' '.join(part.report(p) for part in self.parts)
 
     def reg(self, p):
         return tf.reduce_sum([part.reg(p) for part in self.parts], axis=0)
 
-class Product(GP):
-    def __init__(self, parts: List[GP]):
+class Product(Kernel):
+    def __init__(self, parts: List[Kernel]):
         self.parts = parts
         super().__init__({}, dict(locs1='locs1', locs2='locs2', parts=parts))
 
     def vars(self):
         return [p for part in self.parts for p in part.vars()]
 
     def __mul__(self, other):
-        if isinstance(other, GP):
+        if isinstance(other, Kernel):
             return Product(self.parts + [other])
     
     def call(self, p, e):
-        MM, CC = zip(*e['parts'])
-        MM = [M for M in MM if M is not None]
-        CC = [C for C in CC if C is not None]
-        M = tf.reduce_prod(MM, axis=0)
-        C = tf.reduce_prod(CC, axis=0)
-        return M, C
+        return tf.reduce_prod(e['parts'], axis=0)
 
     def report(self, p):
         return ' '.join(part.report(p) for part in self.parts)
 
     def reg(self, p):
         return tf.reduce_sum([part.reg(p) for part in self.parts], axis=0)
 
@@ -348,15 +392,15 @@
 def gamma_exp(d2, gamma):
     return tf.exp(-safepow(tf.maximum(d2, 0.0), 0.5 * gamma))
 
 class Observation(Op):
 
     def __init__(self,
         coefs: List,
-        noise: GP
+        noise: Kernel
     ):
         self.coefs = coefs
         self.noise = noise
         super().__init__({}, self.noise)
 
     def vars(self):
         vv = [p for c in self.coefs for p in upp(c)]
```

### Comparing `geostat-0.7.2/src/geostat/krige.py` & `geostat-0.8.0/src/geostat/krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/src/geostat/mesh.py` & `geostat-0.8.0/src/geostat/mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/src/geostat/metric.py` & `geostat-0.8.0/src/geostat/metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/src/geostat/model.py` & `geostat-0.8.0/src/geostat/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,54 @@
 # Tensorflow is extraordinarily noisy. Catch warnings during import.
 import warnings
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     import tensorflow as tf
     import tensorflow_probability as tfp
     tfd = tfp.distributions
-    from tensorflow.linalg import LinearOperatorFullMatrix as LOFullMatrix
-    from tensorflow.linalg import LinearOperatorBlockDiag as LOBlockDiag
 
 import tensorflow_probability as tfp
 
-from . import gp
-from .op import Op
+from . import mean as mn
+from . import kernel as krn
+from .op import Op, SingletonTraceType
 from .param import PaperParameter, ParameterSpace, Bound
 from .metric import Euclidean, PerAxisDist2
 from .param import get_parameter_values, ppp, upp, bpp
 
 MVN = tfp.distributions.MultivariateNormalTriL
 
-__all__ = ['Model', 'Featurizer', 'NormalizingFeaturizer']
+__all__ = ['Featurizer', 'GP', 'Mix', 'Model', 'NormalizingFeaturizer']
+
+@dataclass
+class GP:
+    mean: mn.Trend = None
+    kernel: krn.Kernel = None
+
+    def __post_init__(self):
+        if self.mean is None or self.mean == 0:
+            self.mean = mn.ZeroTrend()
+        assert self.kernel is not None
+
+    def __add__(self, other):
+        return GP(self.mean + other.mean, self.kernel + other.kernel)
+
+    def __tf_tracing_type__(self, context):
+        return SingletonTraceType(self)
+
+    def gather_vars(self):
+        return set(self.mean.gather_vars()) | set(self.kernel.gather_vars())
+
+    def reg(self, sp):
+        return self.kernel.reg(sp)
+
+def Mix(inputs, weights=None):
+    return GP(
+        mn.Mix([i.mean for i in inputs], weights), 
+        krn.Mix([i.kernel for i in inputs], weights))
 
 class NormalizingFeaturizer:
     """
     Produces featurized locations (F matrix) and remembers normalization
     parameters.  Adds an intercept feature.
     """
     def __init__(self, featurization, locs):
@@ -68,24 +94,20 @@
                 return tf.stack(feats, axis=1)
         else: # One feature.
             return e(feats)
 
 def e(x, a=-1):
     return tf.expand_dims(x, a)
 
-def block_diag(blocks):
-    """Return a dense block-diagonal matrix."""
-    return LOBlockDiag([LOFullMatrix(b) for b in blocks]).to_dense()
-
 @tf.function
-def gp_covariance(covariance, observation, locs, cats, p):
-    return gp_covariance2(covariance, observation, locs, cats, locs, cats, 0, p)
+def gp_covariance(gp, locs, cats, p):
+    return gp_covariance2(gp, locs, cats, locs, cats, 0, p)
 
 @tf.function
-def gp_covariance2(covariance, observation, locs1, cats1, locs2, cats2, offset, p):
+def gp_covariance2(gp, locs1, cats1, locs2, cats2, offset, p):
     """
     `offset` is i2-i1, where i1 and i2 are the starting indices of locs1
     and locs2.  It is used to create the diagonal non-zero elements
     of a Noise covariance function.  An non-zero offset results in a
     covariance matrix with non-zero entries along an off-center diagonal.
     """
 
@@ -95,87 +117,47 @@
     locs1 = tf.cast(locs1, tf.float32)
     locs2 = tf.cast(locs2, tf.float32)
 
     cache = {}
     cache['offset'] = offset
     cache['locs1'] = locs1
     cache['locs2'] = locs2
+    cache['cats1'] = cats1
+    cache['cats2'] = cats2
     cache['per_axis_dist2'] = PerAxisDist2().run(cache, p)
     cache['euclidean'] = Euclidean().run(cache, p)
 
-    MM, CC = zip(*[c.run(cache, p) for c in covariance])
-    M = tf.stack(MM, axis=-1) # [locs, hidden].
-    C = tf.stack(CC, axis=-1) # [locs, locs, hidden].
-
-    numobs = len(observation)
-
-    if numobs == 0:
-        assert len(covariance) == 1, 'With no observation model, I only want one covariance model'
-        C = tf.cast(C[..., 0], tf.float64)
-        M = tf.cast(M[..., 0], tf.float64)
-        return M, C
-
-    A = tf.convert_to_tensor(gp.get_parameter_values([o.coefs for o in observation], p)) # [surface, hidden].
-    M = tf.gather(tf.einsum('lh,sh->ls', M, A), cats1, batch_dims=1) # [locs]
-
-    Aaug1 = tf.gather(A, cats1) # [locs, hidden].
-    Aaug2 = tf.gather(A, cats2) # [locs, hidden].
-    outer = tf.einsum('ac,bc->abc', Aaug1, Aaug2) # [locs, locs, hidden].
-    C = tf.einsum('abc,abc->ab', C, outer) # [locs, locs].
-
-    catcounts1 = tf.math.bincount(cats1, minlength=numobs, maxlength=numobs)
-    catcounts2 = tf.math.bincount(cats2, minlength=numobs, maxlength=numobs)
-    catindices1 = tf.math.cumsum(catcounts1, exclusive=True)
-    catindices2 = tf.math.cumsum(catcounts2, exclusive=True)
-    catdiffs = tf.unstack(catindices2 - catindices1, num=numobs)
-    locsegs1 = tf.split(locs1, catcounts1, num=numobs)
-    locsegs2 = tf.split(locs2, catcounts2, num=numobs)
-
-    CC = [] # Observation noise submatrices.
-    MM = [] # Mean subvectors.
-    for sublocs1, sublocs2, catdiff, o in zip(locsegs1, locsegs2, catdiffs, observation):
-        cache['offset'] = offset + catdiff
-        cache['locs1'] = sublocs1
-        cache['locs2'] = sublocs2
-        cache['per_axis_dist2'] = PerAxisDist2().run(cache, p)
-        cache['euclidean'] = Euclidean().run(cache, p)
-        Msub, Csub = o.noise.run(cache, p)
-        CC.append(Csub)
-        MM.append(Msub)
-
-    C += block_diag(CC)
-    C = tf.cast(C, tf.float64)
-
-    M += tf.concat(MM, axis=0)
+    M = gp.mean.run(cache, p)
+    C = gp.kernel.run(cache, p)
     M = tf.cast(M, tf.float64)
-
+    C = tf.cast(C, tf.float64)
     return M, C
 
 @tf.function
 def mvn_log_pdf(u, m, cov):
     """Log PDF of a multivariate gaussian."""
     u_adj = u - m
     logdet = tf.linalg.logdet(2 * np.pi * cov)
     quad = tf.matmul(e(u_adj, 0), tf.linalg.solve(cov, e(u_adj, -1)))[0, 0]
     return tf.cast(-0.5 * (logdet + quad), tf.float32)
 
 @tf.function
-def gp_log_likelihood(data, surf_params, covariance, observation):
-    m, S = gp_covariance(covariance, observation, data['locs'], data['cats'], surf_params)
+def gp_log_likelihood(data, surf_params, gp):
+    m, S = gp_covariance(gp, data['locs'], data['cats'], surf_params)
     u = tf.cast(data['vals'], tf.float64)
     return mvn_log_pdf(u, m, S)
 
-def gp_train_step(optimizer, data, parameters, parameter_space, covariance, observation, reg=None):
+def gp_train_step(optimizer, data, parameters, parameter_space, gp, reg=None):
     with tf.GradientTape() as tape:
         sp = parameter_space.get_surface(parameters)
 
-        ll = gp_log_likelihood(data, sp, covariance, observation)
+        ll = gp_log_likelihood(data, sp, gp)
 
         if reg:
-            reg_penalty = reg * tf.reduce_sum([c.reg(sp) for c in covariance])
+            reg_penalty = reg * gp.reg(sp)
         else:
             reg_penalty = 0.
 
         loss = -ll + reg_penalty
 
     gradients = tape.gradient(loss, parameters.values())
     optimizer.apply_gradients(zip(gradients, parameters.values()))
@@ -193,16 +175,15 @@
         assert name in values, 'Parameter `%s` is missing' % name
         assert np.all(lo <= values[name]) and np.all(values[name] <= hi), 'Parameter `%s` is out of bounds' % name
         out[name] = Bound(lo, hi)
     return out
 
 @dataclass
 class Model():
-    latent: List[gp.GP] = None
-    observed: List[gp.Observation] = None
+    gp: GP
     parameters: Dict[str, np.ndarray] = None
     parameter_sample_size: Optional[int] = None
     locs: np.ndarray = None
     vals: np.ndarray = None
     cats: np.ndarray = None
     report: Callable = None
     verbose: bool = True
@@ -218,15 +199,15 @@
                 featurization : function, optional
                     Should be a function that takes x1 (n-dim array of input data)
                     and returns the coordinates, i.e., x, y, x**2, y**2.
                     Example: def featurization(x1):
                                 return x1[:, 0], x1[:, 1], x1[:, 0]**2, x1[:, 1]**2.
                     Default is None.
 
-                latent : List[gp.GP]
+                latent : List[GP]
                      Name of the covariance function to use in the GP.
                      Should be 'squared-exp' or 'gamma-exp'.
                      Default is 'squared-exp'.
 
                 parameters : dict, optional
                     The starting point for the parameters.
                     Example: parameters=dict(range=2.0, sill=5.0, nugget=1.0).
@@ -235,22 +216,14 @@
                 verbose : boolean, optional
                     Whether or not to print parameters.
                     Default is True.
 
         Performs Gaussian process training and prediction.
         '''
 
-        super().__init__()
-
-        assert self.latent is not None, 'I need at least one latent variable'
-        if isinstance(self.latent, gp.GP):
-            self.latent = [self.latent]
-
-        if self.observed is None: self.observed = []
-
         # Default reporting function.
         def default_report(p, prefix=None):
             if prefix: print(prefix, end=' ')
 
             def fmt(x):
                 if isinstance(x, tf.Tensor):
                     x = x.numpy()
@@ -269,18 +242,16 @@
 
         if self.locs is not None: self.locs = np.array(self.locs)
         if self.vals is not None: self.vals = np.array(self.vals)
         if self.cats is not None: self.cats = np.array(self.cats)
 
         # Collect paraameters.
         if self.parameters is None: self.parameters = {}
-        vv = {v for c in self.latent for v in c.gather_vars()}
-        vv |= {v for o in self.observed for v in o.gather_vars()}
 
-        self.parameter_space = ParameterSpace(check_parameters(vv, self.parameters))
+        self.parameter_space = ParameterSpace(check_parameters(self.gp.gather_vars(), self.parameters))
 
     def fit(self, locs, vals, cats=None,
         step_size=0.01, iters=100, reg=None):
 
         # Permute datapoints if cats is given.
         if cats is not None:
             cats = np.array(cats)
@@ -298,15 +269,15 @@
         optimizer = tf.keras.optimizers.Adam(learning_rate=step_size)
 
         j = 0 # Iteration count.
         for i in range(10):
             t0 = time.time()
             while j < (i + 1) * iters / 10:
                 p, ll, reg_penalty = gp_train_step(optimizer, self.data, up, self.parameter_space,
-                    self.latent, self.observed, reg)
+                    self.gp, reg)
                 j += 1
 
             time_elapsed = time.time() - t0
             if self.verbose == True:
                 self.report(dict(iter=j, ll=ll, time=time_elapsed, reg=reg_penalty, **p))
 
         new_parameters = self.parameter_space.get_surface(up, numpy=True)
@@ -339,15 +310,15 @@
 
         # Initial MCMC state.
         initial_up = self.parameter_space.get_underlying(self.parameters)
 
         # Unnormalized log posterior distribution.
         def g(up):
             sp = self.parameter_space.get_surface(up)
-            return gp_log_likelihood(self.data, sp, self.latent, self.observed)
+            return gp_log_likelihood(self.data, sp, self.gp)
 
         def f(*up_flat):
             up = tf.nest.pack_sequence_as(initial_up, up_flat)
             ll = tf.map_fn(g, up, fn_output_signature=tf.float32)
             # log_prior = -tf.reduce_sum(tf.math.log(1. + tf.square(up_flat)), axis=0)
             return ll # + log_prior
 
@@ -454,16 +425,15 @@
             locs, cats = locs[perm], cats[perm]
 
         up = self.parameter_space.get_underlying(self.parameters)
 
         p = self.parameter_space.get_surface(up)
 
         m, S = gp_covariance(
-            self.latent,
-            self.observed,
+            self.gp,
             tf.constant(locs, dtype=tf.float32),
             None if cats is None else tf.constant(cats, dtype=tf.int32),
             p)
 
         vals = MVN(m, tf.linalg.cholesky(S)).sample().numpy()
 
         # Restore order if things were permuted.
@@ -500,26 +470,24 @@
 
             # Permute datapoints if cats is given.
             if cats2 is not None:
                 perm = np.argsort(cats2)
                 locs2, cats2 = locs2[perm], cats2[perm]
 
             _, A12 = gp_covariance2(
-                self.latent,
-                self.observed,
+                self.gp,
                 tf.constant(locs1, dtype=tf.float32),
                 None if cats1 is None else tf.constant(cats1, dtype=tf.int32),
                 tf.constant(locs2, dtype=tf.float32),
                 None if cats2 is None else tf.constant(cats2, dtype=tf.int32),
                 N1,
                 parameters)
 
             m2, A22 = gp_covariance(
-                self.latent,
-                self.observed,
+                self.gp,
                 tf.constant(locs2, dtype=tf.float32),
                 None if cats2 is None else tf.constant(cats2, dtype=tf.int32),
                 parameters)
 
             # Restore order if things were permuted.
             if cats2 is not None:
                 revperm = np.argsort(perm)
@@ -550,16 +518,15 @@
 
             # Permute datapoints if cats is given.
             if cats1 is not None:
                 perm = np.argsort(cats1)
                 locs1, vals1, cats1 = locs1[perm], vals1[perm], cats1[perm]
 
             m1, A11 = gp_covariance(
-                self.latent,
-                self.observed,
+                self.gp,
                 tf.constant(locs1, dtype=tf.float32),
                 None if cats1 is None else tf.constant(cats1, dtype=tf.int32),
                 parameters)
 
             A11i = tf.linalg.inv(A11)
 
             u2_mean_s = []
```

### Comparing `geostat-0.7.2/src/geostat/op.py` & `geostat-0.8.0/src/geostat/op.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,19 @@
     fa: Dict[str, object] # Formal arguments.
     autoinputs: object # Blob of Ops and strings.
 
     def vars(self): # Parameters
         return []
 
     def gather_vars(self, cache=None):
+        """`cache` maps from Op ids to sets of variable names."""
         if cache is None: cache = {}
         if id(self) not in cache:
             vv = {v for op in tf.nest.flatten(self.autoinputs) if isinstance(op, Op) for v in op.gather_vars(cache)}
+            # print(self, '<-', [x.name for x in vv], '|', [x.name for x in set(self.vars())], '\n')
             cache[id(self)] = vv | set(self.vars())
         return cache[id(self)]
 
     def __call__(self, p, e):
         """
         `p` is a dict of model parameters.
```

### Comparing `geostat-0.7.2/src/geostat/param.py` & `geostat-0.8.0/src/geostat/param.py`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/src/geostat.egg-info/PKG-INFO` & `geostat-0.8.0/src/geostat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.7.2
+Version: 0.8.0
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.7.2/src/geostat.egg-info/SOURCES.txt` & `geostat-0.8.0/src/geostat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/geostat/__init__.py
-src/geostat/gp.py
+src/geostat/kernel.py
 src/geostat/krige.py
+src/geostat/mean.py
 src/geostat/mesh.py
 src/geostat/metric.py
 src/geostat/model.py
 src/geostat/op.py
 src/geostat/param.py
 src/geostat.egg-info/PKG-INFO
 src/geostat.egg-info/SOURCES.txt
```

### Comparing `geostat-0.7.2/tests/test_antiderivative.py` & `geostat-0.8.0/tests/test_antiderivative.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import tensorflow as tf
-from geostat import gp, Model, Mesh, NormalizingFeaturizer
+from geostat import GP, Model, Mesh, NormalizingFeaturizer
+import geostat.kernel as krn
 
 
 def test_int_sq_exp():
 
     np.random.seed(2)
     tf.random.set_seed(2)
 
@@ -13,31 +14,33 @@
     ydim = 0.5
 
     mesh = Mesh.from_bounds([0., 0., xdim, ydim], nx=numsteps)
     def trend_terms(x, y): return x, y, x*x, x*y, y*y
     featurizer = NormalizingFeaturizer(trend_terms, mesh.locations())
 
     mesh_vals = Model(
-        gp.SquaredExponential(scale=[1., 1.]) + gp.Noise(nugget=1e-4),
+        GP(0, krn.SquaredExponential(scale=[1., 1.]) + krn.Noise(nugget=1e-4)),
         parameters = dict(range=0.1, sill=1.),
         verbose=True).generate(mesh.locations()).vals
 
     vmin, vmax = mesh_vals.min(), mesh_vals.max()
     meshx, meshy, mesh_vals_2d = mesh.slice(mesh_vals) # Each return value is a 2d array.
 
     int_vals = np.cumsum(mesh_vals_2d, axis=-1) / numsteps * xdim # Numerical integration on x-axis.
 
     sample_indices = np.random.choice(len(int_vals.ravel()), [500], replace=False)
     locs = np.stack([meshx.ravel()[sample_indices], meshy.ravel()[sample_indices]], axis=-1)
     vals = int_vals.ravel()[sample_indices]
 
+    kernel = krn.SquaredExponential(scale=[0., 1.], range='y_range') * \
+        krn.IntSquaredExponential(axis=0, start=0., range='x_range') + \
+        krn.Noise(nugget=1e-4)
+
     model = Model(
-        gp.SquaredExponential(scale=[0., 1.], range='y_range') * \
-        gp.IntSquaredExponential(axis=0, start=0., range='x_range') + \
-        gp.Noise(nugget=1e-4),
+        GP(0, kernel),
         parameters = dict(x_range=1., y_range=1., sill=2.),
         verbose=True).fit(locs, vals, iters=2000, step_size=1e-1)
 
     assert np.allclose(
         [model.parameters[p] for p in ['x_range', 'y_range', 'sill']],
         [0.1, 0.1, 1.],
         rtol=0.5)
@@ -51,33 +54,38 @@
     xdim = 4.
     ydim = 0.5
 
     mesh = Mesh.from_bounds([0., 0., xdim, ydim], nx=numsteps)
     def trend_terms(x, y): return x, y, x*x, x*y, y*y
     featurizer = NormalizingFeaturizer(trend_terms, mesh.locations())
 
+    kernel1 = krn.SquaredExponential(scale=[0., 1.]) * \
+        krn.GammaExponential(scale=[1., 0.], sill=1., gamma=1.) + krn.Noise(nugget=1e-4)
+
     mesh_vals = Model(
-        gp.SquaredExponential(scale=[0., 1.]) *
-        gp.GammaExponential(scale=[1., 0.], sill=1., gamma=1.) + gp.Noise(nugget=1e-4),
+        GP(0, kernel1),
         parameters = dict(range=0.1, sill=1.),
         verbose=True).generate(mesh.locations()).vals
 
     vmin, vmax = mesh_vals.min(), mesh_vals.max()
     meshx, meshy, mesh_vals_2d = mesh.slice(mesh_vals) # Each return value is a 2d array.
 
     int_vals = np.cumsum(mesh_vals_2d, axis=-1) / numsteps * xdim # Numerical integration on x-axis.
 
     sample_indices = np.random.choice(len(int_vals.ravel()), [500], replace=False)
     locs = np.stack([meshx.ravel()[sample_indices], meshy.ravel()[sample_indices]], axis=-1)
     vals = int_vals.ravel()[sample_indices]
 
+    kernel2 = \
+        krn.SquaredExponential(scale=[0., 1.], range='y_range') * \
+        krn.IntExponential(axis=0, start=0., range='x_range') + \
+        krn.Noise(nugget=1e-3)
+
     model = Model(
-        gp.SquaredExponential(scale=[0., 1.], range='y_range') * \
-        gp.IntExponential(axis=0, start=0., range='x_range') + \
-        gp.Noise(nugget=1e-3),
+        GP(0, kernel2),
         parameters = dict(x_range=1., y_range=1., sill=2.),
         verbose=True).fit(locs, vals, iters=2000, step_size=1e-1)
 
     assert np.allclose(
         [model.parameters[p] for p in ['x_range', 'y_range', 'sill']],
         [0.1, 0.1, 1.],
         rtol=0.5)
@@ -90,32 +98,37 @@
     numsteps = 80
     xdim = 2.
 
     mesh = Mesh.from_bounds([0., 0., xdim, 1.], nx=numsteps)
     def trend_terms(x, y): return x, y, x*x, x*y, y*y
     featurizer = NormalizingFeaturizer(trend_terms, mesh.locations())
 
+    kernel1 = \
+        krn.SquaredExponential(scale=[0., 1.], sill=1., range=0.3) * \
+        krn.SquaredExponential(scale=[1., 0.], sill=1., range=1e-4) + krn.Noise(nugget=1e-4)
+
     mesh_vals = Model(
-        gp.SquaredExponential(scale=[0., 1.], sill=1., range=0.3) *
-        gp.SquaredExponential(scale=[1., 0.], sill=1., range=1e-4) + gp.Noise(nugget=1e-4),
+        GP(0, kernel1),
         parameters = dict(),
         verbose=True).generate(mesh.locations()).vals
 
     vmin, vmax = mesh_vals.min(), mesh_vals.max()
     meshx, meshy, mesh_vals_2d = mesh.slice(mesh_vals) # Each return value is a 2d array.
 
     # Numerical integration on x-axis. Scaling is tricky.
     int_vals = np.cumsum(mesh_vals_2d, axis=-1) / np.sqrt(numsteps / xdim)
 
     sample_indices = np.random.choice(len(int_vals.ravel()), [500], replace=False)
     locs = np.stack([meshx.ravel()[sample_indices], meshy.ravel()[sample_indices]], axis=-1)
     vals = int_vals.ravel()[sample_indices]
 
+    kernel2 = krn.SquaredExponential(scale=[0., 1.]) * krn.Wiener(axis=0, start=0.) + krn.Noise(nugget=1e-4)
+
     model = Model(
-        gp.SquaredExponential(scale=[0., 1.]) * gp.Wiener(axis=0, start=0.) + gp.Noise(nugget=1e-4),
+        GP(0, kernel2),
         parameters = dict(range=1., sill=2.),
         verbose=True).fit(locs, vals, iters=2000, step_size=1e-1)
 
     assert np.allclose(
         [model.parameters[p] for p in ['range', 'sill']],
         [0.3, 1.],
         rtol=0.5)
```

### Comparing `geostat-0.7.2/tests/test_gp.py` & `geostat-0.8.0/tests/test_trend.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,126 @@
 import numpy as np
-from geostat import gp, Model, NormalizingFeaturizer
+from geostat import gp, Model, Featurizer, NormalizingFeaturizer
+import geostat.kernel as krn
 
-
-def test_gp2d():
+def test_coefs1():
     # Create 100 random locations in a square centered on the origin.
-    locs1 = np.random.uniform(-1., 1., [500, 2])
+    locs1 = np.random.uniform(-1., 1., [100, 2])
 
     # Initialize featurizer of location for trends.
-    def trend_terms(x, y): return x, y, x*y
-    featurizer = NormalizingFeaturizer(trend_terms, locs1)
-    covariance = gp.TrendPrior(featurizer) + gp.SquaredExponential(sill=1.) + gp.Noise()
+    def trend_terms(x, y): return 1, y
+    featurizer = Featurizer(trend_terms)
+    gp = GP(Trend(featurizer, beta='b'),
+            krn.SquaredExponential(range=0.5, sill=0.01) + krn.Noise())
 
     # Generating GP.
     model1 = Model(
-        latent = covariance,
-        parameters = dict(alpha=1., range=0.5, nugget=1.),
-        verbose=True)
+        gp,
+        parameters = dict(b=[1.0, 0.5], nugget=0.1),
+        verbose = True)
 
     # Generate data.
     vals1 = model1.generate(locs1).vals
 
     # Fit GP.
     model2 = Model(
-        latent = covariance,
-        parameters = dict(alpha=2., range=1., nugget=0.5),
-        verbose=True).fit(locs1, vals1, iters=200)
+        gp,
+        parameters = dict(b=[1.0, 0.5], nugget=0.1),
+        verbose = True).fit(locs1, vals1, iters=200)
+    print()
 
     # Interpolate using GP.
-    N = 20
-    xx, yy = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N))
+    N = 2
+    xx, yy = np.meshgrid(np.linspace(0, 1, N), np.linspace(0, 1, N))
     locs2 = np.stack([xx, yy], axis=-1).reshape([-1, 2])
 
     mean, var = model2.predict(locs2)
-    mean2, var2 = model2.predict(locs2)
 
-    assert np.all(mean == mean2)
-    assert np.all(var == var2)
+    target_mean = [1., 1., 1.5, 1.5]
 
+    assert np.square(mean - target_mean).mean() < 0.1
 
-def test_gp3d():
-    # Create 100 random locations in a square centered on the origin.
-    locs1 = np.random.uniform(-1., 1., [500, 3])
+def test_coefs2():
+    # Create 500 random locations in a square centered on the origin.
+    locs1 = np.random.uniform(-1., 1., [500, 2])
 
     # Initialize featurizer of location for trends.
-    def trend_terms(x, y, z): return z, z*z
+    def trend_terms(x, y): return x, y, x*y
     featurizer = NormalizingFeaturizer(trend_terms, locs1)
-    covariance = \
-        gp.TrendPrior(featurizer) + \
-        gp.GammaExponential(scale=[1., 1., 'zscale']) + \
-        gp.Delta(axes=[0, 1]) + \
-        gp.Noise()
+    gp = GP(Trend(featurizer, beta=[1., 'b1', 'b2', 'b3']),
+            krn.SquaredExponential(sill=1.) + krn.Noise())
 
     # Generating GP.
     model1 = Model(
-        latent = covariance,
-        parameters = dict(alpha=1., zscale=5., range=0.5, sill=1., gamma=1., dsill=1., nugget=1.),
-        verbose=True)
+        gp,
+        parameters = dict(b1=0.5, b2=0.5, b3=0.25, range=0.5, nugget=1.),
+        verbose = True)
 
     # Generate data.
     vals1 = model1.generate(locs1).vals
 
     # Fit GP.
     model2 = Model(
-        latent = covariance,
-        parameters = dict(alpha=2., zscale=1., range=1.0, sill=0.5, gamma=0.5, dsill=0.5, nugget=0.5),
-        verbose=True).fit(locs1, vals1, iters=500)
+        gp,
+        parameters = dict(b1=0., b2=0., b3=0., range=1., nugget=0.5),
+        verbose = True).fit(locs1, vals1, iters=200)
+    print()
+
+    # MCMC.
+    model3 = Model(
+        gp,
+        parameters = dict(b1=0., b2=0., b3=0., range=1., nugget=0.5),
+        verbose = True).mcmc(locs1, vals1, burnin=500, samples=500)
 
     # Interpolate using GP.
-    N = 10
-    xx, yy, zz = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N), np.linspace(-1, 1, N))
-    locs2 = np.stack([xx, yy, zz], axis=-1).reshape([-1, 3])
+    N = 20
+    xx, yy = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N))
+    locs2 = np.stack([xx, yy], axis=-1).reshape([-1, 2])
 
     mean, var = model2.predict(locs2)
     mean2, var2 = model2.predict(locs2)
 
     assert np.all(mean == mean2)
     assert np.all(var == var2)
 
-
-def test_gp3d_stacked():
-    # Create random locations centered on the origin.
-    locs1 = np.random.normal(size=[1000, 3])
+def test_explicit_trend():
+    # Create 500 random locations in a square centered on the origin.
+    locs1 = np.random.uniform(-1., 1., [500, 2])
 
     # Initialize featurizer of location for trends.
-    def trend_terms(x, y, z): return z, z*z
+    def trend_terms(x, y): return x, y, x*y
     featurizer = NormalizingFeaturizer(trend_terms, locs1)
-
-    # Covariance structure
-    covariance = \
-        gp.TrendPrior(featurizer) + \
-        gp.SquaredExponential(range='r1', sill='s1', scale=[1., 1., 'zscale']) + \
-        gp.SquaredExponential(range='r2', sill='s2', scale=[1., 1., 0.]) + \
-        gp.Noise()
+    gp = GP(Trend(featurizer, beta='beta'),
+            krn.SquaredExponential(sill=1.) + krn.Noise())
 
     # Generating GP.
     model1 = Model(
-        latent = covariance,
-        parameters = dict(alpha=1., zscale=5., r1=0.25, s1=1., r2=1.0, s2=0.25, nugget=1.),
-        verbose=True)
+        gp,
+        parameters = dict(beta=[1., 0.5, 0.5, 0.25], range=0.5, nugget=1.),
+        verbose = True)
 
     # Generate data.
     vals1 = model1.generate(locs1).vals
 
     # Fit GP.
     model2 = Model(
-        latent = covariance,
-        parameters = dict(alpha=2., zscale=2.5, r1=0.125, s1=0.5, r2=0.5, s2=0.125, nugget=0.5),
-        verbose=True).fit(locs1, vals1, iters=500)
+        gp,
+        parameters = dict(beta=[0., 0., 0., 0.], range=1., nugget=0.5),
+        verbose = True).fit(locs1, vals1, iters=200)
+    print()
+
+    # MCMC.
+    model3 = Model(
+        gp,
+        parameters = dict(beta=[0., 0., 0., 0.], range=1., nugget=0.5),
+        verbose = True).mcmc(locs1, vals1, burnin=500, samples=500)
 
     # Interpolate using GP.
-    N = 10
-    xx, yy, zz = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N), np.linspace(-1, 1, N))
-    locs2 = np.stack([xx, yy, zz], axis=-1).reshape([-1, 3])
+    N = 20
+    xx, yy = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N))
+    locs2 = np.stack([xx, yy], axis=-1).reshape([-1, 2])
 
     mean, var = model2.predict(locs2)
     mean2, var2 = model2.predict(locs2)
 
     assert np.all(mean == mean2)
     assert np.all(var == var2)
```

### Comparing `geostat-0.7.2/tests/test_krige.py` & `geostat-0.8.0/tests/test_krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/tests/test_mcmc.py` & `geostat-0.8.0/tests/test_mcmc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import numpy as np
-from geostat import gp, Model, Featurizer, NormalizingFeaturizer
+from geostat import GP, Model, Featurizer, NormalizingFeaturizer, Mix, Trend
+import geostat.kernel as krn
 from types import SimpleNamespace
 
 def test_mcmc():
     
     # Create 100 random locations in a square centered on the origin.
     locs1 = np.random.uniform(-1., 1., [1000, 2])
 
     # Initialize featurizer of location for trends.
     def trend_terms(x, y): return x, y, x*y
     featurizer = NormalizingFeaturizer(trend_terms, locs1)
-    covariance = gp.TrendPrior(featurizer) + gp.SquaredExponential(sill=1.) + gp.Noise()
+    kernel = krn.TrendPrior(featurizer) + krn.SquaredExponential(sill=1.) + krn.Noise()
 
     # Generating GP.
     model1 = Model(
-        latent = covariance,
+        GP(0, kernel),
         parameters = dict(alpha=1., range=0.5, nugget=1.),
         verbose=True)
 
     # Generate data.
     vals1 = model1.generate(locs1).vals
 
     # Fit GP.
     model2 = Model(
-        latent = covariance,
+        GP(0, kernel),
         parameters = dict(alpha=2., range=1., nugget=0.5),
         verbose=True).mcmc(locs1, vals1,
             step_size=0.05, samples=100, burnin=100, report_interval=50)
 
     # Interpolate using GP.
     N = 20
     xx, yy = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N))
@@ -43,26 +44,27 @@
     # Triple data with offsets.
     N *= 3
     locs1 = np.concatenate([locs1 - [0.1, 0], locs1, locs1 + [0.1, 0]], axis=-1).reshape([-1, 2])
 
     # Initialize featurizer of location for trends.
     def trend_terms(x, y): return x, y, x*y
     featurizer = NormalizingFeaturizer(trend_terms, locs1)
-    cov1 = gp.TrendPrior(featurizer, alpha='a1') + gp.SquaredExponential(sill='s1', range='r1')
-    cov2 = gp.TrendPrior(featurizer, alpha='a2') + gp.SquaredExponential(sill='s2', range='r2')
+    in1 = GP(0, krn.TrendPrior(featurizer, alpha='a1') + krn.SquaredExponential(sill='s1', range='r1'))
+    in2 = GP(0, krn.TrendPrior(featurizer, alpha='a2') + krn.SquaredExponential(sill='s2', range='r2'))
 
     f2 = Featurizer(lambda x, y: (1, x + y*y))
-    obs1 = gp.Observation([1., 0.], gp.Trend(f2, beta=[0., 0.]) + gp.Noise(nugget='n1'))
-    obs2 = gp.Observation([0., 1.], gp.Trend(f2, beta=[1., 0.]) + gp.Noise(nugget='n2'))
-    obs3 = gp.Observation(['k1', 'k2'], gp.Trend(f2, beta=[0., 1.]) + gp.Noise(nugget='n3') + gp.Delta(dsill='d', axes=[1]))
+    out1 = GP(Trend(f2, beta=[0., 0.]), krn.Noise(nugget='n1'))
+    out2 = GP(Trend(f2, beta=[1., 0.]), krn.Noise(nugget='n2'))
+    out3 = GP(Trend(f2, beta=[0., 1.]), krn.Noise(nugget='n3') + krn.Delta(dsill='d', axes=[1]))
+
+    gp = Mix([in1, in2], [[1., 0.], [0., 1.], ['k1', 'k2']]) + Mix([out1, out2, out3])
 
     # Generating GP.
     model1 = Model(
-        latent = [cov1, cov2],
-        observed = [obs1, obs2, obs3],
+        gp,
         parameters = dict(
             a1=1., s1=1., r1=0.5, k1=2.,
             a2=1., s2=1., r2=0.5, k2=3.,
             n1=0.1, n2=0.2, n3=0.3, d=0.1),
         verbose=True)
 
     # Generate data.
@@ -75,16 +77,15 @@
         print('{} {:5.3s} {:5.3s} {:5.3s} {:5.3s} {:5.3s} {:5.3s} {:5.3s}'.format(prefix, '', 'a', 's', 'r', 'k', 'n', 'd'))
         print('{} {:5.3s} {:5.3f} {:5.3f} {:5.3f} {:5.3f} {:5.3f} {:5.3s}'.format(prefix, '1', x.a1, x.s1, x.r1, x.k1, x.n1, ''))
         print('{} {:5.3s} {:5.3f} {:5.3f} {:5.3f} {:5.3f} {:5.3f} {:5.3s}'.format(prefix, '2', x.a2, x.s2, x.r2, x.k2, x.n2, ''))
         print('{} {:5.3s} {:5.3s} {:5.3s} {:5.3s} {:5.3s} {:5.3f} {:5.3f}'.format(prefix, '3', '', '', '', '', x.n3, x.d))
 
     # Fit GP.
     model2 = Model(
-        latent = [cov1, cov2],
-        observed = [obs1, obs2, obs3],
+        gp,
         parameters = dict(
             a1=1., s1=1., r1=1., k1=0.,
             a2=1., s2=1., r2=1., k2=0.,
             n1=0.1, n2=0.1, n3=0.1, d=0.1),
         report=report,
         verbose=True
     ).mcmc(locs1, vals1, cats1,
```

### Comparing `geostat-0.7.2/tests/test_mesh.py` & `geostat-0.8.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.7.2/tests/test_metric.py` & `geostat-0.8.0/tests/test_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import geostat.metric as gm
 
 def test_euclidean():
     # Create 100 random locations in a square centered on the origin.
     locs = np.random.uniform(-1., 1., [1000, 3])
 
     metric = gm.Euclidean(scale=[1., 1., 'zscale'])
-    covariance = \
-        gp.GammaExponential(metric=metric) + \
-        gp.SquaredExponential(range=2., sill='alpha') + \
-        gp.Noise()
+    kernel = GP(0,
+        krn.GammaExponential(metric=metric) +
+        krn.SquaredExponential(range=2., sill='alpha') +
+        krn.Noise())
 
     # Generating GP.
     model1 = Model(
-        latent = covariance,
+        latent = kernel,
         parameters = dict(alpha=1., zscale=5., range=0.5, sill=1., gamma=1., nugget=1.),
         verbose=True)
 
     # Generate data.
     vals = model1.generate(locs).vals
 
     # Fit GP.
     model2 = Model(
-        latent = covariance,
+        latent = kernel,
         parameters = dict(alpha=2., zscale=1., range=1.0, sill=0.5, gamma=0.5, nugget=0.5),
         verbose=True).fit(locs, vals, iters=500)
 
     # Interpolate using GP.
     N = 10
     xx, yy, zz = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N), np.linspace(-1, 1, N))
     locs2 = np.stack([xx, yy, zz], axis=-1).reshape([-1, 3])
@@ -46,31 +46,31 @@
     locs[:, 2] = 3. - np.exp(locs[:, 2]) # Make z to be 3 or lower.
 
     # Transform z to be positive, and make it the first axis.
     zmax = locs[:, 2].max()
     def xform(x, y, z): return zmax-z, x, y
 
     metric = gm.Poincare(xform=xform, scale=['zscale', 1., 1.], zoff='zoff')
-    covariance = \
-        gp.GammaExponential(metric=metric) + \
-        gp.SquaredExponential(metric=metric, range=2., sill='alpha') + \
-        gp.Noise()
+    kernel = GP(0,
+        krn.GammaExponential(metric=metric) +
+        krn.SquaredExponential(metric=metric, range=2., sill='alpha') +
+        krn.Noise())
 
     # Generating GP.
     model1 = Model(
-        latent = covariance,
+        latent = kernel,
         parameters = dict(zoff=2.0, alpha=1., zscale=5., range=0.5, sill=1., gamma=1., nugget=1.),
         verbose=True)
 
     # Generate data.
     vals = model1.generate(locs).vals
 
     # Fit GP.
     model2 = Model(
-        latent = covariance,
+        latent = kernel,
         parameters = dict(zoff=2.0, alpha=2., zscale=1., range=1.0, sill=0.5, gamma=0.5, nugget=0.5),
         verbose=True).fit(locs, vals, iters=500)
 
     # Interpolate using GP.
     N = 10
     xx, yy, zz = np.meshgrid(np.linspace(-1, 1, N), np.linspace(-1, 1, N), np.linspace(-1, 1, N))
     locs2 = np.stack([xx, yy, zz], axis=-1).reshape([-1, 3])
```

