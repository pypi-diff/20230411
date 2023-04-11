# Comparing `tmp/alethiometer-1.0.3.tar.gz` & `tmp/alethiometer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.0.3.tar", last modified: Tue Apr 11 12:17:54 2023, max compression
+gzip compressed data, was "alethiometer-1.0.4.tar", last modified: Tue Apr 11 12:56:24 2023, max compression
```

## Comparing `alethiometer-1.0.3.tar` & `alethiometer-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.053321 alethiometer-1.0.3/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.3/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1521 2023-04-11 12:17:54.053321 alethiometer-1.0.3/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      812 2023-04-11 12:16:45.000000 alethiometer-1.0.3/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.049321 alethiometer-1.0.3/alethiometer/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.3/alethiometer/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-11 12:12:58.000000 alethiometer-1.0.3/alethiometer/__version__.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.053321 alethiometer-1.0.3/alethiometer/datasets/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.3/alethiometer/datasets/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4252 2023-04-07 18:02:54.000000 alethiometer-1.0.3/alethiometer/datasets/dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.3/alethiometer/datasets/h5py_dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.3/alethiometer/datasets/imagenet16.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.3/alethiometer/utils.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2445 2023-04-11 12:11:31.000000 alethiometer-1.0.3/alethiometer/zc_proxy.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.053321 alethiometer-1.0.3/alethiometer/zero_cost_metrics/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1162 2023-04-07 15:02:02.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/grad_norm.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/grasp.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/snip.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.3/alethiometer/zero_cost_metrics/synflow.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:17:54.049321 alethiometer-1.0.3/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1521 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      654 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-11 12:17:54.000000 alethiometer-1.0.3/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-11 12:17:54.053321 alethiometer-1.0.3/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.3/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.4/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1578 2023-04-11 12:56:24.207460 alethiometer-1.0.4/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      869 2023-04-11 12:55:39.000000 alethiometer-1.0.4/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.4/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-11 12:55:03.000000 alethiometer-1.0.4/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.4/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4252 2023-04-07 18:02:54.000000 alethiometer-1.0.4/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.4/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.4/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.4/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2999 2023-04-11 12:50:22.000000 alethiometer-1.0.4/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1327 2023-04-11 12:38:17.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/synflow.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1578 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      654 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-11 12:56:24.207460 alethiometer-1.0.4/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.4/setup.py
```

### Comparing `alethiometer-1.0.3/LICENSE` & `alethiometer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/PKG-INFO` & `alethiometer-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.0.3
+Version: 1.0.4
 Summary: ZC proxies calculation repo, altered from foresight package.
 Home-page: https://github.com/iViolinSolo/zero-cost-proxies
 Author: ViolinSolo
 Author-email: i.violinsolo@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-04-11 13:16:45
+ * @LastEditTime: 2023-04-11 13:55:39
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -42,10 +42,12 @@
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.0.4  
+fix bugs in calculation, add more test codes.
 - V1.0.3  
 add shortcuts to import directly from package root directory.
