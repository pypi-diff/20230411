# Comparing `tmp/pypaq-1.1.2.tar.gz` & `tmp/pypaq-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypaq-1.1.2.tar", last modified: Sun Apr  2 18:41:15 2023, max compression
+gzip compressed data, was "dist/pypaq-1.1.3.tar", last modified: Tue Apr 11 18:16:45 2023, max compression
```

## Comparing `pypaq-1.1.2.tar` & `pypaq-1.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-02 18:41:15.000000 pypaq-1.1.2/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-04-02 18:41:15.000000 pypaq-1.1.2/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      538 2023-03-05 14:20:43.000000 pypaq-1.1.2/README.md
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       41 2023-03-09 20:19:41.000000 pypaq-1.1.2/pypaq/exception.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq/lipytools/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/lipytools/__init__.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4111 2023-03-10 11:50:02.000000 pypaq-1.1.2/pypaq/lipytools/decorators.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      826 2023-03-24 23:09:04.000000 pypaq-1.1.2/pypaq/lipytools/double_hinge.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3559 2023-03-20 19:23:47.000000 pypaq-1.1.2/pypaq/lipytools/files.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1173 2023-03-09 20:19:41.000000 pypaq-1.1.2/pypaq/lipytools/moving_average.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4954 2023-03-20 14:10:43.000000 pypaq-1.1.2/pypaq/lipytools/plots.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     2995 2023-03-18 14:06:25.000000 pypaq-1.1.2/pypaq/lipytools/printout.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1750 2023-03-26 12:28:29.000000 pypaq-1.1.2/pypaq/lipytools/pylogger.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       73 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/lipytools/softmax.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)      977 2023-03-26 08:26:06.000000 pypaq-1.1.2/pypaq/lipytools/stats.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq/mpython/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/mpython/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     6005 2023-03-09 20:42:47.000000 pypaq-1.1.2/pypaq/mpython/devices.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1563 2023-02-28 16:27:57.000000 pypaq-1.1.2/pypaq/mpython/mpdecor.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5315 2023-03-27 15:53:38.000000 pypaq-1.1.2/pypaq/mpython/mptools.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq/pms/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/pms/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2939 2023-03-20 19:29:23.000000 pypaq-1.1.2/pypaq/pms/base.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2609 2023-03-11 12:18:25.000000 pypaq-1.1.2/pypaq/pms/config_manager.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    11938 2023-03-09 20:43:48.000000 pypaq-1.1.2/pypaq/pms/parasave.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    18475 2023-04-02 18:34:58.000000 pypaq-1.1.2/pypaq/pms/paspa.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     7749 2023-03-24 18:14:54.000000 pypaq-1.1.2/pypaq/pms/subscriptable.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      152 2023-03-31 21:11:22.000000 pypaq-1.1.2/pypaq/pytypes.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq/textools/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/textools/__init__.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1210 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/textools/text_metrics.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      586 2023-02-27 23:13:46.000000 pypaq-1.1.2/pypaq/textools/text_processing.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq.egg-info/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq.egg-info/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      827 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq.egg-info/SOURCES.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq.egg-info/dependency_links.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       89 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq.egg-info/requires.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        6 2023-04-02 18:41:15.000000 pypaq-1.1.2/pypaq.egg-info/top_level.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-04-02 18:41:15.000000 pypaq-1.1.2/setup.cfg
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      622 2023-04-02 18:40:57.000000 pypaq-1.1.2/setup.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-04-11 18:16:45.000000 pypaq-1.1.3/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      538 2023-03-05 14:20:43.000000 pypaq-1.1.3/README.md
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       41 2023-03-09 20:19:41.000000 pypaq-1.1.3/pypaq/exception.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/lipytools/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/lipytools/__init__.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4111 2023-03-10 11:50:02.000000 pypaq-1.1.3/pypaq/lipytools/decorators.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      826 2023-03-24 23:09:04.000000 pypaq-1.1.3/pypaq/lipytools/double_hinge.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3559 2023-03-20 19:23:47.000000 pypaq-1.1.3/pypaq/lipytools/files.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1173 2023-03-09 20:19:41.000000 pypaq-1.1.3/pypaq/lipytools/moving_average.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4954 2023-03-20 14:10:43.000000 pypaq-1.1.3/pypaq/lipytools/plots.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     2995 2023-03-18 14:06:25.000000 pypaq-1.1.3/pypaq/lipytools/printout.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1750 2023-03-26 12:28:29.000000 pypaq-1.1.3/pypaq/lipytools/pylogger.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       73 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/lipytools/softmax.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)      977 2023-03-26 08:26:06.000000 pypaq-1.1.3/pypaq/lipytools/stats.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/mpython/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/mpython/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5927 2023-04-11 17:27:08.000000 pypaq-1.1.3/pypaq/mpython/devices.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1563 2023-02-28 16:27:57.000000 pypaq-1.1.3/pypaq/mpython/mpdecor.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5315 2023-03-27 15:53:38.000000 pypaq-1.1.3/pypaq/mpython/mptools.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/pms/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/pms/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2939 2023-03-20 19:29:23.000000 pypaq-1.1.3/pypaq/pms/base.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2609 2023-03-11 12:18:25.000000 pypaq-1.1.3/pypaq/pms/config_manager.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    11938 2023-03-09 20:43:48.000000 pypaq-1.1.3/pypaq/pms/parasave.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    18475 2023-04-02 18:34:58.000000 pypaq-1.1.3/pypaq/pms/paspa.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     7749 2023-03-24 18:14:54.000000 pypaq-1.1.3/pypaq/pms/subscriptable.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      152 2023-03-31 21:11:22.000000 pypaq-1.1.3/pypaq/pytypes.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/textools/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/textools/__init__.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1210 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/textools/text_metrics.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      586 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/textools/text_processing.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      827 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/SOURCES.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/dependency_links.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       89 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/requires.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        6 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/top_level.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-04-11 18:16:45.000000 pypaq-1.1.3/setup.cfg
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      622 2023-04-11 18:16:12.000000 pypaq-1.1.3/setup.py
```

### Comparing `pypaq-1.1.2/README.md` & `pypaq-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/decorators.py` & `pypaq-1.1.3/pypaq/lipytools/decorators.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/double_hinge.py` & `pypaq-1.1.3/pypaq/lipytools/double_hinge.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/files.py` & `pypaq-1.1.3/pypaq/lipytools/files.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/moving_average.py` & `pypaq-1.1.3/pypaq/lipytools/moving_average.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/plots.py` & `pypaq-1.1.3/pypaq/lipytools/plots.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/printout.py` & `pypaq-1.1.3/pypaq/lipytools/printout.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/pylogger.py` & `pypaq-1.1.3/pypaq/lipytools/pylogger.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/lipytools/stats.py` & `pypaq-1.1.3/pypaq/lipytools/stats.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/mpython/devices.py` & `pypaq-1.1.3/pypaq/mpython/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,21 +69,20 @@
     if not logger: logger = get_pylogger(level=loglevel)
 
     if type(devices) is not list: devices = [devices]  # first convert to list
 
     cpu_count = sys_res_nfo()['cpu_count']
     logger.debug(f'got {cpu_count} CPU devices in a system')
 
