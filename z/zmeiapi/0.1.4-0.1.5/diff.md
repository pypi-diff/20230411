# Comparing `tmp/zmeiapi-0.1.4.tar.gz` & `tmp/zmeiapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmeiapi-0.1.4.tar", last modified: Tue Apr 11 08:33:45 2023, max compression
+gzip compressed data, was "zmeiapi-0.1.5.tar", last modified: Tue Apr 11 08:49:34 2023, max compression
```

## Comparing `zmeiapi-0.1.4.tar` & `zmeiapi-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.4/LICENSE.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.4/MANIFEST.in
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.4/README.md
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-04-11 08:33:41.000000 zmeiapi-0.1.4/setup.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.4/zmeiapi/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/abstract_factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.4/zmeiapi/abstract_factories/MaterialCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1875 2023-04-10 15:33:15.000000 zmeiapi-0.1.4/zmeiapi/abstract_factories/PinCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.4/zmeiapi/abstract_factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/data/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.4/zmeiapi/data/Parameters.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.4/zmeiapi/data/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.4/zmeiapi/data/nuclides_dict.pkl
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.4/zmeiapi/factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/objects/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1715 2023-04-07 13:44:27.000000 zmeiapi-0.1.4/zmeiapi/objects/BurnupInput.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3419 2023-04-11 08:33:28.000000 zmeiapi-0.1.4/zmeiapi/objects/Cell.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-10 14:28:31.000000 zmeiapi-0.1.4/zmeiapi/objects/General.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.4/zmeiapi/objects/Lattice.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.4/zmeiapi/objects/Material.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.4/zmeiapi/objects/Pin.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5532 2023-04-07 13:50:01.000000 zmeiapi-0.1.4/zmeiapi/objects/Surface.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.4/zmeiapi/objects/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/readers/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.4/zmeiapi/readers/BumatReader.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3243 2023-03-31 09:50:59.000000 zmeiapi-0.1.4/zmeiapi/readers/SerpentOut.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.4/zmeiapi/readers/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/utilities/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.4/zmeiapi/utilities/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi/zmei_io/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.4/zmeiapi/zmei_io/Logger.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.4/zmeiapi/zmei_io/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:33:45.575340 zmeiapi-0.1.4/zmeiapi.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 08:33:45.000000 zmeiapi-0.1.4/zmeiapi.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-04-11 08:33:45.000000 zmeiapi-0.1.4/zmeiapi.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-11 08:33:45.000000 zmeiapi-0.1.4/zmeiapi.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-04-11 08:33:45.000000 zmeiapi-0.1.4/zmeiapi.egg-info/top_level.txt
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.5/LICENSE.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.5/MANIFEST.in
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.5/README.md
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-04-11 08:49:29.000000 zmeiapi-0.1.5/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.511010 zmeiapi-0.1.5/zmeiapi/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.5/zmeiapi/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/zmeiapi/abstract_factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.5/zmeiapi/abstract_factories/MaterialCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1875 2023-04-10 15:33:15.000000 zmeiapi-0.1.5/zmeiapi/abstract_factories/PinCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.5/zmeiapi/abstract_factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/zmeiapi/data/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.5/zmeiapi/data/Parameters.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.5/zmeiapi/data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.5/zmeiapi/data/nuclides_dict.pkl
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/zmeiapi/factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.5/zmeiapi/factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/zmeiapi/objects/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1715 2023-04-07 13:44:27.000000 zmeiapi-0.1.5/zmeiapi/objects/BurnupInput.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3266 2023-04-11 08:49:11.000000 zmeiapi-0.1.5/zmeiapi/objects/Cell.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-10 14:28:31.000000 zmeiapi-0.1.5/zmeiapi/objects/General.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.5/zmeiapi/objects/Lattice.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.5/zmeiapi/objects/Material.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.5/zmeiapi/objects/Pin.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5532 2023-04-07 13:50:01.000000 zmeiapi-0.1.5/zmeiapi/objects/Surface.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.5/zmeiapi/objects/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/zmeiapi/readers/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.5/zmeiapi/readers/BumatReader.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3243 2023-03-31 09:50:59.000000 zmeiapi-0.1.5/zmeiapi/readers/SerpentOut.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.5/zmeiapi/readers/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/zmeiapi/utilities/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.5/zmeiapi/utilities/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.515010 zmeiapi-0.1.5/zmeiapi/zmei_io/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.5/zmeiapi/zmei_io/Logger.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.5/zmeiapi/zmei_io/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:49:34.511010 zmeiapi-0.1.5/zmeiapi.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 08:49:34.000000 zmeiapi-0.1.5/zmeiapi.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-04-11 08:49:34.000000 zmeiapi-0.1.5/zmeiapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-11 08:49:34.000000 zmeiapi-0.1.5/zmeiapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-04-11 08:49:34.000000 zmeiapi-0.1.5/zmeiapi.egg-info/top_level.txt
```

### Comparing `zmeiapi-0.1.4/LICENSE.txt` & `zmeiapi-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/setup.py` & `zmeiapi-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='zmeiapi',
-    version='0.1.4',
+    version='0.1.5',
     description='Useful tools to work with Zmei calculation code',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     include_package_data = True,
     author='Vladislav Romanenko',
