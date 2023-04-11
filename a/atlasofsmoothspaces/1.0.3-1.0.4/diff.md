# Comparing `tmp/atlasofsmoothspaces-1.0.3.tar.gz` & `tmp/atlasofsmoothspaces-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasofsmoothspaces-1.0.3.tar", last modified: Tue Apr 11 07:32:23 2023, max compression
+gzip compressed data, was "atlasofsmoothspaces-1.0.4.tar", last modified: Tue Apr 11 07:56:26 2023, max compression
```

## Comparing `atlasofsmoothspaces-1.0.3.tar` & `atlasofsmoothspaces-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/PKG-INFO
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/__init__.py
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7684 2023-04-11 07:21:08.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/main.py
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/PKG-INFO
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/SOURCES.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/dependency_links.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 07:32:23.000000 atlasofsmoothspaces-1.0.3/atlasofsmoothspaces.egg-info/top_level.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 07:32:23.868679 atlasofsmoothspaces-1.0.3/setup.cfg
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 07:32:19.000000 atlasofsmoothspaces-1.0.3/setup.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/PKG-INFO
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/__init__.py
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7773 2023-04-11 07:55:48.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/main.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/PKG-INFO
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 07:56:26.000000 atlasofsmoothspaces-1.0.4/atlasofsmoothspaces.egg-info/top_level.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 07:56:26.546502 atlasofsmoothspaces-1.0.4/setup.cfg
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 07:56:23.000000 atlasofsmoothspaces-1.0.4/setup.py
```

### Comparing `atlasofsmoothspaces-1.0.3/atlasofsmoothspaces/main.py` & `atlasofsmoothspaces-1.0.4/atlasofsmoothspaces/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,25 +99,30 @@
     NotAdmissibleType : Exception = Exception("Smoothness Type needs to be any of the admissible smoothness types: " + SMOOTHNESS_TYPES.__repr__())
 
     def __init__(
             self,
             smoothnessTypes: str or list[str],
             cacheLengths: None or int or list[int] = None, 
             derivativeDegrees: None or int or list[int] = None, 
-            alphas: None or float or list[float] = None):
+            alphas: None or float or list[float] = None,
+            customMidiMax: None or int = None):
         
         isNotAdmissibleSmoothnessType : bool = False
         if isinstance(smoothnessTypes, list):
             isNotAdmissibleSmoothnessType = any(t not in Smoothness.SMOOTHNESS_TYPES for t in smoothnessTypes)
         else:
             isNotAdmissibleSmoothnessType = smoothnessTypes not in Smoothness.SMOOTHNESS_TYPES
         
         if isNotAdmissibleSmoothnessType:
             raise Smoothness.NotAdmissibleType
         
+        if customMidiMax is not None:
+            self.midiMax = customMidiMax
+        else:
+            self.midiMax = Smoothness.MIDI_MAX
 
         if isinstance(smoothnessTypes, list):
             self.smoothnessTypes = smoothnessTypes
         else :
             self.smoothnessTypes = [smoothnessTypes]
         
         self.data : dict[str, SmoothnessBase] = {}
@@ -157,47 +162,47 @@
 
 
     def addNewValues(self, channelData: dict[int, float], returnSmoothness: bool = False):
         for smoothnessType in self.data.keys():
             newValue = self.conversion(smoothnessType, channelData)
             self.data[smoothnessType].addNewValue(newValue)
         if returnSmoothness:
-            self.getSmoothnessMeasure()
+            return self.getSmoothnessMeasure()
         
 
     def getSmoothnessMeasure(self):
         return {t:np.sum(v.smoothness**2) for t, v in self.data.items()}
         
 
 
 
     def conversion(self, smoothnessType: str, data: dict[int, float]):
         if (smoothnessType=="GYRO_LEFT"):
-            theta = data["CC16_1"] * 2 * np.pi / Smoothness.MIDI_MAX
-            phi = data["CC17_1"] * 2 * np.pi / Smoothness.MIDI_MAX
-            psi = data["CC18_1"] * 2 * np.pi / Smoothness.MIDI_MAX
+            theta = data["CC16_1"] * 2 * np.pi / self.midiMax
+            phi = data["CC17_1"] * 2 * np.pi / self.midiMax
+            psi = data["CC18_1"] * 2 * np.pi / self.midiMax
             return np.sqrt(theta**2 + phi**2 + psi**2)
         elif (smoothnessType=="GYRO_RIGHT"):
-            theta = data["CC16_2"] * 2 * np.pi / Smoothness.MIDI_MAX
-            phi = data["CC17_2"] * 2 * np.pi / Smoothness.MIDI_MAX
-            psi = data["CC18_2"] * 2 * np.pi / Smoothness.MIDI_MAX
+            theta = data["CC16_2"] * 2 * np.pi / self.midiMax
+            phi = data["CC17_2"] * 2 * np.pi / self.midiMax
+            psi = data["CC18_2"] * 2 * np.pi / self.midiMax
             return np.sqrt(theta**2 + phi**2 + psi**2)
         elif (smoothnessType=="VEL_LEFT"):
-            return data["CC22_1"] / Smoothness.MIDI_MAX
+            return data["CC22_1"] / self.midiMax
         elif (smoothnessType=="VEL_RIGHT"):
-            return data["CC22_2"] / Smoothness.MIDI_MAX
+            return data["CC22_2"] / self.midiMax
         elif (smoothnessType=="VEL_AVG"):
-            return (data["CC22_1"] + data["CC22_2"] ) / (2 * Smoothness.MIDI_MAX)
+            return (data["CC22_1"] + data["CC22_2"] ) / (2 * self.midiMax)
         if (smoothnessType=="ACCEL_LEFT"):
-            ax = data["CC19_1"]  / Smoothness.MIDI_MAX
-            ay = data["CC20_1"]  / Smoothness.MIDI_MAX
-            az = data["CC21_1"]  / Smoothness.MIDI_MAX
+            ax = data["CC19_1"]  / self.midiMax
+            ay = data["CC20_1"]  / self.midiMax
+            az = data["CC21_1"]  / self.midiMax
             return np.sqrt(ax**2 + ay**2 + az**2)
         elif (smoothnessType=="ACCEL_RIGHT"):
-            ax = data["CC19_2"] / Smoothness.MIDI_MAX
-            ay = data["CC20_2"] / Smoothness.MIDI_MAX
-            az = data["CC21_2"] / Smoothness.MIDI_MAX
+            ax = data["CC19_2"] / self.midiMax
+            ay = data["CC20_2"] / self.midiMax
+            az = data["CC21_2"] / self.midiMax
             return np.sqrt(ax**2 + ay**2 + az**2)
```

### Comparing `atlasofsmoothspaces-1.0.3/setup.py` & `atlasofsmoothspaces-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3' 
+VERSION = '1.0.4' 
 DESCRIPTION = 'Calculating Smoothness from Input Stream'
 LONG_DESCRIPTION = 'Smoothness is calculated from an input stream. The input data format is midi.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="atlasofsmoothspaces",
```

