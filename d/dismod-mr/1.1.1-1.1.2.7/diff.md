# Comparing `tmp/dismod_mr-1.1.1.tar.gz` & `tmp/dismod_mr-1.1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dismod_mr-1.1.1.tar", last modified: Wed Nov  6 18:13:54 2019, max compression
+gzip compressed data, was "dismod_mr-1.1.2.7.tar", last modified: Tue Apr 11 02:27:59 2023, max compression
```

## Comparing `dismod_mr-1.1.1.tar` & `dismod_mr-1.1.2.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4674 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/src/dismod_mr/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15467 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/fit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16480 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/plot.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/src/dismod_mr/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)    23722 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/covariates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7754 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/priors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12070 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/likelihood.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2568 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/ode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23400 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3060 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/spline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5652 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/age_groups.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      950 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23529 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       77 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/__about__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/src/dismod_mr/testing/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/src/dismod_mr/testing/example_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6527 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/testing/example_data/hierarchy.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1494 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/testing/example_data/input_data.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       29 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/testing/example_data/output_template.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/testing/example_data/nodes_to_fit.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/testing/example_data/parameters.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4106 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/testing/data_simulation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/src/dismod_mr/testing/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/src/dismod_mr.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4674 2019-11-06 18:13:53.000000 dismod_mr-1.1.1/src/dismod_mr.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-06 18:13:53.000000 dismod_mr-1.1.1/src/dismod_mr.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-11-06 18:13:53.000000 dismod_mr-1.1.1/src/dismod_mr.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-06 18:13:53.000000 dismod_mr-1.1.1/src/dismod_mr.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2019-11-06 18:13:53.000000 dismod_mr-1.1.1/src/dismod_mr.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2019-11-06 18:13:53.000000 dismod_mr-1.1.1/src/dismod_mr.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    34520 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2778 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2125 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-06 18:13:54.000000 dismod_mr-1.1.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20182 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_covariates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      972 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_model_likelihood.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      715 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_fit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      750 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_spline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_plot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_model_setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1981 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_priors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4718 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2178 2019-11-06 18:11:03.000000 dismod_mr-1.1.1/tests/test_age_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.988964 dismod_mr-1.1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-11 02:27:59.988964 dismod_mr-1.1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:27:59.988964 dismod_mr-1.1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.984964 dismod_mr-1.1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.984964 dismod_mr-1.1.2.7/src/dismod_mr/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.984964 dismod_mr-1.1.2.7/src/dismod_mr/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/age_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/covariates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/model/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.984964 dismod_mr-1.1.2.7/src/dismod_mr/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/testing/data_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.988964 dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/hierarchy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/input_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/nodes_to_fit.json
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/output_template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/parameters.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.984964 dismod_mr-1.1.2.7/src/dismod_mr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-11 02:27:59.000000 dismod_mr-1.1.2.7/src/dismod_mr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-11 02:27:59.000000 dismod_mr-1.1.2.7/src/dismod_mr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:27:59.000000 dismod_mr-1.1.2.7/src/dismod_mr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:27:59.000000 dismod_mr-1.1.2.7/src/dismod_mr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 02:27:59.000000 dismod_mr-1.1.2.7/src/dismod_mr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 02:27:59.000000 dismod_mr-1.1.2.7/src/dismod_mr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:27:59.988964 dismod_mr-1.1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_age_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_covariates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_model_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_model_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-11 02:27:52.000000 dismod_mr-1.1.2.7/tests/test_spline.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dismod_mr-1.1.1/PKG-INFO` & `dismod_mr-1.1.2.7/src/dismod_mr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,15 @@
-Metadata-Version: 1.1
-Name: dismod_mr
-Version: 1.1.1
+Metadata-Version: 2.1
+Name: dismod-mr
+Version: 1.1.2.7
 Summary: Integrative Meta-Regression Framework for Descriptive Epidemmiology
 Home-page: https://github.com/ihmeuw/dismod_mr
 Author: Abraham D. Flaxman
 Author-email: abie@uw.edu
 License: GNU GPLv3
