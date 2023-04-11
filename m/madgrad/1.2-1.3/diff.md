# Comparing `tmp/madgrad-1.2.tar.gz` & `tmp/madgrad-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/private/home/adefazio/madgrad/dist/tmpq2y1xbg2/madgrad-1.2.tar", last modified: Tue Mar  8 18:11:27 2022, max compression
+gzip compressed data, was "dist/madgrad-1.3.tar", last modified: Tue Apr 11 19:32:17 2023, max compression
```

## Comparing `madgrad-1.2.tar` & `madgrad-1.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2022-03-08 18:11:27.000000 madgrad-1.2/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1086 2021-02-03 15:56:57.000000 madgrad-1.2/LICENSE
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3556 2022-03-08 18:11:27.000000 madgrad-1.2/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3086 2022-03-08 17:31:44.000000 madgrad-1.2/README.md
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2022-03-08 18:11:27.000000 madgrad-1.2/madgrad/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      433 2022-03-08 17:31:44.000000 madgrad-1.2/madgrad/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3884 2022-03-08 17:31:44.000000 madgrad-1.2/madgrad/fairseq_madgrad.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3868 2022-03-08 17:31:44.000000 madgrad-1.2/madgrad/fairseq_mirror_madgrad.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7546 2022-03-08 17:31:44.000000 madgrad-1.2/madgrad/madgrad.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5741 2022-03-08 17:31:44.000000 madgrad-1.2/madgrad/mirror_madgrad.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2022-03-08 18:11:27.000000 madgrad-1.2/madgrad.egg-info/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3556 2022-03-08 18:11:27.000000 madgrad-1.2/madgrad.egg-info/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      291 2022-03-08 18:11:27.000000 madgrad-1.2/madgrad.egg-info/SOURCES.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2022-03-08 18:11:27.000000 madgrad-1.2/madgrad.egg-info/dependency_links.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        8 2022-03-08 18:11:27.000000 madgrad-1.2/madgrad.egg-info/top_level.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      282 2021-02-08 20:16:37.000000 madgrad-1.2/pyproject.toml
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2022-03-08 18:11:27.000000 madgrad-1.2/setup.cfg
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      845 2022-03-08 18:02:37.000000 madgrad-1.2/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-11 19:32:17.000000 madgrad-1.3/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1086 2021-02-03 15:56:57.000000 madgrad-1.3/LICENSE
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3556 2023-04-11 19:32:17.000000 madgrad-1.3/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3086 2023-04-11 19:24:56.000000 madgrad-1.3/README.md
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-11 19:32:17.000000 madgrad-1.3/madgrad/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      433 2023-04-11 19:24:56.000000 madgrad-1.3/madgrad/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3868 2023-04-11 19:24:56.000000 madgrad-1.3/madgrad/fairseq_madgrad.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3836 2023-04-11 19:24:56.000000 madgrad-1.3/madgrad/fairseq_mirror_madgrad.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8146 2023-04-11 19:25:01.000000 madgrad-1.3/madgrad/madgrad.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5795 2023-04-11 19:25:01.000000 madgrad-1.3/madgrad/mirror_madgrad.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-11 19:32:17.000000 madgrad-1.3/madgrad.egg-info/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3556 2023-04-11 19:32:16.000000 madgrad-1.3/madgrad.egg-info/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      341 2023-04-11 19:32:17.000000 madgrad-1.3/madgrad.egg-info/SOURCES.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2023-04-11 19:32:16.000000 madgrad-1.3/madgrad.egg-info/dependency_links.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        8 2023-04-11 19:32:16.000000 madgrad-1.3/madgrad.egg-info/top_level.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      282 2021-02-08 20:16:37.000000 madgrad-1.3/pyproject.toml
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2023-04-11 19:32:17.000000 madgrad-1.3/setup.cfg
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      845 2023-04-11 19:25:01.000000 madgrad-1.3/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-11 19:32:17.000000 madgrad-1.3/tests/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3457 2021-02-03 16:00:31.000000 madgrad-1.3/tests/test_madgrad.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2528 2023-04-11 19:24:56.000000 madgrad-1.3/tests/test_mirrormadgrad.py
```

### Comparing `madgrad-1.2/LICENSE` & `madgrad-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `madgrad-1.2/PKG-INFO` & `madgrad-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madgrad
-Version: 1.2
+Version: 1.3
 Summary: A general purpose PyTorch Optimizer
 Home-page: https://github.com/facebookresearch/madgrad
 Author: Aaron Defazio
 Author-email: adefazio@fb.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `madgrad-1.2/README.md` & `madgrad-1.3/README.md`

 * *Files identical despite different names*

### Comparing `madgrad-1.2/madgrad/fairseq_madgrad.py` & `madgrad-1.3/madgrad/fairseq_madgrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import torch.optim
 from .madgrad import MADGRAD
 
 try:
     import fairseq
     from fairseq.optim import register_optimizer
     try:
-        from fairseq.optim import FairseqOptimizer
-    except:
         from fairseq.optim import LegacyFairseqOptimizer as FairseqOptimizer 
+    except:
+        from fairseq.optim import FairseqOptimizer
 except ImportError:
     _has_fairseq = False
 else:
     _has_fairseq = True
 
 if _has_fairseq:
     @register_optimizer('madgrad')
@@ -66,15 +66,15 @@
         def add_args(parser):
             """Add optimizer-specific arguments to the parser."""
             # fmt: off
             parser.add_argument('--weight-decay', '--wd', default=0.0, type=float, metavar='WD',
                                 help='weight decay')
             parser.add_argument('--momentum', default=0.9, type=float, metavar='M',
                                 help='momentum factor')
-            parser.add_argument('--madgrad_eps', default=1e-6, type=float, metavar='M',
+            parser.add_argument('--eps', default=1e-6, type=float, metavar='M',
                                 help='Denominator epsilon')
             parser.add_argument('--decouple_decay', default=False, type=bool, metavar='M',
                                 help='Decouple weight decay (EXPERIMENTAL)')
             # fmt: on
 
         @property
         def optimizer_config(self):
@@ -84,10 +84,10 @@
             resume training using a different set of optimizer args, e.g., with a
             different learning rate.
             """
             return {
                 'lr': self.args.lr[0],
                 'momentum': self.args.momentum,
                 'weight_decay': self.args.weight_decay,
-                'eps': self.args.madgrad_eps,
+                'eps': self.args.eps,
                 'decouple_decay': self.args.decouple_decay,
             }
```

### Comparing `madgrad-1.2/madgrad/fairseq_mirror_madgrad.py` & `madgrad-1.3/madgrad/fairseq_mirror_madgrad.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import torch.optim
 from .mirror_madgrad import MirrorMADGRAD
 
 try:
     import fairseq
     from fairseq.optim import register_optimizer
     try:
-        from fairseq.optim import FairseqOptimizer
-    except:
         from fairseq.optim import LegacyFairseqOptimizer as FairseqOptimizer 
+    except:
+        from fairseq.optim import FairseqOptimizer
 except ImportError:
     _has_fairseq = False
 else:
     _has_fairseq = True
 
 if _has_fairseq:
     @register_optimizer('mirror_madgrad')
@@ -43,15 +43,15 @@
                 Iterable of parameters to optimize or dicts defining parameter groups.
             lr (float): 
                 Learning rate (default: 1e-2).
             momentum (float): 
                 Momentum value in the range [0,1) (default: 0.9).
             weight_decay (float): 
                 Weight decay, i.e. a L2 penalty (default: 0).
-            madgrad_eps (float): 
+            eps (float): 
                 Term added to the denominator outside of the root operation to improve numerical stability. (default: 0).
                 This parameter is less important in MADGRAD than in Adam. A value of 0 will likely give the best results.
             decouple_decay (bool):
                 Apply AdamW style decoupled weight decay (EXPERIMENTAL). 
                 Application of decay occurs before the step.
         """
 
@@ -63,15 +63,15 @@
         def add_args(parser):
             """Add optimizer-specific arguments to the parser."""
             # fmt: off
             parser.add_argument('--weight-decay', '--wd', default=0.0, type=float, metavar='WD',
                                 help='weight decay')
             parser.add_argument('--momentum', default=0.9, type=float, metavar='M',
                                 help='momentum factor')
-            parser.add_argument('--madgrad_eps', default=0, type=float, metavar='M',
+            parser.add_argument('--eps', default=0, type=float, metavar='M',
                                 help='Denominator epsilon')
             parser.add_argument('--decouple_decay', default=False, type=bool, metavar='M',
                                 help='Decouple weight decay (EXPERIMENTAL)')
             # fmt: on
 
         @property
         def optimizer_config(self):
@@ -81,10 +81,10 @@
             resume training using a different set of optimizer args, e.g., with a
             different learning rate.
             """
             return {
                 'lr': self.args.lr[0],
                 'momentum': self.args.momentum,
                 'weight_decay': self.args.weight_decay,
-                'madgrad_eps': self.args.madgrad_eps,
+                'eps': self.args.eps,
                 'decouple_decay': self.args.decouple_decay,
             }
```

### Comparing `madgrad-1.2/madgrad/madgrad.py` & `madgrad-1.3/madgrad/madgrad.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,28 +54,28 @@
 
     def __init__(
         self, params: _params_t, lr: float = 1e-2, momentum: float = 0.9, 
         weight_decay: float = 0, eps: float = 1e-6, decouple_decay=False,
     ):
         if momentum < 0 or momentum >= 1:
             raise ValueError(f"Momentum {momentum} must be in the range [0,1)")
-        if lr <= 0:
-            raise ValueError(f"Learning rate {lr} must be positive")
+        if lr < 0:
+            raise ValueError(f"Learning rate {lr} must be non-negative")
         if weight_decay < 0:
             raise ValueError(f"Weight decay {weight_decay} must be non-negative")
         if eps < 0:
             raise ValueError(f"Eps must be non-negative")
 
         defaults = dict(lr=lr, eps=eps, momentum=momentum, 
                         weight_decay=weight_decay, decouple_decay=decouple_decay)
         super().__init__(params, defaults)
 
     @property
     def supports_memory_efficient_fp16(self) -> bool:
-        return False
+        return True
 
     @property
     def supports_flat_params(self) -> bool:
         return True
 
     def step(self, closure: Optional[Callable[[], float]] = None) -> Optional[float]:
         """Performs a single optimization step.
@@ -92,52 +92,63 @@
         # optimizer sharding
         if 'k' not in self.state:
             self.state['k'] = torch.tensor([0], dtype=torch.long)
         k = self.state['k'].item()
 
         for group in self.param_groups:
             eps = group["eps"]
-            lr = group["lr"] + eps
+            lr = group["lr"]
+            if lr != 0.0:
+                lr = lr + eps # For stability
             decay = group["weight_decay"]
             momentum = group["momentum"]
-            decouple_decay = group["decouple_decay"]
+            decouple_decay = group.get("decouple_decay", False)
 
             ck = 1 - momentum
             lamb = lr * math.pow(k + 1, 0.5)
 
             for p in group["params"]:
                 if p.grad is None:
                     continue
+                # grad = p.grad.data
+                # state = self.state[p]
                 grad = p.grad.data
+                if grad.dtype in {torch.float16, torch.bfloat16}:
+                    grad = grad.float()
                 state = self.state[p]
 
+                p_data_fp32 = p.data
+                if p.data.dtype in {torch.float16, torch.bfloat16}:
+                    p_data_fp32 = p_data_fp32.float()
+
+
                 if "grad_sum_sq" not in state:
-                    state["grad_sum_sq"] = torch.zeros_like(p.data).detach()
-                    state["s"] = torch.zeros_like(p.data).detach()
+                    state["grad_sum_sq"] = torch.zeros_like(p_data_fp32).detach()
+                    state["s"] = torch.zeros_like(p_data_fp32).detach()
                     if momentum != 0:
-                        state["x0"] = torch.clone(p.data).detach()
+                        state["x0"] = torch.clone(p_data_fp32).detach()
 
                 if momentum != 0.0 and grad.is_sparse:
                     raise RuntimeError("momentum != 0 is not compatible with sparse gradients")
 
                 grad_sum_sq = state["grad_sum_sq"]
                 s = state["s"]
 
                 # Apply weight decay
                 if decay != 0 and not decouple_decay:
                     if grad.is_sparse:
                         raise RuntimeError("weight_decay option is not compatible with sparse gradients")
 
-                    grad.add_(p.data, alpha=decay)
+                    grad.add_(p_data_fp32, alpha=decay)
 
                 if grad.is_sparse:
                     grad = grad.coalesce()
                     grad_val = grad._values()
 
-                    p_masked = p.sparse_mask(grad)
+                    p_masked = p_data_fp32.sparse_mask(grad)
                     grad_sum_sq_masked = grad_sum_sq.sparse_mask(grad)
                     s_masked = s.sparse_mask(grad)
 
                     # Compute x_0 from other known quantities
                     rms_masked_vals = grad_sum_sq_masked._values().pow(1 / 3).add_(eps)
                     x0_masked_vals = p_masked._values().addcdiv(s_masked._values(), rms_masked_vals, value=1)
 
@@ -159,39 +170,41 @@
                     # Copy updated masked p to dense p using an add operation
                     p_masked._values().add_(p_kp1_masked_vals, alpha=-1)
                     p.data.add_(p_masked, alpha=-1)
                 else:
                     if momentum == 0:
                         # Compute x_0 from other known quantities
                         rms = grad_sum_sq.pow(1 / 3).add_(eps)
-                        x0 = p.data.addcdiv(s, rms, value=1)
+                        x0 = p_data_fp32.addcdiv(s, rms, value=1)
                     else:
                         x0 = state["x0"]
 
                     # Accumulate second moments
                     grad_sum_sq.addcmul_(grad, grad, value=lamb)
                     rms = grad_sum_sq.pow(1 / 3).add_(eps)
 
                     if eps == 0:
                         rms[rms == 0] = float('inf')
 
                     # Update s
                     s.data.add_(grad, alpha=lamb)
 
                     if decay != 0 and decouple_decay:
-                        p_old = p.data.clone()
+                        p_old = p_data_fp32.clone()
 
                     # Step
                     if momentum == 0:
-                        p.data.copy_(x0.addcdiv(s, rms, value=-1))
+                        p_data_fp32.copy_(x0.addcdiv(s, rms, value=-1))
                     else:
                         z = x0.addcdiv(s, rms, value=-1)
 
                         # p is a moving average of z
-                        p.data.mul_(1 - ck).add_(z, alpha=ck)
+                        p_data_fp32.mul_(1 - ck).add_(z, alpha=ck)
                     
                     if decay != 0 and decouple_decay:
-                        p.data.add_(p_old, alpha=-lr*decay)
+                        p_data_fp32.add_(p_old, alpha=-lr*decay)
 
+                    if p.data.dtype in {torch.float16, torch.bfloat16}:
+                        p.data.copy_(p_data_fp32)
 
         self.state['k'] += 1
         return loss
```

### Comparing `madgrad-1.2/madgrad/mirror_madgrad.py` & `madgrad-1.3/madgrad/mirror_madgrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 
     def __init__(
         self, params: _params_t, lr: float = 1e-2, momentum: float = 0.9, 
         weight_decay: float = 0, eps: float = 0, decouple_decay=False,
     ):
         if momentum < 0 or momentum >= 1:
             raise ValueError(f"Momentum {momentum} must be in the range [0,1]")
-        if lr <= 0:
-            raise ValueError(f"Learning rate {lr} must be positive")
+        if lr < 0:
+            raise ValueError(f"Learning rate {lr} must be non-negative")
         if weight_decay < 0:
             raise ValueError(f"Weight decay {weight_decay} must be non-negative")
         if eps < 0:
             raise ValueError(f"Eps must be non-negative")
 
         defaults = dict(lr=lr, eps=eps, momentum=momentum, 
             weight_decay=weight_decay, decouple_decay=decouple_decay)
@@ -92,18 +92,20 @@
         k = self.state['k'].item()
 
         update_ratio = math.pow(k/(k+1), 1/2)
         lamb = math.pow(k+1, 1/3)
 
         for group in self.param_groups:
             eps = group["eps"]
-            lr = group["lr"] + eps
+            lr = group["lr"]
+            if lr != 0.0:
+                lr = lr + eps # For stability
             decay = group["weight_decay"]
             momentum = group["momentum"]
-            decouple_decay = group["decouple_decay"]
+            decouple_decay = group.get("decouple_decay", False)
 
             ck = 1 - momentum
 
             for p in group["params"]:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
@@ -131,16 +133,14 @@
                     if grad.is_sparse:
                         raise RuntimeError("weight_decay option is not compatible with sparse gradients")
 
                     if decouple_decay:
                         z.data.add_(z.data, alpha=-lr*decay)
                     else:
                         grad.add_(p_data_fp32, alpha=decay)
-                        
-
 
                 grad_sum_sq.mul_(update_ratio)
                 # Accumulate second moments
                 grad_sum_sq.addcmul_(grad, grad, value=1)
                 rms = grad_sum_sq.pow(1 / 3).add_(eps)
 
                 if eps == 0:
```

### Comparing `madgrad-1.2/madgrad.egg-info/PKG-INFO` & `madgrad-1.3/madgrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madgrad
-Version: 1.2
+Version: 1.3
 Summary: A general purpose PyTorch Optimizer
 Home-page: https://github.com/facebookresearch/madgrad
 Author: Aaron Defazio
 Author-email: adefazio@fb.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `madgrad-1.2/setup.py` & `madgrad-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="madgrad",
-    version="1.2",
+    version="1.3",
     author="Aaron Defazio",
     author_email="adefazio@fb.com",
     description="A general purpose PyTorch Optimizer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/madgrad",
     packages=setuptools.find_packages(),
```

