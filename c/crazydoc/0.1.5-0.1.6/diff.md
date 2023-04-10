# Comparing `tmp/crazydoc-0.1.5.tar.gz` & `tmp/crazydoc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crazydoc-0.1.5.tar", last modified: Wed May  4 18:21:23 2022, max compression
+gzip compressed data, was "crazydoc-0.1.6.tar", last modified: Mon Apr 10 22:09:38 2023, max compression
```

## Comparing `crazydoc-0.1.5.tar` & `crazydoc-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-04 18:21:23.422144 crazydoc-0.1.5/
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-04 17:59:14.000000 crazydoc-0.1.5/LICENCE.txt
--rwxrwxr-x   0 peter     (1000) peter     (1000)       86 2022-05-04 17:59:14.000000 crazydoc-0.1.5/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     1520 2022-05-04 18:21:23.418144 crazydoc-0.1.5/PKG-INFO
--rwxrwxr-x   0 peter     (1000) peter     (1000)     4662 2022-05-04 18:18:45.000000 crazydoc-0.1.5/README.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-04 18:21:23.418144 crazydoc-0.1.5/crazydoc/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4135 2022-05-04 17:59:14.000000 crazydoc-0.1.5/crazydoc/CrazydocParser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4521 2022-05-04 17:59:14.000000 crazydoc-0.1.5/crazydoc/Observers.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      272 2022-05-04 17:59:14.000000 crazydoc-0.1.5/crazydoc/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3247 2022-05-04 17:59:14.000000 crazydoc-0.1.5/crazydoc/biotools.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      512 2022-05-04 17:59:14.000000 crazydoc-0.1.5/crazydoc/conf.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1053 2022-05-04 17:59:14.000000 crazydoc-0.1.5/crazydoc/plots.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)       22 2022-05-04 18:18:45.000000 crazydoc-0.1.5/crazydoc/version.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-04 18:21:23.418144 crazydoc-0.1.5/crazydoc.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1520 2022-05-04 18:21:22.000000 crazydoc-0.1.5/crazydoc.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      402 2022-05-04 18:21:23.000000 crazydoc-0.1.5/crazydoc.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2022-05-04 18:21:23.000000 crazydoc-0.1.5/crazydoc.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       22 2022-05-04 18:21:23.000000 crazydoc-0.1.5/crazydoc.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        9 2022-05-04 18:21:23.000000 crazydoc-0.1.5/crazydoc.egg-info/top_level.txt
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-04 18:21:23.418144 crazydoc-0.1.5/examples/
--rw-rw-r--   0 peter     (1000) peter     (1000)      720 2022-05-04 17:59:14.000000 crazydoc-0.1.5/examples/basic_example.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     8490 2022-05-04 17:59:14.000000 crazydoc-0.1.5/ez_setup.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1214 2022-05-04 18:18:45.000000 crazydoc-0.1.5/pypi-readme.rst
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2022-05-04 18:21:23.422144 crazydoc-0.1.5/setup.cfg
--rwxrwxr-x   0 peter     (1000) peter     (1000)      590 2022-05-04 17:59:14.000000 crazydoc-0.1.5/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-10 22:09:38.941854 crazydoc-0.1.6/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2023-04-10 13:45:02.000000 crazydoc-0.1.6/LICENCE.txt
+-rwxrwxr-x   0 peter     (1000) peter     (1000)       86 2023-04-10 13:45:02.000000 crazydoc-0.1.6/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1520 2023-04-10 22:09:38.941854 crazydoc-0.1.6/PKG-INFO
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     5317 2023-04-10 22:09:09.000000 crazydoc-0.1.6/README.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-10 22:09:38.937854 crazydoc-0.1.6/crazydoc/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4135 2023-04-10 13:45:02.000000 crazydoc-0.1.6/crazydoc/CrazydocParser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4521 2023-04-10 13:45:02.000000 crazydoc-0.1.6/crazydoc/Observers.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      346 2023-04-10 22:08:22.000000 crazydoc-0.1.6/crazydoc/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3247 2023-04-10 13:45:02.000000 crazydoc-0.1.6/crazydoc/biotools.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      512 2023-04-10 13:45:02.000000 crazydoc-0.1.6/crazydoc/conf.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    12148 2023-04-10 22:09:09.000000 crazydoc-0.1.6/crazydoc/crazydoc_writers.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1053 2023-04-10 13:45:02.000000 crazydoc-0.1.6/crazydoc/plots.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)       22 2023-04-10 22:09:09.000000 crazydoc-0.1.6/crazydoc/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-10 22:09:38.937854 crazydoc-0.1.6/crazydoc.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1520 2023-04-10 22:09:38.000000 crazydoc-0.1.6/crazydoc.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      431 2023-04-10 22:09:38.000000 crazydoc-0.1.6/crazydoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-04-10 22:09:38.000000 crazydoc-0.1.6/crazydoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       22 2023-04-10 22:09:38.000000 crazydoc-0.1.6/crazydoc.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        9 2023-04-10 22:09:38.000000 crazydoc-0.1.6/crazydoc.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-10 22:09:38.941854 crazydoc-0.1.6/examples/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      720 2023-04-10 13:45:02.000000 crazydoc-0.1.6/examples/basic_example.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     8490 2023-04-10 13:45:02.000000 crazydoc-0.1.6/ez_setup.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1214 2023-04-10 13:45:02.000000 crazydoc-0.1.6/pypi-readme.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-04-10 22:09:38.941854 crazydoc-0.1.6/setup.cfg
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      590 2023-04-10 13:45:02.000000 crazydoc-0.1.6/setup.py
```

### Comparing `crazydoc-0.1.5/LICENCE.txt` & `crazydoc-0.1.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/PKG-INFO` & `crazydoc-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crazydoc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Read genetic sequences from stylized docx files
 Home-page: https://github.com/Edinburgh-Genome-Foundry/crazydoc
 Author: Zulko
 License: MIT
 Keywords: dna-sequence bioinformatics systems-biology docx
 Platform: UNKNOWN
 License-File: LICENCE.txt