-Description: .. image:: https://travis-ci.org/ihmeuw/dismod_mr.svg?branch=master
-            :target: https://travis-ci.org/ihmeuw/dismod_mr
-            :alt: Latest Version
-        
-        ============
-        Introduction
-        ============
-        
-        This project is the descriptive epidemiological meta-regression tool,
-        DisMod-MR, which grew out of the Global Burden of Disease (GBD) Study
-        2010.  DisMod-MR has been developed for the Institute of Health
-        Metrics and Evaluation at the University of Washington from 2008-2013.
-        
-        .. contents::
-        
-        Examples
-        --------
-        
-        `A motivating example: descriptive epidemiological meta-regression of Parkinson's Disease <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/blob/master/examples/pd_sim_data.ipynb>`_
-        
-        `All examples <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/tree/master/examples/>`_
-        
-        Installation
-        ------------
-        
-        Dismod MR requires PyMC2 which does not play nicely with normal Python
-        installation tools.  Fortunately, ``conda`` has solved this issue for us.
-        So first you'll need to setup a conda environment
-        (after `installing conda, if necessary <https://docs.conda.io/projects/conda/en/latest/user-guide/install/>`_)
-        and install ``pymc``.  Then you can install ``dismod_mr`` using ``pip``.
-        
-        .. code-block:: sh
-        
-           conda create --name=dismod_mr python=3.6 pymc
-           conda activate dismod_mr
-           pip install dismod_mr
-        
-        If you get an error stating
-        
-        .. code-block:: sh
-        
-           ERROR: Complete output from command python setup.py egg_info:
-           ERROR: Traceback (most recent call last):
-             File "<string>", line 1, in <module>
-             File "/tmp/pip-install-d9fbq7v3/pymc/setup.py", line 8, in <module>
-               from numpy.distutils.misc_util import Configuration
-           ModuleNotFoundError: No module named 'numpy'
-           ----------------------------------------
-           ERROR: Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-install-d9fbq7v3/pymc/
-        
-        or something similar, you do not have ``pymc`` properly installed.
-        
-        
-        Installing from source
-        ++++++++++++++++++++++
-        
-        If you want to install ``dismod_mr`` locally in an editable mode, the
-        instructions are very similar.  We'll clone the repository and install it
-        from a local directory instead of using ``pip`` to grab it from the Python
-        package index.
-        
-        .. code-block:: sh
-        
-           conda create --name=dismod_mr python=3.6 pymc
-           conda activate dismod_mr
-           git clone git@github.com:ihmeuw/dismod_mr.git
-           cd dismod_mr
-           pip install -e .
-        
-        Coding Practices
-        ----------------
-        
-        * Write tests before code
-        * Write equations before tests
-        
-        * Test quantitatively with simulation data
-        * Test qualitatively with real data
-        * Automate tests
-        
-        * Use a package instead of DIY
-        * Test the package
-        
-        * Optimize code later
-        * Optimize code for readability before speed
-        
-        * `.py` files should be short, less than 500 lines
-        * Functions should be short, less than 25 lines
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -109,7 +20,103 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ihmeuw/dismod_mr.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/dismod_mr
+    :alt: Latest Version
+
+This project is the descriptive epidemiological meta-regression tool,
+DisMod-MR, which grew out of the Global Burden of Disease (GBD) Study
+2010.  DisMod-MR has been developed for the Institute of Health
+Metrics and Evaluation at the University of Washington from 2008-2013.
+
+.. contents::
+
+Examples
+--------
+
+`A motivating example: descriptive epidemiological meta-regression of Parkinson's Disease <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/blob/master/examples/pd_sim_data.ipynb>`_
+
+`All examples <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/tree/master/examples/>`_
+
+Installation
+------------
+
+Dismod MR requires PyMC2 which does not play nicely with normal Python
+installation tools.  Fortunately, ``conda`` has solved this issue for us.
+So first you'll need to setup a conda environment
+(after `installing conda, if necessary <https://docs.conda.io/projects/conda/en/latest/user-guide/install/>`_)
+and install ``pymc`` version ``2.3.8``.  Then you can install ``dismod_mr`` using ``pip``.
+
+.. code-block:: sh
+
+   conda create --name=dismod_mr python=3.6 pymc==2.3.8
+   conda activate dismod_mr
+   pip install dismod_mr
+
+If you get an error stating
+
+.. code-block:: sh
+
+   ERROR: Complete output from command python setup.py egg_info:
+   ERROR: Traceback (most recent call last):
+     File "<string>", line 1, in <module>
+     File "/tmp/pip-install-d9fbq7v3/pymc/setup.py", line 8, in <module>
+       from numpy.distutils.misc_util import Configuration
+   ModuleNotFoundError: No module named 'numpy'
+   ----------------------------------------
+   ERROR: Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-install-d9fbq7v3/pymc/
+
+or something similar, you do not have ``pymc`` properly installed.
+
+
+Installing from source
+++++++++++++++++++++++
+
+If you want to install ``dismod_mr`` locally in an editable mode, the
+instructions are very similar.  We'll clone the repository and install it
+from a local directory instead of using ``pip`` to grab it from the Python
+package index.
+
+.. code-block:: sh
+
+   conda create --name=dismod_mr python=3.6 pymc==2.3.8
+   conda activate dismod_mr
+   git clone git@github.com:ihmeuw/dismod_mr.git
+   cd dismod_mr
+   pip install -e .
+
+To test this, you can use ``pytest``, which you must first install.
+
+.. code-block:: sh
+
+   pip install pytest
+   pytest
+
+If you have things setup right, this will still generate many
+warnings, but there should be no tests that produce failures or
+errors.
+
+Coding Practices
+----------------
+
+* Write tests before code
+* Write equations before tests
+
+* Test quantitatively with simulation data
+* Test qualitatively with real data
+* Automate tests
+
+* Use a package instead of DIY
+* Test the package
+
+* Optimize code later
+* Optimize code for readability before speed
+
+* `.py` files should be short, less than 500 lines
+* Functions should be short, less than 25 lines
```

### Comparing `dismod_mr-1.1.1/src/dismod_mr/fit.py` & `dismod_mr-1.1.2.7/src/dismod_mr/fit.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/plot.py` & `dismod_mr-1.1.2.7/src/dismod_mr/plot.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/covariates.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/covariates.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/priors.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/priors.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/likelihood.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/likelihood.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/ode.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/ode.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         dc_da  = +           i * s - (r + other + e) * c
         return np.array( [ ds_da , dc_da ] )
 
 
 @numba.jit(nopython=True)
 def ode_function(susceptible, condition, num_step, age_local, all_cause, incidence, remission, excess, s0, c0):
         age          = age_local
