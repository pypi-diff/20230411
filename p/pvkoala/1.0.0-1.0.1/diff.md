# Comparing `tmp/pvkoala-1.0.0.tar.gz` & `tmp/pvkoala-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvkoala-1.0.0.tar", last modified: Tue Feb  7 01:16:33 2023, max compression
+gzip compressed data, was "pvkoala-1.0.1.tar", last modified: Tue Apr 11 00:43:02 2023, max compression
```

## Comparing `pvkoala-1.0.0.tar` & `pvkoala-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/
--rw-rw-r--   0 nash      (1000) nash      (1000)      164 2023-02-07 01:16:33.000000 pvkoala-1.0.0/MANIFEST.in
--rw-rw-r--   0 nash      (1000) nash      (1000)     3284 2023-02-07 01:16:33.922816 pvkoala-1.0.0/PKG-INFO
--rw-rw-r--   0 nash      (1000) nash      (1000)     2083 2023-02-06 19:53:23.000000 pvkoala-1.0.0/README.md
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala/
--rw-rw-r--   0 nash      (1000) nash      (1000)    11357 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala/LICENSE
--rw-rw-r--   0 nash      (1000) nash      (1000)      570 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala/__init__.py
--rw-rw-r--   0 nash      (1000) nash      (1000)     1458 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala/_factory.py
--rw-rw-r--   0 nash      (1000) nash      (1000)     8370 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala/_koala.py
--rw-rw-r--   0 nash      (1000) nash      (1000)     3083 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala/_util.py
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala/lib/
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.918816 pvkoala-1.0.0/pvkoala/lib/common/
--rw-rw-r--   0 nash      (1000) nash      (1000)  4007735 2023-02-03 00:35:17.000000 pvkoala-1.0.0/pvkoala/lib/common/koala_params.pv
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala/lib/jetson/
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/jetson/cortex-a57-aarch64/
--rwxrwxr-x   0 nash      (1000) nash      (1000)   133600 2023-02-03 00:26:36.000000 pvkoala-1.0.0/pvkoala/lib/jetson/cortex-a57-aarch64/libpv_koala.so
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala/lib/linux/
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/linux/x86_64/
--rwxr-xr-x   0 nash      (1000) nash      (1000)   150352 2023-02-02 22:07:53.000000 pvkoala-1.0.0/pvkoala/lib/linux/x86_64/libpv_koala.so
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala/lib/mac/
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/mac/arm64/
--rwxr-xr-x   0 nash      (1000) nash      (1000)   203166 2023-02-02 22:07:57.000000 pvkoala-1.0.0/pvkoala/lib/mac/arm64/libpv_koala.dylib
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/mac/x86_64/
--rwxr-xr-x   0 nash      (1000) nash      (1000)   217912 2023-02-02 22:07:57.000000 pvkoala-1.0.0/pvkoala/lib/mac/x86_64/libpv_koala.dylib
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a53/
--rwxr-xr-x   0 nash      (1000) nash      (1000)   120620 2023-02-02 22:08:00.000000 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a53/libpv_koala.so
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a53-aarch64/
--rwxr-xr-x   0 nash      (1000) nash      (1000)   133688 2023-02-02 22:08:01.000000 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a53-aarch64/libpv_koala.so
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a72/
--rwxr-xr-x   0 nash      (1000) nash      (1000)   124716 2023-02-02 22:08:01.000000 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a72/libpv_koala.so
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a72-aarch64/
--rwxr-xr-x   0 nash      (1000) nash      (1000)   133688 2023-02-02 22:08:02.000000 pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a72-aarch64/libpv_koala.so
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala/lib/windows/
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.922816 pvkoala-1.0.0/pvkoala/lib/windows/amd64/
--rw-rw-rw-   0 nash      (1000) nash      (1000)   303104 2023-02-02 19:43:50.000000 pvkoala-1.0.0/pvkoala/lib/windows/amd64/libpv_koala.dll
-drwxrwxr-x   0 nash      (1000) nash      (1000)        0 2023-02-07 01:16:33.914816 pvkoala-1.0.0/pvkoala.egg-info/
--rw-rw-r--   0 nash      (1000) nash      (1000)     3284 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala.egg-info/PKG-INFO
--rw-rw-r--   0 nash      (1000) nash      (1000)      716 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala.egg-info/SOURCES.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)        1 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala.egg-info/dependency_links.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)        8 2023-02-07 01:16:33.000000 pvkoala-1.0.0/pvkoala.egg-info/top_level.txt
--rw-rw-r--   0 nash      (1000) nash      (1000)       38 2023-02-07 01:16:33.922816 pvkoala-1.0.0/setup.cfg
--rw-rw-r--   0 nash      (1000) nash      (1000)     2367 2023-02-04 01:23:05.000000 pvkoala-1.0.0/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.743717 pvkoala-1.0.1/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      164 2023-04-11 00:43:02.000000 pvkoala-1.0.1/MANIFEST.in
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2785 2023-04-11 00:43:02.743717 pvkoala-1.0.1/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2083 2023-02-07 23:09:03.000000 pvkoala-1.0.1/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/
+-rw-rw-r--   0 eric      (1000) eric      (1000)    11357 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)      570 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1458 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala/_factory.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8370 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala/_koala.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3135 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala/_util.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)  4007735 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/common/koala_params.pv
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/jetson/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/jetson/cortex-a57-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   133600 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/jetson/cortex-a57-aarch64/libpv_koala.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/linux/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/linux/x86_64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   150352 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/linux/x86_64/libpv_koala.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/mac/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/mac/arm64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   203166 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/mac/arm64/libpv_koala.dylib
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.743717 pvkoala-1.0.1/pvkoala/lib/mac/x86_64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   217912 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/mac/x86_64/libpv_koala.dylib
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.743717 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a53/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   120620 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a53/libpv_koala.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.743717 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a53-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   133688 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a53-aarch64/libpv_koala.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.743717 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a72/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   124716 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a72/libpv_koala.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.743717 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a72-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   133688 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a72-aarch64/libpv_koala.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala/lib/windows/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.743717 pvkoala-1.0.1/pvkoala/lib/windows/amd64/
+-rw-rw-r--   0 eric      (1000) eric      (1000)   303104 2023-02-07 23:09:03.000000 pvkoala-1.0.1/pvkoala/lib/windows/amd64/libpv_koala.dll
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:02.739716 pvkoala-1.0.1/pvkoala.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2785 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      716 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        8 2023-04-11 00:43:02.000000 pvkoala-1.0.1/pvkoala.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-04-11 00:43:02.743717 pvkoala-1.0.1/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2367 2023-04-10 21:21:46.000000 pvkoala-1.0.1/setup.py
```

### Comparing `pvkoala-1.0.0/PKG-INFO` & `pvkoala-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 Metadata-Version: 2.1
 Name: pvkoala
