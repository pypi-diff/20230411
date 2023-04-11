# Comparing `tmp/gastimator-0.4.6.tar.gz` & `tmp/gastimator-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gastimator-0.4.6.tar", last modified: Tue Mar 14 17:46:22 2023, max compression
+gzip compressed data, was "gastimator-0.4.7.tar", last modified: Tue Apr 11 11:04:37 2023, max compression
```

## Comparing `gastimator-0.4.6.tar` & `gastimator-0.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-03-14 17:46:22.966176 gastimator-0.4.6/
--rw-r--r--   0 tdavis     (501) staff       (20)    35149 2020-08-19 16:59:58.000000 gastimator-0.4.6/LICENSE
--rw-r--r--   0 tdavis     (501) staff       (20)     1873 2023-03-14 17:46:22.966026 gastimator-0.4.6/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)     1308 2022-02-14 17:26:04.000000 gastimator-0.4.6/README.md
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-03-14 17:46:22.964311 gastimator-0.4.6/gastimator/
--rwxr-xr-x   0 tdavis     (501) staff       (20)      120 2020-08-19 16:59:58.000000 gastimator-0.4.6/gastimator/__init__.py
--rw-r--r--   0 tdavis     (501) staff       (20)    19153 2023-03-10 17:24:42.000000 gastimator-0.4.6/gastimator/corner_plot.py
--rwxr-xr-x   0 tdavis     (501) staff       (20)    16794 2023-02-24 13:47:39.000000 gastimator-0.4.6/gastimator/gastimator.py
--rwxr-xr-x   0 tdavis     (501) staff       (20)      422 2022-06-01 11:02:19.000000 gastimator-0.4.6/gastimator/priors.py
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-03-14 17:46:22.965155 gastimator-0.4.6/gastimator.egg-info/
--rw-r--r--   0 tdavis     (501) staff       (20)     1873 2023-03-14 17:46:22.000000 gastimator-0.4.6/gastimator.egg-info/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)      404 2023-03-14 17:46:22.000000 gastimator-0.4.6/gastimator.egg-info/SOURCES.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-03-14 17:46:22.000000 gastimator-0.4.6/gastimator.egg-info/dependency_links.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-08-19 17:27:19.000000 gastimator-0.4.6/gastimator.egg-info/not-zip-safe
--rw-r--r--   0 tdavis     (501) staff       (20)       45 2023-03-14 17:46:22.000000 gastimator-0.4.6/gastimator.egg-info/requires.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       11 2023-03-14 17:46:22.000000 gastimator-0.4.6/gastimator.egg-info/top_level.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-03-14 17:46:22.966222 gastimator-0.4.6/setup.cfg
--rw-r--r--   0 tdavis     (501) staff       (20)      962 2023-03-14 17:46:19.000000 gastimator-0.4.6/setup.py
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-03-14 17:46:22.965743 gastimator-0.4.6/test/
--rw-r--r--   0 tdavis     (501) staff       (20)     1108 2023-02-21 10:50:31.000000 gastimator-0.4.6/test/test_gastimator.py
--rw-r--r--   0 tdavis     (501) staff       (20)     1256 2022-08-30 09:40:28.000000 gastimator-0.4.6/test/test_gastimator_prior.py
--rw-r--r--   0 tdavis     (501) staff       (20)     3693 2023-02-13 18:18:51.000000 gastimator-0.4.6/test/test_gastimator_ul.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.006528 gastimator-0.4.7/
+-rw-r--r--   0 tdavis     (501) staff       (20)    35149 2020-08-19 16:59:58.000000 gastimator-0.4.7/LICENSE
+-rw-r--r--   0 tdavis     (501) staff       (20)     1853 2023-04-11 11:04:37.006342 gastimator-0.4.7/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)     1308 2022-02-14 17:26:04.000000 gastimator-0.4.7/README.md
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.003936 gastimator-0.4.7/gastimator/
+-rwxr-xr-x   0 tdavis     (501) staff       (20)      120 2020-08-19 16:59:58.000000 gastimator-0.4.7/gastimator/__init__.py
+-rw-r--r--   0 tdavis     (501) staff       (20)    19149 2023-04-11 10:46:06.000000 gastimator-0.4.7/gastimator/corner_plot.py
+-rwxr-xr-x   0 tdavis     (501) staff       (20)    16794 2023-02-24 13:47:39.000000 gastimator-0.4.7/gastimator/gastimator.py
+-rwxr-xr-x   0 tdavis     (501) staff       (20)      422 2022-06-01 11:02:19.000000 gastimator-0.4.7/gastimator/priors.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.004927 gastimator-0.4.7/gastimator.egg-info/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1853 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)      404 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/SOURCES.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/dependency_links.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-08-19 17:27:19.000000 gastimator-0.4.7/gastimator.egg-info/not-zip-safe
+-rw-r--r--   0 tdavis     (501) staff       (20)       45 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/requires.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       11 2023-04-11 11:04:36.000000 gastimator-0.4.7/gastimator.egg-info/top_level.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-04-11 11:04:37.006576 gastimator-0.4.7/setup.cfg
+-rw-r--r--   0 tdavis     (501) staff       (20)      962 2023-04-11 10:46:42.000000 gastimator-0.4.7/setup.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-04-11 11:04:37.005846 gastimator-0.4.7/test/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1108 2023-02-21 10:50:31.000000 gastimator-0.4.7/test/test_gastimator.py
+-rw-r--r--   0 tdavis     (501) staff       (20)     1256 2022-08-30 09:40:28.000000 gastimator-0.4.7/test/test_gastimator_prior.py
+-rw-r--r--   0 tdavis     (501) staff       (20)     3693 2023-02-13 18:18:51.000000 gastimator-0.4.7/test/test_gastimator_ul.py
```

### Comparing `gastimator-0.4.6/LICENSE` & `gastimator-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.6/PKG-INFO` & `gastimator-0.4.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gastimator
-Version: 0.4.6
+Version: 0.4.7
 Summary: Implementation of a Python MCMC gibbs-sampler with adaptive stepping
 Home-page: https://github.com/TimothyADavis/GAStimator
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: GNU GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -39,9 +38,7 @@
 Author & License
 -----------------
 
 Copyright 2019 Timothy A. Davis
 
 Built by `Timothy A. Davis <https://github.com/TimothyADavis>`. Licensed under
 the GNU General Public License v3 (GPLv3) license (see ``LICENSE``).
