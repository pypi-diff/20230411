# Comparing `tmp/abml-0.1.5.tar.gz` & `tmp/abml-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abml-0.1.5.tar", max compression
+gzip compressed data, was "abml-0.1.6.tar", max compression
```

## Comparing `abml-0.1.5.tar` & `abml-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      586 2023-03-22 07:33:36.000000 abml-0.1.5/abml/__init__.py
--rw-r--r--   0        0        0    12263 2023-04-03 09:51:54.771609 abml-0.1.5/abml/abml_assembly.py
--rw-r--r--   0        0        0     3969 2023-03-22 07:48:31.000000 abml-0.1.5/abml/abml_bcs.py
--rw-r--r--   0        0        0        0 2023-03-27 09:39:35.423232 abml-0.1.5/abml/abml_config.py
--rw-r--r--   0        0        0     1280 2023-03-15 10:30:19.000000 abml-0.1.5/abml/abml_constraints.py
--rw-r--r--   0        0        0    18544 2023-04-07 14:37:44.840721 abml-0.1.5/abml/abml_dataclass.py
--rw-r--r--   0        0        0     6639 2023-04-05 08:01:55.000000 abml-0.1.5/abml/abml_helpers.py
--rw-r--r--   0        0        0     4223 2023-04-03 10:04:11.809675 abml-0.1.5/abml/abml_interaction_prop.py
--rw-r--r--   0        0        0     2678 2023-04-07 15:07:46.560016 abml-0.1.5/abml/abml_interactions.py
--rw-r--r--   0        0        0     5198 2023-03-28 12:54:48.000000 abml-0.1.5/abml/abml_jnl_loader.py
--rw-r--r--   0        0        0     2691 2023-04-07 15:17:38.239648 abml-0.1.5/abml/abml_jobs.py
--rw-r--r--   0        0        0     2028 2023-04-05 08:25:23.000000 abml-0.1.5/abml/abml_loads.py
--rw-r--r--   0        0        0     1680 2023-04-05 06:54:56.000000 abml-0.1.5/abml/abml_loggers.py
--rw-r--r--   0        0        0     4833 2023-03-30 12:29:52.222897 abml-0.1.5/abml/abml_materials.py
--rw-r--r--   0        0        0     6246 2023-03-30 14:44:49.120625 abml-0.1.5/abml/abml_mesh.py
--rw-r--r--   0        0        0    23005 2023-04-03 11:14:38.410167 abml-0.1.5/abml/abml_parts.py
--rw-r--r--   0        0        0      823 2023-03-14 07:49:32.000000 abml-0.1.5/abml/abml_sections.py
--rw-r--r--   0        0        0     4338 2023-04-05 07:47:19.000000 abml-0.1.5/abml/abml_sketch.py
--rw-r--r--   0        0        0      552 2023-03-14 09:57:29.000000 abml-0.1.5/abml/abml_steps.py
--rw-r--r--   0        0        0       22 2023-04-05 06:54:54.000000 abml-0.1.5/abml/logging.yaml
--rw-r--r--   0        0        0      381 2023-04-07 15:20:54.603904 abml-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-07 14:05:32.000000 abml-0.1.5/README.md
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 abml-0.1.5/setup.py
--rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 abml-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-04-08 14:31:24.000000 abml-0.1.6/abml/__init__.py
+-rw-r--r--   0        0        0    12263 2023-04-03 09:51:54.000000 abml-0.1.6/abml/abml_assembly.py
+-rw-r--r--   0        0        0     3969 2023-03-22 07:48:31.449857 abml-0.1.6/abml/abml_bcs.py
+-rw-r--r--   0        0        0        0 2023-03-27 09:39:35.000000 abml-0.1.6/abml/abml_config.py
+-rw-r--r--   0        0        0     1280 2023-03-15 10:30:19.422097 abml-0.1.6/abml/abml_constraints.py
+-rw-r--r--   0        0        0    18780 2023-04-11 06:35:31.492437 abml-0.1.6/abml/abml_dataclass.py
+-rw-r--r--   0        0        0     8020 2023-04-11 07:17:39.600876 abml-0.1.6/abml/abml_helpers.py
+-rw-r--r--   0        0        0     4223 2023-04-03 10:04:11.000000 abml-0.1.6/abml/abml_interaction_prop.py
+-rw-r--r--   0        0        0     2678 2023-04-07 15:07:46.000000 abml-0.1.6/abml/abml_interactions.py
+-rw-r--r--   0        0        0     5198 2023-03-28 12:54:48.239612 abml-0.1.6/abml/abml_jnl_loader.py
+-rw-r--r--   0        0        0     2691 2023-04-07 15:17:38.000000 abml-0.1.6/abml/abml_jobs.py
+-rw-r--r--   0        0        0     2028 2023-04-05 08:25:23.318715 abml-0.1.6/abml/abml_loads.py
+-rw-r--r--   0        0        0     1727 2023-04-08 14:04:31.000000 abml-0.1.6/abml/abml_loggers.py
+-rw-r--r--   0        0        0     4833 2023-03-30 12:29:52.000000 abml-0.1.6/abml/abml_materials.py
+-rw-r--r--   0        0        0     6246 2023-03-30 14:44:49.000000 abml-0.1.6/abml/abml_mesh.py
+-rw-r--r--   0        0        0    23347 2023-04-09 19:25:35.000000 abml-0.1.6/abml/abml_parts.py
+-rw-r--r--   0        0        0      823 2023-03-14 07:49:32.486729 abml-0.1.6/abml/abml_sections.py
+-rw-r--r--   0        0        0     6676 2023-04-11 07:11:20.706006 abml-0.1.6/abml/abml_sketch.py
+-rw-r--r--   0        0        0      552 2023-03-21 10:29:46.264400 abml-0.1.6/abml/abml_steps.py
+-rw-r--r--   0        0        0       22 2023-04-05 06:54:54.905037 abml-0.1.6/abml/logging.yaml
+-rw-r--r--   0        0        0      397 2023-04-11 07:34:16.484479 abml-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-07 14:05:32.882361 abml-0.1.6/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 abml-0.1.6/setup.py
+-rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 abml-0.1.6/PKG-INFO
```

### Comparing `abml-0.1.5/abml/__init__.py` & `abml-0.1.6/abml/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from . import abml_helpers  # noqa
 from . import abml_dataclass  # noqa
 from . import abml_jnl_loader  # noqa
