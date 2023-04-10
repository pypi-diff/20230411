# Comparing `tmp/suta_ble_bed-0.3.0.tar.gz` & `tmp/suta_ble_bed-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suta_ble_bed-0.3.0.tar", last modified: Fri Mar 24 03:14:29 2023, max compression
+gzip compressed data, was "suta_ble_bed-0.3.2.tar", last modified: Mon Apr 10 22:02:19 2023, max compression
```

## Comparing `suta_ble_bed-0.3.0.tar` & `suta_ble_bed-0.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-03-24 03:14:29.499353 suta_ble_bed-0.3.0/
--rw-r--r--   0 simon     (1000) simon     (1002)     3581 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      585 2023-03-24 03:13:31.000000 suta_ble_bed-0.3.0/HISTORY.rst
--rw-r--r--   0 simon     (1000) simon     (1002)     1069 2023-03-04 01:55:36.000000 suta_ble_bed-0.3.0/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1002)      242 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1002)     3345 2023-03-24 03:14:29.499353 suta_ble_bed-0.3.0/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1002)     2005 2023-03-22 00:10:14.000000 suta_ble_bed-0.3.0/README.rst
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-03-24 03:14:29.498353 suta_ble_bed-0.3.0/docs/
--rw-r--r--   0 simon     (1000) simon     (1002)      613 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/Makefile
--rwxr-xr-x   0 simon     (1000) simon     (1002)     4843 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/conf.py
--rw-r--r--   0 simon     (1000) simon     (1002)       33 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/contributing.rst
--rw-r--r--   0 simon     (1000) simon     (1002)       28 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/history.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      298 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/index.rst
--rw-r--r--   0 simon     (1000) simon     (1002)     1150 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/installation.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      810 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/make.bat
--rw-r--r--   0 simon     (1000) simon     (1002)       27 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/readme.rst
--rw-r--r--   0 simon     (1000) simon     (1002)       79 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/docs/usage.rst
--rw-r--r--   0 simon     (1000) simon     (1002)      384 2023-03-24 03:14:29.500353 suta_ble_bed-0.3.0/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1002)     1495 2023-03-24 03:13:54.000000 suta_ble_bed-0.3.0/setup.py
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-03-24 03:14:29.498353 suta_ble_bed-0.3.0/suta_ble_bed/
--rw-r--r--   0 simon     (1000) simon     (1002)      320 2023-03-24 03:13:54.000000 suta_ble_bed-0.3.0/suta_ble_bed/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1002)      234 2023-03-24 02:10:42.000000 suta_ble_bed-0.3.0/suta_ble_bed/__main__.py
--rwxr-xr-x   0 simon     (1000) simon     (1002)     1707 2023-03-24 03:11:51.000000 suta_ble_bed-0.3.0/suta_ble_bed/cli.py
--rw-r--r--   0 simon     (1000) simon     (1002)     6103 2023-03-24 03:14:23.000000 suta_ble_bed-0.3.0/suta_ble_bed/suta_ble_bed.py
--rw-r--r--   0 simon     (1000) simon     (1002)     1366 2023-03-24 03:11:51.000000 suta_ble_bed-0.3.0/suta_ble_bed/suta_ble_bed_controller.py
--rw-r--r--   0 simon     (1000) simon     (1002)     1665 2023-03-04 03:24:35.000000 suta_ble_bed-0.3.0/suta_ble_bed/suta_ble_consts.py
--rw-r--r--   0 simon     (1000) simon     (1002)     1313 2023-03-24 03:11:51.000000 suta_ble_bed-0.3.0/suta_ble_bed/suta_ble_scanner.py
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-03-24 03:14:29.499353 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1002)     3345 2023-03-24 03:14:29.000000 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1002)      728 2023-03-24 03:14:29.000000 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1002)        1 2023-03-24 03:14:29.000000 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1002)       56 2023-03-24 03:14:29.000000 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1002)        1 2023-03-22 00:41:32.000000 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/not-zip-safe
--rw-r--r--   0 simon     (1000) simon     (1002)       43 2023-03-24 03:14:29.000000 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1002)       13 2023-03-24 03:14:29.000000 suta_ble_bed-0.3.0/suta_ble_bed.egg-info/top_level.txt
-drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-03-24 03:14:29.499353 suta_ble_bed-0.3.0/tests/
--rw-r--r--   0 simon     (1000) simon     (1002)       42 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/tests/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1002)      412 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.0/tests/test_suta_ble_bed.py
+drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/
+-rw-r--r--   0 simon     (1000) simon     (1002)     3581 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)      888 2023-04-10 21:50:37.000000 suta_ble_bed-0.3.2/HISTORY.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)     1069 2023-03-04 01:55:36.000000 suta_ble_bed-0.3.2/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1002)      242 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1002)     3919 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1002)     2239 2023-04-10 22:02:04.000000 suta_ble_bed-0.3.2/README.rst
+drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.228831 suta_ble_bed-0.3.2/docs/
+-rw-r--r--   0 simon     (1000) simon     (1002)      613 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/Makefile
+-rwxr-xr-x   0 simon     (1000) simon     (1002)     4843 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/conf.py
+-rw-r--r--   0 simon     (1000) simon     (1002)       33 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/contributing.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)       28 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/history.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)      298 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/index.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)     1150 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/installation.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)      810 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/make.bat
+-rw-r--r--   0 simon     (1000) simon     (1002)       27 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/readme.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)       79 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/docs/usage.rst
+-rw-r--r--   0 simon     (1000) simon     (1002)      384 2023-04-10 22:02:19.231831 suta_ble_bed-0.3.2/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1002)     1543 2023-04-10 22:00:37.000000 suta_ble_bed-0.3.2/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.229831 suta_ble_bed-0.3.2/suta_ble_bed/
+-rw-r--r--   0 simon     (1000) simon     (1002)      320 2023-04-10 21:47:02.000000 suta_ble_bed-0.3.2/suta_ble_bed/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1002)      234 2023-03-24 02:10:42.000000 suta_ble_bed-0.3.2/suta_ble_bed/__main__.py
+-rwxr-xr-x   0 simon     (1000) simon     (1002)     1727 2023-04-10 21:43:38.000000 suta_ble_bed-0.3.2/suta_ble_bed/cli.py
+-rw-r--r--   0 simon     (1000) simon     (1002)     4199 2023-04-10 21:43:38.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_bed.py
+-rw-r--r--   0 simon     (1000) simon     (1002)     3219 2023-03-24 21:42:50.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_bed_controller.py
+-rw-r--r--   0 simon     (1000) simon     (1002)     1656 2023-03-24 21:25:34.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_consts.py
+-rw-r--r--   0 simon     (1000) simon     (1002)     1322 2023-03-24 20:28:13.000000 suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_scanner.py
+drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1002)     3919 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1002)      728 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1002)        1 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1002)       56 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1002)        1 2023-03-22 00:41:32.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/not-zip-safe
+-rw-r--r--   0 simon     (1000) simon     (1002)       43 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1002)       13 2023-04-10 22:02:19.000000 suta_ble_bed-0.3.2/suta_ble_bed.egg-info/top_level.txt
+drwxr-xr-x   0 simon     (1000) simon     (1002)        0 2023-04-10 22:02:19.230831 suta_ble_bed-0.3.2/tests/
+-rw-r--r--   0 simon     (1000) simon     (1002)       42 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/tests/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1002)      412 2023-03-22 00:00:51.000000 suta_ble_bed-0.3.2/tests/test_suta_ble_bed.py
```

### Comparing `suta_ble_bed-0.3.0/CONTRIBUTING.rst` & `suta_ble_bed-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.0/HISTORY.rst` & `suta_ble_bed-0.3.2/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 =======
 History
 =======
 
