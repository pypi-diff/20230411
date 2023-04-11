# Comparing `tmp/pvcheetahdemo-1.1.3.tar.gz` & `tmp/pvcheetahdemo-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvcheetahdemo-1.1.3.tar", last modified: Mon Feb 27 19:43:52 2023, max compression
+gzip compressed data, was "pvcheetahdemo-1.1.4.tar", last modified: Tue Apr 11 00:49:17 2023, max compression
```

## Comparing `pvcheetahdemo-1.1.3.tar` & `pvcheetahdemo-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-27 19:43:52.305253 pvcheetahdemo-1.1.3/
--rw-rw-r--   0 nash      (1000) nash      (1000)      115 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/MANIFEST.in
--rw-rw-r--   0 nash      (1000) nash      (1000)     2858 2023-02-27 19:43:52.305253 pvcheetahdemo-1.1.3/PKG-INFO
--rw-rw-r--   0 nash      (1000) nash      (1000)     1687 2023-01-28 00:03:25.000000 pvcheetahdemo-1.1.3/README.md
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-27 19:43:52.305253 pvcheetahdemo-1.1.3/pvcheetahdemo/
--rw-rw-r--   0 nash      (1000) nash      (1000)    11344 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo/LICENSE
--rw-rw-r--   0 nash      (1000) nash      (1000)     3023 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo/cheetah_demo_file.py
--rw-rw-r--   0 nash      (1000) nash      (1000)     2931 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo/cheetah_demo_mic.py
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-27 19:43:52.305253 pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/
--rw-rw-r--   0 nash      (1000) nash      (1000)     2858 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/PKG-INFO
--rw-rw-r--   0 nash      (1000) nash      (1000)      345 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/SOURCES.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)        1 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/dependency_links.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)      131 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/entry_points.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)       35 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/requires.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)       14 2023-02-27 19:43:52.000000 pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/top_level.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)       38 2023-02-27 19:43:52.305253 pvcheetahdemo-1.1.3/setup.cfg
--rw-rw-r--   0 nash      (1000) nash      (1000)     2014 2023-02-27 19:29:06.000000 pvcheetahdemo-1.1.3/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      115 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/MANIFEST.in
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2399 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1687 2022-08-18 00:29:46.000000 pvcheetahdemo-1.1.4/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/pvcheetahdemo/
+-rw-rw-r--   0 eric      (1000) eric      (1000)    11344 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3023 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_file.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2931 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_mic.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2399 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      345 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      131 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       35 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-04-11 00:49:17.000000 pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-04-11 00:49:17.345500 pvcheetahdemo-1.1.4/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2014 2023-04-11 00:48:37.000000 pvcheetahdemo-1.1.4/setup.py
```

### Comparing `pvcheetahdemo-1.1.3/PKG-INFO` & `pvcheetahdemo-1.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 Metadata-Version: 2.1
 Name: pvcheetahdemo
