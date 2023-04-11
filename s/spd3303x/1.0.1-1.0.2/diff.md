# Comparing `tmp/spd3303x-1.0.1.tar.gz` & `tmp/spd3303x-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spd3303x-1.0.1.tar", last modified: Sun Sep 25 16:56:11 2022, max compression
+gzip compressed data, was "spd3303x-1.0.2.tar", last modified: Tue Apr 11 07:01:11 2023, max compression
```

## Comparing `spd3303x-1.0.1.tar` & `spd3303x-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:56:11.701096 spd3303x-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-09-25 16:56:02.000000 spd3303x-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-09-25 16:56:11.701096 spd3303x-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-09-25 16:56:02.000000 spd3303x-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-25 16:56:11.701096 spd3303x-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-09-25 16:56:02.000000 spd3303x-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:56:11.701096 spd3303x-1.0.1/spd3303x/
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2022-09-25 16:56:02.000000 spd3303x-1.0.1/spd3303x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-09-25 16:56:02.000000 spd3303x-1.0.1/spd3303x/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 16:56:11.701096 spd3303x-1.0.1/spd3303x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-09-25 16:56:11.000000 spd3303x-1.0.1/spd3303x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-25 16:56:11.000000 spd3303x-1.0.1/spd3303x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 16:56:11.000000 spd3303x-1.0.1/spd3303x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-25 16:56:11.000000 spd3303x-1.0.1/spd3303x.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-25 16:56:11.000000 spd3303x-1.0.1/spd3303x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-25 16:56:11.000000 spd3303x-1.0.1/spd3303x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:01:11.949669 spd3303x-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 07:00:52.000000 spd3303x-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-11 07:01:11.949669 spd3303x-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-11 07:00:52.000000 spd3303x-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 07:00:52.000000 spd3303x-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-11 07:01:11.949669 spd3303x-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 07:00:52.000000 spd3303x-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:01:11.949669 spd3303x-1.0.2/spd3303x/
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-11 07:00:52.000000 spd3303x-1.0.2/spd3303x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-11 07:00:52.000000 spd3303x-1.0.2/spd3303x/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:01:11.949669 spd3303x-1.0.2/spd3303x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-11 07:01:11.000000 spd3303x-1.0.2/spd3303x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-11 07:01:11.000000 spd3303x-1.0.2/spd3303x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:01:11.000000 spd3303x-1.0.2/spd3303x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 07:01:11.000000 spd3303x-1.0.2/spd3303x.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 07:01:11.000000 spd3303x-1.0.2/spd3303x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 07:01:11.000000 spd3303x-1.0.2/spd3303x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:01:11.949669 spd3303x-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-11 07:00:52.000000 spd3303x-1.0.2/tests/test_api.py
```

### Comparing `spd3303x-1.0.1/LICENSE` & `spd3303x-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spd3303x-1.0.1/PKG-INFO` & `spd3303x-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spd3303x
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API for SigLent SPD3303X
 Author: Kai Geissdoerfer
 Author-email: kai.geissdoerfer@tu-dresden.de
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spd3303x-1.0.1/README.md` & `spd3303x-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spd3303x-1.0.1/setup.py` & `spd3303x-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
-requirements = ["numpy", "pyvisa-py", "click", "python-vxi11"]
+requirements = ["numpy", "pyvisa-py", "click", "python-vxi11", "zeroconf", "psutil"]
 
 setup(
     name="spd3303x",
-    version="1.0.1",
+    version="1.0.2",
     description="Python API for SigLent SPD3303X",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=["spd3303x"],
     license="MIT",
     classifiers=[
         # How mature is this project? Common values are
```

### Comparing `spd3303x-1.0.1/spd3303x/__init__.py` & `spd3303x-1.0.2/spd3303x/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 import vxi11
 
 consoleHandler = logging.StreamHandler()
 logger = logging.getLogger("spd3303x")
 logger.addHandler(consoleHandler)
 logger.setLevel(logging.DEBUG)
 
-class SPD3303X(object):
 
+class SPD3303X(object):
     KNOWN_MODELS = [
         "SPD3303X",
         "SPD3303X-E",
         "SPD3XIDD5R7170",
+        "NPD3XHBC4R0026",
     ]
 
     MANUFACTURERS = {
         "SPD3303X": "Siglent",
         "SPD3303X-E": "Siglent",
         # This one is called RSPD3303X-E by RS PRO.
         "SPD3XIDD5R7170": "[RS PRO]",
+        "NPD3XHBC4R0026": "[RS PRO]",
     }
 
-
     @classmethod
-    def usb_device(cls, visa_rscr: str=None):
+    def usb_device(cls, visa_rscr: str = None):
         return USBDevice(visa_rscr)
 
     @classmethod
     def ethernet_device(cls, host: str):
         return EthernetDevice(host)
 
     class Channel(object):
@@ -70,60 +71,62 @@
             dsc = self.query("*IDN?")
         except pyvisa.errors.VisaIOError:
             self._inst.close()
             raise
         identity_items = dsc.split(",")
         if len(identity_items) == 3:
             # RS PRO RSPD3303X-E ?
-            model, _, _= dsc.split(",")
+            model, _, _ = dsc.split(",")
             mnf = self.MANUFACTURERS.get(model, "[Unknown]")
         else:
             # Proper Siglent device probably.
-            mnf, model,_,_,_ = identity_items
+            mnf, model, _, _, _ = identity_items
         logger.debug(f"Discovered {model} by {mnf}")
         if model not in self.KNOWN_MODELS:
             raise Exception(f"Device {model} not supported")
         self.CH1 = SPD3303X.ControlledChannel(1, self)
         self.CH2 = SPD3303X.ControlledChannel(2, self)
         self.CH3 = SPD3303X.Channel(3, self)
         return self
 
     def __exit__(self, *args):
         self._inst.close()
 
+
 class USBDevice(SPD3303X):
-    def __init__(self, visa_rscr: str=None):
+    def __init__(self, visa_rscr: str = None):
         self._visa_rscr = visa_rscr
 
     def __enter__(self):
         rm = pyvisa.ResourceManager("@py")
         if self._visa_rscr is None:
             logger.debug("Trying to auto-detect USB device")
             resources = rm.list_resources()
             for res_str in resources:
                 if "SPD3XID" in res_str:
                     self._visa_rscr = res_str
             if self._visa_rscr is None:
                 raise Exception("No device found")
 
         self._inst = rm.open_resource(self._visa_rscr)
-        self._inst.write_termination="\n"
-        self._inst.read_termination="\n"
+        self._inst.write_termination = "\n"
+        self._inst.read_termination = "\n"
         return super().__enter__()
 
     def write(self, cmd: str):
         self._inst.write(cmd)
         time.sleep(0.1)
 
     def query(self, cmd: str):
         self.write(cmd)
         rep = self._inst.read()
         time.sleep(0.1)
         return rep
 
+
 class EthernetDevice(SPD3303X):
     def __init__(self, host: str):
         self._host = host
 
     def __enter__(self):
         try:
             logger.debug(f"Trying to resolve host {self._host}")
@@ -136,8 +139,7 @@
 
     def write(self, cmd: str):
         self._inst.write(cmd)
         time.sleep(0.1)
 
     def query(self, cmd: str):
         return self._inst.ask(cmd)
-
```

### Comparing `spd3303x-1.0.1/spd3303x/cli.py` & `spd3303x-1.0.2/spd3303x/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 import click
 import logging
 import re
 from spd3303x import SPD3303X
 
 logger = logging.getLogger("spd3303x")
 
+
 @click.group(context_settings=dict(help_option_names=["-h", "--help"], obj={}))
 @click.option("-v", "--verbose", count=True, default=2)
 @click.option("-d", "--device", type=str)
 @click.pass_context
 def cli(ctx, verbose, device):
-
-
     if verbose == 0:
         logger.setLevel(logging.ERROR)
     elif verbose == 1:
         logger.setLevel(logging.WARNING)
     elif verbose == 2:
         logger.setLevel(logging.INFO)
     elif verbose > 2:
```

### Comparing `spd3303x-1.0.1/spd3303x.egg-info/PKG-INFO` & `spd3303x-1.0.2/spd3303x.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spd3303x
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API for SigLent SPD3303X
 Author: Kai Geissdoerfer
 Author-email: kai.geissdoerfer@tu-dresden.de
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

