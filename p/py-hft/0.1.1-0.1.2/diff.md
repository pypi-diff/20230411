# Comparing `tmp/py_hft-0.1.1.tar.gz` & `tmp/py_hft-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_hft-0.1.1.tar", last modified: Mon Sep 19 02:43:00 2022, max compression
+gzip compressed data, was "py_hft-0.1.2.tar", last modified: Tue Apr 11 11:47:49 2023, max compression
```

## Comparing `py_hft-0.1.1.tar` & `py_hft-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 02:43:00.975420 py_hft-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      294 2022-09-19 02:43:00.975420 py_hft-0.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 02:43:00.974420 py_hft-0.1.1/py_hft/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 02:43:00.975420 py_hft-0.1.1/py_hft/hft_struct/
--rw-r--r--   0 root         (0) root         (0)     3096 2022-09-16 08:46:58.000000 py_hft-0.1.1/py_hft/hft_struct/Reader.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/hft_struct/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1412 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/hft_struct/exchange_info.py
--rw-r--r--   0 root         (0) root         (0)     2309 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/hft_struct/market_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     2156 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/hft_struct/order.py
--rw-r--r--   0 root         (0) root         (0)     1065 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/hft_struct/struct_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 02:43:00.975420 py_hft-0.1.1/py_hft/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3085 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/util/factor.py
--rw-r--r--   0 root         (0) root         (0)     7802 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/util/mploter.py
--rw-r--r--   0 root         (0) root         (0)     6173 2022-09-12 16:13:27.000000 py_hft-0.1.1/py_hft/util/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 02:43:00.975420 py_hft-0.1.1/py_hft/vendor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 02:41:54.000000 py_hft-0.1.1/py_hft/vendor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8195 2022-09-19 02:41:54.000000 py_hft-0.1.1/py_hft/vendor/ali_oss_tools.py
--rw-r--r--   0 root         (0) root         (0)     9113 2022-09-19 02:41:54.000000 py_hft-0.1.1/py_hft/vendor/jq_tools.py
--rw-r--r--   0 root         (0) root         (0)     1649 2022-09-19 02:41:54.000000 py_hft-0.1.1/py_hft/vendor/rq_tools.py
--rw-r--r--   0 root         (0) root         (0)     8012 2022-09-19 02:41:54.000000 py_hft-0.1.1/py_hft/vendor/tushare_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 02:43:00.974420 py_hft-0.1.1/py_hft.egg-info/
--rw-r--r--   0 root         (0) root         (0)      294 2022-09-19 02:43:00.000000 py_hft-0.1.1/py_hft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      595 2022-09-19 02:43:00.000000 py_hft-0.1.1/py_hft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-19 02:43:00.000000 py_hft-0.1.1/py_hft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2022-09-19 02:43:00.000000 py_hft-0.1.1/py_hft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-09-19 02:43:00.000000 py_hft-0.1.1/py_hft.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-19 02:43:00.975420 py_hft-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3365 2022-09-19 02:42:58.000000 py_hft-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.586935 py_hft-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-04-11 11:47:49.585935 py_hft-0.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.584935 py_hft-0.1.2/py_hft/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.585935 py_hft-0.1.2/py_hft/hft_struct/
+-rw-r--r--   0 root         (0) root         (0)     3096 2022-10-02 00:43:47.000000 py_hft-0.1.2/py_hft/hft_struct/Reader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/exchange_info.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-04-11 11:46:12.000000 py_hft-0.1.2/py_hft/hft_struct/market_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/order.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/struct_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.585935 py_hft-0.1.2/py_hft/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2022-09-20 15:24:18.000000 py_hft-0.1.2/py_hft/util/factor.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/util/mploter.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/util/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.585935 py_hft-0.1.2/py_hft/vendor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8195 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/ali_oss_tools.py
+-rw-r--r--   0 root         (0) root         (0)     9113 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/jq_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/rq_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/tushare_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.584935 py_hft-0.1.2/py_hft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 11:47:49.586935 py_hft-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-04-11 11:47:41.000000 py_hft-0.1.2/setup.py
```

### Comparing `py_hft-0.1.1/py_hft/hft_struct/Reader.py` & `py_hft-0.1.2/py_hft/hft_struct/Reader.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/hft_struct/exchange_info.py` & `py_hft-0.1.2/py_hft/hft_struct/exchange_info.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/hft_struct/market_snapshot.py` & `py_hft-0.1.2/py_hft/hft_struct/market_snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     self.lp_ = 0.
     self.tvr_ = 0.
     self.ls_ = 0
     self.vol_ = 0
     self.oi_ = 0
   
   @property
