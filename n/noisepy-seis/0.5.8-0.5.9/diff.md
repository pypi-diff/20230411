# Comparing `tmp/noisepy_seis-0.5.8.tar.gz` & `tmp/noisepy_seis-0.5.9.tar.gz`

## Comparing `noisepy_seis-0.5.8.tar` & `noisepy_seis-0.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112593 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35203 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/LICENSE
--rw-r--r--   0        0        0    13682 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/README.md
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/pyproject.toml
--rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112593 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35203 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/LICENSE
+-rw-r--r--   0        0        0    13682 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/README.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 noisepy_seis-0.5.9/PKG-INFO
```

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.5.9/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.5.9/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.5.9/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.5.9/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/__init__.py` & `noisepy_seis-0.5.9/src/noisepy/seis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # no-qa F401
 from .S0A_download_ASDF_MPI import download  # noqa: F401
 from .S1_fft_cc_MPI import cross_correlate  # noqa: F401
 from .S2_stacking import stack  # noqa: F401
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 """
 NoisePy is a Python package designed for fast and easy computation of ambient noise cross-correlation functions.
 It provides additional functionality for noise monitoring and surface wave dispersion analysis.
 
 The main functions exported by the package are:
 - download:         download continous noise data based on obspy's core functions of
                     https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html and
```

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/main.py` & `noisepy_seis-0.5.9/src/noisepy/seis/main.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.5.9/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.5.9/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.5.9/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.5.9/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.5.9/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.5.9/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/LICENSE` & `noisepy_seis-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/README.md` & `noisepy_seis-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/pyproject.toml` & `noisepy_seis-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.8/PKG-INFO` & `noisepy_seis-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.5.8
+Version: 0.5.9
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@fas.harvard.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
```

