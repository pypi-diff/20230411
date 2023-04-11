# Comparing `tmp/pfhedge-0.8.1.tar.gz` & `tmp/pfhedge-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfhedge-0.8.1.tar", max compression
+gzip compressed data, was "pfhedge-0.9.0.tar", max compression
```

## Comparing `pfhedge-0.8.1.tar` & `pfhedge-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1071 2021-07-16 00:45:39.110603 pfhedge-0.8.1/LICENSE
--rw-r--r--   0        0        0      132 2021-07-16 00:45:39.125320 pfhedge-0.8.1/pfhedge/__init__.py
--rw-r--r--   0        0        0        0 2021-07-16 00:45:39.125421 pfhedge-0.8.1/pfhedge/_utils/__init__.py
--rw-r--r--   0        0        0     2460 2021-08-16 05:11:22.847779 pfhedge-0.8.1/pfhedge/_utils/bisect.py
--rw-r--r--   0        0        0      335 2021-08-15 05:54:16.180609 pfhedge-0.8.1/pfhedge/_utils/doc.py
--rw-r--r--   0        0        0      721 2021-08-16 05:11:22.848241 pfhedge-0.8.1/pfhedge/_utils/hook.py
--rw-r--r--   0        0        0      228 2021-08-16 05:11:22.848480 pfhedge-0.8.1/pfhedge/_utils/lazy.py
--rw-r--r--   0        0        0      856 2021-07-16 00:45:39.125861 pfhedge-0.8.1/pfhedge/_utils/operations.py
--rw-r--r--   0        0        0      576 2021-08-15 14:09:52.178287 pfhedge-0.8.1/pfhedge/_utils/parse.py
--rw-r--r--   0        0        0     5215 2021-08-16 05:11:22.848681 pfhedge-0.8.1/pfhedge/autogreek.py
--rw-r--r--   0        0        0      422 2021-07-16 00:45:39.126722 pfhedge-0.8.1/pfhedge/features/__init__.py
--rw-r--r--   0        0        0     1164 2021-07-16 00:45:39.126971 pfhedge-0.8.1/pfhedge/features/_base.py
--rw-r--r--   0        0        0     1268 2021-08-16 08:29:58.981855 pfhedge-0.8.1/pfhedge/features/_getter.py
--rw-r--r--   0        0        0     6304 2021-08-16 08:29:58.982252 pfhedge-0.8.1/pfhedge/features/features.py
--rw-r--r--   0        0        0     1576 2021-08-16 08:29:58.982547 pfhedge-0.8.1/pfhedge/features/functional.py
--rw-r--r--   0        0        0      376 2021-07-16 00:45:39.127480 pfhedge-0.8.1/pfhedge/instruments/__init__.py
--rw-r--r--   0        0        0     3994 2021-08-16 08:29:58.982883 pfhedge-0.8.1/pfhedge/instruments/base.py
--rw-r--r--   0        0        0        0 2021-07-16 00:45:39.127785 pfhedge-0.8.1/pfhedge/instruments/derivative/__init__.py
--rw-r--r--   0        0        0     4649 2021-08-16 08:29:58.983212 pfhedge-0.8.1/pfhedge/instruments/derivative/american_binary.py
--rw-r--r--   0        0        0     5453 2021-08-16 08:29:58.983479 pfhedge-0.8.1/pfhedge/instruments/derivative/base.py
--rw-r--r--   0        0        0     4213 2021-08-16 08:29:58.983749 pfhedge-0.8.1/pfhedge/instruments/derivative/european.py
--rw-r--r--   0        0        0     4450 2021-08-16 08:29:58.984020 pfhedge-0.8.1/pfhedge/instruments/derivative/european_binary.py
--rw-r--r--   0        0        0     4292 2021-08-16 08:29:58.984286 pfhedge-0.8.1/pfhedge/instruments/derivative/lookback.py
--rw-r--r--   0        0        0        0 2021-07-16 00:45:39.128609 pfhedge-0.8.1/pfhedge/instruments/primary/__init__.py
--rw-r--r--   0        0        0     5902 2021-08-16 08:29:58.984719 pfhedge-0.8.1/pfhedge/instruments/primary/base.py
--rw-r--r--   0        0        0     5060 2021-08-16 08:29:58.984963 pfhedge-0.8.1/pfhedge/instruments/primary/brownian.py
--rw-r--r--   0        0        0     5728 2021-08-16 08:29:58.985222 pfhedge-0.8.1/pfhedge/instruments/primary/heston.py
--rw-r--r--   0        0        0      707 2021-07-16 00:45:39.129309 pfhedge-0.8.1/pfhedge/nn/__init__.py
--rw-r--r--   0        0        0     7307 2021-08-16 08:29:58.985507 pfhedge-0.8.1/pfhedge/nn/functional.py
--rw-r--r--   0        0        0        0 2021-07-16 00:45:39.129594 pfhedge-0.8.1/pfhedge/nn/modules/__init__.py
--rw-r--r--   0        0        0        0 2021-07-16 00:45:39.129704 pfhedge-0.8.1/pfhedge/nn/modules/bs/__init__.py
--rw-r--r--   0        0        0     2768 2021-08-16 08:29:58.985823 pfhedge-0.8.1/pfhedge/nn/modules/bs/_base.py
--rw-r--r--   0        0        0     7985 2021-08-16 08:29:58.986114 pfhedge-0.8.1/pfhedge/nn/modules/bs/american_binary.py
--rw-r--r--   0        0        0     3197 2021-08-16 05:11:22.855807 pfhedge-0.8.1/pfhedge/nn/modules/bs/black_scholes.py
--rw-r--r--   0        0        0     6579 2021-08-16 08:29:58.986425 pfhedge-0.8.1/pfhedge/nn/modules/bs/european.py
--rw-r--r--   0        0        0     6615 2021-08-16 08:29:58.986672 pfhedge-0.8.1/pfhedge/nn/modules/bs/european_binary.py
--rw-r--r--   0        0        0     8609 2021-08-16 08:29:58.986964 pfhedge-0.8.1/pfhedge/nn/modules/bs/lookback.py
--rw-r--r--   0        0        0     5373 2021-08-16 08:29:58.987256 pfhedge-0.8.1/pfhedge/nn/modules/clamp.py
--rw-r--r--   0        0        0    16268 2021-08-16 08:29:58.987753 pfhedge-0.8.1/pfhedge/nn/modules/hedger.py
--rw-r--r--   0        0        0     8888 2021-08-16 08:29:58.988209 pfhedge-0.8.1/pfhedge/nn/modules/loss.py
--rw-r--r--   0        0        0     4429 2021-08-16 05:11:22.860746 pfhedge-0.8.1/pfhedge/nn/modules/mlp.py
--rw-r--r--   0        0        0     1100 2021-08-16 05:11:22.862054 pfhedge-0.8.1/pfhedge/nn/modules/naked.py
--rw-r--r--   0        0        0     4024 2021-08-16 08:29:58.988593 pfhedge-0.8.1/pfhedge/nn/modules/ww.py
--rw-r--r--   0        0        0      156 2021-07-16 00:45:39.131765 pfhedge-0.8.1/pfhedge/stochastic/__init__.py
--rw-r--r--   0        0        0     5642 2021-08-15 05:54:16.188006 pfhedge-0.8.1/pfhedge/stochastic/brownian.py
--rw-r--r--   0        0        0     4637 2021-08-16 08:29:58.988990 pfhedge-0.8.1/pfhedge/stochastic/cir.py
--rw-r--r--   0        0        0     4435 2021-08-16 08:29:58.989428 pfhedge-0.8.1/pfhedge/stochastic/heston.py
--rw-r--r--   0        0        0      618 2021-08-16 08:29:58.989755 pfhedge-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      896 2021-08-16 08:30:57.780805 pfhedge-0.8.1/setup.py
--rw-r--r--   0        0        0      636 2021-08-16 08:30:57.781031 pfhedge-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-07-16 00:45:39.110603 pfhedge-0.9.0/LICENSE
+-rw-r--r--   0        0        0      132 2021-07-16 00:45:39.125320 pfhedge-0.9.0/pfhedge/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-16 00:45:39.125421 pfhedge-0.9.0/pfhedge/_utils/__init__.py
+-rw-r--r--   0        0        0     2460 2021-08-17 12:06:22.470088 pfhedge-0.9.0/pfhedge/_utils/bisect.py
+-rw-r--r--   0        0        0      333 2021-08-17 12:06:22.470601 pfhedge-0.9.0/pfhedge/_utils/doc.py
+-rw-r--r--   0        0        0      723 2021-08-17 12:06:22.471026 pfhedge-0.9.0/pfhedge/_utils/hook.py
+-rw-r--r--   0        0        0      157 2021-08-17 12:06:22.471429 pfhedge-0.9.0/pfhedge/_utils/lazy.py
+-rw-r--r--   0        0        0      856 2021-07-16 00:45:39.125861 pfhedge-0.9.0/pfhedge/_utils/operations.py
+-rw-r--r--   0        0        0      576 2021-08-15 14:09:52.178287 pfhedge-0.9.0/pfhedge/_utils/parse.py
+-rw-r--r--   0        0        0     5268 2021-08-17 12:06:22.471773 pfhedge-0.9.0/pfhedge/autogreek.py
+-rw-r--r--   0        0        0      422 2021-07-16 00:45:39.126722 pfhedge-0.9.0/pfhedge/features/__init__.py
+-rw-r--r--   0        0        0     1170 2021-08-17 12:06:22.472168 pfhedge-0.9.0/pfhedge/features/_base.py
+-rw-r--r--   0        0        0     1213 2021-08-17 12:06:22.472609 pfhedge-0.9.0/pfhedge/features/_getter.py
+-rw-r--r--   0        0        0     6301 2021-08-17 12:06:22.473058 pfhedge-0.9.0/pfhedge/features/features.py
+-rw-r--r--   0        0        0     1576 2021-08-16 23:51:45.107918 pfhedge-0.9.0/pfhedge/features/functional.py
+-rw-r--r--   0        0        0      427 2021-08-17 12:06:22.473568 pfhedge-0.9.0/pfhedge/instruments/__init__.py
+-rw-r--r--   0        0        0     3967 2021-08-17 12:06:22.473991 pfhedge-0.9.0/pfhedge/instruments/base.py
+-rw-r--r--   0        0        0        0 2021-07-16 00:45:39.127785 pfhedge-0.9.0/pfhedge/instruments/derivative/__init__.py
+-rw-r--r--   0        0        0     4671 2021-08-17 12:06:22.474337 pfhedge-0.9.0/pfhedge/instruments/derivative/american_binary.py
+-rw-r--r--   0        0        0     5502 2021-08-17 12:06:22.474638 pfhedge-0.9.0/pfhedge/instruments/derivative/base.py
+-rw-r--r--   0        0        0     4239 2021-08-17 12:06:22.474940 pfhedge-0.9.0/pfhedge/instruments/derivative/european.py
+-rw-r--r--   0        0        0     4472 2021-08-17 12:06:22.475262 pfhedge-0.9.0/pfhedge/instruments/derivative/european_binary.py
+-rw-r--r--   0        0        0     4314 2021-08-17 12:06:22.475578 pfhedge-0.9.0/pfhedge/instruments/derivative/lookback.py
+-rw-r--r--   0        0        0     3641 2021-08-17 12:06:22.475835 pfhedge-0.9.0/pfhedge/instruments/derivative/variance_swap.py
+-rw-r--r--   0        0        0        0 2021-07-16 00:45:39.128609 pfhedge-0.9.0/pfhedge/instruments/primary/__init__.py
+-rw-r--r--   0        0        0     6092 2021-08-17 12:06:22.476433 pfhedge-0.9.0/pfhedge/instruments/primary/base.py
+-rw-r--r--   0        0        0     5147 2021-08-17 12:06:22.476916 pfhedge-0.9.0/pfhedge/instruments/primary/brownian.py
+-rw-r--r--   0        0        0     5769 2021-08-17 12:06:22.477301 pfhedge-0.9.0/pfhedge/instruments/primary/heston.py
+-rw-r--r--   0        0        0      707 2021-07-16 00:45:39.129309 pfhedge-0.9.0/pfhedge/nn/__init__.py
+-rw-r--r--   0        0        0     8834 2021-08-17 12:06:22.477811 pfhedge-0.9.0/pfhedge/nn/functional.py
+-rw-r--r--   0        0        0        0 2021-07-16 00:45:39.129594 pfhedge-0.9.0/pfhedge/nn/modules/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-16 00:45:39.129704 pfhedge-0.9.0/pfhedge/nn/modules/bs/__init__.py
+-rw-r--r--   0        0        0     2794 2021-08-17 12:06:22.478301 pfhedge-0.9.0/pfhedge/nn/modules/bs/_base.py
+-rw-r--r--   0        0        0     7991 2021-08-17 12:06:22.479051 pfhedge-0.9.0/pfhedge/nn/modules/bs/american_binary.py
+-rw-r--r--   0        0        0     3205 2021-08-17 12:06:22.479520 pfhedge-0.9.0/pfhedge/nn/modules/bs/black_scholes.py
+-rw-r--r--   0        0        0     6581 2021-08-17 12:06:22.480167 pfhedge-0.9.0/pfhedge/nn/modules/bs/european.py
+-rw-r--r--   0        0        0     6621 2021-08-17 12:06:22.480615 pfhedge-0.9.0/pfhedge/nn/modules/bs/european_binary.py
+-rw-r--r--   0        0        0     8615 2021-08-17 12:06:22.481021 pfhedge-0.9.0/pfhedge/nn/modules/bs/lookback.py
+-rw-r--r--   0        0        0     5381 2021-08-17 12:06:22.481437 pfhedge-0.9.0/pfhedge/nn/modules/clamp.py
+-rw-r--r--   0        0        0    16301 2021-08-17 12:06:22.482461 pfhedge-0.9.0/pfhedge/nn/modules/hedger.py
+-rw-r--r--   0        0        0     8925 2021-08-17 12:06:22.483138 pfhedge-0.9.0/pfhedge/nn/modules/loss.py
+-rw-r--r--   0        0        0     4445 2021-08-17 12:06:22.483859 pfhedge-0.9.0/pfhedge/nn/modules/mlp.py
+-rw-r--r--   0        0        0     1102 2021-08-17 12:06:22.484343 pfhedge-0.9.0/pfhedge/nn/modules/naked.py
+-rw-r--r--   0        0        0     4058 2021-08-17 12:06:22.485038 pfhedge-0.9.0/pfhedge/nn/modules/ww.py
+-rw-r--r--   0        0        0      156 2021-07-16 00:45:39.131765 pfhedge-0.9.0/pfhedge/stochastic/__init__.py
+-rw-r--r--   0        0        0     5697 2021-08-17 12:06:22.485675 pfhedge-0.9.0/pfhedge/stochastic/brownian.py
+-rw-r--r--   0        0        0     4663 2021-08-17 12:06:22.486507 pfhedge-0.9.0/pfhedge/stochastic/cir.py
+-rw-r--r--   0        0        0     4453 2021-08-17 12:06:22.487262 pfhedge-0.9.0/pfhedge/stochastic/heston.py
+-rw-r--r--   0        0        0      618 2021-08-17 12:06:22.487981 pfhedge-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      896 2021-08-17 12:06:57.791658 pfhedge-0.9.0/setup.py
+-rw-r--r--   0        0        0      636 2021-08-17 12:06:57.791883 pfhedge-0.9.0/PKG-INFO
```

### Comparing `pfhedge-0.8.1/LICENSE` & `pfhedge-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfhedge-0.8.1/pfhedge/_utils/bisect.py` & `pfhedge-0.9.0/pfhedge/_utils/bisect.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         max_iter (int, default 100000): If the number of iterations exceeds this
             value, abort computation and raise RuntimeError.
 
     Returns:
         torch.Tensor
 
     Raises:
