# Comparing `tmp/zmeiapi-0.1.6.tar.gz` & `tmp/zmeiapi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmeiapi-0.1.6.tar", last modified: Tue Apr 11 11:43:35 2023, max compression
+gzip compressed data, was "zmeiapi-0.1.7.tar", last modified: Tue Apr 11 11:45:19 2023, max compression
```

## Comparing `zmeiapi-0.1.6.tar` & `zmeiapi-0.1.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.466369 zmeiapi-0.1.6/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.6/LICENSE.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.6/MANIFEST.in
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 11:43:35.466369 zmeiapi-0.1.6/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.6/README.md
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-11 11:43:35.466369 zmeiapi-0.1.6/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-04-11 11:43:29.000000 zmeiapi-0.1.6/setup.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.462369 zmeiapi-0.1.6/zmeiapi/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.6/zmeiapi/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.462369 zmeiapi-0.1.6/zmeiapi/abstract_factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.6/zmeiapi/abstract_factories/MaterialCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1887 2023-04-11 11:43:15.000000 zmeiapi-0.1.6/zmeiapi/abstract_factories/PinCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.6/zmeiapi/abstract_factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.462369 zmeiapi-0.1.6/zmeiapi/data/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.6/zmeiapi/data/Parameters.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.6/zmeiapi/data/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.6/zmeiapi/data/nuclides_dict.pkl
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.462369 zmeiapi-0.1.6/zmeiapi/factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.6/zmeiapi/factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.466369 zmeiapi-0.1.6/zmeiapi/objects/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1715 2023-04-07 13:44:27.000000 zmeiapi-0.1.6/zmeiapi/objects/BurnupInput.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3266 2023-04-11 08:49:11.000000 zmeiapi-0.1.6/zmeiapi/objects/Cell.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-10 14:28:31.000000 zmeiapi-0.1.6/zmeiapi/objects/General.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.6/zmeiapi/objects/Lattice.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.6/zmeiapi/objects/Material.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.6/zmeiapi/objects/Pin.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5532 2023-04-07 13:50:01.000000 zmeiapi-0.1.6/zmeiapi/objects/Surface.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.6/zmeiapi/objects/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.466369 zmeiapi-0.1.6/zmeiapi/readers/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.6/zmeiapi/readers/BumatReader.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3243 2023-03-31 09:50:59.000000 zmeiapi-0.1.6/zmeiapi/readers/SerpentOut.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.6/zmeiapi/readers/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.466369 zmeiapi-0.1.6/zmeiapi/utilities/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.6/zmeiapi/utilities/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.466369 zmeiapi-0.1.6/zmeiapi/zmei_io/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.6/zmeiapi/zmei_io/Logger.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.6/zmeiapi/zmei_io/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:43:35.462369 zmeiapi-0.1.6/zmeiapi.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 11:43:35.000000 zmeiapi-0.1.6/zmeiapi.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-04-11 11:43:35.000000 zmeiapi-0.1.6/zmeiapi.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-11 11:43:35.000000 zmeiapi-0.1.6/zmeiapi.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-04-11 11:43:35.000000 zmeiapi-0.1.6/zmeiapi.egg-info/top_level.txt
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.7/LICENSE.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.7/MANIFEST.in
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.7/README.md
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-04-11 11:45:13.000000 zmeiapi-0.1.7/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.7/zmeiapi/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/abstract_factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.7/zmeiapi/abstract_factories/MaterialCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1897 2023-04-11 11:45:05.000000 zmeiapi-0.1.7/zmeiapi/abstract_factories/PinCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.7/zmeiapi/abstract_factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/data/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.7/zmeiapi/data/Parameters.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.7/zmeiapi/data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.7/zmeiapi/data/nuclides_dict.pkl
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.7/zmeiapi/factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/objects/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1715 2023-04-07 13:44:27.000000 zmeiapi-0.1.7/zmeiapi/objects/BurnupInput.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3266 2023-04-11 08:49:11.000000 zmeiapi-0.1.7/zmeiapi/objects/Cell.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-10 14:28:31.000000 zmeiapi-0.1.7/zmeiapi/objects/General.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.7/zmeiapi/objects/Lattice.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.7/zmeiapi/objects/Material.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.7/zmeiapi/objects/Pin.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5532 2023-04-07 13:50:01.000000 zmeiapi-0.1.7/zmeiapi/objects/Surface.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.7/zmeiapi/objects/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/readers/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.7/zmeiapi/readers/BumatReader.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3243 2023-03-31 09:50:59.000000 zmeiapi-0.1.7/zmeiapi/readers/SerpentOut.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.7/zmeiapi/readers/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/utilities/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.7/zmeiapi/utilities/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi/zmei_io/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.7/zmeiapi/zmei_io/Logger.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.7/zmeiapi/zmei_io/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:45:19.102593 zmeiapi-0.1.7/zmeiapi.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 11:45:19.000000 zmeiapi-0.1.7/zmeiapi.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-04-11 11:45:19.000000 zmeiapi-0.1.7/zmeiapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-11 11:45:19.000000 zmeiapi-0.1.7/zmeiapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-04-11 11:45:19.000000 zmeiapi-0.1.7/zmeiapi.egg-info/top_level.txt
```

### Comparing `zmeiapi-0.1.6/LICENSE.txt` & `zmeiapi-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/setup.py` & `zmeiapi-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='zmeiapi',
-    version='0.1.6',
+    version='0.1.7',
     description='Useful tools to work with Zmei calculation code',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     include_package_data = True,
     author='Vladislav Romanenko',
```

### Comparing `zmeiapi-0.1.6/zmeiapi/abstract_factories/MaterialCreators.py` & `zmeiapi-0.1.7/zmeiapi/abstract_factories/MaterialCreators.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/abstract_factories/PinCreators.py` & `zmeiapi-0.1.7/zmeiapi/abstract_factories/PinCreators.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 class FA2DPinsCreator(ABC):
     def __init__(self):
         self.pins = []
         pass
 
     @abstractmethod
-    def create_pins(self, cells_numbers, cells_types, pins_types, pins_materials, pins_radiuses):
+    def create_pins(self, cells_numbers, cells_types, pins_types, pins_materials, pins_radiuses, **kwargs):
         pass
 
 
 class NumberedPinsCreator(ABC):
     @abstractmethod
     def __init__(self, number, materials, radiuses):
         self.number = number
```

### Comparing `zmeiapi-0.1.6/zmeiapi/data/nuclides_dict.pkl` & `zmeiapi-0.1.7/zmeiapi/data/nuclides_dict.pkl`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/objects/BurnupInput.py` & `zmeiapi-0.1.7/zmeiapi/objects/BurnupInput.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/objects/Cell.py` & `zmeiapi-0.1.7/zmeiapi/objects/Cell.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/objects/General.py` & `zmeiapi-0.1.7/zmeiapi/objects/General.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/objects/Lattice.py` & `zmeiapi-0.1.7/zmeiapi/objects/Lattice.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/objects/Material.py` & `zmeiapi-0.1.7/zmeiapi/objects/Material.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/objects/Pin.py` & `zmeiapi-0.1.7/zmeiapi/objects/Pin.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/objects/Surface.py` & `zmeiapi-0.1.7/zmeiapi/objects/Surface.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/readers/BumatReader.py` & `zmeiapi-0.1.7/zmeiapi/readers/BumatReader.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi/readers/SerpentOut.py` & `zmeiapi-0.1.7/zmeiapi/readers/SerpentOut.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.6/zmeiapi.egg-info/SOURCES.txt` & `zmeiapi-0.1.7/zmeiapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

