# Comparing `tmp/ratinabox-1.3.4.tar.gz` & `tmp/ratinabox-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.3.4.tar", last modified: Tue Apr 11 09:22:25 2023, max compression
+gzip compressed data, was "ratinabox-1.4.0.tar", last modified: Tue Apr 11 09:24:48 2023, max compression
```

## Comparing `ratinabox-1.3.4.tar` & `ratinabox-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.715743 ratinabox-1.3.4/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.3.4/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:22:25.715871 ratinabox-1.3.4/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    24591 2023-04-11 09:20:54.000000 ratinabox-1.3.4/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.3.4/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.709092 ratinabox-1.3.4/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    41094 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    79913 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.3.4/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.711114 ratinabox-1.3.4/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.3.4/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.3.4/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.3.4/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.3.4/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.3.4/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    14973 2023-03-07 14:34:45.000000 ratinabox-1.3.4/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.3.4/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.3.4/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.712255 ratinabox-1.3.4/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.3.4/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.3.4/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.3.4/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.3.4/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    29721 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.709924 ratinabox-1.3.4/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      103 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      996 2023-04-11 09:22:25.716185 ratinabox-1.3.4/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.3.4/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.715631 ratinabox-1.3.4/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-01-09 16:43:43.000000 ratinabox-1.3.4/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.3.4/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.3.4/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.3.4/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.313537 ratinabox-1.4.0/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.4.0/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:24:48.313729 ratinabox-1.4.0/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    24591 2023-04-11 09:20:54.000000 ratinabox-1.4.0/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.4.0/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.306439 ratinabox-1.4.0/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    41094 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    79913 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.4.0/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.308395 ratinabox-1.4.0/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.4.0/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.4.0/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.4.0/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.4.0/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.4.0/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    14973 2023-03-07 14:34:45.000000 ratinabox-1.4.0/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.4.0/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.4.0/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.309725 ratinabox-1.4.0/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.4.0/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.4.0/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.4.0/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.4.0/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    29721 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.307183 ratinabox-1.4.0/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      103 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      996 2023-04-11 09:24:48.314080 ratinabox-1.4.0/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.4.0/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.313392 ratinabox-1.4.0/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-01-09 16:43:43.000000 ratinabox-1.4.0/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.4.0/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.4.0/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.4.0/tests/test_neurons.py
```

### Comparing `ratinabox-1.3.4/LICENSE` & `ratinabox-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/PKG-INFO` & `ratinabox-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.3.4
+Version: 1.4.0
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.3.4/README.md` & `ratinabox-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/Agent.py` & `ratinabox-1.4.0/ratinabox/Agent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/Environment.py` & `ratinabox-1.4.0/ratinabox/Environment.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/Neurons.py` & `ratinabox-1.4.0/ratinabox/Neurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/README.md` & `ratinabox-1.4.0/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/__init__.py` & `ratinabox-1.4.0/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.4.0/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.4.0/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.4.0/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/contribs/README.md` & `ratinabox-1.4.0/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.4.0/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.4.0/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.4.0/ratinabox/contribs/ValueNeuron.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/data/README.md` & `ratinabox-1.4.0/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/data/rat.png` & `ratinabox-1.4.0/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/data/sargolini.npz` & `ratinabox-1.4.0/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/data/tanni.npz` & `ratinabox-1.4.0/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox/utils.py` & `ratinabox-1.4.0/ratinabox/utils.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.4.0/ratinabox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.3.4
+Version: 1.4.0
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.3.4/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.4.0/ratinabox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/setup.cfg` & `ratinabox-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.3.4
+version = 1.4.0
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.3.4/tests/test_advanced.py` & `ratinabox-1.4.0/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.4/tests/test_environment.py` & `ratinabox-1.4.0/tests/test_environment.py`

 * *Files identical despite different names*