-Version: 1.0.0
+Version: 1.0.1
 Summary: Koala Noise Suppression Engine.
 Home-page: https://github.com/Picovoice/koala
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
-Description: # Koala Noise Suppression Engine
-        
-        Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
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
-        - Python 3.5 or higher
-        - Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
-        
-        ## Installation
-        
-        ```console
-        pip3 install pvkoala
-        ```
-        
-        ## AccessKey
-        
-        Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
-        SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
-        Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
-        
-        ### Usage
-        
-        Create an instance of the engine and enhance audio:
-        
-        ```python
-        import pvkoala
-        
-        koala = pvkoala.create(access_key='${ACCESS_KEY}')
-        
-        def get_next_audio_frame():
-            pass
-        
-        while True:
-            enhanced_audio = koala.process(get_next_audio_frame())
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from [Picovoice Console](https://console.picovoice.ai/). 
-        The input audio must come from a single-channel stream with integer 16-bit encoding. The sample rate must be identical
-        to `koala.sample_rate`. The stream must be split into *frames* with a fixed length in samples that can be obtained 
-        from `koala.frame_length`.
-        
-        The output of `koala.process()` is a frame of enhanced audio with the same 16-bit integer encoding. The delay in 
-        samples between the start time of the input frame and the start time of the output frame can be attained from 
-        `koala.delay_sample`.
-        
-        In case the next audio frame does not directly follow the previous one, call `koala.reset()`.
-        When done be sure to explicitly release the resources using `koala.delete()`.
-        
-        ## Demos
-        
-        [pvkoalademo](https://pypi.org/project/pvkoalademo/) provides command-line utilities for processing audio using Koala.
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
+# Koala Noise Suppression Engine
+
+Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
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
+- Python 3.5 or higher
+- Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
+
+## Installation
+
+```console
+pip3 install pvkoala
+```
+
+## AccessKey
+
+Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
+SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
+Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
+
+### Usage
+
+Create an instance of the engine and enhance audio:
+
+```python
+import pvkoala
+
+koala = pvkoala.create(access_key='${ACCESS_KEY}')
+
+def get_next_audio_frame():
+    pass
+
+while True:
+    enhanced_audio = koala.process(get_next_audio_frame())
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from [Picovoice Console](https://console.picovoice.ai/). 
+The input audio must come from a single-channel stream with integer 16-bit encoding. The sample rate must be identical
+to `koala.sample_rate`. The stream must be split into *frames* with a fixed length in samples that can be obtained 
+from `koala.frame_length`.
+
+The output of `koala.process()` is a frame of enhanced audio with the same 16-bit integer encoding. The delay in 
+samples between the start time of the input frame and the start time of the output frame can be attained from 
+`koala.delay_sample`.
+
+In case the next audio frame does not directly follow the previous one, call `koala.reset()`.
+When done be sure to explicitly release the resources using `koala.delete()`.
+
+## Demos
+
+[pvkoalademo](https://pypi.org/project/pvkoalademo/) provides command-line utilities for processing audio using Koala.
+
+
```

### Comparing `pvkoala-1.0.0/README.md` & `pvkoala-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/LICENSE` & `pvkoala-1.0.1/pvkoala/LICENSE`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/__init__.py` & `pvkoala-1.0.1/pvkoala/__init__.py`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/_factory.py` & `pvkoala-1.0.1/pvkoala/_factory.py`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/_koala.py` & `pvkoala-1.0.1/pvkoala/_koala.py`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/_util.py` & `pvkoala-1.0.1/pvkoala/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 #
 
 import os
 import platform
 import subprocess
 
 
+def _is_64bit():
+    return '64bit' in platform.architecture()[0]
+
+
 def _linux_machine() -> str:
     machine = platform.machine()
     if machine == 'x86_64':
         return machine
-    elif machine == 'aarch64':
-        arch_info = '-' + machine
-    elif machine == 'armv7l':
-        arch_info = ''
+    elif machine in ['aarch64', 'armv7l']:
+        arch_info = ('-' + machine) if _is_64bit() else ''
     else:
         raise NotImplementedError("Unsupported CPU architecture: `%s`" % machine)
 
     cpu_info = ''
     try:
         cpu_info = subprocess.check_output(['cat', '/proc/cpuinfo']).decode('utf-8')
         cpu_part_list = [x for x in cpu_info.split('\n') if 'CPU part' in x]
```

### Comparing `pvkoala-1.0.0/pvkoala/lib/common/koala_params.pv` & `pvkoala-1.0.1/pvkoala/lib/common/koala_params.pv`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/jetson/cortex-a57-aarch64/libpv_koala.so` & `pvkoala-1.0.1/pvkoala/lib/jetson/cortex-a57-aarch64/libpv_koala.so`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/linux/x86_64/libpv_koala.so` & `pvkoala-1.0.1/pvkoala/lib/linux/x86_64/libpv_koala.so`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/mac/arm64/libpv_koala.dylib` & `pvkoala-1.0.1/pvkoala/lib/mac/arm64/libpv_koala.dylib`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/mac/x86_64/libpv_koala.dylib` & `pvkoala-1.0.1/pvkoala/lib/mac/x86_64/libpv_koala.dylib`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a53/libpv_koala.so` & `pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a53/libpv_koala.so`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a53-aarch64/libpv_koala.so` & `pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a53-aarch64/libpv_koala.so`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a72/libpv_koala.so` & `pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a72/libpv_koala.so`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/raspberry-pi/cortex-a72-aarch64/libpv_koala.so` & `pvkoala-1.0.1/pvkoala/lib/raspberry-pi/cortex-a72-aarch64/libpv_koala.so`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala/lib/windows/amd64/libpv_koala.dll` & `pvkoala-1.0.1/pvkoala/lib/windows/amd64/libpv_koala.dll`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/pvkoala.egg-info/PKG-INFO` & `pvkoala-1.0.1/pvkoala.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 Metadata-Version: 2.1
 Name: pvkoala
-Version: 1.0.0
+Version: 1.0.1
 Summary: Koala Noise Suppression Engine.
 Home-page: https://github.com/Picovoice/koala
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
-Description: # Koala Noise Suppression Engine
-        
-        Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
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
-        - Python 3.5 or higher
-        - Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
-        
-        ## Installation
-        
-        ```console
-        pip3 install pvkoala
-        ```
-        
-        ## AccessKey
-        
-        Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
-        SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
-        Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
-        
-        ### Usage
-        
-        Create an instance of the engine and enhance audio:
-        
-        ```python
-        import pvkoala
-        
-        koala = pvkoala.create(access_key='${ACCESS_KEY}')
-        
-        def get_next_audio_frame():
-            pass
-        
-        while True:
-            enhanced_audio = koala.process(get_next_audio_frame())
-        ```
-        
-        Replace `${ACCESS_KEY}` with yours obtained from [Picovoice Console](https://console.picovoice.ai/). 
-        The input audio must come from a single-channel stream with integer 16-bit encoding. The sample rate must be identical
-        to `koala.sample_rate`. The stream must be split into *frames* with a fixed length in samples that can be obtained 
-        from `koala.frame_length`.
-        
-        The output of `koala.process()` is a frame of enhanced audio with the same 16-bit integer encoding. The delay in 
-        samples between the start time of the input frame and the start time of the output frame can be attained from 
-        `koala.delay_sample`.
-        
-        In case the next audio frame does not directly follow the previous one, call `koala.reset()`.
-        When done be sure to explicitly release the resources using `koala.delete()`.
-        
-        ## Demos
-        
-        [pvkoalademo](https://pypi.org/project/pvkoalademo/) provides command-line utilities for processing audio using Koala.
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
+# Koala Noise Suppression Engine
+
+Made in Vancouver, Canada by [Picovoice](https://picovoice.ai)
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
+- Python 3.5 or higher
+- Runs on Linux (x86_64), macOS (x86_64, arm64), Windows (x86_64), Raspberry Pi (4, 3), and NVIDIA Jetson Nano.
+
+## Installation
+
+```console
+pip3 install pvkoala
+```
+
+## AccessKey
+
+Koala requires a valid Picovoice `AccessKey` at initialization. `AccessKey` acts as your credentials when using Koala 
+SDKs. You can get your `AccessKey` for free. Make sure to keep your `AccessKey` secret.
+Signup or Login to [Picovoice Console](https://console.picovoice.ai/) to get your `AccessKey`.
+
+### Usage
+
+Create an instance of the engine and enhance audio:
+
+```python
+import pvkoala
+
+koala = pvkoala.create(access_key='${ACCESS_KEY}')
+
+def get_next_audio_frame():
+    pass
+
+while True:
+    enhanced_audio = koala.process(get_next_audio_frame())
+```
+
+Replace `${ACCESS_KEY}` with yours obtained from [Picovoice Console](https://console.picovoice.ai/). 
+The input audio must come from a single-channel stream with integer 16-bit encoding. The sample rate must be identical
+to `koala.sample_rate`. The stream must be split into *frames* with a fixed length in samples that can be obtained 
+from `koala.frame_length`.
+
+The output of `koala.process()` is a frame of enhanced audio with the same 16-bit integer encoding. The delay in 
+samples between the start time of the input frame and the start time of the output frame can be attained from 
+`koala.delay_sample`.
+
+In case the next audio frame does not directly follow the previous one, call `koala.reset()`.
+When done be sure to explicitly release the resources using `koala.delete()`.
+
+## Demos
+
+[pvkoalademo](https://pypi.org/project/pvkoalademo/) provides command-line utilities for processing audio using Koala.
+
+
```

### Comparing `pvkoala-1.0.0/pvkoala.egg-info/SOURCES.txt` & `pvkoala-1.0.1/pvkoala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pvkoala-1.0.0/setup.py` & `pvkoala-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     f.write(manifest_in)
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvkoala",
-    version="1.0.0",
+    version="1.0.1",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Koala Noise Suppression Engine.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/koala",
     packages=["pvkoala"],
```

