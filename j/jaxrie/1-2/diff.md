# Comparing `tmp/jaxrie-1.tar.gz` & `tmp/jaxrie-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrie-1.tar", last modified: Fri Apr  7 20:59:53 2023, max compression
+gzip compressed data, was "jaxrie-2.tar", last modified: Tue Apr 11 06:28:50 2023, max compression
```

## Comparing `jaxrie-1.tar` & `jaxrie-2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0       30 2023-03-13 06:20:14.074104 jaxrie-1/README.md
--rw-r--r--   0        0        0     3950 2023-04-07 20:59:53.653905 jaxrie-1/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-07 20:46:24.940931 jaxrie-1/src/jaxrie/__init__.py
--rw-r--r--   0        0        0       18 2023-04-07 20:40:04.578896 jaxrie-1/src/jaxrie/__version__.py
--rw-r--r--   0        0        0      183 2023-04-07 20:42:03.402217 jaxrie-1/src/jaxrie/manifold/__init__.py
--rw-r--r--   0        0        0     3537 2023-04-06 23:07:18.982516 jaxrie-1/src/jaxrie/manifold/base.py
--rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-1/src/jaxrie/manifold/lorentz.py
--rw-r--r--   0        0        0    22397 2023-04-07 18:35:05.145985 jaxrie-1/src/jaxrie/manifold/math.py
--rw-r--r--   0        0        0     4790 2023-04-07 20:36:56.242091 jaxrie-1/src/jaxrie/manifold/stereographic.py
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 jaxrie-1/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-2/README.md
+-rw-r--r--   0        0        0     3959 2023-04-11 06:28:50.427612 jaxrie-2/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-04-11 06:06:22.543202 jaxrie-2/src/jaxrie/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-11 06:25:07.371360 jaxrie-2/src/jaxrie/__version__.py
+-rw-r--r--   0        0        0      183 2023-04-07 20:42:03.402217 jaxrie-2/src/jaxrie/manifold/__init__.py
+-rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-2/src/jaxrie/manifold/base.py
+-rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-2/src/jaxrie/manifold/lorentz.py
+-rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-2/src/jaxrie/manifold/math.py
+-rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-2/src/jaxrie/manifold/stereographic.py
+-rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-2/src/jaxrie/modules/__init__.py
+-rw-r--r--   0        0        0     4816 2023-04-11 06:13:42.344173 jaxrie-2/src/jaxrie/modules/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-2/src/jaxrie/nets/__init__.py
+-rw-r--r--   0        0        0     2342 2023-04-11 06:23:40.424342 jaxrie-2/src/jaxrie/nets/basic.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-2/PKG-INFO
```

### Comparing `jaxrie-1/pyproject.toml` & `jaxrie-2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 ]
 import_heading_plot = "Plot"
 import_heading_thirdparty = "Others"
 import_heading_localfolder = "Local"
 known_localfolder = [
     "sites",
     "src",
+    "jaxrie",
 ]
 import_heading_utils = "Utils"
 known_utils = [
     "tqdm",
     "rich",
 ]
 sections = [
@@ -210,28 +211,28 @@
 
 [tool.pyink]
 pyink_indentation = 2
 preview = true
 
 [project]
 name = "jaxrie"
-description = "Riemannian with JAX"
+description = "Riemannian JAX"
 authors = [
     { name = "Nasy", email = "nasyxx+git@gmail.com" },
 ]
 dependencies = [
     "jax>=0.4.6",
     "jaxlib>=0.4.6",
     "dm-haiku>=0.0.9",
     "optax>=0.1.4",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 dynamic = []
-version = "1"
+version = "2"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `jaxrie-1/src/jaxrie/manifold/base.py` & `jaxrie-2/src/jaxrie/manifold/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,85 +33,98 @@
 license  : MIT
 
 Manifold base.
 """
 import jax
 from jax.typing import ArrayLike
 from abc import abstractmethod, ABCMeta
+from .math import EPS
 
 Array = jax.Array
 
 
 class Manifold(metaclass=ABCMeta):
   """Manifold base."""
 
   @staticmethod
   @abstractmethod
-  def add(x: Array, y: Array, k: ArrayLike, eps: float) -> Array:
+  def add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Addition on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def sub(x: Array, y: Array, k: ArrayLike, eps: float) -> Array:
+  def adde(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
+    """Addition on manifold (left H, right E) with curvature k."""
+    raise NotImplementedError
+
+  @staticmethod
+  @abstractmethod
+  def sub(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Subtraction on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def mul(r: Array, x: Array, k: ArrayLike, eps: float) -> Array:
+  def mul(r: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Scala multiplication on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def matvec(m: Array, x: Array, k: ArrayLike, eps: float) -> Array:
+  def matvec(m: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix vector multiplication on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def matmul(x1: Array, x2: Array, k: ArrayLike, eps: float) -> Array:
+  def matmul(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix multiplication on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def matmull(x1: Array, x2: Array, k: ArrayLike, eps: float) -> Array:
+  def matmull(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix multiplication (left H, right E) with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def matmulr(x1: Array, x2: Array, k: ArrayLike, eps: float) -> Array:
+  def matmulr(x1: Array, x2: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Matrix multiplication (left E, right H) with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def expmap(x: Array, y: Array, k: ArrayLike, eps: float) -> Array:
+  def expmap(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Exponential map on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def logmap(x: Array, y: Array, k: ArrayLike, eps: float) -> Array:
+  def logmap(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Logarithm map on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def expmap0(u: Array, k: ArrayLike, eps: float) -> Array:
+  def expmap0(u: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Exponential map on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def logmap0(y: Array, k: ArrayLike, eps: float) -> Array:
+  def logmap0(y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Logarithm map on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
   @abstractmethod
-  def egrad2rgrad(x: Array, grad: Array, k: ArrayLike, eps: float) -> Array:
+  def egrad2rgrad(x: Array, grad: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Euclidean gradient to Riemannian gradient."""
     raise NotImplementedError
+
+  @staticmethod
+  @abstractmethod
+  def proj(x: Array, k: ArrayLike, eps: float = EPS) -> Array:
+    """Projection on manifold with curvature k."""
+    raise NotImplementedError
```

### Comparing `jaxrie-1/src/jaxrie/manifold/lorentz.py` & `jaxrie-2/src/jaxrie/manifold/lorentz.py`

 * *Files identical despite different names*

### Comparing `jaxrie-1/src/jaxrie/manifold/math.py` & `jaxrie-2/src/jaxrie/manifold/math.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,19 +306,20 @@
   sqny = k * sqnorm(y, axis=-1, keepdims=True)
   xy = k * inner(x, y, axis=-1, keepdims=True)
   num = (1 - 2 * xy - sqny) * x + (1 + sqnx) * y
   denom = 1 - 2 * xy + sqnx * sqny
   return safe_div(num, denom, eps=eps)
 
 
-# TODO
 @partial(jax.jit, static_argnames=("eps",), inline=True)
 def mobius_adde(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
-  """Mobius addition of two vectors x(in H) & y(in E) in manifold with curvature k."""
-  return stereo_expmap(x, stereo_ptrans0(x, y, k, eps=eps), k, eps=eps)
+  """Mobius addition of two vectors x(in H) & y(in E) with curvature k."""
+  return stereo_expmap(
+      x, stereo_ptrans0(x, y, k, eps=eps), k, eps=eps
+  )
 
 
 @partial(jax.jit, static_argnames=("eps",), inline=True)
 def mobius_scala_mul(alpha: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Mobius multiplication of a vector by a scalar in manifold with curvature k."""
   c = radius(k, eps=eps)
   x_norm = norm(x, axis=-1, keepdims=True, eps=eps) / c
@@ -533,15 +534,23 @@
       / lambda_x(y, k, axis=-1, keepdims=True)
   )
 
 
 @partial(jax.jit, static_argnames=("eps",), inline=True)
 def stereo_ptrans0(y: Array, v: Array, k: ArrayLike, eps: float = EPS) -> Array:
   """Compute the parallel transport of v from the origin to y."""
-  return stereo_ptrans(jnp.zeros_like(y), y, v, k, eps=eps)
+  # NOTE: we do not need to depend on addition.  Thus, we can
+  #       implement addition with parallel transport.
+  # return stereo_ptrans(jnp.zeros_like(y), y, v, k, eps=eps)
+  del eps
+  return (
+      v
+      * lambda_x(jnp.zeros_like(y), k, axis=-1, keepdims=True)
+      / lambda_x(y, k, axis=-1, keepdims=True)
+  )
 
 
 # @partial(jax.jit, static_argnames=("eps",), inline=True)
 def _sh_ptrans_v1(
     x: Array, y: Array, v: Array, k: ArrayLike, eps: float = EPS
 ) -> Array:
   """Compute the parallel transport of v from x to y with curvature k."""
```

### Comparing `jaxrie-1/src/jaxrie/manifold/stereographic.py` & `jaxrie-2/src/jaxrie/manifold/stereographic.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 from jax.typing import ArrayLike
 
 # JAX
 import jax
 
 # Local
 from .base import Manifold
-from .math import (EPS, mobius_add, mobius_matmulh, mobius_matmull,
+from .math import (EPS, mobius_add, mobius_adde, mobius_matmulh, mobius_matmull,
                    mobius_matmulr, mobius_matvec_mul, mobius_scala_mul,
                    stereo_egrad2rgrad, stereo_expmap, stereo_expmap0,
-                   stereo_logmap, stereo_logmap0)
+                   stereo_logmap, stereo_logmap0, stereo_proj)
 
 Array = jax.Array
 
 
 class Stereographic(Manifold):
   """The universal Stereographic projection model."""
 
@@ -63,14 +63,20 @@
   @partial(jax.jit, static_argnames=("eps",), inline=True)
   def add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius addition on manifold with curvature k."""
     return mobius_add(x, y, k, eps)
 
   @staticmethod
   @partial(jax.jit, static_argnames=("eps",), inline=True)
+  def adde(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
+    """Mobius addition on manifold (left H, right E) with curvature k."""
+    return mobius_adde(x, y, k, eps)
+
+  @staticmethod
+  @partial(jax.jit, static_argnames=("eps",), inline=True)
   def sub(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Mobius subtraction on manifold with curvature k."""
     return mobius_add(x, -y, k, eps)
 
   @staticmethod
   @partial(jax.jit, static_argnames=("eps",), inline=True)
   def mul(r: Array, x: Array, k: ArrayLike, eps: float = EPS) -> Array:
@@ -126,7 +132,13 @@
     return stereo_logmap0(y, k, axis=-1, eps=eps)
 
   @staticmethod
   @partial(jax.jit, static_argnames=("eps",), inline=True)
   def egrad2rgrad(x: Array, grad: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Euclidean gradient to Riemannian gradient."""
     return stereo_egrad2rgrad(x, grad, k, eps=eps)
+
+  @staticmethod
+  @partial(jax.jit, static_argnames=("eps",), inline=True)
+  def proj(x: Array, k: ArrayLike, eps: float = EPS) -> Array:
+    """Projection on manifold with curvature k."""
+    return stereo_proj(x, k, eps=eps)
```

