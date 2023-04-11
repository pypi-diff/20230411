# Comparing `tmp/zmeiapi-0.1.2.tar.gz` & `tmp/zmeiapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmeiapi-0.1.2.tar", last modified: Fri Apr  7 13:28:38 2023, max compression
+gzip compressed data, was "zmeiapi-0.1.3.tar", last modified: Tue Apr 11 08:25:50 2023, max compression
```

## Comparing `zmeiapi-0.1.2.tar` & `zmeiapi-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.2/LICENSE.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.2/MANIFEST.in
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.2/README.md
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-04-07 13:28:28.000000 zmeiapi-0.1.2/setup.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.326747 zmeiapi-0.1.2/zmeiapi/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.2/zmeiapi/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.326747 zmeiapi-0.1.2/zmeiapi/abstract_factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.2/zmeiapi/abstract_factories/MaterialCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1665 2023-03-31 09:50:59.000000 zmeiapi-0.1.2/zmeiapi/abstract_factories/PinCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.2/zmeiapi/abstract_factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/zmeiapi/data/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.2/zmeiapi/data/Parameters.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.2/zmeiapi/data/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.2/zmeiapi/data/nuclides_dict.pkl
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/zmeiapi/factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.2/zmeiapi/factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/zmeiapi/objects/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1712 2023-04-05 13:11:45.000000 zmeiapi-0.1.2/zmeiapi/objects/BurnupInput.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2377 2023-04-07 13:28:10.000000 zmeiapi-0.1.2/zmeiapi/objects/Cell.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-07 07:19:48.000000 zmeiapi-0.1.2/zmeiapi/objects/General.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.2/zmeiapi/objects/Lattice.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.2/zmeiapi/objects/Material.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.2/zmeiapi/objects/Pin.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5531 2023-04-07 13:11:15.000000 zmeiapi-0.1.2/zmeiapi/objects/Surface.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.2/zmeiapi/objects/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/zmeiapi/readers/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.2/zmeiapi/readers/BumatReader.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3243 2023-03-31 09:50:59.000000 zmeiapi-0.1.2/zmeiapi/readers/SerpentOut.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.2/zmeiapi/readers/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/zmeiapi/utilities/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.2/zmeiapi/utilities/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.330746 zmeiapi-0.1.2/zmeiapi/zmei_io/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.2/zmeiapi/zmei_io/Logger.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.2/zmeiapi/zmei_io/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-07 13:28:38.326747 zmeiapi-0.1.2/zmeiapi.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-07 13:28:38.000000 zmeiapi-0.1.2/zmeiapi.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-04-07 13:28:38.000000 zmeiapi-0.1.2/zmeiapi.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-07 13:28:38.000000 zmeiapi-0.1.2/zmeiapi.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-04-07 13:28:38.000000 zmeiapi-0.1.2/zmeiapi.egg-info/top_level.txt
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.3/LICENSE.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.3/MANIFEST.in
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.3/README.md
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-04-11 08:25:37.000000 zmeiapi-0.1.3/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.3/zmeiapi/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/abstract_factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.3/zmeiapi/abstract_factories/MaterialCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1875 2023-04-10 15:33:15.000000 zmeiapi-0.1.3/zmeiapi/abstract_factories/PinCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.3/zmeiapi/abstract_factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/data/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.3/zmeiapi/data/Parameters.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.3/zmeiapi/data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.3/zmeiapi/data/nuclides_dict.pkl
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.3/zmeiapi/factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/objects/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1715 2023-04-07 13:44:27.000000 zmeiapi-0.1.3/zmeiapi/objects/BurnupInput.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3414 2023-04-11 08:25:16.000000 zmeiapi-0.1.3/zmeiapi/objects/Cell.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-10 14:28:31.000000 zmeiapi-0.1.3/zmeiapi/objects/General.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.3/zmeiapi/objects/Lattice.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.3/zmeiapi/objects/Material.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.3/zmeiapi/objects/Pin.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5532 2023-04-07 13:50:01.000000 zmeiapi-0.1.3/zmeiapi/objects/Surface.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.3/zmeiapi/objects/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/readers/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.3/zmeiapi/readers/BumatReader.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3243 2023-03-31 09:50:59.000000 zmeiapi-0.1.3/zmeiapi/readers/SerpentOut.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.3/zmeiapi/readers/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/utilities/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.3/zmeiapi/utilities/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi/zmei_io/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.3/zmeiapi/zmei_io/Logger.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.3/zmeiapi/zmei_io/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 08:25:50.530295 zmeiapi-0.1.3/zmeiapi.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 08:25:50.000000 zmeiapi-0.1.3/zmeiapi.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-04-11 08:25:50.000000 zmeiapi-0.1.3/zmeiapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-11 08:25:50.000000 zmeiapi-0.1.3/zmeiapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-04-11 08:25:50.000000 zmeiapi-0.1.3/zmeiapi.egg-info/top_level.txt
```

### Comparing `zmeiapi-0.1.2/LICENSE.txt` & `zmeiapi-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/setup.py` & `zmeiapi-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='zmeiapi',
-    version='0.1.2',
+    version='0.1.3',
     description='Useful tools to work with Zmei calculation code',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     include_package_data = True,
     author='Vladislav Romanenko',