-    # look for available CUDA
+    # try to get available CUDA
     available_cuda_id = []
-    if platform.system() == 'Darwin': # OSX
-        logger.warning('no GPUs available for OSX, using only CPU')
-    else:
+    try:
         available_cuda_id = get_available_cuda_id()
-    logger.debug(f'got available GPU devices: {available_cuda_id}')
+    except Exception as e:
+        logger.warning(f'could not get CUDA devices, got EXCEPTION: {e}')
 
     if devices == []:
         return available_cuda_id
 
     devices_base = []
     for d in devices:
```

### Comparing `pypaq-1.1.2/pypaq/mpython/mpdecor.py` & `pypaq-1.1.3/pypaq/mpython/mpdecor.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/mpython/mptools.py` & `pypaq-1.1.3/pypaq/mpython/mptools.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/pms/base.py` & `pypaq-1.1.3/pypaq/pms/base.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/pms/config_manager.py` & `pypaq-1.1.3/pypaq/pms/config_manager.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/pms/parasave.py` & `pypaq-1.1.3/pypaq/pms/parasave.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/pms/paspa.py` & `pypaq-1.1.3/pypaq/pms/paspa.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/pms/subscriptable.py` & `pypaq-1.1.3/pypaq/pms/subscriptable.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/textools/text_metrics.py` & `pypaq-1.1.3/pypaq/textools/text_metrics.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq/textools/text_processing.py` & `pypaq-1.1.3/pypaq/textools/text_processing.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/pypaq.egg-info/SOURCES.txt` & `pypaq-1.1.3/pypaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.2/setup.py` & `pypaq-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('requirements.txt') as file:
         lines = [l[:-1] if l[-1]=='\n' else l for l in file.readlines()]
         return lines
 
 
 setup(
     name=               'pypaq',
-    version=            'v1.1.2',
+    version=            'v1.1.3',
     url=                'https://github.com/piteren/pypaq.git',
     author=             'Piotr Niewinski',
     author_email=       'pioniewinski@gmail.com',
     description=        'little python tools',
     packages=           find_packages(),
     install_requires=   get_requirements(),
     license=            'MIT')
```