-from . import abml_helpers  # noqa
 from . import abml_materials  # noqa
 from . import abml_sections  # noqa
 from . import abml_parts  # noqa
 from . import abml_sketch  # noqa
 from . import abml_assembly  # noqa
 from . import abml_mesh  # noqa
 from . import abml_steps  # noqa
```

### Comparing `abml-0.1.5/abml/abml_assembly.py` & `abml-0.1.6/abml/abml_assembly.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_bcs.py` & `abml-0.1.6/abml/abml_bcs.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_constraints.py` & `abml-0.1.6/abml/abml_constraints.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_dataclass.py` & `abml-0.1.6/abml/abml_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 from collections import OrderedDict
 from collections import defaultdict
 import sys
 import yaml
 from io import open
 from abaqus import mdb
 from abaqusConstants import STANDARD_EXPLICIT
-from abml import abml_helpers
 import interaction
 from abaqus import openMdb
+import logging
+import abml_helpers
+
+logger = logging.getLogger(__name__)
 
 
 class Abml_Registry:
     registry = defaultdict(lambda: OrderedDict)
 
     @classmethod
     def register(cls, key):
@@ -22,15 +25,15 @@
             cls.registry[key] = dataclass
             return dataclass
 
         return decorator
 
 
 @Abml_Registry.register("cae")
-class Abml_Cae:
+class Abml_Cae(abml_helpers.Abml_History):
     def __init__(self, models, **kwargs):
         self.kwargs = kwargs
 
         cae_path = self.kwargs.get("cae", None)
         cae_path = models.pop("cae") if "cae" in models else None
         if cae_path is not None:
             self.open_cae(cae_path)
@@ -176,20 +179,18 @@
 
     def create_sketches(self, **kwargs):
         sketches_list = [value for key, value in kwargs.items() if "sketches" in key]
         for sketches in sketches_list:
             if sketches is not None:
                 sketches = OrderedDict(sorted(sketches.items()))
 
-                sketch_name = sketches.keys()[0]
-                sketch_cmds = sketches.values()[0]
-
-                self.sketches.update(
-                    {sketch_name: to_object_cmd_mode(sketch_cmds, "sketch", model=self, name=sketch_name)}
-                )
+                for sketch_name, sketch_cmds in sketches.items():
+                    self.sketches.update(
+                        {sketch_name: to_object_cmd_mode(sketch_cmds, "sketch", model=self, name=sketch_name)}
+                    )
 
     def create_materials(self, **kwargs):
         materials_list = [value for key, value in kwargs.items() if "materials" in key]
         for materials in materials_list:
             if materials is not None:
                 materials = OrderedDict(sorted(materials.items()))
                 self.materials.update(to_object_key_mode(materials, "materials", model=self))
