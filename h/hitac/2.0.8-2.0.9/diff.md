# Comparing `tmp/hitac-2.0.8.tar.gz` & `tmp/hitac-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hitac-2.0.8.tar", last modified: Fri Dec 24 11:59:22 2021, max compression
+gzip compressed data, was "hitac-2.0.9.tar", last modified: Wed Jul 20 13:11:24 2022, max compression
```

## Comparing `hitac-2.0.8.tar` & `hitac-2.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 11:59:22.957713 hitac-2.0.8/
--rwxrwxrwx   0 root         (0) root         (0)    35058 2021-12-24 11:59:14.000000 hitac-2.0.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      122 2021-12-24 11:59:14.000000 hitac-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6963 2021-12-24 11:59:22.957713 hitac-2.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6177 2021-12-24 11:59:14.000000 hitac-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 11:59:22.958713 hitac-2.0.8/hitac/
--rw-rw-rw-   0 root         (0) root         (0)      288 2021-12-24 11:59:14.000000 hitac-2.0.8/hitac/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6605 2021-12-24 11:59:14.000000 hitac-2.0.8/hitac/_hierarchical_taxonomic_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)     7581 2021-12-24 11:59:14.000000 hitac-2.0.8/hitac/_utils.py
--rw-r--r--   0 root         (0) root         (0)      497 2021-12-24 11:59:22.958713 hitac-2.0.8/hitac/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2021-12-24 11:59:14.000000 hitac-2.0.8/hitac/citations.bib
--rw-rw-rw-   0 root         (0) root         (0)     9378 2021-12-24 11:59:14.000000 hitac-2.0.8/hitac/classifier.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2021-12-24 11:59:14.000000 hitac-2.0.8/hitac/plugin_setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 11:59:22.957713 hitac-2.0.8/hitac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6963 2021-12-24 11:59:22.000000 hitac-2.0.8/hitac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      396 2021-12-24 11:59:22.000000 hitac-2.0.8/hitac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-24 11:59:22.000000 hitac-2.0.8/hitac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2021-12-24 11:59:22.000000 hitac-2.0.8/hitac.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2021-12-24 11:59:22.000000 hitac-2.0.8/hitac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-12-24 11:59:22.000000 hitac-2.0.8/hitac.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      557 2021-12-24 11:59:22.958713 hitac-2.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4422 2021-12-24 11:59:14.000000 hitac-2.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    70238 2021-12-24 11:59:14.000000 hitac-2.0.8/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 13:11:24.217494 hitac-2.0.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1529 2022-07-20 13:11:15.000000 hitac-2.0.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      122 2022-07-20 13:11:15.000000 hitac-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6971 2022-07-20 13:11:24.217494 hitac-2.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6185 2022-07-20 13:11:15.000000 hitac-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 13:11:24.218495 hitac-2.0.9/hitac/
+-rw-rw-rw-   0 root         (0) root         (0)      288 2022-07-20 13:11:15.000000 hitac-2.0.9/hitac/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6605 2022-07-20 13:11:15.000000 hitac-2.0.9/hitac/_hierarchical_taxonomic_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     7581 2022-07-20 13:11:15.000000 hitac-2.0.9/hitac/_utils.py
+-rw-r--r--   0 root         (0) root         (0)      497 2022-07-20 13:11:24.218495 hitac-2.0.9/hitac/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2022-07-20 13:11:15.000000 hitac-2.0.9/hitac/citations.bib
+-rw-rw-rw-   0 root         (0) root         (0)     9378 2022-07-20 13:11:15.000000 hitac-2.0.9/hitac/classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2022-07-20 13:11:15.000000 hitac-2.0.9/hitac/plugin_setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 13:11:24.217494 hitac-2.0.9/hitac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6971 2022-07-20 13:11:24.000000 hitac-2.0.9/hitac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      396 2022-07-20 13:11:24.000000 hitac-2.0.9/hitac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-20 13:11:24.000000 hitac-2.0.9/hitac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2022-07-20 13:11:24.000000 hitac-2.0.9/hitac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2022-07-20 13:11:24.000000 hitac-2.0.9/hitac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-07-20 13:11:24.000000 hitac-2.0.9/hitac.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      557 2022-07-20 13:11:24.218495 hitac-2.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4422 2022-07-20 13:11:15.000000 hitac-2.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    70238 2022-07-20 13:11:15.000000 hitac-2.0.9/versioneer.py
```

### Comparing `hitac-2.0.8/PKG-INFO` & `hitac-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hitac
-Version: 2.0.8
+Version: 2.0.9
 Summary: Hierarchical taxonomic classifier.
 Home-page: UNKNOWN
 Author: Fabio Malcher Miranda
 Author-email: fabio.malchermiranda@hpi.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://gitlab.com/dacs-hpi/hitac/-/issues
 Project-URL: Source Code, https://gitlab.com/dacs-hpi/hitac
