# Comparing `tmp/DA4RDM_Vis_ProcessBased-0.1.7.tar.gz` & `tmp/DA4RDM_Vis_ProcessBased-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DA4RDM_Vis_ProcessBased-0.1.7.tar", last modified: Tue Apr 11 15:30:28 2023, max compression
+gzip compressed data, was "DA4RDM_Vis_ProcessBased-0.1.8.tar", last modified: Tue Apr 11 15:42:46 2023, max compression
```

## Comparing `DA4RDM_Vis_ProcessBased-0.1.7.tar` & `DA4RDM_Vis_ProcessBased-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:30:28.005045 DA4RDM_Vis_ProcessBased-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-04-11 15:30:27.959054 DA4RDM_Vis_ProcessBased-0.1.7/DA4RDM_Vis_ProcessBased.egg-info/
--rw-rw-rw-   0        0        0     4075 2023-04-11 15:30:27.000000 DA4RDM_Vis_ProcessBased-0.1.7/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2023-04-11 15:30:27.000000 DA4RDM_Vis_ProcessBased-0.1.7/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:30:27.000000 DA4RDM_Vis_ProcessBased-0.1.7/DA4RDM_Vis_ProcessBased.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-11 15:30:27.000000 DA4RDM_Vis_ProcessBased-0.1.7/DA4RDM_Vis_ProcessBased.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1072 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       51 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4075 2023-04-11 15:30:28.005562 DA4RDM_Vis_ProcessBased-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3613 2023-04-11 15:28:46.000000 DA4RDM_Vis_ProcessBased-0.1.7/README.md
--rw-rw-rw-   0        0        0      473 2023-04-11 15:28:58.000000 DA4RDM_Vis_ProcessBased-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0      303 2023-04-11 15:30:28.016438 DA4RDM_Vis_ProcessBased-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      999 2023-04-11 15:29:41.000000 DA4RDM_Vis_ProcessBased-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:30:27.823938 DA4RDM_Vis_ProcessBased-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 15:30:27.972823 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/
--rw-rw-rw-   0        0        0     1764 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py
--rw-rw-rw-   0        0        0     1351 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/Extract.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:30:28.002470 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/
--rw-rw-rw-   0        0        0      581 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv
--rw-rw-rw-   0        0        0      503 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Analysis.csv
--rw-rw-rw-   0        0        0      619 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv
--rw-rw-rw-   0        0        0      929 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv
--rw-rw-rw-   0        0        0     1001 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv
--rw-rw-rw-   0        0        0      687 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv
--rw-rw-rw-   0        0        0     3586 2023-04-11 15:17:03.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/Visualize.py
--rw-rw-rw-   0        0        0        0 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:42:46.274939 DA4RDM_Vis_ProcessBased-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:42:46.249827 DA4RDM_Vis_ProcessBased-0.1.8/DA4RDM_Vis_ProcessBased.egg-info/
+-rw-rw-rw-   0        0        0     4109 2023-04-11 15:42:46.000000 DA4RDM_Vis_ProcessBased-0.1.8/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2023-04-11 15:42:46.000000 DA4RDM_Vis_ProcessBased-0.1.8/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:42:46.000000 DA4RDM_Vis_ProcessBased-0.1.8/DA4RDM_Vis_ProcessBased.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-11 15:42:46.000000 DA4RDM_Vis_ProcessBased-0.1.8/DA4RDM_Vis_ProcessBased.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1072 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4109 2023-04-11 15:42:46.274939 DA4RDM_Vis_ProcessBased-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3613 2023-04-11 15:28:46.000000 DA4RDM_Vis_ProcessBased-0.1.8/README.md
+-rw-rw-rw-   0        0        0      507 2023-04-11 15:42:04.000000 DA4RDM_Vis_ProcessBased-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      303 2023-04-11 15:42:46.284576 DA4RDM_Vis_ProcessBased-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-04-11 15:41:17.000000 DA4RDM_Vis_ProcessBased-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:42:46.211081 DA4RDM_Vis_ProcessBased-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:42:46.258816 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/
+-rw-rw-rw-   0        0        0     1764 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py
+-rw-rw-rw-   0        0        0     1351 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/Extract.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:42:46.272895 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/
+-rw-rw-rw-   0        0        0      581 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv
+-rw-rw-rw-   0        0        0      503 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Analysis.csv
+-rw-rw-rw-   0        0        0      619 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv
+-rw-rw-rw-   0        0        0      929 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv
+-rw-rw-rw-   0        0        0     1001 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv
+-rw-rw-rw-   0        0        0      687 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv
+-rw-rw-rw-   0        0        0     3586 2023-04-11 15:17:03.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/Visualize.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/__init__.py
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO` & `DA4RDM_Vis_ProcessBased-0.1.8/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: DA4RDM-Vis-ProcessBased
-Version: 0.1.7
-Summary: Test package to get visualisation for a given projectid as reference analyzed on different RDLC phase process models
+Version: 0.1.8
+Summary: Package to get visualisation of fitness values corresponding to RDLC phases for a reference projectid using alignment based process mining evaluations
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DA4RDM_Vis_ProcessBased
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt` & `DA4RDM_Vis_ProcessBased-0.1.8/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/LICENSE` & `DA4RDM_Vis_ProcessBased-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/PKG-INFO` & `DA4RDM_Vis_ProcessBased-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: DA4RDM_Vis_ProcessBased
-Version: 0.1.7
-Summary: Test package to get visualisation for a given projectid as reference analyzed on different RDLC phase process models
+Version: 0.1.8
+Summary: Package to get visualisation of fitness values corresponding to RDLC phases for a reference projectid using alignment based process mining evaluations
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DA4RDM_Vis_ProcessBased
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/README.md` & `DA4RDM_Vis_ProcessBased-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/setup.py` & `DA4RDM_Vis_ProcessBased-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='DA4RDM_Vis_ProcessBased',
-      version='0.1.7',
-      description='Test package to get visualisation for a given projectid as reference analyzed '
-                  'on different RDLC phase process models',
+      version='0.1.8',
+      description='Package to get visualisation of fitness values corresponding to RDLC phases for a reference projectid'
+                  'using alignment based process mining evaluations',
       long_description=readme(),
       classifiers=[
           "Programming Language :: Python :: 3.9",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",	
       ],
       packages = ['DA4RDM_Vis_ProcessBased'],
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/Extract.py` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/Extract.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.7/src/DA4RDM_Vis_ProcessBased/Visualize.py` & `DA4RDM_Vis_ProcessBased-0.1.8/src/DA4RDM_Vis_ProcessBased/Visualize.py`

 * *Files identical despite different names*

