# Comparing `tmp/pytorch_optimizer-2.5.1.tar.gz` & `tmp/pytorch_optimizer-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.5.1.tar", max compression
+gzip compressed data, was "pytorch_optimizer-2.5.2.tar", max compression
```

## Comparing `pytorch_optimizer-2.5.1.tar` & `pytorch_optimizer-2.5.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    11357 2023-03-12 05:48:39.506780 pytorch_optimizer-2.5.1/LICENSE
--rw-r--r--   0        0        0    27626 2023-03-12 05:48:39.506780 pytorch_optimizer-2.5.1/README.rst
--rw-r--r--   0        0        0     3463 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     6018 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1575 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     4183 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0        0 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0      131 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4148 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0     1255 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     7108 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5460 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     7217 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     5941 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     5223 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     5004 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     5828 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5053 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0      781 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3862 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5428 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0    18710 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     4165 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0     5540 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/diffrgrad.py
--rw-r--r--   0        0        0    10702 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0      474 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     7601 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     5563 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3954 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     2920 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4493 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6701 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3330 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4149 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4293 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     3702 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     5242 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6827 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/ralamb.py
--rw-r--r--   0        0        0     6224 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12664 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0     4718 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0     3907 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    15763 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    19701 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     7890 2023-03-12 05:48:39.514780 pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0    29628 1970-01-01 00:00:00.000000 pytorch_optimizer-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 13:47:49.754721 pytorch_optimizer-2.5.2/LICENSE
+-rw-r--r--   0        0        0    27626 2023-04-11 13:47:49.754721 pytorch_optimizer-2.5.2/README.rst
+-rw-r--r--   0        0        0     3655 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6018 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1561 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0     4183 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2761 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      491 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0      131 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0     1255 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0        0 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     7108 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5460 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     7217 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     5941 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     5223 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     5004 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     5828 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5053 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0      781 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3862 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5428 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0    18352 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     4165 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0     5540 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffrgrad.py
+-rw-r--r--   0        0        0    10702 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0      474 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     7601 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/gsam.py
+-rw-r--r--   0        0        0     5563 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3954 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     2920 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     4178 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6550 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3639 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4149 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4314 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     3702 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     5242 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6827 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ralamb.py
+-rw-r--r--   0        0        0     6224 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12516 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0     4718 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0     3907 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    15763 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    19688 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     7895 2023-04-11 13:47:49.762721 pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0    29741 1970-01-01 00:00:00.000000 pytorch_optimizer-2.5.2/PKG-INFO
```

### Comparing `pytorch_optimizer-2.5.1/LICENSE` & `pytorch_optimizer-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/README.rst` & `pytorch_optimizer-2.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pyproject.toml` & `pytorch_optimizer-2.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.5.1"
+version = "2.5.2"
 description = "optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas."
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
@@ -33,21 +33,27 @@
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 numpy = [
     { version = "=1.21.1", python = ">=3.7,<3.8" },
     { version = "*", python = ">=3.8" },
 ]
-torch = { version = ">=1.10", source = "torch" }
+torch = [
+    { version = ">=1.10,>=2.0", python = ">=3.8", source = "torch" },
+    { version = "^1.10", python = ">=3.7,<3.8", source = "torch" },
+]
 
 [tool.poetry.dev-dependencies]
-isort = "^5.11.5"
-black = "^23.1.0"
-ruff = "^0.0.244"
-pytest = "^7.2.1"
+isort = [
+    { version = "==5.11.5", python = ">=3.7,<3.8"},
+    { version = "^5.12.0", python = ">=3.8"}
+]
+black = "^23.3.0"
+ruff = "^0.0.260"
+pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 
 [[tool.poetry.source]]
 name = "torch"
 url = "https://download.pytorch.org/whl/cpu"
 secondary = true
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/__init__.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/base/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     """Raised when the gradient is sparse gradient.
 
     :param optimizer_name: str. optimizer name.
     :param note: str. special conditions to note (default '').
     """
 
     def __init__(self, optimizer_name: str, note: str = ''):
-        self.note: str = ' ' if note == '' else f' w/ {note} '
+        self.note: str = ' ' if not note else f' w/ {note} '
         self.message: str = f'[-] {optimizer_name}{self.note}does not support sparse gradient.'
         super().__init__(self.message)
 
 
 class ZeroParameterSizeError(Exception):
     """Raised when the parameter size is 0."""
 
@@ -27,19 +27,19 @@
         super().__init__(self.message)
 
 
 class NegativeLRError(Exception):
     """Raised when learning rate is negative."""
 
     def __init__(self, lr: float, lr_type: str = ''):
-        self.note: str = 'learning rate' if lr_type == '' else lr_type
+        self.note: str = lr_type if lr_type else 'learning rate'
         self.message: str = f'[-] {self.note} must be positive. ({lr} > 0)'
         super().__init__(self.message)
 
 
 class NegativeStepError(Exception):
     """Raised when step is negative."""
 
     def __init__(self, num_steps: int, step_type: str = ''):
