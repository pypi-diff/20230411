# Comparing `tmp/fringes-0.1.4.tar.gz` & `tmp/fringes-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fringes-0.1.4.tar", max compression
+gzip compressed data, was "fringes-0.1.5.tar", max compression
```

## Comparing `fringes-0.1.4.tar` & `fringes-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      100 2023-03-30 08:48:36.306705 fringes-0.1.4/fringes/__init__.py
--rw-r--r--   0        0        0    15097 2023-03-11 22:31:14.190169 fringes-0.1.4/fringes/decoder.py
--rw-r--r--   0        0        0   101206 2023-03-30 08:45:18.171361 fringes-0.1.4/fringes/fringes.py
--rw-r--r--   0        0        0     4240 2023-03-20 11:38:51.156757 fringes-0.1.4/fringes/grid.py
--rw-r--r--   0        0        0    12568 2023-03-14 20:14:39.634222 fringes-0.1.4/fringes/util.py
--rw-r--r--   0        0        0    21278 2023-01-20 12:12:32.656203 fringes-0.1.4/LICENSE
--rw-r--r--   0        0        0      816 2023-03-30 08:48:36.313688 fringes-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    25943 2023-03-29 17:12:31.313598 fringes-0.1.4/README.md
--rw-r--r--   0        0        0    26939 1970-01-01 00:00:00.000000 fringes-0.1.4/setup.py
--rw-r--r--   0        0        0    26357 1970-01-01 00:00:00.000000 fringes-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-04-02 10:36:06.093945 fringes-0.1.5/fringes/__init__.py
+-rw-r--r--   0        0        0    15118 2023-04-11 17:47:00.201815 fringes-0.1.5/fringes/decoder.py
+-rw-r--r--   0        0        0   103433 2023-04-11 17:50:18.840652 fringes-0.1.5/fringes/fringes.py
+-rw-r--r--   0        0        0     4240 2023-03-20 11:38:51.156757 fringes-0.1.5/fringes/grid.py
+-rw-r--r--   0        0        0    12901 2023-04-02 11:05:36.206594 fringes-0.1.5/fringes/util.py
+-rw-r--r--   0        0        0    21278 2023-01-20 12:12:32.656203 fringes-0.1.5/LICENSE
+-rw-r--r--   0        0        0      816 2023-03-31 19:52:30.401871 fringes-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    26112 2023-04-11 17:47:00.199821 fringes-0.1.5/README.md
+-rw-r--r--   0        0        0    27109 1970-01-01 00:00:00.000000 fringes-0.1.5/setup.py
+-rw-r--r--   0        0        0    26522 1970-01-01 00:00:00.000000 fringes-0.1.5/PKG-INFO
```

### Comparing `fringes-0.1.4/fringes/decoder.py` & `fringes-0.1.5/fringes/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     if d > c / 2:
         d -= c
     elif d < - c / 2:
         d += c
     return d
 
 