-
         N = len(age)
+        t0 = age[0]
 
         susceptible[0] = s0
         condition[0]   = c0
 
         sc             = np.array( [s0, c0] )
         for j in range(N-1) :
                 a_step = (age[j+1] - age[j]) / num_step
@@ -51,18 +51,18 @@
                 ti = a_tmp
                 yi = sc
 
                 for step in range(num_step) :
 
                         # copied from http://www.seanet.com/~bradbell/pycppad/runge_kutta_4.xml
 
-                        k1 = dt * f(ti         , yi, incidence, remission, excess, all_cause)
-                        k2 = dt * f(ti + .5*dt , yi + .5*k1, incidence, remission, excess, all_cause)
-                        k3 = dt * f(ti + .5*dt , yi + .5*k2, incidence, remission, excess, all_cause)
-                        k4 = dt * f(ti + dt    , yi + k3, incidence, remission, excess, all_cause)
+                        k1 = dt * f(-t0 + ti         , yi, incidence, remission, excess, all_cause)
+                        k2 = dt * f(-t0 + ti + .5*dt , yi + .5*k1, incidence, remission, excess, all_cause)
+                        k3 = dt * f(-t0 + ti + .5*dt , yi + .5*k2, incidence, remission, excess, all_cause)
+                        k4 = dt * f(-t0 + ti + dt    , yi + k3, incidence, remission, excess, all_cause)
                         yf = yi + (1./6.) * ( k1 + 2.*k2 + 2.*k3 + k4 )
 
                         sc    = yf
 
                         a_tmp = a_tmp + a_step
                 susceptible[j+1] = sc[0]
                 condition[j+1]   = sc[1]
