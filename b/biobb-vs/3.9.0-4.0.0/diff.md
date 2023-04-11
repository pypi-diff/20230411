# Comparing `tmp/biobb_vs-3.9.0.tar.gz` & `tmp/biobb_vs-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_vs-3.9.0.tar", last modified: Tue Dec 27 15:46:58 2022, max compression
+gzip compressed data, was "dist/biobb_vs-4.0.0.tar", last modified: Tue Apr 11 16:01:52 2023, max compression
```

## Comparing `biobb_vs-3.9.0.tar` & `biobb_vs-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:36:06.000000 biobb_vs-3.9.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4162 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3397 2022-12-27 15:44:57.000000 biobb_vs-3.9.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       78 2022-12-27 15:44:49.000000 biobb_vs-3.9.0/biobb_vs/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs/fpocket/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       78 2022-05-26 11:36:06.000000 biobb_vs-3.9.0/biobb_vs/fpocket/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5790 2022-12-27 15:25:29.000000 biobb_vs-3.9.0/biobb_vs/fpocket/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9968 2022-12-27 15:22:05.000000 biobb_vs-3.9.0/biobb_vs/fpocket/fpocket_filter.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9653 2022-12-27 15:25:10.000000 biobb_vs-3.9.0/biobb_vs/fpocket/fpocket_run.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7433 2022-12-27 15:27:02.000000 biobb_vs-3.9.0/biobb_vs/fpocket/fpocket_select.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:36:06.000000 biobb_vs-3.9.0/biobb_vs/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs/utils/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       86 2022-05-26 11:36:06.000000 biobb_vs-3.9.0/biobb_vs/utils/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17903 2022-12-27 15:29:19.000000 biobb_vs-3.9.0/biobb_vs/utils/bindingsite.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8919 2022-12-27 15:32:06.000000 biobb_vs-3.9.0/biobb_vs/utils/box.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10730 2022-12-27 15:31:04.000000 biobb_vs-3.9.0/biobb_vs/utils/box_residues.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    36419 2022-09-22 10:24:34.000000 biobb_vs-3.9.0/biobb_vs/utils/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7223 2022-12-27 15:33:08.000000 biobb_vs-3.9.0/biobb_vs/utils/extract_model_pdbqt.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs/vina/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       45 2022-05-26 11:36:06.000000 biobb_vs-3.9.0/biobb_vs/vina/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10516 2022-12-27 15:34:19.000000 biobb_vs-3.9.0/biobb_vs/vina/autodock_vina_run.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2671 2022-05-26 11:36:06.000000 biobb_vs-3.9.0/biobb_vs/vina/common.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4162 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      683 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      417 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/biobb_vs.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2022-12-27 15:46:58.000000 biobb_vs-3.9.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1663 2022-12-27 15:44:40.000000 biobb_vs-3.9.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:36:06.000000 biobb_vs-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6081 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5316 2023-04-11 16:01:31.000000 biobb_vs-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2023-04-11 16:01:19.000000 biobb_vs-4.0.0/biobb_vs/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs/fpocket/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       78 2022-05-26 11:36:06.000000 biobb_vs-4.0.0/biobb_vs/fpocket/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5794 2023-03-03 15:15:07.000000 biobb_vs-4.0.0/biobb_vs/fpocket/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9968 2022-12-27 15:22:05.000000 biobb_vs-4.0.0/biobb_vs/fpocket/fpocket_filter.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9654 2023-03-27 16:17:20.000000 biobb_vs-4.0.0/biobb_vs/fpocket/fpocket_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7433 2022-12-27 15:27:02.000000 biobb_vs-4.0.0/biobb_vs/fpocket/fpocket_select.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:36:06.000000 biobb_vs-4.0.0/biobb_vs/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs/utils/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       86 2022-05-26 11:36:06.000000 biobb_vs-4.0.0/biobb_vs/utils/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17903 2022-12-27 15:29:19.000000 biobb_vs-4.0.0/biobb_vs/utils/bindingsite.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8919 2022-12-27 15:32:06.000000 biobb_vs-4.0.0/biobb_vs/utils/box.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10730 2022-12-27 15:31:04.000000 biobb_vs-4.0.0/biobb_vs/utils/box_residues.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    36573 2023-03-27 16:17:20.000000 biobb_vs-4.0.0/biobb_vs/utils/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7223 2022-12-27 15:33:08.000000 biobb_vs-4.0.0/biobb_vs/utils/extract_model_pdbqt.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs/vina/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       45 2022-05-26 11:36:06.000000 biobb_vs-4.0.0/biobb_vs/vina/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10704 2023-03-27 16:15:36.000000 biobb_vs-4.0.0/biobb_vs/vina/autodock_vina_run.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2671 2022-05-26 11:36:06.000000 biobb_vs-4.0.0/biobb_vs/vina/common.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6081 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      683 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      417 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        9 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/biobb_vs.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 16:01:52.000000 biobb_vs-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1663 2023-04-11 16:01:12.000000 biobb_vs-4.0.0/setup.py
```

### Comparing `biobb_vs-3.9.0/LICENSE` & `biobb_vs-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs/fpocket/common.py` & `biobb_vs-4.0.0/biobb_vs/fpocket/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,20 @@
 	data = {}
 
 	# parse input_info.txt file to python object
 	pocket = ''
 	for line in lines:
 		if not line.startswith('\t'):
 			# first level: pocket
