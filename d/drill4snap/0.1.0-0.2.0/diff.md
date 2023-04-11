# Comparing `tmp/drill4snap-0.1.0.tar.gz` & `tmp/drill4snap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drill4snap-0.1.0.tar", max compression
+gzip compressed data, was "drill4snap-0.2.0.tar", max compression
```

## Comparing `drill4snap-0.1.0.tar` & `drill4snap-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7651 2023-04-10 13:42:06.746487 drill4snap-0.1.0/LICENSE
--rw-r--r--   0        0        0     2038 2023-04-11 13:02:18.729446 drill4snap-0.1.0/README.md
--rw-r--r--   0        0        0       21 2023-04-10 14:07:12.271506 drill4snap-0.1.0/drill4snap/__init__.py
--rwxr-xr-x   0        0        0     1899 2023-04-11 12:20:30.196491 drill4snap-0.1.0/drill4snap/cli.py
--rw-r--r--   0        0        0      482 2023-04-11 07:51:33.373595 drill4snap-0.1.0/drill4snap/devices.py
--rw-r--r--   0        0        0     9412 2023-04-11 08:48:07.713290 drill4snap-0.1.0/drill4snap/drill_pict.png
--rw-r--r--   0        0        0      542 2023-04-11 10:16:54.449059 drill4snap-0.1.0/drill4snap/jobs.py
--rw-r--r--   0        0        0     5123 2023-04-11 10:18:45.062407 drill4snap-0.1.0/drill4snap/parser.py
--rw-r--r--   0        0        0     1171 2023-04-11 12:22:12.864748 drill4snap-0.1.0/drill4snap/templates.py
--rw-r--r--   0        0        0     6675 2023-04-11 12:16:49.446798 drill4snap-0.1.0/drill4snap/writer.py
--rw-r--r--   0        0        0      515 2023-04-11 09:51:14.838168 drill4snap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 drill4snap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7651 2023-04-10 13:42:06.746487 drill4snap-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2997 2023-04-11 13:34:53.661106 drill4snap-0.2.0/README.md
+-rw-r--r--   0        0        0       21 2023-04-10 14:07:12.271506 drill4snap-0.2.0/drill4snap/__init__.py
+-rwxr-xr-x   0        0        0     1899 2023-04-11 12:20:30.196491 drill4snap-0.2.0/drill4snap/cli.py
+-rw-r--r--   0        0        0      482 2023-04-11 07:51:33.373595 drill4snap-0.2.0/drill4snap/devices.py
+-rw-r--r--   0        0        0     9412 2023-04-11 08:48:07.713290 drill4snap-0.2.0/drill4snap/drill_pict.png
+-rw-r--r--   0        0        0      542 2023-04-11 10:16:54.449059 drill4snap-0.2.0/drill4snap/jobs.py
+-rw-r--r--   0        0        0     5123 2023-04-11 10:18:45.062407 drill4snap-0.2.0/drill4snap/parser.py
+-rw-r--r--   0        0        0     1171 2023-04-11 12:22:12.864748 drill4snap-0.2.0/drill4snap/templates.py
+-rw-r--r--   0        0        0     6675 2023-04-11 12:16:49.446798 drill4snap-0.2.0/drill4snap/writer.py
+-rw-r--r--   0        0        0      515 2023-04-11 13:35:13.141362 drill4snap-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 drill4snap-0.2.0/PKG-INFO
```

### Comparing `drill4snap-0.1.0/LICENSE` & `drill4snap-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drill4snap-0.1.0/README.md` & `drill4snap-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # drill4snap
 
 **DISCLAIMER: Take great care and check your gcode files before using them! No responsibility is taken by the developer of this software!**
 
+![file_preview](docs/header_image.jpg)
+
 Convert Excellon drill files to GCode that can be used with the CNC/milling ability of Snapmaker devices.
 
 Provides a small command line tool to generate one gcode file for every drill size in the drill file. These files can
 be used either directly via a USB stick or loaded into the Luban software for execution.
 
 ## About
 
@@ -36,14 +38,51 @@
 
 - only tested for newest Snapmaker firmware on Snapmaker 2.0 A350
 - not tested for GRBL based devices
 - only tested for files produced by Kicad
 
 ## Usage
 