-@nb.jit(cache=True, nopython=True, nogil=True, parallel=True, fastmath=True)
+# @nb.jit(cache=True, nopython=True, nogil=True, parallel=True, fastmath=True)
+@nb.jit(cache=True, fastmath=True)
 def decode(
     I: np.ndarray,
     N: np.ndarray,
     v: np.ndarray,
     f: np.ndarray,
     R: np.ndarray,  # range
     o: float = np.pi,
@@ -109,15 +110,15 @@
     # dt = np.float64 if I.itemsize == 8 else np.float32  # todo: numba crashes
     dt = np.float32  # float32's precision is usually better than quantization noise in phase shifting sequence
     bri = np.empty((D, Y, X, C), dt)  # brightness must be identical for all sets, therefore we arverage over them
     mod = np.empty((D, K, Y, X, C), dt)
     phi = np.empty((D, K, Y, X, C), dt)
     reg = np.empty((D, Y, X, C), dt)
     res = np.empty((D, Y, X, C), dt)
-    fid = np.empty((D, K, Y, X, C), np.int_)
+    fid = np.empty((D, K, Y, X, C), dt)
 
     for x in nb.prange(X):  # usually X > Y -> put X first, because parallelization only affects outer for-loop
         for y in nb.prange(Y):
             for c in nb.prange(C):
                 for d in nb.prange(D):
 
                     # temporal demodulation
@@ -167,26 +168,26 @@
                                 if verbose:
                                     res[d, y, x, c] = 0
                                     fid[d, 0, y, x, c] = 0
                             else:  # elif R[d] > 1:
                                 reg[d, y, x, c] = np.nan  # no spatial modulation, therefore we can't compute value
                                 if verbose:
                                     res[d, y, x, c] = np.nan
-                                    fid[d, 0, y, x, c] = -1  # np.nan
+                                    fid[d, 0, y, x, c] = np.nan
                         elif v[d, 0] <= 1:  # one period covers whole screen: no unwrapping required
                             pn = (p[0] + o) / PI2 % 1  # revert offset and change codomain from [-PI, PI] to [0, 1) -> normalized phi
                             reg[d, y, x, c] = pn * l[d, 0]
                             if verbose:
                                 res[d, y, x, c] = 0  # todo: uncertainty
                                 fid[d, 0, y, x, c] = 0
                         else:  # v[d, 0] > 1: # spatial phase unwrapping (to be done in a later step)
                             reg[d, y, x, c] = p[0]
                             if verbose:
-                                # residuals are to be received from SPU (spatial phase unwrapping)
-                                fid[d, 0, y, x, c] = -1  # np.nan  # unknown
+                                # todo: residuals are to be received from SPU (spatial phase unwrapping)
+                                fid[d, 0, y, x, c] = np.nan  # unknown
                     else:  # K > 1: temporal phase unwrapping
                         if False:    # todo
                             # cw = np.empty(K)  # fringe visibility (fringe contrast) squared for multiplying into weights
                             #                         # for k in nb.prange(K):  # softmax?
                             #                         #     if B[k] > 2 * A[k]:
                             #                         #         cm[k] = 0
                             #                         #     elif B[k] > A[k]:
@@ -252,14 +253,14 @@
                                         if mn <= ssdlim:
                                             break
 
                             if mn >= ssdmax[d]:
                                 reg[d, y, x, c] = np.nan  # np.nan  # no suitable fringe orders found
                                 if verbose:
                                     res[d, y, x, c] = np.inf  # no suitable fringe orders found
-                                    fid[d, :, y, x, c] = -1  # np.nan  # no suitable fringe orders found
+                                    fid[d, :, y, x, c] = np.nan  # no suitable fringe orders found
                             else:
                                 reg[d, y, x, c] = avg
                                 if verbose:
                                     res[d, y, x, c] = np.sqrt(mn / K)  # ssd (sum of squared distances) -> std
 
     return phi.reshape(-1, Y, X, C), bri, mod.reshape(-1, Y, X, C), reg, res, fid.reshape(-1, Y, X, C)
```

### Comparing `fringes-0.1.4/fringes/fringes.py` & `fringes-0.1.5/fringes/fringes.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 class Fringes:
     """Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns."""
 
     # value limits
     _Hmax = 101  # this is arbitrary
     _Dmax = 2  # max 2 dimensions
     _Kmax = 101  # this is arbitrary, but must be < 128 when deploying spatial or frequency multiplexing @ uint8
-    _Nmax = 1001  # this is arbitrary; more is better but the improvement scales with sqrt(M)
-    _Mmax = 101  # this is arbitrary; more is better but the improvement scales with sqrt(N)
+    _Nmax = 1001  # this is arbitrary; more is better but the improvement scales with sqrt(N); @FDM: > 2 * Dmax * Kmax + 1
+    _Mmax = 101  # this is arbitrary; more is better but the improvement scales with sqrt(M)
     # _Pmax: int = 35651584  # ~8K i.e. max luma picture size of h264, h265, h266 video codecs as of 2022; todo: update
     _Pmax = 2 ** 30  # 2^30 = 1,073,741,824 i.e. default size   limit of imread() in OpenCV
     _Xmax = 2 ** 20  # 2^20 = 1,048,576     i.e. default width  limit of imread() in OpenCV
     _Ymax = 2 ** 20  # 2^20 = 1,048,576     i.e. default height limit of imread() in OpenCV
     _Lmax = 2 ** 20  # 2^20 = 1,048,576     i.e. default height limit of imread() in OpenCV
     _Tmax = _Hmax * _Dmax * _Kmax * _Nmax
-    _deltamax = 2
+    _alphamax = 2
     _gammamax = 3  # most screens have a gamma of ~2.2
 
     # allowed values; take care to only use immutable types!
     _grids = ("image", "Cartesian", "polar", "log-polar")
     _modes = ("fast", "precise", "robust")
     _hues = (
         np.array([[255, 255, 255]]),  # white
@@ -55,82 +55,88 @@
         "uint16",
         # 'uint32',  # integer overflow in pyqtgraph -> replace line 528 of ImageItem.py with:
         # 'uint64',  # bins = self._xp.arange(mn, mx + 1.01 * step, step, dtype="uint64")
         # "float16",  # numba doesn't handle float16, also most algorithms convert float16 to float32 anyway
         "float32",
         "float64",
     )
+    _loader = {
+        ".json": json.load,
+        # todo: ".toml": toml.load,
+        ".yaml": yaml.safe_load,
+        ".asdf": asdf.open,
+    }
 
     # default values are defined here; take care to only use immutable types!
     def __init__(self,
                  Y: int = 1200,
                  X: int = 1920,
                  H: int = 1,  # H is inferred from h
-                 M: float = 1,  # M is inferred from h
+                 M: float = 1.,  # M is inferred from h
                  D: int = 2,
                  K: int = 3,
                  T: int = 24,
                  N: tuple | np.ndarray = np.array([[4, 4, 4], [4, 4, 4]], int),
                  l: tuple | np.ndarray = 1920 / np.array([[13, 7, 89], [13, 7, 89]], float),
                  v: tuple | np.ndarray = np.array([[13, 7, 89], [13, 7, 89]], float),
                  f: tuple | np.ndarray = np.array([[1, 1, 1], [1, 1, 1]], float),
                  h: tuple | np.ndarray = _hues[0],  # np.array([[255, 255, 255]], int)
                  o: float = np.pi,
-                 gamma: float = 1,
+                 gamma: float = 1.,
                  A: float = 255 / 2,  # Imax / 2 @ uint8
                  B: float = 255 / 2,  # Imax / 2 @ uint8
-                 V: float = 1,
-                 delta: float = 1,
+                 V: float = 1.,
+                 alpha: float = 1.,
                  dtype: str | np.dtype = "uint8",
                  grid: str = "image",
-                 angle: float = 0,
+                 angle: float = 0.,
                  axis: int = 0,
                  TDM: bool = True,
                  SDM: bool = False,
                  WDM: bool = False,
                  FDM: bool = False,
                  static: bool = False,
-                 lmin: float = 4,
+                 lmin: float = 8.,
                  reverse: bool = False,
                  verbose: bool = False,
                  mode: str = "fast",
-                 Vmin: float = 0,
-                 DN: float = 0,  # todo: 3?  # Manta G-419
-                 PN: float = 0,  # K = (2 ** 12 - 1) / 9600 * 255 / 2  # Manta G-419
+                 Vmin: float = 0.,
+                 esat: float = np.inf,
+                 dark: float = 0.,
                  ) -> None:
 
         given = {k: v for k, v in sorted(locals().items()) if k in self.defaults and not np.array_equal(v, self.defaults[k])}
 
         self.logger = lg.getLogger(self.__class__.__name__)  # todo: give each logger instance its own instance name
         self.logger.setLevel("CRITICAL")
         if not self.logger.hasHandlers():
             formatter = lg.Formatter("%(asctime)s %(levelname)-8s %(name)7s.%(funcName)-11s: %(message)s")
             handler = lg.StreamHandler()
             handler.setFormatter(formatter)
             self.logger.addHandler(handler)
 
+        a = self.logger.handlers
+
         # set values each using initial if initial else config if config else default values
         for k, v in self.defaults.items():
             setattr(self, f"_{k}", v)  # initially define private variables
 
         fname = os.path.join(os.path.dirname(__file__), "params.yaml")
         if os.path.isfile(fname):  # load params from config file if existent
             self.load(fname)
-
-        for k, v in given.items():
-            if k in self.defaults:
-                setattr(self, k, v)
-        for k, v in given.items():
-            if not np.array_equal(v, getattr(self, k)):  # getattr(self, "_" + k)
-                self.logger.warning(f"'{k}' got overwritten by interdependencies. Choose consistent init values.")
+        else:
+            for k, v in given.items():
+                if k in self.defaults:
+                    setattr(self, k, v)
+            for k, v in given.items():
+                if not np.array_equal(v, getattr(self, k)):  # getattr(self, "_" + k)
+                    self.logger.warning(f"'{k}' got overwritten by interdependencies. Choose consistent init values.")
 
         self._UMR = None
-        if np.any(self.UMR < self.R):
-            self.logger.warning(
-                "UMR < R. Unwrapping will not be spatially independent and only yield a relative phase map.")
+        UMR = self.UMR  # property 'UMR' logs warning if necessary
 
     defaults = dict(sorted(dict(zip(__init__.__annotations__, __init__.__defaults__)).items()))
 
     # restrict class attributes to the ones listed here (add "__dict__" or commend the next line out to circumvent this)
     __slots__ = tuple("_" + k for k in __init__.__annotations__.keys()) + ("logger", "_UMR", "t",)
 
     def __call__(self, *args, **kwargs) -> np.ndarray:
@@ -174,56 +180,50 @@
 
         if not fname:
             return {}
         elif not os.path.isfile(fname):
             self.logger.error(f"File '{fname}' does not exist.")
             return {}
 
-        loader = {
-            ".json": json.load,
-            # ".toml": toml.load,
-            ".yaml": yaml.safe_load,
-            ".asdf": asdf.open,
-        }
-
         ext = os.path.splitext(fname)[-1]
         if ext == ".asdf":
             with asdf.open(fname) as f:
                 p = f.copy()
         else:
             with open(fname, "r") as f:
                 if ext == ".json":
                     p = json.load(f)
                 elif ext == ".yaml":
                     p = yaml.safe_load(f)
+                # todo:
                 # elif ext == ".toml":
                 #     p = toml.load(f)
                 else:
                     self.logger.error(f"Unknown file type '{ext}'.")
                     return {}
 
         if "fringes" in p:
-            self.logger.debug(f"{fname}.")  # todo: does order in which params are loaded affect final param state?
-
             params = p["fringes"]
-            for k in self.params.keys():
+            for k in self.params.keys():  # todo: does order in which params are loaded affect final param state?
                 if k in params and k != "T":
                     setattr(self, k, params[k])
             for k in self.params.keys():
                 if not np.array_equal(params[k], getattr(self, k)):
                     self.logger.warning(f"'{k}' got overwritten by interdependencies. Choose consistent config values.")
 
+            self.logger.info(f"Loaded parameters from {fname}.")
+
             return params
         else:
             return {}
 
     def save(self, fname: str = "") -> None:
         """Save parameters to file."""
 
-        if not os.path.isdir(os.path.dirname(fname)) or os.path.splitext(fname)[-1] not in (".json", ".yaml", ".asdf"):  # ".toml"
+        if not os.path.isdir(os.path.dirname(fname)) or os.path.splitext(fname)[-1] not in self._loader.keys():
             fname = os.path.join(os.path.dirname(__file__), "params.yaml")
 
         ext = os.path.splitext(fname)[-1]
         if ext == ".asdf":
             asdf.AsdfFile({"fringes": self.params}).write_to(fname)
         else:
             with open(fname, "w") as f:
@@ -231,34 +231,37 @@
                     json.dump({"fringes": self.params}, f)
                 elif ext == ".yaml":
                     yaml.dump({"fringes": self.params}, f)
                 # elif ext == ".toml":
                 #     toml.dump({"fringes": self.params}, f)
                 # todo: ".ini"
 
-        self.logger.debug(f"{fname}.")
+        self.logger.info(f"Saved parameters to {fname}.")
 
     def reset(self) -> None:
         """Reset parameters to defaults."""
         # self.__init__()  # attention: config file might be reloaded
 
         for k, v in self.defaults.items():
-            setattr(self, k, v)  # initially define private variables
+            if k in self.params:
+                if k != "T":
+                    setattr(self, k, v)  # attention: private variables have to be defined within __init__()
 
         self.logger.info("Set parameters back to defaults.")
 
     def auto(self, T: int = 24) -> None:
         """Automatically set the optimal parameters based on:
          T: Given number of frames.
          lmin: Minimum resolvable wavelength.
          L: Length of fringe patterns."""
         self.h = "w"  # todo: try h = "rgb"
-        self.D = 2
+        # self.D = 2  # todo
         self.T = (T, 4)
         self.v = "auto"
+        self.logger.info("Auto set parameters.")
 
     # def gamma_auto_correct(self, I: np.ndarray) -> np.ndarray:
     #     """Automatically compensate gamma by histogram analysis."""
     #     J = I  # todo: autodegamma -> assume evenly distributed histogram
     #     return J
 
     def setMTF(self, B: np.ndarray, show: bool = True) -> np.ndarray:  # todo: check return type
@@ -287,31 +290,43 @@
                 mtf = interp(v)
                 idx = np.argmin(mtf >= 0.5) - 1  # index of last element where MTF >= 0.5
                 vmax[d, c] = v[idx]
 
         # self.vmax = vmax  # todo: per hue?
         self.lmin = self.L / vmax
 
-        print(MTF)
+        self.logger.info(f"MTF is: {MTF}")
         return MTF  # todo: return interpolated mtf?
 
     def deinterlace(self, I: np.ndarray) -> np.ndarray:
         """Deinterlace fringe patterns acquired with a line scan camera
         while each frame has been displayed and captured
         while the object has been moved by one pixel."""
+
+        t0 = time.perf_counter()
+
         T, Y, X, C = vshape(I).shape
         assert T * Y % self.T == 0, "Number of frames of parameters and data don't match."
         # I = I.reshape((T * Y, X, C))  # concatenate
+
+        self.logger.info(f"{si(time.perf_counter() - t0)}s")
+
         return I.reshape((-1, self.T, X, C)).swapaxes(0, 1)
 
     def coordinates(self) -> np.ndarray:
         """uv-coordinates of grid to encode."""
+
+        t0 = time.perf_counter()
+
         centered = False if self.grid == "image" else True
         sys = "img" if self.grid == "image" else "cart" if self.grid == "Cartesian" else "pol" if self.grid == "polar" else "logpol"
-        uv = np.array(getattr(grid, sys)(self.Y, self.X, self.angle, centered))  # * self.L  # todo: numba
+        uv = np.array(getattr(grid, sys)(self.Y, self.X, self.angle, centered))[self.axis if self.D == 1 else ...]  # * self.L  # todo: numba
+
+        self.logger.info(f"{si(time.perf_counter() - t0)}s")
+
         return uv.reshape((self.D, self.Y, self.X, 1))
 
     def _modulate(self, frame: tuple = None, rint: bool = True) -> np.ndarray:  # todo: rint = False as default? influence on residuals?
         """Encode base fringe patterns by spatio-temporal modulation."""
 
         # dd = [d for d in range(self.D) for k in range(self.K) for n in range(self._N[d, k])]
         # kk = [k for d in range(self.D) for k in range(self.K) for n in range(self._N[d, k])]
@@ -340,37 +355,48 @@
         except:
             T = 1
             frame = [frame]
         frames = np.array(frame)
 
         if self.grid != "image" or self.angle != 0:
             uv = self.coordinates()[..., 0]
+            assert uv.ndim == 3, "uv-coordinates are not three-dimensional with shape (D, Y, X)"
         else:
             uv = None
 
         # is_pure = all(c == 0 or c == 255 for h in self.h for c in h)
         # dtype = np.dtype("float64") if self.SDM or self.FDM or not is_pure else self.dtype
         dtype = np.dtype("float64") if self.SDM or self.FDM else self.dtype
 
         I = np.empty([T, self.Y, self.X], dtype)
         i = 0
         f = 0
         for d in range(self.D):
             if uv is None and self.grid == "image":
                 x = np.arange(self.R[d]) / self.L  # gets broadcasted
+                if self.D == 2:
+                    if d == 0:
+                        x = x[None, :]
+                    else:
+                        x = x[:, None]
+                else:
+                    if self.axis == 0:
+                        x = x[None, :]
+                    else:
+                        x = x[:, None]
             else:
                 x = uv[d]
 
             for k in range(self.K):
                 q = 2 * np.pi * self._v[d, k]
                 w = 2 * np.pi * self._f[d, k] * (-1 if self.reverse else 1)
                 for n in range(self._N[d, k]):
                     if f in frames:
                         t = n / 4 if self._N[d, k] == 2 else n / self._N[d, k]  # t = o if N[d, k] == 1
-                        cos = np.cos(q * (x if x.ndim == 2 else x[None, :] if d == 0 else x[:, None]) - w * t - self.o)
+                        cos = np.cos(q * x - w * t - self.o)
 
                         if self.gamma == 1:
                             val = self.A + self.B * cos
                         else:
                             val = self.A + self.B * (.5 + .5 * cos) ** self.gamma
 
                         if dtype.kind in "ui" and rint:
@@ -543,15 +569,15 @@
             Vmin = self.Vmin
             if self.SDM:
                 Vmin /= self.D
             elif self.FDM:
                 Vmin /= self.D * self.K
 
             if self.mode == "fast":
-                SQNR = self.B / self.QN
+                SQNR = self.B / self.quant
                 Vmin = max(Vmin, 1 / SQNR)
                 r = min(self.u, 1)  # todo: 0.5 or self.u
             else:
                 r = 0
             r = 0  # todo
 
             # """Weights for inverse variance weighting."""
@@ -771,28 +797,31 @@
             elif np.array_equal(idx, [2, 0, 1]):  # BRG
                 I = I[..., 2:2:-1, :]
 
             if C == 1:
                 I = I[..., 0]
             elif C == 3:
                 I = np.diagonal(I, axis1=-2, axis2=-1)  # returns a view
-        elif self.H == 2 and C == 3 and is_single_and_value and is_equal_or_zero:  # C == 3 avoids CMY colors appearing twice as bright as RGB colors (as it is with mono cameras) assuming spectral bands don't overlap todo
+        elif self.H == 2 and C == 3 and is_single_and_value and is_equal_or_zero:  # todo: C == 3 avoids CMY colors appearing twice as bright as RGB colors (as it is with mono cameras) assuming spectral bands don't overlap
             I = np.moveaxis(I, 0, -2)  # returns a view
             idx = self.h != 0
             I = I[..., idx]  # advanced indexing doesn't return a view
         else:  # fuse colors by weighted averaging
             w = self.h / np.sum(self.h, axis=0)  # normalized weights
-            w[np.isnan(w)] = 0
+            # w[np.isnan(w)] = 0
 
             if np.all((w == 0) | (w == 1)):
                 w = w.astype(bool, copy=False)  # multiplying with bool preserves dtype
                 dtype = I.dtype  # without this, np.sum chooses a dtype which can hold the theoretical maximal sum
             else:
                 dtype = float  # without this, np.sum chooses a dtype which can hold the theoretical maximal sum
 
+
+            # I = I.astype(float, copy=False)
+            # I[w[:, None, None, None, :] == 0] = np.nan
             I = np.sum(I * w[:, None, None, None, :], axis=0, dtype=dtype)
 
         self.logger.debug(f"{si(time.perf_counter() - t0)}s")
 
         return I
 
     def encode(self, frame: int | tuple | list = None, rint: bool = True) -> np.ndarray:
@@ -835,32 +864,36 @@
         if self.SDM or self.WDM or self.FDM:
             I = self._multiplex(I, rint)
 
         # colorize (extended averaging)
         if self.H > 1 or np.any(self.h != 255):  # can be used for extended averaging
             I = self._colorize(I, frames)
 
-        self.logger.debug(f"{si(time.perf_counter() - t0)}s")
+        self.logger.info(f"{si(time.perf_counter() - t0)}s")
 
         return I
 
     def decode(self, I: np.ndarray, verbose: bool = False, denoise: bool = False, despike: bool = False) -> namedtuple:
         """Decode fringe patterns."""
 
         t0 = time.perf_counter()
 
         # get and apply videoshape
         T, Y, X, C = vshape(I).shape  # extract Y, X, C from data as these parameters depend on used camera
         I = I.reshape((T, Y, X, C))
 
         # assertions
+        if T != self.T:
+            self.logger.error("Number of frames of parameters and data don't match.")
+            return
+
         if np.any(self.UMR < self.R):
             self.logger.warning(
                 "UMR < R. Unwrapping will not be spatially independent and only yield a relative phase map.")
-        assert T == self.T, "Number of frames of parameters and data don't match."
+
         if self.FDM:
             assert len(np.unique(self.N)) == 1, "Shifts aren't equal."
 
         # decolorize i.e. fuse hues/colors
         if self.H > 1 or not self._ismono:  # for gray fringes, color fusion is not performed, but extended averaging is
             I = self._decolorize(I)
 
@@ -921,15 +954,15 @@
         # create named tuple to return
         if self.verbose or verbose:
             dec = namedtuple("decoding", "brightness modulation phase registration residuals orders")(bri, mod, phi,
                                                                                                       reg, res, fid)
         else:
             dec = namedtuple("decoding", "brightness modulation registration")(bri, mod, reg)
 
-        self.logger.debug(f"{si(time.perf_counter() - t0)}s")
+        self.logger.info(f"{si(time.perf_counter() - t0)}s")
 
         return dec
 
     def _unwrap(self, phi: np.ndarray, B: np.ndarray = None, func: str = "ski") -> namedtuple:  # todo: use B for quality guidance
         """Unwrap phase maps spacially."""
 
         t0 = time.perf_counter()
@@ -1054,15 +1087,15 @@
 
         if T == 1:
             if self.axis == 0:
                 x = np.vstack((x, np.zeros_like(x)))
             else:  # self.axis == 1
                 x = np.vstack((np.zeros_like(x), x))
 
-        src = np.zeros((int(np.round(self.Y * scale)), int(np.round(self.X * scale)), C))
+        src = np.zeros((int(np.round(self.Y * scale)), int(np.round(self.X * scale)), C), np.float32)
         idx = np.rint(x.swapaxes(1, 2) * scale).astype(int, copy=False)
         if B is not None:
             val = np.mean(B.swapaxes(1, 2), axis=0)
             if Bmin > 0:
                 val *= val >= Bmin
         else:
             val = np.ones((Y, X, C), np.uint8)
@@ -1070,22 +1103,24 @@
             src[idx[1].ravel(), idx[0].ravel(), c] += val[..., c].ravel()
 
         if normalize:
             mx = src.max()
             if mx > 0:
                 src /= mx
 
-        self.logger.debug(f"{si(time.perf_counter() - t0)}s")
+        self.logger.info(f"{si(time.perf_counter() - t0)}s")
 
         return src
 
     def _error(self):  # todo: remove
         """Error."""
         # """Mean absolute distance between decoded and true coordinates, considering only quantization noise."""
 
+        t0 = time.perf_counter()
+
         # f = Fringes(**{k: v for k, v in self.params.items() if k in Fringes.defaults})
         I = self.encode()
         dec = self.decode(I)
 
         centered = False if self.grid == "image" else True
         sys = "img" if self.grid == "image" else "cart" if self.grid == "Cartesian" else "pol" if self.grid == "polar" else "logpol"
         uv = np.array(getattr(grid, sys)(self.Y, self.X, self.angle, centered))[:, :, :, None] * self.L
@@ -1116,14 +1151,15 @@
             )(DR, DRP, B, xavg, xmed, xmax, xstd, reserve, SNR, SPNR, ravg, rmed, rmax, )
         else:
             errors = namedtuple(
                 "errors",
                 "dynrange dynrangepeak bits meanabsdist medabsdist maxabsdist stdabsdist reserve SNR SPNR"
             )(DR, DRP, B, xavg, xmed, xmax, xstd, reserve, SNR, SPNR, )
 
+        self.logger.debug(f"{si(time.perf_counter() - t0)}s")
         return errors
 
     @property
     def grid(self) -> str:
         """Coordinate system of fringe patterns."""
         return self._grid
 
@@ -1196,15 +1232,23 @@
 
     @property
     def axis(self) -> int:
         """Axis along which to shift if number of directions equals one."""
         return self._axis
 
     @axis.setter
-    def axis(self, axis: int):
+    def axis(self, axis: int | str):
+        if isinstance(axis, str):
+            if axis.lower() in ["x", "u"]:
+                axis = 0
+            elif axis.lower() in ["y", "v"]:
+                axis = 1
+            else:
+                return
+
         _axis = int(min(max(0, axis), 1))
 
         if self._axis != _axis:
             self._axis = _axis
             self.logger.debug(f"{self._axis = }")
             self.l = self.L / self.v  # l triggers v
 