-0.3.0 (2023-030-23)
+0.3.2 (2023-04-10)
+------------------
+* Fix disconnect callback
+* Correct comment on BLE characteristics
+
+0.3.1 (2023-03-23)
+------------------
+* Fix connection handling with Controller interface
+* Fix CLI in case MAC is not provided
+* Pass correct parameter when constructing SutaBleBed under callback
+
+0.3.0 (2023-03-23)
 -------------------
 
 * Change to Controller interface
 * Fix copy-paste errors
 * Add "is_connected" helper
 
 0.2.0 (2023-03-21)
```

### Comparing `suta_ble_bed-0.3.0/LICENSE` & `suta_ble_bed-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.0/PKG-INFO` & `suta_ble_bed-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suta_ble_bed
-Version: 0.3.0
+Version: 0.3.2
 Summary: Handle BLE communications for a SUTA bed frame such as the i500 or i800.
 Home-page: https://github.com/sredman/suta_ble_bed
 Author: Simon Redman
 Author-email: simon@ergotech.com
 License: MIT license
 Keywords: SUTA,sleepmotion,i500,i900,i200
 Platform: UNKNOWN
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 SUTA BLE Bed
 ============
 
 
@@ -60,46 +61,61 @@
 --------
 
 * TODO
 
 Usage
 --------
 