```

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/process.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/process.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/spline.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/spline.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/age_groups.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/age_groups.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/model/__init__.py` & `dismod_mr-1.1.2.7/src/dismod_mr/model/__init__.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/data.py` & `dismod_mr-1.1.2.7/src/dismod_mr/data.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/testing/example_data/hierarchy.json` & `dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/hierarchy.json`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/testing/example_data/input_data.csv` & `dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/input_data.csv`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/testing/example_data/parameters.json` & `dismod_mr-1.1.2.7/src/dismod_mr/testing/example_data/parameters.json`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr/testing/data_simulation.py` & `dismod_mr-1.1.2.7/src/dismod_mr/testing/data_simulation.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/src/dismod_mr.egg-info/PKG-INFO` & `dismod_mr-1.1.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,104 +1,15 @@
-Metadata-Version: 1.1
-Name: dismod-mr
-Version: 1.1.1
+Metadata-Version: 2.1
+Name: dismod_mr
+Version: 1.1.2.7
 Summary: Integrative Meta-Regression Framework for Descriptive Epidemmiology
 Home-page: https://github.com/ihmeuw/dismod_mr
 Author: Abraham D. Flaxman
 Author-email: abie@uw.edu
 License: GNU GPLv3
-Description: .. image:: https://travis-ci.org/ihmeuw/dismod_mr.svg?branch=master
-            :target: https://travis-ci.org/ihmeuw/dismod_mr
-            :alt: Latest Version
-        
-        ============
-        Introduction
-        ============
-        
-        This project is the descriptive epidemiological meta-regression tool,
-        DisMod-MR, which grew out of the Global Burden of Disease (GBD) Study
-        2010.  DisMod-MR has been developed for the Institute of Health
-        Metrics and Evaluation at the University of Washington from 2008-2013.
-        
-        .. contents::
-        
-        Examples
-        --------
-        
-        `A motivating example: descriptive epidemiological meta-regression of Parkinson's Disease <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/blob/master/examples/pd_sim_data.ipynb>`_
-        
-        `All examples <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/tree/master/examples/>`_
-        
-        Installation
-        ------------
-        
-        Dismod MR requires PyMC2 which does not play nicely with normal Python
-        installation tools.  Fortunately, ``conda`` has solved this issue for us.
-        So first you'll need to setup a conda environment
-        (after `installing conda, if necessary <https://docs.conda.io/projects/conda/en/latest/user-guide/install/>`_)
-        and install ``pymc``.  Then you can install ``dismod_mr`` using ``pip``.
-        
-        .. code-block:: sh
-        
-           conda create --name=dismod_mr python=3.6 pymc
-           conda activate dismod_mr
-           pip install dismod_mr
-        
-        If you get an error stating
-        
-        .. code-block:: sh
-        
-           ERROR: Complete output from command python setup.py egg_info:
-           ERROR: Traceback (most recent call last):
-             File "<string>", line 1, in <module>
-             File "/tmp/pip-install-d9fbq7v3/pymc/setup.py", line 8, in <module>
-               from numpy.distutils.misc_util import Configuration
-           ModuleNotFoundError: No module named 'numpy'
-           ----------------------------------------
-           ERROR: Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-install-d9fbq7v3/pymc/
-        
-        or something similar, you do not have ``pymc`` properly installed.
-        
-        
-        Installing from source
-        ++++++++++++++++++++++
-        
-        If you want to install ``dismod_mr`` locally in an editable mode, the
-        instructions are very similar.  We'll clone the repository and install it
-        from a local directory instead of using ``pip`` to grab it from the Python
-        package index.
-        
-        .. code-block:: sh
-        
-           conda create --name=dismod_mr python=3.6 pymc
-           conda activate dismod_mr
-           git clone git@github.com:ihmeuw/dismod_mr.git
-           cd dismod_mr
-           pip install -e .
-        
-        Coding Practices
-        ----------------
-        
-        * Write tests before code
-        * Write equations before tests
-        
-        * Test quantitatively with simulation data
-        * Test qualitatively with real data
-        * Automate tests
-        
-        * Use a package instead of DIY
-        * Test the package
-        
-        * Optimize code later
-        * Optimize code for readability before speed
-        
-        * `.py` files should be short, less than 500 lines
-        * Functions should be short, less than 25 lines
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -109,7 +20,103 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ihmeuw/dismod_mr.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/dismod_mr
+    :alt: Latest Version
+
+This project is the descriptive epidemiological meta-regression tool,
+DisMod-MR, which grew out of the Global Burden of Disease (GBD) Study
+2010.  DisMod-MR has been developed for the Institute of Health
+Metrics and Evaluation at the University of Washington from 2008-2013.
+
+.. contents::
+
+Examples
+--------
+
+`A motivating example: descriptive epidemiological meta-regression of Parkinson's Disease <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/blob/master/examples/pd_sim_data.ipynb>`_
+
+`All examples <http://nbviewer.ipython.org/github/ihmeuw/dismod_mr/tree/master/examples/>`_
+
+Installation
+------------
+
+Dismod MR requires PyMC2 which does not play nicely with normal Python
+installation tools.  Fortunately, ``conda`` has solved this issue for us.
+So first you'll need to setup a conda environment
+(after `installing conda, if necessary <https://docs.conda.io/projects/conda/en/latest/user-guide/install/>`_)
+and install ``pymc`` version ``2.3.8``.  Then you can install ``dismod_mr`` using ``pip``.
+
+.. code-block:: sh
+
+   conda create --name=dismod_mr python=3.6 pymc==2.3.8
+   conda activate dismod_mr
+   pip install dismod_mr
+
+If you get an error stating
+
+.. code-block:: sh
+
+   ERROR: Complete output from command python setup.py egg_info:
+   ERROR: Traceback (most recent call last):
+     File "<string>", line 1, in <module>
+     File "/tmp/pip-install-d9fbq7v3/pymc/setup.py", line 8, in <module>
+       from numpy.distutils.misc_util import Configuration
+   ModuleNotFoundError: No module named 'numpy'
+   ----------------------------------------
+   ERROR: Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-install-d9fbq7v3/pymc/
+
+or something similar, you do not have ``pymc`` properly installed.
+
+
+Installing from source
+++++++++++++++++++++++
+
+If you want to install ``dismod_mr`` locally in an editable mode, the
+instructions are very similar.  We'll clone the repository and install it
+from a local directory instead of using ``pip`` to grab it from the Python
+package index.
+
+.. code-block:: sh
+
+   conda create --name=dismod_mr python=3.6 pymc==2.3.8
+   conda activate dismod_mr
+   git clone git@github.com:ihmeuw/dismod_mr.git
+   cd dismod_mr
+   pip install -e .
+
+To test this, you can use ``pytest``, which you must first install.
+
+.. code-block:: sh
+
+   pip install pytest
+   pytest
+
+If you have things setup right, this will still generate many
+warnings, but there should be no tests that produce failures or
+errors.
+
+Coding Practices
+----------------
+
+* Write tests before code
+* Write equations before tests
+
+* Test quantitatively with simulation data
+* Test qualitatively with real data
+* Automate tests
+
+* Use a package instead of DIY
+* Test the package
+
+* Optimize code later
+* Optimize code for readability before speed
+
+* `.py` files should be short, less than 500 lines
+* Functions should be short, less than 25 lines
```

### Comparing `dismod_mr-1.1.1/src/dismod_mr.egg-info/SOURCES.txt` & `dismod_mr-1.1.2.7/src/dismod_mr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/LICENSE` & `dismod_mr-1.1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/README.rst` & `dismod_mr-1.1.2.7/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 .. image:: https://travis-ci.org/ihmeuw/dismod_mr.svg?branch=master
     :target: https://travis-ci.org/ihmeuw/dismod_mr
     :alt: Latest Version
 
