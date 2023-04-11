# Comparing `tmp/resampler-0.7.2.tar.gz` & `tmp/resampler-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resampler-0.7.2.tar", last modified: Wed Mar 29 00:54:13 2023, max compression
+gzip compressed data, was "resampler-0.7.3.tar", last modified: Tue Apr 11 06:02:51 2023, max compression
```

## Comparing `resampler-0.7.2.tar` & `resampler-0.7.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-03-29 00:54:05.769573 resampler-0.7.2/LICENSE
--rw-r--r--   0        0        0     6566 2023-03-29 00:54:05.769573 resampler-0.7.2/README.md
--rw-r--r--   0        0        0     2959 2023-03-29 00:54:05.785574 resampler-0.7.2/pyproject.toml
--rw-r--r--   0        0        0   143316 2023-03-29 00:54:05.785574 resampler-0.7.2/resampler/__init__.py
--rw-r--r--   0        0        0    18618 2023-03-29 00:54:05.785574 resampler-0.7.2/resampler/__init__.pyi
--rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 resampler-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-11 06:02:41.761574 resampler-0.7.3/LICENSE
+-rw-r--r--   0        0        0     6566 2023-04-11 06:02:41.761574 resampler-0.7.3/README.md
+-rw-r--r--   0        0        0     2959 2023-04-11 06:02:41.777574 resampler-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0   143499 2023-04-11 06:02:41.777574 resampler-0.7.3/resampler/__init__.py
+-rw-r--r--   0        0        0    18967 2023-04-11 06:02:41.777574 resampler-0.7.3/resampler/__init__.pyi
+-rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 resampler-0.7.3/PKG-INFO
```

### Comparing `resampler-0.7.2/LICENSE` & `resampler-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resampler-0.7.2/README.md` & `resampler-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `resampler-0.7.2/pyproject.toml` & `resampler-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "resampler"
 description = "Fast differentiable resizing and warping of arbitrary grids"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "Hugues Hoppe", email="hhoppe@gmail.com"}]
 classifiers = [
     'Intended Audience :: Developers',
     'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
```