-```
-device = await suta_scanner.discover()[0]
-bed = BleSutaBed(device)
-await bed.raise_feet()
-```
+.. code-block:: python
+
+    async with SutaBleBedController() as controller:
+      async for bed in controller.devices():
+        await bed.raise_feet()
+        break
+
+Note that the `async for` will return a result each time the advertising data changes,
+which includes any time the signal strength changes.
 
 or
 
-```
-./suta_ble_bed_cli.py raise-feet
-```
+.. code-block:: sh
+
+   python -m suta_ble_bed --MAC=AA:BB:CC:DD:EE:FF head-down
 
 Credits
 -------
 
 This module would not have been possible without the research done by stevendodd on Github:
 https://github.com/stevendodd/sleepmotion-ble/blob/main/pi-zero/sleepmotion-ble.py
 
-Code structure inspirired by:
+Inspirired by:
 https://github.com/sopelj/python-ember-mug/blob/main/ember_mug/mug.py
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.3.0 (2023-030-23)
+0.3.2 (2023-04-10)
+------------------
+* Fix disconnect callback
+* Correct comment on BLE characteristics
+
+0.3.1 (2023-03-23)
+------------------
+* Fix connection handling with Controller interface
+* Fix CLI in case MAC is not provided
+* Pass correct parameter when constructing SutaBleBed under callback
+
+0.3.0 (2023-03-23)
 -------------------
 
 * Change to Controller interface
 * Fix copy-paste errors
 * Add "is_connected" helper
 
 0.2.0 (2023-03-21)
```

### Comparing `suta_ble_bed-0.3.0/README.rst` & `suta_ble_bed-0.3.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -39,32 +39,36 @@
 --------
 
 * TODO
 
 Usage
 --------
 
-```
-device = await suta_scanner.discover()[0]
-bed = BleSutaBed(device)
-await bed.raise_feet()
-```
+.. code-block:: python
+
+    async with SutaBleBedController() as controller:
+      async for bed in controller.devices():
+        await bed.raise_feet()
+        break
+
+Note that the `async for` will return a result each time the advertising data changes,
+which includes any time the signal strength changes.
 
 or
 
-```
-./suta_ble_bed_cli.py raise-feet
-```
+.. code-block:: sh
+
+   python -m suta_ble_bed --MAC=AA:BB:CC:DD:EE:FF head-down
 
 Credits
 -------
 
 This module would not have been possible without the research done by stevendodd on Github:
 https://github.com/stevendodd/sleepmotion-ble/blob/main/pi-zero/sleepmotion-ble.py
 