-  def fmt(self): return '16s2Q10d10idd3i4s'
+  def fmt(self): return '8s16s2Q10d10idd3i4s'
 
   def pack(self):
-    return struct.pack(self.fmt, bytes(self.tk_, 'utf-8'), self.ts_, self.uts_, self.bp0_, self.bp1_, self.bp2_, self.bp3_, self.bp4_, self.ap0_, self.ap1_, self.ap2_, self.ap3_, self.ap4_, self.bs0_, self.bs1_, self.bs2_, self.bs3_, self.bs4_, self.as0_, self.as1_, self.as2_, self.as3_, self.as4_, self.lp_, self.tvr_, self.ls_, self.vol_, self.oi_, b'')
+    return struct.pack(self.fmt, bytes(self.tk_, 'utf-8'), bytes(self.tk_, 'utf-8'), self.ts_, self.uts_, self.bp0_, self.bp1_, self.bp2_, self.bp3_, self.bp4_, self.ap0_, self.ap1_, self.ap2_, self.ap3_, self.ap4_, self.bs0_, self.bs1_, self.bs2_, self.bs3_, self.bs4_, self.as0_, self.as1_, self.as2_, self.as3_, self.as4_, self.lp_, self.tvr_, self.ls_, self.vol_, self.oi_, b'')
 
   def Check(self, ts_check=False):
     if self.price_check:
       if self.bs0_ < 0.1 or self.as0_ < 0.1 or self.lp_ < 0.1 or self.bp0_ < 0.1 or self.ap0_ < 0.1 or len(self.tk_) > 20: return False
     if self.tk_ == 'tk': return False
     if self.tk_ == 'CODE': return False
     return True
```

### Comparing `py_hft-0.1.1/py_hft/hft_struct/order.py` & `py_hft-0.1.2/py_hft/hft_struct/order.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/hft_struct/struct_util.py` & `py_hft-0.1.2/py_hft/hft_struct/struct_util.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/util/factor.py` & `py_hft-0.1.2/py_hft/util/factor.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/util/mploter.py` & `py_hft-0.1.2/py_hft/util/mploter.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/util/util.py` & `py_hft-0.1.2/py_hft/util/util.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/vendor/ali_oss_tools.py` & `py_hft-0.1.2/py_hft/vendor/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/vendor/jq_tools.py` & `py_hft-0.1.2/py_hft/vendor/jq_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/vendor/rq_tools.py` & `py_hft-0.1.2/py_hft/vendor/rq_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft/vendor/tushare_tools.py` & `py_hft-0.1.2/py_hft/vendor/tushare_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/py_hft.egg-info/SOURCES.txt` & `py_hft-0.1.2/py_hft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.1/setup.py` & `py_hft-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'py_hft'
 DESCRIPTION = 'util for hft'
 URL = 'https://zhuanlan.zhihu.com/p/26159930'
 EMAIL = 'arockie123@gmail.com'
 AUTHOR = 'arockie'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['tushare', 'matplotlib', 'tqdm', 'psutil', 'pandas', 'tabulate', 'ipython', 'catboost', 'statsmodels', 'scipy', 'termcolor', 'jupyter', 'tushare']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