-        self.note: str = 'step' if step_type == '' else step_type
+        self.note: str = step_type if step_type else 'step'
         self.message: str = f'[-] {self.note} must be positive. ({num_steps} > 0)'
         super().__init__(self.message)
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/base/optimizer.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/base/optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/base/scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/chebyshev.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,30 +87,27 @@
             self.step_in_cycle = self.step_in_cycle + 1
             if self.step_in_cycle >= self.cur_cycle_steps:
                 self.cycle += 1
                 self.step_in_cycle = self.step_in_cycle - self.cur_cycle_steps
                 self.cur_cycle_steps = (
                     int((self.cur_cycle_steps - self.warmup_steps) * self.cycle_mult) + self.warmup_steps
                 )
-        else:
-            if epoch >= self.first_cycle_steps:
-                if self.cycle_mult == 1.0:
-                    self.step_in_cycle = epoch % self.first_cycle_steps
-                    self.cycle = epoch // self.first_cycle_steps
-                else:
-                    n: int = int(
-                        math.log((epoch / self.first_cycle_steps * (self.cycle_mult - 1) + 1), self.cycle_mult)
-                    )
-                    self.cycle = n
-                    self.step_in_cycle = epoch - int(
-                        self.first_cycle_steps * (self.cycle_mult ** n - 1) / (self.cycle_mult - 1)
-                    )  # fmt: skip
-                    self.cur_cycle_steps = self.first_cycle_steps * self.cycle_mult ** n  # fmt: skip
+        elif epoch >= self.first_cycle_steps:
+            if self.cycle_mult == 1.0:
+                self.step_in_cycle = epoch % self.first_cycle_steps
+                self.cycle = epoch // self.first_cycle_steps
             else:
-                self.cur_cycle_steps = self.first_cycle_steps
-                self.step_in_cycle = epoch
+                n: int = int(math.log((epoch / self.first_cycle_steps * (self.cycle_mult - 1) + 1), self.cycle_mult))
+                self.cycle = n
+                self.step_in_cycle = epoch - int(
+                    self.first_cycle_steps * (self.cycle_mult ** n - 1) / (self.cycle_mult - 1)
+                )  # fmt: skip
+                self.cur_cycle_steps = self.first_cycle_steps * self.cycle_mult ** n  # fmt: skip
+        else:
+            self.cur_cycle_steps = self.first_cycle_steps
+            self.step_in_cycle = epoch
 
         self.max_lr = self.base_max_lr * (self.gamma ** self.cycle)  # fmt: skip
         self.last_epoch = math.floor(epoch)
 
         for param_group, lr in zip(self.optimizer.param_groups, self.get_lr()):
             param_group['lr'] = lr
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabelief.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adabound.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adafactor.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adai.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adamp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adams.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adams.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adan.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/adapnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/agc.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/agc.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/alig.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/apollo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/dadapt.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,19 +73,15 @@
         for group in self.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 state = self.state[p]
 
-                try:
-                    state['alpha_k'] = torch.full_like(p, fill_value=1e-6)
-                except NotImplementedError:  # there's no fill_() op for SpareTensorCPU
-                    state['alpha_k'] = torch.zeros_like(p)
-
+                state['alpha_k'] = torch.full_like(p, fill_value=1e-6)
                 state['sk'] = torch.zeros_like(p)
                 state['x0'] = torch.clone(p)
                 if p.grad.is_sparse:
                     state['weighted_sk'] = torch.zeros_like(p)
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
@@ -115,19 +111,15 @@
                 if p.grad is None:
                     continue
 
                 grad = p.grad
 
                 state = self.state[p]
                 if 'alpha_k' not in state:
-                    try:
-                        state['alpha_k'] = torch.full_like(p, fill_value=1e-6)
-                    except NotImplementedError:  # there's no fill_() op for SpareTensorCPU
-                        state['alpha_k'] = torch.zeros_like(p)
-
+                    state['alpha_k'] = torch.full_like(p, fill_value=1e-6)
                     state['sk'] = torch.zeros_like(p)
                     state['x0'] = torch.clone(p)
                     if grad.is_sparse:
                         state['weighted_sk'] = torch.zeros_like(p)
 
                 sk, alpha_k = state['sk'], state['alpha_k']
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/diffrgrad.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/diffrgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/fp16.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/gsam.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/gsam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/lookahead.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,126 @@
 from collections import defaultdict
 from typing import Dict
 
 import torch
-from torch.optim import Optimizer
 
 from pytorch_optimizer.base.optimizer import BaseOptimizer
