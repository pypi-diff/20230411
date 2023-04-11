# Comparing `tmp/pvkoalademo-1.0.1.tar.gz` & `tmp/pvkoalademo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvkoalademo-1.0.1.tar", last modified: Wed Feb  8 00:13:08 2023, max compression
+gzip compressed data, was "pvkoalademo-1.0.2.tar", last modified: Tue Apr 11 00:49:25 2023, max compression
```

## Comparing `pvkoalademo-1.0.1.tar` & `pvkoalademo-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-08 00:13:08.470420 pvkoalademo-1.0.1/
--rw-rw-r--   0 nash      (1000) nash      (1000)      105 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/MANIFEST.in
--rw-rw-r--   0 nash      (1000) nash      (1000)     3379 2023-02-08 00:13:08.470420 pvkoalademo-1.0.1/PKG-INFO
--rw-rw-r--   0 nash      (1000) nash      (1000)     2169 2023-02-07 18:46:01.000000 pvkoalademo-1.0.1/README.md
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-08 00:13:08.470420 pvkoalademo-1.0.1/pvkoalademo/
--rw-rw-r--   0 nash      (1000) nash      (1000)    11357 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo/LICENSE
--rw-rw-r--   0 nash      (1000) nash      (1000)     5041 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo/koala_demo_file.py
--rw-rw-r--   0 nash      (1000) nash      (1000)     5190 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo/koala_demo_mic.py
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-08 00:13:08.470420 pvkoalademo-1.0.1/pvkoalademo.egg-info/
--rw-rw-r--   0 nash      (1000) nash      (1000)     3379 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo.egg-info/PKG-INFO
--rw-rw-r--   0 nash      (1000) nash      (1000)      323 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo.egg-info/SOURCES.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)        1 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo.egg-info/dependency_links.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)      119 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo.egg-info/entry_points.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)       33 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo.egg-info/requires.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)       12 2023-02-08 00:13:08.000000 pvkoalademo-1.0.1/pvkoalademo.egg-info/top_level.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)       38 2023-02-08 00:13:08.470420 pvkoalademo-1.0.1/setup.cfg
--rw-rw-r--   0 nash      (1000) nash      (1000)     1773 2023-02-07 22:37:47.000000 pvkoalademo-1.0.1/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:25.669546 pvkoalademo-1.0.2/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      105 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/MANIFEST.in
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2880 2023-04-11 00:49:25.669546 pvkoalademo-1.0.2/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2169 2023-02-07 23:09:03.000000 pvkoalademo-1.0.2/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:25.669546 pvkoalademo-1.0.2/pvkoalademo/
+-rw-rw-r--   0 eric      (1000) eric      (1000)    11357 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)     5041 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo/koala_demo_file.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     5190 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo/koala_demo_mic.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:49:25.669546 pvkoalademo-1.0.2/pvkoalademo.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2880 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      323 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      119 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       33 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       12 2023-04-11 00:49:25.000000 pvkoalademo-1.0.2/pvkoalademo.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-04-11 00:49:25.669546 pvkoalademo-1.0.2/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1773 2023-04-11 00:49:00.000000 pvkoalademo-1.0.2/setup.py
```

### Comparing `pvkoalademo-1.0.1/PKG-INFO` & `pvkoalademo-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 Metadata-Version: 2.1
 Name: pvkoalademo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Koala Noise Suppression Engine demos
 Home-page: https://github.com/Picovoice/koala
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
-Description: # Koala Noise Suppression Demos
-        
-        Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
-        
-        ## Koala
-        
-        Koala is an on-device noise suppression engine. Koala is:
-        
-        - Private; All voice processing runs locally.
-        - Cross-Platform:
-          - Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64)
-          - Android and iOS
-          - Chrome, Safari, Firefox, and Edge
-          - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
-        
-        ## Compatibility
-        
-        - Python 3.5+
-        - Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
-        
-        ## Installation
-        
-        ```console
-        pip3 install pvkoalademo
-        ```
-        
-        ## AccessKey
-        
-        Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
-        SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
-        Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
-        
-        ## Usage
-        
-        ### Microphone Demo
-        
-        The microphone demo collects audio from a microphone connected to your machine. The audio is passed through the Koala
-        noise suppression engine and stored in a `.wav` file.
-        Run the following in the terminal:
-        
-        ```console
-        koala_demo_mic --access_key ${ACCESS_KEY} --output-path ${WAV_OUTPUT_PATH}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_OUTPUT_PATH}` with a path to a `.wav` file
-        where the enhanced audio will be stored. Terminate the demo with `Ctrl+C`.
-        
-        ### File Demo
-        
-        The file demo passes audio stored in a `.wav` file through the Koala noise suppression engine. The result is shifted to
-        compensate for the delay introduced by Koala and stored in a separate `.wav` file that will have the same length as the
-        input file without any delay.
-        Run the following in the terminal:
-        
-        ```console
-        koala_demo_file --access_key ${ACCESS_KEY} --input_path ${WAV_INPUT_PATH} --output_path ${WAV_OUTPUT_PATH}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console, `${WAV_INPUT_PATH}` with a path to a compatible
-        (single-channel, 16 kHz, 16-bit PCM) `.wav` file you wish to enhance, and `${WAV_OUTPUT_PATH}` with a path to a `.wav` 
-        file where the enhanced audio will be stored.
-        
 Keywords: Noise Cancellation,Noise Suppression,Noise Removal,Speech Enhancement,Speech Denoising
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
+# Koala Noise Suppression Demos
+
+Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
+
+## Koala
+
+Koala is an on-device noise suppression engine. Koala is:
+
+- Private; All voice processing runs locally.
+- Cross-Platform:
+  - Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64)
+  - Android and iOS
+  - Chrome, Safari, Firefox, and Edge
+  - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
+
+## Compatibility
+
+- Python 3.5+
+- Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
+
+## Installation
+
+```console
+pip3 install pvkoalademo
+```
+
+## AccessKey
+
+Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
+SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
+Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
+
+## Usage
+
+### Microphone Demo
+
+The microphone demo collects audio from a microphone connected to your machine. The audio is passed through the Koala
+noise suppression engine and stored in a `.wav` file.
+Run the following in the terminal:
+
+```console
+koala_demo_mic --access_key ${ACCESS_KEY} --output-path ${WAV_OUTPUT_PATH}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_OUTPUT_PATH}` with a path to a `.wav` file
+where the enhanced audio will be stored. Terminate the demo with `Ctrl+C`.
+
+### File Demo
+
+The file demo passes audio stored in a `.wav` file through the Koala noise suppression engine. The result is shifted to
+compensate for the delay introduced by Koala and stored in a separate `.wav` file that will have the same length as the
+input file without any delay.
+Run the following in the terminal:
+
+```console
+koala_demo_file --access_key ${ACCESS_KEY} --input_path ${WAV_INPUT_PATH} --output_path ${WAV_OUTPUT_PATH}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console, `${WAV_INPUT_PATH}` with a path to a compatible
+(single-channel, 16 kHz, 16-bit PCM) `.wav` file you wish to enhance, and `${WAV_OUTPUT_PATH}` with a path to a `.wav` 
+file where the enhanced audio will be stored.
+
+
```

### Comparing `pvkoalademo-1.0.1/README.md` & `pvkoalademo-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pvkoalademo-1.0.1/pvkoalademo/LICENSE` & `pvkoalademo-1.0.2/pvkoalademo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvkoalademo-1.0.1/pvkoalademo/koala_demo_file.py` & `pvkoalademo-1.0.2/pvkoalademo/koala_demo_file.py`

 * *Files identical despite different names*

### Comparing `pvkoalademo-1.0.1/pvkoalademo/koala_demo_mic.py` & `pvkoalademo-1.0.2/pvkoalademo/koala_demo_mic.py`

 * *Files identical despite different names*

### Comparing `pvkoalademo-1.0.1/pvkoalademo.egg-info/PKG-INFO` & `pvkoalademo-1.0.2/pvkoalademo.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 Metadata-Version: 2.1
 Name: pvkoalademo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Koala Noise Suppression Engine demos
 Home-page: https://github.com/Picovoice/koala
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
-Description: # Koala Noise Suppression Demos
-        
-        Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
-        
-        ## Koala
-        
-        Koala is an on-device noise suppression engine. Koala is:
-        
-        - Private; All voice processing runs locally.
-        - Cross-Platform:
-          - Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64)
-          - Android and iOS
-          - Chrome, Safari, Firefox, and Edge
-          - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
-        
-        ## Compatibility
-        
-        - Python 3.5+
-        - Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
-        
-        ## Installation
-        
-        ```console
-        pip3 install pvkoalademo
-        ```
-        
-        ## AccessKey
-        
-        Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
-        SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
-        Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
-        
-        ## Usage
-        
-        ### Microphone Demo
-        
-        The microphone demo collects audio from a microphone connected to your machine. The audio is passed through the Koala
-        noise suppression engine and stored in a `.wav` file.
-        Run the following in the terminal:
-        
-        ```console
-        koala_demo_mic --access_key ${ACCESS_KEY} --output-path ${WAV_OUTPUT_PATH}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_OUTPUT_PATH}` with a path to a `.wav` file
-        where the enhanced audio will be stored. Terminate the demo with `Ctrl+C`.
-        
-        ### File Demo
-        
-        The file demo passes audio stored in a `.wav` file through the Koala noise suppression engine. The result is shifted to
-        compensate for the delay introduced by Koala and stored in a separate `.wav` file that will have the same length as the
-        input file without any delay.
-        Run the following in the terminal:
-        
-        ```console
-        koala_demo_file --access_key ${ACCESS_KEY} --input_path ${WAV_INPUT_PATH} --output_path ${WAV_OUTPUT_PATH}
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console, `${WAV_INPUT_PATH}` with a path to a compatible
-        (single-channel, 16 kHz, 16-bit PCM) `.wav` file you wish to enhance, and `${WAV_OUTPUT_PATH}` with a path to a `.wav` 
-        file where the enhanced audio will be stored.
-        
 Keywords: Noise Cancellation,Noise Suppression,Noise Removal,Speech Enhancement,Speech Denoising
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
+# Koala Noise Suppression Demos
+
+Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
+
+## Koala
+
+Koala is an on-device noise suppression engine. Koala is:
+
+- Private; All voice processing runs locally.
+- Cross-Platform:
+  - Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64)
+  - Android and iOS
+  - Chrome, Safari, Firefox, and Edge
+  - Raspberry Pi (4, 3) and NVIDIA Jetson Nano
+
+## Compatibility
+
+- Python 3.5+
+- Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
+
+## Installation
+
+```console
+pip3 install pvkoalademo
+```
+
+## AccessKey
+
+Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
+SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
+Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
+
+## Usage
+
+### Microphone Demo
+
+The microphone demo collects audio from a microphone connected to your machine. The audio is passed through the Koala
+noise suppression engine and stored in a `.wav` file.
+Run the following in the terminal:
+
+```console
+koala_demo_mic --access_key ${ACCESS_KEY} --output-path ${WAV_OUTPUT_PATH}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console and `${WAV_OUTPUT_PATH}` with a path to a `.wav` file
+where the enhanced audio will be stored. Terminate the demo with `Ctrl+C`.
+
+### File Demo
+
+The file demo passes audio stored in a `.wav` file through the Koala noise suppression engine. The result is shifted to
+compensate for the delay introduced by Koala and stored in a separate `.wav` file that will have the same length as the
+input file without any delay.
+Run the following in the terminal:
+
+```console
+koala_demo_file --access_key ${ACCESS_KEY} --input_path ${WAV_INPUT_PATH} --output_path ${WAV_OUTPUT_PATH}
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from Picovoice Console, `${WAV_INPUT_PATH}` with a path to a compatible
+(single-channel, 16 kHz, 16-bit PCM) `.wav` file you wish to enhance, and `${WAV_OUTPUT_PATH}` with a path to a `.wav` 
+file where the enhanced audio will be stored.
+
+
```

### Comparing `pvkoalademo-1.0.1/setup.py` & `pvkoalademo-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     f.write(manifest_in)
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvkoalademo",
-    version="1.0.1",
+    version="1.0.2",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Koala Noise Suppression Engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/koala",
     packages=["pvkoalademo"],
-    install_requires=["pvkoala==1.0.0", "pvrecorder==1.1.1"],
+    install_requires=["pvkoala==1.0.1", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