-Code structure inspirired by:
+Inspirired by:
 https://github.com/sopelj/python-ember-mug/blob/main/ember_mug/mug.py
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `suta_ble_bed-0.3.0/docs/Makefile` & `suta_ble_bed-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.0/docs/conf.py` & `suta_ble_bed-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.0/docs/installation.rst` & `suta_ble_bed-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.0/docs/make.bat` & `suta_ble_bed-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `suta_ble_bed-0.3.0/setup.py` & `suta_ble_bed-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,18 @@
         'console_scripts': [
             'suta_ble_bed=suta_ble_bed.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
+    long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords=['SUTA','sleepmotion','i500','i900','i200'],
     name='suta_ble_bed',
     packages=find_packages(include=['suta_ble_bed', 'suta_ble_bed.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/sredman/suta_ble_bed',
-    version='0.3.0',
+    version='0.3.2',
     zip_safe=False,
 )
```

### Comparing `suta_ble_bed-0.3.0/suta_ble_bed/cli.py` & `suta_ble_bed-0.3.2/suta_ble_bed/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 async def worker(args: Namespace):
 
     async with SutaBleBedController() as controller:
         async for bed in controller.devices():
             logger.info(f"Discovered {bed.device}")
 
-            if (bed.device.address == args.MAC):
+            if (args.MAC is None or bed.device.address == args.MAC):
                 match args.command:
                     case "feet-up":
                         await bed.raise_feet()
                     case "feet-down":
                         await bed.lower_feet()
                     case "head-up":
                         await bed.raise_head()
```

### Comparing `suta_ble_bed-0.3.0/suta_ble_bed/suta_ble_bed.py` & `suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_bed.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,40 +22,43 @@
 
 import asyncio
 import contextlib
 
 from bleak import BleakClient, BleakError, BleakScanner
 from bleak.backends.characteristic import BleakGATTCharacteristic
 from bleak.backends.device import BLEDevice
-from bleak_retry_connector import establish_connection
 
 from collections.abc import AsyncIterator
+import typing
 from typing import Any, Callable, Literal
 import logging
 
+if typing.TYPE_CHECKING:
+    from .suta_ble_bed_controller import SutaBleBedController
+
 from .suta_ble_consts import BedServices, BedCommands, BedCharacteristic
 
 logger = logging.getLogger(__name__)
 
 class BleSutaBed:
 
     def __init__(
         self,
         ble_device: BLEDevice,
-        controller,
+        controller: SutaBleBedController,
         **kwargs: Any,
     ) -> None:
         """
         Constructor
 
         @param ble_device: The bleak.BLEDevice which represents the connection to the bed
         @param controller: The SutaBleBedController which controls this connection
         """
         self.device = ble_device
-        self.controller = controller
+        self.controller: SutaBleBedController = controller
 
         self._client: BleakClient = None  # type: ignore[assignment]
         self._connect_lock = asyncio.Lock()
         self._operation_lock = asyncio.Lock()
         self._expected_disconnect = False
 
     def is_connected(self) -> bool:
@@ -102,51 +105,10 @@
         """Connect to bed."""
         if self._connect_lock.locked():
             logger.debug("Connection to %s already in progress. Waiting first.", self.device.name)
 
         if self.is_connected():
             return
 
-        async with self._connect_lock:
-            # Also check after lock is acquired
-            if self.is_connected:
-                return
-            try:
-                logger.debug(f"Connecting to {self.device}")
-                async with BleakScanner():
-                    # Need to have the scanner running in order for Bluez to populate the device
-                    client = await establish_connection(
-                        client_class=BleakClient,
-                        device=self.device,
-                        name=f'{self.device.name} ({self.device.address})',
-                        use_services_cache=True,
-                        disconnected_callback=self._disconnect_callback,  # type: ignore
-                        ble_device_callback=lambda: self.device,
-                    )
-                    self._expected_disconnect = False
-                    self._client = client
-            except (asyncio.TimeoutError, BleakError) as error:
-                logger.error("%s: Failed to connect to the bed: %s", self.device, error)
-                raise
+        self._client = await self.controller.connect(self)
+        self._expected_disconnect = False
         return
-
-    def _disconnect_callback(self, client: BleakClient) -> None:
-        """Disconnect from device."""
-        if self._expected_disconnect:
-            logger.debug("Disconnect callback called")
-        else:
-            logger.warning("Unexpectedly disconnected")
-
-    def set_client_options(self, **kwargs: str) -> None:
-        """Update options in case they need to overriden in some cases."""
-        if kwargs.get('adapter') and IS_LINUX is False:
-            raise ValueError('The adapter option is only valid for the Linux BlueZ Backend.')
-        self._client_kwargs = {**kwargs}
-
-    @contextlib.asynccontextmanager
-    async def connection(self, **kwargs: str) -> AsyncIterator[BleSutaBed]:
-        """Helper for establishing a connection and automatically closing it."""
-        self.set_client_options(**kwargs)
-        # This will happen automatically, but calling it now will give us immediate feedback
-        await self._ensure_connection()
-        yield self
-        await self.disconnect()
```

### Comparing `suta_ble_bed-0.3.0/suta_ble_bed/suta_ble_consts.py` & `suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     CONTROL = '0000fee9-0000-1000-8000-00805f9b34fb' # Control the bed
     ACK_CMD = '0000ffe0-0000-1000-8000-00805f9b34fb' # I don't know what this is
     UPDATE = '00010203-0405-0607-0809-0a0b0c0d1912' # I can guess what this is, best not to mess with it
 
 # Characteristics exposed by the bed
 class BedCharacteristic(Enum):
     CONTROL_COMMAND = 'd44bc439-abfd-45a2-b575-925416129600' # Send commands here - Write
-    CONTROL_READ = 'd44bc439-abfd-45a2-b575-925416129601' # Read the current state here. Read/Notify
-    ACK_CMD_ACK = '0000ffe1-0000-1000-8000-00805f9b34fb' # "ACK OutPut" - Read/Notify
+    CONTROL_READ = 'd44bc439-abfd-45a2-b575-925416129601' # Read the current state here - Notify
+    ACK_CMD_ACK = '0000ffe1-0000-1000-8000-00805f9b34fb' # "ACK OutPut" - Notify
     ACK_CMD_CMD = '0000ffe2-0000-1000-8000-00805f9b34fb' # "CMD Input" - Write
     UPDATE_OTA = '00010203-0405-0607-0809-0a0b0c0d2b12' # Brick your bed here - Write
 
 class BedCommands(IntEnum):
     '''
     These were reverse engineered and documented in
     https://github.com/stevendodd/sleepmotion-ble/blob/main/pi-zero/sleepmotion-ble.py
```

### Comparing `suta_ble_bed-0.3.0/suta_ble_bed/suta_ble_scanner.py` & `suta_ble_bed-0.3.2/suta_ble_bed/suta_ble_scanner.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from typing import Any
 
 from .suta_ble_bed import BleSutaBed
 from .suta_ble_consts import BedCharacteristic, IS_LINUX, BED_LOCAL_NAME
 
 class SutaBleScanner():
 
-    def __init__(self) -> None:
-        self.scanner_running_lock = asyncio.Lock()
+    def __init__(self, controller) -> None:
+        self.controller = controller
 
         self._new_devices = asyncio.Queue()
 
         self._tasks = set()
 
     def __aiter__(self):
         return self
@@ -34,8 +34,8 @@
     def _scanner_discovery_callback(self, device: BLEDevice, advertising_data: AdvertisementData) -> None:
         task = asyncio.create_task(self._scanner_discovery_callback_int(device, advertising_data))
         self._tasks.add(task)
         task.add_done_callback(self._tasks.discard)
 
     async def _scanner_discovery_callback_int(self, device: BLEDevice, advertising_data: AdvertisementData) -> None:
         if advertising_data.local_name == BED_LOCAL_NAME:
-            await self._new_devices.put(BleSutaBed(device, self))
+            await self._new_devices.put(BleSutaBed(device, self.controller))
```

### Comparing `suta_ble_bed-0.3.0/suta_ble_bed.egg-info/PKG-INFO` & `suta_ble_bed-0.3.2/suta_ble_bed.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suta-ble-bed
-Version: 0.3.0
+Version: 0.3.2
 Summary: Handle BLE communications for a SUTA bed frame such as the i500 or i800.
 Home-page: https://github.com/sredman/suta_ble_bed
 Author: Simon Redman
 Author-email: simon@ergotech.com
 License: MIT license
 Keywords: SUTA,sleepmotion,i500,i900,i200
 Platform: UNKNOWN
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 SUTA BLE Bed
 ============
 
 
@@ -60,46 +61,61 @@
 --------
 
 * TODO
 
 Usage
 --------
 
-```
-device = await suta_scanner.discover()[0]
-bed = BleSutaBed(device)
-await bed.raise_feet()
-```
+.. code-block:: python
+
+    async with SutaBleBedController() as controller:
+      async for bed in controller.devices():
+        await bed.raise_feet()
+        break
+
+Note that the `async for` will return a result each time the advertising data changes,
+which includes any time the signal strength changes.
 
 or
 
-```
-./suta_ble_bed_cli.py raise-feet
-```
+.. code-block:: sh
+
+   python -m suta_ble_bed --MAC=AA:BB:CC:DD:EE:FF head-down
 
 Credits
 -------
 
 This module would not have been possible without the research done by stevendodd on Github:
 https://github.com/stevendodd/sleepmotion-ble/blob/main/pi-zero/sleepmotion-ble.py
 
-Code structure inspirired by:
+Inspirired by:
 https://github.com/sopelj/python-ember-mug/blob/main/ember_mug/mug.py
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.3.0 (2023-030-23)
+0.3.2 (2023-04-10)
+------------------
+* Fix disconnect callback
+* Correct comment on BLE characteristics
+
+0.3.1 (2023-03-23)
+------------------
+* Fix connection handling with Controller interface
+* Fix CLI in case MAC is not provided
+* Pass correct parameter when constructing SutaBleBed under callback
+
+0.3.0 (2023-03-23)
 -------------------
 
 * Change to Controller interface
 * Fix copy-paste errors
 * Add "is_connected" helper
 
 0.2.0 (2023-03-21)
```

### Comparing `suta_ble_bed-0.3.0/suta_ble_bed.egg-info/SOURCES.txt` & `suta_ble_bed-0.3.2/suta_ble_bed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