+1. Install via pip:
+
+```shell
+pip install drill4snap
+```
+
+2. Generate you drill file from Kicad using the plot suboption:
+
+![Kicad drill file options](docs/kicad_generate_drill_file.png)
+
+3. Generate the CNC files for Snapmaker using the `drill4snap` command:
+
+```shell
+drill4snap --device s2m my_drill_file.drl
+```
+
+This will produce a CNC file with the drill diameter as postfixed for every tool in the drill file:
+
+```
+my_drill_file_0.95.cnc
+my_drill_file_1.0.cnc
+my_drill_file_2.3.cnc
+```
+4. Use either Luban or the device screen to position the tool head at the work origin and then setting the work origin.
+
+![luban set origin](docs/set_origin.png)
+
+5. Load the gcode files into Luban workspace or transfer them using a USB storage:
+
+![Luban load GCode panel](docs/load_panel.png)
+
+6. Using Luban you can now start the Job using ''
+
+![job running](docs/running_job.png)
+
+Let the Snapmaker do the work and enjoy!
+
 ## Credits
 
 Based on drl2gcode (https://github.com/jes/drl2gcode) by James Stanley
 which is based on
 drl2gcode (https://git.nexlab.net/machinery/drl2gcode) by Franco Lanza.
 
 Licensed under LGPL
```

### Comparing `drill4snap-0.1.0/drill4snap/cli.py` & `drill4snap-0.2.0/drill4snap/cli.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.1.0/drill4snap/drill_pict.png` & `drill4snap-0.2.0/drill4snap/drill_pict.png`

 * *Files identical despite different names*

### Comparing `drill4snap-0.1.0/drill4snap/jobs.py` & `drill4snap-0.2.0/drill4snap/jobs.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.1.0/drill4snap/parser.py` & `drill4snap-0.2.0/drill4snap/parser.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.1.0/drill4snap/templates.py` & `drill4snap-0.2.0/drill4snap/templates.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.1.0/drill4snap/writer.py` & `drill4snap-0.2.0/drill4snap/writer.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.1.0/pyproject.toml` & `drill4snap-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drill4snap"
-version = "0.1.0"
+version = "0.2.0"
 description = "Convert Excellion drill files (such as those produced by KiCad) into G-Code for SnapMaker CNC usage"
 authors = ["Michael Jonathan Lee"]
 license = "LGPL"
 readme = "README.md"
 packages = [{include = "drill4snap"}]
 
 [tool.poetry.dependencies]
```

### Comparing `drill4snap-0.1.0/PKG-INFO` & `drill4snap-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drill4snap
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convert Excellion drill files (such as those produced by KiCad) into G-Code for SnapMaker CNC usage
 License: LGPL
 Author: Michael Jonathan Lee
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,16 @@
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # drill4snap
 
 **DISCLAIMER: Take great care and check your gcode files before using them! No responsibility is taken by the developer of this software!**
 
+![file_preview](docs/header_image.jpg)
+
 Convert Excellon drill files to GCode that can be used with the CNC/milling ability of Snapmaker devices.
 
 Provides a small command line tool to generate one gcode file for every drill size in the drill file. These files can
 be used either directly via a USB stick or loaded into the Luban software for execution.
 
 ## About
 
@@ -52,14 +54,51 @@
 
 - only tested for newest Snapmaker firmware on Snapmaker 2.0 A350
 - not tested for GRBL based devices
 - only tested for files produced by Kicad
 
 ## Usage
 
+1. Install via pip:
+
+```shell
+pip install drill4snap
+```
+
+2. Generate you drill file from Kicad using the plot suboption:
+
+![Kicad drill file options](docs/kicad_generate_drill_file.png)
+
+3. Generate the CNC files for Snapmaker using the `drill4snap` command:
+
+```shell
+drill4snap --device s2m my_drill_file.drl
+```
+
+This will produce a CNC file with the drill diameter as postfixed for every tool in the drill file:
+
+```
+my_drill_file_0.95.cnc
+my_drill_file_1.0.cnc
+my_drill_file_2.3.cnc
+```
+4. Use either Luban or the device screen to position the tool head at the work origin and then setting the work origin.
+
+![luban set origin](docs/set_origin.png)
+
+5. Load the gcode files into Luban workspace or transfer them using a USB storage:
+
+![Luban load GCode panel](docs/load_panel.png)
+
+6. Using Luban you can now start the Job using ''
+
+![job running](docs/running_job.png)
+
+Let the Snapmaker do the work and enjoy!
+
 ## Credits
 
 Based on drl2gcode (https://github.com/jes/drl2gcode) by James Stanley
 which is based on
 drl2gcode (https://git.nexlab.net/machinery/drl2gcode) by Franco Lanza.
 
 Licensed under LGPL
```