-Version: 1.1.3
+Version: 1.1.4
 Summary: Cheetah speech-to-text engine demos
 Home-page: https://github.com/Picovoice/cheetah
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
-Description: # Cheetah Speech-to-Text Demos
-        
-        Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
-        
-        ## Cheetah
-        
-        Cheetah is an on-device streaming speech-to-text engine. Cheetah is:
-        
-        - Private; All voice processing runs locally.
-        - [Accurate](https://picovoice.ai/docs/benchmark/stt/)
-        - [Compact and Computationally-Efficient](https://github.com/Picovoice/speech-to-text-benchmark#rtf)
-        - Cross-Platform:
-            - Linux (x86_64), macOS (x86_64, arm64), and Windows (x86_64)
-            - Android and iOS
-            - Chrome, Safari, Firefox, and Edge
-            - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
-        
-        ## Compatibility
-        
-        - Python 3.5+
-        - Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
-        
-        ## Installation
-        
-        ```console
-        pip3 install pvcheetahdemo
-        ```
-        
-        ## AccessKey
-        
-        Cheetah requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Cheetah SDKs.
-        You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
-        Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
-        
-        ## Usage
-        
-        ### Microphone Demo
-        
-        You need a working microphone connected to your machine for this demo. Run the following in the terminal:
-        
-        ```console
-        cheetah_demo_mic --access_key ${ACCESS_KEY}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console.
-        
-        ### File Demo
-        
-        Run the following in the terminal:
-        
-        ```console
-        cheetah_demo_file --access_key ${ACCESS_KEY} --wav_paths ${WAV_PATH}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_PATH}` with a path to a compatible
-        (single-channel, 16 kHz, 16-bit PCM) wav file you wish to transcribe.
-        
 Keywords: Speech-to-Text,ASR,Speech Recognition,Voice Recognition,Automatic Speech Recognition
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# Cheetah Speech-to-Text Demos
+
+Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
+
+## Cheetah
+
+Cheetah is an on-device streaming speech-to-text engine. Cheetah is:
+
+- Private; All voice processing runs locally.
+- [Accurate](https://picovoice.ai/docs/benchmark/stt/)
+- [Compact and Computationally-Efficient](https://github.com/Picovoice/speech-to-text-benchmark#rtf)
+- Cross-Platform:
+    - Linux (x86_64), macOS (x86_64, arm64), and Windows (x86_64)
+    - Android and iOS
+    - Chrome, Safari, Firefox, and Edge
+    - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
+
+## Compatibility
+
+- Python 3.5+
+- Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
+
+## Installation
+
+```console
+pip3 install pvcheetahdemo
+```
+
+## AccessKey
+
+Cheetah requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Cheetah SDKs.
+You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
+Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
+
+## Usage
+
+### Microphone Demo
+
+You need a working microphone connected to your machine for this demo. Run the following in the terminal:
+
+```console
+cheetah_demo_mic --access_key ${ACCESS_KEY}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console.
+
+### File Demo
+
+Run the following in the terminal:
+
+```console
+cheetah_demo_file --access_key ${ACCESS_KEY} --wav_paths ${WAV_PATH}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_PATH}` with a path to a compatible
+(single-channel, 16 kHz, 16-bit PCM) wav file you wish to transcribe.
+
+
```

### Comparing `pvcheetahdemo-1.1.3/README.md` & `pvcheetahdemo-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pvcheetahdemo-1.1.3/pvcheetahdemo/LICENSE` & `pvcheetahdemo-1.1.4/pvcheetahdemo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvcheetahdemo-1.1.3/pvcheetahdemo/cheetah_demo_file.py` & `pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvcheetahdemo-1.1.3/pvcheetahdemo/cheetah_demo_mic.py` & `pvcheetahdemo-1.1.4/pvcheetahdemo/cheetah_demo_mic.py`

 * *Files identical despite different names*

### Comparing `pvcheetahdemo-1.1.3/pvcheetahdemo.egg-info/PKG-INFO` & `pvcheetahdemo-1.1.4/pvcheetahdemo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 Metadata-Version: 2.1
 Name: pvcheetahdemo
-Version: 1.1.3
+Version: 1.1.4
 Summary: Cheetah speech-to-text engine demos
 Home-page: https://github.com/Picovoice/cheetah
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
-Description: # Cheetah Speech-to-Text Demos
-        
-        Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
-        
-        ## Cheetah
-        
-        Cheetah is an on-device streaming speech-to-text engine. Cheetah is:
-        
-        - Private; All voice processing runs locally.
-        - [Accurate](https://picovoice.ai/docs/benchmark/stt/)
-        - [Compact and Computationally-Efficient](https://github.com/Picovoice/speech-to-text-benchmark#rtf)
-        - Cross-Platform:
-            - Linux (x86_64), macOS (x86_64, arm64), and Windows (x86_64)
-            - Android and iOS
-            - Chrome, Safari, Firefox, and Edge
-            - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
-        
-        ## Compatibility
-        
-        - Python 3.5+
-        - Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
-        
-        ## Installation
-        
-        ```console
-        pip3 install pvcheetahdemo
-        ```
-        
-        ## AccessKey
-        
-        Cheetah requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Cheetah SDKs.
-        You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
-        Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
-        
-        ## Usage
-        
-        ### Microphone Demo
-        
-        You need a working microphone connected to your machine for this demo. Run the following in the terminal:
-        
-        ```console
-        cheetah_demo_mic --access_key ${ACCESS_KEY}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console.
-        
-        ### File Demo
-        
-        Run the following in the terminal:
-        
-        ```console
-        cheetah_demo_file --access_key ${ACCESS_KEY} --wav_paths ${WAV_PATH}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_PATH}` with a path to a compatible
-        (single-channel, 16 kHz, 16-bit PCM) wav file you wish to transcribe.
-        
 Keywords: Speech-to-Text,ASR,Speech Recognition,Voice Recognition,Automatic Speech Recognition
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# Cheetah Speech-to-Text Demos
+
+Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
+
+## Cheetah
+
+Cheetah is an on-device streaming speech-to-text engine. Cheetah is:
+
+- Private; All voice processing runs locally.
+- [Accurate](https://picovoice.ai/docs/benchmark/stt/)
+- [Compact and Computationally-Efficient](https://github.com/Picovoice/speech-to-text-benchmark#rtf)
+- Cross-Platform:
+    - Linux (x86_64), macOS (x86_64, arm64), and Windows (x86_64)
+    - Android and iOS
+    - Chrome, Safari, Firefox, and Edge
+    - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
+
+## Compatibility
+
+- Python 3.5+
+- Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
+
+## Installation
+
+```console
+pip3 install pvcheetahdemo
+```
+
+## AccessKey
+
+Cheetah requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Cheetah SDKs.
+You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
+Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
+
+## Usage
+
+### Microphone Demo
+
+You need a working microphone connected to your machine for this demo. Run the following in the terminal:
+
+```console
+cheetah_demo_mic --access_key ${ACCESS_KEY}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console.
+
+### File Demo
+
+Run the following in the terminal:
+
+```console
+cheetah_demo_file --access_key ${ACCESS_KEY} --wav_paths ${WAV_PATH}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_PATH}` with a path to a compatible
+(single-channel, 16 kHz, 16-bit PCM) wav file you wish to transcribe.
+
+
```

### Comparing `pvcheetahdemo-1.1.3/setup.py` & `pvcheetahdemo-1.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvcheetahdemo/cheetah_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvcheetahdemo",
-    version="1.1.3",
+    version="1.1.4",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Cheetah speech-to-text engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/cheetah",
     packages=["pvcheetahdemo"],
-    install_requires=["pvcheetah==1.1.2", "pvrecorder==1.1.1"],
+    install_requires=["pvcheetah==1.1.3", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

