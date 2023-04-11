# Comparing `tmp/multicons-0.1.0.tar.gz` & `tmp/multicons-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicons-0.1.0.tar", last modified: Wed May 18 08:27:06 2022, max compression
+gzip compressed data, was "multicons-0.2.0.tar", last modified: Tue Apr 11 12:51:51 2023, max compression
```

## Comparing `multicons-0.1.0.tar` & `multicons-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-18 08:27:06.487258 multicons-0.1.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2022-05-18 08:27:05.000000 multicons-0.1.0/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2022-05-18 08:27:06.487258 multicons-0.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1024 2022-05-18 08:27:05.000000 multicons-0.1.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1733 2022-05-18 08:27:06.487258 multicons-0.1.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2022-05-18 08:27:05.000000 multicons-0.1.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-18 08:27:06.487258 multicons-0.1.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-18 08:27:06.487258 multicons-0.1.0/src/multicons/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      394 2022-05-18 08:27:05.000000 multicons-0.1.0/src/multicons/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10315 2022-05-18 08:27:05.000000 multicons-0.1.0/src/multicons/consensus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16948 2022-05-18 08:27:05.000000 multicons-0.1.0/src/multicons/core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4867 2022-05-18 08:27:05.000000 multicons-0.1.0/src/multicons/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-18 08:27:06.487258 multicons-0.1.0/src/multicons.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2022-05-18 08:27:06.000000 multicons-0.1.0/src/multicons.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2022-05-18 08:27:06.000000 multicons-0.1.0/src/multicons.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-18 08:27:06.000000 multicons-0.1.0/src/multicons.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      386 2022-05-18 08:27:06.000000 multicons-0.1.0/src/multicons.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-05-18 08:27:06.000000 multicons-0.1.0/src/multicons.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-18 08:27:06.000000 multicons-0.1.0/src/multicons.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1066 2023-04-11 12:51:51.000000 multicons-0.2.0/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2023-04-11 12:51:51.783020 multicons-0.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1167 2023-04-11 12:51:51.000000 multicons-0.2.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1777 2023-04-11 12:51:51.787020 multicons-0.2.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-04-11 12:51:51.000000 multicons-0.2.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/src/multicons/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      394 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10315 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/consensus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16948 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4867 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 12:51:51.783020 multicons-0.2.0/src/multicons.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-11 12:51:51.000000 multicons-0.2.0/src/multicons.egg-info/zip-safe
```

### Comparing `multicons-0.1.0/LICENSE.md` & `multicons-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multicons-0.1.0/PKG-INFO` & `multicons-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicons
-Version: 0.1.0
+Version: 0.2.0
 Summary: MultiCons (Multiple Consensuses) algorithm
 Home-page: https://github.com/SergioSim/multicons
 Author: SergioSim
 Author-email: sergio.simonian@etu.univ-cotedazur.fr
 License: MIT
 Keywords: MultiCons,Multiple Consensuses,Consensus clustering
 Platform: UNKNOWN
@@ -27,15 +27,23 @@
 
 MultiCons is a consensus clustering method that uses the frequent closed itemset mining
 technique to find similarities in the base clustering solutions.
 
 The implementation aims to follow the original description of the MultiCons method from
 the references below.
 