@@ -276,14 +277,19 @@
                 elif isinstance(modules, list):
                     for module in modules:
                         module = OrderedDict(sorted(module.items()))
                         self.create_instances(**module)
 
     def create(self):
         if self.name not in mdb.models.keys():
+            info = {
+                "call": "mdb.Model",
+                "kwargs": {"modelType": "STANDARD_EXPLICIT", "name": self.name},
+            }
+            logger.info(info)
             mdb.Model(modelType=STANDARD_EXPLICIT, name=self.name)
 
         if "Model-1" in mdb.models.keys():
             del mdb.models["Model-1"]
 
 
 def data_to_object(data, type_="models", key_based=True, **kwargs):
```

### Comparing `abml-0.1.5/abml/abml_helpers.py` & `abml-0.1.6/abml/abml_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from abaqus import mdb
 import sys
 import os
 import re
+from copy import deepcopy
 
 
 class IterReg(type):
     # Register of all objects for iteration
     def __iter__(cls):
         return iter(cls._reg.values())
 
 
+def is_iterable(obj):
+    try:
+        # Check if the object has __iter__ attribute
+        return hasattr(obj, "__iter__")
+    except TypeError:
+        return False
+
+
 class Abml_Helpers(object):
     """
     A utility class that provides helper methods for various tasks.
 
     Methods
     -------
     map_function(cls, key)
@@ -100,14 +109,22 @@
                 position_list = [position_list]
             elif depth_list == 0:
                 position_list = [position_list]
             return position_list
         return None
 
 
+class Abml_History:
+    def __init__(self):
+        self.call_history = {}
+
+    def get_call_history(self):
+        return self.call_history
+
+
 def exit_handler():
     """
     Deletes all files in the current directory with the extensions '.rpy', '.rec', and '.dmp' to clean up after program execution.
     """
     for file in os.listdir("."):
         if ".rpy" in file:
             try:
@@ -246,7 +263,43 @@
     p = m.parts
 
     return m, a, p
 
 
 def get_kwargs_string(**kwargs):
     return " ".join(["{}:{}".format(key, value) for key, value in kwargs.items()])
+
+
+def convert_kwargs_to_string(kwargs):
+    kwargs = deepcopy(kwargs)
+    for key in kwargs:
+        if is_iterable(kwargs[key]):
+            kwargs[key] = list(kwargs[key])
+        elif not isinstance(kwargs[key], (int, float)):
+            kwargs[key] = str(kwargs[key])
+
+    return kwargs
+
+
+# class FunctionHistory:
+#     history = []
+
+#     @classmethod
+#     def track_calls(cls, func):
+#         def wrapper(*args, **kwargs):
+#             cls.history.append((func.__name__, args, kwargs))
+#             return func(*args, **kwargs)
+
+#         return wrapper
+
+#     def print_history(self):
+#         history_str = "\n".join(
+#             [
+#                 "{}({}), {}".format(
+#                     call[0],
+#                     ", ".join([str(arg) for arg in call[1]]),
+#                     ", ".join([f"{key}={value}" for key, value in call[2].items()]),
+#                 )
+#                 for call in self.history
+#             ]
+#         )
+#         cprint(history_str)
```

### Comparing `abml-0.1.5/abml/abml_interaction_prop.py` & `abml-0.1.6/abml/abml_interaction_prop.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_interactions.py` & `abml-0.1.6/abml/abml_interactions.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_jnl_loader.py` & `abml-0.1.6/abml/abml_jnl_loader.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_jobs.py` & `abml-0.1.6/abml/abml_jobs.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_loads.py` & `abml-0.1.6/abml/abml_loads.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_loggers.py` & `abml-0.1.6/abml/abml_loggers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
-import logging.config
 
+# import logging.config
+
+logger = logging.getLogger("abml_logger")
 
 # debug_level = logging.CRITICAL
 
 # parts_logger = logging.getLogger("abml.parser")
 # parts_logger.addHandler(logging.FileHandler("parser.log", encoding="utf-8", mode="w"))
 # parts_logger.setLevel(debug_level)
 # parts_logger.propagate = False
```

### Comparing `abml-0.1.5/abml/abml_materials.py` & `abml-0.1.6/abml/abml_materials.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_mesh.py` & `abml-0.1.6/abml/abml_mesh.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_parts.py` & `abml-0.1.6/abml/abml_parts.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 from abaqusConstants import THREE_D, DEFORMABLE_BODY, XZPLANE  # noqa
 from abaqusConstants import XYPLANE, YZPLANE, XZPLANE  # noqa
 from abaqusConstants import MIDDLE_SURFACE, FROM_SECTION  # noqa
 from abaqusConstants import ON, OFF, STANDALONE  # noqa
 from regionToolset import Region
 from abml_dataclass import Abml_Registry
 from abml_dataclass import to_object_option_mode, to_object_key_mode, to_object_cmd_mode
-from abml_helpers import Abml_Helpers
+from abml_helpers import Abml_Helpers, Abml_History
 from abml_sketch import Abml_Sketch
 from numpy import array, abs
 from abaqus import mdb
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 @Abml_Registry.register("parts")
-class Abml_Part:
+class Abml_Part(Abml_History):
     """
     A class representing a part in an Abaqus/Explicit model.
 
     Parameters
     ----------
     name : str
         The name of the part.
