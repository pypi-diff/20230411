# Comparing `tmp/PyNiteFEA-0.0.71.tar.gz` & `tmp/PyNiteFEA-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNiteFEA-0.0.71.tar", last modified: Thu Mar 16 15:21:09 2023, max compression
+gzip compressed data, was "PyNiteFEA-0.0.72.tar", last modified: Tue Apr 11 00:38:16 2023, max compression
```

## Comparing `PyNiteFEA-0.0.71.tar` & `PyNiteFEA-0.0.72.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:21:09.132059 PyNiteFEA-0.0.71/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-03-16 15:21:09.132059 PyNiteFEA-0.0.71/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:21:09.128059 PyNiteFEA-0.0.71/PyNite/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/BeamSegY.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/BeamSegZ.py
--rw-r--r--   0 runner    (1001) docker     (123)   152195 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/FEModel3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/FixedEndReactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/LoadCombo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/MainStyleSheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    78437 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Member3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    59347 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Node3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/PhysMember.py
--rw-r--r--   0 runner    (1001) docker     (123)    35578 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Plate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Quad3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Report_Template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Spring3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/PyNite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:21:09.132059 PyNiteFEA-0.0.71/PyNiteFEA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-03-16 15:21:09.000000 PyNiteFEA-0.0.71/PyNiteFEA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-16 15:21:09.000000 PyNiteFEA-0.0.71/PyNiteFEA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 15:21:09.000000 PyNiteFEA-0.0.71/PyNiteFEA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-16 15:21:09.000000 PyNiteFEA-0.0.71/PyNiteFEA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 15:21:09.000000 PyNiteFEA-0.0.71/PyNiteFEA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 15:21:09.132059 PyNiteFEA-0.0.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-16 15:20:56.000000 PyNiteFEA-0.0.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/PyNite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/BeamSegY.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/BeamSegZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152209 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/FEModel3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/FixedEndReactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/LoadCombo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/MainStyleSheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Member3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66665 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Node3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/PhysMember.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Plate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Quad3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Report_Template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Spring3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/PyNite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 00:38:16.000000 PyNiteFEA-0.0.72/PyNiteFEA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:38:16.870403 PyNiteFEA-0.0.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-11 00:38:04.000000 PyNiteFEA-0.0.72/setup.py
```

### Comparing `PyNiteFEA-0.0.71/LICENSE` & `PyNiteFEA-0.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PKG-INFO` & `PyNiteFEA-0.0.72/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.71
+Version: 0.0.72
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 </div>
 
 ![Build Status](https://github.com/JWock82/PyNite/actions/workflows/build-and-test.yml/badge.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyNiteFEA)
 <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/JWock82/PyNite">
 ![GitHub last commit](https://img.shields.io/github/last-commit/JWock82/PyNite)
 ![GitHub](https://img.shields.io/github/license/JWock82/PyNite)
+[![Documentation Status](https://readthedocs.org/projects/pynite/badge/?version=latest)](https://pynite.readthedocs.io/en/latest/?badge=latest)
 
 An easy to use elastic 3D structural engineering finite element analysis library for Python.
 
 # Installation
 The easiest way to install Pynite is with pip: `pip install PyNiteFEA`
 
 # Current Capabilities
@@ -88,14 +89,18 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.72
+* Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
+* Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
+
 v0.0.71
 * WARNING: This version will require reworking your models to incorporate `Materials`. Be prepared to rework your models before you upgrade. The examples have all been updated to show you how to do this.
 * Added `Material` definitions. This does not change Pynite's behavior much, but it prepares the way for future features.
 * Greatly simplified the process of meshing plates/quads. Meshes can now be generated directly from the `FEModel3D` object.
 * Added data types to the many dictionaries storing data in the `FEModel3D` object. Most development environments will now offer hints when using these dictionaries directly. This makes accessing the results you're interested in more intuitive.
 * Simplified internal code for finding unique names for objects.
```

### Comparing `PyNiteFEA-0.0.71/PyNite/BeamSegY.py` & `PyNiteFEA-0.0.72/PyNite/BeamSegY.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/BeamSegZ.py` & `PyNiteFEA-0.0.72/PyNite/BeamSegZ.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/FEModel3D.py` & `PyNiteFEA-0.0.72/PyNite/FEModel3D.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,19 @@
 from PyNite.Quad3D import Quad3D
 from PyNite.Plate3D import Plate3D
 from PyNite.LoadCombo import LoadCombo
 from PyNite.Mesh import Mesh, RectangleMesh, AnnulusMesh, FrustrumMesh, CylinderMesh
 
 # %%
 class FEModel3D():
-    """
-    A 3D finite element model.
+    """A 3D finite element model.
     """
 
     def __init__(self):
-
-        """
-        Returns a new 3D finite element model.
+        """Creates a new 3D finite element model.
         """
         
         # Initialize the model's various dictionaries. The dictionaries will be prepopulated with
         # the data types they store, and then those types will be removed. This will give us the
         # ability to get type-based hints when using the dictionaries.
 
         self.Nodes = {str:Node3D}          # A dictionary of the model's nodes
@@ -54,16 +51,15 @@
         self._D = {str:[]}                 # A dictionary of the model's nodal displacements by load combination
         self._D.pop(str)
         
         self.solution = None  # Indicates the solution type for the latest run of the model
 
     @property
     def LoadCases(self):
-        """
-        Returns a list of all the load cases in the model (in ascending order).
+        """Returns a list of all the load cases in the model (in alphabetical order).
         """
         
         # Create an empty list of load cases
         cases = []
 
         # Step through each node
         for node in self.Nodes.values():
@@ -90,39 +86,28 @@
                 # Get the load case for each plate/quad pressure
                 cases.append(load[1])
 
         # Remove duplicates and return the list (sorted ascending)
         return sorted(list(dict.fromkeys(cases)))
 
     def add_node(self, name, X, Y, Z):
-        """
-        Adds a new node to the model.
-
-        Parameters
-        ----------
-        name : string
-            A unique user-defined name for the node. If set to None or "" a
-            name will be automatically assigned.
-        X : number
-            The global X-coordinate of the node.
-        Y : number
-            The global Y-coordinate of the node.
-        Z : number
-            The global Z-coordinate of the node.
-
-        Raises
-        ------
-        NameError
-            Occurs when the specified name already exists in the model.
-
-        Returns
-        -------
-        name : string
-            The name of the node that was added to the model.
+        """Adds a new node to the model.
 
+        :param name: A unique user-defined name for the node. If set to None or "" a name will be
+                     automatically assigned.
+        :type name: str
+        :param X: The node's global X-coordinate.
+        :type X: number
+        :param Y: The node's global Y-coordinate.
+        :type Y: number
+        :param Z: The node's global Z-coordinate.
+        :type Z: number
+        :raises NameError: Occurs when the specified name already exists in the model.
+        :return: The name of the node added to the model.
+        :rtype: str
         """
         
         # Name the node or check it doesn't already exist
         if name:
             if name in self.Nodes:
                 raise NameError(f"Node name '{name}' already exists")
         else:
@@ -142,44 +127,32 @@
         # Flag the model as unsolved
         self.solution = None
 
         #Return the node name
         return name
 
     def add_auxnode(self, name, X, Y, Z):
-        """
-        Adds a new auxiliary node to the model.
-        
-        Together with a member's `i` and `j` nodes, an auxiliary node defines
-        the plane in which the member's local z-axis lies, and the side of the
-        member the z-axis point toward. If no auxiliary node is specified for
-        a member, PyNite uses its own default configuration.
-
-        Parameters
-        ----------
-        name : string
-            A unique user-defined name for the node. If None or "", a name will be automatically assigned
-        X : number
-            The global X-coordinate of the node.
-        Y : number
-            The global Y-coordinate of the node.
-        Z : number
-            The global Z-coordinate of the node.
-        
-        Raises
-        ------
-        NameError
-            Occurs when the specified name already exists in the model.
-
-        Returns
-        -------
-        name : string
-            The name of the auxiliary node that was added to the model.
-        
-        """
+        """Adds a new auxiliary node to the model. Together with a member's `i` and `j` nodes, an
+        auxiliary node defines the plane in which the member's local z-axis lies, and the side of
+        the member the z-axis points toward. If no auxiliary node is specified for a member, PyNite
+        uses its own default configuration.
+
+        :param name: A unique user-defined name for the node. If None or "", a name will be
+                     automatically assigned.
+        :type name: str
+        :param X: The global X-coordinate of the node.
+        :type X: number
+        :param Y: The global Y-coordinate of the node.
+        :type Y: number
+        :param Z: The global Z-coordinate of the node.
+        :type Z: number
+        :raises NameError: Occurs when the specified name already exists in the model.
+        :return: The name of the auxiliary node that was added to the model.
+        :rtype: str
+        """ 
         
         # Name the node or check it doesn't already exist
         if name:
             if name in self.AuxNodes:
                 raise NameError(f"Auxnode name '{name}' already exists")
         else:
             # As a guess, start with the length of the dictionary
@@ -198,29 +171,27 @@
         # Flag the model as unsolved
         self.solution = None
         
         #Return the node name
         return name 
 
     def add_material(self, name, E, G, nu, rho):
-        """
-        Adds a new material to the model.
+        """Adds a new material to the model.
 
-        Parameters
-        ----------
-        name : string
-            A unique user-defined name for the material
-        E : number
-            The modulus of elasticity of the material
-        G : number
-            The shear modulus of elasticity of the material
-        nu : number
-            Poisson's ratio of the material
-        rho : number
-            The density of the material
+        :param name: A unique user-defined name for the material.
+        :type name: str
+        :param E: The modulus of elasticity of the material.
+        :type E: number
+        :param G: The shear modulus of elasticity of the material.
+        :type G: number
+        :param nu: Poisson's ratio of the material.
+        :type nu: number
+        :param rho: The density of the material
+        :type rho: number
+        :raises NameError: Occurs when the specified name already exists in the model.
         """
 
         # Name the material or check it doesn't already exist
         if name:
             if name in self.Materials:
                 raise NameError(f"Material name '{name}' already exists")
         else:
@@ -237,44 +208,34 @@
         # Add the new material to the list
         self.Materials[name] = new_material
         
         # Flag the model as unsolved
         self.solution = None
 
     def add_spring(self, name, i_node, j_node, ks, tension_only=False, comp_only=False):
-        """
-        Adds a new spring to the model.
-        
-        Parameters
-        ----------
-        name : string
-            A unique user-defined name for the member. If None or "", a name will be automatically assigned
-        i_node : string
-            The name of the i-node (start node).
-        j_node : string
-            The name of the j-node (end node).
-        ks : number
-            The spring constant (force/displacement).
-        tension_only : bool, optional
-            Indicates if the member is tension-only. Default is False.
-        comp_only : bool, optional
-            Indicates if the member is compression-only. Default is False.
-        
-        Raises
-        ------
-        NameError
-            Occurs when the specified name already exists in the model.
-        
-        Returns
-        -------
-        name : string
-            The name of the spring that was added to the model.
-            
-        """
+        """Adds a new spring to the model.
 
+        :param name: A unique user-defined name for the member. If None or "", a name will be
+                    automatically assigned
+        :type name: str
+        :param i_node: The name of the i-node (start node).
+        :type i_node: str
+        :param j_node: The name of the j-node (end node).
+        :type j_node: str
+        :param ks: The spring constant (force/displacement).
+        :type ks: number
+        :param tension_only: Indicates if the member is tension-only, defaults to False
+        :type tension_only: bool, optional
+        :param comp_only: Indicates if the member is compression-only, defaults to False
+        :type comp_only: bool, optional
+        :raises NameError: Occurs when the specified name already exists in the model.
+        :return: The name of the spring that was added to the model.
+        :rtype: str
+        """ 
+        
         # Name the spring or check it doesn't already exist
         if name:
             if name in self.Springs:
                 raise NameError(f"Spring name '{name}' already exists")
         else:
             # As a guess, start with the length of the dictionary
             name = "S" + str(len(self.Springs))
@@ -295,44 +256,45 @@
         self.solution = None
 
         # Return the spring name
         return name
 
     def add_member(self, name, i_node, j_node, material, Iy, Iz, J, A, auxNode=None,
                    tension_only=False, comp_only=False):
-        '''
-        Adds a new physical member to the model. The member name will be returned.
-        
-        Parameters
-        ----------
-        name : string
-            A unique user-defined name for the member. If None or "", a name will be automatically assigned
-        i_node : string
-            The name of the i-node (start node).
-        j_node : string
-            The name of the j-node (end node).
-        material : string
-            The name of the material of the member.
-        Iy : number
-            The moment of inertia of the member about its local y-axis.
-        Iz : number
-            The moment of inertia of the member about its local z-axis.
-        J : number
-            The polar moment of inertia of the member.
-        A : number
-            The cross-sectional area of the member.
-        auxNode : string, optional
-            The name of the auxialary node used to define the local z-axis.
-            The default is for the program to define the axis instead of
-            using an auxiliary node.
-        tension_only : bool, optional
-            Indicates if the member is tension-only. Default is False.
-        comp_only : bool, optional
-            Indicates if the member is compression-only. Default is False.
-        '''
+        """Adds a new physical member to the model.
+
+        :param name: A unique user-defined name for the member. If None or "", a name will be
+                    automatically assigned
+        :type name: str
+        :param i_node: The name of the i-node (start node).
+        :type i_node: str
+        :param j_node: The name of the j-node (end node).
+        :type j_node: str
+        :param material: The name of the material of the member.
+        :type material: str
+        :param Iy: The moment of inertia of the member about its local y-axis.
+        :type Iy: number
+        :param Iz: The moment of inertia of the member about its local z-axis.
+        :type Iz: number
+        :param J: The polar moment of inertia of the member.
+        :type J: number
+        :param A: The cross-sectional area of the member.
+        :type A: number
+        :param auxNode: The name of the auxiliary node used to define the local z-axis. The default
+                        is None, in which case the program defines the axis instead of using an
+                        auxiliary node.
+        :type auxNode: str, optional
+        :param tension_only: Indicates if the member is tension-only, defaults to False
+        :type tension_only: bool, optional
+        :param comp_only: Indicates if the member is compression-only, defaults to False
+        :type comp_only: bool, optional
+        :raises NameError: Occurs if the specified name already exists.
+        :return: The name of the member added to the model.
+        :rtype: str
+        """
 
         # Name the member or check it doesn't already exist
         if name:
             if name in self.Members: raise NameError(f"Member name '{name}' already exists")
         else:
             # As a guess, start with the length of the dictionary
             name = "M" + str(len(self.Members))
@@ -343,58 +305,57 @@
                 
         # Create a new member
         if auxNode == None:
             new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J,
                                     A, model=self, tension_only=tension_only, comp_only=comp_only)
         else:
             new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J,
-                                    A, self.GetAuxNode(auxNode), model=self,
+                                    A, model=self, auxnode=self.GetAuxNode(auxNode),
                                     tension_only=tension_only, comp_only=comp_only)
         
         # Add the new member to the list
         self.Members[name] = new_member
         
         # Flag the model as unsolved
         self.solution = None
 
         # Return the member name
         return name
 
-    def add_plate(self, name, i_node, j_node, m_node, n_node, t, material, kx_mod=1, ky_mod=1):
-        """
-        Adds a new rectangular plate to the model.
-
-        The plate formulation for in-plane (membrane) stiffness is based on an isoparametric
-        formulation. For bending, it is based on a 12-term polynomial formulation. This element
-        must be rectangular, and must not be used where a thick plate formulation is needed. For
-        a more versatile plate element that can handle distortion and thick plate conditions,
-        consider using the `add_quad` method instead.
-        
-        Parameters
-        ----------
-        name : string
-            A unique user-defined name for the plate. If None or "", a name will be automatically assigned
-        i_node : string
-            The name of the i-node.
-        j_node : string
-            The name of the j-node.
-        m_node : string
-            The name of the m-node.
-        n_node : string
-            The name of the n-node.
-        t : number
-            The thickness of the element.
-        material : string
-            The name of the material for the element.
-        kx_mod : number
-            Stiffness modification factor for in-plane stiffness in the element's local
-            x-direction. Default value is 1.0 (no modification).
-        ky_mod : number
-            Stiffness modification factor for in-plane stiffness in the element's local
-            y-direction. Default value is 1.0 (no modification).
+    def add_plate(self, name, i_node, j_node, m_node, n_node, t, material, kx_mod=1.0, ky_mod=1.0):
+        """Adds a new rectangular plate to the model. The plate formulation for in-plane (membrane)
+        stiffness is based on an isoparametric formulation. For bending, it is based on a 12-term
+        polynomial formulation. This element must be rectangular, and must not be used where a
+        thick plate formulation is needed. For a more versatile plate element that can handle
+        distortion and thick plate conditions, consider using the `add_quad` method instead.
+
+        :param name: A unique user-defined name for the plate. If None or "", a name will be
+                     automatically assigned.
+        :type name: str
+        :param i_node: The name of the i-node.
+        :type i_node: str
+        :param j_node: The name of the j-node.
+        :type j_node: str
+        :param m_node: The name of the m-node.
+        :type m_node: str
+        :param n_node: The name of the n-node.
+        :type n_node: str
+        :param t: The thickness of the element.
+        :type t: number
+        :param material: The name of the material for the element.
+        :type material: str
+        :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local
+                       x-direction, defaults to 1 (no modification).
+        :type kx_mod: number, optional
+        :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local
+                       y-direction, defaults to 1 (no modification).
+        :type ky_mod: number, optional
+        :raises NameError: Occurs when the specified name already exists in the model.
+        :return: The name of the element added to the model.
+        :rtype: str
         """
         
         # Name the plate or check it doesn't already exist
         if name:
             if name in self.Plates: raise NameError(f"Plate name '{name}' already exists")
         else:
             # As a guess, start with the length of the dictionary
@@ -413,47 +374,47 @@
 
         # Flag the model as unsolved
         self.solution = None
         
         # Return the plate name
         return name
 
-    def add_quad(self, name, i_node, j_node, m_node, n_node, t, material, kx_mod=1, ky_mod=1):
-        """
-        Adds a new quadrilateral to the model.
-
-        The quad formulation for in-plane (membrane) stiffness is based on an isoparametric
-        formulation. For bending, it is based on an MITC4 formulation. This element handles
-        distortion relatively well, and is appropriate for thick and thin plates. One limitation
-        with this element is that it does a poor job of reporting corner stresses. Corner forces,
-        however are very accurate. Center stresses are very accurate as well. For cases where
-        corner stress results are important, consider using the `add_plate` method instead.
-        
-        Parameters
-        ----------
-        name : string
-            A unique user-defined name for the quadrilateral. If None or "", a name will be automatically assigned
-        i_node : string
-            The name of the i-node.
-        j_node : string
-            The name of the j-node.
-        m_node : string
-            The name of the m-node.
-        n_node : string
-            The name of the n-node.
-        t : number
-            The thickness of the element.
-        material : string
-            The name of the material for the element.
-        kx_mod : number
-            Stiffness modification factor for in-plane stiffness in the element's local
-            x-direction. Default value is 1.0 (no modification).
-        ky_mod : number
-            Stiffness modification factor for in-plane stiffness in the element's local
-            y-direction. Default value is 1.0 (no modification).
+    def add_quad(self, name, i_node, j_node, m_node, n_node, t, material, kx_mod=1.0, ky_mod=1.0):
+        """Adds a new quadrilateral to the model. The quad formulation for in-plane (membrane)
+        stiffness is based on an isoparametric formulation. For bending, it is based on an MITC4
+        formulation. This element handles distortion relatively well, and is appropriate for thick
+        and thin plates. One limitation with this element is that it does a poor job of reporting
+        corner stresses. Corner forces, however are very accurate. Center stresses are very
+        accurate as well. For cases where corner stress results are important, consider using the
+        `add_plate` method instead.
+
+        :param name: A unique user-defined name for the quadrilateral. If None or "", a name will
+                     be automatically assigned.
+        :type name: str
+        :param i_node: The name of the i-node.
+        :type i_node: str
+        :param j_node: The name of the j-node.
+        :type j_node: str
+        :param m_node: The name of the m-node.
+        :type m_node: str
+        :param n_node: The name of the n-node.
+        :type n_node: str
+        :param t: The thickness of the element.
+        :type t: number
+        :param material: The name of the material for the element.
+        :type material: str
+        :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local
+            x-direction, defaults to 1 (no modification).
+        :type kx_mod: number, optional
+        :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local
+            y-direction, defaults to 1 (no modification).
+        :type ky_mod: number, optional
+        :raises NameError: Occurs when the specified name already exists in the model.
+        :return: The name of the element added to the model.
+        :rtype: str
         """
         
         # Name the quad or check it doesn't already exist
         if name:
             if name in self.Quads: raise NameError(f"Quad name '{name}' already exists")
         else:
             # As a guess, start with the length of the dictionary
@@ -472,80 +433,77 @@
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the quad name
         return name
 
-    def add_rectangle_mesh(self, name, mesh_size, width, height, thickness, material, kx_mod=1, 
-            ky_mod=1, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node=None,
+    def add_rectangle_mesh(self, name, mesh_size, width, height, thickness, material, kx_mod=1.0, 
+            ky_mod=1.0, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node=None,
             start_element = None, element_type='Quad'):
-        """
-        Adds a rectangular mesh of elements to the model.
+        """Adds a rectangular mesh of elements to the model.
 
-        Parameters
-        ----------
-        name : string
-            A unique name for the mesh.
-        width : number
-            The overall width of the mesh measured along its local
-            x-axis.
-        height : number
-            The overall height of the mesh measured along its local
-            y-axis.
-        thickness : number
-            Element thickness.
-        material : string
-            The name of the element material.
-        kx_mod : number
-            Stiffness modification factor for in-plane stiffness in the
-            element's local x-direction. Default value is 1.0 (no
-            modification).
-        ky_mod : number
-            Stiffness modification factor for in-plane stiffness in the
-            element's local y-direction. Default value is 1.0 (no
-            modification).
-        origin : list, optional
-            The origin of the regtangular mesh's local coordinate
-            system. The default is [0, 0, 0].
-        plane : string, optional
-            The plane the mesh will be parallel to. Options are 'XY',
-            'YZ', and 'XZ'. The default is 'XY'.
-        x_control : list, optional
-            A list of control points along the mesh's local x-axis work
-            into the mesh.
-        y_control : list, optional
-            A list of control points along the mesh's local y-axis work
-            into the mesh.
-        start_node : string, optional
-            The name of the first node in the mesh. If set to `None` the program will use the next
-            available node name. Default is `None`
-        start_element : string, optional
-            The name of the first element in the mesh. If set to `None` the program will use the
-            next available element name. Default is `None`
-        element_type : string, optional
-            The type of element to make the mesh out of. Either 'Quad' or 'Rect'. The default is
-            'Quad'.
+        :param name: A unique name for the mesh.
+        :type name: str
+        :param mesh_size: The desired mesh size.
+        :type mesh_size: number
+        :param width: The overall width of the rectangular mesh measured along its local x-axis.
+        :type width: number
+        :param height: The overall height of the rectangular mesh measured along its local y-axis.
+        :type height: number
+        :param thickness: The thickness of each element in the mesh.
+        :type thickness: number
+        :param material: The name of the material for elements in the mesh.
+        :type material: str
+        :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local
+                       x-direction. Defaults to 1.0 (no modification).
+        :type kx_mod: float, optional
+        :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local
+                       y-direction. Defaults to 1.0 (no modification).
+        :type ky_mod: float, optional
+        :param origin: The origin of the regtangular mesh's local coordinate system. Defaults to [0, 0, 0]
+        :type origin: list, optional
+        :param plane: The plane the mesh will be parallel to. Options are 'XY', 'YZ', and 'XZ'.
+                      Defaults to 'XY'.
+        :type plane: str, optional
+        :param x_control: A list of control points along the mesh's local x-axis to work into the
+                          mesh. Defaults to `None`.
+        :type x_control: list, optional
+        :param y_control: A list of control points along the mesh's local y-axis to work into the
+                          mesh. Defaults to None.
+        :type y_control: list, optional
+        :param start_node: The name of the first node in the mesh. If set to `None` the program
+                           will use the next available node name. Default is `None`.
+        :type start_node: str, optional
+        :param start_element: The name of the first element in the mesh. If set to `None` the
+                              program will use the next available element name. Default is `None`.
+        :type start_element: str, optional
+        :param element_type: They type of element to make the mesh out of. Either 'Quad' or 'Rect'.
+                             Defaults to 'Quad'.
+        :type element_type: str, optional
+        :raises NameError: Occurs when the specified name already exists in the model.
+        :return: The name of the mesh added to the model.
+        :rtype: str
         """
         
         # Check if a mesh name has been provided
         if name:
             # Check that the mesh name isn't already being used
             if name in self.Meshes: raise NameError(f"Mesh name '{name}' already exists")
         # Rename the mesh if necessary
         else:
-            name = self._unique_name(self.Meshes, 'MSH')
+            name = self.unique_name(self.Meshes, 'MSH')
         
         # Identify the starting node and element
         if start_node is None:
-            start_node = self._unique_name(self.Nodes, 'N')
+            start_node = self.unique_name(self.Nodes, 'N')
         if element_type == 'Rect' and start_element is None:
-            start_element = self._unique_name(self.Plates, 'R')
+            start_element = self.unique_name(self.Plates, 'R')
         elif element_type == 'Quad' and start_element is None:
-            start_element = self._unique_name(self.Quads, 'Q')
+            start_element = self.unique_name(self.Quads, 'Q')
         
         # Create the mesh
         new_mesh = RectangleMesh(mesh_size, width, height, thickness, material, self, kx_mod,
                                  ky_mod, origin, plane, x_control, y_control, start_node,
                                  start_element, element_type=element_type)
 
         # Add the new mesh to the `Meshes` dictionary
@@ -553,66 +511,64 @@
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the mesh's name
         return name
     
-    def add_annulus_mesh(self, name, mesh_size, outer_radius, inner_radius, thickness, material, kx_mod=1, 
-            ky_mod=1, origin=[0, 0, 0], axis='Y', start_node=None, start_element=None):
-        """
-        Adds a mesh of quadrilaterals forming an annulus (a donut).
-
-        Parameters
-        ----------
-        name : string
-            A unique name for the mesh.
-        mesh_size : number
-            The target mesh size
-        outer_radius : number
-            The radius to the outside of the annulus.
-        inner_radius : number
-            The radius to the inside of the annulus.
-        thickness : number
-            Element thickness.
-        material : string
-            The name of the element material.
-        kx_mod : number
-            Stiffness modification factor for radial stiffness in the
-            element's local x-direction. Default value is 1.0 (no
-            modification).
-        ky_mod : number
-            Stiffness modification factor for meridional stiffness in the
-            element's local y-direction. Default value is 1.0 (no
-            modification).
-        origin : list, optional
-            The origin of the mesh. The default is [0, 0, 0].
-        axis : string, optional
-            The global axis about which the mesh will be generated. The default is 'Y'.
-        start_node : string, optional
-            The name of the first node in the mesh. If set to `None` the program will use the next
-            available node name. Default is `None`
-        start_element : string, optional
-            The name of the first element in the mesh. If set to `None` the program will use the
-            next available element name. Default is `None`
+    def add_annulus_mesh(self, name, mesh_size, outer_radius, inner_radius, thickness, material, kx_mod=1.0, 
+            ky_mod=1.0, origin=[0, 0, 0], axis='Y', start_node=None, start_element=None):
+        """Adds a mesh of quadrilaterals forming an annulus (a donut).
+
+        :param name: A unique name for the mesh.
+        :type name: str
+        :param mesh_size: The target mesh size.
+        :type mesh_size: float
+        :param outer_radius: The radius to the outside of the annulus.
+        :type outer_radius: float
+        :param inner_radius: The radius to the inside of the annulus.
+        :type inner_radius: float
+        :param thickness: Element thickness.
+        :type thickness: float
+        :param material: The name of the element material.
+        :type material: str
+        :param kx_mod: Stiffness modification factor for radial stiffness in the element's local
+                       x-direction. Default is 1.0 (no modification).
+        :type kx_mod: float, optional
+        :param ky_mod: Stiffness modification factor for meridional stiffness in the element's
+                       local y-direction. Default is 1.0 (no modification).
+        :type ky_mod: float, optional
+        :param origin: The origin of the mesh. The default is [0, 0, 0].
+        :type origin: list, optional
+        :param axis: The global axis about which the mesh will be generated. The default is 'Y'.
+        :type axis: str, optional
+        :param start_node: The name of the first node in the mesh. If set to `None` the program
+                           will use the next available node name. Default is `None`.
+        :type start_node: str, optional
+        :param start_element: The name of the first element in the mesh. If set to `None` the
+                              program will use the next available element name. Default is `None`.
+        :type start_element: str, optional
+        :raises NameError: Occurs if the specified name already exists in the model.
+        :return: The name of the mesh added to the model.
+        :rtype: str
         """
         
         # Check if a mesh name has been provided
         if name:
             # Check that the mesh name doesn't already exist
             if name in self.Meshes: raise NameError(f"Mesh name '{name}' already exists")
         # Give the mesh a new name if necessary
         else:
-            name = self._unique_name(self.Meshes, 'MSH')
+            name = self.unique_name(self.Meshes, 'MSH')
 
         # Identify the starting node and element
         if start_node is None:
-            start_node = self._unique_name(self.Nodes, 'N')
+            start_node = self.unique_name(self.Nodes, 'N')
         if start_element is None:
-            start_element = self._unique_name(self.Quads, 'Q')
+            start_element = self.unique_name(self.Quads, 'Q')
         
         # Create a new mesh
         new_mesh = AnnulusMesh(mesh_size, outer_radius, inner_radius, thickness, material, self,
                                kx_mod, ky_mod, origin, axis, start_node, start_element)
 
         # Add the new mesh to the `Meshes` dictionary
         self.Meshes[name] = new_mesh
@@ -620,69 +576,67 @@
         # Flag the model as unsolved
         self.solution = None
         
         #Return the mesh's name
         return name
 
     def add_frustrum_mesh(self, name, mesh_size, large_radius, small_radius, height, thickness,
-                          material, kx_mod=1, ky_mod=1, origin=[0, 0, 0], axis='Y',
+                          material, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], axis='Y',
                           start_node=None, start_element=None):
-        """
-        Adds a mesh of quadrilaterals forming a frustrum (a cone intersected by
-        a horizontal plane).
+        """Adds a mesh of quadrilaterals forming a frustrum (a cone intersected by a horizontal
+        plane).
 
-        Parameters
-        ----------
-        name : string
-            A unique name for the mesh.
-        mesh_size : number
-            The target mesh size
-        large_radius : number
-            The larger of the two end radii.
-        small_radius : number
-            The smaller of the two end radii.
-        height : number
-            The height of the frustrum.
-        thickness : number
-            Element thickness.
-        material : string
-            The name of the element material.
-        kx_mod : number
-            Stiffness modification factor for radial stiffness in each
-            element's local x-direction. Default value is 1.0 (no
-            modification).
-        ky_mod : number
-            Stiffness modification factor for meridional stiffness in each
-            element's local y-direction. Default value is 1.0 (no
-            modification).
-        origin : list, optional
-            The origin of the mesh. The default is [0, 0, 0].
-        axis : string, optional
-            The global axis about which the mesh will be generated. The default is 'Y'.
-        start_node : string, optional
-            The name of the first node in the mesh. If set to `None` the program will use the next
-            available node name. Default is `None`
-        start_element : string, optional
-            The name of the first element in the mesh. If set to `None` the program will use the
-            next available element name. Default is `None`
+        :param name: A unique name for the mesh.
+        :type name: str
+        :param mesh_size: The target mesh size
+        :type mesh_size: number
+        :param large_radius: The larger of the two end radii.
+        :type large_radius: number
+        :param small_radius: The smaller of the two end radii.
+        :type small_radius: number
+        :param height: The height of the frustrum.
+        :type height: number
+        :param thickness: The thickness of the elements.
+        :type thickness: number
+        :param material: The name of the element material.
+        :type material: str
+        :param kx_mod: Stiffness modification factor for radial stiffness in each element's local
+                       x-direction, defaults to 1 (no modification).
+        :type kx_mod: number, optional
+        :param ky_mod: Stiffness modification factor for meridional stiffness in each
+                       element's local y-direction, defaults to 1 (no modification).
+        :type ky_mod: number, optional
+        :param origin: The origin of the mesh, defaults to [0, 0, 0].
+        :type origin: list, optional
+        :param axis: The global axis about which the mesh will be generated, defaults to 'Y'.
+        :type axis: str, optional
+        :param start_node: The name of the first node in the mesh. If set to None the program
+                           will use the next available node name, defaults to None.
+        :type start_node: str, optional
+        :param start_element: The name of the first element in the mesh. If set to `None` the
+                              program will use the next available element name, defaults to None
+        :type start_element: str, optional
+        :raises NameError: Occurs if the specified name already exists.
+        :return: The name of the mesh added to the model.
+        :rtype: str
         """
-        
+
         # Check if a name has been provided
         if name:
             # Check that the mesh name doesn't already exist
             if name in self.Meshes: raise NameError(f"Mesh name '{name}' already exists")
         # Give the mesh a new name if necessary
         else:
-            name = self._unique_name(self.Meshes, 'MSH')
+            name = self.unique_name(self.Meshes, 'MSH')
 
         # Identify the starting node and element
         if start_node is None:
-            start_node = self._unique_name(self.Nodes, 'N')
+            start_node = self.unique_name(self.Nodes, 'N')
         if start_element is None:
-            start_element = self._unique_name(self.Quads, 'Q')
+            start_element = self.unique_name(self.Quads, 'Q')
         
         # Create a new mesh
         new_mesh = FrustrumMesh(mesh_size, large_radius, small_radius, height, thickness, material,
                                 self, kx_mod, ky_mod, origin, axis, start_node, start_element)
 
         # Add the new mesh to the `Meshes` dictionary
         self.Meshes[name] = new_mesh
@@ -697,70 +651,70 @@
                           ky_mod=1, origin=[0, 0, 0], axis='Y', num_elements=None, start_node=None,
                           start_element=None, element_type='Quad'):
         """
         Adds a mesh of elements forming a cylinder.
 
         Parameters
         ----------
-        name : string
+        name : str
             A unique name for the mesh.
         mesh_size : number
             The target mesh size
         radius : number
             The radius of the cylinder.
         height : number
             The height of the cylinder.
         thickness : number
             Element thickness.
-        material : string
+        material : str
             The name of the element material.
         kx_mod : number
             Stiffness modification factor for hoop stiffness in each
             element's local x-direction. Default value is 1.0 (no
             modification).
         ky_mod : number
             Stiffness modification factor for meridional stiffness in each
             element's local y-direction. Default value is 1.0 (no
             modification).
         origin : list, optional
             The origin of the mesh. The default is [0, 0, 0].
-        axis : string, optional
+        axis : str, optional
             The global axis about which the mesh will be generated. The default is 'Y'.
         num_elements : number
             The number of elements to use to form the perimeter of each course. This is typically
             only used if you are trying to match the nodes to another mesh's nodes. If set to
             `None` the program will automatically calculate the number of elements to use based on
             the mesh size. The default is None.
-        start_node : string
+        start_node : str
             The name of the first node in the mesh. If set to `None` the program will use the next
             available node name. Default is `None`
-        start_element : string
+        start_element : str
             The name of the first element in the mesh. If set to `None` the program will use the
             next available element name. Default is `None`
-        element_type : string, optional
+        element_type : str, optional
             The type of element to make the mesh out of. Either 'Quad' or 'Rect'. The default is
             'Quad'.
 
         """
         
         # Check if a name has been provided
         if name:
             # Check that the mesh name doesn't already exist
             if name in self.Meshes: raise NameError(f"Mesh name '{name}' already exists")
         # Give the mesh a new name if necessary
         else:
-            name = self._unique_name(self.Meshes, 'MSH')
+            name = self.unique_name(self.Meshes, 'MSH')
 
         # Identify the starting node and element
         if start_node is None:
-            start_node = self._unique_name(self.Nodes, 'N')
+            start_node = self.unique_name(self.Nodes, 'N')
         if element_type == 'Rect' and start_element is None:
-            start_element = self._unique_name(self.Plates, 'R')
+            start_element = self.unique_name(self.Plates, 'R')
         elif element_type == 'Quad' and start_element is None:
-            start_element = self._unique_name(self.Quads, 'Q')
+            start_element = self.unique_name(self.Quads, 'Q')
         
         # Create a new mesh
         new_mesh = CylinderMesh(mesh_size, radius, height, thickness, material, self,
                                kx_mod, ky_mod, origin, axis, start_node, start_element,
                                num_elements, element_type)
 
         # Add the new mesh to the `Meshes` dictionary
@@ -787,67 +741,78 @@
             A list of th enames of the nodes that were removed.
         """
 
         # Initialize a list of nodes to be removed from the `Nodes` dictionary
         node_remove_list = []
 
         # Initialize a dictionary marking where each node is used
-        node_lookup = {node: [] for node in self.Nodes.values()}
+        node_lookup = {node_name: [] for node_name in self.Nodes.keys()}
         element_dicts = ('Springs', 'Members', 'Plates', 'Quads')
         node_types = ('i_node', 'j_node', 'm_node', 'n_node')
 
-        # Step through each dictionary of elements in the model (springs, member, plates, quads)
+        # Step through each dictionary of elements in the model (springs, members, plates, quads)
         for element_dict in element_dicts:
 
             # Step through each element in the dictionary
             for element in getattr(self, element_dict).values():
 
                 # Step through each possible node type in the element (i-node, j-node, m-node, n-node)
                 for node_type in node_types:
 
                     # Get the current element's node having the current type
                     # Return `None` if the element doesn't have this node type
                     node = getattr(element, node_type, None)
 
                     # Determine if the node exists on the element
-                    if node:
-
+                    if node is not None:
                         # Add the element to the list of elements attached to the node
-                        node_lookup[node].append((element, node_type))
+                        node_lookup[node.name].append((element, node_type))
 
         # Make a copy of the `Nodes` dictionary
         temp = list(self.Nodes.values())
 
-        # Step through each node in the `Nodes` dictionary
+        # Step through each node in the copy of the `Nodes` dictionary
         for i, node_1 in enumerate(temp):
 
             # Skip iteration if `node_1` has already been removed
-            if node_lookup[node_1] is None:
+            if node_lookup[node_1.name] is None:
                 continue
 
             # There is no need to check `node_1` against itself
             for node_2 in temp[i + 1:]:
 
                 # Skip iteration if node_2 has already been removed
-                if node_lookup[node_2] is None:
+                if node_lookup[node_2.name] is None:
                     continue
 
                 # Calculate the distance between nodes
                 if self.Nodes[node_1.name].distance(self.Nodes[node_2.name]) > tolerance:
                     continue
 
-                # Overwrite node_2
-                for element, node_type in node_lookup[node_2]:
+                # Replace references to `node_2` in each element with references to `node_1`
+                for element, node_type in node_lookup[node_2.name]:
                     setattr(element, node_type, node_1)
 
+                # Replace references to `node_2` in each mesh with references to `node_1`
+                for mesh in self.Meshes.values():
+
+                    if node_2.name in mesh.nodes.keys():
+                        mesh.nodes[node_2.name] = node_1
+
+                    for element in mesh.elements.values():
+                        if element.i_node is node_2: element.i_node = node_1
+                        if element.j_node is node_2: element.j_node = node_1
+                        if element.m_node is node_2: element.m_node = node_1
+                        if element.n_node is node_2: element.n_node = node_1
+
                 # Mark `node_2` for removal from the `Nodes` dictionary
                 node_remove_list.append(node_2.name)
 
                 # Flag `node_2` as not used
-                node_lookup[node_2] = None
+                node_lookup[node_2.name] = None
 
                 # Merge any boundary conditions
                 support_cond = ('support_DX', 'support_DY', 'support_DZ', 'support_RX', 'support_RY', 'support_RZ')
                 for dof in support_cond:
                     if getattr(node_2, dof) == True:
                         setattr(node_1, dof, True)
                 
@@ -871,15 +836,15 @@
     def delete_node(self, node_name):
         '''
         Removes a node from the model. All nodal loads associated with the
         node and elements attached to the node will also be removed.
         
         Parameters
         ----------
-        node_name : string
+        node_name : str
             The name of the node to be removed.
         '''
         
         # Remove the node. Nodal loads are stored within the node, so they
         # will be deleted automatically when the node is deleted.
         self.Nodes.pop(node_name)
         
@@ -893,15 +858,15 @@
 
     def delete_auxnode(self, auxnode_name):
         '''
         Removes an auxiliary node from the model.
 
         Parameters
         ----------
-        auxnode_name : string
+        auxnode_name : str
             The name of the auxiliary node to be removed
         '''
 
         # Remove the auxiliary node
         self.AuxNodes.pop(auxnode_name)
 
         # Remove the auxiliary node from any members that were using it
@@ -914,15 +879,15 @@
 
     def delete_spring(self, spring_name):
         '''
         Removes a spring from the model.
         
         Parameters
         ----------
-        spring_name : string
+        spring_name : str
             The name of the spring to be removed.
         '''
         
         # Remove the spring
         self.Springs.pop(spring_name)
 
         # Flag the model as unsolved
@@ -931,49 +896,50 @@
     def delete_member(self, member_name):
         '''
         Removes a member from the model. All member loads associated with the
         member will also be removed.
         
         Parameters
         ----------
-        member_name : string
+        member_name : str
             The name of the member to be removed.
         '''
         
         # Remove the member. Member loads are stored within the member, so they
         # will be deleted automatically when the member is deleted.
         self.Members.pop(member_name)
 
         # Flag the model as unsolved
         self.solution = None
         
     def def_support(self, node_name, support_DX=False, support_DY=False, support_DZ=False, support_RX=False, support_RY=False, support_RZ=False):
-        """
-        Defines the support conditions at a node.
-        
-        Nodes will default to fully unsupported unless specified otherwise.
-        
-        Parameters
-        ----------
-        node_name : string
-            The name of the node where the support is being defined
-        support_DX : bool
-            Indicates whether the node is supported against translation in the global X-direction.
-        support_DY : bool
-            Indicates whether the node is supported against translation in the global Y-direction.
-        support_DZ : bool
-            Indicates whether the node is supported against translation in the global Z-direction.
-        support_RX : bool
-            Indicates whether the node is supported against rotation about the global X-axis.
-        support_RY : bool
-            Indicates whether the node is supported against rotation about the global Y-axis.
-        support_RZ : bool
-            Indicates whether the node is supported against rotation about the global Z-axis.
-            
-        """
+        """Defines the support conditions at a node. Nodes will default to fully unsupported
+           unless specified otherwise.
+
+        :param node_name: The name of the node where the support is being defined.
+        :type node_name: str
+        :param support_DX: Indicates whether the node is supported against translation in the
+                           global X-direction. Defaults to False.
+        :type support_DX: bool, optional
+        :param support_DY: Indicates whether the node is supported against translation in the
+                           global Y-direction. Defaults to False.
+        :type support_DY: bool, optional
+        :param support_DZ: Indicates whether the node is supported against translation in the
+                           global Z-direction. Defaults to False.
+        :type support_DZ: bool, optional
+        :param support_RX: Indicates whether the node is supported against rotation about the
+                           global X-axis. Defaults to False.
+        :type support_RX: bool, optional
+        :param support_RY: Indicates whether the node is supported against rotation about the
+                           global Y-axis. Defaults to False.
+        :type support_RY: bool, optional
+        :param support_RZ: Indicates whether the node is supported against rotation about the
+                           global Z-axis. Defaults to False.
+        :type support_RZ: bool, optional
+        """            
         
         # Get the node to be supported
         node = self.Nodes[node_name]
                 
         # Set the node's support conditions
         node.support_DX = support_DX
         node.support_DY = support_DY
@@ -987,21 +953,21 @@
 
     def def_support_spring(self, node_name, dof, stiffness, direction=None):
         """
         Defines a spring support at a node.
 
         Parameters
         ----------
-        node_name : string
+        node_name : str
             The name of the node to apply the spring support to.
-        dof : string ('DX', 'DY', 'DZ', 'RX', 'RY', or 'RZ')
+        dof : str ('DX', 'DY', 'DZ', 'RX', 'RY', or 'RZ')
             The degree of freedom to apply the spring support to.
         stiffness : number
             The translational or rotational stiffness of the spring support.
-        direction : string or None ('+', '-', None)
+        direction : str or None ('+', '-', None)
             The direction in which the spring can act. '+' allows the spring
             to resist positive displacements. '-' allows the spring to resist
             negative displacements. None allows the spring to act in both
             directions. Default is None.
         """
         
         if dof in ('DX', 'DY', 'DZ', 'RX', 'RY', 'RZ'):
@@ -1026,17 +992,17 @@
         # Flag the model as unsolved
         self.solution = None
 
     def def_node_disp(self, node_name, direction, magnitude): 
         '''
         Defines a nodal displacement at a node.
 
-        node_name : string
+        node_name : str
             The name of the node where the nodal displacement is being applied.
-        direction : string
+        direction : str
             The global direction the nodal displacement is being applied in. Displacements are 'DX', 'DY', and 'DZ'. Rotations are 'RX', 'RY', and 'RZ'.
         magnitude : number
             The magnitude of the displacement.
         '''
         # Validate the value of Direction
         if direction not in ('DX', 'DY', 'DZ', 'RX', 'RY', 'RZ'):
             raise ValueError(f"Direction must be 'DX', 'DY', 'DZ', 'RX', 'RY', or 'RZ'. {direction} was given.")
@@ -1063,15 +1029,15 @@
         '''
         Defines member end releases.
         
         All member end releases will default to unreleased unless specified otherwise.
         
         Parameters
         ----------
-        Member : string
+        Member : str
             The name of the member to have its releases modified.
         Dxi : boolean
             Indicates whether the member is released axially at its start.
         Dyi : boolean
             Indicates whether the member is released for shear in the local y-axis at its start.
         Dzi : boolean
             Indicates whether the member is released for shear in the local z-axis at its start.
@@ -1103,19 +1069,19 @@
 
     def add_load_combo(self, name, factors, combo_type='strength'):
         '''
         Adds a load combination to the model
 
         Parameters
         ----------
-        name : string
+        name : str
             A unique name for the load combination (e.g. '1.2D+1.6L+0.5S' or 'Gravity Combo').
         factors : dictionary
             A dictionary containing load cases and their corresponding factors (e.g. {'D':1.2, 'L':1.6, 'S':0.5}).
-        combo_type : string
+        combo_type : str
             A description of the type of load combination (e.g. 'strength', 'service'). Currently
             this does nothing in the program, and is a placeholder for future features.
         '''
 
         # Create a new load combination object
         new_combo = LoadCombo(name, combo_type, factors)
 
@@ -1127,21 +1093,21 @@
 
     def add_node_load(self, Node, Direction, P, case='Case 1'):
         '''
         Adds a nodal load to the model.
         
         Parameters
         ----------
-        Node : string
+        Node : str
             The name of the node where the load is being applied.
         Direction : {'FX', 'FY', 'FZ', 'MX', 'MY', 'MZ'}
             The global direction the load is being applied in. Forces are 'FX', 'FY', and 'FZ'. Moments are 'MX', 'MY', and 'MZ'.
         P : number
             The numeric value (magnitude) of the load.
-        case : string
+        case : str
             The name of the load case the load belongs to.
         '''
         # Validate the value of Direction
         if Direction not in ('FX', 'FY', 'FZ', 'MX', 'MY', 'MZ'):
             raise ValueError(f"Direction must be 'FX', 'FY', 'FZ', 'MX', 'MY', or 'MZ'. {Direction} was given.")
         # Add the node load to the model
         self.Nodes[Node].NodeLoads.append((Direction, P, case))
@@ -1151,15 +1117,15 @@
 
     def add_member_pt_load(self, Member, Direction, P, x, case='Case 1'):
         '''
         Adds a member point load to the model.
         
         Parameters
         ----------
-        Member : string
+        Member : str
             The name of the member the load is being applied to.
         Direction : {'Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz'}
             The direction in which the force is to be applied. Note that
             typical beam sign convention is used. Transverse forces acting
             toward the beam are positive. Moments are positive if they act
             counter-clockwise relative to the beam's local coordinate system.
             Torsional point loads follow the right hand rule for sign convention.
@@ -1181,15 +1147,15 @@
 
     def add_member_dist_load(self, Member, Direction, w1, w2, x1=None, x2=None, case='Case 1'):
         '''
         Adds a member distributed load to the model.
         
         Parameters
         ----------
-        Member : string
+        Member : str
             The name of the member the load is being appied to
         Direction : {'Fx', 'Fy', 'Fz'}
             The direction in which the load is to be applied. Note that
             typical beam sign convention is used. Forces acting toward the beam
             are positive.
         w1 : number
             The starting value (magnitude) of the load.
@@ -1225,19 +1191,19 @@
 
     def add_plate_surface_pressure(self, plate_name, pressure, case='Case 1'):
         """
         Adds a surface pressure to the rectangular plate element.
 
         Parameters
         ----------
-        plate_name : string
+        plate_name : str
             The name for the rectangular plate to add the surface pressure to.
         pressure : number
             The value for the surface pressure.
-        case : string, optional
+        case : str, optional
             The load case to add the surface pressure to. Default is 'Case 1'.
         
         """
 
         # Add the surface pressure to the rectangle
         if plate_name in self.Plates.keys():
             self.Plates[plate_name].pressures.append([pressure, case])
@@ -1249,19 +1215,19 @@
 
     def add_quad_surface_pressure(self, quad_name, pressure, case='Case 1'):
         """
         Adds a surface pressure to the quadrilateral element.
 
         Parameters
         ----------
-        quad_name : string
+        quad_name : str
             The name for the quad to add the surface pressure to.
         pressure : number
             The value for the surface pressure.
-        case : string, optional
+        case : str, optional
             The load case to add the surface pressure to. Default is 'Case 1'.
         
         """
 
         # Add the surface pressure to the quadrilateral
         if quad_name in self.Quads.keys():
             self.Quads[quad_name].pressures.append([pressure, case])
@@ -1310,136 +1276,23 @@
             node.RxnMX = {}
             node.RxnMY = {}
             node.RxnMZ = {}
         
         # Flag the model as unsolved
         self.solution = None
 
-    def GetNode(self, name):
-        '''
-        Returns the node with the given name.
-        
-        Parameters
-        ----------
-        name : string
-            The name of the node to be returned.
-        '''
-        
-        warnings.warn('`GetNode` will be deleted in a future version of PyNite. Use `Nodes[node_name]` instead.', FutureWarning)
-
-        try:
-            return self.Nodes[name]
-        except:
-            # If the node name is not found
-            raise ValueError(f"Node '{name}' was not found in the model.")
-         
-    def GetAuxNode(self, name):
-        '''
-        Returns the auxiliary node with the given name.
-        
-        Parameters
-        ----------
-        name : string
-            The name of the auxiliary node to be returned.
-        '''
-        
-        warnings.warn('`GetAuxNode` will be deleted in a future version of PyNite. Use `AuxNodes[auxnode_name]` instead.', FutureWarning)
-
-        try:
-            return self.AuxNodes[name]
-        except:
-            # If the auxiliary node name is not found
-            raise ValueError(f"Auxiliary node '{name}' was not found in the model.")
-
-    def GetSpring(self, name):
-        '''
-        Returns the spring with the given name.
-        
-        Parameters
-        ----------
-        name : string
-            The name of the spring to be returned.
-        '''
-        
-        warnings.warn('`GetSpring` will be deleted in a future version of PyNite. Use `Springs[spring_name]` instead.', FutureWarning)
-        
-        try:
-            return self.Springs[name]
-        except:
-            # If the auxiliary node name is not found
-            raise ValueError(f"Spring '{name}' was not found in the model.")
-
-    def GetMember(self, name):
-        '''
-        Returns the member with the given name.
-        
-        Parameters
-        ----------
-        name : string
-            The name of the member to be returned.
-        '''
-
-        warnings.warn('`GetMember` will be deleted in a future version of PyNite. Use `Members[member_name]` instead.', FutureWarning)
-
-        try:
-            return self.Members[name]
-        except:
-            # If the member name is not found
-            raise ValueError(f"Member '{name}' was not found in the model.")
-
-    def GetPlate(self, name):
-        '''
-        Returns the plate with the given name.
-        
-        Parameters
-        ----------
-        name : string
-            The name of the plate to be returned.
-        '''
-        
-        warnings.warn('`GetPlate` will be deleted in a future version of PyNite. Use `Plates[plate_name]` instead.', FutureWarning)
-
-        try:
-            return self.Plates[name]
-        except:
-            # If the plate name is not found
-            raise ValueError(f"Plate '{name}' was not found in the model")
-
-    def GetQuad(self, name):
-        '''
-        Returns the quadrilateral with the given name.
-        
-        Parameters
-        ----------
-        name : string
-            The name of the quadrilateral to be returned.
-        '''
-        
-        warnings.warn('`GetQuad` will be deleted in a future version of PyNite. Use `Quads[quad_name]` instead.', FutureWarning)
-        
-        try:
-            return self.Quads[name]
-        except:
-            # If the quad name is not found
-            raise ValueError(f"Quad '{name}' was not found in the model")
-
     def _aux_list(self):
-        '''
-        Builds a list with known nodal displacements and with the positions in global stiffness matrix of known 
-        and unknown nodal displacements
+        """Builds a list with known nodal displacements and with the positions in global stiffness
+           matrix of known and unknown nodal displacements
 
-        Returns
-        -------
-        D1_indices : number
-            A list of the global matrix indices for the unknown nodal displacements
-        D2_indices : number
-            A list of the global matrix indices for the known nodal displacements
-        D2 : number
-            A list of the known nodal displacements
-        '''
+        :return: A list of the global matrix indices for the unknown nodal displacements (D1_indices). A
+                 list of the global matrix indices for the known nodal displacements (D2_indices). A list
+                 of the known nodal displacements (D2).
+        :rtype: list, list, list
+        """
 
         D1_indices = [] # A list of the indices for the unknown nodal displacements
         D2_indices = [] # A list of the indices for the known nodal displacements
         D2 = []         # A list of the values of the known nodal displacements (D != None)
 
         # Create the auxiliary table
         for node in self.Nodes.values():
@@ -1525,15 +1378,15 @@
 
         The stiffness matrix will be returned in scipy's sparse lil format,
         which reduces memory usage and can be easily converted to other
         formats.
 
         Parameters
         ----------
-        combo_name : string, optional
+        combo_name : str, optional
             The load combination to get the stiffness matrix for. Default is 'Combo 1'.
         log : bool, optional
             Prints updates to the console if set to True. Default is False.
         sparse : bool, optional
             Returns a sparse matrix if set to True, and a dense matrix
             otherwise. Default is True
         
@@ -1847,15 +1700,15 @@
         Returns the model's global geometric stiffness matrix.
 
         The model must have a static solution prior to obtaining the geometric stiffness matrix.
         Stiffness of plates is not included.
 
         Parameters
         ----------
-        combo_name : string, optional.
+        combo_name : str, optional.
             The name of the load combination to derive the matrix for (not the load combination itself).
         log : bool, optional
             Prints updates to the console if set to True. Default is False.
         sparse : bool, optional
             Returns a sparse matrix if set to True, and a dense matrix
             otherwise. Default is True.
                 
@@ -1927,15 +1780,15 @@
       
     def FER(self, combo_name='Combo 1'):
         '''
         Assembles and returns the global fixed end reaction vector.
 
         Parameters
         ----------
-        combo_name : string
+        combo_name : str
             The name of the load combination to get the fixed end reaction vector for (not the load combination itself).
         '''
         
         # Initialize a zero vector to hold all the terms
         FER = zeros((len(self.Nodes) * 6, 1))
         
         # Step through each physical member in the model
@@ -2027,15 +1880,15 @@
     
     def P(self, combo_name='Combo 1'):
         '''
         Assembles and returns the global nodal force vector.
 
         Parameters
         ----------
-        combo_name : string
+        combo_name : str
             The name of the load combination to get the force vector for (not the load combination itself).
         '''
             
         # Initialize a zero vector to hold all the terms
         P = zeros((len(self.Nodes)*6, 1))
         
         # Get the load combination for the given 'combo_name'
@@ -2068,22 +1921,22 @@
                         elif load[0] == 'MZ':
                             P[ID*6 + 5, 0] += factor*load[1]
         
         # Return the global nodal force vector
         return P
 
     def D(self, combo_name='Combo 1'):
-        '''
-        Returns the global displacement vector for the model.
+        """Returns the global displacement vector for the model.
 
-        Parameters
-        ----------
-        combo_name : string
-            The name of the load combination to get the displacements for (not the load combination itself).
-        '''
+        :param combo_name: The name of the load combination to get the results for. Defaults to
+                           'Combo 1'.
+        :type combo_name: str, optional
+        :return: The global displacement vector for the model
+        :rtype: array
+        """
  
         # Return the global displacement vector
         return self._D[combo_name]
 
     def _partition(self, unp_matrix, D1_indices, D2_indices):
         '''
         Partitions a matrix (or vector) into submatrices (or subvectors) based on degree of freedom
@@ -3330,15 +3183,15 @@
 
         # Print the static check table
         print(statics_table)
         print('')
     
     def _renumber(self):
         """
-        Assigns noe and element ID numbers to be used internally by the program. Numbers are
+        Assigns node and element ID numbers to be used internally by the program. Numbers are
         assigned according to the order in which they occur in each dictionary.
         """
         
         # Number each node in the model
         for id, node in enumerate(self.Nodes.values()):
             node.ID = id
         
@@ -3358,23 +3211,31 @@
         for id, plate in enumerate(self.Plates.values()):
             plate.ID = id
         
         # Number each quadrilateral in the model
         for id, quad in enumerate(self.Quads.values()):
             quad.ID = id
     
-    def _unique_name(self, dictionary, prefix):
-        """
-        Returns the next available unique name for a dictionary of objects
+    def unique_name(self, dictionary, prefix):
+        """Returns the next available unique name for a dictionary of objects.
+
+        :param dictionary: The dictionary to get a unique name for.
+        :type dictionary: dict
+        :param prefix: The prefix to use for the unique name.
+        :type prefix: str
+        :return: A unique name for the dictionary.
+        :rtype: str
         """
 
         # Select a trial value for the next available name
         name = prefix + str(len(dictionary) + 1)
+        i = 1
         while name in dictionary.keys():
-            name = prefix + str(len(dictionary) + 1)
+            name = prefix + str(len(dictionary) + i)
+            i += 1
         
         # Return the next available name
         return name
     
     def rename(self):
         """
         Renames all the nodes and elements in the model.
```

### Comparing `PyNiteFEA-0.0.71/PyNite/FixedEndReactions.py` & `PyNiteFEA-0.0.72/PyNite/FixedEndReactions.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/LoadCombo.py` & `PyNiteFEA-0.0.72/PyNite/LoadCombo.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/MainStyleSheet.css` & `PyNiteFEA-0.0.72/PyNite/MainStyleSheet.css`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/Member3D.py` & `PyNiteFEA-0.0.72/PyNite/Member3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,30 +778,27 @@
                 
                 if round(x,10) >= round(segment.x1,10) and round(x,10) < round(segment.x2,10):
                     
                     return segment.moment(x - segment.x1)
                 
             if isclose(x, self.L()):
                 
-                lastIndex = len(self.SegmentsY) - 1
-                return self.SegmentsY[lastIndex].moment(x - self.SegmentsY[lastIndex].x1)
+                return self.SegmentsY[-1].moment(x - self.SegmentsY[-1].x1)
                 
         elif Direction == 'Mz':
             
             for segment in self.SegmentsZ:
                 
                 if round(x,10) >= round(segment.x1,10) and round(x,10) < round(segment.x2,10):
                     
                     return segment.moment(x - segment.x1)
                 
             if isclose(x, self.L()):
                 
-                lastIndex = len(self.SegmentsZ) - 1
-                return self.SegmentsZ[lastIndex].moment(x - self.SegmentsZ[lastIndex].x1)
-                return self.SegmentsZ[lastIndex].Moment(x - self.SegmentsZ[lastIndex].x1)
+                return self.SegmentsZ[-1].moment(x - self.SegmentsZ[-1].x1)
         
         else:
             raise ValueError(f"Direction must be 'My' or 'Mz'. {Direction} was given.")
             
 #%%
     def max_moment(self, Direction, combo_name='Combo 1'):
         """
```

### Comparing `PyNiteFEA-0.0.71/PyNite/Mesh.py` & `PyNiteFEA-0.0.72/PyNite/Mesh.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,70 @@
         self.ky_mod = ky_mod                # Local y stiffness modification factor for elements in the mesh
         self.start_node = start_node        # The name of the first node in the mesh
         self.last_node = None               # The name of the last node in the mesh
         self.start_element = start_element  # The name of the first element in the mesh
         self.last_element = None            # The name of the last element in the mesh
         self.nodes = {}                     # A dictionary containing the nodes in the mesh
         self.elements = {}                  # A dictionary containing the elements in the mesh
+        self.element_type = 'Quad'          # The type of element used in the mesh
         self._is_generated = False          # A flag indicating whether the mesh has been generated
     
     def is_generated(self):
         return self._is_generated
     
+    def _rename_duplicates(self):
+        """Renames any nodes or elements in the mesh that are already in the model
+        """
+
+        # Initialize lists to track node and element name changes
+        revised_nodes = {}
+        revised_elements = {}
+
+        # Step through each node in the mesh
+        for node in self.nodes.values():
+
+            # Check if this node name is already being used in the model's `Nodes` dictionary
+            if node.name in self.model.Nodes.keys():
+
+                # Come up with a new node name
+                node.name = self.model.unique_name(self.model.Nodes, 'N')
+            
+            # Save the element to the model
+            self.model.Nodes[node.name] = node
+
+            # Prepare to save the element to the mesh
+            revised_nodes[node.name] = node
+            
+        # Step through each element in the mesh
+        for element in self.elements.values():
+
+            # Check if this element name is already being used in the model's `Plates` dictionary
+            if element.name in self.model.Plates.keys():
+
+                # Come up with a new element name
+                element.name = self.model.unique_name(self.model.Plates, 'R')
+
+                # Save the element to the model
+                self.model.Plates[element.name] = element
+
+            # Check if this element name is already being used in the model's `Quads` dictionary
+            elif element.name in self.model.Quads.keys():
+
+                # Come up with a new element name
+                element.name = self.model.unique_name(self.model.Quads, prefix='Q')
+
+                # Save the element to the model
+                self.model.Quads[element.name] = element
+            
+            revised_elements[element.name] = element
+        
+        # Replace the old dictionaries of nodes and elements with the revised dictionaries
+        self.nodes = revised_nodes
+        self.elements = revised_elements
+            
     def generate(self):
         """
         A placeholder to be overwritten by subclasses inheriting from this class
         """
         pass
 
     def max_shear(self, direction='Qx', combo=None):
@@ -523,16 +574,16 @@
             else:
                 self.elements[element_name] = Plate3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                                     self.nodes['N' + str(j_node + node_offset)],
                                                                     self.nodes['N' + str(m_node + node_offset)],
                                                                     self.nodes['N' + str(n_node + node_offset)],
                                                                     self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
 
-        # Initialize a list of nodes and associated elements that fall within
-        # opening boundaries that will be deleted
+        # Initialize a list of nodes and associated elements that fall within opening boundaries
+        # that will be deleted
         node_del_list = []
         element_del_list = []
 
         # Go back through the mesh and delete any nodes that are in the openings
         for node in self.nodes.values():
             
             # Get the node's position in the mesh's local coordinate sytem.
@@ -591,23 +642,37 @@
         for node_name in node_del_list:
             del self.nodes[node_name]
 
         # Identify the last node and last element in the mesh
         self.last_node = list(self.nodes.values())[-1]
         self.last_element = list(self.elements.values())[-1]
 
-        # Add the nodes and elements to the model
-        for node in self.nodes.values():
-            self.model.Nodes[node.name] = node
+        print(' ')
+        print('Mesh Check Before Renaming:')
+        print('***************************')
+        print(check_mesh_integrity(self))
+
+        # At this point we have a mesh, but some of the element or node names may already be
+        # being used in the model. Rename any names that are already being used.
+        self._rename_duplicates()
+
+        # Add the nodes to the model
+        for key, node in self.nodes.items():
+            self.model.Nodes[key] = node
         
-        for element in self.elements.values():
+        # Add the elements to the model
+        for key, element in self.elements.items():
             if element.type == 'Quad':
-                self.model.Quads[element.name] = element
-            else:
-                self.model.Plates[element.name] = element
+                self.model.Quads[key] = element
+            elif element.type == 'Rect':
+                self.model.Plates[key] = element
+        
+        print('Mesh Check After Renaming:')
+        print('**************************')
+        print(check_mesh_integrity(self))
 
         # Flag the mesh as generated
         self._is_generated = True
 
     def node_local_coords(self, node):
         """
         Calculates a node's position in the mesh's local coordinate system
@@ -760,23 +825,24 @@
         # nodes that are no longer in the dictionary. Attach these plates to the nodes that are
         # still in the dictionary instead. 
         for element in self.elements.values():
             element.i_node = self.nodes[element.i_node.name]
             element.j_node = self.nodes[element.j_node.name]
             element.m_node = self.nodes[element.m_node.name]
             element.n_node = self.nodes[element.n_node.name]
-        
-        # Add the nodes and elements to the model
+
+        # Add the nodes to the model
         for node in self.nodes.values():
             self.model.Nodes[node.name] = node
         
+        # Add the elements to the model
         for element in self.elements.values():
-            if element.type == 'Quad':
+            if element.type.upper() == 'QUAD':
                 self.model.Quads[element.name] = element
-            else:
+            elif element.type.upper() == 'RECT':
                 self.model.Plates[element.name] = element
         
         # Flag the mesh as generated
         self._is_generated = True
 
 #%%
 class AnnulusRingMesh(Mesh):
@@ -884,23 +950,24 @@
                 j_node = 1 + n
 
             self.elements[element_name] = Quad3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                                self.nodes['N' + str(j_node + node_offset)],
                                                                self.nodes['N' + str(m_node + node_offset)],
                                                                self.nodes['N' + str(n_node + node_offset)],
                                                                self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
-            
+
         # Add the nodes and elements to the model
         for node in self.nodes.values():
             self.model.Nodes[node.name] = node
         
+        # Add the elements to the model
         for element in self.elements.values():
-            if element.type == 'Quad':
+            if element.type.upper() == 'QUAD':
                 self.model.Quads[element.name] = element
-            else:
+            if element.type.upper() == 'RECT':
                 self.model.Plates[element.name] = element
         
         # Flag the mesh as generated
         self._is_generated = True
 
 #%%
 class AnnulusTransRingMesh(Mesh):
@@ -1061,15 +1128,15 @@
                     j_node = 1 + 3*n
 
             self.elements[element_name] = Quad3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                                self.nodes['N' + str(j_node + node_offset)],
                                                                self.nodes['N' + str(m_node + node_offset)],
                                                                self.nodes['N' + str(n_node + node_offset)],
                                                                self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
-        
+
         # Add the nodes and elements to the model
         for node in self.nodes.values():
             self.model.Nodes[node.name] = node
         
         for element in self.elements.values():
             if element.type == 'Quad':
                 self.model.Quads[element.name] = element
@@ -1238,15 +1305,15 @@
         # nodes that are no longer in the dictionary. Attach these plates to the nodes that are
         # still in the dictionary instead. 
         for element in self.elements.values():
             element.i_node = self.nodes[element.i_node.name]
             element.j_node = self.nodes[element.j_node.name]
             element.m_node = self.nodes[element.m_node.name]
             element.n_node = self.nodes[element.n_node.name]
-        
+
         # Add the nodes and elements to the model
         for node in self.nodes.values():
             self.model.Nodes[node.name] = node
         
         for element in self.elements.values():
             if element.type == 'Quad':
                 self.model.Quads[element.name] = element
@@ -1434,7 +1501,129 @@
             if element.type == 'Quad':
                 self.model.Quads[element.name] = element
             else:
                 self.model.Plates[element.name] = element
             
         # Flag the mesh as generated
         self._is_generated = True
+        
+def check_mesh_integrity(mesh, console_log=True):
+    """Runs basic integrity checks to ensure the mesh is in sync with its model. Usually you don't
+    want to run this check unless the mesh has been generated since generating the mesh is what
+    syncs it to the model.
+
+    :param mesh: A mesh of finite elements.
+    :type mesh: Mesh
+    :param console_log: Determines whether the results will be printed to the console or returned
+                        as a list of strings. Defaults to True.
+    :type console_log: bool, optional
+    :return: Any errors discovered by the integrity check
+    :rtype: list
+    """
+
+    # Initialize an empty list for error messages
+    errors = []
+
+    # Check that every element in the mesh is attached at all four nodes to nodes that are in the mesh
+    count = 0
+    for element in mesh.elements.values():
+
+        if (element.i_node not in mesh.nodes.values() or
+            element.j_node not in mesh.nodes.values() or
+            element.m_node not in mesh.nodes.values() or
+            element.n_node not in mesh.nodes.values()):
+
+            count += 1
+    
+    # Prepare the error message
+    if count != 0:
+        errors.append(str(count) + ' elements are attached to nodes that are not in the mesh.')
+
+    # Check that every element in the mesh is attached at all four nodes to nodes that are in the model
+    count = 0
+    for element in mesh.elements.values():
+
+        if (element.i_node not in mesh.model.Nodes.values() or
+            element.j_node not in mesh.model.Nodes.values() or
+            element.m_node not in mesh.model.Nodes.values() or
+            element.n_node not in mesh.model.Nodes.values()):
+
+            count += 1
+    
+    # Prepare the error message
+    if count != 0:
+        errors.append(str(count) + ' elements are attached to nodes that are not in the model.')
+    
+    # Check that each element has 4 unique nodes
+    count = 0
+    for element in mesh.elements.values():
+
+        if (element.i_node is element.j_node or
+            element.i_node is element.m_node or
+            element.i_node is element.n_node or
+            element.j_node is element.m_node or
+            element.j_node is element.n_node or
+            element.m_node is element.n_node):
+
+            count += 1
+        
+    # Prepare the error message
+    if count != 0:
+        errors.append(str(count) + ' elements have duplicate nodes in them.')
+
+    # Check that each element's name in the mesh is in the model
+    count = 0
+    for element in mesh.elements.values():
+        if element.name not in mesh.model.Plates.keys() and element.name not in mesh.model.Quads.keys():
+            count += 1
+    
+    if count != 0:
+        errors.append(str(count) + ' element names in the mesh were not found in the model.')
+    
+    # Check that each element in the mesh is in the model
+    count = 0
+    for element in mesh.elements.values():
+        if element not in mesh.model.Plates.values() and element.name not in mesh.model.Quads.values():
+            count += 1
+    
+    if count != 0:
+        errors.append(str(count) + ' elements in the mesh were not found in the model.')
+
+    # Check that each element in the mesh matches its corresponding element in the model
+    count = 0
+    for element in mesh.elements.values():
+        
+        if mesh.element_type == 'Rect':
+            if element.name not in mesh.model.Plates.keys() or mesh.elements[element.name] is not mesh.model.Plates[element.name]:
+                count +=1
+        elif mesh.element_type == 'Quad':
+            if element.name not in mesh.model.Quads.keys() or mesh.elements[element.name] is not mesh.model.Quads[element.name]:
+                count += 1
+    
+    # Prepare the error message
+    if count != 0:
+        errors.append(str(count) + ' elements in the mesh do not match their respective elements in the model.')
+    
+    # Check that each node in the mesh matches its corresponding node in the model
+    count = 0
+    for node in mesh.nodes.values():
+
+        if node.name not in mesh.model.Nodes.keys() or mesh.nodes[node.name] is not mesh.model.Nodes[node.name]:
+            count += 1
+    
+    # Prepare the error message
+    if count != 0:
+        errors.append(str(count) + ' nodes in the mesh do not match their respective nodes in the model.')
+
+    # TODO: Add more integrity checks and error messages
+
+    # Report if no errors were found
+    if errors == []:
+        errors = ['No errors detected.']
+
+    # Return the error messages
+    if console_log == True:
+        for error in errors:
+            print(error)
+            return ''
+    else:
+        return errors
```

### Comparing `PyNiteFEA-0.0.71/PyNite/Node3D.py` & `PyNiteFEA-0.0.72/PyNite/Node3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/PhysMember.py` & `PyNiteFEA-0.0.72/PyNite/PhysMember.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                 
                 direction = pt_load[0]
                 P = pt_load[1]
                 x = pt_load[2]
                 case = pt_load[3]
 
                 # Determine if the point load should be applied to this segment
-                if x >= xi and x < xj or isclose(x, self.L()):
+                if x >= xi and x < xj or (isclose(x, xj) and isclose(xj, self.L())):
 
                     x = x - xi
                     
                     # Add the load to the sub-member
                     new_sub_member.PtLoads.append([direction, P, x, case])
 
             # Add the new sub-member to the sub-member dictionary for this physical member
```

### Comparing `PyNiteFEA-0.0.71/PyNite/Plate3D.py` & `PyNiteFEA-0.0.72/PyNite/Plate3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         self.t = t
         
         self.kx_mod = kx_mod
         self.ky_mod = ky_mod
 
         self.pressures = []  # A list of surface pressures [pressure, case='Case 1']
-        
+
         # Plates need a link to the model they belong to
         self.model = model
 
         # Get material properties for the plate from the model
         try:
             self.E = self.model.Materials[material].E
             self.nu = self.model.Materials[material].nu
```

### Comparing `PyNiteFEA-0.0.71/PyNite/Quad3D.py` & `PyNiteFEA-0.0.72/PyNite/Quad3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/Report_Template.html` & `PyNiteFEA-0.0.72/PyNite/Report_Template.html`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/Reporting.py` & `PyNiteFEA-0.0.72/PyNite/Reporting.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/Spring3D.py` & `PyNiteFEA-0.0.72/PyNite/Spring3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNite/Visualization.py` & `PyNiteFEA-0.0.72/PyNite/Visualization.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/PyNiteFEA.egg-info/PKG-INFO` & `PyNiteFEA-0.0.72/PyNiteFEA.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.71
+Version: 0.0.72
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 </div>
 
 ![Build Status](https://github.com/JWock82/PyNite/actions/workflows/build-and-test.yml/badge.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyNiteFEA)
 <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/JWock82/PyNite">
 ![GitHub last commit](https://img.shields.io/github/last-commit/JWock82/PyNite)
 ![GitHub](https://img.shields.io/github/license/JWock82/PyNite)
+[![Documentation Status](https://readthedocs.org/projects/pynite/badge/?version=latest)](https://pynite.readthedocs.io/en/latest/?badge=latest)
 
 An easy to use elastic 3D structural engineering finite element analysis library for Python.
 
 # Installation
 The easiest way to install Pynite is with pip: `pip install PyNiteFEA`
 
 # Current Capabilities
@@ -88,14 +89,18 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.72
+* Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
+* Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
+
 v0.0.71
 * WARNING: This version will require reworking your models to incorporate `Materials`. Be prepared to rework your models before you upgrade. The examples have all been updated to show you how to do this.
 * Added `Material` definitions. This does not change Pynite's behavior much, but it prepares the way for future features.
 * Greatly simplified the process of meshing plates/quads. Meshes can now be generated directly from the `FEModel3D` object.
 * Added data types to the many dictionaries storing data in the `FEModel3D` object. Most development environments will now offer hints when using these dictionaries directly. This makes accessing the results you're interested in more intuitive.
 * Simplified internal code for finding unique names for objects.
```

### Comparing `PyNiteFEA-0.0.71/PyNiteFEA.egg-info/SOURCES.txt` & `PyNiteFEA-0.0.72/PyNiteFEA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.71/README.md` & `PyNiteFEA-0.0.72/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 </div>
 
 ![Build Status](https://github.com/JWock82/PyNite/actions/workflows/build-and-test.yml/badge.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyNiteFEA)
 <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/JWock82/PyNite">
 ![GitHub last commit](https://img.shields.io/github/last-commit/JWock82/PyNite)
 ![GitHub](https://img.shields.io/github/license/JWock82/PyNite)
+[![Documentation Status](https://readthedocs.org/projects/pynite/badge/?version=latest)](https://pynite.readthedocs.io/en/latest/?badge=latest)
 
 An easy to use elastic 3D structural engineering finite element analysis library for Python.
 
 # Installation
 The easiest way to install Pynite is with pip: `pip install PyNiteFEA`
 
 # Current Capabilities
@@ -69,14 +70,18 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.72
+* Bug fix for point loads at the ends of physical members. These point loads were erroneously being applied at the end of all segments of the physical member. This error was introduced with the new physical member feature late last year. Prior to that this error did not exist.
+* Improvements to plate meshing: (1) Rectangular meshes now automatically renumber nodes and elements to avoid duplicating names that are already in the model. This feature is only available for rectangular meshes at the moment. For other types of meshes you'll need to manually specify the start node and start element for numbering. (2) Meshes also now automatically stay in sync with the model. A node moved in the model will automatically reflect back on the mesh. Changes to elements in the model will automatically be reflected in the mesh. The program used to lose track of this. Once the mesh was generated it was "one and done" and no more.
+
 v0.0.71
 * WARNING: This version will require reworking your models to incorporate `Materials`. Be prepared to rework your models before you upgrade. The examples have all been updated to show you how to do this.
 * Added `Material` definitions. This does not change Pynite's behavior much, but it prepares the way for future features.
 * Greatly simplified the process of meshing plates/quads. Meshes can now be generated directly from the `FEModel3D` object.
 * Added data types to the many dictionaries storing data in the `FEModel3D` object. Most development environments will now offer hints when using these dictionaries directly. This makes accessing the results you're interested in more intuitive.
 * Simplified internal code for finding unique names for objects.
```

### Comparing `PyNiteFEA-0.0.71/setup.py` & `PyNiteFEA-0.0.72/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNiteFEA",
-    version="0.0.71",
+    version="0.0.72",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="A simple elastic 3D structural finite element library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/PyNite.git",
     packages=setuptools.find_packages(include=['PyNite', 'Pynite.*']),
```