-# Documentation
+## Installation
+
+MultiCons is available on the Python Package Index (PyPI). It's installable using `pip`:
+
+```bash
+pip install multicons
+```
+
+## Documentation
 
 To get started, check out some examples or look up the reference API, please visit our
 [documentation page](https://sergiosim.github.io/multicons/).
 
 ## References
 
 Atheer A. "A closed patterns-based approach to the consensus clustering problem".
```

### Comparing `multicons-0.1.0/README.md` & `multicons-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 
 MultiCons is a consensus clustering method that uses the frequent closed itemset mining
 technique to find similarities in the base clustering solutions.
 
 The implementation aims to follow the original description of the MultiCons method from
 the references below.
 
-# Documentation
+## Installation
+
+MultiCons is available on the Python Package Index (PyPI). It's installable using `pip`:
+
+```bash
+pip install multicons
+```
+
+## Documentation
 
 To get started, check out some examples or look up the reference API, please visit our
 [documentation page](https://sergiosim.github.io/multicons/).
 
 ## References
 
 Atheer A. "A closed patterns-based approach to the consensus clustering problem".
```

### Comparing `multicons-0.1.0/setup.cfg` & `multicons-0.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multicons
-version = 0.1.0
+version = 0.2.0
 description = MultiCons (Multiple Consensuses) algorithm
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = SergioSim
 author_email = sergio.simonian@etu.univ-cotedazur.fr
 url = https://github.com/SergioSim/multicons
 license = MIT
@@ -16,45 +16,46 @@
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 
 [options]
 include_package_data = True
 install_requires = 
-	graphviz==0.20
-	numpy==1.22.3
-	pandas==1.4.2
-	pyfim==6.28
-	scikit-learn==1.0.2
+	graphviz>=0.20
+	numpy>=1.24.0
+	pandas>=2.0.0
+	pyfim>=6.28
+	scikit-learn>=1.2.0
 package_dir = 
 	=src
 packages = find:
 zip_safe = True
 python_requires = >= 3.9
 
 [options.extras_require]
 dev = 
-	bandit==1.7.4
-	black==22.3.0
-	flake8==4.0.1
-	fuzzy-c-means==1.6.4
-	isort==5.10.1
-	jupyterlab==3.4.0
-	jupytext==1.13.8
-	matplotlib==3.5.2
-	mkdocs==1.3.0
-	mkdocs-jupyter==0.20.1
-	mkdocs-material==8.2.13
-	mkdocstrings==0.18.1
-	pylint==2.13.7
-	pytest==7.1.2
-	pytest-cov==3.0.0
-	scikit-learn-extra==0.2.0
+	bandit==1.7.5
+	black==23.3.0
+	flake8==6.0.0
+	fuzzy-c-means==1.7.0
+	isort==5.12.0
+	jupyterlab==3.6.3
+	jupyter_contrib_nbextensions==0.7.0
+	jupytext==1.14.5
+	matplotlib==3.7.1
+	mkdocs==1.4.2
+	mkdocs-jupyter==0.24.1
+	mkdocs-material==9.1.6
+	mkdocstrings[python]==0.21.2
+	pylint==2.17.2
+	pytest==7.3.0
+	pytest-cov==4.0.0
+	scikit-learn-extra==0.3.0
 ci = 
-	twine==3.5.0
+	twine==4.0.2
 
 [options.packages.find]
 where = src
 
 [wheel]
 universal = 1
```

### Comparing `multicons-0.1.0/src/multicons/consensus.py` & `multicons-0.2.0/src/multicons/consensus.py`

 * *Files identical despite different names*

### Comparing `multicons-0.1.0/src/multicons/core.py` & `multicons-0.2.0/src/multicons/core.py`

 * *Files identical despite different names*

### Comparing `multicons-0.1.0/src/multicons/utils.py` & `multicons-0.2.0/src/multicons/utils.py`

 * *Files identical despite different names*

### Comparing `multicons-0.1.0/src/multicons.egg-info/PKG-INFO` & `multicons-0.2.0/src/multicons.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicons
-Version: 0.1.0
+Version: 0.2.0
 Summary: MultiCons (Multiple Consensuses) algorithm
 Home-page: https://github.com/SergioSim/multicons
 Author: SergioSim
 Author-email: sergio.simonian@etu.univ-cotedazur.fr
 License: MIT
 Keywords: MultiCons,Multiple Consensuses,Consensus clustering
 Platform: UNKNOWN
@@ -27,15 +27,23 @@
 
 MultiCons is a consensus clustering method that uses the frequent closed itemset mining
 technique to find similarities in the base clustering solutions.
 
 The implementation aims to follow the original description of the MultiCons method from
 the references below.
 
-# Documentation
+## Installation
+
+MultiCons is available on the Python Package Index (PyPI). It's installable using `pip`:
+
+```bash
+pip install multicons
+```
+
+## Documentation
 
 To get started, check out some examples or look up the reference API, please visit our
 [documentation page](https://sergiosim.github.io/multicons/).
 
 ## References
 
 Atheer A. "A closed patterns-based approach to the consensus clustering problem".
```