### Comparing `resampler-0.7.2/resampler/__init__.py` & `resampler-0.7.3/resampler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 .. include:: ../README.md
 ."""
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '0.7.2'
+__version__ = '0.7.3'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 from collections.abc import Callable, Iterable, Sequence
 import abc
 import dataclasses
 import functools
 import itertools
 import math
 import typing
-from typing import Any, Generic, Literal, TypeVar, Union
+from typing import Any, Generic, Literal, Union
 
 import numpy as np
 import numpy.typing as npt
 import scipy.interpolate
 import scipy.linalg
 import scipy.ndimage
 import scipy.sparse.linalg
@@ -35,31 +35,33 @@
 
 if typing.TYPE_CHECKING:
   import jax.numpy
   import tensorflow as tf
   import torch
 
   _DType = np.dtype[Any]  # (Requires Python 3.9 or TYPE_CHECKING.)
-  _NDArray = npt.NDArray[Any]
+  _NDArray = np.ndarray[Any, Any]
   _DTypeLike = npt.DTypeLike
   _ArrayLike = npt.ArrayLike
   _TensorflowTensor: typing.TypeAlias = tf.Tensor
   _TorchTensor: typing.TypeAlias = torch.Tensor
   _JaxArray: typing.TypeAlias = jax.numpy.ndarray
 
 else:
-  _DType = Any
-  _NDArray = Any
-  _DTypeLike = Any  # Else `pdoc` uses a long type expression for documentation.
-  _ArrayLike = Any  # Same.
+  # Create named types for use in the `pdoc` documentation.
+  # Actually, these are superseded by the declarations in __init__.pyi!
+  _DType = typing.TypeVar('_DType')  # pylint: disable=invalid-name
+  _NDArray = typing.TypeVar('_NDArray')
+  _DTypeLike = typing.TypeVar('_DTypeLike')
+  _ArrayLike = typing.TypeVar('_ArrayLike')
   _TensorflowTensor = Any
   _TorchTensor = Any
   _JaxArray = Any
 
-_Array = TypeVar('_Array', _NDArray, _TensorflowTensor, _TorchTensor, _JaxArray)
+_Array = typing.TypeVar('_Array', _NDArray, _TensorflowTensor, _TorchTensor, _JaxArray)
 _AnyArray = Union[_NDArray, _TensorflowTensor, _TorchTensor, _JaxArray]
 
 
 def _check_eq(a: Any, b: Any, /) -> None:
   """If the two values or arrays are not equal, raise an exception with a useful message."""
   are_equal = np.all(a == b) if isinstance(a, np.ndarray) else a == b
   if not are_equal:
@@ -2736,15 +2738,15 @@
   if _arr_arraylib(array) == 'numpy':
     return _arr_numpy(
         _original_resize(_make_array(typing.cast(_ArrayLike, array), arraylib), *args, **kwargs)
     )
   return _original_resize(array, *args, **kwargs)
 
 
-@functools.lru_cache()
+@functools.cache
 def _create_jaxjit_resize() -> Callable[..., _Array]:
   """Lazily invoke `jax.jit` on `resize`."""
   import jax
 
   jitted: Callable[..., _Array] = jax.jit(
       _original_resize, static_argnums=(1,), static_argnames=list(_original_resize.__kwdefaults__)
   )
```

### Comparing `resampler-0.7.2/resampler/__init__.pyi` & `resampler-0.7.3/resampler/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,43 @@
+from __future__ import annotations
+
 import abc
 from collections.abc import Callable, Iterable, Sequence
 import dataclasses
-from typing import Any, Union
+import typing
+from typing import Any
 
 import numpy as np
 import numpy.typing as npt
 
-_DType = np.dtype[Any]
-_NDArray = npt.NDArray[Any]
-_DTypeLike = npt.DTypeLike
-_ArrayLike = npt.ArrayLike
-
-# We avoid taking typing dependencies on these large packages as it unnecessarily slows down mypy.
-_TensorflowTensor = Any
-_TorchTensor = Any
-_JaxArray = Any
-
-_Array = Any
-_AnyArray = Any
+if typing.TYPE_CHECKING:
+  _DType = np.dtype[Any]  # (Requires Python 3.9 or TYPE_CHECKING.)
+  _NDArray = np.ndarray[Any, Any]
+  _DTypeLike = npt.DTypeLike
+  _ArrayLike = npt.ArrayLike
+  # We avoid taking typing dependencies on these large packages as it unnecessarily slows down mypy.
+  _TensorflowTensor = Any
+  _TorchTensor = Any
+  _JaxArray = Any
+  #
+  _Array = Any
+  _AnyArray = Any
+else:
+  # Create named types for use in the `pdoc` documentation.
+  _DType = typing.TypeVar('_DType')  # pylint: disable=invalid-name
+  _NDArray = typing.TypeVar('_NDArray')
+  _DTypeLike = typing.TypeVar('_DTypeLike')
+  _ArrayLike = typing.TypeVar('_ArrayLike')
+  #
+  _TensorflowTensor = typing.TypeVar('_TensorflowTensor')
+  _TorchTensor = typing.TypeVar('_TorchTensor')
+  _JaxArray = typing.TypeVar('_JaxArray')
+  #
+  _Array = typing.TypeVar('_Array')
+  _AnyArray = typing.TypeVar('_AnyArray')
 
 __docformat__: str
 __version_info__: tuple[int, ...]
 
 ARRAYLIBS: list[str]
 
 @dataclasses.dataclass(frozen=True)
@@ -156,23 +172,23 @@
   def __call__(self, x: _ArrayLike) -> _NDArray: ...
 
 class BoxFilter(Filter):
   def __init__(self) -> None: ...
   def __call__(self, x: _ArrayLike) -> _NDArray: ...
 
 class TrapezoidFilter(Filter):
-  def __init__(self, *, radius: Union[float, None] = ...) -> None: ...
+  def __init__(self, *, radius: float | None = ...) -> None: ...
   def __call__(self, x: _ArrayLike) -> _NDArray: ...
 
 class TriangleFilter(Filter):
   def __init__(self) -> None: ...
   def __call__(self, x: _ArrayLike) -> _NDArray: ...
 
 class CubicFilter(Filter):
-  def __init__(self, *, b: float, c: float, name: Union[str, None] = ...) -> None: ...
+  def __init__(self, *, b: float, c: float, name: str | None = ...) -> None: ...
   def __call__(self, x: _ArrayLike) -> _NDArray: ...
 
 class CatmullRomFilter(CubicFilter):
   def __init__(self) -> None: ...
   def __call__(self, x: _ArrayLike) -> _NDArray: ...
 
 class MitchellFilter(CubicFilter):
@@ -246,36 +262,36 @@
   def decode(self, array: _Array, dtype: _DTypeLike = ...) -> _Array: ...
   def encode(self, array: _Array, dtype: _DTypeLike) -> _Array: ...
 
 GAMMAS: list[str]
 
 _DEFAULT_FILTER: str = 'lanczos3'
 
-def resize(array: _Array, shape: Iterable[int], *, gridtype: Union[str, Gridtype, None] = None, src_gridtype: Union[str, Gridtype, Iterable[Union[str, Gridtype]], None] = None, dst_gridtype: Union[str, Gridtype, Iterable[Union[str, Gridtype]], None] = None, boundary: Union[str, Boundary, Iterable[Union[str, Boundary]]] = 'auto', cval: _ArrayLike = 0, filter: Union[str, Filter, Iterable[Union[str, Filter]]] = _DEFAULT_FILTER, prefilter: Union[str, Filter, Iterable[Union[str, Filter]], None] = None, gamma: Union[str, Gamma, None] = None, src_gamma: Union[str, Gamma, None] = None, dst_gamma: Union[str, Gamma, None] = None, scale: Union[float, Iterable[float]] = 1.0, translate: Union[float, Iterable[float]] = 0.0, precision: _DTypeLike = None, dtype: _DTypeLike = None, dim_order: Union[Iterable[int], None] = None) -> _Array: ...
+def resize(array: _Array, shape: Iterable[int], *, gridtype: str | Gridtype | None = None, src_gridtype: str | Gridtype | Iterable[str | Gridtype] | None = None, dst_gridtype: str | Gridtype | Iterable[str | Gridtype] | None = None, boundary: str | Boundary | Iterable[str | Boundary] = 'auto', cval: _ArrayLike = 0, filter: str | Filter | Iterable[str | Filter] = _DEFAULT_FILTER, prefilter: str | Filter | Iterable[str | Filter] | None = None, gamma: str | Gamma | None = None, src_gamma: str | Gamma | None = None, dst_gamma: str | Gamma | None = None, scale: float | Iterable[float] = 1.0, translate: float | Iterable[float] = 0.0, precision: _DTypeLike = None, dtype: _DTypeLike = None, dim_order: Iterable[int] | None = None) -> _Array: ...
 # def resize_in_arraylib(array: _NDArray, *args: Any, arraylib: str, **kwargs: Any) -> _NDArray: ...
 def resize_in_arraylib(array: _NDArray, shape: Iterable[int], *args: Any, arraylib: str, **kwargs: Any) -> _NDArray: ...
 
 def resize_in_numpy(array: _NDArray, shape: Iterable[int], *args: Any, **kwargs: Any) -> _NDArray: ...
 def resize_in_tensorflow(array: _NDArray, shape: Iterable[int], *args: Any, **kwargs: Any) -> _NDArray: ...
 def resize_in_torch(array: _NDArray, shape: Iterable[int], *args: Any, **kwargs: Any) -> _NDArray: ...
 def resize_in_jax(array: _NDArray, shape: Iterable[int], *args: Any, **kwargs: Any) -> _NDArray: ...
 
 def jaxjit_resize(array: _Array, *args: Any, **kwargs: Any) -> _Array: ...
-def uniform_resize(array: _Array, shape: Iterable[int], *, gridtype: Union[str, Gridtype, None] = None, src_gridtype: Union[str, Gridtype, Iterable[Union[str, Gridtype]], None] = None, dst_gridtype: Union[str, Gridtype, Iterable[Union[str, Gridtype]], None] = None, boundary: Union[str, Boundary, Iterable[Union[str, Boundary]]] = 'border', scale: Union[float, Iterable[float]] = 1.0, translate: Union[float, Iterable[float]] = 0.0, **kwargs: Any) -> _Array: ...
-def resample(array: _Array, coords: _ArrayLike, *, gridtype: Union[str, Gridtype, Iterable[Union[str, Gridtype]]] = 'dual', boundary: Union[str, Boundary, Iterable[Union[str, Boundary]]] = 'auto', cval: _ArrayLike = 0, filter: Union[str, Filter, Iterable[Union[str, Filter]]] = _DEFAULT_FILTER, prefilter: Union[str, Filter, Iterable[Union[str, Filter]], None] = None, gamma: Union[str, Gamma, None] = None, src_gamma: Union[str, Gamma, None] = None, dst_gamma: Union[str, Gamma, None] = None, jacobian: Union[_ArrayLike, None] = None, precision: _DTypeLike = None, dtype: _DTypeLike = None, max_block_size: int = 40_000, debug: bool = False) -> _Array: ...
-def resample_affine(array: _Array, shape: Iterable[int], matrix: _ArrayLike, *, gridtype: Union[str, Gridtype, None] = 'dual', src_gridtype: Union[str, Gridtype, Iterable[Union[str, Gridtype]], None] = None, dst_gridtype: Union[str, Gridtype, Iterable[Union[str, Gridtype]], None] = None, filter: Union[str, Filter, Iterable[Union[str, Filter]]] = _DEFAULT_FILTER, prefilter: Union[str, Filter, Iterable[Union[str, Filter]], None] = None, precision: _DTypeLike = None, dtype: _DTypeLike = None, **kwargs: Any) -> _Array: ...
-def rotation_about_center_in_2d(src_shape: _ArrayLike, angle: float, *, new_shape: Union[_ArrayLike, None] = None, scale: float = 1.0) -> _NDArray: ...
-def rotate_image_about_center(image: _NDArray, angle: float, *, new_shape: Union[_ArrayLike, None] = None, scale: float = 1.0, num_rotations: int = 1, **kwargs: Any) -> _NDArray: ...
+def uniform_resize(array: _Array, shape: Iterable[int], *, gridtype: str | Gridtype | None = None, src_gridtype: str | Gridtype | Iterable[str | Gridtype] | None = None, dst_gridtype: str | Gridtype | Iterable[str | Gridtype] | None = None, boundary: str | Boundary | Iterable[str | Boundary] = 'border', scale: float | Iterable[float] = 1.0, translate: float | Iterable[float] = 0.0, **kwargs: Any) -> _Array: ...
+def resample(array: _Array, coords: _ArrayLike, *, gridtype: str | Gridtype | Iterable[str | Gridtype] = 'dual', boundary: str | Boundary | Iterable[str | Boundary] = 'auto', cval: _ArrayLike = 0, filter: str | Filter | Iterable[str | Filter] = _DEFAULT_FILTER, prefilter: str | Filter | Iterable[str | Filter] | None = None, gamma: str | Gamma | None = None, src_gamma: str | Gamma | None = None, dst_gamma: str | Gamma | None = None, jacobian: _ArrayLike | None = None, precision: _DTypeLike = None, dtype: _DTypeLike = None, max_block_size: int = 40_000, debug: bool = False) -> _Array: ...
+def resample_affine(array: _Array, shape: Iterable[int], matrix: _ArrayLike, *, gridtype: str | Gridtype | None = 'dual', src_gridtype: str | Gridtype | Iterable[str | Gridtype] | None = None, dst_gridtype: str | Gridtype | Iterable[str | Gridtype] | None = None, filter: str | Filter | Iterable[str | Filter] = _DEFAULT_FILTER, prefilter: str | Filter | Iterable[str | Filter] | None = None, precision: _DTypeLike = None, dtype: _DTypeLike = None, **kwargs: Any) -> _Array: ...
+def rotation_about_center_in_2d(src_shape: _ArrayLike, angle: float, *, new_shape: _ArrayLike | None = None, scale: float = 1.0) -> _NDArray: ...
+def rotate_image_about_center(image: _NDArray, angle: float, *, new_shape: _ArrayLike | None = None, scale: float = 1.0, num_rotations: int = 1, **kwargs: Any) -> _NDArray: ...
 def pil_image_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str) -> _NDArray: ...
 def cv_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str) -> _NDArray: ...
 def scipy_ndimage_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str, boundary: str = 'reflect', cval: float = 0) -> _NDArray: ...
 def skimage_transform_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str, boundary: str = 'reflect', cval: float = 0) -> _NDArray: ...
 def tf_image_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str, antialias: bool = True) -> _TensorflowTensor: ...
 def torch_nn_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str, antialias: bool = False) -> _TorchTensor: ...
-def jax_image_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str, scale: Union[float, Iterable[float]] = 1.0, translate: Union[float, Iterable[float]] = 0.0) -> _JaxArray: ...
+def jax_image_resize(array: _ArrayLike, shape: Iterable[int], *, filter: str, scale: float | Iterable[float] = 1.0, translate: float | Iterable[float] = 0.0) -> _JaxArray: ...
 
 def _check_eq(a: Any, b: Any, /) -> None: ...
 def _real_precision(dtype: _DTypeLike, /) -> _DType: ...
 def _complex_precision(dtype: _DTypeLike, /) -> _DType: ...
 def _get_precision(precision: _DTypeLike, dtypes: list[_DType], weight_dtypes: list[_DType], /) -> _DType: ...
 def _sinc(x: _ArrayLike, /) -> _NDArray: ...
 def _is_symmetric(matrix: _NDArray, /, tol: float = ...) -> bool: ...
```

### Comparing `resampler-0.7.2/PKG-INFO` & `resampler-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: resampler
-Version: 0.7.2
+Version: 0.7.3
 Summary: Fast differentiable resizing and warping of arbitrary grids
 Keywords: 
 Author-email: Hugues Hoppe <hhoppe@gmail.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