-============
-Introduction
-============
-
 This project is the descriptive epidemiological meta-regression tool,
 DisMod-MR, which grew out of the Global Burden of Disease (GBD) Study
 2010.  DisMod-MR has been developed for the Institute of Health
 Metrics and Evaluation at the University of Washington from 2008-2013.
 
 .. contents::
 
@@ -23,19 +19,19 @@
 Installation
 ------------
 
 Dismod MR requires PyMC2 which does not play nicely with normal Python
 installation tools.  Fortunately, ``conda`` has solved this issue for us.
 So first you'll need to setup a conda environment
 (after `installing conda, if necessary <https://docs.conda.io/projects/conda/en/latest/user-guide/install/>`_)
-and install ``pymc``.  Then you can install ``dismod_mr`` using ``pip``.
+and install ``pymc`` version ``2.3.8``.  Then you can install ``dismod_mr`` using ``pip``.
 
 .. code-block:: sh
 
-   conda create --name=dismod_mr python=3.6 pymc
+   conda create --name=dismod_mr python=3.6 pymc==2.3.8
    conda activate dismod_mr
    pip install dismod_mr
 
 If you get an error stating
 
 .. code-block:: sh
 
@@ -57,20 +53,31 @@
 If you want to install ``dismod_mr`` locally in an editable mode, the
 instructions are very similar.  We'll clone the repository and install it
 from a local directory instead of using ``pip`` to grab it from the Python
 package index.
 
 .. code-block:: sh
 
