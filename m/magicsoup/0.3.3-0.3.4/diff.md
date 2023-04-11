# Comparing `tmp/magicsoup-0.3.3.tar.gz` & `tmp/magicsoup-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.3.3.tar", last modified: Sat Apr  8 10:51:11 2023, max compression
+gzip compressed data, was "magicsoup-0.3.4.tar", last modified: Tue Apr 11 15:53:30 2023, max compression
```

## Comparing `magicsoup-0.3.3.tar` & `magicsoup-0.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-08 10:51:11.587141 magicsoup-0.3.3/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.3/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-08 10:51:11.587141 magicsoup-0.3.3/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.3/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.3/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-08 10:51:11.587141 magicsoup-0.3.3/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-08 10:51:11.583141 magicsoup-0.3.3/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-08 10:51:11.587141 magicsoup-0.3.3/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-08 10:50:58.000000 magicsoup-0.3.3/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.3/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.3/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-08 10:51:11.587141 magicsoup-0.3.3/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.3/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.3/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.3/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.3/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    11993 2023-04-06 09:43:57.000000 magicsoup-0.3.3/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    28797 2023-04-07 15:20:43.000000 magicsoup-0.3.3/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4140 2023-03-31 15:15:22.000000 magicsoup-0.3.3/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.3/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    42177 2023-04-08 10:23:19.000000 magicsoup-0.3.3/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-08 10:51:11.587141 magicsoup-0.3.3/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-08 10:51:11.000000 magicsoup-0.3.3/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-08 10:51:11.000000 magicsoup-0.3.3/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-08 10:51:11.000000 magicsoup-0.3.3/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-08 10:51:11.000000 magicsoup-0.3.3/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-08 10:51:11.587141 magicsoup-0.3.3/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.3/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.3/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.3/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.3/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    16060 2023-04-08 10:20:58.000000 magicsoup-0.3.3/tests/test_world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.4/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-11 15:53:30.558584 magicsoup-0.3.4/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.4/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.4/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-11 15:53:30.558584 magicsoup-0.3.4/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.554584 magicsoup-0.3.4/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.554584 magicsoup-0.3.4/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-11 15:53:18.000000 magicsoup-0.3.4/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.4/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.4/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.4/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.4/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.4/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.4/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    11993 2023-04-06 09:43:57.000000 magicsoup-0.3.4/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    28797 2023-04-07 15:20:43.000000 magicsoup-0.3.4/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4140 2023-03-31 15:15:22.000000 magicsoup-0.3.4/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.4/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    43105 2023-04-11 15:46:53.000000 magicsoup-0.3.4/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.4/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.4/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.4/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.4/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.4/tests/test_world.py
```

### Comparing `magicsoup-0.3.3/LICENSE` & `magicsoup-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/PKG-INFO` & `magicsoup-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.3/README.md` & `magicsoup-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/pyproject.toml` & `magicsoup-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/constants.py` & `magicsoup-0.3.4/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/containers.py` & `magicsoup-0.3.4/src/magicsoup/containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.3.4/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.3.4/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.3.4/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/genetics.py` & `magicsoup-0.3.4/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/kinetics.py` & `magicsoup-0.3.4/src/magicsoup/kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/mutations.py` & `magicsoup-0.3.4/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/util.py` & `magicsoup-0.3.4/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/src/magicsoup/world.py` & `magicsoup-0.3.4/src/magicsoup/world.py`

 * *Files 2% similar despite different names*

```diff
@@ -571,14 +571,40 @@
 
             # move cells
             new_pos = pxls[random.randint(0, n - 1)]
             self.cell_map[old_pos[0], old_pos[1]] = False
             self.cell_map[new_pos[0], new_pos[1]] = True
             self.cell_positions[cell_idx] = new_pos
 
+    def reposition_cells(self, cell_idxs: list[int]):
+        """
+        Reposition cells randomly on cell map without changing them.
+
+        Parameters:
+            cell_idxs: Indexes of cells that should be moved
+
+        Cells are removed from their current pixels on the cell map
+        and repositioned randomly on any free pixel on the cell map.
+        Only cell positions change (_e.g._ genomes, proteomes, cell molecules, cell indexes stay the same).
+        """
+        n_cells = len(cell_idxs)
+        if n_cells == 0:
+            return
+
+        old_xs = self.cell_positions[cell_idxs, 0]
+        old_ys = self.cell_positions[cell_idxs, 1]
+        self.cell_map[old_xs, old_ys] = False
+
+        new_pos = self._find_free_random_positions(n_cells=n_cells)
+        new_xs = new_pos[:, 0]
+        new_ys = new_pos[:, 1]
+
+        self.cell_map[new_xs, new_ys] = True
+        self.cell_positions[cell_idxs] = new_pos
+
     def enzymatic_activity(self):
         """
         Catalyze reactions for one time step.
         This includes molecule transport into or out of the cell.
         `world.molecule_map` and `world.cell_molecules` are updated.
         """
         if self.n_cells == 0:
```

### Comparing `magicsoup-0.3.3/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.3.4/src/magicsoup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.3/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.3.4/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/tests/test_containers.py` & `magicsoup-0.3.4/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/tests/test_genetics.py` & `magicsoup-0.3.4/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/tests/test_kinetics.py` & `magicsoup-0.3.4/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/tests/test_util.py` & `magicsoup-0.3.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.3/tests/test_world.py` & `magicsoup-0.3.4/tests/test_world.py`

 * *Files 14% similar despite different names*

```diff
@@ -469,7 +469,77 @@
     assert world.n_cells == 3
     assert world.cell_divisions[0] == 2
     assert world.cell_divisions[1] == 11
     assert world.cell_divisions[2] == 2
     assert world.cell_survival[0] == 1
     assert world.cell_survival[1] == 16
     assert world.cell_survival[2] == 1
+
+
+def test_reference_to_tensors_not_lost():
+    class A:
+        def __init__(self, world: ms.World):
+            self.world = world
+
+        def f(self, d: float):
+            self.world.molecule_map = torch.full_like(self.world.molecule_map, d)
+            self.world.cell_molecules = torch.full_like(self.world.cell_molecules, d)
+
+    chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
+    world = ms.World(chemistry=chemistry, map_size=3, mol_map_init="zeros")
+    world.add_cells(genomes=[ms.random_genome(s=500) for _ in range(2)])
+    a = A(world=world)
+
+    assert id(world.molecule_map) == id(a.world.molecule_map)
+    assert id(world.cell_molecules) == id(a.world.cell_molecules)
+    assert id(world.cell_map) == id(a.world.cell_map)
+    assert world.molecule_map.mean() == 0.0
+
+    world.diffuse_molecules()
+    world.enzymatic_activity()
+    world.degrade_molecules()
+
+    assert id(world.molecule_map) == id(a.world.molecule_map)
+    assert id(world.cell_molecules) == id(a.world.cell_molecules)
+    assert id(world.cell_map) == id(a.world.cell_map)
+
+    a.f(2.0)
+    assert id(world.molecule_map) == id(a.world.molecule_map)
+    assert id(world.cell_molecules) == id(a.world.cell_molecules)
+    assert id(world.cell_map) == id(a.world.cell_map)
+    assert world.molecule_map.mean() == 2.0
+
+    world.diffuse_molecules()
+    world.enzymatic_activity()
+    world.degrade_molecules()
+
+    assert id(world.molecule_map) == id(a.world.molecule_map)
+    assert id(world.cell_molecules) == id(a.world.cell_molecules)
+    assert id(world.cell_map) == id(a.world.cell_map)
+
+
+def test_reposition_cells():
+    chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
+    world = ms.World(chemistry=chemistry)
+    world.add_cells(genomes=[ms.random_genome(s=500) for _ in range(3)])
+
+    c0_0 = world.get_cell(by_idx=0)
+    c1_0 = world.get_cell(by_idx=1)
+    c2_0 = world.get_cell(by_idx=2)
+
+    world.reposition_cells(cell_idxs=[0, 2])
+    c0_1 = world.get_cell(by_idx=0)
+    c1_1 = world.get_cell(by_idx=1)
+    c2_1 = world.get_cell(by_idx=2)
+
+    assert c0_1.position != c0_0.position
+    assert c1_1.position == c1_0.position
+    assert c2_1.position != c2_0.position
+    assert (c0_1.int_molecules == c0_0.int_molecules).all()
+    assert (c1_1.int_molecules == c1_0.int_molecules).all()
+    assert (c2_1.int_molecules == c2_0.int_molecules).all()
+    assert c0_1.genome == c0_0.genome
+    assert c1_1.genome == c1_0.genome
+    assert c2_1.genome == c2_0.genome
+    assert c0_1.label == c0_0.label
+    assert c1_1.label == c1_0.label
+    assert c2_1.label == c2_0.label
```

