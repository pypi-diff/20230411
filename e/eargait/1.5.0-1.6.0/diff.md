# Comparing `tmp/eargait-1.5.0.tar.gz` & `tmp/eargait-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eargait-1.5.0.tar", max compression
+gzip compressed data, was "eargait-1.6.0.tar", max compression
```

## Comparing `eargait-1.5.0.tar` & `eargait-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-03-15 14:59:25.463918 eargait-1.5.0/LICENSE
--rw-r--r--   0        0        0     5531 2023-03-15 14:59:25.463918 eargait-1.5.0/README.md
--rw-r--r--   0        0        0      154 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/base/__init__.py
--rw-r--r--   0        0        0     5028 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/base/base_eargait.py
--rw-r--r--   0        0        0    13447 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/eargait.py
--rw-r--r--   0        0        0      411 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/event_detection/__init__.py
--rw-r--r--   0        0        0    10084 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/event_detection/base_event_detection.py
--rw-r--r--   0        0        0     4957 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/event_detection/diao_adapted_event_detection.py
--rw-r--r--   0        0        0     8327 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/event_detection/diao_event_detection.py
--rw-r--r--   0        0        0     9077 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/event_detection/jarchi_event_detection.py
--rw-r--r--   0        0        0     9367 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/event_detection/mixed_event_detection.py
--rw-r--r--   0        0        0      307 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/preprocessing/__init__.py
--rw-r--r--   0        0        0     2275 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/preprocessing/load_data_helpers.py
--rw-r--r--   0        0        0     6833 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/preprocessing/rotations.py
--rw-r--r--   0        0        0      204 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/spatial_params/__init__.py
--rw-r--r--   0        0        0      296 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/spatial_params/spatial_params_base.py
--rw-r--r--   0        0        0     1340 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/spatial_params/spatial_params_example_class.py
--rw-r--r--   0        0        0        0 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/utils/__init__.py
--rw-r--r--   0        0        0      609 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/utils/consts.py
--rw-r--r--   0        0        0     1334 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/utils/example_data.py
--rw-r--r--   0        0        0     5535 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/utils/gait_parameters.py
--rw-r--r--   0        0        0     3809 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/utils/helper_datatype.py
--rw-r--r--   0        0        0    58034 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/utils/helper_gaitmap.py
--rw-r--r--   0        0        0     2033 2023-03-15 14:59:25.471918 eargait-1.5.0/eargait/utils/helpers.py
--rw-r--r--   0        0        0     2458 2023-03-15 14:59:25.535918 eargait-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 eargait-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-11 06:58:46.010700 eargait-1.6.0/LICENSE
+-rw-r--r--   0        0        0     5531 2023-04-11 06:58:46.010700 eargait-1.6.0/README.md
+-rw-r--r--   0        0        0      154 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/base/__init__.py
+-rw-r--r--   0        0        0     5028 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/base/base_eargait.py
+-rw-r--r--   0        0        0    13447 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/eargait.py
+-rw-r--r--   0        0        0      411 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/__init__.py
+-rw-r--r--   0        0        0    10101 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/base_event_detection.py
+-rw-r--r--   0        0        0     4990 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/diao_adapted_event_detection.py
+-rw-r--r--   0        0        0     8327 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/diao_event_detection.py
+-rw-r--r--   0        0        0     9077 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/jarchi_event_detection.py
+-rw-r--r--   0        0        0     9367 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/mixed_event_detection.py
+-rw-r--r--   0        0        0      307 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/preprocessing/load_data_helpers.py
+-rw-r--r--   0        0        0     6833 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/preprocessing/rotations.py
+-rw-r--r--   0        0        0      204 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/spatial_params/__init__.py
+-rw-r--r--   0        0        0      296 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/spatial_params/spatial_params_base.py
+-rw-r--r--   0        0        0     1340 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/spatial_params/spatial_params_example_class.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/__init__.py
+-rw-r--r--   0        0        0      609 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/consts.py
+-rw-r--r--   0        0        0     1334 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/example_data.py
+-rw-r--r--   0        0        0     5535 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/gait_parameters.py
+-rw-r--r--   0        0        0     3809 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/helper_datatype.py
+-rw-r--r--   0        0        0    58034 2023-04-11 06:58:46.026700 eargait-1.6.0/eargait/utils/helper_gaitmap.py
+-rw-r--r--   0        0        0     2033 2023-04-11 06:58:46.026700 eargait-1.6.0/eargait/utils/helpers.py
+-rw-r--r--   0        0        0     2458 2023-04-11 06:58:46.090701 eargait-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 eargait-1.6.0/PKG-INFO
```

### Comparing `eargait-1.5.0/LICENSE` & `eargait-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/README.md` & `eargait-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/base/base_eargait.py` & `eargait-1.6.0/eargait/base/base_eargait.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/eargait.py` & `eargait-1.6.0/eargait/eargait.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/event_detection/base_event_detection.py` & `eargait-1.6.0/eargait/event_detection/base_event_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         Returns
         -------
         self
             The class instance with all result attributes populated
 
         """
-        dataset_type = is_sensor_data(data, frame="body")
+        dataset_type = is_sensor_data(data, frame="body", check_gyr=False)
 
         self.data = data
 
         if dataset_type == "single":
             results = self._detect_single_dataset(self.data)  # noqa
         else:
             results_dict: Dict[Hashable, Dict[str, pd.DataFrame]] = {}
```

### Comparing `eargait-1.5.0/eargait/event_detection/diao_adapted_event_detection.py` & `eargait-1.6.0/eargait/event_detection/diao_adapted_event_detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,16 @@
 
         ic, ic_sides = self._detect_ic(acc_ssa_si[1], acc_ssa_ml[1], sample_rate_hz)
         tc, tc_sides = self._detect_tc(acc_ssa_ml[2] + acc_ssa_ml[1] + acc_ssa_ml[3], ic, ic_sides)
 
         ic += acc.index[0]
         tc += acc.index[0]
 
-        if np.abs(acc.shape[0] / (sample_rate_hz * ic.shape[0]) - 0.5) > 0.15:
+        step_time_ration = acc.shape[0] / sample_rate_hz / ic.shape[0]
+        if 0.3 > step_time_ration > 0.8:
             # print(np.abs(acc.shape[0]/(sample_rate_hz*ic.shape[0])-0.5))
             msg = (
                 f"Walking bout length and number of ICs are unrealistic: "
                 f"{acc.shape[0] / sample_rate_hz:.2f}s and {ic.shape[0]} steps"
             )
             warnings.warn(msg, UserWarning)
```

### Comparing `eargait-1.5.0/eargait/event_detection/diao_event_detection.py` & `eargait-1.6.0/eargait/event_detection/diao_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/event_detection/jarchi_event_detection.py` & `eargait-1.6.0/eargait/event_detection/jarchi_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/event_detection/mixed_event_detection.py` & `eargait-1.6.0/eargait/event_detection/mixed_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/preprocessing/load_data_helpers.py` & `eargait-1.6.0/eargait/preprocessing/load_data_helpers.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/preprocessing/rotations.py` & `eargait-1.6.0/eargait/preprocessing/rotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 def _get_rotation(session: Union[SyncedSession, Session, str]) -> Dict:
     if isinstance(session, Session) or session == "signia":
 
         if "D12" in session.info.version_firmware[0]:
             if "BMA400" == session.info.imu_sensor_type[0]:
                 rot_matrices = _get_rot_matrix_d12_bma400()
-                print("bma 400 and D12")
+                print("BMA 400 and D12")
             else:
                 rot_matrices = _get_rot_matrix_d12()
                 print("D12")
         else:
             rot_matrices = _get_rot_matrix_default()
             print("D11, default")
```

### Comparing `eargait-1.5.0/eargait/spatial_params/spatial_params_example_class.py` & `eargait-1.6.0/eargait/spatial_params/spatial_params_example_class.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/utils/consts.py` & `eargait-1.6.0/eargait/utils/consts.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/utils/example_data.py` & `eargait-1.6.0/eargait/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/utils/gait_parameters.py` & `eargait-1.6.0/eargait/utils/gait_parameters.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/utils/helper_datatype.py` & `eargait-1.6.0/eargait/utils/helper_datatype.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/utils/helper_gaitmap.py` & `eargait-1.6.0/eargait/utils/helper_gaitmap.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/eargait/utils/helpers.py` & `eargait-1.6.0/eargait/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `eargait-1.5.0/pyproject.toml` & `eargait-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eargait"
-version = "1.5.0"
+version = "1.6.0"
 description = "*Eargait* provides a set of algorithms and functions to process IMU data recorded with ear-worn IMU sensors and to estimate characteristic gait parameters. "
 authors = ["Ann-Kristin Seifer <ann-kristin.seifer@fau.de>",
             "Arne Küderle <arne.kuederle@fau.de>"]
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/eargait"
 repository = "https://github.com/mad-lab-fau/eargait"
```

### Comparing `eargait-1.5.0/PKG-INFO` & `eargait-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eargait
-Version: 1.5.0
+Version: 1.6.0
 Summary: *Eargait* provides a set of algorithms and functions to process IMU data recorded with ear-worn IMU sensors and to estimate characteristic gait parameters. 
 Home-page: https://github.com/mad-lab-fau/eargait
 Author: Ann-Kristin Seifer
 Author-email: ann-kristin.seifer@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