@@ -18,15 +18,15 @@
 Requires-Python: >=3.8.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # HiTaC
 
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![pipeline status](https://gitlab.com/dacs-hpi/hitac/badges/master/pipeline.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master) [![coverage report](https://gitlab.com/dacs-hpi/hitac/badges/master/coverage.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![pipeline status](https://gitlab.com/dacs-hpi/hitac/badges/master/pipeline.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master) [![coverage report](https://gitlab.com/dacs-hpi/hitac/badges/master/coverage.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master)
 
 A hierarchical taxonomic classifier for fungal ITS sequences.
 
 ## Installation
 
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/hitac/README.html)
```

### Comparing `hitac-2.0.8/README.md` & `hitac-2.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HiTaC
 
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![pipeline status](https://gitlab.com/dacs-hpi/hitac/badges/master/pipeline.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master) [![coverage report](https://gitlab.com/dacs-hpi/hitac/badges/master/coverage.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![pipeline status](https://gitlab.com/dacs-hpi/hitac/badges/master/pipeline.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master) [![coverage report](https://gitlab.com/dacs-hpi/hitac/badges/master/coverage.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master)
 
 A hierarchical taxonomic classifier for fungal ITS sequences.
 
 ## Installation
 
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/hitac/README.html)
```

### Comparing `hitac-2.0.8/hitac/_hierarchical_taxonomic_classifier.py` & `hitac-2.0.9/hitac/_hierarchical_taxonomic_classifier.py`

 * *Files identical despite different names*

### Comparing `hitac-2.0.8/hitac/_utils.py` & `hitac-2.0.9/hitac/_utils.py`

 * *Files identical despite different names*

### Comparing `hitac-2.0.8/hitac/classifier.py` & `hitac-2.0.9/hitac/classifier.py`

 * *Files identical despite different names*

### Comparing `hitac-2.0.8/hitac/plugin_setup.py` & `hitac-2.0.9/hitac/plugin_setup.py`

 * *Files identical despite different names*

### Comparing `hitac-2.0.8/hitac.egg-info/PKG-INFO` & `hitac-2.0.9/hitac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hitac
-Version: 2.0.8
+Version: 2.0.9
 Summary: Hierarchical taxonomic classifier.
 Home-page: UNKNOWN
 Author: Fabio Malcher Miranda
 Author-email: fabio.malchermiranda@hpi.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://gitlab.com/dacs-hpi/hitac/-/issues
 Project-URL: Source Code, https://gitlab.com/dacs-hpi/hitac
@@ -18,15 +18,15 @@
 Requires-Python: >=3.8.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # HiTaC
 
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![pipeline status](https://gitlab.com/dacs-hpi/hitac/badges/master/pipeline.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master) [![coverage report](https://gitlab.com/dacs-hpi/hitac/badges/master/coverage.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![pipeline status](https://gitlab.com/dacs-hpi/hitac/badges/master/pipeline.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master) [![coverage report](https://gitlab.com/dacs-hpi/hitac/badges/master/coverage.svg)](https://gitlab.com/dacs-hpi/hitac/-/commits/master)
 
 A hierarchical taxonomic classifier for fungal ITS sequences.
 
 ## Installation
 
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/hitac/README.html)
```

### Comparing `hitac-2.0.8/setup.cfg` & `hitac-2.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 max-line-length = 120
 exclude = **/__init__.py,  docs/source/conf.py
 
 [requires]
 python_version = ">=3.8.3"
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = hitac/_version.py
 versionfile_build = hitac/_version.py
 tag_prefix = 
 parentdir_prefix = hitac-
 
 [egg_info]
```

### Comparing `hitac-2.0.8/setup.py` & `hitac-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `hitac-2.0.8/versioneer.py` & `hitac-2.0.9/versioneer.py`

 * *Files identical despite different names*

