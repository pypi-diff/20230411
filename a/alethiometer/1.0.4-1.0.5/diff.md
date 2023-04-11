# Comparing `tmp/alethiometer-1.0.4.tar.gz` & `tmp/alethiometer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.0.4.tar", last modified: Tue Apr 11 12:56:24 2023, max compression
+gzip compressed data, was "alethiometer-1.0.5.tar", last modified: Tue Apr 11 16:59:22 2023, max compression
```

## Comparing `alethiometer-1.0.4.tar` & `alethiometer-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.4/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1578 2023-04-11 12:56:24.207460 alethiometer-1.0.4/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      869 2023-04-11 12:55:39.000000 alethiometer-1.0.4/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.4/alethiometer/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-11 12:55:03.000000 alethiometer-1.0.4/alethiometer/__version__.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer/datasets/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.4/alethiometer/datasets/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4252 2023-04-07 18:02:54.000000 alethiometer-1.0.4/alethiometer/datasets/dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.4/alethiometer/datasets/h5py_dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.4/alethiometer/datasets/imagenet16.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.4/alethiometer/utils.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2999 2023-04-11 12:50:22.000000 alethiometer-1.0.4/alethiometer/zc_proxy.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer/zero_cost_metrics/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1327 2023-04-11 12:38:17.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/grad_norm.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/grasp.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/snip.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.4/alethiometer/zero_cost_metrics/synflow.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 12:56:24.207460 alethiometer-1.0.4/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1578 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      654 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-11 12:56:24.000000 alethiometer-1.0.4/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-11 12:56:24.207460 alethiometer-1.0.4/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.4/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.5/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-11 16:59:22.216346 alethiometer-1.0.5/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      951 2023-04-11 15:49:09.000000 alethiometer-1.0.5/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.5/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-11 15:47:53.000000 alethiometer-1.0.5/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.5/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4252 2023-04-07 18:02:54.000000 alethiometer-1.0.5/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.5/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.5/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.5/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3223 2023-04-11 16:58:07.000000 alethiometer-1.0.5/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1348 2023-04-11 15:46:48.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/naswot.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.5/alethiometer/zero_cost_metrics/synflow.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-11 16:59:22.216346 alethiometer-1.0.5/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      695 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-11 16:59:22.000000 alethiometer-1.0.5/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-11 16:59:22.216346 alethiometer-1.0.5/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.5/setup.py
```

### Comparing `alethiometer-1.0.4/LICENSE` & `alethiometer-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/PKG-INFO` & `alethiometer-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.0.4
+Version: 1.0.5
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
- * @LastEditTime: 2023-04-11 13:55:39
+ * @LastEditTime: 2023-04-11 16:49:09
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -32,22 +32,26 @@
 
 Supported zc-metrics are:
 ```
 grad_norm,
 grasp,
 snip,
 synflow,
+nwot, (NASWOT)
+lnwot, (Layerwise NASWOT)
 ```
 
 
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.0.6  
+add `naswot, lnwot` into mats
 - V1.0.4  
 fix bugs in calculation, add more test codes.
 - V1.0.3  
 add shortcuts to import directly from package root directory.
```

### Comparing `alethiometer-1.0.4/README.md` & `alethiometer-1.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-04-11 13:55:39
+ * @LastEditTime: 2023-04-11 16:49:09
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -13,22 +13,26 @@
 
 Supported zc-metrics are:
 ```
 grad_norm,
 grasp,
 snip,
 synflow,
+nwot, (NASWOT)
+lnwot, (Layerwise NASWOT)
 ```
 
 
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.0.6  
+add `naswot, lnwot` into mats
 - V1.0.4  
 fix bugs in calculation, add more test codes.
 - V1.0.3  
 add shortcuts to import directly from package root directory.