-			num = re.findall('\d+', line)[0]
+			num = re.findall('\\d+', line)[0]
 			pocket = 'pocket' + num
 			data[pocket] = {}
 		else:
 			# second level: pocket properties
-			groups = re.findall('(.*)(?:\ *\:\ *)(.*)', line)[0]
+			groups = re.findall('(.*)(?:\\ *\\:\\ *)(.*)', line)[0]
 			key = groups[0].lower().strip()
 			key = re.sub(r'\-|\.', '', key)
 			key = re.sub(r'\s+', '_', key)
 			value = float(groups[1]) if '.' in groups[1] else int(groups[1])
 			data[pocket][key] = value
 
 	# get number of pockets
```

### Comparing `biobb_vs-3.9.0/biobb_vs/fpocket/fpocket_filter.py` & `biobb_vs-4.0.0/biobb_vs/fpocket/fpocket_filter.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs/fpocket/fpocket_run.py` & `biobb_vs-4.0.0/biobb_vs/fpocket/fpocket_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_pdb_path, output_pockets_zip, output_summary, 
-                properties=None, **kwargs) -> None:
+                 properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
```

### Comparing `biobb_vs-3.9.0/biobb_vs/fpocket/fpocket_select.py` & `biobb_vs-4.0.0/biobb_vs/fpocket/fpocket_select.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs/utils/bindingsite.py` & `biobb_vs-4.0.0/biobb_vs/utils/bindingsite.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs/utils/box.py` & `biobb_vs-4.0.0/biobb_vs/utils/box.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs/utils/box_residues.py` & `biobb_vs-4.0.0/biobb_vs/utils/box_residues.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs/utils/common.py` & `biobb_vs-4.0.0/biobb_vs/utils/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 
 from Bio import BiopythonDeprecationWarning
 import warnings
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", BiopythonDeprecationWarning)
     import Bio.PDB
     import Bio.pairwise2
-    import Bio.SubsMat.MatrixInfo
-    #from Bio.Align import substitution_matrices
+    try:
+        import Bio.SubsMat.MatrixInfo
+    except ImportError:
+        import Bio.Align.substitution_matrices
     from Bio.Data.SCOPData import protein_letters_3to1 as prot_one_letter
 
 # CHECK PARAMETERS
 
 def check_input_path(path, argument, out_log, classname):
 	""" Checks input file """ 
 	if not Path(path).exists():
