# Comparing `tmp/VVER-1000package-0.0.3.tar.gz` & `tmp/VVER-1000package-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VVER-1000package-0.0.3.tar", last modified: Thu Apr  6 10:00:18 2023, max compression
+gzip compressed data, was "VVER-1000package-0.0.4.tar", last modified: Tue Apr 11 11:28:14 2023, max compression
```

## Comparing `VVER-1000package-0.0.3.tar` & `VVER-1000package-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-06 10:00:18.593325 VVER-1000package-0.0.3/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 VVER-1000package-0.0.3/LICENSE.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       35 2023-04-05 14:01:26.000000 VVER-1000package-0.0.3/MANIFEST.in
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      395 2023-04-06 10:00:18.593325 VVER-1000package-0.0.3/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 VVER-1000package-0.0.3/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-06 10:00:18.589325 VVER-1000package-0.0.3/VVER1000package/
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-06 10:00:18.589325 VVER-1000package-0.0.3/VVER1000package/TVSA/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     6295 2023-04-06 09:56:20.000000 VVER-1000package-0.0.3/VVER1000package/TVSA/SerpentCreator.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     4836 2023-04-04 09:58:30.000000 VVER-1000package-0.0.3/VVER1000package/TVSA/TVSAConcentrations.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    15478 2023-04-04 13:13:43.000000 VVER-1000package-0.0.3/VVER1000package/TVSA/TVSAParameters.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-26 14:27:26.000000 VVER-1000package-0.0.3/VVER1000package/TVSA/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-22 23:04:17.000000 VVER-1000package-0.0.3/VVER1000package/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-06 10:00:18.589325 VVER-1000package-0.0.3/VVER1000package/absfabrics/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5323 2023-04-04 21:42:35.000000 VVER-1000package-0.0.3/VVER1000package/absfabrics/Concentrations.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-26 12:32:18.000000 VVER-1000package-0.0.3/VVER1000package/absfabrics/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-06 10:00:18.589325 VVER-1000package-0.0.3/VVER1000package/data/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1300 2023-04-04 10:04:45.000000 VVER-1000package-0.0.3/VVER1000package/data/MaterialsParameters.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      435 2023-03-23 10:31:24.000000 VVER-1000package-0.0.3/VVER1000package/data/Parameters.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-22 23:04:06.000000 VVER-1000package-0.0.3/VVER1000package/data/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 VVER-1000package-0.0.3/VVER1000package/data/nuclides_dict.pkl
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     8931 2023-03-23 13:43:04.000000 VVER-1000package-0.0.3/VVER1000package/data/nuclides_masses.pkl
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      435 2023-03-23 13:43:04.000000 VVER-1000package-0.0.3/VVER1000package/data/parse_nuclides_masses.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-06 10:00:18.593325 VVER-1000package-0.0.3/VVER_1000package.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      395 2023-04-06 10:00:18.000000 VVER-1000package-0.0.3/VVER_1000package.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      706 2023-04-06 10:00:18.000000 VVER-1000package-0.0.3/VVER_1000package.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-06 10:00:18.000000 VVER-1000package-0.0.3/VVER_1000package.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       16 2023-04-06 10:00:18.000000 VVER-1000package-0.0.3/VVER_1000package.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-06 10:00:18.593325 VVER-1000package-0.0.3/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      842 2023-04-06 09:58:46.000000 VVER-1000package-0.0.3/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:28:14.859710 VVER-1000package-0.0.4/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 VVER-1000package-0.0.4/LICENSE.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       35 2023-04-05 14:01:26.000000 VVER-1000package-0.0.4/MANIFEST.in
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      395 2023-04-11 11:28:14.859710 VVER-1000package-0.0.4/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 VVER-1000package-0.0.4/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:28:14.855710 VVER-1000package-0.0.4/VVER1000package/
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:28:14.855710 VVER-1000package-0.0.4/VVER1000package/TVSA/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     8007 2023-04-11 11:27:40.000000 VVER-1000package-0.0.4/VVER1000package/TVSA/SerpentCreator.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     4836 2023-04-04 09:58:30.000000 VVER-1000package-0.0.4/VVER1000package/TVSA/TVSAConcentrations.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    12666 2023-04-11 09:42:27.000000 VVER-1000package-0.0.4/VVER1000package/TVSA/TVSAParameters.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-26 14:27:26.000000 VVER-1000package-0.0.4/VVER1000package/TVSA/__init__.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-22 23:04:17.000000 VVER-1000package-0.0.4/VVER1000package/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:28:14.855710 VVER-1000package-0.0.4/VVER1000package/absfabrics/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5323 2023-04-04 21:42:35.000000 VVER-1000package-0.0.4/VVER1000package/absfabrics/Concentrations.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-26 12:32:18.000000 VVER-1000package-0.0.4/VVER1000package/absfabrics/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:28:14.855710 VVER-1000package-0.0.4/VVER1000package/data/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1300 2023-04-04 10:04:45.000000 VVER-1000package-0.0.4/VVER1000package/data/MaterialsParameters.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      435 2023-03-23 10:31:24.000000 VVER-1000package-0.0.4/VVER1000package/data/Parameters.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-22 23:04:06.000000 VVER-1000package-0.0.4/VVER1000package/data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 VVER-1000package-0.0.4/VVER1000package/data/nuclides_dict.pkl
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     8931 2023-03-23 13:43:04.000000 VVER-1000package-0.0.4/VVER1000package/data/nuclides_masses.pkl
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      435 2023-03-23 13:43:04.000000 VVER-1000package-0.0.4/VVER1000package/data/parse_nuclides_masses.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:28:14.859710 VVER-1000package-0.0.4/VVER_1000package.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      395 2023-04-11 11:28:14.000000 VVER-1000package-0.0.4/VVER_1000package.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      706 2023-04-11 11:28:14.000000 VVER-1000package-0.0.4/VVER_1000package.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-11 11:28:14.000000 VVER-1000package-0.0.4/VVER_1000package.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       16 2023-04-11 11:28:14.000000 VVER-1000package-0.0.4/VVER_1000package.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-11 11:28:14.859710 VVER-1000package-0.0.4/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      842 2023-04-11 11:28:02.000000 VVER-1000package-0.0.4/setup.py
```

### Comparing `VVER-1000package-0.0.3/LICENSE.txt` & `VVER-1000package-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VVER-1000package-0.0.3/VVER1000package/TVSA/SerpentCreator.py` & `VVER-1000package-0.0.4/VVER1000package/TVSA/SerpentCreator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,110 @@
 from zmeiapi.objects.Material import Material
 from zmeiapi.objects.Pin import Pin
