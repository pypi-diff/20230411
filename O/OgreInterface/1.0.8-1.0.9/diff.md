# Comparing `tmp/OgreInterface-1.0.8.tar.gz` & `tmp/OgreInterface-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OgreInterface-1.0.8.tar", last modified: Thu Feb  9 20:45:20 2023, max compression
+gzip compressed data, was "OgreInterface-1.0.9.tar", last modified: Fri Feb 10 15:19:19 2023, max compression
```

## Comparing `OgreInterface-1.0.8.tar` & `OgreInterface-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-09 20:45:20.940389 OgreInterface-1.0.8/
--rw-rw-r--   0 dd        (1000) dd        (1000)     1513 2022-12-30 19:20:57.000000 OgreInterface-1.0.8/LICENSE.txt
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-09 20:45:20.940389 OgreInterface-1.0.8/OgreInterface/
--rw-rw-r--   0 dd        (1000) dd        (1000)        0 2022-12-30 19:20:57.000000 OgreInterface-1.0.8/OgreInterface/__init__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     2160 2023-02-02 16:32:33.000000 OgreInterface-1.0.8/OgreInterface/example.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    38639 2023-02-08 13:45:45.000000 OgreInterface-1.0.8/OgreInterface/generate.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    16999 2023-02-09 17:03:46.000000 OgreInterface-1.0.8/OgreInterface/lattice_match.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    16488 2023-02-08 13:45:45.000000 OgreInterface-1.0.8/OgreInterface/miller.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-09 20:45:20.940389 OgreInterface-1.0.8/OgreInterface/score_function/
--rw-rw-r--   0 dd        (1000) dd        (1000)        0 2023-01-31 01:28:22.000000 OgreInterface-1.0.8/OgreInterface/score_function/__init__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     3436 2023-02-04 14:30:05.000000 OgreInterface-1.0.8/OgreInterface/score_function/born.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     7129 2023-02-04 14:30:05.000000 OgreInterface-1.0.8/OgreInterface/score_function/ewald.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     6201 2023-02-04 14:30:05.000000 OgreInterface-1.0.8/OgreInterface/score_function/generate_inputs.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     8000 2023-01-08 21:11:57.000000 OgreInterface-1.0.8/OgreInterface/score_function/neighbors.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     2738 2023-02-06 17:55:48.000000 OgreInterface-1.0.8/OgreInterface/score_function/overlap.py
--rw-rw-r--   0 dd        (1000) dd        (1000)      740 2023-01-05 15:13:57.000000 OgreInterface-1.0.8/OgreInterface/score_function/scatter.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-09 20:45:20.940389 OgreInterface-1.0.8/OgreInterface/surface_match/
--rw-rw-r--   0 dd        (1000) dd        (1000)      184 2023-01-27 17:38:14.000000 OgreInterface-1.0.8/OgreInterface/surface_match/__init__.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    17541 2023-02-04 14:30:05.000000 OgreInterface-1.0.8/OgreInterface/surface_match/ionic_surface_matcher.py
--rw-rw-r--   0 dd        (1000) dd        (1000)     9372 2023-02-04 14:30:05.000000 OgreInterface-1.0.8/OgreInterface/surface_match/sphere_surface_matcher.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    86486 2023-02-09 20:43:26.000000 OgreInterface-1.0.8/OgreInterface/surfaces.py
--rw-rw-r--   0 dd        (1000) dd        (1000)    13437 2023-02-08 13:45:45.000000 OgreInterface-1.0.8/OgreInterface/utils.py
-drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-09 20:45:20.940389 OgreInterface-1.0.8/OgreInterface.egg-info/
--rw-rw-r--   0 dd        (1000) dd        (1000)      311 2023-02-09 20:45:20.000000 OgreInterface-1.0.8/OgreInterface.egg-info/PKG-INFO
--rw-rw-r--   0 dd        (1000) dd        (1000)      834 2023-02-09 20:45:20.000000 OgreInterface-1.0.8/OgreInterface.egg-info/SOURCES.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)        1 2023-02-09 20:45:20.000000 OgreInterface-1.0.8/OgreInterface.egg-info/dependency_links.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)       41 2023-02-09 20:45:20.000000 OgreInterface-1.0.8/OgreInterface.egg-info/requires.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)       29 2023-02-09 20:45:20.000000 OgreInterface-1.0.8/OgreInterface.egg-info/top_level.txt
--rw-rw-r--   0 dd        (1000) dd        (1000)      311 2023-02-09 20:45:20.940389 OgreInterface-1.0.8/PKG-INFO
--rw-rw-r--   0 dd        (1000) dd        (1000)      164 2022-12-30 19:20:57.000000 OgreInterface-1.0.8/README.md
--rw-rw-r--   0 dd        (1000) dd        (1000)      522 2023-02-09 20:45:06.000000 OgreInterface-1.0.8/pyproject.toml
--rw-rw-r--   0 dd        (1000) dd        (1000)       38 2023-02-09 20:45:20.940389 OgreInterface-1.0.8/setup.cfg
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-10 15:19:18.997776 OgreInterface-1.0.9/
+-rw-rw-r--   0 dd        (1000) dd        (1000)     1513 2022-12-30 19:20:57.000000 OgreInterface-1.0.9/LICENSE.txt
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-10 15:19:18.997776 OgreInterface-1.0.9/OgreInterface/
+-rw-rw-r--   0 dd        (1000) dd        (1000)        0 2022-12-30 19:20:57.000000 OgreInterface-1.0.9/OgreInterface/__init__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     2160 2023-02-02 16:32:33.000000 OgreInterface-1.0.9/OgreInterface/example.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    38639 2023-02-08 13:45:45.000000 OgreInterface-1.0.9/OgreInterface/generate.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    16999 2023-02-09 17:03:46.000000 OgreInterface-1.0.9/OgreInterface/lattice_match.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    16488 2023-02-08 13:45:45.000000 OgreInterface-1.0.9/OgreInterface/miller.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-10 15:19:18.997776 OgreInterface-1.0.9/OgreInterface/score_function/
+-rw-rw-r--   0 dd        (1000) dd        (1000)        0 2023-01-31 01:28:22.000000 OgreInterface-1.0.9/OgreInterface/score_function/__init__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     3436 2023-02-04 14:30:05.000000 OgreInterface-1.0.9/OgreInterface/score_function/born.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     7129 2023-02-04 14:30:05.000000 OgreInterface-1.0.9/OgreInterface/score_function/ewald.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     6201 2023-02-04 14:30:05.000000 OgreInterface-1.0.9/OgreInterface/score_function/generate_inputs.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     8000 2023-01-08 21:11:57.000000 OgreInterface-1.0.9/OgreInterface/score_function/neighbors.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     2738 2023-02-06 17:55:48.000000 OgreInterface-1.0.9/OgreInterface/score_function/overlap.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)      740 2023-01-05 15:13:57.000000 OgreInterface-1.0.9/OgreInterface/score_function/scatter.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-10 15:19:18.997776 OgreInterface-1.0.9/OgreInterface/surface_match/
+-rw-rw-r--   0 dd        (1000) dd        (1000)      184 2023-01-27 17:38:14.000000 OgreInterface-1.0.9/OgreInterface/surface_match/__init__.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    17541 2023-02-04 14:30:05.000000 OgreInterface-1.0.9/OgreInterface/surface_match/ionic_surface_matcher.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)     9372 2023-02-04 14:30:05.000000 OgreInterface-1.0.9/OgreInterface/surface_match/sphere_surface_matcher.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    91489 2023-02-10 15:18:24.000000 OgreInterface-1.0.9/OgreInterface/surfaces.py
+-rw-rw-r--   0 dd        (1000) dd        (1000)    13437 2023-02-08 13:45:45.000000 OgreInterface-1.0.9/OgreInterface/utils.py
+drwxrwxr-x   0 dd        (1000) dd        (1000)        0 2023-02-10 15:19:18.997776 OgreInterface-1.0.9/OgreInterface.egg-info/
+-rw-rw-r--   0 dd        (1000) dd        (1000)      311 2023-02-10 15:19:18.000000 OgreInterface-1.0.9/OgreInterface.egg-info/PKG-INFO
+-rw-rw-r--   0 dd        (1000) dd        (1000)      834 2023-02-10 15:19:18.000000 OgreInterface-1.0.9/OgreInterface.egg-info/SOURCES.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)        1 2023-02-10 15:19:18.000000 OgreInterface-1.0.9/OgreInterface.egg-info/dependency_links.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)       41 2023-02-10 15:19:18.000000 OgreInterface-1.0.9/OgreInterface.egg-info/requires.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)       29 2023-02-10 15:19:18.000000 OgreInterface-1.0.9/OgreInterface.egg-info/top_level.txt
+-rw-rw-r--   0 dd        (1000) dd        (1000)      311 2023-02-10 15:19:18.997776 OgreInterface-1.0.9/PKG-INFO
+-rw-rw-r--   0 dd        (1000) dd        (1000)      164 2022-12-30 19:20:57.000000 OgreInterface-1.0.9/README.md
+-rw-rw-r--   0 dd        (1000) dd        (1000)      522 2023-02-10 15:18:34.000000 OgreInterface-1.0.9/pyproject.toml
+-rw-rw-r--   0 dd        (1000) dd        (1000)       38 2023-02-10 15:19:18.997776 OgreInterface-1.0.9/setup.cfg
```

### Comparing `OgreInterface-1.0.8/LICENSE.txt` & `OgreInterface-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/example.py` & `OgreInterface-1.0.9/OgreInterface/example.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/generate.py` & `OgreInterface-1.0.9/OgreInterface/generate.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/lattice_match.py` & `OgreInterface-1.0.9/OgreInterface/lattice_match.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/miller.py` & `OgreInterface-1.0.9/OgreInterface/miller.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/score_function/born.py` & `OgreInterface-1.0.9/OgreInterface/score_function/born.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/score_function/ewald.py` & `OgreInterface-1.0.9/OgreInterface/score_function/ewald.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/score_function/generate_inputs.py` & `OgreInterface-1.0.9/OgreInterface/score_function/generate_inputs.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/score_function/neighbors.py` & `OgreInterface-1.0.9/OgreInterface/score_function/neighbors.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/score_function/overlap.py` & `OgreInterface-1.0.9/OgreInterface/score_function/overlap.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/score_function/scatter.py` & `OgreInterface-1.0.9/OgreInterface/score_function/scatter.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/surface_match/ionic_surface_matcher.py` & `OgreInterface-1.0.9/OgreInterface/surface_match/ionic_surface_matcher.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/surface_match/sphere_surface_matcher.py` & `OgreInterface-1.0.9/OgreInterface/surface_match/sphere_surface_matcher.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface/surfaces.py` & `OgreInterface-1.0.9/OgreInterface/surfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -917,14 +917,131 @@
                 return self._orthogonal_film_structure
         else:
             if return_atoms:
                 return self._non_orthogonal_film_atoms
             else:
                 return self._non_orthogonal_film_structure
 