```

### Comparing `alethiometer-1.0.4/alethiometer/datasets/dataset.py` & `alethiometer-1.0.5/alethiometer/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer/datasets/h5py_dataset.py` & `alethiometer-1.0.5/alethiometer/datasets/h5py_dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer/datasets/imagenet16.py` & `alethiometer-1.0.5/alethiometer/datasets/imagenet16.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer/utils.py` & `alethiometer-1.0.5/alethiometer/utils.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer/zc_proxy.py` & `alethiometer-1.0.5/alethiometer/zc_proxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 18:35:04
-LastEditTime: 2023-04-11 13:49:23
+LastEditTime: 2023-04-11 17:57:53
 LastEditors: ViolinSolo
 Description: entry program
 FilePath: /zero-cost-proxies/alethiometer/zc_proxy.py
 '''
 import types
 import copy
 import torch
@@ -85,16 +85,21 @@
 
     @return: dict of values, key is metric name of @params metrics, value is the calculated zcmetric result, 
     """
     mt_vals = calc_vals(net_orig=model, trainloader=train_queue, device=device, metric_names=metrics, loss_fn=loss_fn)
 
     def sum_arr(arr):
         sum = 0.
-        for i in range(len(arr)):
-            sum += torch.sum(arr[i])
+        if hasattr(arr, '__len__'):  # ignore some cases like str or tuple.
+            for i in range(len(arr)):
+                val = arr[i]
+                val = val if type(val) is torch.Tensor else torch.tensor(val)
+                sum += torch.sum(val)
+        else:
+            sum = arr
         return sum.item()
     
     results = {}
     for k, v in mt_vals.items():
         results[k] = v if not aggregate else sum_arr(v)
 
     return results
```

### Comparing `alethiometer-1.0.4/alethiometer/zero_cost_metrics/__init__.py` & `alethiometer-1.0.5/alethiometer/zero_cost_metrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 17:43:34
-LastEditTime: 2023-04-11 13:37:59
+LastEditTime: 2023-04-11 16:46:48
 LastEditors: ViolinSolo
 Description: init files 
 FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/__init__.py
 '''
 
 import gc
 import torch
@@ -41,7 +41,8 @@
 
 
 # using the following import to trigger metric registration when using @metric
 from . import snip
 from . import synflow
 from . import grasp
 from . import grad_norm
+from . import naswot
```

### Comparing `alethiometer-1.0.4/alethiometer/zero_cost_metrics/grad_norm.py` & `alethiometer-1.0.5/alethiometer/zero_cost_metrics/grad_norm.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer/zero_cost_metrics/grasp.py` & `alethiometer-1.0.5/alethiometer/zero_cost_metrics/grasp.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer/zero_cost_metrics/snip.py` & `alethiometer-1.0.5/alethiometer/zero_cost_metrics/snip.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer/zero_cost_metrics/synflow.py` & `alethiometer-1.0.5/alethiometer/zero_cost_metrics/synflow.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.4/alethiometer.egg-info/PKG-INFO` & `alethiometer-1.0.5/alethiometer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.0.4
+Version: 1.0.5
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
- * @LastEditTime: 2023-04-11 13:55:39
+ * @LastEditTime: 2023-04-11 16:49:09
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -32,22 +32,26 @@
 
 Supported zc-metrics are:
 ```
 grad_norm,
 grasp,
 snip,
 synflow,
+nwot, (NASWOT)
+lnwot, (Layerwise NASWOT)
 ```
 
 
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
+- V1.0.6  
+add `naswot, lnwot` into mats
 - V1.0.4  
 fix bugs in calculation, add more test codes.
 - V1.0.3  
 add shortcuts to import directly from package root directory.
```

### Comparing `alethiometer-1.0.4/alethiometer.egg-info/SOURCES.txt` & `alethiometer-1.0.5/alethiometer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 alethiometer/datasets/__init__.py
 alethiometer/datasets/dataset.py
 alethiometer/datasets/h5py_dataset.py
 alethiometer/datasets/imagenet16.py
 alethiometer/zero_cost_metrics/__init__.py
 alethiometer/zero_cost_metrics/grad_norm.py
 alethiometer/zero_cost_metrics/grasp.py
+alethiometer/zero_cost_metrics/naswot.py
 alethiometer/zero_cost_metrics/snip.py
 alethiometer/zero_cost_metrics/synflow.py
```

### Comparing `alethiometer-1.0.4/setup.py` & `alethiometer-1.0.5/setup.py`

 * *Files identical despite different names*