-from zmeiapi.abstract_factories.PinCreators import NumberedPinsCreator
+from zmeiapi.abstract_factories.PinCreators import FA2DPinsCreator
 from zmeiapi.abstract_factories.MaterialCreators import NumberedMaterialsCreator
 from zmeiapi.objects.General import General
 from VVER1000package.TVSA.TVSAConcentrations import CoolantConcentrationsTVSA, UFuelConcentrationsTVSA, \
     GdFuelConcentrationsTVSA, SimpleMaterialConcentrationsTVSA
 from VVER1000package.TVSA.TVSAParameters import TVSA_cells_numbers, TVSA_30AV5_cells_types, \
     TVSA_pins_materials, TVSA_pins_radiuses, TVSA_pins_types, r_ohe
+import math
 
 
 def int_val(string):
     val = int(string.split('_')[-1])
     return val
 
 
 # creating pins
-class TVSAPinsCreator(NumberedPinsCreator):
-    def __init__(self, number, materials, radiuses):
-        super().__init__(number, materials, radiuses)
-        self.pins = []
-
-    def create_pins(self, name: str, cells_numbers=TVSA_cells_numbers, cells_types=TVSA_30AV5_cells_types,
-                    pins_materials=TVSA_pins_materials, pins_radiuses=TVSA_pins_radiuses, **kwargs):
-
-        for i, row in enumerate(TVSA_cells_numbers):
-            for j, pin_number in enumerate(TVSA_cells_numbers[i]):
+class TVSAPinsCreator(FA2DPinsCreator):
+    def __init__(self):
+        super().__init__()
+
+    def create_pins(self, cells_numbers, cells_types, pins_materials, pins_radiuses,
+                    split_fu=False, split_gd=True, n_fu_layers=1, n_gd_layers=10):
+        for i, row in enumerate(cells_numbers):
+            for j, pin_number in enumerate(cells_numbers[i]):
                 if pin_number == 0:
-                   continue
+                    continue
 
-                pin_type = TVSA_pins_types[TVSA_30AV5_cells_types[i][j]]
-                # if pin_type.startswith('FU'):
-                #     pin_type = 'FU'
-                # elif pin_type.startswith('GDFU'):
-                #     pin_type = 'GD'
-
-                _pin_materials = []
-                for material in pins_materials[pin_type]:
-                    if material.startswith('FU') or material.startswith('GDFU') \
-                            or material.startswith('GC') or material.startswith('CC'):
-                        _pin_materials.append(f'{material}_{pin_number:03}')
-                    else:
-                        _pin_materials.append(material)
-                self.pins.append(Pin(f'{pin_type}_{pin_number:03}', _pin_materials, pins_radiuses[pin_type]))
+                pin_type = TVSA_pins_types[cells_types[i][j]]
+
+                # _pin_materials = []
+                # _pin_radiuses = []
+                # for material in pins_materials[pin_type]:
+                #     if material.startswith('FU') or material.startswith('GDFU') \
+                #             or material.startswith('GC') or material.startswith('CC'):
+                #         _pin_materials.append(f'{material}_{pin_number:03}')
+                #     else:
+                #         _pin_materials.append(material)
+                _pin_materials, _pin_radiuses = self.create_pin_materials_and_radiuses(
+                    pins_materials[pin_type], pins_radiuses[pin_type],
+                    split_fu=split_fu, split_gd=split_gd,
+                    n_fu_layers=n_fu_layers, n_gd_layers=n_gd_layers
+                                                       )
+                self.pins.append(Pin(f'{pin_type}_{pin_number:03}', _pin_materials, _pin_radiuses))
         return self.pins
 
+    def create_pin_materials_and_radiuses(self, pin_materials, pin_radiuses,
+                                          split_fu=False, split_gd=True, n_fu_layers=1, n_gd_layers=10):
+        _new_pin_materials = []
+        _new_pin_radiuses = []
+        for i, material in enumerate(pin_materials):
+            if split_fu and material.startswith('FU'):
+                _fu_radiuses, _fu_materials = \
+                    self.get_radiuses_for_splitting(pin_radiuses[i], n_fu_layers, pin_materials[i])
+                _new_pin_materials += _fu_materials
+                _new_pin_radiuses += _fu_radiuses
+            elif split_gd and material.startswith('GDFU'):
+                _gd_radiuses, _gd_materials = \
+                    self.get_radiuses_for_splitting(pin_radiuses[i], n_gd_layers, pin_materials[i])
+                _new_pin_materials += _gd_materials
+                _new_pin_radiuses += _gd_radiuses
+            else:
+                _new_pin_materials.append(material)
+                if i != len(pin_materials):
+                    _new_pin_radiuses.append(pin_radiuses[i])
+
+        return _new_pin_materials, _new_pin_radiuses
+
+    @staticmethod
+    def get_radiuses_for_splitting(outer_radius, n_layers, material_name):
+        s_average = math.pi * outer_radius * outer_radius / n_layers
+        radiuses = []
+        materials = []
+        for i in range(n_layers - 1):
+            radiuses[i] = math.sqrt((i + 1) * s_average / math.pi)
+            materials.append(f'{material_name}_r{i:02}')
+        radiuses.append(outer_radius)
+        materials.append(f'{material_name}_r{n_layers - 1:02}')
+        return radiuses, materials
+
     def get_pins_materials(self):
         _all_materials = []
         for pin in self.pins:
             for mat in pin.materials:
                 _all_materials.append(mat)
 
         _all_materials = list(set(_all_materials))
         _all_materials.sort()
