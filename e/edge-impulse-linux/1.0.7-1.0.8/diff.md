# Comparing `tmp/edge_impulse_linux-1.0.7.tar.gz` & `tmp/edge_impulse_linux-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_impulse_linux-1.0.7.tar", last modified: Mon Jul 18 09:29:43 2022, max compression
+gzip compressed data, was "edge_impulse_linux-1.0.8.tar", last modified: Tue Apr 11 12:09:47 2023, max compression
```

## Comparing `edge_impulse_linux-1.0.7.tar` & `edge_impulse_linux-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 janjongboom   (501) staff       (20)        0 2022-07-18 09:29:43.146546 edge_impulse_linux-1.0.7/
--rw-r--r--   0 janjongboom   (501) staff       (20)     9115 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.7/LICENSE
--rw-r--r--   0 janjongboom   (501) staff       (20)     4775 2022-07-18 09:29:43.146645 edge_impulse_linux-1.0.7/PKG-INFO
--rw-r--r--   0 janjongboom   (501) staff       (20)     4176 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.7/README.md
-drwxr-xr-x   0 janjongboom   (501) staff       (20)        0 2022-07-18 09:29:43.144939 edge_impulse_linux-1.0.7/edge_impulse_linux/
--rw-r--r--   0 janjongboom   (501) staff       (20)      112 2022-07-18 09:18:44.000000 edge_impulse_linux-1.0.7/edge_impulse_linux/__init__.py
--rw-r--r--   0 janjongboom   (501) staff       (20)     5731 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.7/edge_impulse_linux/audio.py
--rw-r--r--   0 janjongboom   (501) staff       (20)     5105 2022-07-18 09:25:36.000000 edge_impulse_linux-1.0.7/edge_impulse_linux/image.py
--rwxr-xr-x   0 janjongboom   (501) staff       (20)     3352 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.7/edge_impulse_linux/runner.py
-drwxr-xr-x   0 janjongboom   (501) staff       (20)        0 2022-07-18 09:29:43.146324 edge_impulse_linux-1.0.7/edge_impulse_linux.egg-info/
--rw-r--r--   0 janjongboom   (501) staff       (20)     4775 2022-07-18 09:29:42.000000 edge_impulse_linux-1.0.7/edge_impulse_linux.egg-info/PKG-INFO
--rw-r--r--   0 janjongboom   (501) staff       (20)      376 2022-07-18 09:29:43.000000 edge_impulse_linux-1.0.7/edge_impulse_linux.egg-info/SOURCES.txt
--rw-r--r--   0 janjongboom   (501) staff       (20)        1 2022-07-18 09:29:42.000000 edge_impulse_linux-1.0.7/edge_impulse_linux.egg-info/dependency_links.txt
--rw-r--r--   0 janjongboom   (501) staff       (20)       50 2022-07-18 09:29:43.000000 edge_impulse_linux-1.0.7/edge_impulse_linux.egg-info/requires.txt
--rw-r--r--   0 janjongboom   (501) staff       (20)       19 2022-07-18 09:29:43.000000 edge_impulse_linux-1.0.7/edge_impulse_linux.egg-info/top_level.txt
--rw-r--r--   0 janjongboom   (501) staff       (20)      105 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.7/pyproject.toml
--rw-r--r--   0 janjongboom   (501) staff       (20)      701 2022-07-18 09:29:43.147169 edge_impulse_linux-1.0.7/setup.cfg
--rw-r--r--   0 janjongboom   (501) staff       (20)       38 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.7/setup.py
+drwxr-xr-x   0 janjongboom   (501) staff       (20)        0 2023-04-11 12:09:47.747646 edge_impulse_linux-1.0.8/
+-rw-r--r--   0 janjongboom   (501) staff       (20)     9115 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.8/LICENSE
+-rw-r--r--   0 janjongboom   (501) staff       (20)     4905 2023-04-11 12:09:47.747738 edge_impulse_linux-1.0.8/PKG-INFO
+-rw-r--r--   0 janjongboom   (501) staff       (20)     4343 2023-04-11 12:08:10.000000 edge_impulse_linux-1.0.8/README.md
+drwxr-xr-x   0 janjongboom   (501) staff       (20)        0 2023-04-11 12:09:47.746473 edge_impulse_linux-1.0.8/edge_impulse_linux/
+-rw-r--r--   0 janjongboom   (501) staff       (20)      112 2022-07-18 09:18:44.000000 edge_impulse_linux-1.0.8/edge_impulse_linux/__init__.py
+-rw-r--r--   0 janjongboom   (501) staff       (20)     5731 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.8/edge_impulse_linux/audio.py
+-rw-r--r--   0 janjongboom   (501) staff       (20)     5105 2022-07-18 09:25:36.000000 edge_impulse_linux-1.0.8/edge_impulse_linux/image.py
+-rwxr-xr-x   0 janjongboom   (501) staff       (20)     3434 2023-04-11 12:05:46.000000 edge_impulse_linux-1.0.8/edge_impulse_linux/runner.py
+drwxr-xr-x   0 janjongboom   (501) staff       (20)        0 2023-04-11 12:09:47.747437 edge_impulse_linux-1.0.8/edge_impulse_linux.egg-info/
+-rw-r--r--   0 janjongboom   (501) staff       (20)     4905 2023-04-11 12:09:47.000000 edge_impulse_linux-1.0.8/edge_impulse_linux.egg-info/PKG-INFO
+-rw-r--r--   0 janjongboom   (501) staff       (20)      376 2023-04-11 12:09:47.000000 edge_impulse_linux-1.0.8/edge_impulse_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 janjongboom   (501) staff       (20)        1 2023-04-11 12:09:47.000000 edge_impulse_linux-1.0.8/edge_impulse_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 janjongboom   (501) staff       (20)       26 2023-04-11 12:09:47.000000 edge_impulse_linux-1.0.8/edge_impulse_linux.egg-info/requires.txt
+-rw-r--r--   0 janjongboom   (501) staff       (20)       19 2023-04-11 12:09:47.000000 edge_impulse_linux-1.0.8/edge_impulse_linux.egg-info/top_level.txt
+-rw-r--r--   0 janjongboom   (501) staff       (20)      105 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.8/pyproject.toml
+-rw-r--r--   0 janjongboom   (501) staff       (20)      676 2023-04-11 12:09:47.748041 edge_impulse_linux-1.0.8/setup.cfg
+-rw-r--r--   0 janjongboom   (501) staff       (20)       38 2022-02-20 11:53:36.000000 edge_impulse_linux-1.0.8/setup.py
```

### Comparing `edge_impulse_linux-1.0.7/LICENSE` & `edge_impulse_linux-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_impulse_linux-1.0.7/PKG-INFO` & `edge_impulse_linux-1.0.8/edge_impulse_linux.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
-Name: edge_impulse_linux
-Version: 1.0.7
+Name: edge-impulse-linux
+Version: 1.0.8
 Summary: Python runner for real-time ML classification
 Home-page: https://github.com/edgeimpulse/linux-sdk-python
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/edgeimpulse/linux-sdk-python/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Edge Impulse Linux SDK for Python
 
 This library lets you run machine learning models and collect sensor data on Linux machines using Python. This SDK is part of [Edge Impulse](https://www.edgeimpulse.com) where we enable developers to create the next generation of intelligent device solutions with embedded machine learning. [Start here to learn more and train your first model](https://docs.edgeimpulse.com).
 
 ## Installation guide
 
-1. Install a recent version of [Python 3](https://www.python.org/downloads/).
+1. Install a recent version of [Python 3](https://www.python.org/downloads/) and `pip` tools.
 1. Install the SDK:
 
     **Raspberry Pi**
 
     ```
-    $ sudo apt-get install libatlas-base-dev libportaudio0 libportaudio2 libportaudiocpp0 portaudio19-dev
+    $ sudo apt-get install libatlas-base-dev libportaudio0 libportaudio2 libportaudiocpp0 portaudio19-dev libopenjp2-7 libgtk-3-0 libswscale-dev libavformat58 libavcodec58
     $ pip3 install edge_impulse_linux -i https://pypi.python.org/simple
     ```
 
     **Other platforms**
 
     ```
     $ pip3 install edge_impulse_linux
@@ -39,25 +37,27 @@
 
 1. Clone this repository to get the examples:
 
     ```
     $ git clone https://github.com/edgeimpulse/linux-sdk-python
     ```
 
+    For the computer vision examples you'll want `opencv-python>=4.5.1.48`
+
 ## Collecting data
 
 Before you can classify data you'll first need to collect it. If you want to collect data from the camera or microphone on your system you can use the Edge Impulse CLI, and if you want to collect data from different sensors (like accelerometers or proprietary control systems) you can do so in a few lines of code.
 
 ### Collecting data from the camera or microphone
 
 To collect data from the camera or microphone, follow the [getting started guide](https://docs.edgeimpulse.com/docs/edge-impulse-for-linux) for your development board.
 
 ### Collecting data from other sensors
 
-To collect data from other sensors you'll need to write some code to collect the data from an external sensor, wrap it in the Edge Impulse Data Acquisition format, and upload the data to the Ingestion service. [Here's an end-to-end example](https://github.com/edgeimpulse/linux-sdk-python/blob/master/custom/collect.py).
+To collect data from other sensors you'll need to write some code to collect the data from an external sensor, wrap it in the Edge Impulse Data Acquisition format, and upload the data to the Ingestion service. [Here's an end-to-end example](https://github.com/edgeimpulse/linux-sdk-python/blob/master/examples/custom/collect.py).
 
 ## Classifying data
 
 To classify data (whether this is from the camera, the microphone, or a custom sensor) you'll need a model file. This model file contains all signal processing code, classical ML algorithms and neural networks - and typically contains hardware optimizations to run as fast as possible. To grab a model file:
 
 1. Train your model in Edge Impulse.
 1. Install the [Edge Impulse for Linux CLI](https://docs.edgeimpulse.com/docs/edge-impulse-for-linux).
@@ -88,9 +88,7 @@
 brew uninstall --ignore-dependencies portaudio
 brew install portaudio --HEAD​
 ```
 
 ### Abort trap (6) (macOS)
 
 This error shows when you want to gain access to the camera or the microphone on macOS from a virtual shell (like the terminal in Visual Studio Code). Try to run the command from the normal Terminal.app.
-
-
```

### Comparing `edge_impulse_linux-1.0.7/README.md` & `edge_impulse_linux-1.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Edge Impulse Linux SDK for Python
 
 This library lets you run machine learning models and collect sensor data on Linux machines using Python. This SDK is part of [Edge Impulse](https://www.edgeimpulse.com) where we enable developers to create the next generation of intelligent device solutions with embedded machine learning. [Start here to learn more and train your first model](https://docs.edgeimpulse.com).
 
 ## Installation guide
 
-1. Install a recent version of [Python 3](https://www.python.org/downloads/).
+1. Install a recent version of [Python 3](https://www.python.org/downloads/) and `pip` tools.
 1. Install the SDK:
 
     **Raspberry Pi**
 
     ```
-    $ sudo apt-get install libatlas-base-dev libportaudio0 libportaudio2 libportaudiocpp0 portaudio19-dev
+    $ sudo apt-get install libatlas-base-dev libportaudio0 libportaudio2 libportaudiocpp0 portaudio19-dev libopenjp2-7 libgtk-3-0 libswscale-dev libavformat58 libavcodec58
     $ pip3 install edge_impulse_linux -i https://pypi.python.org/simple
     ```
 
     **Other platforms**
 
     ```
     $ pip3 install edge_impulse_linux
@@ -22,25 +22,27 @@
 
 1. Clone this repository to get the examples:
 
     ```
     $ git clone https://github.com/edgeimpulse/linux-sdk-python
     ```
 
+    For the computer vision examples you'll want `opencv-python>=4.5.1.48`
+
 ## Collecting data
 
 Before you can classify data you'll first need to collect it. If you want to collect data from the camera or microphone on your system you can use the Edge Impulse CLI, and if you want to collect data from different sensors (like accelerometers or proprietary control systems) you can do so in a few lines of code.
 
 ### Collecting data from the camera or microphone
 
 To collect data from the camera or microphone, follow the [getting started guide](https://docs.edgeimpulse.com/docs/edge-impulse-for-linux) for your development board.
 
 ### Collecting data from other sensors
 
-To collect data from other sensors you'll need to write some code to collect the data from an external sensor, wrap it in the Edge Impulse Data Acquisition format, and upload the data to the Ingestion service. [Here's an end-to-end example](https://github.com/edgeimpulse/linux-sdk-python/blob/master/custom/collect.py).
+To collect data from other sensors you'll need to write some code to collect the data from an external sensor, wrap it in the Edge Impulse Data Acquisition format, and upload the data to the Ingestion service. [Here's an end-to-end example](https://github.com/edgeimpulse/linux-sdk-python/blob/master/examples/custom/collect.py).
 
 ## Classifying data
 
 To classify data (whether this is from the camera, the microphone, or a custom sensor) you'll need a model file. This model file contains all signal processing code, classical ML algorithms and neural networks - and typically contains hardware optimizations to run as fast as possible. To grab a model file:
 
 1. Train your model in Edge Impulse.
 1. Install the [Edge Impulse for Linux CLI](https://docs.edgeimpulse.com/docs/edge-impulse-for-linux).
```

### Comparing `edge_impulse_linux-1.0.7/edge_impulse_linux/audio.py` & `edge_impulse_linux-1.0.8/edge_impulse_linux/audio.py`

 * *Files identical despite different names*

### Comparing `edge_impulse_linux-1.0.7/edge_impulse_linux/image.py` & `edge_impulse_linux-1.0.8/edge_impulse_linux/image.py`

 * *Files identical despite different names*

### Comparing `edge_impulse_linux-1.0.7/edge_impulse_linux/runner.py` & `edge_impulse_linux-1.0.8/edge_impulse_linux/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,15 +95,18 @@
                     resp = json.loads(line)
             elif braces_open > 0:
                 line = line + c
 
             if (not resp is None):
                 break
 
-        if (not resp or resp["id"] != ix):
+        if (resp is None):
+            raise Exception('No data or corrupted data received')
+
+        if (resp["id"] != ix):
             raise Exception('Wrong id, expected: ' + str(ix) + ' but got ' + resp["id"])
 
         if not resp["success"]:
             raise Exception(resp["error"])
 
         del resp["id"]
         del resp["success"]
```

### Comparing `edge_impulse_linux-1.0.7/edge_impulse_linux.egg-info/PKG-INFO` & `edge_impulse_linux-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
-Name: edge-impulse-linux
-Version: 1.0.7
+Name: edge_impulse_linux
+Version: 1.0.8
 Summary: Python runner for real-time ML classification
 Home-page: https://github.com/edgeimpulse/linux-sdk-python
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/edgeimpulse/linux-sdk-python/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Edge Impulse Linux SDK for Python
 
 This library lets you run machine learning models and collect sensor data on Linux machines using Python. This SDK is part of [Edge Impulse](https://www.edgeimpulse.com) where we enable developers to create the next generation of intelligent device solutions with embedded machine learning. [Start here to learn more and train your first model](https://docs.edgeimpulse.com).
 
 ## Installation guide
 
-1. Install a recent version of [Python 3](https://www.python.org/downloads/).
+1. Install a recent version of [Python 3](https://www.python.org/downloads/) and `pip` tools.
 1. Install the SDK:
 
     **Raspberry Pi**
 
     ```
-    $ sudo apt-get install libatlas-base-dev libportaudio0 libportaudio2 libportaudiocpp0 portaudio19-dev
+    $ sudo apt-get install libatlas-base-dev libportaudio0 libportaudio2 libportaudiocpp0 portaudio19-dev libopenjp2-7 libgtk-3-0 libswscale-dev libavformat58 libavcodec58
     $ pip3 install edge_impulse_linux -i https://pypi.python.org/simple
     ```
 
     **Other platforms**
 
     ```
     $ pip3 install edge_impulse_linux
@@ -39,25 +37,27 @@
 
 1. Clone this repository to get the examples:
 
     ```
     $ git clone https://github.com/edgeimpulse/linux-sdk-python
     ```
 
+    For the computer vision examples you'll want `opencv-python>=4.5.1.48`
+
 ## Collecting data
 
 Before you can classify data you'll first need to collect it. If you want to collect data from the camera or microphone on your system you can use the Edge Impulse CLI, and if you want to collect data from different sensors (like accelerometers or proprietary control systems) you can do so in a few lines of code.
 
 ### Collecting data from the camera or microphone
 
 To collect data from the camera or microphone, follow the [getting started guide](https://docs.edgeimpulse.com/docs/edge-impulse-for-linux) for your development board.
 
 ### Collecting data from other sensors
 
-To collect data from other sensors you'll need to write some code to collect the data from an external sensor, wrap it in the Edge Impulse Data Acquisition format, and upload the data to the Ingestion service. [Here's an end-to-end example](https://github.com/edgeimpulse/linux-sdk-python/blob/master/custom/collect.py).
+To collect data from other sensors you'll need to write some code to collect the data from an external sensor, wrap it in the Edge Impulse Data Acquisition format, and upload the data to the Ingestion service. [Here's an end-to-end example](https://github.com/edgeimpulse/linux-sdk-python/blob/master/examples/custom/collect.py).
 
 ## Classifying data
 
 To classify data (whether this is from the camera, the microphone, or a custom sensor) you'll need a model file. This model file contains all signal processing code, classical ML algorithms and neural networks - and typically contains hardware optimizations to run as fast as possible. To grab a model file:
 
 1. Train your model in Edge Impulse.
 1. Install the [Edge Impulse for Linux CLI](https://docs.edgeimpulse.com/docs/edge-impulse-for-linux).
@@ -88,9 +88,7 @@
 brew uninstall --ignore-dependencies portaudio
 brew install portaudio --HEAD​
 ```
 
 ### Abort trap (6) (macOS)
 
 This error shows when you want to gain access to the camera or the microphone on macOS from a virtual shell (like the terminal in Visual Studio Code). Try to run the command from the normal Terminal.app.
-
-
```

### Comparing `edge_impulse_linux-1.0.7/setup.cfg` & `edge_impulse_linux-1.0.8/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edge_impulse_linux
-version = 1.0.7
+version = 1.0.8
 author = EdgeImpulse Inc.
 author_email = hello@edgeimpulse.com
 description = Python runner for real-time ML classification
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/edgeimpulse/linux-sdk-python
 project_urls = 
@@ -15,14 +15,13 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy>=1.19
-	opencv-python>=4.5.1.48
 	psutil>=5.8.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