+    def get_substrate_layer_indices(
+        self, layer_from_interface: int
+    ) -> np.ndarray:
+        """
+        This function is used to extract the atom-indicies of specific layers of the substrate part of the interface.
+
+        Examples:
+        ```
+        >>> interface.get_substrate_layer_indices(layer_from_interface=0)
+        >>> [234 235 236 237 254 255 256 257]
+        ```
+
+        Args:
+            layer_from_interface: The layer number of the substrate which you would like to get
+                atom-indices for. The layer number is reference from the interface, so layer_from_interface=0
+                would be the layer of the substrate that is at the interface.
+
+        Returns:
+            A numpy array of integer indices corresponding to the atom index of the interface structure
+        """
+        interface = self._non_orthogonal_structure
+        site_props = interface.site_properties
+        is_sub = np.array(site_props["is_sub"])
+        layer_index = np.array(site_props["layer_index"])
+        sub_n_layers = self.substrate.layers - 1
+        rel_layer_index = sub_n_layers - layer_index
+        is_layer = rel_layer_index == layer_from_interface
+
+        return np.where(np.logical_and(is_sub, is_layer))[0]
+
+    def get_film_layer_indices(self, layer_from_interface: int) -> np.ndarray:
+        """
+        This function is used to extract the atom-indicies of specific layers of the film part of the interface.
+
+        Examples:
+        ```
+        >>> interface.get_substrate_layer_indices(layer_from_interface=0)
+        >>> [0 1 2 3 4 5 6 7 8 9 10 11 12]
+        ```
+
+        Args:
+            layer_from_interface: The layer number of the film which you would like to get atom-indices for.
+            The layer number is reference from the interface, so layer_from_interface=0
+            would be the layer of the film that is at the interface.
+
+        Returns:
+            A numpy array of integer indices corresponding to the atom index of the interface structure
+        """
+        interface = self._non_orthogonal_structure
+        site_props = interface.site_properties
+        is_film = np.array(site_props["is_film"])
+        layer_index = np.array(site_props["layer_index"])
+        is_layer = layer_index == layer_from_interface
+
+        return np.where(np.logical_and(is_film, is_layer))[0]
+
+    def replace_species(
+        self, site_index: int, species_mapping: Dict[str, str]
+    ) -> None:
+        """
+        This function can be used to replace the species at a given site in the interface structure
+
+        Examples:
+        ```
+        >>> interface.replace_species(site_index=42, species_mapping={"In": "Zn", "As": "Te"})
+        ```
+
+        Args:
+            site_index: Index of the site to be replaced
+            species_mapping: Dictionary showing the mapping between species.
+                For example if you wanted to replace InAs with ZnTe then the species mapping would
+                be as shown in the example above.
+        """
+        species_str = self._orthogonal_structure[site_index].species_string
+
+        if species_str in species_mapping:
+            is_sub = self._non_orthogonal_structure[site_index].properties[
+                "is_sub"
+            ]
+            self._non_orthogonal_structure[site_index].species = Element(
+                species_mapping[species_str]
+            )
+            self._orthogonal_structure[site_index].species = Element(
+                species_mapping[species_str]
+            )
+
+            if is_sub:
+                sub_iface_equiv = np.array(
+                    self._orthogonal_substrate_structure.site_properties[
+                        "interface_equivalent"
+                    ]
+                )
+                sub_site_ind = np.where(sub_iface_equiv == site_index)[0][0]
+                self._non_orthogonal_substrate_structure[
+                    sub_site_ind
+                ].species = Element(species_mapping[species_str])
+                self._orthogonal_substrate_structure[
+                    sub_site_ind
+                ].species = Element(species_mapping[species_str])
+            else:
+                film_iface_equiv = np.array(
+                    self._orthogonal_film_structure.site_properties[
+                        "interface_equivalent"
+                    ]
+                )
+                film_site_ind = np.where(film_iface_equiv == site_index)[0][0]
+                self._non_orthogonal_film_structure[
+                    film_site_ind
+                ].species = Element(species_mapping[species_str])
+                self._orthogonal_film_structure[
+                    film_site_ind
+                ].species = Element(species_mapping[species_str])
+        else:
+            raise ValueError(
+                f"Species: {species_str} is not is species mapping"
+            )
+
     @property
     def area(self) -> float:
         """
         Cross section area of the interface in Angstroms^2
 
         Examples:
             >>> interface.area
@@ -1868,14 +1985,18 @@
             coords=interface_coords,
             to_unit_cell=True,
             coords_are_cartesian=False,
             site_properties=interface_site_properties,
         )
         non_ortho_interface_struc.sort()
 
+        non_ortho_interface_struc.add_site_property(
+            "interface_equivalent", list(range(len(non_ortho_interface_struc)))
+        )
+
         if self.center:
             # Get the new vacuum length, needed for shifting
             vacuum_len = interface_c_len - interface_structure_len
 
             # Find the fractional coordinates of shifting the structure up by half the amount of vacuum cells
             center_shift = np.ceil(vacuum_len / oriented_bulk_c) // 2
             center_shift *= oriented_bulk_c / interface_c_len
```

### Comparing `OgreInterface-1.0.8/OgreInterface/utils.py` & `OgreInterface-1.0.9/OgreInterface/utils.py`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/OgreInterface.egg-info/SOURCES.txt` & `OgreInterface-1.0.9/OgreInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OgreInterface-1.0.8/pyproject.toml` & `OgreInterface-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OgreInterface"
-version = "1.0.8"
+version = "1.0.9"
 description = "A Python library used to generate and optimize epitaxial inorganic interface structures."
 authors = [{name = "Derek Dardzinski", email = "dardzinski.derek@gmail.com"}]
 dependencies = ["pymatgen", "matplotlib", "numpy", "tqdm", "ase", "torch"]
 
 [project.urls]
 source = "https://github.com/DerekDardzinski/OgreInterface"
```