@@ -1244,45 +1288,50 @@
             #     d = int(c)
             #     T = int(np.ceil(np.max(np.sum(self._N, axis=1)) / 2))
 
         return int(T)  # use int() to ensure type is "int" instead of "numpy.core.multiarray.scalar"  # todo: necessary?
 
     @T.setter
     def T(self, T: int):
+        # attention: params may change even if Tnew == Told
+
         # todo: the setter can only take one argument, so we check for an iterable to get two arguments: T and Nmin
         # try:
         #     T, Nmin = T
         #     Nmin = int(min(max(3, Nmin), self._Nmax))
         # except:
         #     Nmin = 3
 
         Nmin = 3
 
         _T = int(min(max(1, T), self._Tmax))
 
         if _T == 1:  # WDM + SDM todo: SSB?
-            self.H = 1
             if self.grid not in self._grids[:2]:
                 self.logger.error(f"Couldn't set 'T = 1': grid not in {self._grids[:2]}'.")
                 return
-            self.FDM = False
-            self.N = 3
-            self.WDM = True
+
+            self.H = 1
             self.K = 1
+
+            self.FDM = False  # reset FDM before setting N
+            self.N = 3  # set N before WDM
+            self.WDM = True
+
             if self.D == 2:
                 self.SDM = True
         elif _T == 2:  # WDM
             self.H = 1
-            if self.grid not in self._grids[:2]:
-                self.logger.error(f"Couldn't set 'T = 1': grid not in {self._grids[:2]}'.")
-                return
-            self.FDM = False
-            self.N = 3
+            self.D = 2
+            self.K = 1
+
+            self.FDM = False  # reset FDM before setting N
+            self.N = 3  # set N before WDM
             self.WDM = True
-            self.K = _T // self.D
+
             self.SDM = False
         else:
             # as long as enough shifts are there to compensate for nonlinearities,
             # it doesn't matter if we use more shifts or more sets
             if _T < Nmin:
                 Nmin = _T
             Nmin = max(3, Nmin)  # minimum number of phase shifts for first set to de demodulated/decoded
@@ -1290,17 +1339,19 @@
             # todo: N12 = 1 in self.N or 2 in self.N
             Ngood = 4  # minimum number of phase shifts to obtain good results i.e. reliable results in practice
             self.SDM = False
             self.WDM = False
             # todo: T == 4 -> no mod
             #  T == 5 -> FDM if _T >= Nmin?
 
-            # try to keep directions  # todo: mux
-            if _T < self.D * Nmin:
+            # try D == 2  # todo: mux
+            if _T < 2 * Nmin:
                 self.D = 1
+            else:
+                self.D = 2
 
             # try to keep hues  # todo: mux
             if _T < self.H * self.D * Nmin:
                 self.H = _T // (self.D * Nmin)
 
             while _T % self.H != 0:
                 self.H -= 1
@@ -1411,28 +1462,29 @@
 
     @property
     def P(self) -> int:
         """Number of pixels per color channel and frame."""
         return self.Y * self.X
 
     @property
-    def delta(self) -> float:
+    def alpha(self) -> float:
         """Additional relative buffer coding range."""
-        return self._delta
+        return self._alpha
 
-    @delta.setter
-    def delta(self, delta: float):
-        # _delta = float(min(max(1, delta), self.deltamax))
-        _delta = float(max(1, delta))
+    @alpha.setter
+    def alpha(self, alpha: float):
+        # _alpha = float(min(max(1, alpha), self.alphamax))
+        _alpha = float(max(1, alpha))
 
-        if self._delta != _delta:
-            self._delta = _delta
+        if self._alpha != _alpha:
+            self._alpha = _alpha
+            self.l = self.L / self._v
 
     @property
-    def R(self) -> np.ndarray[int]:
+    def R(self) -> np.ndarray:
         """Range of fringe patterns for each direction [px]."""
         if self.D == 2:
             R = np.array([self.X, self.Y])
         else:
             if self.axis == 0:
                 R = np.array([self.X])
             else:
@@ -1454,47 +1506,47 @@
         # # todo: polar, log-polar coordinates
         return R
 
     @property
     def L(self) -> int | float:
         """Length of fringe patterns [px]."""
 
-        if self.grid in ["image", "Cartesian"]:
+        if True:#self.grid in ["image", "Cartesian"]:
             if self.angle % 90 == 0:
                 if self.D == 2:
                     L = max(self.X, self.Y)
                 else:
                     if self.axis == 0:
                         L = self.X
                     else:  # self.axis == 1
                         L = self.Y
             else:
-                a = np.deg2rad(self.a)
+                a = np.deg2rad(self.angle)
                 if self.D == 2:
                     L = self.X * np.cos(a) + self.Y * np.sin(a)
                     # Lx = self.X + self.Y * tan
                     # Ly = self.Y + self.X * tan
                     # L = max(Lx, Ly)
                 else:
                     if self.axis == 0:
                         L = self.X + self.Y * np.tan(a)
                     else:
                         L = self.Y + self.X * np.tan(a)
         elif self.grid == "polar":
             if self.angle % 90 == 0:
-                L = np.sqrt(self.X ** 2 + self.Y ** 2)
+                L = np.sqrt(self.X ** 2 + self.Y ** 2)  # todo
             else:
-                pass  # todo: L for pol & ang
-        elif self.grid == "logpol":
+                L = self.X ** 2 + self.Y ** 2  # todo
+        elif self.grid == "log-polar":
             if self.angle % 90 == 0:
-                L = np.log(np.sqrt(self.X ** 2 + self.Y ** 2))
+                L = np.log(np.sqrt(self.X ** 2 + self.Y ** 2))  # todo
             else:
-                pass  # todo: L for logpol & ang
+                L = self.X ** 2 + self.Y ** 2  # todo
 
-        return L * self.delta
+        return L * self.alpha
 
     @property
     def UMR(self) -> np.ndarray:
         """Unambiguous measurement range."""
         # If neither wavelength nor periods are integers, lcm resp. gcd are extended to rational numbers.
 
         if self._UMR is not None:  # cache
@@ -1580,15 +1632,15 @@
         """Number of averaged intensity samples."""
         M = np.sum(self.h, axis=0) / 255
         if len(set(M)) == 1:
             M = M[0]
         else:
             # todo: M = M[None, None, :]
             pass
-        return np.amax(M)  # todo: fix
+        return float(M.max())  # convert Numpy float64 to Python float  # todo: fix M.max()
 
     @M.setter
     def M(self, M: float):
         _M = min(max(1 / 255, M), self._Mmax)
 
         if np.any(self.M != _M):
             h = np.array([[255, 255, 255]] * int(_M), np.uint8)
@@ -1670,15 +1722,15 @@
             _h = _h[:self._Hmax, :3, ..., -1]
 
         if _h.shape[1] == 2:  # C-axis must equal 3
             self.logger.error("Couldn't set 'h': Only 2 instead of 3 color channels provided.")
             return
 
         if np.any(np.max(_h, axis=1) == 0):
-            self.logger.error("Couldn't set 'h': Black color is not allowed.")
+            self.logger.error("Didn't set 'h': Black color is not allowed.")
             return
 
         if self.WDM and not self._ismono:
             self.logger.error("Couldn't set 'h': 'WDM' is active, but not all hues are monochromatic.")
             return
 
         if _h.size and not np.array_equal(self._h, _h):
@@ -1777,15 +1829,18 @@
 
         if self._FDM != _FDM:
             self._FDM = _FDM
             self.logger.debug(f"{self._FDM = }")
             # self.K = self._K
             self.N = self._N
             self.l = self._l  # l triggers v
-            self.f = self._f
+            if self.FDM:
+                self.f = self._f
+            else:
+                self.f = "auto"
 
             if self.FDM:
                 self.B /= (self.D * self.K)
             else:
                 self.B *= (self.D * self.K)
 
     @property
@@ -1839,15 +1894,17 @@
             self.f = np.append(self._f, np.tile(self.defaults["f"][0, 0], (self.D, _K - self._f.shape[1])), axis=1)
 
             self.B = self.B
 
     @property
     def eta(self) -> float:
         """Coding efficiency."""
-        return self.L / self.UMR  # todo: self.R / self.UMR
+        eta = self.R / self.UMR
+        eta[self.UMR < self.R] = 0
+        return eta
 
     @property
     def N(self) -> np.ndarray:
         """Number of phase shifts."""
         if self.D == 1 or len(np.unique(self._N, axis=0)) == 1:  # sets in directions are identical
             N = self._N[0]  # 1D
         else:
@@ -1995,16 +2052,16 @@
                 #
                 #         # # alternating smallest two consecutive wavelengths, starting with smallest
                 #         # i = np.empty(self.K, int)  # indices which are alternating between 0 and 1
                 #         # i[0::2] = 0
                 #         # i[1::2] = 1
                 #         # l = np.array([lmin, lmin + 1])[i]
             elif l == "exponential":
-                K = int(np.ceil(np.log2(self.vmax))) + 1  # + 1: 2 ** 0 = 1
-                l = np.concatenate(([np.inf], np.geomspace(self.L, self.lmin, K)))
+                # K = int(np.ceil(np.log2(self.vmax))) + 1  # + 1: 2 ** 0 = 1
+                l = np.concatenate(([np.inf], np.geomspace(self.L, self.lmin, self.K)))
             elif l == "linear":
                 l = np.concatenate(([np.inf], np.linspace(self.L, self.lmin, self.K - 1)))
             elif l == "default":
                 l = self.defaults["l"]
             else:
                 return
 
@@ -2050,15 +2107,15 @@
             self.logger.debug(f"self._v = {str(self.v.round(3)).replace(chr(10), ',')}")
             self._UMR = None
             self.D, self.K = self._l.shape  # set l before K and K before f
             self.f = self._f
 
     @property
     def v(self) -> np.ndarray:
-        """Spatial frequencies, i.e. number of periods/fringes across maximum length times delta."""
+        """Spatial frequencies, i.e. number of periods/fringes across maximum length times alpha."""
         if self.D == 1 or len(np.unique(self._v, axis=0)) == 1:  # sets in directions are identical
             v = self._v[0]  # 1D
         else:
             v = self._v  # 2D
         return v
 
     @v.setter
@@ -2089,16 +2146,16 @@
                         # i = np.empty(self.K, int)  # indices which are alternating between 0 and 1
                         # i[0::2] = 0
                         # i[1::2] = 1
                         # l = np.array([lmin, lmin + 1])[i]
 
                         v = self.L / l
             elif v == "exponential":
-                K = int(np.ceil(np.log2(self.vmax))) + 1  # + 1: 2 ** 0 = 1
-                v = np.concatenate(([0], np.geomspace(1, self.vmax, K)))
+                # K = int(np.ceil(np.log2(self.vmax))) + 1  # + 1: 2 ** 0 = 1
+                v = np.concatenate(([0], np.geomspace(1, self.vmax, self.K)))
             elif v == "linear":
                 v = np.concatenate(([0], np.linspace(1, self.vmax, self.K - 1)))
             elif v == "default":
                 v = self.defaults["v"]
             else:
                 return
 
@@ -2117,28 +2174,28 @@
         elif _v.ndim == 2:
             _v = _v[:self._Dmax, :self._Kmax]
         else:
             _v = _v[:self._Dmax, :self._Kmax, ..., -1]
 
         if self.FDM:
             if self.static:
-                if _v.size != self.D * self.K or not np.all(_v % 1 == 0) or not np.lcm.reduce(
-                        _v.astype(int, copy=False).ravel()) == np.prod(_v):  # todo: allow coprimes?!
+                if _v.size != self.D * self.K or not np.all(_v % 1 == 0) or \
+                        not np.lcm.reduce(_v.astype(int, copy=False).ravel()) == np.prod(_v):  # todo: allow coprimes?!
                     n = min(10, self.vmax // 2)
                     ith = self.D * self.K
                     pmax = sympy.ntheory.generate.nextprime(n, ith + 1)
                     p = np.array(list(sympy.ntheory.generate.primerange(n, pmax + 1)))[:ith]  # primes
                     p = [p[-i // 2] if i % 2 else p[i // 2] for i in range(len(p))]  # resort primes
                     _v = np.sort(np.array(p, float).reshape((self.D, self.K)), axis=1)  # resort primes
                     self.logger.warning(f"Periods were not coprime. "
                                         f"Changing values to {str(_v.round(3)).replace(chr(10), ',')}.")
-            else:
-                vmax = (self._Nmax - 1) / 2 > _v
-                if np.any(_v > vmax):  # clip v so that Nmax <= 2 * max(v) + 1 = 2 * max(f) + 1
-                    _v = np.maximum(_v, vmax)
+            # else:
+            #     # from Nmin: fmax = (self.Nmax - 1) / 2, but this is already ensured by Nmax >= 2 * D * K + 1
+            #     vmax = (self._Nmax - 1) / 2 > _v
+            #     _v = np.maximum(_v, vmax)
 
         if _v.size and not np.array_equal(self._v, _v):
             self._v = _v  # set v before D and K
             self.logger.debug(f"self._v = {str(self.v.round(3)).replace(chr(10), ',')}")
             self._l = self.L / self._v
             self.logger.debug(f"self._l = {str(self.l.round(3)).replace(chr(10), ',')}")
             self._UMR = None
@@ -2162,14 +2219,17 @@
             elif f == "default":
                 f = self.defaults[f]
             else:
                 return
 
         # make array, ensure dtype and clip
         _f = np.array(f, float, ndmin=1)
+        if self.FDM:
+            if self.static:
+                pass
 
         # empty array
         if not _f.size:
             return
 
         # change shape to (D, K) or limit shape
         if _f.shape == (1,):
@@ -2179,18 +2239,18 @@
         elif _f.ndim == 2:
             _f = _f[:self._Dmax, :self._Kmax]
         else:
             _f = _f[:self._Dmax, :self._Kmax, ..., -1]
 
         if self.FDM:
             if self.static:
-                _f = self._v  # periods to shift over: take min spatial frequency i.e. max wavelength
+                _f = self._v  # todo: periods to shift over: take min spatial frequency i.e. max wavelength?
             else:
-                if _f.shape != (self.D, self.K) or not np.all(i % 1 == 0 for i in _f) or len(
-                        np.unique(np.abs(_f))) < _f.size:  # assure _f are int, absolute values of _f differ
+                if _f.shape != (self.D, self.K) or not np.all(i % 1 == 0 for i in _f) or \
+                        len(np.unique(np.abs(_f))) < _f.size:  # assure _f are int, absolute values of _f differ
                     _f = np.arange(1, self.D * self.K + 1, dtype=float).reshape((self.D, self.K))
 
         if _f.size and 0 not in _f and not np.array_equal(self._f, _f):
             self._f = _f  # set f before D and K
             self.logger.debug(f"self._f = {str((self.f * (-1 if self.reverse else 1)).round(3)).replace(chr(10), ',')}")
             self.D, self.K = self._f.shape
             self.N = self._N  # todo: remove if fractional periods is implemented, log warning
@@ -2214,15 +2274,15 @@
         return all(len(set(h)) == 1 for h in self.h)
 
     @property
     def Nmin(self) -> int:
         """Minimum number of shifts to (uniformly) sample temporal frequencies."""
         if self.FDM:
             if self.static:
-                Nmin = int(np.ceil(2 * self.f.max() + 1))
+                Nmin = int(np.ceil(2 * self.f.max() + 1))  # todo: 2 * D * K + 1 -> fractional periods
             else:
                 Nmin = 2 * self.D * self.K + 1
         else:
             Nmin = 1
         return Nmin
 
     @property
@@ -2326,16 +2386,15 @@
         """Shape of fringe pattern sequence in video shape, i.e. (frames, height, with, color channels).
         """
         return self.T, self.Y, self.X, self.C
 
     @property
     def size(self) -> np.uint64:
         """Number of pixels of fringe pattern sequence, i.e. frames * height * width * color channels."""
-        # return int(np.prod(self.shape))  # use int() to ensure type is "int" instead of "numpy.core.multiarray.scalar"
-        return np.prod(self.shape, dtype=np.uint64)
+        return float(np.prod(self.shape, dtype=np.uint64))  # use uint64 prevent integer overflow
 
     @property
     def nbytes(self) -> int:
         """Total bytes consumed by fringe pattern sequence.
         Does not include memory consumed by non-element attributes of the array object."""
         return self.size * self.dtype.itemsize
 
@@ -2417,119 +2476,130 @@
     def V(self) -> float:
         """Fringe visibility (fringe contrast)."""
         return self.B / self.A
 
     @V.setter
     def V(self, V: float):
         _V = float(min(max(0, V), self.Vmax))
-        self.B = _V * self.A
+
+        if self._B != _V * self.A:
+            self.B = _V * self.A
+            self.logger.debug(f"{self._V = }")
 
     @property
     def Vmin(self) -> float:
         """Minimum fringe visibility (fringe contrast) for measurement to be valid, within interval [0, 1]."""
         return self._Vmin
 
     @Vmin.setter
     def Vmin(self, Vmin: float):
         _Vmin = float(min(max(0, Vmin), 1))
 
         if self._Vmin != _Vmin:
             self._Vmin = _Vmin
             self.logger.debug(f"{self._Vmin = }")
 
-    # @property
-    # def Q(self) -> int:
-    #     """Number of quantization bits."""
-    #     return 1 if self.dtype.kind in "b" else np.iinfo(
-    #         self.dtype).bits if self.dtype.kind in "ui" else 10 ** np.finfo(self.dtype).precision
+    @property
+    def r(self) -> int:
+        """Number of quantization bits."""
+        return 1 if self.dtype.kind in "b" else np.iinfo(
+            self.dtype).bits if self.dtype.kind in "ui" else 10 ** np.finfo(self.dtype).precision
+
+    @property
+    def Q(self) -> float:
+        """Number of quantization levels."""
+        return 2 ** self.r
 
     @property
     def q(self) -> float:
         """Quantization step size."""
         return 1.0 if self.dtype.kind in "uib" else np.finfo(self.dtype).resolution
 
     @property
-    def QN(self) -> float:
-        """Quantization noise's standard deviation."""
-        return self.q / np.sqrt(12)
+    def quant(self) -> float:
+        """Quantization noise (standard deviation) [DN]."""
+        return float(self.q / np.sqrt(12))  # convert Numpy float64 to Python float
 
     @property
-    def DN(self) -> float:
-        """Dark noise's standard deviation."""
-        return self._DN
+    def dark(self) -> float:
+        """Dark noise of digital camera (standard deviation) [electrons]."""
+        return self._dark
 
-    @DN.setter
-    def DN(self, DN: float):
-        _DN = float(min(max(0, DN), np.sqrt(self.Imax)))
+    @dark.setter
+    def dark(self, dark: float):
+        _dark = float(min(max(0, dark), np.sqrt(self.Imax)))
 
-        _DN = max(0, _DN - np.sqrt(1 / 12))  # correct for quantization noise contained in dark noise measurement
+        # _dark = max(_dark, 0.49)  # todo: temporal noise is dominated by quantization noise ->
 
-        if self._DN != _DN:
-            self._DN = _DN
-            self.logger.debug(f"{self._DN = }")
+        _dark = max(0, _dark - self.quant)  # correct for quantization noise contained in dark noise measurement
+
+        if self._dark != _dark:
+            self._dark = _dark
+            self.logger.debug(f"{self._dark = }")
 
     @property
-    def PN(self) -> float:
-        """Photon noise's standard deviation."""
-        return self._PN
+    def shot(self) -> float:
+        """Shot noise of digital camera (standard deviation) [DN]."""
+        return np.sqrt(self.A / self.gain) if self.gain != 0 else 0  # average intensity is bias
 
-    @PN.setter
-    def PN(self, PN: float):
-        _PN = float(min(max(0, PN), np.sqrt(self.Imax)))
+    @property
+    def esat(self) -> float:
+        """Saturation capacity of digital camera (standard deviation) [electrons]."""
+        return self._esat
 
-        if self._PN != _PN:
-            self._PN = _PN
-            self.logger.debug(f"{self._PN = }")
+    @esat.setter
+    def esat(self, esat: float):
+        _esat = float(max(0, esat))
+
+        if _esat == 0:
+            return
+
+        if self._esat != _esat:
+            self._esat = _esat
+            self.logger.debug(f"{self._esat = }")
+
+    @property
+    def gain(self) -> float:
+        """Overall system gain of digital camera [DN / electrons]."""
+        return self.Q / self._esat
 
     @property
     def u(self) -> np.ndarray:
-        """Uncertainty of measurement [px]."""
-        # if self.SDM:
-        #     B = self.B / self.D
-        # elif self.FDM:
-        #     B = self.B / (self.D * self.K)
-        # else:
-        #     B = self.B
-        SNR = self.B / np.sqrt(self.PN ** 2 + self.DN ** 2 + self.QN ** 2)
+        """Uncertainty of measurement (standard deviation) [px]."""
+        noise = np.sqrt(self.gain ** 2 * self.dark ** 2 + self.quant ** 2 + self.gain ** 2 * self.shot ** 2)
+        SNR = self.B / noise
         upi = np.sqrt(2) / np.sqrt(self.M) / np.sqrt(self._N) / SNR  # local phase uncertainties
         upin = upi / (2 * np.pi)  # normalized local phase uncertainty
         uxi = upin * self._l  # local positional uncertainties
         ux = np.sqrt(1 / np.sum(1 / uxi ** 2))  # global phase uncertainty (by inverse variance weighting of uxi)
-        return ux
+        return float(ux)  # convert Numpy float64 to Python float
 
     @property
     def DR(self) -> float:
         """Dynamic range."""
-        return self.UMR / self.u
+        return self.R / self.u
 
     @property
     def DRdB(self) -> float:
         """Dynamic range [dB]."""
         return 20 * np.log10(self.DR)
 
     @property
     def params(self) -> dict:
         """Base parameters required for en- & decoding fringe patterns."""
         # All property objects which have a setter method i.e. are (usually) not derived from others.
         params = {}
         for p in sorted(dir(self)):
             if isinstance(getattr(type(self), p, None), property) and getattr(type(self), p, None).fset is not None:
-                if p in ["T", "eta"]:  # derived values, but informative, so we want them to be listed
-                    p_ = p
-                else:
-                    p_ = "_" + p
-
-                if isinstance(getattr(self, p_, None), np.ndarray):
-                    param = getattr(self, p_, None).tolist()
-                elif isinstance(getattr(self, p_, None), np.dtype):
-                    param = str(getattr(self, p_, None))
+                if isinstance(getattr(self, p, None), np.ndarray):
+                    params[p] = getattr(self, p, None).tolist()
+                elif isinstance(getattr(self, p, None), np.dtype):
+                    params[p] = str(getattr(self, p, None))
                 else:
-                    param = getattr(self, p_, None)
-
-                params[p] = param
+                    params[p] = getattr(self, p, None)
         return params
 
     # docstrings of properties
     doc = {k: v.__doc__ for k, v in sorted(vars().items()) if isinstance(v, property) and v.__doc__ is not None}
 
     # amplitude = B
```

### Comparing `fringes-0.1.4/fringes/grid.py` & `fringes-0.1.5/fringes/grid.py`

 * *Files identical despite different names*

### Comparing `fringes-0.1.4/fringes/util.py` & `fringes-0.1.5/fringes/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,32 +47,41 @@
         Y, X = I.shape
     elif I.ndim == 1:
         T = I.shape
 
     return I.reshape(T, Y, X, C)
 
 
-def curvature(reg: np.ndarray, calibrated: bool = False) -> np.ndarray:  # todo: test + readme
+def curvature(reg: np.ndarray, calibrated: bool = False) -> np.ndarray:  # todo: test
+    """Local curvature map by deriving a slope map."""
+
     T, Y, X, C = vshape(reg).shape
     reg = reg.reshape(T, Y, X, C)  # returns a view
 
+    assert T == 2, "More than 2 directions."
     assert X >= 2 and Y >= 2, "Shape too small to calculate numerical gradient."
 
-    curv = np.sum(np.gradient(reg[d], axis=0) + np.gradient(reg[d], axis=1) for d in range(T))
+    curv = np.gradient(reg[0], axis=0) + np.gradient(reg[0], axis=1) + \
+           np.gradient(reg[1], axis=0) + np.gradient(reg[1], axis=1)
 
     if not calibrated:
         # curv -= np.mean(curv, axis=(0, 1))
         curv -= np.median(curv, axis=(0, 1))
 
     curv = np.arctan(curv) * 2 / np.pi  # scale [-inf, inf] to [-1, 1]
 
     return curv
 
 
-def relief(curv: np.ndarray, iterations: int = 3) -> np.ndarray:  # todo: test + readme
+def height(curv: np.ndarray, iterations: int = 3) -> np.ndarray:  # todo: test
+    """
+    Local height map by dual local integration via an inverse laplace filter [[19]](#19).\
+    Think of it as a relief, where height is only relative to the local neighborhood.
+    """
+
     k = np.array([[0, 1, 0],
                   [1, 0, 1],
                   [0, 1, 0]], np.float32)
     # k *= iterations  # todo
 
     T, Y, X, C = vshape(curv).shape
     curv = curv.reshape(T, Y, X, C)  # returns a view
```

### Comparing `fringes-0.1.4/LICENSE` & `fringes-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fringes-0.1.4/pyproject.toml` & `fringes-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Fringes"
-version = "0.1.4"
+version = "0.1.5"
 description = "Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns."
 license = "CC-BY-NC-SA-4.0"
 authors = ["Christian Kludt"]
 readme = "README.md"
 repository = "https://github.com/comimag/fringes"
 keywords = ["phase shifting", "fringe analysis", "fringe projection", "deflectometry", "computational imaging"]
```

### Comparing `fringes-0.1.4/README.md` & `fringes-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Fringes
 
 Author: Christian Kludt
 
+[//]: # (![Parameter Interdependencies]&#40;docs/spirals.png&#41;)
+
 ## Description
-This package provides the handy `Fringes` class which handles all the required parameters for configuring a fringe pattern
+This package provides the handy `Fringes` class which handles all the required parameters
+for configuring fringe pattern sequences
 and provides methods for fringe analysis.
 <!---
 link to  paper, please cite
 --->
 
 ### Features
 <!---
@@ -149,28 +152,14 @@
 hence dependent parameters might change as well. 
 The attributes in rectangular boxes are readonly, i.e. they are inferred from the others.
 Only the ones in white boxes will never influence others.
 
 ![Parameter Interdependencies](docs/interdependencies.svg)\
 Parameter and their Interdependencies.
 
-### __Coordinate System__
-The following coordinate systems can be used by setting `grid` to:
-- `'image'`: The top left corner pixel of the grid is the origin (0, 0)
-and positive directions are right- resp. downwards.
-- `'Cartesian'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.
-- `'polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
-- `'log-polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
-
-`D` denotes the number of directions to be encoded.
-If <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system
-(index 0 or 1) the fringes are shifted.
-
-`angle` can be used to tilt the coordinate system. The origin stays the same.
-
 ### __Video Shape__
 Standardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with
 - `T`: number of frames
 - `Y`: height
 - `X`: width
 - `C`: number of color channels
 
@@ -181,14 +170,28 @@
 
 The length `L` is the maximum of `X` and `Y`.
 
 `C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.
 
 `size` is the product of `shape`.
 
+### __Coordinate System__
+The following coordinate systems can be used by setting `grid` to:
+- `'image'`: The top left corner pixel of the grid is the origin (0, 0)
+and positive directions are right- resp. downwards.
+- `'Cartesian'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.
+- `'polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
+- `'log-polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
+
+`D` denotes the number of directions to be encoded.
+If <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system
+(index 0 or 1) the fringes are shifted.
+
+`angle` can be used to tilt the coordinate system. The origin stays the same.
+
 ### __Set__
 Each set consists of the following parameters:
 - `N`: number of shifts
 - `l`: wavelength [px]
 - `v`: spatial frequency, i.e. number of periods (per screen length `L`)
 - `f`: temporal frequency, i.e. number of periods to shift over
 
@@ -314,20 +317,20 @@
 It is influenced by the fringe parameters
 - `M`: number of [averaged](#coloring-and-averaging) intensity samples
 - `N`: number of phase shifts
 - `l`: wavelengths of the fringes
 - `B`: measured amplitude
 
 and the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)
-- `PN`: photon noise of light itself
-- `DN`: dark noise of the used camera
-- `QN`: quantization noise of the light source or camera
+- `dark`: dark noise of the used camera
+- `shot`: photon noise of light itself
+- `quant`: quantization noise of the light source or camera
 
-The maximum possible dynamic range of the measurement is `DR = UMR / u`.
-It describes how many points can be discriminated on the interval `[0, UMR)`.
+The maximum possible dynamic range of the measurement is `DR = L / u`.
+It describes how many points can be discriminated on the interval `[0, L)`.
 It remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).
 
 ## Methods
 - `load(fname)`\
   Load a parameter set from the file `fname` to a `Fringes` instance.
   Supported file formats are `.json`, `.yaml` and `.asdf`.
 - `save(fname)`\
@@ -380,16 +383,17 @@
 - `vshape(I)`\
   Transforms video data of arbitrary shape and dimensionality into the standardized shape `(T, Y, X, C)`, where
   `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.
   Ensures that the array becomes 4-dimensional and that the size of the last dimension,
   i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.
 - `curvature(registration)`\
   Returns a curvature map. 
-- `relief(curvature)`\
-  Local height map by local integration via an inverse laplace filter [[19]](#19).
+- `height(curvature)`\
+  Local height map by local integration via an inverse laplace filter [[19]](#19).\
+  Think of it as a relief, where height is only relative to the local neighborhood.`
 
 ## __Optimal Coding Strategy__
 As makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.
 A minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.
 Any additional 2 shifts compensate for one harmonic of the recorded fringe pattern.
 Therefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them 
 sets a practical upper limit to the feasible number of shifts.
```

### Comparing `fringes-0.1.4/setup.py` & `fringes-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'scikit-image>=0.19.3,<0.20.0',
  'scipy>=1.10.0,<2.0.0',
  'si-prefix>=1.2.2,<2.0.0',
  'sympy>=1.11.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'fringes',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns.',
-    'long_description': '# Fringes\n\nAuthor: Christian Kludt\n\n## Description\nThis package provides the handy `Fringes` class which handles all the required parameters for configuring a fringe pattern\nand provides methods for fringe analysis.\n<!---\nlink to  paper, please cite\n--->\n\n### Features\n<!---\n- Generalized Temporal Phase Unwrappting (GTPU)[[14](#14-kludt-2024)]\n--->\n- Generalized Temporal Phase Unwrappting (GTPU)\n- Uncertainty Propagation\n- Optimal Coding Strategy\n- Deinterlacing\n- Multiplexing\n- Filtering Phase Maps\n- Remapping\n\n### Background\nMany applications, such as fringe projection [[11]](#11-burke-2002) or deflectometry [[1]](#1-burke-2022),\nrequire the ability to encode positional data.\nTo do this, fringe patterns are used to encode the position on the screen / projector (in pixel coordinates)\nat which the camera pixels were looking at during acquisition.\n\n--- FIGURE coding ---\n\n```\nI = A + B * cos(2πvξ/L - 2πft - φ₀)\n  = A + B * cos(kx - wt - φ₀)\n  = A + B * cos(Φ)\n```\n\n- **Encoding**\n  - **Spatial Modulation**\\\nThe x- resp. y-coordinate `ξ` of the screen/projector is normalized into the range `[0, 1)`\nby dividing through the maximum coordinate `L`\nand used to modulate the luminance in a sinusoidal fringe pattern `I`\nwith offset `A`, amplitude `B` and spatial frequency `v`.\n  - **Temporal Modulation**\\\nThe pattern is then shifted `N` times with an equidistant phase shift of `2πf/N` radian each.\nAn additional phase offset `φ₀` may be set, e.g. to let the fringe patterns start with a gray value of zero.\n- **Decoding**\n  - **Temporal Demodulation**\\\nFrom these shifts, the phase map `φ` is determined [[13]](#13-burke-2012). Due to the trigonometric functions used,\nthe global phase `Φ` is wrapped into the interval <code>[0, 2 &pi;]</code> with `v` periods:\n<code>φ &equiv; Φ mod 2&pi;</code>.\n  - **Spatial Demodulation / Phase Unwrapping**\\\nIf only one set with spatial frequency <code>v &le; 1</code> is used,\nno unwrapping is required because one period covers the complete coding range.\nHence, the coordinates `ξ` are computed directly by scaling: <code>ξ = φ / (2&pi;) * L / v</code>.\nThis constitutes the registration, which is a mapping in the same pixel grid as the camera sensor\nand contains the information where each camera pixel, i.e. each camera sightray, was looking at\nduring the fringe pattern acquisition.\nNote that in contrast to binary coding schemes, e.g. Gray code,\nthe coordinates are obtained with sub-pixel precision.\n    - **Temporal Phase Unwrapping (TPU)**\\\nIf multiple sets with different spatial frequencies `v` are used\nand the [unmbiguous measurement range](#quality-metrics) is larger than the coding range <code>UMR &ge; L</code>,\nthe ambiguity of the phase map is resolved by\ngeneralized multi-frequency temporal phase unwrapping (GTPU) [[14]](#14-kludt-2024).\n    - **Spatial Phase Unwrapping (SPU)**\\\nHowever, if only one set with `v > 1` is used, or multiple sets but  `UMR < L`, the ambiguous phase `φ`\nis unwrapped analyzing the neighbouring phase values [[15]](#15-herráez-2002) [[16]](#16-lei-2015).\nThis only yields a relative phase map, therefore absolute positions are unknown.\n\n## Contents\n- [Installation](#installation)\n- [Usage](#usage)\n- [Graphical User Interface](#graphical-user-interface)\n- [Attributes](#attributes)\n- [Methods](#methods)\n- [Optimal Coding Strategy](#optimal-coding-strategy)\n- [Troubleshooting](#troubleshooting)\n- [License](#license)\n- [Project Status](#project-status)\n\n## Installation\nYou can install `fringes` directly from [PyPi](https://pypi.org/) via `pip`:\n\n```\npip install fringes\n```\n\n## Usage\nYou instantiate and deploy the `Fringes` class:\n\n```python\nimport fringes as frng\n\nf = frng.Fringes()      # instanciate class\n```\n\nFor creating the fringe pattern sequence `I`, use the method `encode()`.\nIt will return a [NumPy array](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) \nin [videoshape](#video-shape) (frames, width, height, color channels).\n\n```python\nI = f.encode()          # encode fringe patterns\n```\n\nFor analyzing (recorded) fringe patterns, use the method `decode()`.\nIt will return a [namedtuple](https://docs.python.org/3/library/collections.html#collections.namedtuple), \ncontaining the Numpy arrays brightness `A`, modulation `B` and the coordinates `ξ`,\nall in [videoshape](#video-shape).\n\n```python\nA, B, xi = f.decode(I)  # decode fringe patterns\n```\n\nAll parameters are accesible by the respective attributes of the `Fringes` class.\n\n```python\nf.X = 1920              # set width of the fringe patterns\nf.Y = 1080              # set height of the fringe patterns\nf.K = 2                 # set number of sets\nf.N = 4                 # set number of shifts\nf.v = [9, 10]           # set spatial frequencies\nf.T                     # get the number of frames\n```\n\nA glossary of them is obtained by the class attribute `doc`.\n\n```python\nfrng.Fringes.doc        # get glossary\n```\n\nYou can change the [logging level](https://docs.python.org/3/library/logging.html#levels) of a `Fringes` instance.\nChanging it to `\'DEBUG\'` gives you verbose feedback on which parameters are changed\nand how long functions take to execute.\n\n```python\nf.logger.setLevel("DEBUG")\n```\n<!---\n## Graphical User Interface\nDo you need a GUI? `Fringes` has a sister project that is called `Fringes GUI`:\nhttps://pypi.org/project/fringes-gui/\n--->\n## Attributes\nAll parameters are parsed when setting, so usually several input formats are accepted, e.g.\n`bool`, `int`, `float`, `str` for scalars and additionally `list`, `tuple`, `ndarray` for arrays.\n\nNote that parameters might have circular dependencies which are resolved automatically,\nhence dependent parameters might change as well. \nThe attributes in rectangular boxes are readonly, i.e. they are inferred from the others.\nOnly the ones in white boxes will never influence others.\n\n![Parameter Interdependencies](docs/interdependencies.svg)\\\nParameter and their Interdependencies.\n\n### __Coordinate System__\nThe following coordinate systems can be used by setting `grid` to:\n- `\'image\'`: The top left corner pixel of the grid is the origin (0, 0)\nand positive directions are right- resp. downwards.\n- `\'Cartesian\'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.\n- `\'polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n- `\'log-polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n\n`D` denotes the number of directions to be encoded.\nIf <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system\n(index 0 or 1) the fringes are shifted.\n\n`angle` can be used to tilt the coordinate system. The origin stays the same.\n\n### __Video Shape__\nStandardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with\n- `T`: number of frames\n- `Y`: height\n- `X`: width\n- `C`: number of color channels\n\n`T` depends on the paremeters `H`, `D`, `K`, `N` and the [multiplexing](#multiplexing) methods:\\\nIf all `N` are identical, then `T = H * D * K * N` with `N` as a scalar,\nelse <code>T = H * &sum; N<sub>i</sub></code> with `N` as an array.\\\nIf a [multiplexing](#multiplexing) methods is activated, `T` reduces further.\n\nThe length `L` is the maximum of `X` and `Y`.\n\n`C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.\n\n`size` is the product of `shape`.\n\n### __Set__\nEach set consists of the following parameters:\n- `N`: number of shifts\n- `l`: wavelength [px]\n- `v`: spatial frequency, i.e. number of periods (per screen length `L`)\n- `f`: temporal frequency, i.e. number of periods to shift over\n\nEach is an array with shape (number of directions `D`, number of sets `K`).\\\nFor example, if <code>N.shape &equiv; (2, 3)</code>, it means that we encode `D = 2` directions with `K = 3` sets each.\n\nChanging `D` or `K` directly, changes the shape of all set parameters.\nWhen setting a set parameter with a new shape (`D\'`, `K\'`),\n`D` and `K` are updated as well as the shape of the other set parameters.\n\nPer direction at least one set with <code>N &ge; 3</code> is necessary\nto solve for the three unknowns brightness `A`, modulation `B` and coordinates `ξ`.\n\n`l` and `v` are related by `l = L / v`.\nWhen `L` changes, `v` is kept constant and only `l` is changed.\n\nUsually `f = 1` and is essentially only changed if [frequency division multiplexing](#multiplexing) `FDM` is activated.\n\n`reverse` is a boolean which reverses the direction of the shifts (by multiplying `f` with `-1`).\n\n`o` denotes the phase offset `φ₀` which can be used to\ne.g. let the fringe patterns start (at the origin) with a gray value of zero.\n\n`UMR` denotes the unambiguous measurement range.\nThe coding is only unique in the interval `[0, UMR)`; after that it repeats itself.\nThe `UMR` is derived from `l` and `v`:\n- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.\n- Else, if <code>v &isin; &#8469;</code>,\n  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.\n- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.\n- Else, if <code>l &and; v &isin; &#8477; \\ &#8474;</code>, `l` and `v` are approximated by rational numbers\n  with a fixed length of decimal digits.\n\n### __Coloring and Averaging__\nThe fringe pattern sequence `I` can be colorized by setting the hue `h` to any RGB color tuple\nin the interval `[0, 255]`. However, black `(0, 0, 0)` is not allowed. `h` must be in shape `(H, 3)`:\\\n`H` is the number of hues and can be set directly; 3 is the length of the RGB color tuple.\\\nThe hues `h` can also be set by assigning any combination of the following characters as a string:\n- `\'r\'`: red\n- `\'g\'`: green\n- `\'b\'`: blue\n- `\'c\'`: cyan\n- `\'m\'`: magenta\n- `\'y\'`: yellow\n- `\'w\'`: white\n\n`C` is the number of color channels required for either the set of hues `h`\nor [wavelength division multiplexing](#multiplexing).\nFor example, if all hues are monochromatic, i.e. the RGB values are identical for each hue, `C` equals 1, else 3.\n\nRepeating hues will be fused by averaging them before decoding.\\\n`M` is the number of averaged intensity samples and can be set directly.\n\n### __Multiplexing__\nThe following multiplexing methods can be activated by setting them to `True`:\n- `SDM`: Spatial Division Multiplexing [[2]](#2)\\\n  This results in crossed fringe patterns. The amplitude `B` is halved.\\\n  It can only be activated if we have two directions <code>D &equiv; 2</code>.\\\n  The number of frames `T` is reduced by a factor of 2.\n- `WDM`: Wavelength Divison Multiplexing [[3]](#3)\\\n  All shifts `N` must equal 3. Then, the shifts are multiplexed into the color channel,\n  resulting in an RGB fringe pattern.\\\n  The number of frames `T` is reduced by a factor of 3.\n- `FDM`: Frequency Division Multiplexing [[4]](#4), [[5]](#5)\\\n  Here, the directions `D` and the sets `K` are multiplexed.\n  Hence, the amplitude `B` is reduced by a factor of `D * K`.\\\n  It can only be activated if <code>D &or; K > 1</code> i.e. `D * K > 1`.\\\n  This results in crossed fringe patterns if <code>D &equiv; 2</code>.\\\n  Each set per direction receives an individual temporal frequency `f`,\n  which is used in [temporal demodulation](#temporal-demodulation) to distinguish the individual sets.\\\n  A minimal number of shifts <code>N<sub>min</sub> &ge; &LeftCeiling;</sub> 2 * f<sub>max</sub> + 1 &RightCeiling;</code>\n  is required to satisfy the sampling theorem and `N` is updated automatically if necessary.\\\n  If one wants a static pattern, i.e. one that remains congruent when shifted, set `static` to `True`.\n\n`SDM` and `WDM` can be used together [[6]](#6) (reducing `T` by a factor of 2 * 3 = 6), `FDM` with neighter.\n\nBy default, the aforementioned multiplexing methods are deactivated,\nso we then only have `TDM`: Time Divison Multiplexing.\n\n### __Data Type__\n`dtype` denotes the data type of the fringe pattern sequence `I`.\\\nPossible values are:\n- `\'bool\'`\n- `\'uint8\'` (the default)\n- `\'uint16\'`\n- `\'float32\'`\n- `\'float64\'`\n\nThe total number of bytes `nbytes` consumed by the fringe pattern sequence\nas well as its maximum gray value `Imax` are derived directly from it:\\\n`Imax = 1` for `float` and `bool`,\nand <code>Imax = 2<sup>Q</sup> - 1</code> for `unsigned integers` with `Q` bits.\n\n`Imax` in turn limits the offset `A` and the amplitude `B`.\nThe fringe visibility (also called fringe contrast) is `V = A / B` with <code>V &isin; [0, 1]</code>.\n\nThe quantization step size `q` is also derived from `dtype`:\n`q = 1` for `bool` and `Q`-bit `unsigned integers`, \nand for `float` its corresponding [resolution](https://numpy.org/doc/stable/reference/generated/numpy.finfo.html).\n\nThe standard deviation of the quantization noise  is <code>QN = q / &radic; 12</code>.\n\n### Unwrapping\n- `PU` denotes the phase unwrapping method and is eihter `\'none\'`, `\'temporal\'`, `\'spatial\'` or `\'SSB\'`.\nSee [spatial demodulation](#spatial-demodulation--phase-unwrapping--pu-) for more details.\n- `mode` denotes the mode used for [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-).\n  Choose either `\'fast\'` (the default) or `\'precise\'`.\n- `Vmin` denotes the minimal fringe visibility (fringe contrast) required for the measurement to be valid\nand is in the interval `[0, 1]`. During decoding, pixels with less are discarded, which can speed up the computation.\n- `verbose` can be set to `True` to also receive the wrapped phase map `φ`,\nthe fringe orders `k` and the residuals `r` from decoding.\n- `SSB` denotes **Single Sideband Demodulation** [[17]](#17-takeda) and is deployed\nif <code>K &equiv; H &equiv; N &equiv; 1</code>, i.e. <code>T &equiv; 1</code>\nand the [coordinate system](#coordinate-system) is eighter `\'image\'` or `\'Cartesian\'`.\n\n### __Quality Metrics__\n`eta` denotes the coding efficiency `L / UMR`. It makes no sense to choose `UMR` much larger than `L`,\nbecause then a significant part of the coding range is not used.\n\n`u` denotes the minimum possible uncertainty of the measurement in pixels.\nIt is based on the phase noise model from [[7]](#7),\npropagated through [generalized temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) and converted from phase to pixel units.\nIt is influenced by the fringe parameters\n- `M`: number of [averaged](#coloring-and-averaging) intensity samples\n- `N`: number of phase shifts\n- `l`: wavelengths of the fringes\n- `B`: measured amplitude\n\nand the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)\n- `PN`: photon noise of light itself\n- `DN`: dark noise of the used camera\n- `QN`: quantization noise of the light source or camera\n\nThe maximum possible dynamic range of the measurement is `DR = UMR / u`.\nIt describes how many points can be discriminated on the interval `[0, UMR)`.\nIt remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).\n\n## Methods\n- `load(fname)`\\\n  Load a parameter set from the file `fname` to a `Fringes` instance.\n  Supported file formats are `.json`, `.yaml` and `.asdf`.\n- `save(fname)`\\\n  Save the parameter set of the current `Fringes` instance to the file `fname`.\n  If `fname` is not provided, the default is `params.yaml` within the package\'s directory \'fringes\'.\n- `reset()`\\\n  Reset the parameter set of the current `Fringes` instance to the default values.\n- `auto(T)`\\\n  Automatically set the [optimal parameters](#optimal-coding-strategy) based on the argument `T` (number of frames).\n  This also takes into account the minimum resolvable wavelength `lmin` and the length of the fringe patterns `L`.\n- `setMTF(B)`\\\n  Compute the normalized modulation transfer function at spatial frequencies `v`\n  and use the result to set the optimal `lmin`.\n  `B` is the modulation from decoding. For more details, see [Optimal Coding Strategy](#optimal-coding-strategy).\n- `coordinates()`\\\n  Generate the coordinate matrices of the defined [coordinate system](#coordinate-system).\n- `encode(frames)`\\\n  [Encode](#encoding) the fringe pattern sequence `I`.\\\n  The frames <code>I<sub>t</sub></code> can be encoded indiviually\n  by passing the frame indices `frames`, either as an `integer` or a `tuple`.\n  The default is `None` in which case all frames are encoded.\\\n  To receive the frames iteratively (i.e. in a lazy manner), simply iterate over the `Fringes` instance.\n- `decode(I, verbose)`\\\n  [Decode](#decoding) the fringe pattern sequence `I`.\\\n  If either the argument `verbose` or the attribute with the same name is `True`,\n  additional infomation is computed and retuned: phase maps `φ`, residuals `r` and fringe orders `k`.\\\n  If the argument `denoise` is `True`, the unwrapped phase map is smoothened by a bilateral filter\n  which is edge-preserving.\\\n  If the argument `despike` is `True`, single pixel outliers in the unwrapped phase map\n  are replaced by their local neighborhood using a median filter.\n- `remap(registration, modulation)`\\\n  Mapping decoded registered coordinates `ξ` (having sub-pixel accuracy)\n  from camera grid to (integer) positions on the pattern/screen grid\n  with weights from modulation `B`.\n  The default for `modulation` is `None`, in which case all weights are assumed to equal one.\n  The method yields a grid representing the screen (light source)\n  with the pixel values being a relative measure\n  of how much a screen (light source) pixel contributed\n  to the exposure of the camera sensor.\n- `deinterlace(I)`\\\n  Deinterlace a fringe pattern sequence `I` acquired with a line scan camera\n  while each frame has been displayed and captured\n  while the object has been moved by one pixel.\n\nThe next methods are class-methods:\n- `unwrap(phi)`\\\n  [Unwrap](#spatial-phase-unwrapping--spu-) the phase map `phi` i.e. `φ` spacially.\n\nThe next methods are package-methods:\n- `vshape(I)`\\\n  Transforms video data of arbitrary shape and dimensionality into the standardized shape `(T, Y, X, C)`, where\n  `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.\n  Ensures that the array becomes 4-dimensional and that the size of the last dimension,\n  i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.\n- `curvature(registration)`\\\n  Returns a curvature map. \n- `relief(curvature)`\\\n  Local height map by local integration via an inverse laplace filter [[19]](#19).\n\n## __Optimal Coding Strategy__\nAs makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.\nA minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.\nAny additional 2 shifts compensate for one harmonic of the recorded fringe pattern.\nTherefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them \nsets a practical upper limit to the feasible number of shifts.\n\nGenerally, shorter wavelengths `l` (or equivalently more periods `v`) reduce the uncertainty `u`,\nbut the resolution of the camera and the display must resolve the fringe pattern spatially.\nHence, the used hardware imposes a lower bound for the wavelength (or upper bound for the number of periods).\n   \nAlso, small wavelengths might result in a smaller unambiguous measurement range `UMR`.\nIf two or more sets `K` are used and their wavelengths `l` resp. number of periods `v` are relative primes,\nthe unmbiguous measurement range can be increased many times.\nAs a consequence, one can use much smaller wavelenghts `l` (larger number of periods `v`).\nHowever, it must be assured that the unambiguous measurment range is always equal or larger than both,\nthe width `X` and the height `Y`.\nElse, [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) would yield wrong results and thus instead\n[spatial phase unwrapping](#spatial-phase-unwrapping--spu-) is used.\nBe aware that in the latter case only a relative phase map is obtained,\nwhich lacks the information of where exactly the camera sight rays were looking at during acquisition.\n\nTo simplify finding and setting the optimal parameters, the following methods can be used:\n- `setMTF()`: The optimal `vmax` is determined automativally [[18]](#18-bothe-2008)\nby measuring the **modulation transfer function** `MTF`.\\\n  Therefore, a sequence of exponentially increasing `v` is acquired:\n    1. Set `v` to `\'exponential\'`.\n    2. Encode, acquire and decode the fringe pattern sequence.\n    3. Call the function `setMTF(B)` with the argument `B` from decoding.\n- `v` can be set to `\'auto\'`. This automatically determines the optimal integer set of `v`\n  based on the maximal resolvable spatial frequency `vmax`.\n-  Equivalently, `l` can also be set to `\'auto\'`. This will automatically determine the optimal integer set of `l`\n  based on the minimal resolvable wavelength `lmin = L / vmax`.\n- `T` can be set directly, based on the desired acquisition time.\n  The optimal `K`, `N` and the [multiplexing](#multiplexing) methods will be determined automatically.\n\nAlternatively, simply use the function `auto()`\nto automatically set the optimal `v`, `T` and [multiplexing](#multiplexing) methods.\n\n## Troubleshooting\n<!---\n- __`poetry install` does not work__\n  \n  First, ensure that poetry is installed correctly as descibed onthe [Poetry Website](https://python-poetry.org/docs/).\\\n  Secondly, ensure the correct python version is installed on your system, as specified in the file `pyproject.toml`!\\\n  Thirdly, this can be caused by a proxy which `pip` does not handle correctly.\n  Manually setting the proxy in the Windows settings or even adding a system variable \n`https_proxy = http://YOUR_PROXY:PORT` can resolve this.\n--->\n\n- __Decoding takes a long time__\n  \n  This is probably related to the just-in-time compiler [Numba](https://numba.pydata.org/) \n  used for this computationally expensive function:\n  During the first execution, an initial compilation is executed. \n  This can take several tens of seconds up to single digit minutes, depending on your CPU.\n  However, for any subsequent execution, the compiled code is cached and the code of the function runs much faster, \n  approaching the speeds of code written in C.\n\n\n- __My decoded coordinates show lots of noise__\n\n  Try using more, sets `K` and/or shifts `N` and adjust the used wavelengths `l` resp. number of periods `v`.\\\n  Also, make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.\\\n  Try to avoid under- and overexposure during acquisition.\n\n\n- #### My decoded coordinates show systematic offsets\n  First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.\n  If the timings are not set correctly, the sequence may be a frame off.\\\n  Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.\n  Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value\n  <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.\n  Alternatively, change the gamma value of the light source or camera directly.\n  You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.\n\n## References\n\n#### [11] [Burke 2002]\n[J. Burke, T. Bothe, W. Osten, and C. Hess,\n“Reverse engineering by fringe projection,”\nin Interferometry XI: Applications (W. Osten, ed.), vol. 4778, pp. 312–324, SPIE,\n2002.](https://doi.org/10.1117/12.473547)\n\n#### [1] [Burke 2022] \n[J. Burke, A. Pak, S. Höfer, M. Ziebarth, M. Roschani, J. Beyerer,\n"Deflectometry for specular surfaces: an overview",\narXiv:2204.11592v1 [physics.optics],\n2022.](https://arxiv.org/abs/2204.11592)\n\n#### [2] [Park2008]?\n\n#### [3] [Huang 1999]\n\n#### [4] [Liu 2014] [Liu2010] [Park2008]?\n\n#### [5] [Kludt 2018]\n\n#### [6] [Trumper 2016]\n\n#### [7] [Surrel 1997]\n\n#### [8] [EMVA1288]\n\n#### [9] [Bothe2008]\n\n#### [10] [Fischer]\n\n#### [13] [Burke 2012]\n[J. Burke,\n"Phase Decoding and Reconstruction",\nvol. Optical Methods for Solid Mechanics: A Full-Field Approach, ch. 3, pp. 83–141. Wiley, Weinheim,\n2012.](https://www.wiley.com/en-us/Optical+Methods+for+Solid+Mechanics%3A+A+Full+Field+Approach-p-9783527411115)\n\n#### [14] [Kludt 2024]\n\n#### [15] [Herráez 2002]\n[Miguel Arevallilo Herráaez, David R. Burton, Michael J. Lalor, and Munther A. Gdeisat.\nFast two-dimensional phase-unwrapping algorithm based on sorting by reliability following a noncontinuous path.\nAppl. Opt., 41(35):7437-7444,\nDec 2002.](https://opg.optica.org/ao/abstract.cfm?uri=ao-41-35-7437)\n\n#### [16] [Lei 2015]\n[Hai Lei, Xin yu Chang, Fei Wang, Xiao-Tang Hu, and Xiao-Dong Hu.\nA novel algorithm based on histogram processing of reliability for two-dimensional phase unwrapping.\nOptik - International Journal for Light and Electron Optics, 126(18):1640 - 1644,\n2015.](https://www.sciencedirect.com/science/article/abs/pii/S0030402615003228?via%3Dihub)\n\n#### [17] [Takeda]\n\n#### [18] [Bothe 2008]\n\n#### [19]\nInverse Laplace Filter\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n\n## Project Status\nThis package is in an early stage and under active development,\nso features and functionally will be added in the future.\nFeature requests are warmly welcomed!',
+    'long_description': '# Fringes\n\nAuthor: Christian Kludt\n\n[//]: # (![Parameter Interdependencies]&#40;docs/spirals.png&#41;)\n\n## Description\nThis package provides the handy `Fringes` class which handles all the required parameters\nfor configuring fringe pattern sequences\nand provides methods for fringe analysis.\n<!---\nlink to  paper, please cite\n--->\n\n### Features\n<!---\n- Generalized Temporal Phase Unwrappting (GTPU)[[14](#14-kludt-2024)]\n--->\n- Generalized Temporal Phase Unwrappting (GTPU)\n- Uncertainty Propagation\n- Optimal Coding Strategy\n- Deinterlacing\n- Multiplexing\n- Filtering Phase Maps\n- Remapping\n\n### Background\nMany applications, such as fringe projection [[11]](#11-burke-2002) or deflectometry [[1]](#1-burke-2022),\nrequire the ability to encode positional data.\nTo do this, fringe patterns are used to encode the position on the screen / projector (in pixel coordinates)\nat which the camera pixels were looking at during acquisition.\n\n--- FIGURE coding ---\n\n```\nI = A + B * cos(2πvξ/L - 2πft - φ₀)\n  = A + B * cos(kx - wt - φ₀)\n  = A + B * cos(Φ)\n```\n\n- **Encoding**\n  - **Spatial Modulation**\\\nThe x- resp. y-coordinate `ξ` of the screen/projector is normalized into the range `[0, 1)`\nby dividing through the maximum coordinate `L`\nand used to modulate the luminance in a sinusoidal fringe pattern `I`\nwith offset `A`, amplitude `B` and spatial frequency `v`.\n  - **Temporal Modulation**\\\nThe pattern is then shifted `N` times with an equidistant phase shift of `2πf/N` radian each.\nAn additional phase offset `φ₀` may be set, e.g. to let the fringe patterns start with a gray value of zero.\n- **Decoding**\n  - **Temporal Demodulation**\\\nFrom these shifts, the phase map `φ` is determined [[13]](#13-burke-2012). Due to the trigonometric functions used,\nthe global phase `Φ` is wrapped into the interval <code>[0, 2 &pi;]</code> with `v` periods:\n<code>φ &equiv; Φ mod 2&pi;</code>.\n  - **Spatial Demodulation / Phase Unwrapping**\\\nIf only one set with spatial frequency <code>v &le; 1</code> is used,\nno unwrapping is required because one period covers the complete coding range.\nHence, the coordinates `ξ` are computed directly by scaling: <code>ξ = φ / (2&pi;) * L / v</code>.\nThis constitutes the registration, which is a mapping in the same pixel grid as the camera sensor\nand contains the information where each camera pixel, i.e. each camera sightray, was looking at\nduring the fringe pattern acquisition.\nNote that in contrast to binary coding schemes, e.g. Gray code,\nthe coordinates are obtained with sub-pixel precision.\n    - **Temporal Phase Unwrapping (TPU)**\\\nIf multiple sets with different spatial frequencies `v` are used\nand the [unmbiguous measurement range](#quality-metrics) is larger than the coding range <code>UMR &ge; L</code>,\nthe ambiguity of the phase map is resolved by\ngeneralized multi-frequency temporal phase unwrapping (GTPU) [[14]](#14-kludt-2024).\n    - **Spatial Phase Unwrapping (SPU)**\\\nHowever, if only one set with `v > 1` is used, or multiple sets but  `UMR < L`, the ambiguous phase `φ`\nis unwrapped analyzing the neighbouring phase values [[15]](#15-herráez-2002) [[16]](#16-lei-2015).\nThis only yields a relative phase map, therefore absolute positions are unknown.\n\n## Contents\n- [Installation](#installation)\n- [Usage](#usage)\n- [Graphical User Interface](#graphical-user-interface)\n- [Attributes](#attributes)\n- [Methods](#methods)\n- [Optimal Coding Strategy](#optimal-coding-strategy)\n- [Troubleshooting](#troubleshooting)\n- [License](#license)\n- [Project Status](#project-status)\n\n## Installation\nYou can install `fringes` directly from [PyPi](https://pypi.org/) via `pip`:\n\n```\npip install fringes\n```\n\n## Usage\nYou instantiate and deploy the `Fringes` class:\n\n```python\nimport fringes as frng\n\nf = frng.Fringes()      # instanciate class\n```\n\nFor creating the fringe pattern sequence `I`, use the method `encode()`.\nIt will return a [NumPy array](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) \nin [videoshape](#video-shape) (frames, width, height, color channels).\n\n```python\nI = f.encode()          # encode fringe patterns\n```\n\nFor analyzing (recorded) fringe patterns, use the method `decode()`.\nIt will return a [namedtuple](https://docs.python.org/3/library/collections.html#collections.namedtuple), \ncontaining the Numpy arrays brightness `A`, modulation `B` and the coordinates `ξ`,\nall in [videoshape](#video-shape).\n\n```python\nA, B, xi = f.decode(I)  # decode fringe patterns\n```\n\nAll parameters are accesible by the respective attributes of the `Fringes` class.\n\n```python\nf.X = 1920              # set width of the fringe patterns\nf.Y = 1080              # set height of the fringe patterns\nf.K = 2                 # set number of sets\nf.N = 4                 # set number of shifts\nf.v = [9, 10]           # set spatial frequencies\nf.T                     # get the number of frames\n```\n\nA glossary of them is obtained by the class attribute `doc`.\n\n```python\nfrng.Fringes.doc        # get glossary\n```\n\nYou can change the [logging level](https://docs.python.org/3/library/logging.html#levels) of a `Fringes` instance.\nChanging it to `\'DEBUG\'` gives you verbose feedback on which parameters are changed\nand how long functions take to execute.\n\n```python\nf.logger.setLevel("DEBUG")\n```\n<!---\n## Graphical User Interface\nDo you need a GUI? `Fringes` has a sister project that is called `Fringes GUI`:\nhttps://pypi.org/project/fringes-gui/\n--->\n## Attributes\nAll parameters are parsed when setting, so usually several input formats are accepted, e.g.\n`bool`, `int`, `float`, `str` for scalars and additionally `list`, `tuple`, `ndarray` for arrays.\n\nNote that parameters might have circular dependencies which are resolved automatically,\nhence dependent parameters might change as well. \nThe attributes in rectangular boxes are readonly, i.e. they are inferred from the others.\nOnly the ones in white boxes will never influence others.\n\n![Parameter Interdependencies](docs/interdependencies.svg)\\\nParameter and their Interdependencies.\n\n### __Video Shape__\nStandardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with\n- `T`: number of frames\n- `Y`: height\n- `X`: width\n- `C`: number of color channels\n\n`T` depends on the paremeters `H`, `D`, `K`, `N` and the [multiplexing](#multiplexing) methods:\\\nIf all `N` are identical, then `T = H * D * K * N` with `N` as a scalar,\nelse <code>T = H * &sum; N<sub>i</sub></code> with `N` as an array.\\\nIf a [multiplexing](#multiplexing) methods is activated, `T` reduces further.\n\nThe length `L` is the maximum of `X` and `Y`.\n\n`C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.\n\n`size` is the product of `shape`.\n\n### __Coordinate System__\nThe following coordinate systems can be used by setting `grid` to:\n- `\'image\'`: The top left corner pixel of the grid is the origin (0, 0)\nand positive directions are right- resp. downwards.\n- `\'Cartesian\'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.\n- `\'polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n- `\'log-polar\'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.\n\n`D` denotes the number of directions to be encoded.\nIf <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system\n(index 0 or 1) the fringes are shifted.\n\n`angle` can be used to tilt the coordinate system. The origin stays the same.\n\n### __Set__\nEach set consists of the following parameters:\n- `N`: number of shifts\n- `l`: wavelength [px]\n- `v`: spatial frequency, i.e. number of periods (per screen length `L`)\n- `f`: temporal frequency, i.e. number of periods to shift over\n\nEach is an array with shape (number of directions `D`, number of sets `K`).\\\nFor example, if <code>N.shape &equiv; (2, 3)</code>, it means that we encode `D = 2` directions with `K = 3` sets each.\n\nChanging `D` or `K` directly, changes the shape of all set parameters.\nWhen setting a set parameter with a new shape (`D\'`, `K\'`),\n`D` and `K` are updated as well as the shape of the other set parameters.\n\nPer direction at least one set with <code>N &ge; 3</code> is necessary\nto solve for the three unknowns brightness `A`, modulation `B` and coordinates `ξ`.\n\n`l` and `v` are related by `l = L / v`.\nWhen `L` changes, `v` is kept constant and only `l` is changed.\n\nUsually `f = 1` and is essentially only changed if [frequency division multiplexing](#multiplexing) `FDM` is activated.\n\n`reverse` is a boolean which reverses the direction of the shifts (by multiplying `f` with `-1`).\n\n`o` denotes the phase offset `φ₀` which can be used to\ne.g. let the fringe patterns start (at the origin) with a gray value of zero.\n\n`UMR` denotes the unambiguous measurement range.\nThe coding is only unique in the interval `[0, UMR)`; after that it repeats itself.\nThe `UMR` is derived from `l` and `v`:\n- If <code>l &isin; &#8469;</code>, <code>UMR = lcm(l<sub>i</sub>)</code> with `lcm` being the least common multiple.\n- Else, if <code>v &isin; &#8469;</code>,\n  <code>UMR = `L`/ gcd(v<sub>i</sub>)</code> with `gcd` being the greatest common divisor.\n- Else, if <code>l &and; v &isin; &#8474;</code>, `lcm` resp. `gdc` are extended to rational numbers.\n- Else, if <code>l &and; v &isin; &#8477; \\ &#8474;</code>, `l` and `v` are approximated by rational numbers\n  with a fixed length of decimal digits.\n\n### __Coloring and Averaging__\nThe fringe pattern sequence `I` can be colorized by setting the hue `h` to any RGB color tuple\nin the interval `[0, 255]`. However, black `(0, 0, 0)` is not allowed. `h` must be in shape `(H, 3)`:\\\n`H` is the number of hues and can be set directly; 3 is the length of the RGB color tuple.\\\nThe hues `h` can also be set by assigning any combination of the following characters as a string:\n- `\'r\'`: red\n- `\'g\'`: green\n- `\'b\'`: blue\n- `\'c\'`: cyan\n- `\'m\'`: magenta\n- `\'y\'`: yellow\n- `\'w\'`: white\n\n`C` is the number of color channels required for either the set of hues `h`\nor [wavelength division multiplexing](#multiplexing).\nFor example, if all hues are monochromatic, i.e. the RGB values are identical for each hue, `C` equals 1, else 3.\n\nRepeating hues will be fused by averaging them before decoding.\\\n`M` is the number of averaged intensity samples and can be set directly.\n\n### __Multiplexing__\nThe following multiplexing methods can be activated by setting them to `True`:\n- `SDM`: Spatial Division Multiplexing [[2]](#2)\\\n  This results in crossed fringe patterns. The amplitude `B` is halved.\\\n  It can only be activated if we have two directions <code>D &equiv; 2</code>.\\\n  The number of frames `T` is reduced by a factor of 2.\n- `WDM`: Wavelength Divison Multiplexing [[3]](#3)\\\n  All shifts `N` must equal 3. Then, the shifts are multiplexed into the color channel,\n  resulting in an RGB fringe pattern.\\\n  The number of frames `T` is reduced by a factor of 3.\n- `FDM`: Frequency Division Multiplexing [[4]](#4), [[5]](#5)\\\n  Here, the directions `D` and the sets `K` are multiplexed.\n  Hence, the amplitude `B` is reduced by a factor of `D * K`.\\\n  It can only be activated if <code>D &or; K > 1</code> i.e. `D * K > 1`.\\\n  This results in crossed fringe patterns if <code>D &equiv; 2</code>.\\\n  Each set per direction receives an individual temporal frequency `f`,\n  which is used in [temporal demodulation](#temporal-demodulation) to distinguish the individual sets.\\\n  A minimal number of shifts <code>N<sub>min</sub> &ge; &LeftCeiling;</sub> 2 * f<sub>max</sub> + 1 &RightCeiling;</code>\n  is required to satisfy the sampling theorem and `N` is updated automatically if necessary.\\\n  If one wants a static pattern, i.e. one that remains congruent when shifted, set `static` to `True`.\n\n`SDM` and `WDM` can be used together [[6]](#6) (reducing `T` by a factor of 2 * 3 = 6), `FDM` with neighter.\n\nBy default, the aforementioned multiplexing methods are deactivated,\nso we then only have `TDM`: Time Divison Multiplexing.\n\n### __Data Type__\n`dtype` denotes the data type of the fringe pattern sequence `I`.\\\nPossible values are:\n- `\'bool\'`\n- `\'uint8\'` (the default)\n- `\'uint16\'`\n- `\'float32\'`\n- `\'float64\'`\n\nThe total number of bytes `nbytes` consumed by the fringe pattern sequence\nas well as its maximum gray value `Imax` are derived directly from it:\\\n`Imax = 1` for `float` and `bool`,\nand <code>Imax = 2<sup>Q</sup> - 1</code> for `unsigned integers` with `Q` bits.\n\n`Imax` in turn limits the offset `A` and the amplitude `B`.\nThe fringe visibility (also called fringe contrast) is `V = A / B` with <code>V &isin; [0, 1]</code>.\n\nThe quantization step size `q` is also derived from `dtype`:\n`q = 1` for `bool` and `Q`-bit `unsigned integers`, \nand for `float` its corresponding [resolution](https://numpy.org/doc/stable/reference/generated/numpy.finfo.html).\n\nThe standard deviation of the quantization noise  is <code>QN = q / &radic; 12</code>.\n\n### Unwrapping\n- `PU` denotes the phase unwrapping method and is eihter `\'none\'`, `\'temporal\'`, `\'spatial\'` or `\'SSB\'`.\nSee [spatial demodulation](#spatial-demodulation--phase-unwrapping--pu-) for more details.\n- `mode` denotes the mode used for [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-).\n  Choose either `\'fast\'` (the default) or `\'precise\'`.\n- `Vmin` denotes the minimal fringe visibility (fringe contrast) required for the measurement to be valid\nand is in the interval `[0, 1]`. During decoding, pixels with less are discarded, which can speed up the computation.\n- `verbose` can be set to `True` to also receive the wrapped phase map `φ`,\nthe fringe orders `k` and the residuals `r` from decoding.\n- `SSB` denotes **Single Sideband Demodulation** [[17]](#17-takeda) and is deployed\nif <code>K &equiv; H &equiv; N &equiv; 1</code>, i.e. <code>T &equiv; 1</code>\nand the [coordinate system](#coordinate-system) is eighter `\'image\'` or `\'Cartesian\'`.\n\n### __Quality Metrics__\n`eta` denotes the coding efficiency `L / UMR`. It makes no sense to choose `UMR` much larger than `L`,\nbecause then a significant part of the coding range is not used.\n\n`u` denotes the minimum possible uncertainty of the measurement in pixels.\nIt is based on the phase noise model from [[7]](#7),\npropagated through [generalized temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) and converted from phase to pixel units.\nIt is influenced by the fringe parameters\n- `M`: number of [averaged](#coloring-and-averaging) intensity samples\n- `N`: number of phase shifts\n- `l`: wavelengths of the fringes\n- `B`: measured amplitude\n\nand the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)\n- `dark`: dark noise of the used camera\n- `shot`: photon noise of light itself\n- `quant`: quantization noise of the light source or camera\n\nThe maximum possible dynamic range of the measurement is `DR = L / u`.\nIt describes how many points can be discriminated on the interval `[0, L)`.\nIt remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).\n\n## Methods\n- `load(fname)`\\\n  Load a parameter set from the file `fname` to a `Fringes` instance.\n  Supported file formats are `.json`, `.yaml` and `.asdf`.\n- `save(fname)`\\\n  Save the parameter set of the current `Fringes` instance to the file `fname`.\n  If `fname` is not provided, the default is `params.yaml` within the package\'s directory \'fringes\'.\n- `reset()`\\\n  Reset the parameter set of the current `Fringes` instance to the default values.\n- `auto(T)`\\\n  Automatically set the [optimal parameters](#optimal-coding-strategy) based on the argument `T` (number of frames).\n  This also takes into account the minimum resolvable wavelength `lmin` and the length of the fringe patterns `L`.\n- `setMTF(B)`\\\n  Compute the normalized modulation transfer function at spatial frequencies `v`\n  and use the result to set the optimal `lmin`.\n  `B` is the modulation from decoding. For more details, see [Optimal Coding Strategy](#optimal-coding-strategy).\n- `coordinates()`\\\n  Generate the coordinate matrices of the defined [coordinate system](#coordinate-system).\n- `encode(frames)`\\\n  [Encode](#encoding) the fringe pattern sequence `I`.\\\n  The frames <code>I<sub>t</sub></code> can be encoded indiviually\n  by passing the frame indices `frames`, either as an `integer` or a `tuple`.\n  The default is `None` in which case all frames are encoded.\\\n  To receive the frames iteratively (i.e. in a lazy manner), simply iterate over the `Fringes` instance.\n- `decode(I, verbose)`\\\n  [Decode](#decoding) the fringe pattern sequence `I`.\\\n  If either the argument `verbose` or the attribute with the same name is `True`,\n  additional infomation is computed and retuned: phase maps `φ`, residuals `r` and fringe orders `k`.\\\n  If the argument `denoise` is `True`, the unwrapped phase map is smoothened by a bilateral filter\n  which is edge-preserving.\\\n  If the argument `despike` is `True`, single pixel outliers in the unwrapped phase map\n  are replaced by their local neighborhood using a median filter.\n- `remap(registration, modulation)`\\\n  Mapping decoded registered coordinates `ξ` (having sub-pixel accuracy)\n  from camera grid to (integer) positions on the pattern/screen grid\n  with weights from modulation `B`.\n  The default for `modulation` is `None`, in which case all weights are assumed to equal one.\n  The method yields a grid representing the screen (light source)\n  with the pixel values being a relative measure\n  of how much a screen (light source) pixel contributed\n  to the exposure of the camera sensor.\n- `deinterlace(I)`\\\n  Deinterlace a fringe pattern sequence `I` acquired with a line scan camera\n  while each frame has been displayed and captured\n  while the object has been moved by one pixel.\n\nThe next methods are class-methods:\n- `unwrap(phi)`\\\n  [Unwrap](#spatial-phase-unwrapping--spu-) the phase map `phi` i.e. `φ` spacially.\n\nThe next methods are package-methods:\n- `vshape(I)`\\\n  Transforms video data of arbitrary shape and dimensionality into the standardized shape `(T, Y, X, C)`, where\n  `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.\n  Ensures that the array becomes 4-dimensional and that the size of the last dimension,\n  i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.\n- `curvature(registration)`\\\n  Returns a curvature map. \n- `height(curvature)`\\\n  Local height map by local integration via an inverse laplace filter [[19]](#19).\\\n  Think of it as a relief, where height is only relative to the local neighborhood.`\n\n## __Optimal Coding Strategy__\nAs makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.\nA minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.\nAny additional 2 shifts compensate for one harmonic of the recorded fringe pattern.\nTherefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them \nsets a practical upper limit to the feasible number of shifts.\n\nGenerally, shorter wavelengths `l` (or equivalently more periods `v`) reduce the uncertainty `u`,\nbut the resolution of the camera and the display must resolve the fringe pattern spatially.\nHence, the used hardware imposes a lower bound for the wavelength (or upper bound for the number of periods).\n   \nAlso, small wavelengths might result in a smaller unambiguous measurement range `UMR`.\nIf two or more sets `K` are used and their wavelengths `l` resp. number of periods `v` are relative primes,\nthe unmbiguous measurement range can be increased many times.\nAs a consequence, one can use much smaller wavelenghts `l` (larger number of periods `v`).\nHowever, it must be assured that the unambiguous measurment range is always equal or larger than both,\nthe width `X` and the height `Y`.\nElse, [temporal phase unwrapping](#temporal-phase-unwrapping--tpu-) would yield wrong results and thus instead\n[spatial phase unwrapping](#spatial-phase-unwrapping--spu-) is used.\nBe aware that in the latter case only a relative phase map is obtained,\nwhich lacks the information of where exactly the camera sight rays were looking at during acquisition.\n\nTo simplify finding and setting the optimal parameters, the following methods can be used:\n- `setMTF()`: The optimal `vmax` is determined automativally [[18]](#18-bothe-2008)\nby measuring the **modulation transfer function** `MTF`.\\\n  Therefore, a sequence of exponentially increasing `v` is acquired:\n    1. Set `v` to `\'exponential\'`.\n    2. Encode, acquire and decode the fringe pattern sequence.\n    3. Call the function `setMTF(B)` with the argument `B` from decoding.\n- `v` can be set to `\'auto\'`. This automatically determines the optimal integer set of `v`\n  based on the maximal resolvable spatial frequency `vmax`.\n-  Equivalently, `l` can also be set to `\'auto\'`. This will automatically determine the optimal integer set of `l`\n  based on the minimal resolvable wavelength `lmin = L / vmax`.\n- `T` can be set directly, based on the desired acquisition time.\n  The optimal `K`, `N` and the [multiplexing](#multiplexing) methods will be determined automatically.\n\nAlternatively, simply use the function `auto()`\nto automatically set the optimal `v`, `T` and [multiplexing](#multiplexing) methods.\n\n## Troubleshooting\n<!---\n- __`poetry install` does not work__\n  \n  First, ensure that poetry is installed correctly as descibed onthe [Poetry Website](https://python-poetry.org/docs/).\\\n  Secondly, ensure the correct python version is installed on your system, as specified in the file `pyproject.toml`!\\\n  Thirdly, this can be caused by a proxy which `pip` does not handle correctly.\n  Manually setting the proxy in the Windows settings or even adding a system variable \n`https_proxy = http://YOUR_PROXY:PORT` can resolve this.\n--->\n\n- __Decoding takes a long time__\n  \n  This is probably related to the just-in-time compiler [Numba](https://numba.pydata.org/) \n  used for this computationally expensive function:\n  During the first execution, an initial compilation is executed. \n  This can take several tens of seconds up to single digit minutes, depending on your CPU.\n  However, for any subsequent execution, the compiled code is cached and the code of the function runs much faster, \n  approaching the speeds of code written in C.\n\n\n- __My decoded coordinates show lots of noise__\n\n  Try using more, sets `K` and/or shifts `N` and adjust the used wavelengths `l` resp. number of periods `v`.\\\n  Also, make sure the exposure of your camera is adjusted so that the fringe patterns show up with maximum contrast.\\\n  Try to avoid under- and overexposure during acquisition.\n\n\n- #### My decoded coordinates show systematic offsets\n  First, ensure that the correct frame was captured while acquiring the fringe pattern sequence.\n  If the timings are not set correctly, the sequence may be a frame off.\\\n  Secondly, this might occur if either the camera or the display used have a gamma value very different from 1.\n  Typical screens have a gamma value of 2.2;   therefore compensate by setting the inverse value\n  <code>gamma<sup>-1</sup> = 1 / 2.2 &approx; 0.45</code> to the `gamma` attribute of the `Fringes` instance.\n  Alternatively, change the gamma value of the light source or camera directly.\n  You might also use more shifts `N` to compensate for the dominant harmonics of the gamma-nonlinearities.\n\n## References\n\n#### [11] [Burke 2002]\n[J. Burke, T. Bothe, W. Osten, and C. Hess,\n“Reverse engineering by fringe projection,”\nin Interferometry XI: Applications (W. Osten, ed.), vol. 4778, pp. 312–324, SPIE,\n2002.](https://doi.org/10.1117/12.473547)\n\n#### [1] [Burke 2022] \n[J. Burke, A. Pak, S. Höfer, M. Ziebarth, M. Roschani, J. Beyerer,\n"Deflectometry for specular surfaces: an overview",\narXiv:2204.11592v1 [physics.optics],\n2022.](https://arxiv.org/abs/2204.11592)\n\n#### [2] [Park2008]?\n\n#### [3] [Huang 1999]\n\n#### [4] [Liu 2014] [Liu2010] [Park2008]?\n\n#### [5] [Kludt 2018]\n\n#### [6] [Trumper 2016]\n\n#### [7] [Surrel 1997]\n\n#### [8] [EMVA1288]\n\n#### [9] [Bothe2008]\n\n#### [10] [Fischer]\n\n#### [13] [Burke 2012]\n[J. Burke,\n"Phase Decoding and Reconstruction",\nvol. Optical Methods for Solid Mechanics: A Full-Field Approach, ch. 3, pp. 83–141. Wiley, Weinheim,\n2012.](https://www.wiley.com/en-us/Optical+Methods+for+Solid+Mechanics%3A+A+Full+Field+Approach-p-9783527411115)\n\n#### [14] [Kludt 2024]\n\n#### [15] [Herráez 2002]\n[Miguel Arevallilo Herráaez, David R. Burton, Michael J. Lalor, and Munther A. Gdeisat.\nFast two-dimensional phase-unwrapping algorithm based on sorting by reliability following a noncontinuous path.\nAppl. Opt., 41(35):7437-7444,\nDec 2002.](https://opg.optica.org/ao/abstract.cfm?uri=ao-41-35-7437)\n\n#### [16] [Lei 2015]\n[Hai Lei, Xin yu Chang, Fei Wang, Xiao-Tang Hu, and Xiao-Dong Hu.\nA novel algorithm based on histogram processing of reliability for two-dimensional phase unwrapping.\nOptik - International Journal for Light and Electron Optics, 126(18):1640 - 1644,\n2015.](https://www.sciencedirect.com/science/article/abs/pii/S0030402615003228?via%3Dihub)\n\n#### [17] [Takeda]\n\n#### [18] [Bothe 2008]\n\n#### [19]\nInverse Laplace Filter\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n\n## Project Status\nThis package is in an early stage and under active development,\nso features and functionally will be added in the future.\nFeature requests are warmly welcomed!',
     'author': 'Christian Kludt',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/comimag/fringes',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fringes-0.1.4/PKG-INFO` & `fringes-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fringes
-Version: 0.1.4
+Version: 0.1.5
 Summary: Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns.
 Home-page: https://github.com/comimag/fringes
 License: CC-BY-NC-SA-4.0
 Keywords: phase shifting,fringe analysis,fringe projection,deflectometry,computational imaging
 Author: Christian Kludt
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
@@ -21,16 +21,19 @@
 Project-URL: Repository, https://github.com/comimag/fringes
 Description-Content-Type: text/markdown
 
 # Fringes
 
 Author: Christian Kludt
 
+[//]: # (![Parameter Interdependencies]&#40;docs/spirals.png&#41;)
+
 ## Description
-This package provides the handy `Fringes` class which handles all the required parameters for configuring a fringe pattern
+This package provides the handy `Fringes` class which handles all the required parameters
+for configuring fringe pattern sequences
 and provides methods for fringe analysis.
 <!---
 link to  paper, please cite
 --->
 
 ### Features
 <!---
@@ -172,28 +175,14 @@
 hence dependent parameters might change as well. 
 The attributes in rectangular boxes are readonly, i.e. they are inferred from the others.
 Only the ones in white boxes will never influence others.
 
 ![Parameter Interdependencies](docs/interdependencies.svg)\
 Parameter and their Interdependencies.
 
-### __Coordinate System__
-The following coordinate systems can be used by setting `grid` to:
-- `'image'`: The top left corner pixel of the grid is the origin (0, 0)
-and positive directions are right- resp. downwards.
-- `'Cartesian'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.
-- `'polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
-- `'log-polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
-
-`D` denotes the number of directions to be encoded.
-If <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system
-(index 0 or 1) the fringes are shifted.
-
-`angle` can be used to tilt the coordinate system. The origin stays the same.
-
 ### __Video Shape__
 Standardized `shape` `(T, Y, X, C)` of fringe pattern sequence, with
 - `T`: number of frames
 - `Y`: height
 - `X`: width
 - `C`: number of color channels
 
@@ -204,14 +193,28 @@
 
 The length `L` is the maximum of `X` and `Y`.
 
 `C` depends on the [coloring](#coloring-and-averaging) and [multiplexing](#multiplexing) methods.
 
 `size` is the product of `shape`.
 
+### __Coordinate System__
+The following coordinate systems can be used by setting `grid` to:
+- `'image'`: The top left corner pixel of the grid is the origin (0, 0)
+and positive directions are right- resp. downwards.
+- `'Cartesian'`: The center of grid is the origin (0, 0) and positive directions are right- resp. upwards.
+- `'polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
+- `'log-polar'`: The center of grid is the origin (0, 0) and positive directions are clockwise resp. outwards.
+
+`D` denotes the number of directions to be encoded.
+If <code>D &equiv; 1</code>, the parameter `axis` is used to define along which axis of the coordinate system
+(index 0 or 1) the fringes are shifted.
+
+`angle` can be used to tilt the coordinate system. The origin stays the same.
+
 ### __Set__
 Each set consists of the following parameters:
 - `N`: number of shifts
 - `l`: wavelength [px]
 - `v`: spatial frequency, i.e. number of periods (per screen length `L`)
 - `f`: temporal frequency, i.e. number of periods to shift over
 
@@ -337,20 +340,20 @@
 It is influenced by the fringe parameters
 - `M`: number of [averaged](#coloring-and-averaging) intensity samples
 - `N`: number of phase shifts
 - `l`: wavelengths of the fringes
 - `B`: measured amplitude
 
 and the measurement hardware-specific noise sources [[8]](#8), [[9]](#9)
-- `PN`: photon noise of light itself
-- `DN`: dark noise of the used camera
-- `QN`: quantization noise of the light source or camera
+- `dark`: dark noise of the used camera
+- `shot`: photon noise of light itself
+- `quant`: quantization noise of the light source or camera
 
-The maximum possible dynamic range of the measurement is `DR = UMR / u`.
-It describes how many points can be discriminated on the interval `[0, UMR)`.
+The maximum possible dynamic range of the measurement is `DR = L / u`.
+It describes how many points can be discriminated on the interval `[0, L)`.
 It remains constant if `L` and hence `l` are scaled (the scaling factor cancels out).
 
 ## Methods
 - `load(fname)`\
   Load a parameter set from the file `fname` to a `Fringes` instance.
   Supported file formats are `.json`, `.yaml` and `.asdf`.
 - `save(fname)`\
@@ -403,16 +406,17 @@
 - `vshape(I)`\
   Transforms video data of arbitrary shape and dimensionality into the standardized shape `(T, Y, X, C)`, where
   `T` is number of frames, `Y` is height, `X` is width, and `C` is number of color channels.
   Ensures that the array becomes 4-dimensional and that the size of the last dimension,
   i.e. the number of color channels <code>C &isin; {1; 3; 4}</code>. To do this, leading dimensions may be flattened.
 - `curvature(registration)`\
   Returns a curvature map. 
-- `relief(curvature)`\
-  Local height map by local integration via an inverse laplace filter [[19]](#19).
+- `height(curvature)`\
+  Local height map by local integration via an inverse laplace filter [[19]](#19).\
+  Think of it as a relief, where height is only relative to the local neighborhood.`
 
 ## __Optimal Coding Strategy__
 As makes sense intuitively, more sets `K` as well as more shifts `N` per set reduce the uncertainty `u` after decoding.
 A minimum of 3 shifts is needed to solve for the 3 unknowns brightness `A`, modulation `B` and coordinates `ξ`.
 Any additional 2 shifts compensate for one harmonic of the recorded fringe pattern.
 Therefore, higher accuracy can be achieved using more shifts `N`, but the time required to capture them 
 sets a practical upper limit to the feasible number of shifts.
```