```

### Comparing `crazydoc-0.1.5/README.rst` & `crazydoc-0.1.6/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -80,14 +80,30 @@
 
     biopython_records = parse_doc_file(protein_path, is_protein=True)
 
 This will return *protein* records, which will be saved with a GenPept extension 
 (.gp) by ``records_to_genbank(biopython_records, is_protein=True)``, 
 unless specified otherwise with ``extension=``.
 
+You can also save annotated sequences as colourful Word docs.
+``write_crazydoc()`` takes a SeqRecord, the qualifier key to use as a feature name,
+and a path to save the document to.
+
+.. code:: python
+
+    # Load an annotated sequence with Biopython
+    from Bio import SeqIO
+    from crazydoc import write_crazydoc
+    seq = SeqIO.read("examples/examples_outputs/Sequence 1.gbk", "genbank")
+    # Most features will already have some name qualifier but you can add your own
+    for i,f in enumerate(seq.features):
+        f.qualifiers['product'] = f"feature{i}"
+    # Save the annotated sequence as a docx
+    write_crazydoc(seq, 'product', 'test.docx')
+
 
 Installation
 ------------
 
 You can install crazydoc through PIP:
 
 .. code::
```

### Comparing `crazydoc-0.1.5/crazydoc/CrazydocParser.py` & `crazydoc-0.1.6/crazydoc/CrazydocParser.py`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/crazydoc/Observers.py` & `crazydoc-0.1.6/crazydoc/Observers.py`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/crazydoc/biotools.py` & `crazydoc-0.1.6/crazydoc/biotools.py`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/crazydoc/conf.py` & `crazydoc-0.1.6/crazydoc/conf.py`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/crazydoc/plots.py` & `crazydoc-0.1.6/crazydoc/plots.py`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/crazydoc.egg-info/PKG-INFO` & `crazydoc-0.1.6/crazydoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crazydoc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Read genetic sequences from stylized docx files
 Home-page: https://github.com/Edinburgh-Genome-Foundry/crazydoc
 Author: Zulko
 License: MIT
 Keywords: dna-sequence bioinformatics systems-biology docx
 Platform: UNKNOWN
 License-File: LICENCE.txt
```

### Comparing `crazydoc-0.1.5/examples/basic_example.py` & `crazydoc-0.1.6/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/ez_setup.py` & `crazydoc-0.1.6/ez_setup.py`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/pypi-readme.rst` & `crazydoc-0.1.6/pypi-readme.rst`

 * *Files identical despite different names*

### Comparing `crazydoc-0.1.5/setup.py` & `crazydoc-0.1.6/setup.py`

 * *Files identical despite different names*