```

### Comparing `zmeiapi-0.1.2/zmeiapi/abstract_factories/MaterialCreators.py` & `zmeiapi-0.1.3/zmeiapi/abstract_factories/MaterialCreators.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/zmeiapi/abstract_factories/PinCreators.py` & `zmeiapi-0.1.3/zmeiapi/abstract_factories/PinCreators.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,24 @@
             self,
             name: str,
             **kwargs
     ):
         pass
 
 
+class FA2DPinsCreator(ABC):
+    def __init__(self):
+        self.pins = []
+        pass
+
+    @abstractmethod
+    def create_pins(self, cells_numbers, cells_types, pins_materials, pins_radiuses):
+        pass
+
+
 class NumberedPinsCreator(ABC):
     @abstractmethod
     def __init__(self, number, materials, radiuses):
         self.number = number
         self.materials = materials
         self.radiuses = radiuses
         if len(self.materials) - len(self.radiuses) != 1:
```

### Comparing `zmeiapi-0.1.2/zmeiapi/data/nuclides_dict.pkl` & `zmeiapi-0.1.3/zmeiapi/data/nuclides_dict.pkl`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/zmeiapi/objects/BurnupInput.py` & `zmeiapi-0.1.3/zmeiapi/objects/BurnupInput.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def _compile_butot(self, file):
         if self.butot is None:
             pass
         else:
             file.write(f'dep butot \n')
             for burnup in self.butot:
-                file.write(f'{burnup:10.5E}')
+                file.write(f'{burnup:10.5E} \n')
 
     def compile(self, filename):
         with open(filename, 'w') as file:
             self._compile_inventory(file)
             self._compile_printm(file)
             file.write('\n')
             self._compile_mvol(file)
```

### Comparing `zmeiapi-0.1.2/zmeiapi/objects/Cell.py` & `zmeiapi-0.1.3/zmeiapi/objects/Cell.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from zmeiapi.zmei_io.Logger import logger
+
+
 class Cell:
     instances = []
 
     @classmethod
     def write_instances_to_file(cls, filename) -> None:
         """
         Class method to write all instances into the file
@@ -9,42 +12,62 @@
         :type filename: str
         :return: None
         """
         with open(filename, 'w') as file:
             for instance in cls.instances:
                 file.writelines(instance.lines)
 
-    def __init__(self, name, universe, material, surfaces, delimiter='  '):
+    def __init__(self, name, universe, material, surfaces, fill=False, delimiter='  ', **kwargs):
         self.__class__.instances.append(self)
         self.name = f'c{name}'
+        self.universe = universe
+        self.fill = fill
+        if self.fill:
+            self.material = f'fill {material}'
+        else:
+            self.material = material
+        self.surfaces = surfaces
         self.delimiter = delimiter
-        self.line = f'{self.name}{delimiter}{universe}{delimiter}{material}'
-        for surface in surfaces:
-            self.line += f'{delimiter}{surface}'
+        self.line = f'{self.name}{self.delimiter}{self.universe}{self.delimiter}{self.material}'
+
+        for surface in self.surfaces:
+            self.line += f'{self.delimiter}{surface}'
         pass
 
     def __str__(self):
         return self.line
 
     def __add__(self, other):
         if type(other) == str:
-            self.line += f'{self.delimiter}{other}'
-            return self.line
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
+                         fill=self.fill, delimiter=self.delimiter)
+            _cell.line += f'{self.delimiter}{other}'
+            return _cell
         elif type(other) == Cell:
-            self.line += f'{self.delimiter}{other.name}'
-            # return self
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
+                         fill=self.fill, delimiter=self.delimiter)
+            _cell.line += f'{self.delimiter}{other.name}'
+            return _cell
+        else:
+            logger.error.TypeError('Unsupported operand type. Operand must have type str or Cell')
+            raise TypeError('Unsupported operand type. Operand must have type str or Cell')
 
     def __sub__(self, other):
         if type(other) == str:
-            self.line += f'{self.delimiter}-{other}'
-            return self.line
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
+                         fill=self.fill, delimiter=self.delimiter)
+            _cell.line += f'{self.delimiter}-{other}'
+            return _cell
         elif type(other) == Cell:
-            self.line += f'{self.delimiter}#{other.name}'
-            return self.line
+            _cell = Cell(self.name[1:], self.universe, self.material, self.surfaces,
+                         fill=self.fill, delimiter=self.delimiter)
+            _cell.line += f'{self.delimiter}#{other.name}'
+            return _cell
         elif type(other) == list:
+            """!! rebuild this to return Cell type"""
             for i, cell in enumerate(other):
                 if type(cell) == Cell:
                     _cell_name = cell.name
                 elif type(cell) == str:
                     _cell_name = cell
                 else:
                     raise RuntimeError('should be list of str or Cell')
@@ -56,20 +79,15 @@
                 else:
                     self.line += f'{self.delimiter} {_cell_name}'
             return self.line
 
 
 if __name__ == '__main__':
     c = Cell('name', 'uni', 'mat', ['1', '2'])
-    c1 = Cell('name', 'uni', 'mat', ['1', '2'])
-    c2 = Cell('name', 'uni', 'mat', ['1', '2'])
-    print(c)
-    print(c + 'hello')
-    print(c - 'hello')
-    print(c - c1)
-    print(c + c1)
-    print(c - [c1, c2])
-    print(c - ['f', 'e'])
-    inst = Cell.instances[2]
-    print(inst)
-    c3 = c2
+    c1 = Cell('name1', 'uni', 'mat', ['1', '2'])
+    c2 = Cell('name2', 'uni', 'mat', ['1', '2'])
+
+    c3 = c1 + c2
+    for inst in Cell.instances:
+        print(inst)
+
```

### Comparing `zmeiapi-0.1.2/zmeiapi/objects/General.py` & `zmeiapi-0.1.3/zmeiapi/objects/General.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,19 +69,19 @@
         else:
             logger.error(f'Gcu attribute must have a list type {type(self.gcu)}')
             raise AttributeError(f'Gcu attribute must have a list type')
 
     def _compile_bc(self, file):
         if self.bc is None:
             pass
-        elif (self.bc == 0) or (self.bc == 1):
+        elif (self.bc == 1) or (self.bc == 2):
             file.write(f'set bc {self.bc} \n')
         else:
-            logger.error(f'Bc attribute possible values must be 0 or 1')
-            raise AttributeError(f'Bc attribute possible values must be 0 or 1')
+            logger.error(f'Bc attribute possible values must be 1 or 2')
+            raise AttributeError(f'Bc attribute possible values must be 1 or 2')
 
     def _compile_pop(self, file):
         if self.pop is None:
             pass
         elif type(self.pop) is list:
             _line = 'set pop '
             for f in self.pop:
```

### Comparing `zmeiapi-0.1.2/zmeiapi/objects/Lattice.py` & `zmeiapi-0.1.3/zmeiapi/objects/Lattice.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/zmeiapi/objects/Material.py` & `zmeiapi-0.1.3/zmeiapi/objects/Material.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/zmeiapi/objects/Pin.py` & `zmeiapi-0.1.3/zmeiapi/objects/Pin.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/zmeiapi/objects/Surface.py` & `zmeiapi-0.1.3/zmeiapi/objects/Surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             if len(self.params) != 3:
                 logger.error('Wrong parameters number, loot at the class description')
                 raise AttributeError('Wrong parameters number, loot at the class description')
 
     class Hexxap(AbstractSurface):
         def __init__(self, name: str, params: list[float | int]):
             super().__init__(name, params)
-            super()._create_lines('hexxc')
+            super()._create_lines('hexxap')
 
         def _check_surf_parameters(self):
             if len(self.params) != 5:
                 logger.error('Wrong parameters number, loot at the class description')
                 raise AttributeError('Wrong parameters number, loot at the class description')
```

### Comparing `zmeiapi-0.1.2/zmeiapi/readers/BumatReader.py` & `zmeiapi-0.1.3/zmeiapi/readers/BumatReader.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/zmeiapi/readers/SerpentOut.py` & `zmeiapi-0.1.3/zmeiapi/readers/SerpentOut.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.2/zmeiapi.egg-info/SOURCES.txt` & `zmeiapi-0.1.3/zmeiapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