```

### Comparing `alethiometer-1.0.3/alethiometer/datasets/dataset.py` & `alethiometer-1.0.4/alethiometer/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer/datasets/h5py_dataset.py` & `alethiometer-1.0.4/alethiometer/datasets/h5py_dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer/datasets/imagenet16.py` & `alethiometer-1.0.4/alethiometer/datasets/imagenet16.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer/utils.py` & `alethiometer-1.0.4/alethiometer/utils.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer/zc_proxy.py` & `alethiometer-1.0.4/alethiometer/zc_proxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 18:35:04
-LastEditTime: 2023-04-11 13:11:30
+LastEditTime: 2023-04-11 13:49:23
 LastEditors: ViolinSolo
 Description: entry program
 FilePath: /zero-cost-proxies/alethiometer/zc_proxy.py
 '''
 import types
 import copy
 import torch
@@ -52,15 +52,15 @@
     done, ds = False, 1
     metric_vals = {}
 
     while not done:
         try:
             for mt_name in metric_names:
                 if mt_name not in metric_vals:
-                    val = M.calc_measure(mt_name, net_orig, device, inputs, targets, loss_fn=loss_fn, split_data=ds)
+                    val = M.calc_metric(mt_name, net_orig, device, inputs, targets, loss_fn=loss_fn, split_data=ds)
                     metric_vals[mt_name] = val
 
             done = True
         except RuntimeError as e:
             if 'out of memory' in str(e):
                 done=False
                 if ds == inputs.shape[0]//2:
@@ -73,15 +73,29 @@
             else:
                 raise e
 
     net_orig = net_orig.to(device).train()
     return metric_vals
 
 
-def calc_zc_metrics(metrics: list, model: nn.Module, train_queue: D.DataLoader, device: torch.device, loss_fn=F.cross_entropy):
+def calc_zc_metrics(metrics: list, model: nn.Module, train_queue: D.DataLoader, device: torch.device, loss_fn=F.cross_entropy, aggregate=True):
     """
-    Purpose: metrics
+    Purpose: metrics calculation entry.
+    @param: train_queue: train dataset dataloader.
+    @param: aggregate: whether return original layerwise value, when true, return processed aggregated value.
+
+    @return: dict of values, key is metric name of @params metrics, value is the calculated zcmetric result, 
     """
     mt_vals = calc_vals(net_orig=model, trainloader=train_queue, device=device, metric_names=metrics, loss_fn=loss_fn)
 
-    return mt_vals
+    def sum_arr(arr):
+        sum = 0.
+        for i in range(len(arr)):
+            sum += torch.sum(arr[i])
+        return sum.item()
+    
+    results = {}
+    for k, v in mt_vals.items():
+        results[k] = v if not aggregate else sum_arr(v)
+
+    return results
 # end def
```

### Comparing `alethiometer-1.0.3/alethiometer/zero_cost_metrics/__init__.py` & `alethiometer-1.0.4/alethiometer/zero_cost_metrics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 17:43:34
-LastEditTime: 2023-04-07 16:02:02
+LastEditTime: 2023-04-11 13:37:59
 LastEditors: ViolinSolo
 Description: init files 
 FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/__init__.py
 '''
 
 import gc
 import torch
@@ -35,7 +35,13 @@
         return func
     return make_impl
 
 
 def calc_metric(name, net, device, *args, **kwargs):
     return _metric_impls[name](net, device, *args, **kwargs)
 
+
+# using the following import to trigger metric registration when using @metric
+from . import snip
+from . import synflow
+from . import grasp
+from . import grad_norm
```

### Comparing `alethiometer-1.0.3/alethiometer/zero_cost_metrics/grad_norm.py` & `alethiometer-1.0.4/alethiometer/zero_cost_metrics/grad_norm.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer/zero_cost_metrics/grasp.py` & `alethiometer-1.0.4/alethiometer/zero_cost_metrics/grasp.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer/zero_cost_metrics/snip.py` & `alethiometer-1.0.4/alethiometer/zero_cost_metrics/snip.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer/zero_cost_metrics/synflow.py` & `alethiometer-1.0.4/alethiometer/zero_cost_metrics/synflow.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/alethiometer.egg-info/PKG-INFO` & `alethiometer-1.0.4/alethiometer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.0.3
+Version: 1.0.4
 Summary: ZC proxies calculation repo, altered from foresight package.
 Home-page: https://github.com/iViolinSolo/zero-cost-proxies
 Author: ViolinSolo
 Author-email: i.violinsolo@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-04-11 13:16:45
+ * @LastEditTime: 2023-04-11 13:55:39
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -42,10 +42,12 @@
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.0.4  
+fix bugs in calculation, add more test codes.
 - V1.0.3  
 add shortcuts to import directly from package root directory.
```

### Comparing `alethiometer-1.0.3/alethiometer.egg-info/SOURCES.txt` & `alethiometer-1.0.4/alethiometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.3/setup.py` & `alethiometer-1.0.4/setup.py`

 * *Files identical despite different names*