-        RuntimeError: If the number of iteration exceeds `max_iter`.
+        RuntimeError: If the number of iteration exceeds ``max_iter``.
 
     Examples:
 
         >>> target = torch.tensor([-1.0, 0.0, 1.0])
         >>> function = torch.log
         >>> output = bisect(function, target, 0.01, 10.0)
         >>> output
@@ -58,15 +58,15 @@
     """
     lower, upper = map(torch.as_tensor, (lower, upper))
 
     if not (lower < upper).all():
         raise ValueError("condition lower < upper should be satisfied.")
 
     if (function(lower) > function(upper)).all():
-        # If `function` is a decreasing function
+        # If function is a decreasing function
         mf = lambda input: -function(input)
         return bisect(mf, -target, lower, upper, precision=precision, max_iter=max_iter)
 
     n_iter = 0
     while torch.max(upper - lower) > precision:
         n_iter += 1
         if n_iter > max_iter:
```

### Comparing `pfhedge-0.8.1/pfhedge/_utils/hook.py` & `pfhedge-0.9.0/pfhedge/_utils/hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from torch import Tensor
 from torch.nn import Module
 
 
 def save_prev_output(
     module: Module, input: Optional[Tensor], output: Optional[Tensor]
 ) -> None:
-    """A hook to save previous output as a buffer named `prev_output`.
+    """A hook to save previous output as a buffer named ``prev_output``.
 
     Examples:
 
         >>> import torch
         >>> _ = torch.manual_seed(42)
         >>> m = torch.nn.Linear(3, 2)
         >>> hook = m.register_forward_hook(save_prev_output)
```

### Comparing `pfhedge-0.8.1/pfhedge/_utils/operations.py` & `pfhedge-0.9.0/pfhedge/_utils/operations.py`

 * *Files identical despite different names*

### Comparing `pfhedge-0.8.1/pfhedge/_utils/parse.py` & `pfhedge-0.9.0/pfhedge/_utils/parse.py`

 * *Files identical despite different names*

### Comparing `pfhedge-0.8.1/pfhedge/autogreek.py` & `pfhedge-0.9.0/pfhedge/autogreek.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     """Computes and returns delta of a derivative using automatic differentiation.
 
     Delta is a differentiation of a derivative price with respect to
     a price of underlying instrument.
 
     Args:
         pricer (callable): Pricing formula of a derivative.
-        create_graph (bool, default=False): If `True`, graph of the derivative will be
-            constructed, allowing to compute higher order derivative products.
-        **kwargs: Parameters passed to `pricer`.
+        create_graph (bool, default=False): If ``True``, graph of the derivative
+            will be constructed, allowing to compute higher order derivative
+            products.
+        **kwargs: Parameters passed to ``pricer``.
 
     Returns:
         torch.Tensor
 
     Examples:
 
         Delta of a European option can be evaluated as follows.
@@ -54,38 +55,38 @@
         >>> from pfhedge.instruments import BrownianStock
         >>> from pfhedge.instruments import EuropeanOption
         >>> from pfhedge.nn import WhalleyWilmott
         >>> from pfhedge.nn import Hedger
         >>>
         >>> _ = torch.manual_seed(42)
         >>>
-        >>> derivative = EuropeanOption(BrownianStock(cost=1e-4))
+        >>> derivative = EuropeanOption(BrownianStock(cost=1e-4)).to(torch.float64)
         >>> model = WhalleyWilmott(derivative)
-        >>> hedger = Hedger(model, model.inputs())
+        >>> hedger = Hedger(model, model.inputs()).to(torch.float64)
         >>>
         >>> def pricer(spot):
         ...     return hedger.price(
         ...         derivative, init_state=(spot,), enable_grad=True
         ...     )
         >>>
         >>> autogreek.delta(pricer, spot=torch.tensor(1.0))
-        tensor(0.52...)
+        tensor(0.5...)
     """
     if kwargs.get("strike") is None and kwargs.get("spot") is None:
         # Since delta does not depend on strike,
         # assign an arbitrary value (1.0) to strike if not given.
         kwargs["strike"] = torch.tensor(1.0)
 
     spot = parse_spot(**kwargs).requires_grad_()
     kwargs["spot"] = spot
     if "strike" in kwargs:
         kwargs["moneyness"] = spot / kwargs["strike"]
         kwargs["log_moneyness"] = (spot / kwargs["strike"]).log()
 
-    # Delete parameters that are not in the signature of `pricer` to avoid
+    # Delete parameters that are not in the signature of pricer to avoid
     # TypeError: <pricer> got an unexpected keyword argument '<parameter>'
     for parameter in list(kwargs.keys()):
         if parameter not in signature(pricer).parameters.keys():
             del kwargs[parameter]
 
     assert spot.requires_grad
     price = pricer(**kwargs)
@@ -103,17 +104,17 @@
     """Computes and returns gamma of a derivative.
 
     Delta is a second-order differentiation of a derivative price with respect to
     a price of underlying instrument.
 
     Args:
         pricer (callable): Pricing formula of a derivative.
-        create_graph (bool, default=False): If `True`, graph of the derivative will be
+        create_graph (bool, default=False): If ``True``, graph of the derivative will be
             constructed, allowing to compute higher order derivative products.
-        **kwargs: Parameters passed to `pricer`.
+        **kwargs: Parameters passed to ``pricer``.
 
     Returns:
         torch.Tensor
 
     Examples:
 
         Gamma of a European option can be evaluated as follows.