@@ -138,15 +141,21 @@
         if isinstance(other, Abml_Part):
             for attr in dir(other):
                 if not attr.startswith("__") and not callable(getattr(other, attr)):
                     setattr(self, attr, getattr(other, attr))
 
     def create(self):
         if self.name not in self.model.parts.keys():
-            self.model.m.Part(dimensionality=THREE_D, name=self.name, type=DEFORMABLE_BODY)
+            kwargs = {"dimensionality": THREE_D, "name": self.name, "type": DEFORMABLE_BODY}
+            info = {
+                "call": 'mdb.models["{}"].Part'.format(self.model.name),
+                "kwargs": abml_helpers.convert_kwargs_to_string(kwargs),
+            }
+            logger.info(info)
+            self.model.m.Part(**kwargs)
 
     def get_sequence_from_set_list(self, set_list):
         face_seq = None
         cell_seq = None
         edge_seq = None
         for set_ in set_list:
             seq = self.model.p[self.name].sets[set_].faces
```

### Comparing `abml-0.1.5/abml/abml_sections.py` & `abml-0.1.6/abml/abml_sections.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/abml/abml_sketch.py` & `abml-0.1.6/abml/abml_sketch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import abml_helpers
 from abml.abml_dataclass import Abml_Registry
 from numpy import array
 from abaqusConstants import COUNTERCLOCKWISE, CLOCKWISE
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 @Abml_Registry.register("sketch")
 @Abml_Registry.register("sketches")
 class Abml_Sketch:
     def __init__(self, model, name="__profile__", **kwargs):
         self.model = model
@@ -24,72 +27,127 @@
             "autotrim": self._autotrim,
         }
 
         self.create()
 
     def create(self):
         if self.name not in self.model.m.sketches.keys():
-            self.model.m.ConstrainedSketch(name=self.name, sheetSize=200.0)
+            kwargs = {"name": self.name, "sheetSize": 200.0}
+            info = {
+                "call": 'mdb.models["{}"].ConstrainedSketch'.format(self.model.name),
+                "kwargs": kwargs,
+            }
+            logger.info(info)
+            self.model.m.ConstrainedSketch(**kwargs)
         self._sketch_reg.get(self.type, self._create_sketch_rect)(**self.kwargs)
 
         if "construction_line" in self.kwargs:
             self.create_construction_line()
 
     def create_construction_line(self):
         s = self.model.m.sketches[self.name]
         s.ConstructionLine(point1=(0.0, -100.0), point2=(0.0, 100.0))
 
     def _create_sketch_rect(self, p1, p2):
+        kwargs = {"point1": p1, "point2": p2}
+        info = {
+            "call": 'mdb.models["{}"].sketches["{}"].rectangle'.format(self.model.name, self.name),
+            "kwargs": kwargs,
+        }
+        logger.info(info)
         s = self.model.m.sketches[self.name]
-        s.rectangle(point1=p1, point2=p2)
+        s.rectangle(**kwargs)
 
     def _create_sketch_line(self, p1, p2):
+        kwargs = {"point1": p1, "point2": p2}
+        info = {
+            "call": 'mdb.models["{}"].sketches["{}"].Line'.format(self.model.name, self.name),
+            "kwargs": kwargs,
+        }
+        logger.info(info)
         s = self.model.m.sketches[self.name]
-        s.Line(point1=p1, point2=p2)
+        s.Line(**kwargs)
 
     def _create_sketch_pline(self, points):
         s = self.model.m.sketches[self.name]
         lines = create_lines_from_points(array(points))
         for line in lines:
-            s.Line(point1=line[0].astype(float), point2=line[1].astype(float))
+            kwargs = {"point1": line[0].astype(float), "point2": line[1].astype(float)}
+            info = {
+                "call": 'mdb.models["{}"].sketches["{}"].Line'.format(self.model.name, self.name),
+                "kwargs": abml_helpers.convert_kwargs_to_string(kwargs),
+            }
+            abml_helpers.cprint(info)
+            logger.info(info)
+            s.Line(**kwargs)
 
     def _create_sketch_circle(self, center, r):
+        kwargs = {"center": center, "point1": r}
+        info = {
+            "call": 'mdb.models["{}"].sketches["{}"].CircleByCenterPerimeter'.format(self.model.name, self.name),
+            "kwargs": kwargs,
+        }
+        logger.info(info)
         s = self.model.m.sketches[self.name]
-        s.CircleByCenterPerimeter(center=center, point1=r)
+        s.CircleByCenterPerimeter(**kwargs)
 
     def _create_sketch_ellipse(self, center, r1, r2):
+        kwargs = {"center": center, "axisPoint1": r1, "axisPoint2": r2}
+        info = {
+            "call": 'mdb.models["{}"].sketches["{}"].EllipseByCenterPerimeter'.format(self.model.name, self.name),
+            "kwargs": kwargs,
+        }
+        logger.info(info)
         s = self.model.m.sketches[self.name]
-        s.EllipseByCenterPerimeter(center=center, axisPoint1=r1, axisPoint2=r2)
+        s.EllipseByCenterPerimeter(**kwargs)
 
     def _create_sketch_arc_c2p(self, center, p1, p2, **kwargs):
         s = self.model.m.sketches[self.name]
 
         direction = kwargs.get("direction", "ccw")
 
         direction_reg = {
             "ccw": COUNTERCLOCKWISE,
             "counterclockwise": COUNTERCLOCKWISE,
             "cw": COUNTERCLOCKWISE,
             "clockwise": COUNTERCLOCKWISE,
         }
 
-        s.ArcByCenterEnds(center=center, point1=p1, point2=p2, direction=direction_reg[direction.lower()])
+        kwargs = {"center": center, "point1": p1, "point2": p2, "direction": direction_reg[direction.lower()]}
+        info = {
+            "call": 'mdb.models["{}"].sketches["{}"].ArcByCenterEnds'.format(self.model.name, self.name),
+            "kwargs": abml_helpers.convert_kwargs_to_string(kwargs),
+        }
+        logger.info(info)
+
+        s.ArcByCenterEnds(**kwargs)
 
     def _create_sketch_arc_3p(self, p1, p2, p3):
         s = self.model.m.sketches[self.name]
-
+        kwargs = {"point1": p1, "point2": p1, "point3": p3}
+        info = {
+            "call": 'mdb.models["{}"].sketches["{}"].Arc3Points'.format(self.model.name, self.name),
+            "kwargs": kwargs,
+        }
+        logger.info(info)
         s.Arc3Points(point1=p1, point2=p2, point3=p3)
 
     def _autotrim(self, p1):
         s = self.model.m.sketches[self.name]
 
         geometries = self._point_on_geometry(p1)
 
         for geometry in geometries:
-            s.autoTrimCurve(curve1=geometry, point1=p1, parameter1=None)  # noqq
+            kwargs = {"curve1": geometry, "point1": p1, "parameter1": None}
+            info = {
+                "call": 'mdb.models["{}"].sketches["{}"].Arc3Points'.format(self.model.name, self.name),
+                "kwargs": abml_helpers.convert_kwargs_to_string(kwargs),
+            }
+            logger.info(info)
+            s.autoTrimCurve(**kwargs)  # noqq
 
     def _point_on_geometry(self, p1):
         s = self.model.m.sketches[self.name]
         geometries = s.geometry
 
         geometry_list = []
         abml_helpers.cprint(geometries)
```

### Comparing `abml-0.1.5/abml/abml_steps.py` & `abml-0.1.6/abml/abml_steps.py`

 * *Files identical despite different names*

### Comparing `abml-0.1.5/setup.py` & `abml-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['abml']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyaml>=21.10.1,<22.0.0']
+['mock==3.0.5', 'pyaml>=21.10.1,<22.0.0']
 
 setup_kwargs = {
     'name': 'abml',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': '',
     'author': 'DavidNaizheZhou',
     'author_email': '70525024+DavidNaizheZhou@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