-        print(_all_materials)
+        # print(_all_materials)
         return _all_materials
 
 
 class TVSAMaterialsCreator(NumberedMaterialsCreator):
     def __init__(self, number):
         super().__init__(number)
         pass
 
     def create_materials(self, name: str, nuclides: list, concentrations: list, **kwargs):
         pass
 
 
-TVSA_pins = TVSAPinsCreator(1, ['d'], [])
+TVSA_pins = TVSAPinsCreator()
 pins_list = TVSA_pins.create_pins('name')
 # Pin.instances.sort(key=int_val)
 Pin.write_instances_to_file('test_pins')
 print(Pin.instances)
 materials = TVSA_pins.get_pins_materials()
 
 materials_list = []
```

### Comparing `VVER-1000package-0.0.3/VVER1000package/TVSA/TVSAConcentrations.py` & `VVER-1000package-0.0.4/VVER1000package/TVSA/TVSAConcentrations.py`

 * *Files identical despite different names*

### Comparing `VVER-1000package-0.0.3/VVER1000package/TVSA/TVSAParameters.py` & `VVER-1000package-0.0.4/VVER1000package/TVSA/TVSAParameters.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,40 +39,14 @@
 S_coolant = S_fa - n_pins * S_pin - n_cc * S_cc - n_gc * S_gc
 V_coolant = S_coolant * H_az
 
 V_spacer = n_spacers * m_spacer / ro['Э-110']
 
 gamma_spacer = V_spacer / V_coolant
 