```

### Comparing `zmeiapi-0.1.4/zmeiapi/abstract_factories/MaterialCreators.py` & `zmeiapi-0.1.5/zmeiapi/abstract_factories/MaterialCreators.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/abstract_factories/PinCreators.py` & `zmeiapi-0.1.5/zmeiapi/abstract_factories/PinCreators.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/data/nuclides_dict.pkl` & `zmeiapi-0.1.5/zmeiapi/data/nuclides_dict.pkl`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/objects/BurnupInput.py` & `zmeiapi-0.1.5/zmeiapi/objects/BurnupInput.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/objects/Cell.py` & `zmeiapi-0.1.5/zmeiapi/objects/Cell.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,36 +34,32 @@
         pass
 
     def __str__(self):
         return self.line
 
     def __add__(self, other):
         if type(other) == str:
-            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
-                         fill=self.fill, delimiter=self.delimiter)
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces, delimiter=self.delimiter)
             _cell.line += f'{self.delimiter}{other}'
             return _cell
         elif type(other) == Cell:
-            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
-                         fill=self.fill, delimiter=self.delimiter)
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces, delimiter=self.delimiter)
             _cell.line += f'{self.delimiter}{other.name}'
             return _cell
         else:
             logger.error.TypeError('Unsupported operand type. Operand must have type str or Cell')
             raise TypeError('Unsupported operand type. Operand must have type str or Cell')
 
     def __sub__(self, other):
         if type(other) == str:
-            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
-                         fill=self.fill, delimiter=self.delimiter)
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces, delimiter=self.delimiter)
             _cell.line += f'{self.delimiter}-{other}'
             return _cell
         elif type(other) == Cell:
-            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
-                         fill=self.fill, delimiter=self.delimiter)
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces, delimiter=self.delimiter)
             _cell.line += f'{self.delimiter}#{other.name}'
             return _cell
         elif type(other) == list:
             """!! rebuild this to return Cell type"""
             for i, cell in enumerate(other):
                 if type(cell) == Cell:
                     _cell_name = cell.name
@@ -79,15 +75,15 @@
                 else:
                     self.line += f'{self.delimiter} {_cell_name}'
             return self.line
 
 
 if __name__ == '__main__':
     c = Cell('name', 'uni', 'mat', ['1', '2'])
-    c1 = Cell('name1', 'uni', 'mat', ['1', '2'])
+    c1 = Cell('name1', 'uni', 'mat', ['1', '2'], fill=True)
     c2 = Cell('name2', 'uni', 'mat', ['1', '2'])
 
     c3 = c1 + c2
     for inst in Cell.instances:
         print(inst)
```

### Comparing `zmeiapi-0.1.4/zmeiapi/objects/General.py` & `zmeiapi-0.1.5/zmeiapi/objects/General.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/objects/Lattice.py` & `zmeiapi-0.1.5/zmeiapi/objects/Lattice.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/objects/Material.py` & `zmeiapi-0.1.5/zmeiapi/objects/Material.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/objects/Pin.py` & `zmeiapi-0.1.5/zmeiapi/objects/Pin.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/objects/Surface.py` & `zmeiapi-0.1.5/zmeiapi/objects/Surface.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/readers/BumatReader.py` & `zmeiapi-0.1.5/zmeiapi/readers/BumatReader.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi/readers/SerpentOut.py` & `zmeiapi-0.1.5/zmeiapi/readers/SerpentOut.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.4/zmeiapi.egg-info/SOURCES.txt` & `zmeiapi-0.1.5/zmeiapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