-
-
```

### Comparing `gastimator-0.4.6/README.md` & `gastimator-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.6/gastimator/corner_plot.py` & `gastimator-0.4.7/gastimator/corner_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         extents = np.array(extents).T
         assert len(extents) == xs.shape[0], 'lengths of extents must match number of dimensions'
 
     if weights is not None:
         weights = np.asarray(weights)
         assert weights.ndim == 1, 'weights must be 1-D'
         assert xs.shape[1] == weights.shape[0], 'lengths of weights must match number of samples'
-    if "sauron" not in cm._cmap_registry.keys():
+    if "sauron" not in cm._colormaps.keys():
         register_sauron_colormap()
 
     # backwards-compatibility
     plot_contours = kwargs.get("smooth", plot_contours)
 
     K = len(xs)
     if fig is None:
```

### Comparing `gastimator-0.4.6/gastimator/gastimator.py` & `gastimator-0.4.7/gastimator/gastimator.py`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.6/gastimator.egg-info/PKG-INFO` & `gastimator-0.4.7/gastimator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: gastimator
-Version: 0.4.6
+Version: 0.4.7
 Summary: Implementation of a Python MCMC gibbs-sampler with adaptive stepping
 Home-page: https://github.com/TimothyADavis/GAStimator
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: GNU GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -39,9 +38,7 @@
 Author & License
 -----------------
 
 Copyright 2019 Timothy A. Davis
 
 Built by `Timothy A. Davis <https://github.com/TimothyADavis>`. Licensed under
 the GNU General Public License v3 (GPLv3) license (see ``LICENSE``).
-
-
```

### Comparing `gastimator-0.4.6/setup.py` & `gastimator-0.4.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
  
 setup(name='gastimator',
-       version='0.4.6',
+       version='0.4.7',
        description='Implementation of a Python MCMC gibbs-sampler with adaptive stepping',
        url='https://github.com/TimothyADavis/GAStimator',
        author='Timothy A. Davis',
        author_email='DavisT@cardiff.ac.uk',
        long_description=long_description,
        long_description_content_type="text/markdown",
        license='GNU GPLv3',
```

### Comparing `gastimator-0.4.6/test/test_gastimator.py` & `gastimator-0.4.7/test/test_gastimator.py`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.6/test/test_gastimator_prior.py` & `gastimator-0.4.7/test/test_gastimator_prior.py`

 * *Files identical despite different names*

### Comparing `gastimator-0.4.6/test/test_gastimator_ul.py` & `gastimator-0.4.7/test/test_gastimator_ul.py`

 * *Files identical despite different names*

