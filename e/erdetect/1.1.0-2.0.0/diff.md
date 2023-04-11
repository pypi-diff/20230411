# Comparing `tmp/erdetect-1.1.0.tar.gz` & `tmp/erdetect-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdetect-1.1.0.tar", last modified: Fri Nov 11 03:08:35 2022, max compression
+gzip compressed data, was "erdetect-2.0.0.tar", last modified: Tue Apr 11 21:27:05 2023, max compression
```

## Comparing `erdetect-1.1.0.tar` & `erdetect-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-11-11 03:08:35.227782 erdetect-1.1.0/
--rw-rw-rw-   0        0        0    35823 2022-01-28 21:02:26.000000 erdetect-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4965 2022-11-11 03:08:35.227782 erdetect-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3827 2022-11-11 02:53:59.000000 erdetect-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-11 03:08:35.196582 erdetect-1.1.0/erdetect/
--rw-rw-rw-   0        0        0      506 2022-11-11 03:06:45.000000 erdetect-1.1.0/erdetect/__init__.py
--rw-rw-rw-   0        0        0     1318 2022-09-14 18:21:38.000000 erdetect-1.1.0/erdetect/__main__.py
--rw-rw-rw-   0        0        0    44690 2022-11-11 02:30:48.000000 erdetect-1.1.0/erdetect/_erdetect.py
-drwxrwxrwx   0        0        0        0 2022-11-11 03:08:35.212182 erdetect-1.1.0/erdetect/core/
--rw-rw-rw-   0        0        0       12 2022-09-13 21:51:22.000000 erdetect-1.1.0/erdetect/core/__init__.py
--rw-rw-rw-   0        0        0    43840 2022-11-11 02:36:25.000000 erdetect-1.1.0/erdetect/core/config.py
--rw-rw-rw-   0        0        0    13275 2022-05-02 00:57:36.000000 erdetect-1.1.0/erdetect/core/detection.py
-drwxrwxrwx   0        0        0        0 2022-11-11 03:08:35.212182 erdetect-1.1.0/erdetect/core/metrics/
--rw-rw-rw-   0        0        0     3154 2022-09-13 21:38:32.000000 erdetect-1.1.0/erdetect/core/metrics/metric_cross_proj.py
--rw-rw-rw-   0        0        0     3790 2022-09-13 21:38:26.000000 erdetect-1.1.0/erdetect/core/metrics/metric_waveform.py
--rw-rw-rw-   0        0        0     8720 2022-04-25 16:28:07.000000 erdetect-1.1.0/erdetect/core/peak_finder.py
--rw-rw-rw-   0        0        0    27691 2022-11-11 02:35:28.000000 erdetect-1.1.0/erdetect/main_cli.py
-drwxrwxrwx   0        0        0        0 2022-11-11 03:08:35.227782 erdetect-1.1.0/erdetect/utils/
--rw-rw-rw-   0        0        0    13491 2022-04-29 22:11:32.000000 erdetect-1.1.0/erdetect/utils/IeegDataReader.py
--rw-rw-rw-   0        0        0       12 2022-09-13 18:54:10.000000 erdetect-1.1.0/erdetect/utils/__init__.py
--rw-rw-rw-   0        0        0   118009 2022-11-11 02:38:29.000000 erdetect-1.1.0/erdetect/utils/bids.py
--rw-rw-rw-   0        0        0    10610 2022-09-13 22:20:03.000000 erdetect-1.1.0/erdetect/utils/misc.py
--rw-rw-rw-   0        0        0       23 2022-11-11 02:44:13.000000 erdetect-1.1.0/erdetect/version.py
-drwxrwxrwx   0        0        0        0 2022-11-11 03:08:35.227782 erdetect-1.1.0/erdetect/views/
--rw-rw-rw-   0        0        0       12 2022-09-13 22:46:32.000000 erdetect-1.1.0/erdetect/views/__init__.py
--rw-rw-rw-   0        0        0     7934 2022-04-29 22:11:18.000000 erdetect-1.1.0/erdetect/views/output_images.py
-drwxrwxrwx   0        0        0        0 2022-11-11 03:08:35.196582 erdetect-1.1.0/erdetect.egg-info/
--rw-rw-rw-   0        0        0     4965 2022-11-11 03:08:35.000000 erdetect-1.1.0/erdetect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2022-11-11 03:08:35.000000 erdetect-1.1.0/erdetect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-11 03:08:35.000000 erdetect-1.1.0/erdetect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2022-11-11 03:08:35.000000 erdetect-1.1.0/erdetect.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-11 03:08:35.000000 erdetect-1.1.0/erdetect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1300 2022-11-11 03:07:08.000000 erdetect-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      252 2022-11-11 03:08:35.227782 erdetect-1.1.0/setup.cfg
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.393794 erdetect-2.0.0/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35823 2022-01-28 21:02:26.000000 erdetect-2.0.0/LICENSE
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-04-11 21:27:05.393972 erdetect-2.0.0/PKG-INFO
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3745 2023-04-11 19:56:10.000000 erdetect-2.0.0/README.md
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.290667 erdetect-2.0.0/erdetect/
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      592 2023-04-11 19:55:20.000000 erdetect-2.0.0/erdetect/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1318 2022-09-14 18:21:38.000000 erdetect-2.0.0/erdetect/__main__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46087 2023-04-11 20:29:06.000000 erdetect-2.0.0/erdetect/_erdetect.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.324763 erdetect-2.0.0/erdetect/core/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.0.0/erdetect/core/__init__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    43840 2022-11-11 02:45:10.000000 erdetect-2.0.0/erdetect/core/config.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    13275 2022-09-13 16:33:39.000000 erdetect-2.0.0/erdetect/core/detection.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.338553 erdetect-2.0.0/erdetect/core/metrics/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3088 2022-09-13 23:06:23.000000 erdetect-2.0.0/erdetect/core/metrics/metric_cross_proj.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3706 2022-09-13 23:06:25.000000 erdetect-2.0.0/erdetect/core/metrics/metric_waveform.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     8720 2022-09-13 16:33:39.000000 erdetect-2.0.0/erdetect/core/peak_finder.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    28038 2023-04-11 20:29:20.000000 erdetect-2.0.0/erdetect/main_cli.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.351941 erdetect-2.0.0/erdetect/utils/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.0.0/erdetect/utils/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4002 2023-04-11 17:56:08.000000 erdetect-2.0.0/erdetect/utils/misc.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-04-11 16:50:27.000000 erdetect-2.0.0/erdetect/version.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.392319 erdetect-2.0.0/erdetect/views/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:17.000000 erdetect-2.0.0/erdetect/views/__init__.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7934 2022-09-13 16:33:39.000000 erdetect-2.0.0/erdetect/views/output_images.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-04-11 21:27:05.296405 erdetect-2.0.0/erdetect.egg-info/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/PKG-INFO
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      605 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       83 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/requires.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-04-11 21:27:05.000000 erdetect-2.0.0/erdetect.egg-info/top_level.txt
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1412 2023-04-11 19:58:59.000000 erdetect-2.0.0/pyproject.toml
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      192 2023-04-11 21:27:05.399132 erdetect-2.0.0/setup.cfg
```

### Comparing `erdetect-1.1.0/LICENSE` & `erdetect-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erdetect-1.1.0/PKG-INFO` & `erdetect-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,131 @@
-Metadata-Version: 2.1
-Name: erdetect
-Version: 1.1.0
-Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
-Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
-License: GPLv3
-Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
-Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
-Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
-Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Evoked Response Detection
-A python package and docker application for the automatic detection of evoked responses in SPES/CCEP data
-
-## Docker Usage
-
-To launch an instance of the container and analyse data in BIDS format, type:
-
-```
-$ docker run multimodalneuro/n1detect <bids_dir> <output_dir> [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
-```
-For example, to run an analysis, type:
-
-```
-docker run -ti --rm \
--v /local_bids_data_root/:/data \
--v /local_output_path/:/output \
-multimodalneuro/erdetect /data /output --participant_label 01 --skip_bids_validator
-```
-
-
-## Python Usage
-
-1. First install ERdetect, in the command-line run:
-```
-pip install erdetect
-```
-
-2. To run:
-- a) From the commandline:
-```
-python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
-```
-
-- b) A subset of the data directly in a python script:
-```
-import erdetect
-erdetect.process('/bids_data_root/bids_subj/ieeg/data_file', '/output_path/')
-```
-
-
-
-## Configure detection
-From the command-line, a JSON file can be passed using the ```--config_filepath [JSON_FILEPATH]``` parameter to adjust the preprocessing, the evoked response detection and the visualization settings.
-An example JSON containing the standard settings looks as follows:
-```
-{
-    "preprocess": {
-        "high_pass":                        false,
-        "line_noise_removal":               "off",
-        "early_re_referencing": {
-            "enabled":                      false,
-            "method":                       "CAR",
-            "stim_excl_epoch":              [-1.0,        2.0]
-        }
-    },
-	
-    "trials": {
-        "trial_epoch":                      [-1.0,        2.0],
-        "out_of_bounds_handling":           "first_last_only",
-        "baseline_epoch":                   [-0.5,      -0.02],
-        "baseline_norm":                    "median",
-        "concat_bidirectional_pairs":       true,
-        "minimum_stimpair_trials":          5
-    },
-
-    "channels": {
-        "measured_types":                   ["ECOG", "SEEG", "DBS"],
-        "stim_types":                       ["ECOG", "SEEG", "DBS"]
-    },
-
-    "detection": {
-        "negative":                         true,
-        "positive":                         false,
-        "peak_search_epoch":                [ 0,          0.5],
-        "response_search_epoch":            [ 0.009,     0.09],
-        "method":                           "std_base",
-        "std_base": {
-            "baseline_epoch":               [-1,         -0.1],
-            "baseline_threshold_factor":    3.4
-        }
-    },
-
-    "visualization": {
-        "negative":                         true,
-        "positive":                         false,
-        "x_axis_epoch":                     [-0.2,          1],
-        "blank_stim_epoch":                 [-0.015,   0.0025],
-        "generate_electrode_images":        true,
-        "generate_stimpair_images":         true,
-        "generate_matrix_images":           true
-    }
-}
-```
-
-
-## Acknowledgements
-
-- Written by Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
-- Local extremum detection method by Dorien van Blooijs & Dora Hermes (2018), with optimized parameters by Jaap van der Aar
-- Dependencies:
-  - PyMef by Jan Cimbalnik, Matt Stead, Ben Brinkmann, and Dan Crepeau (https://github.com/msel-source/pymef)
-  - MNE-Python (https://mne.tools/)
-  - BIDS-validator (https://github.com/bids-standard/bids-validator)
-  - NumPy
-  - SciPy
-  - Pandas
-  - KiwiSolver
-  - Matplotlib
-  - psutil
-
-- This project was funded by the National Institute Of Mental Health of the National Institutes of Health Award Number R01MH122258 to Dora Hermes
+Metadata-Version: 2.1
+Name: erdetect
+Version: 2.0.0
+Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
+Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
+License: GPLv3
+Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
+Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
+Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
+Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Evoked Response Detection
+A python package and docker application for the automatic detection of evoked responses in SPES/CCEP data
+
+## Docker Usage
+
+To launch an instance of the container and analyse data in BIDS format, in the command-line interface/terminal:
+
+```
+docker run multimodalneuro/erdetect <bids_dir>:/data <output_dir>:/output [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
+```
+For example, to run an analysis, type:
+
+```
+docker run -ti --rm \
+-v /local_bids_data_root/:/data \
+-v /local_output_path/:/output \
+multimodalneuro/erdetect /data /output --participant_label 01
+```
+
+
+## Python Usage
+
+1. First install ERdetect, in the command-line run:
+```
+pip install erdetect
+```
+
+2. To run:
+- a) From the commandline:
+```
+python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
+```
+
+- b) To process a subset directly in a python script:
+```
+import erdetect
+erdetect.process_subset('/bids_data_root/subj-01/ieeg/sub-01_run-06.edf', '/output_path/')
+```
+
+
+
+## Configure detection
+From the command-line, a JSON file can be passed using the ```--config_filepath [JSON_FILEPATH]``` parameter to adjust the preprocessing, the evoked response detection and the visualization settings.
+An example JSON containing the standard settings looks as follows:
+```
+{
+    "preprocess": {
+        "high_pass":                        false,
+        "line_noise_removal":               "off",
+        "early_re_referencing": {
+            "enabled":                      false,
+            "method":                       "CAR",
+            "stim_excl_epoch":              [-1.0,        2.0]
+        }
+    },
+	
+    "trials": {
+        "trial_epoch":                      [-1.0,        2.0],
+        "out_of_bounds_handling":           "first_last_only",
+        "baseline_epoch":                   [-0.5,      -0.02],
+        "baseline_norm":                    "median",
+        "concat_bidirectional_pairs":       true,
+        "minimum_stimpair_trials":          5
+    },
+
+    "channels": {
+        "measured_types":                   ["ECOG", "SEEG", "DBS"],
+        "stim_types":                       ["ECOG", "SEEG", "DBS"]
+    },
+
+    "detection": {
+        "negative":                         true,
+        "positive":                         false,
+        "peak_search_epoch":                [ 0,          0.5],
+        "response_search_epoch":            [ 0.009,     0.09],
+        "method":                           "std_base",
+        "std_base": {
+            "baseline_epoch":               [-1,         -0.1],
+            "baseline_threshold_factor":    3.4
+        }
+    },
+
+    "visualization": {
+        "negative":                         true,
+        "positive":                         false,
+        "x_axis_epoch":                     [-0.2,          1],
+        "blank_stim_epoch":                 [-0.015,   0.0025],
+        "generate_electrode_images":        true,
+        "generate_stimpair_images":         true,
+        "generate_matrix_images":           true
+    }
+}
+```
+
+
+## Acknowledgements
+
+- Written by Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
+- Local extremum detection method by Dorien van Blooijs & Dora Hermes (2018), with optimized parameters by Jaap van der Aar
+- Dependencies:
+  - IeegPrep (https://github.com/MultimodalNeuroimagingLab/ieegprep)
+  - BIDS-validator (https://github.com/bids-standard/bids-validator)
+  - NumPy
+  - SciPy
+  - Matplotlib
+
+- This project was funded by the National Institute Of Mental Health of the National Institutes of Health Award Number R01MH122258 to Dora Hermes
```

### Comparing `erdetect-1.1.0/README.md` & `erdetect-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Evoked Response Detection
 A python package and docker application for the automatic detection of evoked responses in SPES/CCEP data
 
 ## Docker Usage
 
-To launch an instance of the container and analyse data in BIDS format, type:
+To launch an instance of the container and analyse data in BIDS format, in the command-line interface/terminal:
 
 ```
-$ docker run multimodalneuro/n1detect <bids_dir> <output_dir> [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
+docker run multimodalneuro/erdetect <bids_dir>:/data <output_dir>:/output [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
 ```
 For example, to run an analysis, type:
 
 ```
 docker run -ti --rm \
 -v /local_bids_data_root/:/data \
 -v /local_output_path/:/output \
-multimodalneuro/erdetect /data /output --participant_label 01 --skip_bids_validator
+multimodalneuro/erdetect /data /output --participant_label 01
 ```
 
 
 ## Python Usage
 
 1. First install ERdetect, in the command-line run:
 ```
@@ -27,18 +27,18 @@
 
 2. To run:
 - a) From the commandline:
 ```
 python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
 ```
 
-- b) A subset of the data directly in a python script:
+- b) To process a subset directly in a python script:
 ```
 import erdetect
-erdetect.process('/bids_data_root/bids_subj/ieeg/data_file', '/output_path/')
+erdetect.process_subset('/bids_data_root/subj-01/ieeg/sub-01_run-06.edf', '/output_path/')
 ```
 
 
 
 ## Configure detection
 From the command-line, a JSON file can be passed using the ```--config_filepath [JSON_FILEPATH]``` parameter to adjust the preprocessing, the evoked response detection and the visualization settings.
 An example JSON containing the standard settings looks as follows:
@@ -94,18 +94,14 @@
 
 
 ## Acknowledgements
 
 - Written by Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
 - Local extremum detection method by Dorien van Blooijs & Dora Hermes (2018), with optimized parameters by Jaap van der Aar
 - Dependencies:
-  - PyMef by Jan Cimbalnik, Matt Stead, Ben Brinkmann, and Dan Crepeau (https://github.com/msel-source/pymef)
-  - MNE-Python (https://mne.tools/)
+  - IeegPrep (https://github.com/MultimodalNeuroimagingLab/ieegprep)
   - BIDS-validator (https://github.com/bids-standard/bids-validator)
   - NumPy
   - SciPy
-  - Pandas
-  - KiwiSolver
   - Matplotlib
-  - psutil
 
 - This project was funded by the National Institute Of Mental Health of the National Institutes of Health Award Number R01MH122258 to Dora Hermes
```

### Comparing `erdetect-1.1.0/erdetect/__main__.py` & `erdetect-2.0.0/erdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `erdetect-1.1.0/erdetect/_erdetect.py` & `erdetect-2.0.0/erdetect/_erdetect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,71 @@
+"""
+Evoked response detection - Processing functions
+=====================================================
+
+
+Copyright 2022, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
+
+This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
+as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
+warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import os
 import logging
 from math import isnan, ceil
 import numpy as np
 import scipy.io as sio
 from os.path import exists
 
+from ieegprep.bids import load_channel_info, load_event_info, load_ieeg_sidecar
+from ieegprep.bids.data_epoch import load_data_epochs_averages
+from ieegprep.bids.rereferencing import RerefStruct
+from ieegprep.utils.console import multi_line_list, print_progressbar
+from ieegprep.utils.misc import is_number
+
 from erdetect.core.config import write_config, get as cfg, get_config_dict, OUTPUT_IMAGE_SIZE, LOGGING_CAPTION_INDENT_LENGTH
 from erdetect.core.detection import ieeg_detect_er
 from erdetect.views.output_images import calc_sizes_and_fonts, calc_matrix_image_size, gen_amplitude_matrix, gen_latency_matrix
-from erdetect.utils.bids import load_channel_info, load_event_info, load_ieeg_sidecar, load_data_epochs_averages, RerefStruct
-from erdetect.utils.misc import print_progressbar, is_number, multi_line_list, create_figure
+from erdetect.utils.misc import create_figure
 from erdetect.core.metrics.metric_cross_proj import metric_cross_proj
 from erdetect.core.metrics.metric_waveform import metric_waveform
 
 
-def process(bids_subset_data_path, output_dir, preproc_prioritize_speed=False):
+def process_subset(bids_subset_data_path, output_dir, preproc_prioritize_speed=False):
     """
     Process a BIDS subset, perform pre-processing, evoked response detection and produce output
 
     Args:
         bids_subset_data_path (str):          The path to the data of a subset (e.g. /BIDS/sub-01/ses-ieeg01/ieeg/sub-01_task-ccep.mefd)
                                               Paths other required files such as the _channels.tsv and _events.tsv file
                                               will be derived from the data path.
         output_dir (str):                     The path to store the output files in. A subdirectory will be created for each subset.
         preproc_prioritize_speed (bool):      Set the pre-processing priority to either memory (default, False) or speed (True).
 
     """
 
     # check the input arguments
     if not bids_subset_data_path:
-        logging.error('Empty or invalid input data path, exiting...')
+        logging.error('Empty or invalid input data path, make sure to provide a path to subset data (e.g. \'/bids_data_root/subj-01/ieeg/sub-01_run-06.edf\'), exiting...')
         return
     if not exists(bids_subset_data_path):
-        logging.error('Input data path (\'' + bids_subset_data_path +'\') could not be found, exiting...')
+        logging.error('Input data path (\'' + bids_subset_data_path + '\') could not be found.\nMake sure to provide a path to subset data (e.g. \'/bids_data_root/subj-01/ieeg/sub-01_run-06.edf\'), exiting...')
         return
     if not output_dir:
         logging.error('Empty or invalid output directory, exiting...')
         return
 
     # derive the bids subset root from the full path
-    bids_subset_root = bids_subset_data_path[:bids_subset_data_path.rindex('_')]
+    try:
+        bids_subset_root = bids_subset_data_path[:bids_subset_data_path.rindex('_')]
+    except ValueError:
+        logging.error('Invalid input data path, make sure to provide a path to subset data (e.g. \'/bids_data_root/subj-01/ieeg/sub-01_run-06.edf\'), exiting...')
+        return
 
     # determine a subset specific output path
     output_root = os.path.join(output_dir, os.path.basename(os.path.normpath(bids_subset_root)))
 
     # print subset information
     logging.info('------------------------ Processing subset ------------------------')
     log_indented_line('Subset input:', bids_subset_root + '.*')
@@ -140,15 +162,15 @@
 
         # determine if included or excluded from early re-referencing electrodes (by type)
         if cfg('preprocess', 'early_re_referencing', 'enabled'):
             if row['type'].upper() in cfg('preprocess', 'early_re_referencing', 'channel_types'):
 
                 # save for log output and the early-referencing (structure)
                 channels_early_reref_incl_names.append(row['name'])
-                if channels_have_status:
+                if channels_have_headbox:
                     channels_early_reref_incl_headbox.append(row['headbox'])
 
                 # save for data reading (no duplicates)
                 if not row['name'] in channels_incl:
                     channels_incl.append(row['name'])
 
             else:
@@ -156,38 +178,38 @@
 
         # determine if included or excluded from late re-referencing electrodes (by type)
         if cfg('preprocess', 'late_re_referencing', 'enabled'):
             if row['type'].upper() in cfg('preprocess', 'late_re_referencing', 'channel_types'):
 
                 # save for log output and the late-referencing (structure)
                 channels_late_reref_incl_names.append(row['name'])
-                if channels_have_status:
+                if channels_have_headbox:
                     channels_late_reref_incl_headbox.append(row['headbox'])
                     # TODO: what if nan or not a number
 
                 # save for data reading (no duplicates)
                 if not row['name'] in channels_incl:
                     channels_incl.append(row['name'])
 
             else:
                 channels_late_reref_excl_by_type.append(row['name'])   # save for log output
 
     # print channel information
-    logging.info(multi_line_list(channels_excl_bad, LOGGING_CAPTION_INDENT_LENGTH, 'Bad channels (excluded):', 25, ' '))
+    logging.info(multi_line_list(channels_excl_bad, LOGGING_CAPTION_INDENT_LENGTH, 'Bad channels (excluded):', 14, ' '))
     if channels_measured_excl_by_type == channels_stim_excl_by_type:
-        logging.info(multi_line_list(channels_measured_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excluded by type:', 25, ' '))
+        logging.info(multi_line_list(channels_measured_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excluded by type:', 14, ' '))
     else:
-        logging.info(multi_line_list(channels_measured_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excl. (by type) as measured electrodes:', 25, ' '))
-        logging.info(multi_line_list(channels_stim_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excl. (by type) as stim electrodes:', 25, ' '))
+        logging.info(multi_line_list(channels_measured_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excl. (by type) as measured electrodes:', 14, ' '))
+        logging.info(multi_line_list(channels_stim_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excl. (by type) as stim electrodes:', 14, ' '))
     logging.info('')
     if channels_measured_incl == channels_stim_incl:
-        logging.info(multi_line_list(channels_measured_incl, LOGGING_CAPTION_INDENT_LENGTH, 'Channels included as electrodes:', 25, ' ', str(len(channels_measured_incl))))
+        logging.info(multi_line_list(channels_measured_incl, LOGGING_CAPTION_INDENT_LENGTH, 'Channels included as electrodes:', 14, ' ', str(len(channels_measured_incl))))
     else:
-        logging.info(multi_line_list(channels_measured_incl, LOGGING_CAPTION_INDENT_LENGTH, 'Channels incl. as measured electrodes:', 25, ' ', str(len(channels_measured_incl))))
-        logging.info(multi_line_list(channels_stim_incl, LOGGING_CAPTION_INDENT_LENGTH, 'Channels incl. as stim electrodes:', 25, ' ', str(len(channels_stim_incl))))
+        logging.info(multi_line_list(channels_measured_incl, LOGGING_CAPTION_INDENT_LENGTH, 'Channels incl. as measured electrodes:', 14, ' ', str(len(channels_measured_incl))))
+        logging.info(multi_line_list(channels_stim_incl, LOGGING_CAPTION_INDENT_LENGTH, 'Channels incl. as stim electrodes:', 14, ' ', str(len(channels_stim_incl))))
 
 
     # check if there are any channels (as measured electrodes, or to re-reference on)
     if len(channels_measured_incl) == 0:
         logging.error('No channels were found (after filtering by type), exiting...')
         raise RuntimeError('No channels were found')
 
@@ -196,30 +218,30 @@
     if cfg('preprocess', 'early_re_referencing', 'enabled'):
 
         if cfg('preprocess', 'early_re_referencing', 'method') == 'CAR_headbox' and not channels_have_headbox:
             logging.error('Early re-referencing is set to CAR per headbox, but the _channels.tsv file does not have a \'headbox\' column, exiting...')
             raise RuntimeError('No \'headbox\' column in _channels.tsv file, needed to perform early re-referencing per headbox')
 
         if len(channels_early_reref_incl_names) == 0:
-            logging.info(multi_line_list(channels_early_reref_incl_names, LOGGING_CAPTION_INDENT_LENGTH, 'Channels included (by type) for early re-ref:', 25, ' '))
-            logging.info(multi_line_list(channels_early_reref_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excluded by type for early re-ref:', 25, ' '))
+            logging.info(multi_line_list(channels_early_reref_incl_names, LOGGING_CAPTION_INDENT_LENGTH, 'Channels included (by type) for early re-ref:', 14, ' '))
+            logging.info(multi_line_list(channels_early_reref_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excluded by type for early re-ref:', 14, ' '))
             logging.error('Early re-referencing is enabled but (after filtering by type) no channels were found, exiting...')
             raise RuntimeError('No channels were found for early re-referencing')
 
         # generate an early re-referencing object
         if cfg('preprocess', 'early_re_referencing', 'method') == 'CAR':
             early_reref = RerefStruct.generate_car(channels_early_reref_incl_names)
         elif cfg('preprocess', 'early_re_referencing', 'method') == 'CAR_headbox':
             early_reref = RerefStruct.generate_car_per_headbox(channels_early_reref_incl_names, channels_early_reref_incl_headbox)
 
             # print CAR headbox info
             logging.info('')
             log_indented_line('Early re-referencing groups:', '')
             for ind, group in enumerate(early_reref.groups):
-                logging.info(multi_line_list(group, LOGGING_CAPTION_INDENT_LENGTH, '      CAR group ' + str(ind) + ':', 25, ' '))
+                logging.info(multi_line_list(group, LOGGING_CAPTION_INDENT_LENGTH, '      CAR group ' + str(ind) + ':', 14, ' '))
 
             # check to make sure all included channels are also included in early re-referencing
             missing_channels = []
             for channel in channels_measured_incl:
                 if channel not in early_reref.channel_group.keys():
                     missing_channels.append(channel)
             if len(missing_channels) == 1:
@@ -235,45 +257,43 @@
     if cfg('preprocess', 'late_re_referencing', 'enabled'):
 
         if cfg('preprocess', 'late_re_referencing', 'method') == 'CAR_headbox' and not channels_have_headbox:
             logging.error('Late re-referencing is set to CAR per headbox, but the _channels.tsv file does not have a \'headbox\' column, exiting...')
             raise RuntimeError('No \'headbox\' column in _channels.tsv file, needed to perform late re-referencing per headbox')
 
         if len(channels_late_reref_incl_names) == 0:
-            logging.info(multi_line_list(channels_late_reref_incl_names, LOGGING_CAPTION_INDENT_LENGTH, 'Channels included (by type) for late re-ref:', 25, ' '))
-            logging.info(multi_line_list(channels_late_reref_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excluded by type for late re-ref:', 25, ' '))
+            logging.info(multi_line_list(channels_late_reref_incl_names, LOGGING_CAPTION_INDENT_LENGTH, 'Channels included (by type) for late re-ref:', 14, ' '))
+            logging.info(multi_line_list(channels_late_reref_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excluded by type for late re-ref:', 14, ' '))
             logging.error('Late re-referencing is enabled but (after filtering by type) no channels were found, exiting...')
             raise RuntimeError('No channels were found for late re-referencing')
 
         # generate a late re-referencing object
         if cfg('preprocess', 'late_re_referencing', 'method') == 'CAR':
             late_reref = RerefStruct.generate_car(channels_late_reref_incl_names)
         elif cfg('preprocess', 'late_re_referencing', 'method') == 'CAR_headbox':
             late_reref = RerefStruct.generate_car_per_headbox(channels_late_reref_incl_names, channels_late_reref_incl_headbox)
 
             # print CAR headbox info
             logging.info('')
             log_indented_line('Late re-referencing groups:', '')
             for ind, group in enumerate(late_reref.groups):
-                logging.info(multi_line_list(group, LOGGING_CAPTION_INDENT_LENGTH, '      CAR group ' + str(ind) + ':', 25, ' '))
+                logging.info(multi_line_list(group, LOGGING_CAPTION_INDENT_LENGTH, '      CAR group ' + str(ind) + ':', 14, ' '))
 
             # check to make sure all included channels are also included in late re-referencing
             missing_channels = []
             for channel in channels_measured_incl:
                 if channel not in late_reref.channel_group.keys():
                     missing_channels.append(channel)
             if len(missing_channels) == 1:
                 logging.error('Channel \'' + missing_channels[0] + '\' is included but cannot be found in any late re-referencing group, make sure the channel has a valid headbox value in the _channels.tsv')
                 raise RuntimeError('Included channel not in re-referencing group')
             elif len(missing_channels) > 1:
                 logging.error('Channels \'' + ', '.join(missing_channels) + '\' are included but cannot be found in any late re-referencing group, make sure the channels have valid headbox values in the _channels.tsv')
                 raise RuntimeError('Included channel not in re-referencing group')
 
-
-
     logging.info('')
 
 
 
     #
     # retrieve trials
     #
@@ -362,25 +382,25 @@
 
     # remove the stimulus-pairs with too little trials
     if len(stimpair_remove_indices) > 0:
 
         # message
         stimpair_print = [stim_pair + ' (' + str(len(stim_pairs_onsets[stim_pair])) + ' trials)' for stim_pair in stimpair_remove_indices]
         stimpair_print = [str_print.ljust(len(max(stimpair_print, key=len)), ' ') for str_print in stimpair_print]
-        logging.info(multi_line_list(stimpair_print, LOGGING_CAPTION_INDENT_LENGTH, 'Stim-pairs excluded by number of trials:', 4, '   '))
+        logging.info(multi_line_list(stimpair_print, LOGGING_CAPTION_INDENT_LENGTH, 'Stim-pairs excluded by number of trials:', 3, '   '))
 
         # remove those stimulation-pairs
         for stim_pair in stimpair_remove_indices:
             del stim_pairs_onsets[stim_pair]
             del stim_pairs_electrode_names[stim_pair]
 
     # display stimulation-pair/trial information
     stimpair_print = [stim_pair + ' (' + str(len(onsets)) + ' trials)' for stim_pair, onsets in stim_pairs_onsets.items()]
     stimpair_print = [str_print.ljust(len(max(stimpair_print, key=len)), ' ') for str_print in stimpair_print]
-    logging.info(multi_line_list(stimpair_print, LOGGING_CAPTION_INDENT_LENGTH, 'Stimulation pairs included:', 4, '   ', str(len(stim_pairs_onsets))))
+    logging.info(multi_line_list(stimpair_print, LOGGING_CAPTION_INDENT_LENGTH, 'Stimulation pairs included:', 3, '   ', str(len(stim_pairs_onsets))))
 
     # check if there are stimulus-pairs
     if len(stim_pairs_onsets) == 0:
         logging.error('No stimulus-pairs were found, exiting...')
         raise RuntimeError('No stimulus-pairs found')
 
     # set the parts of stimulation (of specific channels) to exclude from early or late re-referencing
```

### Comparing `erdetect-1.1.0/erdetect/core/config.py` & `erdetect-2.0.0/erdetect/core/config.py`

 * *Files identical despite different names*

### Comparing `erdetect-1.1.0/erdetect/core/detection.py` & `erdetect-2.0.0/erdetect/core/detection.py`

 * *Files identical despite different names*

### Comparing `erdetect-1.1.0/erdetect/core/metrics/metric_cross_proj.py` & `erdetect-2.0.0/erdetect/core/metrics/metric_cross_proj.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""
-The cross projection metric
-
-Cross-projection concept adapted from: Dora Hermes and Kai Miller (check)
-
-Copyright 2022, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
-
-This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
-warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-import numpy as np
-from scipy import stats
-from ...core.config import get as config
-
-
-def metric_cross_proj(sampling_rate, data, baseline):
-    """
-    Calculate a cross-projection metric, called per (measurement) channel and per condition (=stim-pair)
-
-    Args:
-        sampling_rate (int):                  The sampling rate of the data
-        data (ndarray):                       2D data matrix (represented as trials x samples)
-        baseline (ndarray):                   2D baseline data matrix (represented as trials x samples)
-
-    Returns:
-        A single metric value
-    """
-
-    trial_epoch = config('trials', 'trial_epoch')
-    baseline_norm = config('trials', 'baseline_norm')
-    cross_proj_epoch = config('metrics', 'cross_proj', 'epoch')
-
-    # calculate the sample indices for the cross-projection epoch (relative to the trial epoch)
-    start_sample = round((cross_proj_epoch[0] - trial_epoch[0]) * sampling_rate)
-    end_sample = round((cross_proj_epoch[1] - trial_epoch[0]) * sampling_rate)
-
-    # extract the data to calculate the metric and normalize
-    if baseline_norm.lower() == 'mean' or baseline_norm.lower() == 'average':
-        metric_data = data[:, start_sample:end_sample] - np.nanmean(baseline, axis=1)[:, None]
-    elif baseline_norm.lower() == 'median':
-        metric_data = data[:, start_sample:end_sample] - np.nanmedian(baseline, axis=1)[:, None]
-    else:
-        #TODO:
-        pass
-    # TODO: check when no normalization to baseline, whether waveform method still works, or should give warning
-    # check if data by ref
-    # if config('trials', 'baseline_norm') == "None"
-
-
-    # normalize (L2 norm) each trial
-    norm_matrix = np.sqrt(np.power(metric_data, 2).sum(axis=1))
-    norm_matrix[norm_matrix == 0] = np.nan                          # prevent division by 0
-    norm_metric_data = metric_data / norm_matrix[:, None]
-
-    # calculate internal projections
-    proj = np.matmul(norm_metric_data, np.transpose(metric_data))
-
-    # perform a one-sample t-test on the values in the upper triangle of the matrix (above the diagonal)
-    test_values = proj[np.triu_indices(proj.shape[0], 1)]
-    test_result = stats.ttest_1samp(test_values, 0)
-
-    # return the t-statistic as the metric
-    return test_result.statistic
+"""
+The cross projection metric
+
+Cross-projection concept adapted from: Dora Hermes and Kai Miller (check)
+
+Copyright 2022, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
+
+This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
+as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
+warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+import numpy as np
+from scipy import stats
+from ...core.config import get as config
+
+
+def metric_cross_proj(sampling_rate, data, baseline):
+    """
+    Calculate a cross-projection metric, called per (measurement) channel and per condition (=stim-pair)
+
+    Args:
+        sampling_rate (int):                  The sampling rate of the data
+        data (ndarray):                       2D data matrix (represented as trials x samples)
+        baseline (ndarray):                   2D baseline data matrix (represented as trials x samples)
+
+    Returns:
+        A single metric value
+    """
+
+    trial_epoch = config('trials', 'trial_epoch')
+    baseline_norm = config('trials', 'baseline_norm')
+    cross_proj_epoch = config('metrics', 'cross_proj', 'epoch')
+
+    # calculate the sample indices for the cross-projection epoch (relative to the trial epoch)
+    start_sample = round((cross_proj_epoch[0] - trial_epoch[0]) * sampling_rate)
+    end_sample = round((cross_proj_epoch[1] - trial_epoch[0]) * sampling_rate)
+
+    # extract the data to calculate the metric and normalize
+    if baseline_norm.lower() == 'mean' or baseline_norm.lower() == 'average':
+        metric_data = data[:, start_sample:end_sample] - np.nanmean(baseline, axis=1)[:, None]
+    elif baseline_norm.lower() == 'median':
+        metric_data = data[:, start_sample:end_sample] - np.nanmedian(baseline, axis=1)[:, None]
+    else:
+        #TODO:
+        pass
+    # TODO: check when no normalization to baseline, whether waveform method still works, or should give warning
+    # check if data by ref
+    # if config('trials', 'baseline_norm') == "None"
+
+
+    # normalize (L2 norm) each trial
+    norm_matrix = np.sqrt(np.power(metric_data, 2).sum(axis=1))
+    norm_matrix[norm_matrix == 0] = np.nan                          # prevent division by 0
+    norm_metric_data = metric_data / norm_matrix[:, None]
+
+    # calculate internal projections
+    proj = np.matmul(norm_metric_data, np.transpose(metric_data))
+
+    # perform a one-sample t-test on the values in the upper triangle of the matrix (above the diagonal)
+    test_values = proj[np.triu_indices(proj.shape[0], 1)]
+    test_result = stats.ttest_1samp(test_values, 0)
+
+    # return the t-statistic as the metric
+    return test_result.statistic
```

### Comparing `erdetect-1.1.0/erdetect/core/metrics/metric_waveform.py` & `erdetect-2.0.0/erdetect/core/metrics/metric_waveform.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""
-The waveform metric
-
-Copyright 2022, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
-
-This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
-warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-import numpy as np
-from scipy import signal
-from ...core.config import get as config
-
-
-def metric_waveform(sampling_rate, data, baseline):
-    """
-    Calculate a waveform (10-30Hz) metric, called per (measurement) channel and per condition (=stim-pair)
-
-    Args:
-        sampling_rate (int):                  The sampling rate of the data
-        data (ndarray):                       2D data matrix (represented as trials x samples)
-        baseline (ndarray):                   2D baseline data matrix (represented as trials x samples)
-
-    Returns:
-        A single metric value
-    """
-
-    trial_epoch = config('trials', 'trial_epoch')
-    baseline_norm = config('trials', 'baseline_norm')
-    waveform_epoch = config('metrics', 'waveform', 'epoch')
-    bandpass = config('metrics', 'waveform', 'bandpass')
-
-    # calculate the sample indices for the waveform epoch (relative to the trial epoch)
-    start_sample = round((waveform_epoch[0] - trial_epoch[0]) * sampling_rate)
-    end_sample = round((waveform_epoch[1] - trial_epoch[0]) * sampling_rate)
-
-    # extract the data to calculate the metric and normalize
-    if baseline_norm.lower() == 'mean' or baseline_norm.lower() == 'average':
-        metric_data = data[:, start_sample:end_sample] - np.nanmean(baseline, axis=1)[:, None]
-    elif baseline_norm.lower() == 'median':
-        metric_data = data[:, start_sample:end_sample] - np.nanmedian(baseline, axis=1)[:, None]
-    else:
-        # TODO: check when no normalization to baseline, whether waveform method still works, or should give warning
-        return np.nan
-
-    # take the average over all trials
-    metric_data = np.nanmean(metric_data, axis=0)
-
-    # recenter the segment to 0
-    metric_data -= np.nanmean(metric_data)
-
-
-    #
-    # perform bandpass filtering using a butterworth filter
-    #
-
-    # third order Butterworth
-    Rp = 3
-    Rs = 60
-
-    #
-    delta = 0.001 * 2 / sampling_rate
-    low_p = bandpass[1] * 2 / sampling_rate
-    high_p = bandpass[0] * 2 / sampling_rate
-    high_s = max(delta, high_p - 0.1)
-    low_s = min(1 - delta, low_p + 0.1)
-
-    # Design a butterworth (band-pass) filter
-    # Note: the 'buttord' output here differs slight from matlab, because the scipy make a change in scipy 0.14.0 where
-    #       the choice of which end of the transition region was switched from the stop-band edge to the pass-band edge
-    n_band, wn_band = signal.buttord([high_p, low_p], [high_s, low_s], Rp, Rs, True)
-    bf_b, bf_a = signal.butter(n_band, wn_band, 'band', analog=False)
-
-    # Perform the band-passing
-    # Note: custom padlen to match the way matlab does it (-1 is omitted in scipy)
-    metric_data = signal.filtfilt(bf_b, bf_a, metric_data, padtype='odd', padlen=3 * (max(len(bf_b), len(bf_a)) - 1))
-
-    # calculate the band power using a hilbert transformation
-    band_power_sm = np.power(abs(signal.hilbert(metric_data)), 2)
-
-    # return the highest power value over time
-    return np.max(band_power_sm)
+"""
+The waveform metric
+
+Copyright 2022, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
+
+This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
+as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
+warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+import numpy as np
+from scipy import signal
+from ...core.config import get as config
+
+
+def metric_waveform(sampling_rate, data, baseline):
+    """
+    Calculate a waveform (10-30Hz) metric, called per (measurement) channel and per condition (=stim-pair)
+
+    Args:
+        sampling_rate (int):                  The sampling rate of the data
+        data (ndarray):                       2D data matrix (represented as trials x samples)
+        baseline (ndarray):                   2D baseline data matrix (represented as trials x samples)
+
+    Returns:
+        A single metric value
+    """
+
+    trial_epoch = config('trials', 'trial_epoch')
+    baseline_norm = config('trials', 'baseline_norm')
+    waveform_epoch = config('metrics', 'waveform', 'epoch')
+    bandpass = config('metrics', 'waveform', 'bandpass')
+
+    # calculate the sample indices for the waveform epoch (relative to the trial epoch)
+    start_sample = round((waveform_epoch[0] - trial_epoch[0]) * sampling_rate)
+    end_sample = round((waveform_epoch[1] - trial_epoch[0]) * sampling_rate)
+
+    # extract the data to calculate the metric and normalize
+    if baseline_norm.lower() == 'mean' or baseline_norm.lower() == 'average':
+        metric_data = data[:, start_sample:end_sample] - np.nanmean(baseline, axis=1)[:, None]
+    elif baseline_norm.lower() == 'median':
+        metric_data = data[:, start_sample:end_sample] - np.nanmedian(baseline, axis=1)[:, None]
+    else:
+        # TODO: check when no normalization to baseline, whether waveform method still works, or should give warning
+        return np.nan
+
+    # take the average over all trials
+    metric_data = np.nanmean(metric_data, axis=0)
+
+    # recenter the segment to 0
+    metric_data -= np.nanmean(metric_data)
+
+
+    #
+    # perform bandpass filtering using a butterworth filter
+    #
+
+    # third order Butterworth
+    Rp = 3
+    Rs = 60
+
+    #
+    delta = 0.001 * 2 / sampling_rate
+    low_p = bandpass[1] * 2 / sampling_rate
+    high_p = bandpass[0] * 2 / sampling_rate
+    high_s = max(delta, high_p - 0.1)
+    low_s = min(1 - delta, low_p + 0.1)
+
+    # Design a butterworth (band-pass) filter
+    # Note: the 'buttord' output here differs slight from matlab, because the scipy make a change in scipy 0.14.0 where
+    #       the choice of which end of the transition region was switched from the stop-band edge to the pass-band edge
+    n_band, wn_band = signal.buttord([high_p, low_p], [high_s, low_s], Rp, Rs, True)
+    bf_b, bf_a = signal.butter(n_band, wn_band, 'band', analog=False)
+
+    # Perform the band-passing
+    # Note: custom padlen to match the way matlab does it (-1 is omitted in scipy)
+    metric_data = signal.filtfilt(bf_b, bf_a, metric_data, padtype='odd', padlen=3 * (max(len(bf_b), len(bf_a)) - 1))
+
+    # calculate the band power using a hilbert transformation
+    band_power_sm = np.power(abs(signal.hilbert(metric_data)), 2)
+
+    # return the highest power value over time
+    return np.max(band_power_sm)
```

### Comparing `erdetect-1.1.0/erdetect/core/peak_finder.py` & `erdetect-2.0.0/erdetect/core/peak_finder.py`

 * *Files identical despite different names*

### Comparing `erdetect-1.1.0/erdetect/main_cli.py` & `erdetect-2.0.0/erdetect/main_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import argparse
 import logging
 import os
 import sys
-from glob import glob
 from bids_validator import BIDSValidator
 
 # add a system path to ensure the absolute imports can be used
 if not __package__:
     SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
     PACKAGE_DIR = os.path.dirname(SCRIPT_DIR)
     if PACKAGE_DIR not in sys.path:
         sys.path.insert(0, PACKAGE_DIR)
 
 # package imports
 from erdetect.version import __version__
 from erdetect.core.config import load_config, get as cfg, set as cfg_set, rem as cfg_rem,\
     LOGGING_CAPTION_INDENT_LENGTH, CONFIG_DETECTION_STD_BASE_BASELINE_EPOCH_DEFAULT, \
     CONFIG_DETECTION_STD_BASE_BASELINE_THRESHOLD_FACTOR, CONFIG_DETECTION_CROSS_PROJ_THRESHOLD, CONFIG_DETECTION_WAVEFORM_PROJ_THRESHOLD
-from erdetect._erdetect import process
-from erdetect.utils.IeegDataReader import VALID_FORMAT_EXTENSIONS
-from erdetect.utils.misc import is_number, multi_line_list
+from erdetect._erdetect import process_subset
+from ieegprep import VALID_FORMAT_EXTENSIONS
+from ieegprep.bids.data_structure import list_bids_datasets
+from ieegprep.utils.console import multi_line_list
+from ieegprep.utils.misc import is_number
 from erdetect._erdetect import log_indented_line
 
 
 def execute():
 
     #
     # define and parse the input arguments
@@ -53,28 +54,31 @@
     parser.add_argument('bids_dir',
                         help='The directory with the input dataset formatted according to the BIDS standard.\n\n')
     parser.add_argument('output_dir',
                         help='The directory where the output files should be stored. If you are running group\n'
                              'level analysis this folder should be prepopulated with the results of the\n'
                              'participant level analysis.\n\n')
     parser.add_argument('--participant_label',
-                        help='The label(s) of the participant(s) that should be analyzed. The label corresponds\n'
-                             'to sub-<participant_label> from the BIDS spec (so it does not include \'sub-\').\n'
-                             'If this parameter is not provided all subjects will be analyzed. Multiple\n'
-                             'participants can be specified with a space separated list.\n\n',
+                        help='This argument can be used to indicate which specific participant(s) in the BIDS\n'
+                             'directory should be analyzed. The given label(s) should correspond to the\n'
+                             'sub-<participant_label> as described in the BIDS specification. Label matching is\n'
+                             'case-insensitive and \'sub-\' prefixes in any of the labels will be ignored.\n'
+                             'If this parameter is not provided then all subjects will be analyzed. Multiple\n'
+                             'participant can be specified with a space separated list.\n\n',
                         nargs="+")
     parser.add_argument('--subset_search_pattern',
-                        help='The subset(s) of data that should be analyzed. The pattern should be part of a BIDS\n'
-                             'compliant folder name (e.g. \'task-ccep_run-01\'). If this parameter is not provided\n'
-                             'all the found subset(s) will be analyzed. Multiple subsets can be specified with\n'
-                             'a space separated list.\n\n',
+                        help='This argument can be used to ensure that a specific text has to occur in the\n'
+                             '(data) subset name for it to be analyzed. The pattern could be part of a BIDS\n'
+                             'compliant folder name (e.g. \'task-ccep_run-01\'). The search is case-insensitive.\n'
+                             'If this parameter is not provided then all the data subset(s) that are found will be\n'
+                             'analyzed. Multiple search patterns can be specified with a space separated list.\n\n',
                         nargs="+")
     parser.add_argument('--format_extension',
-                        help='The data format(s) to include. The format(s) should be specified by their\n'
-                             'extension (e.g. \'.edf\'). If this parameter is not provided, then by default\n'
+                        help='Can be used to limit the data format(s) to include. The format(s) should be specified\n'
+                             'by their extension (e.g. \'.edf\'). If this parameter is not provided, then by default\n'
                              'the European Data Format (\'.edf\'), BrainVision (\'.vhdr\', \'.vmrk\', \'.eeg\')\n'
                              'and MEF3 (\'.mefd\') formats will be included. Multiple formats can be specified\n'
                              'with a space separated list.\n\n',
                         nargs="+")
     parser.add_argument('--config_filepath',
                         help='Configures the app according to the settings in the JSON configuration file\n\n')
     parser.add_argument('--apply_bids_validator',
@@ -143,28 +147,41 @@
                              '      method setting in the configuration file\n\n',
                         nargs="?")
     parser.add_argument('-v', '--version',
                         action='version',
                         version='ER-Detect version {}'.format(__version__))
     args = parser.parse_args()
 
+
+    #
+    # make sure the output directory exists
+    #
+
+    # TODO: potentially the logging output can be written here from now on as well
+    if not os.path.exists(args.output_dir):
+        try:
+            os.makedirs(args.output_dir)
+        except OSError as e:
+            logging.error('Could not create output directory (\'' + args.output_dir + '\'), exiting...')
+            return 1
+
+
     #
     # display application information
     #
-    log_indented_line('Application:', ('Evoked Response Detection - v' + __version__))
-    log_indented_line('BIDS input path:', args.bids_dir)
-    log_indented_line('Output path:', args.output_dir)
-    if args.config_filepath:
-        log_indented_line('Configuration file:', args.config_filepath)
+    logging.info('------------------------ Evoked Response Detection - v' + __version__ + ' ------------------------')
     logging.info('')
 
 
     #
     # configure
     #
+    if args.config_filepath:
+        log_indented_line('Input configuration file:', args.config_filepath)
+        logging.info('')
 
     #  read the configuration file (if passed)
     if args.config_filepath:
         if not load_config(args.config_filepath):
             logging.error('Could not load the configuration file, exiting...')
             return 1
 
@@ -183,33 +200,33 @@
             # TODO: valid number
             cfg_set(str(args.line_noise_removal), 'preprocess', 'line_noise_removal')
         else:
             logging.error('Invalid line_noise_removal argument \'' + args.line_noise_removal + '\', either set to \'json\' or \'sidecar\' to retrieve the line-noise frequency from the *_ieeg.json file, or provide the line-noise frequency as a number.')
             return 1
 
     if args.early_reref:
-        if str(args.early_reref).lower() == 'car':
+        if str(args.early_reref[0]).lower() == 'car':
             cfg_set(True, 'preprocess', 'early_re_referencing', 'enabled')
             cfg_set('CAR', 'preprocess', 'early_re_referencing', 'method')
-        elif str(args.early_reref).lower() == 'car_headbox':
+        elif str(args.early_reref[0]).lower() == 'car_headbox':
             cfg_set(True, 'preprocess', 'early_re_referencing', 'enabled')
             cfg_set('CAR_headbox', 'preprocess', 'early_re_referencing', 'method')
         else:
-            logging.error('Invalid early_reref argument \'' + args.early_reref + '\'')
+            logging.error('Invalid early_reref argument \'' + args.early_reref[0] + '\'')
             return 1
 
     if args.late_reref:
-        if str(args.late_reref).lower() == 'car':
+        if str(args.late_reref[0]).lower() == 'car':
             cfg_set(True, 'preprocess', 'late_re_referencing', 'enabled')
             cfg_set('CAR', 'preprocess', 'late_re_referencing', 'method')
-        elif str(args.late_reref).lower() == 'car_headbox':
+        elif str(args.late_reref[0]).lower() == 'car_headbox':
             cfg_set(True, 'preprocess', 'late_re_referencing', 'enabled')
             cfg_set('CAR_headbox', 'preprocess', 'late_re_referencing', 'method')
         else:
-            logging.error('Invalid late_reref argument \'' + args.late_reref + '\'')
+            logging.error('Invalid late_reref argument \'' + args.late_reref[0] + '\'')
             return 1
 
     # check for methodological arguments
     if args.include_positive_responses:
         cfg_set(True, 'detection', 'positive')
         cfg_set(True, 'visualization', 'positive')
 
@@ -250,30 +267,30 @@
     # print configuration information
     log_indented_line('Preprocessing priority:', ('Speed' if preproc_prioritize_speed else 'Memory'))
     log_indented_line('High-pass filtering:', ('Yes' if cfg('preprocess', 'high_pass') else 'No'))
     log_indented_line('Early re-referencing:', ('Yes' if cfg('preprocess', 'early_re_referencing', 'enabled') else 'No'))
     if cfg('preprocess', 'early_re_referencing', 'enabled'):
         log_indented_line('    Method:', str(cfg('preprocess', 'early_re_referencing', 'method')))
         log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[1]) + 's')
-        logging.info(multi_line_list(cfg('preprocess', 'early_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 25, ' '))
+        logging.info(multi_line_list(cfg('preprocess', 'early_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
     log_indented_line('Line-noise removal:', cfg('preprocess', 'line_noise_removal') + (' Hz' if is_number(cfg('preprocess', 'line_noise_removal')) else ''))
     log_indented_line('Late re-referencing:', ('Yes' if cfg('preprocess', 'late_re_referencing', 'enabled') else 'No'))
     if cfg('preprocess', 'late_re_referencing', 'enabled'):
         log_indented_line('    Method:', str(cfg('preprocess', 'late_re_referencing', 'method')))
         log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[1]) + 's')
-        logging.info(multi_line_list(cfg('preprocess', 'late_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 25, ' '))
+        logging.info(multi_line_list(cfg('preprocess', 'late_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
     logging.info('')
     log_indented_line('Trial epoch window:', str(cfg('trials', 'trial_epoch')[0]) + 's < stim onset < ' + str(cfg('trials', 'trial_epoch')[1]) + 's  (window size ' + str(abs(cfg('trials', 'trial_epoch')[1] - cfg('trials', 'trial_epoch')[0])) + 's)')
     log_indented_line('Trial out-of-bounds handling:', str(cfg('trials', 'out_of_bounds_handling')))
     log_indented_line('Trial baseline window:', str(cfg('trials', 'baseline_epoch')[0]) + 's : ' + str(cfg('trials', 'baseline_epoch')[1]) + 's')
     log_indented_line('Trial baseline normalization:', str(cfg('trials', 'baseline_norm')))
     log_indented_line('Concatenate bidirectional stimulated pairs:', ('Yes' if cfg('trials', 'concat_bidirectional_pairs') else 'No'))
     log_indented_line('Minimum # of required stimulus-pair trials:', str(cfg('trials', 'minimum_stimpair_trials')))
-    logging.info(multi_line_list(cfg('channels', 'measured_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel types as measured:', 25, ' '))
-    logging.info(multi_line_list(cfg('channels', 'stim_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel type for stimulation:', 25, ' '))
+    logging.info(multi_line_list(cfg('channels', 'measured_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel types as measured:', 14, ' '))
+    logging.info(multi_line_list(cfg('channels', 'stim_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel types for stimulation:', 14, ' '))
     logging.info('')
     log_indented_line('Cross-projection metric:', ('Enabled' if cfg('metrics', 'cross_proj', 'enabled') else 'Disabled'))
     if cfg('metrics', 'cross_proj', 'enabled'):
         log_indented_line('    Cross-projection epoch:', str(cfg('metrics', 'cross_proj', 'epoch')[0]) + 's : ' + str(cfg('metrics', 'cross_proj', 'epoch')[1]) + 's')
     log_indented_line('Waveform metric:', ('Enabled' if cfg('metrics', 'waveform', 'enabled') else 'Disabled'))
     if cfg('metrics', 'waveform', 'enabled'):
         log_indented_line('    Waveform epoch:', str(cfg('metrics', 'waveform', 'epoch')[0]) + 's : ' + str(cfg('metrics', 'waveform', 'epoch')[1]) + 's')
@@ -298,19 +315,42 @@
     log_indented_line('    Positive responses:', ('Yes' if cfg('visualization', 'positive') else 'No'))
     log_indented_line('    X-axis epoch:', str(cfg('visualization', 'x_axis_epoch')[0]) + 's : ' + str(cfg('visualization', 'x_axis_epoch')[1]) + 's')
     log_indented_line('    Blank stimulation epoch:', str(cfg('visualization', 'blank_stim_epoch')[0]) + 's : ' + str(cfg('visualization', 'blank_stim_epoch')[1]) + 's')
     log_indented_line('    Generate electrode images:', ('Yes' if cfg('visualization', 'generate_electrode_images') else 'No'))
     log_indented_line('    Generate stimulation-pair images:', ('Yes' if cfg('visualization', 'generate_stimpair_images') else 'No'))
     log_indented_line('    Generate matrix images:', ('Yes' if cfg('visualization', 'generate_matrix_images') else 'No'))
     logging.info('')
+    logging.info('')
+    logging.info('')
 
 
     #
-    # check if the input is a valid BIDS dataset
+    # Find and process participants and their datasets
     #
+
+    logging.info('--------------------------------- Participants and data subsets ----------------------------------')
+    log_indented_line('BIDS input path:', args.bids_dir)
+    log_indented_line('Output path:', args.output_dir)
+    logging.info('')
+
+    # print optional search arguments
+    optional_search_argument = False
+    if args.participant_label:
+        log_indented_line('Participant(s) to include:', ", ".join(args.participant_label))
+        optional_search_argument = True
+    if args.subset_search_pattern:
+        log_indented_line('Subset search pattern(s):', ", ".join(args.subset_search_pattern))
+        optional_search_argument = True
+    if args.format_extension:
+        log_indented_line('Only include subsets with data extension(s):', ", ".join(args.format_extension))
+        optional_search_argument = True
+    if optional_search_argument:
+        logging.info('')
+
+    # check if the input is a valid BIDS dataset
     if args.apply_bids_validator:
         #process = run_cmd('bids-validator %s' % args.bids_dir)
         #logging.info(process.stdout)
         #if process.returncode != 0:
         #    logging.error('BIDS input dataset did not pass BIDS validator. Datasets can be validated online '
         #                    'using the BIDS Validator (http://incf.github.io/bids-validator/).\nRun the detection '
         #                    'without the --apply_bids_validator argument to skip prior BIDS validation.')
@@ -327,103 +367,64 @@
                     bids_error = True
         if bids_error:
             logging.error('BIDS input dataset did not pass the BIDS validator. Datasets can be validated online '
                           'using the BIDS Validator (http://incf.github.io/bids-validator/).\nRun the detection '
                           'without the --apply_bids_validator argument to skip prior BIDS validation.')
             return 1
 
-    #
-    # process per subject and subset
-    #
+    # list the datasets
+    strict_search = True if args.apply_bids_validator else False
+    datasets = list_bids_datasets(args.bids_dir,
+                                  dataset_extensions=VALID_FORMAT_EXTENSIONS,
+                                  subjects_filter=args.participant_label,
+                                  subset_search_pattern=args.subset_search_pattern, strict_search=strict_search,
+                                  only_subjects_with_subsets=True)
 
-    # make sure the output directory exists
-    if not os.path.exists(args.output_dir):
-        try:
-            os.makedirs(args.output_dir)
-        except OSError as e:
-            logging.error('Could not create output directory (\'' + args.output_dir + '\'), exiting...')
-            return 1
-
-    # list the subject to analyze (either based on the input parameter or list all in the BIDS_dir)
-    subjects_to_analyze = []
-    if args.participant_label:
-        # user-specified subjects
-        subjects_to_analyze = args.participant_label
+    #
+    if len(datasets) == 0:
+
+        logging.info('')
+        if optional_search_argument:
+            logging.warning('No datasets were found...\n'
+                            'Input arguments might have limited the search, make sure to check your CLI arguments')
+        else:
+            logging.warning('No datasets were found...')
 
     else:
-        # all subjects
-        subject_dirs = glob(os.path.join(args.bids_dir, 'sub-*'))
-        subjects_to_analyze = [subject_dir.split("-")[-1] for subject_dir in subject_dirs]
-
-    #
-    for subject in subjects_to_analyze:
-
-        # remove the sub part from the subject
-        if len(subject) > 4 and subject[0:4] == 'sub-':
-            subject = subject[4:]
-
-        # see if the subject is exists (in case the user specified the labels)
-        if os.path.isdir(os.path.join(args.bids_dir, ('sub-' + subject))):
-
-            # retrieve the data formats to include
-            if args.format_extension:
-                extensions = args.format_extension
-                for extension in extensions:
-                    if not any(extension in x for x in VALID_FORMAT_EXTENSIONS):
-                        logging.error('Invalid data format extension \'' + extension + '\', exiting...')
-                        return 1
-            else:
-                extensions = VALID_FORMAT_EXTENSIONS
-
-            # build path patterns for the search of subsets
-            subset_patterns = args.subset_search_pattern if args.subset_search_pattern else ('',)
-            subsets = []
-            modalities = ('*eeg',)                    # ieeg and eeg
-            for extension in extensions:
-                for modality in modalities:
-                    for subset_pattern in subset_patterns:
-                        subsets += glob(os.path.join(args.bids_dir, ('sub-' + subject), modality, '*' + subset_pattern + '*' + extension)) + \
-                                   glob(os.path.join(args.bids_dir, ('sub-' + subject), '*', modality, '*' + subset_pattern + '*' + extension))
-
-            # bring subsets with multiple formats down to one format (prioritized to occurrence in the extension var)
-            for subset in subsets:
-                subset_name = subset[:subset.rindex(".")]
-                for subset_other in reversed(subsets):
-                    if not subset == subset_other:
-                        subset_other_name = subset_other[:subset_other.rindex(".")]
-                        if subset_name == subset_other_name:
-                            subsets.remove(subset_other)
-
-            # TODO: mention all subsets before start processing
 
+        # display subject/subset information
+        logging.info('Participant(s) and subset(s) found:')
+        for (subject, subsets) in datasets.items():
+            short_subsets = [os.path.splitext(os.path.basename(os.path.normpath(x)))[0] for x in subsets]
+            short_subsets = [x[0:-5] if x.endswith('_ieeg') else x for x in short_subsets]
+            short_subsets = [x[0:-4] if x.endswith('_eeg') else x for x in short_subsets]
+            logging.info(multi_line_list(list(short_subsets), LOGGING_CAPTION_INDENT_LENGTH, '    ' + subject + ':', 1, ' '))
+        logging.info('')
 
-            # loop through the participant's subsets for analysis
+        # process
+        for (subject, subsets) in datasets.items():
             for subset in subsets:
 
                 # empty space
                 logging.info('')
                 logging.info('')
                 logging.info('')
 
-                #
+                # process
                 try:
-                    process(subset, args.output_dir, preproc_prioritize_speed)
+                    process_subset(subset, args.output_dir, preproc_prioritize_speed)
                 except RuntimeError:
                     logging.error('Error while processing dataset, exiting...')
                     return 1
 
-        else:
-            #
-            logging.warning('Participant \'' + subject + '\' could not be found, skipping')
-
     # empty space and end message
     logging.info('')
     logging.info('')
     logging.info('')
-    logging.info('- Finished running')
+    logging.info('--------------------------------------   Finished running   --------------------------------------')
 
     # return success exit code
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(execute())
```

### Comparing `erdetect-1.1.0/erdetect/views/output_images.py` & `erdetect-2.0.0/erdetect/views/output_images.py`

 * *Files identical despite different names*

### Comparing `erdetect-1.1.0/erdetect.egg-info/PKG-INFO` & `erdetect-2.0.0/erdetect.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,131 @@
-Metadata-Version: 2.1
-Name: erdetect
-Version: 1.1.0
-Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
-Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
-License: GPLv3
-Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
-Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
-Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
-Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Evoked Response Detection
-A python package and docker application for the automatic detection of evoked responses in SPES/CCEP data
-
-## Docker Usage
-
-To launch an instance of the container and analyse data in BIDS format, type:
-
-```
-$ docker run multimodalneuro/n1detect <bids_dir> <output_dir> [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
-```
-For example, to run an analysis, type:
-
-```
-docker run -ti --rm \
--v /local_bids_data_root/:/data \
--v /local_output_path/:/output \
-multimodalneuro/erdetect /data /output --participant_label 01 --skip_bids_validator
-```
-
-
-## Python Usage
-
-1. First install ERdetect, in the command-line run:
-```
-pip install erdetect
-```
-
-2. To run:
-- a) From the commandline:
-```
-python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
-```
-
-- b) A subset of the data directly in a python script:
-```
-import erdetect
-erdetect.process('/bids_data_root/bids_subj/ieeg/data_file', '/output_path/')
-```
-
-
-
-## Configure detection
-From the command-line, a JSON file can be passed using the ```--config_filepath [JSON_FILEPATH]``` parameter to adjust the preprocessing, the evoked response detection and the visualization settings.
-An example JSON containing the standard settings looks as follows:
-```
-{
-    "preprocess": {
-        "high_pass":                        false,
-        "line_noise_removal":               "off",
-        "early_re_referencing": {
-            "enabled":                      false,
-            "method":                       "CAR",
-            "stim_excl_epoch":              [-1.0,        2.0]
-        }
-    },
-	
-    "trials": {
-        "trial_epoch":                      [-1.0,        2.0],
-        "out_of_bounds_handling":           "first_last_only",
-        "baseline_epoch":                   [-0.5,      -0.02],
-        "baseline_norm":                    "median",
-        "concat_bidirectional_pairs":       true,
-        "minimum_stimpair_trials":          5
-    },
-
-    "channels": {
-        "measured_types":                   ["ECOG", "SEEG", "DBS"],
-        "stim_types":                       ["ECOG", "SEEG", "DBS"]
-    },
-
-    "detection": {
-        "negative":                         true,
-        "positive":                         false,
-        "peak_search_epoch":                [ 0,          0.5],
-        "response_search_epoch":            [ 0.009,     0.09],
-        "method":                           "std_base",
-        "std_base": {
-            "baseline_epoch":               [-1,         -0.1],
-            "baseline_threshold_factor":    3.4
-        }
-    },
-
-    "visualization": {
-        "negative":                         true,
-        "positive":                         false,
-        "x_axis_epoch":                     [-0.2,          1],
-        "blank_stim_epoch":                 [-0.015,   0.0025],
-        "generate_electrode_images":        true,
-        "generate_stimpair_images":         true,
-        "generate_matrix_images":           true
-    }
-}
-```
-
-
-## Acknowledgements
-
-- Written by Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
-- Local extremum detection method by Dorien van Blooijs & Dora Hermes (2018), with optimized parameters by Jaap van der Aar
-- Dependencies:
-  - PyMef by Jan Cimbalnik, Matt Stead, Ben Brinkmann, and Dan Crepeau (https://github.com/msel-source/pymef)
-  - MNE-Python (https://mne.tools/)
-  - BIDS-validator (https://github.com/bids-standard/bids-validator)
-  - NumPy
-  - SciPy
-  - Pandas
-  - KiwiSolver
-  - Matplotlib
-  - psutil
-
-- This project was funded by the National Institute Of Mental Health of the National Institutes of Health Award Number R01MH122258 to Dora Hermes
+Metadata-Version: 2.1
+Name: erdetect
+Version: 2.0.0
+Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
+Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
+License: GPLv3
+Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
+Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
+Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
+Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Evoked Response Detection
+A python package and docker application for the automatic detection of evoked responses in SPES/CCEP data
+
+## Docker Usage
+
+To launch an instance of the container and analyse data in BIDS format, in the command-line interface/terminal:
+
+```
+docker run multimodalneuro/erdetect <bids_dir>:/data <output_dir>:/output [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
+```
+For example, to run an analysis, type:
+
+```
+docker run -ti --rm \
+-v /local_bids_data_root/:/data \
+-v /local_output_path/:/output \
+multimodalneuro/erdetect /data /output --participant_label 01
+```
+
+
+## Python Usage
+
+1. First install ERdetect, in the command-line run:
+```
+pip install erdetect
+```
+
+2. To run:
+- a) From the commandline:
+```
+python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
+```
+
+- b) To process a subset directly in a python script:
+```
+import erdetect
+erdetect.process_subset('/bids_data_root/subj-01/ieeg/sub-01_run-06.edf', '/output_path/')
+```
+
+
+
+## Configure detection
+From the command-line, a JSON file can be passed using the ```--config_filepath [JSON_FILEPATH]``` parameter to adjust the preprocessing, the evoked response detection and the visualization settings.
+An example JSON containing the standard settings looks as follows:
+```
+{
+    "preprocess": {
+        "high_pass":                        false,
+        "line_noise_removal":               "off",
+        "early_re_referencing": {
+            "enabled":                      false,
+            "method":                       "CAR",
+            "stim_excl_epoch":              [-1.0,        2.0]
+        }
+    },
+	
+    "trials": {
+        "trial_epoch":                      [-1.0,        2.0],
+        "out_of_bounds_handling":           "first_last_only",
+        "baseline_epoch":                   [-0.5,      -0.02],
+        "baseline_norm":                    "median",
+        "concat_bidirectional_pairs":       true,
+        "minimum_stimpair_trials":          5
+    },
+
+    "channels": {
+        "measured_types":                   ["ECOG", "SEEG", "DBS"],
+        "stim_types":                       ["ECOG", "SEEG", "DBS"]
+    },
+
+    "detection": {
+        "negative":                         true,
+        "positive":                         false,
+        "peak_search_epoch":                [ 0,          0.5],
+        "response_search_epoch":            [ 0.009,     0.09],
+        "method":                           "std_base",
+        "std_base": {
+            "baseline_epoch":               [-1,         -0.1],
+            "baseline_threshold_factor":    3.4
+        }
+    },
+
+    "visualization": {
+        "negative":                         true,
+        "positive":                         false,
+        "x_axis_epoch":                     [-0.2,          1],
+        "blank_stim_epoch":                 [-0.015,   0.0025],
+        "generate_electrode_images":        true,
+        "generate_stimpair_images":         true,
+        "generate_matrix_images":           true
+    }
+}
+```
+
+
+## Acknowledgements
+
+- Written by Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
+- Local extremum detection method by Dorien van Blooijs & Dora Hermes (2018), with optimized parameters by Jaap van der Aar
+- Dependencies:
+  - IeegPrep (https://github.com/MultimodalNeuroimagingLab/ieegprep)
+  - BIDS-validator (https://github.com/bids-standard/bids-validator)
+  - NumPy
+  - SciPy
+  - Matplotlib
+
+- This project was funded by the National Institute Of Mental Health of the National Institutes of Health Award Number R01MH122258 to Dora Hermes
```

### Comparing `erdetect-1.1.0/erdetect.egg-info/SOURCES.txt` & `erdetect-2.0.0/erdetect.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,13 +14,11 @@
 erdetect.egg-info/top_level.txt
 erdetect/core/__init__.py
 erdetect/core/config.py
 erdetect/core/detection.py
 erdetect/core/peak_finder.py
 erdetect/core/metrics/metric_cross_proj.py
 erdetect/core/metrics/metric_waveform.py
-erdetect/utils/IeegDataReader.py
 erdetect/utils/__init__.py
-erdetect/utils/bids.py
 erdetect/utils/misc.py
 erdetect/views/__init__.py
 erdetect/views/output_images.py
```

### Comparing `erdetect-1.1.0/pyproject.toml` & `erdetect-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-[build-system]
-requires = [
-    "setuptools>=42",
-    "wheel"
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "erdetect"
-description = "A package for the automatic detection of evoked responses in SPES/CCEP data"
-readme = "README.md"
-license = { text="GPLv3" }
-requires-python = ">=3.8"
-keywords = ["evoked response", "detection", "ieeg", "n1", "SPES", "CCEP"]
-authors = [{ name="Max van den Boom", email="m.a.vandenboom84@gmail.com" }]
-classifiers = [
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.8",
-    "Topic :: Scientific/Engineering",
-]
-dynamic = ["version"]
-
-[tool.setuptools.dynamic]
-version = {attr = "erdetect.version.__version__"}
-
-[project.urls]
-homepage = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
-documentation = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
-repository = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
+[build-system]
+requires = [
+    "setuptools>=42",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "erdetect"
+description = "A package for the automatic detection of evoked responses in SPES/CCEP data"
+readme = "README.md"
+license = { text="GPLv3" }
+requires-python = ">=3.8"
+dependencies = [
+    "ieegprep >= 1.1.0",
+    "numpy >= 1.22.3",
+    "scipy >= 1.8.0",
+    "matplotlib >= 3.5.1",
+    "bids_validator >= 1.9.3",
+]
+keywords = ["evoked response", "detection", "ieeg", "n1", "SPES", "CCEP"]
+authors = [{ name="Max van den Boom", email="m.a.vandenboom84@gmail.com" }]
+classifiers = [
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
+    "Topic :: Scientific/Engineering",
+]
+dynamic = ["version"]
+
+[tool.setuptools.dynamic]
+version = {attr = "erdetect.version.__version__"}
+
+[project.urls]
+homepage = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
+documentation = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
+repository = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
+
```