-# TVSA_cells_numbers = [
-#     [0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0],
-#     [0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   56,  77,  98,  119, 140, 161, 182, 203, 224, 245, 266, 0],
-#     [0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   46,  67,  88,  109, 130, 151, 172, 193, 214, 235, 256, 277, 0],
-#     [0,   0,   0,   0,   0,   0,   0,   0,   0,   37,  57,  78,  99,  120, 141, 162, 183, 204, 225, 246, 267, 287, 0],
-#     [0,   0,   0,   0,   0,   0,   0,   0,   29,  47,  68,  89,  110, 131, 152, 173, 194, 215, 236, 257, 278, 296, 0],
-#     [0,   0,   0,   0,   0,   0,   0,   22,  38,  58,  79,  100, 121, 142, C163,184, 205, 226, 247, 268, 288, 304, 0],
-#     [0,   0,   0,   0,   0,   0,   16,  30,  48,  69,  90,  C111,132, 153, 174, 195, C216,237, 258, 279, 297, 311, 0],
-#     [0,   0,   0,   0,   0,   11,  23,  39,  59,  80,  101, 122, 143, 164, 185, 206, 227, 248, 269, 289, 305, 317, 0],
-#     [0,   0,   0,   0,   7,   17,  31,  49,  C070,91,  112, 133, C154,175, 196, 217, 238, C259,280, 298, 312, 322, 0],
-#     [0,   0,   0,   4,   12,  24,  40,  60,  81,  102, 123, 144, 165, 186, C207,228, 249, 270, 290, 306, 318, 326, 0],
-#     [0,   0,   2,   8,   18,  32,  50,  71,  92,  C113,134, 155, 176, 197, 218, 239, 260, 281, 299, 313, 323, 329, 0],
-#     [0,   1,   5,   13,  25,  41,  C061,82,  103, 124, 145, C166,187, 208, 229, 250, C271,291, 307, 319, 327, 331, 0],
-#     [0,   3,   9,   19,  33,  51,  72,  93,  114, 135, 156, 177, 198, C219,240, 261, 282, 300, 314, 324, 330, 0,   0],
-#     [0,   6,   14,  26,  42,  62,  83,  104, C125,146, 167, 188, 209, 230, 251, 272, 292, 308, 320, 328, 0,   0,   0],
-#     [0,   10,  20,  34,  52,  C073,94,  115, 136, 157, C178,199, 220, 241, C262,283, 301, 315, 325, 0,   0,   0,   0],
-#     [0,   15,  27,  43,  63,  84,  105, 126, 147, 168, 189, 210, 231, 252, 273, 293, 309, 321, 0,   0,   0,   0,   0],
-#     [0,   21,  35,  53,  74,  95,  C116,137, 158, 179, 200, C221,242, 263, 284, 302, 316, 0,   0,   0,   0,   0,   0],
-#     [0,   28,  44,  64,  85,  106, 127, 148, C169,190, 211, 232, 253, 274, 294, 310, 0,   0,   0,   0,   0,   0,   0],
-#     [0,   36,  54,  75,  96,  117, 138, 159, 180, 201, 222, 243, 264, 285, 303, 0,   0,   0,   0,   0,   0,   0,   0],
-#     [0,   45,  65,  86,  107, 128, 149, 170, 191, 212, 233, 254, 275, 295, 0,   0,   0,   0,   0,   0,   0,   0,   0],
-#     [0,   55,  76,  97,  118, 139, 160, 181, 202, 223, 244, 265, 286, 0,   0,   0,   0,   0,   0,   0,   0,   0,   0],
-#     [0,   66,  87,  108, 129, 150, 171, 192, 213, 234, 255, 276, 0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0],
-#     [0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0]
-# ]
-
 TVSA_cells_numbers = [
     [0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0],
     [0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   56,  77,  98,  119, 140, 161, 182, 203, 224, 245, 266, 0],
     [0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   46,  67,  88,  109, 130, 151, 172, 193, 214, 235, 256, 277, 0],
     [0,   0,   0,   0,   0,   0,   0,   0,   0,   37,  57,  78,  99,  120, 141, 162, 183, 204, 225, 246, 267, 287, 0],
     [0,   0,   0,   0,   0,   0,   0,   0,   29,  47,  68,  89,  110, 131, 152, 173, 194, 215, 236, 257, 278, 296, 0],
     [0,   0,   0,   0,   0,   0,   0,   22,  38,  58,  79,  100, 121, 142, 163, 184, 205, 226, 247, 268, 288, 304, 0],
```

### Comparing `VVER-1000package-0.0.3/VVER1000package/absfabrics/Concentrations.py` & `VVER-1000package-0.0.4/VVER1000package/absfabrics/Concentrations.py`

 * *Files identical despite different names*

### Comparing `VVER-1000package-0.0.3/VVER1000package/data/MaterialsParameters.py` & `VVER-1000package-0.0.4/VVER1000package/data/MaterialsParameters.py`

 * *Files identical despite different names*

### Comparing `VVER-1000package-0.0.3/VVER1000package/data/nuclides_dict.pkl` & `VVER-1000package-0.0.4/VVER1000package/data/nuclides_dict.pkl`

 * *Files identical despite different names*

### Comparing `VVER-1000package-0.0.3/VVER1000package/data/nuclides_masses.pkl` & `VVER-1000package-0.0.4/VVER1000package/data/nuclides_masses.pkl`

 * *Files identical despite different names*

### Comparing `VVER-1000package-0.0.3/VVER_1000package.egg-info/SOURCES.txt` & `VVER-1000package-0.0.4/VVER_1000package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VVER-1000package-0.0.3/setup.py` & `VVER-1000package-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='VVER-1000package',
-    version='0.0.3',
+    version='0.0.4',
     description='Useful tools to work with Zmei calculation code',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     include_package_data = True,
     author='Vladislav Romanenko',
```