-   conda create --name=dismod_mr python=3.6 pymc
+   conda create --name=dismod_mr python=3.6 pymc==2.3.8
    conda activate dismod_mr
    git clone git@github.com:ihmeuw/dismod_mr.git
    cd dismod_mr
    pip install -e .
 
+To test this, you can use ``pytest``, which you must first install.
+
+.. code-block:: sh
+
+   pip install pytest
+   pytest
+
+If you have things setup right, this will still generate many
+warnings, but there should be no tests that produce failures or
+errors.
+
 Coding Practices
 ----------------
 
 * Write tests before code
 * Write equations before tests
 
 * Test quantitatively with simulation data
```

### Comparing `dismod_mr-1.1.1/setup.py` & `dismod_mr-1.1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
     with open(os.path.join(base_dir, "README.rst")) as f:
         long_description = f.read()
 
     install_requirements = [
         'numpy>=1.7.1',
         'scipy>=0.12.0',
-        'pymc>=2.3.6',
+        'pymc==2.3.8',
         'networkx==2.3',
-        'pandas>=0.23.4',
-        'numba>=0.44.0',
-        'matplotlib',
+        'pandas>=0.23.4,<1.1',
+        'numba==0.51.0',
+        'matplotlib<3.3',
     ]
 
     setup(
         name=about['__title__'],
         version=about['__version__'],
 
         description=about['__summary__'],
```

### Comparing `dismod_mr-1.1.1/tests/test_covariates.py` & `dismod_mr-1.1.2.7/tests/test_covariates.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_data.py` & `dismod_mr-1.1.2.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_model_likelihood.py` & `dismod_mr-1.1.2.7/tests/test_model_likelihood.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_fit.py` & `dismod_mr-1.1.2.7/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_spline.py` & `dismod_mr-1.1.2.7/tests/test_spline.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_model_setup.py` & `dismod_mr-1.1.2.7/tests/test_model_setup.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_priors.py` & `dismod_mr-1.1.2.7/tests/test_priors.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_process.py` & `dismod_mr-1.1.2.7/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `dismod_mr-1.1.1/tests/test_age_groups.py` & `dismod_mr-1.1.2.7/tests/test_age_groups.py`

 * *Files identical despite different names*