@@ -91,15 +93,18 @@
         """
 
         #seq list to seq string
         sequence_A = ''.join([i[1] for i in seqA])
         sequence_B = ''.join([i[1] for i in seqB])
 
         # get matrix from matrix_name
-        matrix = getattr(Bio.SubsMat.MatrixInfo, matrix_name)
+        try:
+            matrix = getattr(Bio.SubsMat.MatrixInfo, matrix_name)
+        except AttributeError:
+            matrix = Bio.Align.substitution_matrices.load(matrix_name)
 
         #print(Bio.SubsMat.MatrixInfo)
         #print(type(substitution_matrices.select()))
         #matrix = getattr(substitution_matrices.load(), matrix_name)
 
         # Do pairwaise alignment
         alns = Bio.pairwise2.align.globalds(sequence_A, sequence_B, matrix, gap_open, gap_extend, penalize_end_gaps=(False, False) )
```

### Comparing `biobb_vs-3.9.0/biobb_vs/utils/extract_model_pdbqt.py` & `biobb_vs-4.0.0/biobb_vs/utils/extract_model_pdbqt.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs/vina/autodock_vina_run.py` & `biobb_vs-4.0.0/biobb_vs/vina/autodock_vina_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Args:
         input_ligand_pdbqt_path (str): Path to the input PDBQT ligand. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/vina/vina_ligand.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         input_receptor_pdbqt_path (str): Path to the input PDBQT receptor. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/vina/vina_receptor.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         input_box_path (str): Path to the PDB containig the residues belonging to the binding site. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/vina/vina_box.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_pdbqt_path (str): Path to the output PDBQT file. File type: output. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/reference/vina/ref_output_vina.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         output_log_path (str) (Optional): Path to the log file. File type: output. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/reference/vina/ref_output_vina.log>`_. Accepted formats: log (edam:format_2330).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
+            * **cpu** (*int*) - (1) [1~1000|1] the number of CPUs to use.
             * **binary_path** (*string*) - ('vina') path to vina in your local computer.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('biocontainers/autodock-vina:v1.1.2-5b1-deb_cv1') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
@@ -47,15 +48,15 @@
                             output_pdbqt_path='/path/to/newStructure.pdbqt', 
                             output_log_path='/path/to/newLog.log', 
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: Autodock Vina
-            * version: >=1.1.2
+            * version: >=1.2.3
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
@@ -70,14 +71,15 @@
         # Input/Output files
         self.io_dict = { 
             "in": { "input_ligand_pdbqt_path": input_ligand_pdbqt_path, "input_receptor_pdbqt_path": input_receptor_pdbqt_path, "input_box_path": input_box_path }, 
             "out": { "output_pdbqt_path": output_pdbqt_path, "output_log_path": output_log_path } 
         }
 
         # Properties specific for BB
+        self.cpu = properties.get('cpu', 1)
         self.binary_path = properties.get('binary_path', 'vina')
         self.properties = properties
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
@@ -120,16 +122,18 @@
 
         # create cmd
         self.cmd = [self.binary_path,
                '--ligand', self.stage_io_dict["in"]["input_ligand_pdbqt_path"],
                '--receptor', self.stage_io_dict["in"]["input_receptor_pdbqt_path"],
                '--center_x=' + x0, '--center_y=' + y0, '--center_z=' + z0,
                '--size_x=' + sidex, '--size_y=' + sidey, '--size_z=' + sidez,
+               '--cpu', str(self.cpu),
                '--out', self.stage_io_dict["out"]["output_pdbqt_path"],
-               '--log', self.stage_io_dict["out"]["output_log_path"]]
+               '--verbosity', '1',
+               '>', self.stage_io_dict["out"]["output_log_path"]]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
```

### Comparing `biobb_vs-3.9.0/biobb_vs/vina/common.py` & `biobb_vs-4.0.0/biobb_vs/vina/common.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/biobb_vs.egg-info/SOURCES.txt` & `biobb_vs-4.0.0/biobb_vs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_vs-3.9.0/setup.py` & `biobb_vs-4.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_vs",
-    version="3.9.0",
+    version="4.0.0",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_vs is the Biobb module collection to perform virtual screening studies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_vs",
     project_urls={
         "Documentation": "http://biobb_vs.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==3.9.0'],
+    install_requires=['biobb_common==4.0.0'],
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "fpocket_filter = biobb_vs.fpocket.fpocket_filter:main",
             "fpocket_run = biobb_vs.fpocket.fpocket_run:main",
             "fpocket_select = biobb_vs.fpocket.fpocket_select:main",
             "bindingsite = biobb_vs.utils.bindingsite:main",
```