```

### Comparing `pfhedge-0.8.1/pfhedge/features/_base.py` & `pfhedge-0.9.0/pfhedge/features/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             i (int): The index of the time step to get the feature.
 
         Returns:
             torch.Tensor
         """
 
     def of(self: T, derivative=None, hedger=None) -> T:
-        """Set `derivative` and `hedger` to the attributes of `self`.
+        """Set ``derivative`` and ``hedger`` to the attributes of ``self``.
 
         Args:
             derivative (Derivative, optional): The derivative to compute features.
             hedger (Hedger, optional): The hedger to compute features.
 
         Returns:
             self
```

### Comparing `pfhedge-0.8.1/pfhedge/features/_getter.py` & `pfhedge-0.9.0/pfhedge/features/_getter.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,9 +41,8 @@
             raise ValueError(
                 f"{feature} is not a valid value. "
                 "Use sorted(pfhedge.features.FEATURES) to get valid options."
             )
         feature = dict_features[feature]
     elif not isinstance(feature, Feature):
         raise TypeError(f"{feature} is not an instance of Feature.")
-    # If `feature` is Feature object, pass it through.
     return feature
```

### Comparing `pfhedge-0.8.1/pfhedge/features/features.py` & `pfhedge-0.9.0/pfhedge/features/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 from .functional import zeros
 
 
 class Moneyness(Feature):
     """Moneyness of the underlying instrument of the derivative.
 
     Args:
-        log (bool, default=False): If `True`, represents log moneyness.
+        log (bool, default=False): If ``True``, represents log moneyness.
     """
 
     def __init__(self, log: bool = False) -> None:
         super().__init__()
         self.log = log
 
     def __str__(self) -> str:
         return "log_moneyness" if self.log else "moneyness"
 
     def __getitem__(self, i: int) -> Tensor:
         if self.log:
-            return self.derivative.log_moneyness(i).unsqueeze(-1)
+            return self.derivative.log_moneyness(i)
         else:
-            return self.derivative.moneyness(i).unsqueeze(-1)
+            return self.derivative.moneyness(i)
 
 
 class LogMoneyness(Moneyness):
     """Log moneyness of the underlying instrument of the derivative."""
 
     def __init__(self) -> None:
         super().__init__(log=True)
@@ -45,15 +45,15 @@
 class ExpiryTime(Feature):
     """Remaining time to the maturity of the derivative."""
 
     def __str__(self) -> str:
         return "expiry_time"
 
     def __getitem__(self, i: int) -> Tensor:
-        return self.derivative.time_to_maturity(i).unsqueeze(-1)
+        return self.derivative.time_to_maturity(i)
 
 
 class Volatility(Feature):
     """Volatility of the underlier of the derivative."""
 
     def __str__(self) -> str:
         return "volatility"
@@ -70,22 +70,22 @@
 
     def __getitem__(self, i: int) -> Tensor:
         return prev_hedge(i, derivative=self.derivative, hedger=self.hedger)
 
 
 class Barrier(Feature):
     """A feature which signifies whether the price of the underlier have reached
-    the barrier. The output `1.0` means that the price have touched the barrier,
-    and `0` otherwise.
+    the barrier. The output 1.0 means that the price have touched the barrier,
+    and 0.0 otherwise.
 
     Args:
         threshold (float): The price level of the barrier.
-        up (bool, default True): If `True`, signifies whether the price has exceeded
+        up (bool, default True): If ``True``, signifies whether the price has exceeded
             the barrier upward.
-            If `False`, signifies whether the price has exceeded the barrier downward.
+            If ``False``, signifies whether the price has exceeded the barrier downward.
     """
 
     def __init__(self, threshold: float, up: bool = True) -> None:
         super().__init__()
         self.threshold = threshold
         self.up = up
 
@@ -118,15 +118,15 @@
         return empty(i, derivative=self.derivative)
 
 
 class MaxMoneyness(Feature):
     """Cumulative maximum of moneyness.
 
     Args:
-        log (bool, default=False): If `True`, represents log moneyness.
+        log (bool, default=False): If ``True``, represents log moneyness.
     """
 
     def __init__(self, log: bool = False) -> None:
         super().__init__()
         self.log = log
 
     def __str__(self) -> str:
@@ -143,23 +143,24 @@
     """Cumulative maximum of log Moneyness."""
 
     def __init__(self) -> None:
         super().__init__(log=True)
 
 
 class ModuleOutput(Feature, Module):
-    """The feature computed as an output of a `torch.nn.Module`.
+    """The feature computed as an output of a ``torch.nn.Module``.
 
     Args:
         module (torch.nn.Module): Module to compute the value of the feature.
-            The input and output shapes should be `(N, *, H_in) -> (N, *, 1)`,
-            where `N` stands for the number of Monte Carlo paths of the underlier of
-            the derivative, `H_in` stands for the number of input features
-            (namely, `H_in = len(inputs)`),
-            and `*` means any number of additional dimensions.
+            The input and output shapes should be :math:`(N, *, H_in) -> (N, *, 1)`,
+            where :math:`N` stands for the number of Monte Carlo paths of
+            the underlier of the derivative,
+            :math:`H_in` stands for the number of input features
+            (namely, ``len(inputs)``),
+            and :math:`*` means any number of additional dimensions.
         inputs (list[Feature]): The input features to the module.
 
     Examples:
 
         >>> from torch.nn import Linear
         >>> from pfhedge.instruments import BrownianStock
         >>> from pfhedge.instruments import EuropeanOption
```

### Comparing `pfhedge-0.8.1/pfhedge/features/functional.py` & `pfhedge-0.9.0/pfhedge/features/functional.py`

 * *Files identical despite different names*

### Comparing `pfhedge-0.8.1/pfhedge/instruments/base.py` & `pfhedge-0.9.0/pfhedge/instruments/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         """
 
     @abstractmethod
     def to(self: T, *args, **kwargs) -> T:
         """Performs dtype and/or device conversion of the buffers associated to
         the instument.
 
-        A `torch.dtype` and `torch.device` are inferred from the arguments of
-        `self.to(*args, **kwargs)`.
+        A ``torch.dtype`` and ``torch.device`` are inferred from the arguments of
+        ``self.to(*args, **kwargs)``.
 
         Args:
             dtype (torch.dtype): Desired floating point type of the floating point
                 values of simulated time series.
             device (torch.device): Desired device of the values of simulated time
                 series.
 
@@ -65,51 +65,51 @@
                 Defaults to the current CUDA device.
         """
         return self.to(
             torch.device("cuda:{}".format(device) if device is not None else "cuda")
         )
 
     def double(self: T) -> T:
-        """`self.double()` is equivalent to `self.to(torch.float64)`.
+        """It is equivalent to ``self.to(torch.float64)``.
         See :func:`to()`.
         """
         return self.to(torch.float64)
 
     def float(self: T) -> T:
-        """`self.float()` is equivalent to `self.to(torch.float32)`.
+        """It is equivalent to ``self.to(torch.float32)``.
         See :func:`to()`.
         """
         return self.to(torch.float32)
 
     def half(self: T) -> T:
-        """`self.half()` is equivalent to `self.to(torch.float16)`.
+        """It is equivalent to ``self.to(torch.float16)``.
         See :func:`to()`.
         """
         return self.to(torch.float16)
 
     def bfloat16(self: T) -> T:
-        """`self.bfloat16()` is equivalent to `self.to(torch.bfloat16)`.
+        """It is equivalent to ``self.to(torch.bfloat16)``.
         See :func:`to()`.
         """
         return self.to(torch.bfloat16)
 
     @property
     def dinfo(self) -> List[str]:
-        """Returns list of strings that tell `dtype` and `device` of `self`.
+        """Returns list of strings that tell ``dtype`` and ``device`` of self.
 
-        Intended to be used in `__repr__`.
+        Intended to be used in :func:`__repr__`.
 
-        If `dtype` (`device`) is the one specified in default type,
-        `dinfo` will not have the information of it.
+        If ``dtype`` (``device``) is the one specified in default type,
+        ``dinfo`` will not have the information of it.
 
         Returns:
             list[str]
         """
-        # Implementation here refers to the function `_str_intern` in
-        # `pytorch/_tensor_str.py`.
+        # Implementation here refers to the function _str_intern in
+        # pytorch/_tensor_str.py.
 
         dinfo = []
 
         dtype = getattr(self, "dtype", None)
         if dtype is not None:
             if dtype != torch.get_default_dtype():
                 dinfo.append("dtype=" + str(dtype))
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/derivative/american_binary.py` & `pfhedge-0.9.0/pfhedge/instruments/derivative/american_binary.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,19 @@
     Args:
         underlier (:class:`Primary`): The underlying instrument of the option.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
         maturity (float, default=20/250): The maturity of the option.
         dtype (torch.device, optional): Desired device of returned tensor.
             Default: If None, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): Desired device of returned tensor.
             Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and
             the current CUDA device for CUDA tensor types.
 
     Attributes:
         dtype (torch.dtype): The dtype with which the simulated time-series are
             represented.
         device (torch.device): The device where the simulated time-series are.
 
@@ -74,16 +74,16 @@
         >>> from pfhedge.instruments import AmericanBinaryOption
         >>>
         >>> _ = torch.manual_seed(42)
         >>> derivative = AmericanBinaryOption(BrownianStock(), \
 maturity=5/250, strike=1.01)
         >>> derivative.simulate(n_paths=2)
         >>> derivative.underlier.spot
-        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930],
-                [1.0000, 1.0282, 1.0199, 1.0258, 1.0292]])
+        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930, 0.9906],
+                [1.0000, 0.9919, 0.9976, 1.0009, 1.0076, 1.0179]])
         >>> derivative.payoff()
         tensor([0., 1.])
     """
 
     def __init__(
         self,
         underlier: Primary,
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/derivative/base.py` & `pfhedge-0.9.0/pfhedge/instruments/derivative/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     ) -> None:
         """Simulate time series associated with the underlier.
 
         Args:
             n_paths (int): The number of paths to simulate.
             init_state (tuple[torch.Tensor | float], optional): The initial state of
                 the underlier.
-            **kwargs: Other parameters passed to `self.underlier.simulate()`.
+            **kwargs: Other parameters passed to ``self.underlier.simulate()``.
         """
         self.underlier.simulate(
             n_paths=n_paths, time_horizon=self.maturity, init_state=init_state
         )
 
     def ul(self) -> Primary:
         """Alias for ``self.underlier``."""
