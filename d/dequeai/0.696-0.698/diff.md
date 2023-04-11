# Comparing `tmp/dequeai-0.696.tar.gz` & `tmp/dequeai-0.698.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.696.tar", last modified: Tue Apr 11 16:22:16 2023, max compression
+gzip compressed data, was "dequeai-0.698.tar", last modified: Tue Apr 11 16:25:45 2023, max compression
```

## Comparing `dequeai-0.696.tar` & `dequeai-0.698.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:22:16.784150 dequeai-0.696/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:22:16.784150 dequeai-0.696/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:22:16.780150 dequeai-0.696/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.696/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.696/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.696/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.696/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.696/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    20490 2023-04-11 16:19:53.000000 dequeai-0.696/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.696/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.696/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.696/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.696/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:22:16.780150 dequeai-0.696/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:22:16.000000 dequeai-0.696/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 16:22:16.000000 dequeai-0.696/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:22:16.000000 dequeai-0.696/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 16:22:16.000000 dequeai-0.696/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 16:22:16.000000 dequeai-0.696/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:22:16.784150 dequeai-0.696/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 16:22:04.000000 dequeai-0.696/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:25:45.537189 dequeai-0.698/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:25:45.537189 dequeai-0.698/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:25:45.537189 dequeai-0.698/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.698/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.698/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.698/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.698/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.698/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    20490 2023-04-11 16:19:53.000000 dequeai-0.698/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.698/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.698/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.698/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.698/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:25:45.537189 dequeai-0.698/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 16:25:45.000000 dequeai-0.698/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:25:45.537189 dequeai-0.698/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 16:25:32.000000 dequeai-0.698/setup.py
```

### Comparing `dequeai-0.696/dequeai/datatypes.py` & `dequeai-0.698/dequeai/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pickle
 import json
 import time
 import dequeai.util as util
 import numpy as np
 from dequeai.util import DEQUE_IMAGE,DEQUE_HISTOGRAM,DEQUE_AUDIO, DEQUE_TEXT, DEQUE_TABLE, DEQUE_VIDEO, DEQUE_BOUNDING_BOX, DEQUE_PLOT
 from dequeai.util import *
-import altair
+#import altair
 
 class BoundingBox2D():
     _type = DEQUE_BOUNDING_BOX
     def __init__(self, coordinates, domain=None, scores=None, caption=None):
         self.coordinates = coordinates
         if domain is None:
             self.domain = "relative"
@@ -390,15 +390,15 @@
                     print("checking whether it is deque datatype")
                     print(isinstance(column_val,(Image,Audio,Video,Text,Histogram)))
                     raise TypeError("Each column value must be a deque datatype or a builtin python type")
 
 
     def _validate_columns(self, columns):
         pass
-
+'''
 class Plot:
     _type = DEQUE_PLOT
 
     def __init__(self, data: Table=None, altair_chart=None,plot_type=BAR, plot_attributes=None):
 
         self._data=data
         self._altair_chart = altair_chart
@@ -422,14 +422,15 @@
         return js_rep
 
     def to_vega_json(self):
         return self._vega_json
 
     def to_json(self):
         return {"data":self._data,"plot_type":self._plot_type,"plot_attributes":self._plot_attributes,"vega_json":self._vega_json,"datatype":Plot._type}
+'''
 
 if __name__ == "__main__":
     #bins = [0,1, 2, 3]
     #h = np.histogram([1,2,1], bins=bins)
     import matplotlib.pyplot as plt
 
     #plt.hist(h)
@@ -446,11 +447,11 @@
     })
 
     chart = alt.Chart(source).mark_bar().encode(
         x='a',
         y='b'
     )
 
-    pl =Plot(altair_chart=chart)
-    print(pl.to_vega_json())
+    #pl =Plot(altair_chart=chart)
+    #print(pl.to_vega_json())
```

### Comparing `dequeai-0.696/dequeai/dequeai.py` & `dequeai-0.698/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.696/dequeai/dequeai_run.py` & `dequeai-0.698/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.696/dequeai/parsing_service.py` & `dequeai-0.698/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.696/dequeai/rest_connect.py` & `dequeai-0.698/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.696/dequeai/util.py` & `dequeai-0.698/dequeai/util.py`

 * *Files identical despite different names*