-from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, OPTIMIZER, STATE
+from pytorch_optimizer.base.types import CLOSURE, LOSS, OPTIMIZER, STATE
 
 
-class Lookahead(Optimizer, BaseOptimizer):
+class Lookahead(BaseOptimizer):
     r"""k steps forward, 1 step back.
 
     :param optimizer: OPTIMIZER. base optimizer.
     :param k: int. number of lookahead steps.
     :param alpha: float. linear interpolation factor.
     :param pullback_momentum: str. change to inner optimizer momentum on interpolation update.
     """
 
-    def __init__(  # pylint: disable=super-init-not-called
+    def __init__(
         self,
         optimizer: OPTIMIZER,
         k: int = 5,
         alpha: float = 0.5,
         pullback_momentum: str = 'none',
     ):
         self.optimizer = optimizer
         self.k = k
         self.alpha = alpha
         self.pullback_momentum = pullback_momentum
 
         self.validate_parameters()
 
         self.param_groups = self.optimizer.param_groups
-        self.fast_state: STATE = self.optimizer.state
         self.state: STATE = defaultdict(dict)
-        self.reset()
 
-        self.defaults: DEFAULTS = optimizer.defaults
-        self.defaults.update(
-            {
-                'k': k,
-                'alpha': alpha,
-                'pullback_momentum': pullback_momentum,
-            }
-        )
+        for group in self.param_groups:
+            if 'counter' not in group:
+                group['counter'] = 0
+
+            for p in group['params']:
+                state = self.state[p]
+                state['slow_params'] = torch.empty_like(p)
+                state['slow_params'].copy_(p)
+                if self.pullback_momentum == 'pullback':
+                    state['slow_momentum'] = torch.zeros_like(p)
 
     def validate_parameters(self):
         self.validate_lookahead_k(self.k)
         self.validate_alpha(self.alpha)
         self.validate_pullback_momentum(self.pullback_momentum)
 
+    def __getstate__(self):
+        return {
+            'state': self.state,
+            'optimizer': self.optimizer,
+            'alpha': self.alpha,
+            'k': self.k,
+            'pullback_momentum': self.pullback_momentum,
+        }
+
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             group['counter'] = 0
 
+    def backup_and_load_cache(self):
+        r"""Backup cache parameters."""
+        for group in self.param_groups:
+            for p in group['params']:
+                state = self.state[p]
+                state['backup_params'] = torch.empty_like(p)
+                state['backup_params'].copy_(p)
+                p.data.copy_(state['slow_params'])
+
+    def clear_and_load_backup(self):
+        r"""Load backup parameters."""
+        for group in self.param_groups:
+            for p in group['params']:
+                state = self.state[p]
+                p.data.copy_(state['backup_params'])
+                del state['backup_params']
+
+    def state_dict(self) -> STATE:
+        return self.optimizer.state_dict()
+
+    def load_state_dict(self, state: STATE):
+        r"""Load state."""
+        self.optimizer.load_state_dict(state)
+
+    @torch.no_grad()
+    def zero_grad(self):
+        self.optimizer.zero_grad(set_to_none=True)
+
     @torch.no_grad()
     def update(self, group: Dict):
-        for fast in group['params']:
-            if fast.grad is None:
+        for p in group['params']:
+            if p.grad is None:
                 continue
 
-            param_state = self.state[fast]
-            if 'slow_param' not in param_state:
-                param_state['slow_param'] = torch.empty_like(fast)
-                param_state['slow_param'].copy_(fast)
-                if self.pullback_momentum == 'pullback':
-                    param_state['slow_mom'] = torch.zeros_like(fast)
+            state = self.state[p]
+
+            slow = state['slow_params']
 
-            slow = param_state['slow_param']
-            slow += (fast - slow) * self.alpha
-            fast.copy_(slow)
+            p.mul_(self.alpha).add_(slow, alpha=1.0 - self.alpha)
+            slow.copy_(p)
 
-            if 'momentum_buffer' not in self.optimizer.state[fast]:
-                self.optimizer.state[fast]['momentum_buffer'] = torch.zeros_like(fast)
+            if 'momentum_buffer' not in self.optimizer.state[p]:
+                self.optimizer.state[p]['momentum_buffer'] = torch.zeros_like(p)
 
             if self.pullback_momentum == 'pullback':
-                internal_momentum = self.optimizer.state[fast]['momentum_buffer']
-                self.optimizer.state[fast]['momentum_buffer'] = internal_momentum.mul_(self.alpha).add_(
-                    param_state['slow_mom'], alpha=1.0 - self.alpha
+                internal_momentum = self.optimizer.state[p]['momentum_buffer']
+                self.optimizer.state[p]['momentum_buffer'] = internal_momentum.mul_(self.alpha).add_(
+                    state['slow_momentum'], alpha=1.0 - self.alpha
                 )
-                param_state['slow_mom'] = self.optimizer.state[fast]['momentum_buffer']
+                state['slow_momentum'] = self.optimizer.state[p]['momentum_buffer']
             elif self.pullback_momentum == 'reset':
-                self.optimizer.state[fast]['momentum_buffer'] = torch.zeros_like(fast)
-
-    def update_lookahead(self):
-        for group in self.param_groups:
-            self.update(group)
+                self.optimizer.state[p]['momentum_buffer'] = torch.zeros_like(p)
 
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = self.optimizer.step(closure)
         for group in self.param_groups:
             group['counter'] += 1
             if group['counter'] >= self.k:
                 group['counter'] = 0
                 self.update(group)
         return loss
-
-    def state_dict(self) -> STATE:
-        fast_state_dict: STATE = self.optimizer.state_dict()
-        fast_state = fast_state_dict['state']
-        param_groups = fast_state_dict['param_groups']
-
-        slow_state: STATE = {(id(k) if isinstance(k, torch.Tensor) else k): v for k, v in self.state.items()}
-
-        return {
-            'fast_state': fast_state,
-            'slow_state': slow_state,
-            'param_groups': param_groups,
-        }
-
-    def load_state_dict(self, state_dict: STATE):
-        slow_state_dict: STATE = {
-            'state': state_dict['slow_state'],
-            'param_groups': state_dict['param_groups'],
-        }
-        fast_state_dict: STATE = {
-            'state': state_dict['fast_state'],
-            'param_groups': state_dict['param_groups'],
-        }
-        super().load_state_dict(slow_state_dict)
-
-        self.optimizer.load_state_dict(fast_state_dict)
-        self.fast_state = self.optimizer.state
-
-    def add_param_group(self, param_group):
-        param_group['counter'] = 0
-        self.optimizer.add_param_group(param_group)
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/madgrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,32 +65,28 @@
                 state['grad_sum_sq'] = torch.zeros_like(p)
                 state['s'] = torch.zeros_like(p)
                 if group['momentum'] > 0.0:
                     state['x0'] = torch.clone(p).detach()
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
-        # pylint: disable=W0212
-
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         # step counter must be stored in state to ensure correct behavior under optimizer sharding
         if 'k' not in self.state:
             self.state['k'] = torch.tensor([0], dtype=torch.long, requires_grad=False)
 
-        k = self.state['k']
-
         for group in self.param_groups:
             weight_decay, momentum, eps = group['weight_decay'], group['momentum'], group['eps']
             lr = group['lr'] + eps
 
-            _lambda = lr * math.pow(k + 1, 0.5)
+            _lambda = lr * math.pow(self.state['k'] + 1, 0.5)
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 state = self.state[p]
@@ -101,34 +97,31 @@
                     if momentum > 0.0:
                         state['x0'] = torch.clone(p).detach()
 
                 if momentum > 0.0 and grad.is_sparse:
                     raise NoSparseGradientError(str(self), note='momentum > 0.0')
 
                 grad_sum_sq, s = state['grad_sum_sq'], state['s']
-
                 if weight_decay > 0.0 and not self.decouple_decay:
                     if grad.is_sparse:
                         raise NoSparseGradientError(str(self), note='weight_decay')
 
                     # original implementation. not AdamW style
                     grad.add_(p, alpha=weight_decay)
 
                 if grad.is_sparse:
                     grad = grad.coalesce()
 
                     p_masked = p.sparse_mask(grad)
                     grad_sum_sq_masked = grad_sum_sq.sparse_mask(grad)
                     s_masked = s.sparse_mask(grad)
 
-                    # Compute x_0 from other known quantities
                     rms_masked_values = grad_sum_sq_masked._values().pow(1 / 3).add_(eps)
                     x0_masked_values = p_masked._values().addcdiv(s_masked._values(), rms_masked_values, value=1)
 
-                    # Dense + sparse op
                     grad_sq = grad * grad
                     grad_sum_sq.add_(grad_sq, alpha=_lambda)
                     grad_sum_sq_masked.add_(grad_sq, alpha=_lambda)
 
                     rms_masked_values = grad_sum_sq_masked._values().pow_(1 / 3).add_(eps)
                     if eps == 0.0:
                         rms_masked_values[rms_masked_values == 0] = float('inf')
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/nero.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,39 +10,44 @@
 class Nero(Optimizer, BaseOptimizer):
     """Learning by Turning: Neural Architecture Aware Optimisation.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param beta: float. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param constraints: bool.
+    :param eps: float. term added to the denominator to improve numerical stability.
     """
 
-    def __init__(self, params: PARAMETERS, lr: float = 0.01, beta: float = 0.999, constraints: bool = True):
+    def __init__(
+        self, params: PARAMETERS, lr: float = 0.01, beta: float = 0.999, constraints: bool = True, eps: float = 1e-8
+    ):
         self.lr = lr
         self.beta = beta
+        self.eps = eps
 
         self.validate_parameters()
 
         defaults: DEFAULTS = {'lr': lr, 'constraints': constraints}
         super().__init__(params, defaults)
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_beta(self.beta)
+        self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
         return 'Nero'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
             for p in group['params']:
                 if group['constraints'] and p.dim() > 1:
                     p.sub_(neuron_mean(p))
-                    p.div_(neuron_norm(p))
+                    p.div_(neuron_norm(p) + self.eps)
 
                 state = self.state[p]
 
                 state['step'] = 0
                 state['exp_avg_sq'] = torch.zeros_like(neuron_norm(p))
                 state['scale'] = neuron_norm(p).mean()
 
@@ -65,30 +70,34 @@
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
                 if len(state) == 0:
                     if group['constraints'] and p.dim() > 1:
                         p.sub_(neuron_mean(p))
-                        p.div_(neuron_norm(p))
+                        p.div_(neuron_norm(p) + self.eps)
 
                     state['step'] = 0
                     state['exp_avg_sq'] = torch.zeros_like(neuron_norm(p))
                     state['scale'] = neuron_norm(p).mean()
                     if state['scale'] == 0.0:
                         state['scale'] = 0.01
 
                 state['step'] += 1
 
+                grad_norm = neuron_norm(grad)
+
+                exp_avg_sq = state['exp_avg_sq']
+                exp_avg_sq.mul_(self.beta).addcmul_(grad_norm, grad_norm, value=1.0 - self.beta)
+
                 bias_correction: float = 1.0 - self.beta ** state['step']
-                state['exp_avg_sq'] = self.beta * state['exp_avg_sq'] + (1.0 - self.beta) * neuron_norm(grad) ** 2
 
-                grad_normed = grad / (state['exp_avg_sq'] / bias_correction).sqrt()
-                grad_normed[torch.isnan(grad_normed)] = 0.0
+                grad_normed = grad / ((exp_avg_sq / bias_correction).sqrt() + self.eps)
+                torch.nan_to_num(grad_normed, nan=0.0, out=grad_normed)
 
                 p.sub_(group['lr'] * state['scale'] * grad_normed)
 
                 if group['constraints'] and p.dim() > 1:
                     p.sub_(neuron_mean(p))
-                    p.div_(neuron_norm(p))
+                    p.div_(neuron_norm(p) + self.eps)
 
         return loss
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/novograd.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/novograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         idx: int = 0
         for group in self.optimizer.param_groups:
             for p in group['params']:
                 p.grad = grads[idx]
                 idx += 1
 
     def retrieve_grad(self) -> Tuple[List[torch.Tensor], List[int], List[torch.Tensor]]:
-        r"""get the gradient of the parameters of the network with specific objective."""
+        r"""Get the gradient of the parameters of the network with specific objective."""
         grad, shape, has_grad = [], [], []
         for group in self.optimizer.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     shape.append(p.shape)
                     grad.append(torch.zeros_like(p, device=p.device))
                     has_grad.append(torch.zeros_like(p, device=p.device))
@@ -57,15 +57,15 @@
                 shape.append(p.grad.shape)
                 grad.append(p.grad.clone())
                 has_grad.append(torch.ones_like(p, device=p.device))
 
         return grad, shape, has_grad
 
     def pack_grad(self, objectives: Iterable) -> Tuple[List[torch.Tensor], List[List[int]], List[torch.Tensor]]:
-        r"""pack the gradient of the parameters of the network for each objective.
+        r"""Pack the gradient of the parameters of the network for each objective.
 
         :param objectives: Iterable[nn.Module]. a list of objectives.
         :return: torch.Tensor. packed gradients.
         """
         grads, shapes, has_grads = [], [], []
         for objective in objectives:
             self.optimizer.zero_grad(set_to_none=True)
@@ -76,44 +76,44 @@
             grads.append(flatten_grad(grad))
             has_grads.append(flatten_grad(has_grad))
             shapes.append(shape)
 
         return grads, shapes, has_grads
 
     def project_conflicting(self, grads: List[torch.Tensor], has_grads: List[torch.Tensor]) -> torch.Tensor:
-        r"""project conflicting.
+        r"""Project conflicting.
 
         :param grads: a list of the gradient of the parameters.
         :param has_grads: a list of mask represent whether the parameter has gradient.
         :return: torch.Tensor. merged gradients.
         """
         shared: torch.Tensor = torch.stack(has_grads).prod(0).bool()
 
         pc_grad: List[torch.Tensor] = deepcopy(grads)
-        for g_i in pc_grad:
+        for i, g_i in enumerate(pc_grad):
             random.shuffle(grads)
             for g_j in grads:
                 g_i_g_j: torch.Tensor = torch.dot(g_i, g_j)
                 if g_i_g_j < 0:
-                    g_i -= g_i_g_j * g_j / (g_j.norm() ** 2)
+                    pc_grad[i] -= g_i_g_j * g_j / (g_j.norm() ** 2)
 
         merged_grad: torch.Tensor = torch.zeros_like(grads[0], device=grads[0].device)
 
         shared_pc_gradients: torch.Tensor = torch.stack([g[shared] for g in pc_grad])
         if self.reduction == 'mean':
             merged_grad[shared] = shared_pc_gradients.mean(dim=0)
         else:
             merged_grad[shared] = shared_pc_gradients.sum(dim=0)
 
         merged_grad[~shared] = torch.stack([g[~shared] for g in pc_grad]).sum(dim=0)
 
         return merged_grad
 
     def pc_backward(self, objectives: Iterable[nn.Module]):
-        r"""calculate the gradient of the parameters.
+        r"""Calculate the gradient of the parameters.
 
         :param objectives: Iterable[nn.Module]. a list of objectives.
         """
         grads, shapes, has_grads = self.pack_grad(objectives)
 
         pc_grad = self.project_conflicting(grads, has_grads)
         pc_grad = un_flatten_grad(pc_grad, shapes[0])
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/pnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/ralamb.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ralamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/ranger.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/ranger21.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from typing import Optional
 
 import torch
 from torch.nn import functional as f
 from torch.optim import Optimizer
 
-from pytorch_optimizer.base.exception import NegativeLRError, NoSparseGradientError, ZeroParameterSizeError
+from pytorch_optimizer.base.exception import NoSparseGradientError, ZeroParameterSizeError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 from pytorch_optimizer.optimizer.agc import agc
 from pytorch_optimizer.optimizer.gc import centralize_gradient
 from pytorch_optimizer.optimizer.utils import normalize_gradient, unit_norm
 
 
@@ -69,14 +69,15 @@
         lookahead_blending_alpha: float = 0.5,
         weight_decay: float = 1e-4,
         norm_loss_factor: float = 1e-4,
         adamd_debias_term: bool = False,
         eps: float = 1e-8,
     ):
         self.lr = lr
+        self.min_lr = warm_down_min_lr
         self.beta0 = beta0
         self.betas = betas
         self.use_softplus = use_softplus
         self.beta_softplus = beta_softplus
         self.agc_clipping_value = agc_clipping_value
         self.agc_eps = agc_eps
         self.centralize_gradients = centralize_gradients
@@ -92,15 +93,14 @@
 
         # lookahead
         self.lookahead_step: int = 0
 
         # learning rate
         self.starting_lr = lr
         self.current_lr = lr
-        self.min_lr = warm_down_min_lr
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'adamd_debias_term': adamd_debias_term,
             'eps': eps,
@@ -119,14 +119,15 @@
             else num_warm_down_iterations
         )
         self.start_warm_down: int = num_iterations - self.num_warm_down_iterations
         self.warm_down_lr_delta: float = self.starting_lr - self.min_lr
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
+        self.validate_learning_rate(self.min_lr)
         self.validate_betas(self.betas)
         self.validate_beta0(self.beta0)
         self.validate_weight_decay(self.weight_decay)
         self.validate_epsilon(self.eps)
 
     def __str__(self) -> str:
         return 'Ranger21'
@@ -165,27 +166,28 @@
         warm_up_current_pct: float = min(1.0, (step / self.num_warm_up_iterations))
 
         new_lr: float = lr * warm_up_current_pct
         self.current_lr = new_lr
 
         return new_lr
 
-    def get_warm_down(self, lr: float, iteration: int) -> float:
+    def warm_down(self, lr: float, iteration: int) -> float:
         if iteration < self.start_warm_down:
             return lr
 
         # start iteration from 1, not 0
         warm_down_iteration: int = (iteration + 1) - self.start_warm_down
         warm_down_iteration = max(warm_down_iteration, 1)
 
         warm_down_pct: float = warm_down_iteration / (self.num_warm_down_iterations + 1)
         warm_down_pct = min(warm_down_pct, 1.0)
 
         new_lr: float = self.starting_lr - self.warm_down_lr_delta * warm_down_pct
         new_lr = max(new_lr, self.min_lr)
+
         self.current_lr = new_lr
 
         return new_lr
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
@@ -194,100 +196,90 @@
                 loss = closure()
 
         param_size: int = 0
         variance_ma_sum: float = 1.0
 
         # Phase 1 - Accumulate all the variance_ma_sum to use in stable weight decay
         for group in self.param_groups:
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
             beta1, beta2 = group['betas']
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 param_size += p.numel()
 
                 # Apply Adaptive Gradient Clipping (AGC)
-                p = agc(p, agc_eps=self.agc_eps, agc_clip_val=self.agc_clipping_value)
+                p = agc(p, agc_eps=self.agc_eps, agc_clip_val=self.agc_clipping_value)  # noqa: PLW2901
 
                 state = self.state[p]
                 if len(state) == 0:
-                    state['step'] = 0
                     state['grad_ma'] = torch.zeros_like(p)
                     state['variance_ma'] = torch.zeros_like(p)
                     state['lookahead_params'] = torch.empty_like(p)
                     state['lookahead_params'].copy_(p)
                     state['neg_grad_ma'] = torch.zeros_like(p)
                     state['max_variance_ma'] = torch.zeros_like(p)
 
                 # Apply GC & GradNorm
                 # TODO : Gradient Clipping (Norm)
                 grad = centralize_gradient(grad, gc_conv_only=False)
                 grad = normalize_gradient(grad)
 
-                state['step'] += 1
-
-                bias_correction2 = 1.0 - beta2 ** state['step']
+                bias_correction2 = 1.0 - beta2 ** group['step']
 
                 # second moment estimation
                 # using positive-negative momentum and bias correction
                 variance_ma = state['variance_ma']
                 variance_ma.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
                 variance_ma_sum += (variance_ma / bias_correction2).sum()
 
-        # stable weight decay
         if param_size == 0:
             raise ZeroParameterSizeError()
 
         variance_normalized = math.sqrt(variance_ma_sum / param_size)
         if math.isnan(variance_normalized):
             raise RuntimeError('hit nan for variance_normalized')
 
         # Phase 2 - Apply weight decay and step
         for group in self.param_groups:
-            p = group['params'][0]
-            if p.grad is None:
-                continue
-
             lr = group['lr']
-            step = self.state[group['params'][0]]['step']
-
             beta1, beta2 = group['betas']
-            bias_correction1 = 1.0 - beta1 ** step  # fmt: skip
-            bias_correction2_sq = math.sqrt(1.0 - beta2 ** step)  # fmt: skip
 
-            noise_norm: float = math.sqrt((1.0 + beta2) ** 2 + beta2 ** 2)  # fmt: skip
+            bias_correction1 = 1.0 - beta1 ** group['step']  # fmt: skip
+            bias_correction2_sq = math.sqrt(1.0 - beta2 ** group['step'])  # fmt: skip
 
-            # warm up
-            lr = self.warm_up_dampening(lr, step)
+            noise_norm: float = math.sqrt((1.0 + beta2) ** 2 + beta2 ** 2)  # fmt: skip
 
-            # warm down
-            lr = self.get_warm_down(lr, step)
-            if lr < 0.0:
-                raise NegativeLRError(lr)
-
-            # stable decay
-            decay = group['weight_decay']
-            if decay:
-                p.mul_(1.0 - decay * lr / variance_normalized)
-
-            # norm loss
-            u_norm = unit_norm(p)
-            correction = 2.0 * self.norm_loss_factor * (1.0 - torch.div(1, u_norm + self.eps))
-            p.mul_(1.0 - lr * correction)
+            # warm up & down
+            lr = self.warm_up_dampening(lr, group['step'])
+            lr = self.warm_down(lr, group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
+                # stable weight decay
+                if group['weight_decay']:
+                    p.mul_(1.0 - group['weight_decay'] * lr / variance_normalized)
+
+                # norm loss
+                correction = 2.0 * self.norm_loss_factor * (1.0 - torch.div(1, unit_norm(p) + self.eps))
+                p.mul_(1.0 - lr * correction)
+
                 state = self.state[p]
-                if state['step'] % 2 == 1:
+                if group['step'] % 2 == 1:
                     grad_ma, neg_grad_ma = state['grad_ma'], state['neg_grad_ma']
                 else:
                     grad_ma, neg_grad_ma = state['neg_grad_ma'], state['grad_ma']
 
                 variance_ma = state['variance_ma']
 
                 torch.max(state['max_variance_ma'], variance_ma, out=variance_ma)
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/sam.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/sgdp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             else:
                 split_sizes.append(np.array([d], dtype=np.int32))
 
         self.num_splits: int = len(split_sizes)
         self.pre_conditioner_shapes: List[List[int]] = []
         for t in itertools.product(*split_sizes):
             if not (pre_conditioner_type == PreConditionerType.ALL or self.num_splits <= 1):
-                t = t[:-1]
+                t = t[:-1]  # noqa: PLW2901
             self.pre_conditioner_shapes.extend([[d, d] for d in t])
 
     def shapes_for_pre_conditioners(self) -> List[List[int]]:
         r"""Get shapes of pre-conditioner."""
         return self.pre_conditioner_shapes
 
     def partition(self, x: torch.Tensor) -> List[torch.Tensor]:
@@ -255,15 +255,15 @@
             self.is_same_shapes = len(np.unique(shapes)) == 1
 
         if self.is_same_shapes:
             self.statistics = torch.stack(self.statistics)
             self.pre_conditioners = torch.stack(self.pre_conditioners)
 
     def skip_precondition(self, x: torch.Tensor) -> bool:
-        return (len(x.shape) < 1) or any([s > self.no_preconditioning_for_layers_with_dim_gt for s in x.shape])
+        return (len(x.shape) < 1) or any(s > self.no_preconditioning_for_layers_with_dim_gt for s in x.shape)
 
     def add_statistics(self, grad: torch.Tensor):
         r"""Compute statistics from gradients and add to the correct state entries.
 
         :param grad: torch.Tensor. gradient to compute statistics from.
         """
         if len(self.statistics) == 0:
@@ -353,15 +353,15 @@
 
         Compute the maximum eigenvalue of mat, for scaling. v is a random (uniform) vector with values in (-1, 1).
 
     :param mat_g: torch.Tensor. the symmetric PSD matrix.
     :param error_tolerance: float. Iterative exit condition.
     :param num_iters: int. Number of iterations.
     """
-    v: torch.Tensor = 2.0 * torch.rand(list(mat_g.shape)[0], dtype=mat_g.dtype, device=mat_g.device) - 1
+    v = 2.0 * torch.rand(list(mat_g.shape)[0], dtype=mat_g.dtype, device=mat_g.device) - 1
 
     error: Union[torch.Tensor, float] = 1.0
     iters: int = 0
     singular_val: Union[torch.Tensor, float] = 0.0
     while error > error_tolerance and iters < num_iters:
         v.div_(v.norm())
         mat_v = torch.mv(mat_g, v)
@@ -454,15 +454,15 @@
 
     z = (1 + p) / (2 * torch.norm(mat_g))
 
     mat_root = identity * torch.pow(z, 1.0 / p)
     mat_m = mat_g * z
 
     alpha: float = -1.0 / p
-    alpha_identity: torch.Tensor = (1.0 - alpha) * identity
+    alpha_identity = (1.0 - alpha) * identity
     error = torch.max(torch.abs(mat_m - identity))
     count: int = 0
     while error > error_tolerance and count < iter_count:
         mat_m_i = alpha_identity + alpha * mat_m
         new_mat_root = torch.matmul(mat_root, mat_m_i).float()
         mat_m = torch.matmul(matrix_power(mat_m_i, p), mat_m).float()
```

### Comparing `pytorch_optimizer-2.5.1/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-2.5.2/pytorch_optimizer/optimizer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,29 +195,27 @@
 
 
 def neuron_norm(x: torch.Tensor) -> torch.Tensor:
     r"""Get norm of the tensor."""
     if x.dim() <= 1:
         return x.abs()
 
-    view_shape = [x.shape[0]] + [1] * (x.dim() - 1)
-    x = x.view(x.shape[0], -1)
+    view_shape: List[int] = [x.shape[0]] + [1] * (x.dim() - 1)
 
-    return x.norm(dim=1).view(*view_shape)
+    return channel_view(x).norm(dim=1).view(*view_shape)
 
 
 def neuron_mean(x: torch.Tensor) -> torch.Tensor:
     r"""Get mean of the tensor."""
     if x.dim() <= 1:
         raise ValueError('[-] neuron_mean not defined on 1D tensors.')
 
-    view_shape = [x.shape[0]] + [1] * (x.dim() - 1)
-    x = x.view(x.shape[0], -1)
+    view_shape: List[int] = [x.shape[0]] + [1] * (x.dim() - 1)
 
-    return x.mean(dim=1).view(*view_shape)
+    return channel_view(x).mean(dim=1).view(*view_shape)
 
 
 def disable_running_stats(model):
     r"""Disable running stats (momentum) of BatchNorm."""
 
     def _disable(module):
         if isinstance(module, _BatchNorm):
@@ -240,8 +238,8 @@
 @torch.no_grad()
 def l2_projection(parameters: PARAMETERS, max_norm: float = 1e2):
     r"""Get l2 normalized parameter."""
     global_norm = torch.sqrt(sum(p.norm().pow(2) for p in parameters))
     if global_norm > max_norm:
         ratio = max_norm / global_norm
         for param in parameters:
-            param *= ratio
+            param *= ratio  # noqa: PLW2901
```

### Comparing `pytorch_optimizer-2.5.1/PKG-INFO` & `pytorch_optimizer-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-optimizer
-Version: 2.5.1
+Version: 2.5.2
 Summary: optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas.
 Home-page: https://github.com/kozistr/pytorch_optimizer
 License: Apache-2.0
 Keywords: pytorch,deep-learning,optimizer,lr scheduler
 Author: kozistr
 Author-email: kozistr@gmail.com
 Maintainer: kozistr
@@ -31,15 +31,16 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: numpy (==1.21.1) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: numpy ; python_version >= "3.8"
-Requires-Dist: torch (>=1.10)
+Requires-Dist: torch (>=1.10,<2.0) ; python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: torch (>=2.0) ; python_version >= "3.8"
 Project-URL: Documentation, https://pytorch-optimizers.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/kozistr/pytorch_optimizer
 Description-Content-Type: text/x-rst
 
 =================
 pytorch-optimizer
 =================
```