@@ -92,74 +92,71 @@
     maturity: float
 
     def moneyness(self, time_step: Optional[int] = None) -> Tensor:
         """Returns the moneyness of self.
 
         Args:
             time_step (int, optional): The time step to calculate
-                the moneyness. If `None` (default), the moneyness is calculated
+                the moneyness. If ``None`` (default), the moneyness is calculated
                 at all time steps.
 
         Shape:
             - Output: :math:`(N, T)` where :math:`N` is the number of paths and
               :math:`T` is the number of time steps.
-              If `time_step` is given, the shape is :math:`(N, 1)`.
+              If ``time_step`` is given, the shape is :math:`(N, 1)`.
 
         Returns:
             torch.Tensor
         """
-        spot = self.underlier.spot
-        if time_step is not None:
-            spot = spot[..., time_step]
-        return spot / self.strike
+        index = ... if time_step is None else [time_step]
+        return self.underlier.spot[..., index] / self.strike
 
     def log_moneyness(self, time_step: Optional[int] = None) -> Tensor:
         """Returns the log moneyness of self.
 
         Args:
             time_step (int, optional): The time step to calculate the log
-                moneyness. If `None` (default), the moneyness is calculated
+                moneyness. If ``None`` (default), the moneyness is calculated
                 at all time steps.
 
         Shape:
             - Output: :math:`(N, T)` where :math:`N` is the number of paths and
               :math:`T` is the number of time steps.
-              If `time_step` is given, the shape is :math:`(N, 1)`.
+              If ``time_step`` is given, the shape is :math:`(N, 1)`.
 
         Returns:
             torch.Tensor
         """
         return self.moneyness(time_step=time_step).log()
 
     def time_to_maturity(self, time_step: Optional[int] = None) -> Tensor:
         """Returns the time to maturity of self.
 
         Args:
             time_step (int, optional): The time step to calculate
-                the time to maturity. If `None` (default), the time to
+                the time to maturity. If ``None`` (default), the time to
                 maturity is calculated at all time steps.
 
         Shape:
             - Output: :math:`(N, T)` where :math:`N` is the number of paths and
               :math:`T` is the number of time steps.
-              If `time_step` is given, the shape is :math:`(N, 1)`.
+              If ``time_step`` is given, the shape is :math:`(N, 1)`.
 
         Returns:
             torch.Tensor
         """
         n_paths, n_steps = self.underlier.spot.size()
         if time_step is None:
-            t = self.underlier.dt * torch.arange(n_steps).repeat(n_paths, 1)
-            t.to(self.underlier.device)
-            return self.maturity - t
+            # Time passed from the beginning
+            t = torch.arange(n_steps).to(self.underlier.spot) * self.underlier.dt
+            return (t[-1] - t).unsqueeze(0).expand(n_paths, -1)
         else:
-            t = torch.full_like(
-                self.underlier.spot[:, 0], time_step * self.underlier.dt
-            )
-            return self.maturity - t
+            time = n_steps - (time_step % n_steps) - 1
+            t = torch.tensor([[time]]).to(self.underlier.spot) * self.underlier.dt
+            return t.expand(n_paths, -1)
 
 
 # Assign docstrings so they appear in Sphinx documentation
 set_docstring(Derivative, "to", Instrument.to)
 set_attr_and_docstring(Derivative, "cpu", Instrument.cpu)
 set_attr_and_docstring(Derivative, "cuda", Instrument.cuda)
 set_attr_and_docstring(Derivative, "double", Instrument.double)
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/derivative/european.py` & `pfhedge-0.9.0/pfhedge/instruments/derivative/european.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     Args:
         underlier (:class:`Primary`): The underlying instrument of the option.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
         maturity (float, default=20/250): The maturity of the option.
         dtype (torch.dtype, optional): Desired device of returned tensor.
             Default: If None, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): Desired device of returned tensor.
             Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and
             the current CUDA device for CUDA tensor types.
 
     Attributes:
         dtype (torch.dtype): The dtype with which the simulated time-series are
             represented.
         device (torch.device): The device where the simulated time-series are.
 
@@ -59,20 +59,20 @@
         >>> from pfhedge.instruments import BrownianStock
         >>> from pfhedge.instruments import EuropeanOption
         >>>
         >>> _ = torch.manual_seed(42)
         >>> derivative = EuropeanOption(BrownianStock(), maturity=5/250)
         >>> derivative.simulate(n_paths=2)
         >>> derivative.underlier.spot
-        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930],
-                [1.0000, 1.0282, 1.0199, 1.0258, 1.0292]])
+        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930, 0.9906],
+                [1.0000, 0.9919, 0.9976, 1.0009, 1.0076, 1.0179]])
         >>> derivative.payoff()
-        tensor([0.0000, 0.0292])
+        tensor([0.0000, 0.0179])
 
-        Using custom `dtype` and `device`.
+        Using custom ``dtype`` and ``device``.
 
         >>> derivative = EuropeanOption(BrownianStock())
         >>> derivative.to(dtype=torch.float64, device="cuda:0")
         EuropeanOption(..., dtype=torch.float64, device='cuda:0')
     """
 
     def __init__(
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/derivative/european_binary.py` & `pfhedge-0.9.0/pfhedge/instruments/derivative/european_binary.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,19 +47,19 @@
     Args:
         underlier (:class:`Primary`): The underlying instrument of the option.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1): The strike price of the option.
         maturity (float, default=20/250) The maturity of the option.
         dtype (torch.dtype, optional): Desired device of returned tensor.
             Default: If None, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): Desired device of returned tensor.
             Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and
             the current CUDA device for CUDA tensor types.
 
     Attributes:
         dtype (torch.dtype): The dtype with which the simulated time-series are
             represented.
         device (torch.device): The device where the simulated time-series are.
 
@@ -69,16 +69,16 @@
         >>> from pfhedge.instruments import BrownianStock
         >>> from pfhedge.instruments import EuropeanBinaryOption
         >>>
         >>> _ = torch.manual_seed(42)
         >>> derivative = EuropeanBinaryOption(BrownianStock(), maturity=5/250)
         >>> derivative.simulate(n_paths=2)
         >>> derivative.underlier.spot
-        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930],
-                [1.0000, 1.0282, 1.0199, 1.0258, 1.0292]])
+        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930, 0.9906],
+                [1.0000, 0.9919, 0.9976, 1.0009, 1.0076, 1.0179]])
         >>> derivative.payoff()
         tensor([0., 1.])
     """
 
     def __init__(
         self,
         underlier: Primary,
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/derivative/lookback.py` & `pfhedge-0.9.0/pfhedge/instruments/derivative/lookback.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     Args:
         underlier (:class:`Primary`): The underlying instrument of the option.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
         maturity (float, default=20/250): The maturity of the option.
         dtype (torch.dtype, optional): Desired device of returned tensor.
             Default: If None, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): Desired device of returned tensor.
             Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and
             the current CUDA device for CUDA tensor types.
 
     Attributes:
         dtype (torch.dtype): The dtype with which the simulated time-series are
             represented.
         device (torch.device): The device where the simulated time-series are.
 
@@ -63,18 +63,18 @@
         >>> from pfhedge.instruments import BrownianStock
         >>> from pfhedge.instruments import LookbackOption
         >>>
         >>> _ = torch.manual_seed(42)
         >>> derivative = LookbackOption(BrownianStock(), maturity=5/250)
         >>> derivative.simulate(n_paths=2)
         >>> derivative.underlier.spot
-        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930],
-                [1.0000, 1.0282, 1.0199, 1.0258, 1.0292]])
+        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930, 0.9906],
+                [1.0000, 0.9919, 0.9976, 1.0009, 1.0076, 1.0179]])
         >>> derivative.payoff()
-        tensor([0.0073, 0.0292])
+        tensor([0.0073, 0.0179])
     """
 
     def __init__(
         self,
         underlier: Primary,
         call: bool = True,
         strike: float = 1.0,
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/primary/base.py` & `pfhedge-0.9.0/pfhedge/instruments/primary/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,20 +58,24 @@
         self,
         n_paths: int,
         time_horizon: float,
         init_state: Optional[Tuple[TensorOrFloat, ...]] = None,
     ) -> None:
         """Simulate time series associated with the instrument and add them as buffers.
 
+        The shapes of the registered buffers should be ``(n_paths, n_steps)``
+        where ``n_steps`` is the minimum integer that satisfies
+        ``n_steps * self.dt >= time_horizon``.
+
         Args:
             n_paths (int): The number of paths to simulate.
             time_horizon (float): The period of time to simulate the price.
             init_state (tuple[torch.Tensor | float], optional): The initial state of
                 the instrument.
-                If `None` (default), it uses the default value
+                If ``None`` (default), it uses the default value
                 (See :func:`default_init_state`).
         """
 
     def register_buffer(self, name: str, tensor: Tensor) -> None:
         """Adds a buffer to the module.
 
         Buffers can be accessed as attributes using given names.
@@ -80,15 +84,15 @@
             name (string): name of the buffer. The buffer can be accessed
                 from this module using the given name
             tensor (Tensor or None): buffer to be registered. If ``None``, then
                 operations that run on buffers, such as :attr:`cuda`, are ignored.
                 If ``None``, the buffer is **not** included in the module's
                 :attr:`state_dict`.
         """
-        # Implementation here refers to `torch.nn.Module.register_buffer`.
+        # Implementation here refers to torch.nn.Module.register_buffer.
         if "_buffers" not in self.__dict__:
             raise AttributeError("cannot assign buffer before Primary.__init__() call")
         elif not isinstance(name, torch._six.string_classes):
             raise TypeError(
                 "buffer name should be a string. " "Got {}".format(torch.typename(name))
             )
         elif "." in name:
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/primary/brownian.py` & `pfhedge-0.9.0/pfhedge/instruments/primary/brownian.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from math import ceil
 from typing import Optional
 from typing import Tuple
 from typing import Union
 from typing import cast
 
 import torch
 from torch import Tensor
@@ -25,19 +26,19 @@
 
     Args:
         volatility (float, default=0.2): The volatility of the price.
         cost (float, default=0.0): The transaction cost rate.
         dt (float, default=1/250): The intervals of the time steps.
         dtype (torch.device, optional): Desired device of returned tensor.
             Default: If None, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): Desired device of returned tensor.
             Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and
             the current CUDA device for CUDA tensor types.
 
     Buffers:
         - ``spot`` (``torch.Tensor``): The spot prices of the instrument.
           This attribute is set by a method :func:`simulate()`.
           The shape is :math:`(N, T)` where
           :math:`N` is the number of simulated paths and
@@ -47,18 +48,18 @@
 
         >>> from pfhedge.instruments import BrownianStock
         >>>
         >>> _ = torch.manual_seed(42)
         >>> stock = BrownianStock()
         >>> stock.simulate(n_paths=2, time_horizon=5 / 250)
         >>> stock.spot
-        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930],
-                [1.0000, 1.0282, 1.0199, 1.0258, 1.0292]])
+        tensor([[1.0000, 1.0016, 1.0044, 1.0073, 0.9930, 0.9906],
+                [1.0000, 0.9919, 0.9976, 1.0009, 1.0076, 1.0179]])
 
-        Using custom `dtype` and `device`.
+        Using custom ``dtype`` and ``device``.
 
         >>> stock = BrownianStock()
         >>> stock.to(dtype=torch.float64, device="cuda:0")
         BrownianStock(..., dtype=torch.float64, device='cuda:0')
     """
 
     def __init__(
@@ -83,47 +84,47 @@
 
     def simulate(
         self,
         n_paths: int = 1,
         time_horizon: float = 20 / 250,
         init_state: Optional[Tuple[TensorOrFloat]] = None,
     ) -> None:
-        """Simulate the spot price and add it as a buffer named `spot`.
+        """Simulate the spot price and add it as a buffer named ``spot``.
 
         The shape of the spot is :math:`(N, T)`, where :math:`N` is the number of
         simulated paths and :math:`T` is the number of time steps.
-        The number of time steps is determinded from `dt` and `time_horizon`.
+        The number of time steps is determinded from ``dt`` and ``time_horizon``.
 
         Args:
             n_paths (int, default=1): The number of paths to simulate.
             time_horizon (float, default=20/250): The period of time to simulate
                 the price.
             init_state (tuple[torch.Tensor | float], optional): The initial state of
                 the instrument.
-                This is specified by `(spot,)`, where `spot` is the initial value
+                This is specified by ``(spot,)``, where ``spot`` is the initial value
                 of the stock price.
-                If `None` (default), it uses the default value
+                If ``None`` (default), it uses the default value
                 (See :func:`default_init_state`).
-                It also accepts a float or a `torch.Tensor`.
+                It also accepts a ``float`` or a ``torch.Tensor``.
 
         Examples:
 
             >>> _ = torch.manual_seed(42)
             >>> stock = BrownianStock()
             >>> stock.simulate(n_paths=2, time_horizon=5 / 250, init_state=(2.0,))
             >>> stock.spot
-            tensor([[2.0000, 2.0031, 2.0089, 2.0146, 1.9860],
-                    [2.0000, 2.0565, 2.0398, 2.0516, 2.0584]])
+            tensor([[2.0000, 2.0031, 2.0089, 2.0146, 1.9860, 1.9812],
+                    [2.0000, 1.9838, 1.9952, 2.0018, 2.0153, 2.0358]])
         """
         if init_state is None:
             init_state = cast(Tuple[float], self.default_init_state)
 
         spot = generate_geometric_brownian(
             n_paths=n_paths,
-            n_steps=int(time_horizon / self.dt),
+            n_steps=ceil(time_horizon / self.dt + 1),
             init_state=init_state,
             volatility=self.volatility,
             dt=self.dt,
             dtype=self.dtype,
             device=self.device,
         )
```

### Comparing `pfhedge-0.8.1/pfhedge/instruments/primary/heston.py` & `pfhedge-0.9.0/pfhedge/instruments/primary/heston.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,49 +24,48 @@
         theta (float, default=0.04): The parameter :math:`\\theta`.
         sigma (float, default=2.0): The parameter :math:`\\sigma`.
         rho (float, default=-0.7): The parameter :math:`\\rho`.
         cost (float, default=0.0): The transaction cost rate.
         dt (float, default=1/250): The intervals of the time steps.
         dtype (torch.device, optional): Desired device of returned tensor.
             Default: If None, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): Desired device of returned tensor.
             Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and
             the current CUDA device for CUDA tensor types.
 
     Buffers:
         - ``spot`` (``torch.Tensor``): The spot price of the instrument.
           This attribute is set by a method :func:`simulate()`.
           The shape is :math:`(N, T)` where
           :math:`N` is the number of simulated paths and
           :math:`T` is the number of time steps.
         - ``variance`` (``torch.Tensor``): The variance of the instrument.
           Note that this is different from the realized variance of the spot price.
           This attribute is set by a method :func:`simulate()`.
           The shape is :math:`(N, T)`.
-        - ``volatility`` (``torch.Tensor``): An alias for ``self.variance.sqrt()``.
 
     Examples:
 
         >>> from pfhedge.instruments import HestonStock
         >>>
         >>> _ = torch.manual_seed(42)
         >>> stock = HestonStock()
         >>> stock.simulate(n_paths=2, time_horizon=5/250)
         >>> stock.spot
-        tensor([[1.0000, 0.9941, 0.9905, 0.9846, 0.9706],
-                [1.0000, 1.0031, 0.9800, 0.9785, 0.9735]])
+        tensor([[1.0000, 0.9902, 0.9823, 0.9926, 0.9968, 1.0040],
+                [1.0000, 0.9826, 0.9891, 0.9898, 0.9851, 0.9796]])
         >>> stock.variance
-        tensor([[0.0400, 0.0408, 0.0411, 0.0417, 0.0422],
-                [0.0400, 0.0395, 0.0452, 0.0434, 0.0446]])
+        tensor([[0.0400, 0.0408, 0.0411, 0.0417, 0.0422, 0.0393],
+                [0.0400, 0.0457, 0.0440, 0.0451, 0.0458, 0.0472]])
         >>> stock.volatility
-        tensor([[0.2000, 0.2020, 0.2027, 0.2041, 0.2054],
-                [0.2000, 0.1987, 0.2126, 0.2084, 0.2112]])
+        tensor([[0.2000, 0.2020, 0.2027, 0.2041, 0.2054, 0.1982],
+                [0.2000, 0.2138, 0.2097, 0.2124, 0.2140, 0.2172]])
     """
 
     spot: Tensor
     variance: Tensor
 
     def __init__(
         self,
@@ -92,45 +91,46 @@
 
     @property
     def default_init_state(self) -> Tuple[float, ...]:
         return (1.0, self.theta)
 
     @property
     def volatility(self) -> Tensor:
+        """An alias for ``self.variance.sqrt()``."""
         return self.variance.clamp(min=0.0).sqrt()
 
     def simulate(
         self,
         n_paths: int = 1,
         time_horizon: float = 20 / 250,
         init_state: Optional[Tuple[TensorOrFloat, ...]] = None,
     ) -> None:
-        """Simulate the spot price and add it as a buffer named `spot`.
+        """Simulate the spot price and add it as a buffer named ``spot``.
 
         The shape of the spot is :math:`(N, T)`, where :math:`N` is the number of
         simulated paths and :math:`T` is the number of time steps.
-        The number of time steps is determinded from `dt` and `time_horizon`.
+        The number of time steps is determinded from ``dt`` and ``time_horizon``.
 
         Args:
             n_paths (int, default=1): The number of paths to simulate.
             time_horizon (float, default=20/250): The period of time to simulate
                 the price.
             init_state (tuple[torch.Tensor | float], default=(1.0,)): The initial
                 state of the instrument.
-                This is specified by `(S0, V0)`, where `S0` and `V0` are the initial
-                values of of spot and variance, respectively.
-                If `None` (default), it uses the default value
+                This is specified by ``(S0, V0)``, where ``S0`` and ``V0`` are
+                the initial values of of spot and variance, respectively.
+                If ``None`` (default), it uses the default value
                 (See :func:`default_init_state`).
         """
         if init_state is None:
             init_state = self.default_init_state
 
         spot, variance = generate_heston(
             n_paths=n_paths,
-            n_steps=int(time_horizon / self.dt),
+            n_steps=int(time_horizon / self.dt + 1),
             init_state=init_state,
             kappa=self.kappa,
             theta=self.theta,
             sigma=self.sigma,
             rho=self.rho,
             dt=self.dt,
             dtype=self.dtype,
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/__init__.py` & `pfhedge-0.9.0/pfhedge/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pfhedge-0.8.1/pfhedge/nn/functional.py` & `pfhedge-0.9.0/pfhedge/nn/functional.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from math import ceil
 from typing import Optional
+from typing import Union
 
 import torch
 import torch.nn.functional as fn
 from torch import Tensor
 
 
 def european_payoff(input: Tensor, call: bool = True, strike: float = 1.0) -> Tensor:
@@ -11,15 +12,15 @@
 
     Args:
         input (torch.Tensor): The input tensor representing the price trajectory.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
-        - input: :math:`(*, T)`, where, :math:`T` stands for the number of time steps
+        - input: :math:`(*, T)` where :math:`T` stands for the number of time steps
           and :math:`*` means any number of additional dimensions.
         - output: :math:`(*)`
 
     Returns:
         torch.Tensor
     """
     if call:
@@ -33,15 +34,15 @@
 
     Args:
         input (torch.Tensor): The input tensor representing the price trajectory.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
-        - input: :math:`(*, T)`, where, :math:`T` stands for the number of time steps
+        - input: :math:`(*, T)` where :math:`T` stands for the number of time steps
           and :math:`*` means any number of additional dimensions.
         - output: :math:`(*)`
 
     Returns:
         torch.Tensor
     """
     if call:
@@ -57,15 +58,15 @@
 
     Args:
         input (torch.Tensor): The input tensor representing the price trajectory.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
-        - input: :math:`(*, T)`, where, :math:`T` stands for the number of time steps
+        - input: :math:`(*, T)` where :math:`T` stands for the number of time steps
           and :math:`*` means any number of additional dimensions.
         - output: :math:`(*)`
 
     Returns:
         torch.Tensor
     """
     if call:
@@ -81,15 +82,15 @@
 
     Args:
         input (torch.Tensor): The input tensor representing the price trajectory.
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
-        - input: :math:`(*, T)`, where, :math:`T` stands for the number of time steps
+        - input: :math:`(*, T)` where :math:`T` stands for the number of time steps
           and :math:`*` means any number of additional dimensions.
         - output: :math:`(*)`
 
     Returns:
         torch.Tensor
     """
     if call:
@@ -141,23 +142,23 @@
     if a == 1.0:
         return input.log()
     else:
         return input ** (1.0 - a)
 
 
 def topp(input: Tensor, p: float, dim: Optional[int] = None, largest: bool = True):
-    """Returns the largest `p * N` elements of the given input tensor,
-    where `N` stands for the total number of elements in the input tensor.
+    """Returns the largest :math:`p * N` elements of the given input tensor,
+    where :math:`N` stands for the total number of elements in the input tensor.
 
-    If `dim` is not given, the last dimension of the `input` is chosen.
+    If ``dim`` is not given, the last dimension of the ``input`` is chosen.
 
-    If `largest` is `False` then the smallest elements are returned.
+    If ``largest`` is ``False`` then the smallest elements are returned.
 
-    A namedtuple of `(values, indices)` is returned, where the `indices` are the indices
-    of the elements in the original `input` tensor.
+    A namedtuple of ``(values, indices)`` is returned, where the ``indices``
+    are the indices of the elements in the original ``input`` tensor.
 
     Args:
         input (torch.Tensor): The input tensor.
         p (float): Quantile level.
         dim (int, optional): The dimension to sort along.
         largest (bool, default=True): Controls whether to return largest or smallest
             elements.
@@ -210,15 +211,15 @@
 
 def leaky_clamp(
     input: Tensor,
     min: Optional[Tensor] = None,
     max: Optional[Tensor] = None,
     clamped_slope: float = 0.01,
 ) -> Tensor:
-    """Leakily clamp all elements in `input` into the range :math:`[\\min, \\max]`.
+    """Leakily clamp all elements in ``input`` into the range :math:`[\\min, \\max]`.
 
     The bounds :math:`\\min` and :math:`\\max` can be tensors.
 
     See :class:`pfhedge.nn.LeakyClamp` for details.
     """
     x = input
 
@@ -235,14 +236,64 @@
 
     return x
 
 
 def clamp(
     input: Tensor, min: Optional[Tensor] = None, max: Optional[Tensor] = None
 ) -> Tensor:
-    """Clamp all elements in `input` into the range :math:`[\\min, \\max]`.
+    """Clamp all elements in ``input`` into the range :math:`[\\min, \\max]`.
 
     The bounds :math:`\\min` and :math:`\\max` can be tensors.
 
     See :class:`pfhedge.nn.Clamp` for details.
     """
     return leaky_clamp(input, min=min, max=max, clamped_slope=0.0)
+
+
+def realized_variance(input: Tensor, dt: Union[Tensor, float]) -> Tensor:
+    """Returns the realized variance of the price.
+
+    Realized variance :math:`\\sigma^2` of the stock price :math:`S` is defined as:
+
+    .. math ::
+
+        \\sigma^2 = \\frac{1}{T - 1} \\sum_{i = 1}^{T - 1}
+        \\frac{1}{dt} \\log(S_{i + 1} / S_i)^2
+
+    where :math:`T` is the number of time steps.
+
+    .. note ::
+
+        The mean of log return is assumed to be zero.
+
+    Args:
+        input (torch.Tensor): The input tensor.
+        dt (torch.Tensor or float): The intervals of the time steps.
+
+    Shape:
+        - input: :math:`(*, T)` where :math:`T` stands for the number of time steps
+          and :math:`*` means any number of additional dimensions.
+        - output: :math:`(*)`
+
+    Returns:
+        torch.Tensor
+    """
+    return input.log().diff(dim=-1).square().mean(dim=-1) / dt
+
+
+def realized_volatility(input: Tensor, dt: Union[Tensor, float]) -> Tensor:
+    """Returns the realized volatility of the price.
+    It is square root of :func:`realized_variance`.
+
+    Args:
+        input (torch.Tensor): The input tensor.
+        dt (torch.Tensor or float): The intervals of the time steps.
+
+    Shape:
+        - input: :math:`(*, T)` where :math:`T` stands for the number of time steps
+          and :math:`*` means any number of additional dimensions.
+        - output: :math:`(*)`
+
+    Returns:
+        torch.Tensor
+    """
+    return realized_variance(input, dt=dt).sqrt()
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/bs/_base.py` & `pfhedge-0.9.0/pfhedge/nn/modules/bs/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 
 
 class BSModuleMixin(Module):
     """A mixin class for Black-Scholes formula modules.
 
     Shape:
         - Input: :math:`(N, *, H_\\text{in})`, where :math:`*` means any number of
-          additional dimensions. See `inputs()` for the names of input features.
+          additional dimensions. See :func:`inputs` for the names of input features.
         - Output: :math:`(N, *, 1)`: All but the last dimension are the same shape
           as the input.
     """
 
     def forward(self, input: Tensor) -> Tensor:
         """Returns delta of the derivative.
 
         Args:
             input (torch.Tensor): The input tensor. Features are concatenated along
-                the last dimension. See `inputs()` for the names of the input features.
+                the last dimension.
+                See :func:`inputs()` for the names of the input features.
 
         Returns:
             torch.Tensor
         """
         return self.delta(*(input[..., [i]] for i in range(input.size(-1))))
 
     @abc.abstractmethod
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/bs/american_binary.py` & `pfhedge-0.9.0/pfhedge/nn/modules/bs/american_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,26 @@
     Args:
         call (bool, default=True): Specifies whether the option is call
             or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
         - Input: :math:`(N, *, 4)`, where :math:`*` means any number of additional
-          dimensions. See `inputs()` for the names of input features.
+          dimensions. See :func:`inputs` for the names of input features.
         - Output: :math:`(N, *, 1)`. Delta of the derivative.
           All but the last dimension are the same shape as the input.
 
     .. seealso ::
 
         - :class:`pfhedge.nn.BlackScholes`:
           Initialize Black-Scholes formula module from a derivative.
 
     Examples:
 
-        The `forward` method returns delta of the derivative.
+        The ``forward`` method returns delta of the derivative.
 
         >>> from pfhedge.nn import BSAmericanBinaryOption
         >>>
         >>> m = BSAmericanBinaryOption(strike=1.0)
         >>> m.inputs()
         ['log_moneyness', 'max_log_moneyness', 'expiry_time', 'volatility']
         >>> input = torch.tensor([
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/bs/black_scholes.py` & `pfhedge-0.9.0/pfhedge/nn/modules/bs/black_scholes.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 from .european_binary import BSEuropeanBinaryOption
 from .lookback import BSLookbackOption
 
 
 class BlackScholes(Module):
     """Initialize Black-Scholes formula module from a derivative.
 
-    The `forward` method returns the Black-Scholes delta.
+    The ``forward`` method returns the Black-Scholes delta.
 
     Args:
         derivative (:class:`pfhedge.instruments.Derivative`):
             The derivative to get the Black-Scholes formula.
 
     Shape:
         - Input : :math:`(N, *, H_{\\mathrm{in}})`, where :math:`*` means any number of
           additional dimensions and :math:`H_{\\mathrm{in}}` is the number of input
-          features. See `inputs()` for the names of input features.
+          features. See :func:`inputs` for the names of input features.
         - Output : :math:`(N, *, 1)`. All but the last dimension are the same shape
           as the input.
 
     Examples:
 
         One can instantiate Black-Scholes module by using a derivative.
         For example, one can instantiate :class:`BSEuropeanOption` using
         a :class:`pfhedge.instruments.EuropeanOption`.
-        The `forward` method returns delta of the derivative.
+        The ``forward`` method returns delta of the derivative.
 
         >>> import torch
         >>> from pfhedge.instruments import BrownianStock
         >>> from pfhedge.instruments import EuropeanOption
         >>> from pfhedge.nn import BlackScholes
         >>>
         >>> derivative = EuropeanOption(BrownianStock(), strike=1.1)
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/bs/european.py` & `pfhedge-0.9.0/pfhedge/nn/modules/bs/european.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
     Args:
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
         - Input : :math:`(N, *, 3)`, where :math:`*` means any number
-          of additional dimensions. See `inputs()` for the names of input features.
+          of additional dimensions. See ``inputs`` for the names of input features.
         - Output: :math:`(N, *, 1)`. Delta of the derivative.
           All but the last dimension are the same shape as the input.
 
     .. seealso ::
 
         - :class:`pfhedge.nn.BlackScholes`:
           Initialize Black-Scholes formula module from a derivative.
 
     Examples:
 
-        The `forward` method returns delta of the derivative.
+        The ``forward`` method returns delta of the derivative.
 
         >>> from pfhedge.nn import BSEuropeanOption
         >>>
         >>> m = BSEuropeanOption()
         >>> m.inputs()
         ['log_moneyness', 'expiry_time', 'volatility']
         >>> input = torch.tensor([
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/bs/european_binary.py` & `pfhedge-0.9.0/pfhedge/nn/modules/bs/european_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
     Args:
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
         - Input: :math:`(N, *, 3)`, where :math:`*` means any number of additional
-          dimensions. See `inputs()` for the names of input features.
+          dimensions. See :func:`inputs` for the names of input features.
         - Output: :math:`(N, *, 1)` Delta of the derivative.
           All but the last dimension are the same shape as the input.
 
     .. seealso ::
 
         - :class:`pfhedge.nn.BlackScholes`:
           Initialize Black-Scholes formula module from a derivative.
 
     Examples:
 
-        The `forward` method returns delta of the derivative.
+        The ``forward`` method returns delta of the derivative.
 
         >>> from pfhedge.nn import BSEuropeanBinaryOption
         >>>
         >>> m = BSEuropeanBinaryOption(strike=1.0)
         >>> m.inputs()
         ['log_moneyness', 'expiry_time', 'volatility']
         >>> input = torch.tensor([
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/bs/lookback.py` & `pfhedge-0.9.0/pfhedge/nn/modules/bs/lookback.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
     Args:
         call (bool, default=True): Specifies whether the option is call or put.
         strike (float, default=1.0): The strike price of the option.
 
     Shape:
         - Input: :math:`(N, *, 4)`, where :math:`*` means any number of additional
-          dimensions.  See `inputs()` for the names of input features.
+          dimensions.  See :func:`inputs` for the names of input features.
         - Output: :math:`(N, *, 1)`. Delta of the derivative.
           All but the last dimension are the same shape as the input.
 
     .. seealso ::
 
         - :class:`pfhedge.nn.BlackScholes`:
           Initialize Black-Scholes formula module from a derivative.
 
     Examples:
 
-        The `forward` method returns delta of the derivative.
+        The ``forward`` method returns delta of the derivative.
 
         >>> from pfhedge.nn import BSLookbackOption
         >>>
         >>> m = BSLookbackOption()
         >>> m.inputs()
         ['log_moneyness', 'max_log_moneyness', 'expiry_time', 'volatility']
         >>> input = torch.tensor([
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/clamp.py` & `pfhedge-0.9.0/pfhedge/nn/modules/clamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from torch.nn import Module
 
 from ..functional import clamp
 from ..functional import leaky_clamp
 
 
 class LeakyClamp(Module):
-    """Leakily Clamp all elements in `input` into the range :math:`[\\min, \\max]`.
+    """Leakily Clamp all elements in ``input`` into the range :math:`[\\min, \\max]`.
 
     The bounds :math:`\\min` and :math:`\\max` can be tensors.
 
     If :math:`\\min \\leq \\max`:
 
     .. math ::
 
@@ -64,15 +64,15 @@
 
     def extra_repr(self) -> str:
         return f"clamped_slope={self.clamped_slope}" if self.clamped_slope != 0 else ""
 
     def forward(
         self, input: Tensor, min: Optional[Tensor] = None, max: Optional[Tensor] = None
     ) -> Tensor:
-        """Clamp all elements in `input` into the range :math:`[\\min, \\max]`.
+        """Clamp all elements in ``input`` into the range :math:`[\\min, \\max]`.
 
         Args:
             input (torch.Tensor): The input tensor.
             min (torch.Tensor, optional): Lower-bound of the range to be clamped to.
             max (torch.Tensor, optional): Upper-bound of the range to be clamped to.
 
         Shape:
@@ -85,15 +85,15 @@
         Returns:
             torch.Tensor
         """
         return leaky_clamp(input, min=min, max=max, clamped_slope=self.clamped_slope)
 
 
 class Clamp(Module):
-    """Clamp all elements in `input` into the range :math:`[\\min, \\max]`.
+    """Clamp all elements in ``input`` into the range :math:`[\\min, \\max]`.
 
     The bounds :math:`\\min` and :math:`\\max` can be tensors.
 
     If :math:`\\min \\leq \\max`:
 
     .. math ::
 
@@ -140,15 +140,15 @@
         >>> m(input, min, max)
         tensor([0.0000, 0.5000])
     """
 
     def forward(
         self, input: Tensor, min: Optional[Tensor] = None, max: Optional[Tensor] = None
     ) -> Tensor:
-        """Clamp all elements in `input` into the range :math:`[\\min, \\max]`.
+        """Clamp all elements in ``input`` into the range :math:`[\\min, \\max]`.
 
         Args:
             input (torch.Tensor): The input tensor.
             min (torch.Tensor, optional): Lower-bound of the range to be clamped to.
             max (torch.Tensor, optional): Upper-bound of the range to be clamped to.
 
         Shape:
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/hedger.py` & `pfhedge-0.9.0/pfhedge/nn/modules/hedger.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 from .loss import EntropicRiskMeasure
 from .loss import HedgeLoss
 
 TensorOrFloat = Union[Tensor, float]
 
 
 class Hedger(Module):
-    """A `torch.nn.Module` to hedge and price derivatives.
+    """A ``torch.nn.Module`` to hedge and price derivatives.
 
     Args:
         model (torch.nn.Module): Hedging model to compute the hedge ratio at the
             next time step from the input features at the current time step.
             The input and output shapes should be :math:`(N, H_\\text{in})` and
-            :math:`(N, 1)` respectively, where `N` stands for the number simulated
+            :math:`(N, 1)` respectively, where :math:`N` stands for the number simulated
             paths of the asset prices and :math:`H_\\text{in}` stands for the number of
-            input features (namely, `len(inputs)`).
+            input features (namely, ``len(inputs)``).
         inputs (list[str|Feature]): List of (names of) input features to feed to model.
-            See `[str(f) for f in pfhedge.features.FEATURES]` for valid options.
+            See ``[str(f) for f in pfhedge.features.FEATURES]`` for valid options.
         criterion (HedgeLoss, default=EntropicRiskMeasure()):
             Loss function to minimize by hedging.
             Default: :class:`pfhedge.nn.EntropicRiskMeasure()` .
 
     Shape:
         - Input: :math:`(N, H_{\\text{in}})` where :math:`H_{\\text{in}}` is
           the number of input features.
@@ -125,15 +125,15 @@
         self.model = model
         self.inputs = [get_feature(i) for i in inputs]
         self.criterion = criterion
 
         self.register_forward_hook(save_prev_output)
 
     def forward(self, input: Tensor) -> Tensor:
-        """Returns the outout of `model`.
+        """Returns the outout of ``self.model``.
 
         The output represents the hedge ratio at the next time step.
         """
         return self.model(input)
 
     def extra_repr(self) -> str:
         return "inputs=" + str(list(map(str, self.inputs)))
@@ -144,25 +144,25 @@
         n_paths: int = 1000,
         init_state: Optional[Tuple[TensorOrFloat, ...]] = None,
     ) -> Tensor:
         """Returns the profit and loss distribution after hedging.
 
         A hedger sells the derivative to its customer and obliges to settle the payoff
         at maturity. The dealer hedges the risk of this liability by trading
-        the underlying instrument of the derivative based on `model`.
+        the underlying instrument of the derivative based on ``self.model``.
         The resulting profit and loss is obtained by adding up the payoff to the
         customer, capital gains from the underlying asset, and the transaction cost.
 
         Args:
             derivative (pfhedge.instruments.Derivative): The derivative to hedge.
             n_paths (int, default=1000): The number of simulated price paths of the
                 underlying instrument.
             init_state (tuple[torch.Tensor | float], optional): The initial state of
                 the underlying instrument of the derivative.
-                If `None` (default), it uses the default value.
+                If ``None`` (default), it uses the default value.
 
         Shape:
             - Output: :math:`(N)`, where :math:`N` is the number of paths.
 
         Returns:
             torch.Tensor
 
@@ -230,19 +230,19 @@
     ) -> Tensor:
         """Returns the loss of the profit and loss distribution after hedging.
 
         Args:
             derivative (pfhedge.instruments.Derivative): The derivative to hedge.
             n_paths (int, default=1000): The number of simulated price paths of the
                 underlying instrument.
-            n_times (int, default=1): If `n_times > 1`, returns the ensemble mean
+            n_times (int, default=1): If ``n_times > 1``, returns the ensemble mean
                 of the losses computed through multiple simulations.
             init_state (tuple, optional): The initial price of the underlying
                 instrument of the derivative.
-                If `None` (default), sensible default value is used.
+                If ``None`` (default), sensible default value is used.
             enable_grad (bool, default=True): Context-manager that sets gradient
                 calculation to on or off.
 
         Shape:
             - Output: :math:`()`
 
         Returns:
@@ -283,22 +283,22 @@
         It returns the trade history, that is, validation loss after each simulation.
 
         Args:
             derivative (pfhedge.instruments.Derivative): The derivative to hedge.
             n_epochs (int, default=100): Number of Monte-Carlo simulations.
             n_paths (int, default=1000): The number of simulated price paths of the
                 underlying instrument.
-            n_times (int, default=1): If `n_times > 1`, returns the ensemble mean of
+            n_times (int, default=1): If ``n_times > 1``, returns the ensemble mean of
                 the losses computed through multiple simulations.
             optimizer (torch.optim.Optimizer, default=Adam): The optimizer algorithm
-                to use.  It can be an instance or a class of `torch.optim.Optimizer`.
+                to use.  It can be an instance or a class of ``torch.optim.Optimizer``.
             init_state (tuple, optional): The initial price of the underlying
                 instrument of the derivative.
-                If `None` (default), sensible default value is used.
-            verbose (bool, default=True): If `True`, print progress of the training to
+                If ``None`` (default), sensible default value is used.
+            verbose (bool, default=True): If ``True``, print progress of the training to
                 standard output.
 
         Returns:
             list[float]
 
         Examples:
 
@@ -350,15 +350,15 @@
 
         def compute_loss(**kwargs) -> Tensor:
             return self.compute_loss(
                 derivative, n_paths=n_paths, init_state=init_state, **kwargs
             )
 
         history = []
-        progress = tqdm(range(n_epochs)) if verbose else range(n_epochs)
+        progress = tqdm(range(n_epochs), disable=not verbose)
         for _ in progress:
             # Compute training loss and backpropagate
             self.train()
             optimizer.zero_grad()
             loss = compute_loss()
             loss.backward()
             optimizer.step()
@@ -383,19 +383,19 @@
     ) -> Tensor:
         """Evaluate the premium of the given derivative.
 
         Args:
             derivative (pfhedge.instuments.Derivative): The derivative to price.
             n_paths (int, default=1000): The number of simulated price paths of the
                 underlying instrument.
-            n_times (int, default=1): If `n_times > 1`, returns the ensemble mean of
+            n_times (int, default=1): If ``n_times > 1``, returns the ensemble mean of
                 the losses computed through multiple simulations.
             init_state (tuple, optional): The initial price of the underlying
                 instrument of the derivative.
-                If `None` (default), sensible default value is used.
+                If ``None`` (default), sensible default value is used.
             enable_grad (bool, default=False): Context-manager that sets gradient
                 calculation to on or off.
 
         Shape:
             - Output: :math:`()`
 
         Returns:
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/loss.py` & `pfhedge-0.9.0/pfhedge/nn/modules/loss.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             torch.Tensor
         """
 
     def cash(self, input: Tensor) -> Tensor:
         """Returns the cash amount which is as preferable as
         the given profit-loss distribution in terms of the loss.
 
-        The output `cash` is expected to satisfy the following relation:
+        The output ``cash`` is expected to satisfy the following relation:
 
         .. code::
 
             loss(torch.full_like(pnl, cash)) = loss(pnl)
 
         By default, the output is computed by binary search.
         If analytic form is known, it is recommended to override this method
@@ -60,15 +60,16 @@
         """
         return bisect(self, self(input), input.min(), input.max())
 
 
 class EntropicRiskMeasure(HedgeLoss):
     """Creates a loss given by the entropic risk measure.
 
-    The entropic risk measure of the profit-loss distribution `pnl` is given by:
+    The entropic risk measure of the profit-loss distribution
+    :math:`\\text{pnl}` is given by:
 
     .. math ::
 
         \\text{loss}(\\text{pnl}) = \\frac{1}{a}
         \\log(- \\mathbf{E}[u(\\text{pnl})]) \\,,
         \\quad
         u(x) = -\\exp(-a x) \\,.
@@ -123,15 +124,15 @@
         """
         return -self(input)
 
 
 class EntropicLoss(HedgeLoss):
     """Creates a loss given by the negative of expected exponential utility.
 
-    The loss of the profit-loss `pnl` is given by
+    The loss of the profit-loss :math:`\\text{pnl}` is given by:
 
     .. math ::
 
         \\text{loss}(\\text{pnl}) = -\\mathbf{E}[u(\\text{pnl})] \\,,
         \\quad
         u(x) = -\\exp(-a x) \\,.
 
@@ -186,15 +187,15 @@
         """
         return -(-exp_utility(input, a=self.a).mean(0)).log() / self.a
 
 
 class IsoelasticLoss(HedgeLoss):
     """Creates a loss function that measures the isoelastic utility.
 
-    The loss of the profit-loss distribution `pnl` is given by
+    The loss of the profit-loss :math:`\\text{pnl}` is given by:
 
     .. math ::
 
         \\text{loss}(\\text{pnl}) = -\\mathbf{E}[u(\\text{pnl})] \\,,
         \\quad
         u(x) = \\begin{cases}
         x^{1 - a} & a \\neq 1 \\\\
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/mlp.py` & `pfhedge-0.9.0/pfhedge/nn/modules/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
 class MultiLayerPerceptron(Sequential):
     """A feed-forward neural network.
 
     Number of input features is lazily determined.
 
     Args:
         in_features (int, default=None): Size of each input sample.
-            If `None` (default), the number of input features will be
-            will be inferred from the `input.shape[-1]` after the first call to
-            `forward` is done. Also, before the first `forward` parameters in the
-            module are of `torch.nn.UninitializedParameter` class.
+            If ``None`` (default), the number of input features will be
+            will be inferred from the ``input.shape[-1]`` after the first call to
+            ``forward`` is done. Also, before the first ``forward`` parameters in the
+            module are of ``torch.nn.UninitializedParameter`` class.
         out_features (int, default=1): Size of each output sample.
         n_layers (int, default=4): Number of hidden layers.
         n_units (int or tuple[int], default=32): Number of units in each hidden layer.
-            If `tuple[int]`, it specifies different number of units for each layer.
+            If ``tuple[int]``, it specifies different number of units for each layer.
         activation (torch.nn.Module, default=torch.nn.ReLU()):
             Activation module of the hidden layers.
         out_activation (torch.nn.Module, default=torch.nn.Identity()):
             Activation module of the output layer.
 
     Shape:
         - Input: :math:`(N, *, H_{\\text{in}})`, where where * means any number of
           additional dimensions and :math:`H_{\\text{in}})` is the number of input
           features.
         - Output: :math:`(N, *, H_{\\text{out}})`, where all but the last dimension
           are the same shape as the input and :math:`H_{\\text{in}})` is
-          `out_features`.
+          ``out_features``.
 
     Examples:
 
-        By default, `in_features` is lazily determined:
+        By default, ``in_features`` is lazily determined:
 
         >>> import torch
         >>> from pfhedge.nn import MultiLayerPerceptron
         >>>
         >>> m = MultiLayerPerceptron()
         >>> m
         MultiLayerPerceptron(
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/naked.py` & `pfhedge-0.9.0/pfhedge/nn/modules/naked.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Shape:
         - Input: :math:`(N, *, H_{\\text{in}})`, where where * means any number of
           additional dimensions and :math:`H_{\\text{in}})` is the number of input
           features.
         - Output: :math:`(N, *, H_{\\text{out}})`, where all but the last dimension
           are the same shape as the input and :math:`H_{\\text{in}})` is
-          `out_features`.
+          ``out_features``.
 
     Examples:
 
         >>> from pfhedge.nn import Naked
         >>>
         >>> m = Naked()
         >>> input = torch.empty((2, 3))
```

### Comparing `pfhedge-0.8.1/pfhedge/nn/modules/ww.py` & `pfhedge-0.9.0/pfhedge/nn/modules/ww.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 from .bs.black_scholes import BlackScholes
 from .clamp import Clamp
 
 
 class WhalleyWilmott(Module):
     """Initialize Whalley-Wilmott's hedging strategy of a derivative.
 
-    The `forward` method returns the next hedge ratio.
+    The ``forward`` method returns the next hedge ratio.
 
     This is the optimal hedging strategy for asymptotically small transaction cost.
 
     Args:
         derivative (:class:`pfhedge.instruments.Derivative`): Derivative to hedge.
         a (float, default=1.0): Risk aversion parameter in exponential utility.
 
     Shape:
         - Input: :math:`(N, *, H_{\\text{in}})`.  Here, :math:`*` means any number of
-          additional dimensions and `H_in` is the number of input features.
-          See `inputs()` for the names of input features.
+          additional dimensions and :math:`H_{\\text{in}}` is
+          the number of input features.
+          See :func:`inputs()` for the names of input features.
         - Output: :math:`(N, *, 1)`. The hedge ratio at the next time step.
 
     Examples:
 
         An example for :class:`pfhedge.instruments.EuropeanOption`.
 
         >>> import torch
```

### Comparing `pfhedge-0.8.1/pfhedge/stochastic/brownian.py` & `pfhedge-0.9.0/pfhedge/stochastic/brownian.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,25 +29,26 @@
         dS(t) = \\sigma dW(t) \\,.
 
     Args:
         n_paths (int): The number of simulated paths.
         n_steps (int): The number of time steps.
         init_state (tuple[torch.Tensor | float], default=(0.0,)): The initial state of
             the time series.
-            This is specified by `(S0,)`, where `S0` is the initial value of :math:`S`.
-            It also accepts a float or a `torch.Tensor`.
+            This is specified by ``(S0,)``, where ``S0`` is
+            the initial value of :math:`S`.
+            It also accepts a ``torch.Tensor` or a ``float``.
         volatility (float, default=0.2): The volatility of the Brownian motion.
         dt (float, default=1/250): The intervals of the time steps.
         dtype (torch.dtype, optional): The desired data type of returned tensor.
-            Default: If `None`, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            Default: If ``None``, uses a global default
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): The desired device of returned tensor.
-            Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and the current CUDA device
+            Default: If ``None``, uses the current device for the default tensor type
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and the current CUDA device
             for CUDA tensor types.
 
     Shape:
         - Output: :math:`(N, T)`, where :math:`N` is the number of paths and
           :math:`T` is the number of time steps.
 
     Returns:
@@ -97,25 +98,25 @@
         dS(t) = \\sigma S(t) dW(t) \\,.
 
     Args:
         n_paths (int): The number of simulated paths.
         n_steps (int): The number of time steps.
         init_state (tuple[torch.Tensor | float], default=(1.0,)): The initial state of
             the time series.
-            This is specified by `(S0,)`, where `S0` is the initial value of :math:`S`.
-            It also accepts a float or a `torch.Tensor`.
+            This is specified by ``(S0,)``, where ``S0`` is the initial value of :math:`S`.
+            It also accepts a ``torch.Tensor`` or a ``float``.
         volatility (float, default=0.2): The volatility of the Brownian motion.
         dt (float, default=1/250): The intervals of the time steps.
         dtype (torch.dtype, optional): The desired data type of returned tensor.
-            Default: If `None`, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            Default: If ``None``, uses a global default
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): The desired device of returned tensor.
-            Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and the current CUDA device
+            Default: If ``None``, uses the current device for the default tensor type
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and the current CUDA device
             for CUDA tensor types.
 
     Shape:
         - Output: :math:`(N, T)`, where :math:`T` is the number of time steps and
           :math:`N` is the number of paths.
 
     Returns:
```

### Comparing `pfhedge-0.8.1/pfhedge/stochastic/cir.py` & `pfhedge-0.9.0/pfhedge/stochastic/cir.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,27 +31,28 @@
     Time-series is generated by Andersen's QE-M method (See Reference for details).
 
     Args:
         n_paths (int): The number of simulated paths.
         n_steps (int): The number of time steps.
         init_state (tuple[torch.Tensor | float], default=(0.04,)): The initial state of
             the time series.
-            This is specified by `(X0,)`, where `X0` is the initial value of :math:`X`.
-            It also accepts a float or a `torch.Tensor`.
+            This is specified by ``(X0,)``, where ``X0`` is
+            the initial value of :math:`X`.
+            It also accepts a ``torch.Tensor`` or a float.
         kappa (torch.Tensor or float, default=1.0): The parameter :math:`\\kappa`.
         theta (torch.Tensor or float, default=0.04): The parameter :math:`\\theta`.
         sigma (torch.Tensor or float, default=2.0): The parameter :math:`\\sigma`.
         dt (torch.Tensor or float, default=1/250): The intervals of the time steps.
         dtype (torch.dtype, optional): The desired data type of returned tensor.
-            Default: If `None`, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            Default: If ``None``, uses a global default
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): The desired device of returned tensor.
             Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and the current CUDA device
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and the current CUDA device
             for CUDA tensor types.
 
     Shape:
         - Output: :math:`(N, T)`, where :math:`N` is the number of paths and
           :math:`T` is the number of time steps.
 
     Returns:
```

### Comparing `pfhedge-0.8.1/pfhedge/stochastic/heston.py` & `pfhedge-0.9.0/pfhedge/stochastic/heston.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,28 +37,28 @@
     Time-series is generated by Andersen's QE-M method (See Reference for details).
 
     Args:
         n_paths (int): The number of simulated paths.
         n_steps (int): The number of time steps.
         init_state (tuple[torch.Tensor | float], default=(1.0,)): The initial state of
             the time series.
-            This is specified by `(S0, V0)`, where `S0` and `V0` are the initial values
+            This is specified by ``(S0, V0)``, where ``S0`` and ``V0`` are the initial values
             of :math:`S` and :math:`V`, respectively.
         kappa (float, default=1.0): The parameter :math:`\\kappa`.
         theta (float, default=0.04): The parameter :math:`\\theta`.
         sigma (float, default=2.0): The parameter :math:`\\sigma`.
         rho (float, default=-0.7): The parameter :math:`\\rho`.
         dt (float, default=1/250): The intervals of the time steps.
         dtype (torch.dtype, optional): The desired data type of returned tensor.
-            Default: If `None`, uses a global default
-            (see `torch.set_default_tensor_type()`).
+            Default: If ``None``, uses a global default
+            (see ``torch.set_default_tensor_type()``).
         device (torch.device, optional): The desired device of returned tensor.
-            Default: if None, uses the current device for the default tensor type
-            (see `torch.set_default_tensor_type()`).
-            `device` will be the CPU for CPU tensor types and the current CUDA device
+            Default: If ``None``, uses the current device for the default tensor type
+            (see ``torch.set_default_tensor_type()``).
+            ``device`` will be the CPU for CPU tensor types and the current CUDA device
             for CUDA tensor types.
 
     Shape:
         - Output: :math:`(N, T)`, where :math:`N` is the number of paths and
           :math:`T` is the number of time steps.
 
     Returns:
```

### Comparing `pfhedge-0.8.1/pyproject.toml` & `pfhedge-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pfhedge"
-version = "0.8.1"
+version = "0.9.0"
 description = "Deep Hedging in PyTorch"
 authors = ["Shota Imaki <shota.imaki.0801@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/pfnet-research/pfhedge"
 
 [tool.poetry.dependencies]
 python = "^3.6.13"
```

### Comparing `pfhedge-0.8.1/setup.py` & `pfhedge-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=1.9.0,<2.0.0', 'tqdm>=4.59.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pfhedge',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Deep Hedging in PyTorch',
     'long_description': None,
     'author': 'Shota Imaki',
     'author_email': 'shota.imaki.0801@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pfnet-research/pfhedge',
```

### Comparing `pfhedge-0.8.1/PKG-INFO` & `pfhedge-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfhedge
-Version: 0.8.1
+Version: 0.9.0
 Summary: Deep Hedging in PyTorch
 Home-page: https://github.com/pfnet-research/pfhedge
 License: MIT
 Author: Shota Imaki
 Author-email: shota.imaki.0801@gmail.com
 Requires-Python: >=3.6.13,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

