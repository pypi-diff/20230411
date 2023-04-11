# Comparing `tmp/synth_mapping_helper-1.1.1.tar.gz` & `tmp/synth_mapping_helper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.1.1.tar", last modified: Sun Apr  9 17:27:56 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.2.0.tar", last modified: Tue Apr 11 19:53:00 2023, max compression
```

## Comparing `synth_mapping_helper-1.1.1.tar` & `synth_mapping_helper-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25631 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.750025 synth_mapping_helper-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.754025 synth_mapping_helper-1.2.0/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25631 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27963 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.1.1/LICENSE` & `synth_mapping_helper-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/PKG-INFO` & `synth_mapping_helper-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.1.1
+Version: 1.2.0
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.1.1/README.md` & `synth_mapping_helper-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/setup.py` & `synth_mapping_helper-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/cli.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/companion.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 from pathlib import Path
 from time import strftime, time, sleep
 from zipfile import ZipFile
 
 import numpy as np
 import matplotlib.pyplot as plt
+from matplotlib.colors import PowerNorm
 from matplotlib.lines import Line2D
 from matplotlib.ticker import FuncFormatter
 from matplotlib.widgets import Button, CheckButtons, RadioButtons, Slider
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
 from . import movement, synth_format, utils, __version__
@@ -36,14 +37,16 @@
 DEFAULT_OUTPUT_FILE = Path("output.synth")  # inside working directory
 DEFAULT_BACKUP_DIR = Path("smh_backup")  # inside working directory
 
 DEFAULT_VELOCITY_WINDOW = utils.SecondFloat(0.5)  # half a second gap breaks up velocity / acceleration calculations
 DEFAULT_INTERPOLATION = 1/16
 DEFAULT_VEL_LIMIT = 100
 DEFAULT_ACC_LIMIT = 1000
+DEFAULT_HEATMAP_BIN_COUNT = 3
+DEFAULT_HEATMAP_NORM_POWER = 0.6
 
 DEFAULT_WINDOW_WIDTH = 1600
 DEFAULT_WINDOW_HEIGHT = 900
 DEFAULT_MENU_SIZE = 100
 
 # TODO: make those command line arguments
 AUTORELOAD_DEFAULT = True
@@ -67,14 +70,16 @@
     parser.add_argument("-o", "--output-file", type=Path, default=DEFAULT_OUTPUT_FILE, help=f"Output file. Default: {DEFAULT_OUTPUT_FILE}")
     parser.add_argument("-b", "--backup-dir", type=Path, default=DEFAULT_BACKUP_DIR, help=f"Directory for autobackups. Default: {DEFAULT_BACKUP_DIR}")
 
     parser.add_argument("--velocity-window", type=utils.parse_time, default=DEFAULT_VELOCITY_WINDOW, help=f"Breaks at least this long reset velocity/acceleration calculation. Default: {DEFAULT_VELOCITY_WINDOW}")
     parser.add_argument("--interpolation", type=utils.parse_time, default=DEFAULT_INTERPOLATION, help=f"Interpolation distance for plots and velocity/accelation calculation. Default: {DEFAULT_INTERPOLATION}")
     parser.add_argument("--velocity-limit", type=float, default=DEFAULT_VEL_LIMIT, help=f"Starting limit of the velocity plot. Default: {DEFAULT_VEL_LIMIT}")
     parser.add_argument("--acceleration-limit", type=float, default=DEFAULT_ACC_LIMIT, help=f"Starting limit of the acceleration plot. Default: {DEFAULT_ACC_LIMIT}")
+    parser.add_argument("--heatmap-bin-count", type=float, default=DEFAULT_HEATMAP_BIN_COUNT, help=f"Number of heatmap bins per grid square. Default: {DEFAULT_HEATMAP_BIN_COUNT}")
+    parser.add_argument("--heatmap-norm-power", type=float, default=DEFAULT_HEATMAP_NORM_POWER, help=f"Power of heatmap normalisation. Default: {DEFAULT_HEATMAP_NORM_POWER}")
 
     parser.add_argument("--window-size", type=str, default=f"{DEFAULT_WINDOW_WIDTH}x{DEFAULT_WINDOW_HEIGHT}", help=f"Size of plot window (excluding toolbars) in pixels. Default: {DEFAULT_WINDOW_WIDTH}x{DEFAULT_WINDOW_HEIGHT}")
     parser.add_argument("--menu-size", type=int, default=f"{DEFAULT_MENU_SIZE}", help=f"Height of menu in pixels. Also influences text size. Default: {DEFAULT_MENU_SIZE}")
     return parser
 
 def abort(reason: str):
     logging.error(reason)
@@ -336,22 +341,43 @@
     ]
     ax_density.legend(loc="upper right", ncol=len(wall_markers))
     if platform == "PC":
         ax_status.legend(handles=legend_elements[:2], loc="upper right", ncol=2)
     else:
         ax_status.legend(handles=legend_elements, loc="upper right", ncol=3)
 
+def plot_heatmap(options, fig, infile: SynthFile, data: DataContainer, prepared_data, platform: str):
+    axs = fig.subplots(2,2)
+    axs = (
+        axs[0,1],  # right
+        axs[0,0],  # left
+        axs[1,0],  # single
+        axs[1,1],  # both
+    )
+    for t, note_type in enumerate(synth_format.NOTE_TYPES):
+        _, pos, _, _ = prepared_data[0][t]
+        axs[t].hist2d(
+            pos[:, 0], pos[:,1],
+            bins=[int(17 * options.heatmap_bin_count),int(13 * options.heatmap_bin_count)], range=[[-8,8],[-6,6]],
+            cmap=("Reds", "Blues", "Greens", "Oranges")[t],
+            density=False, norm=PowerNorm(options.heatmap_norm_power),
+        )
+        avg = np.nanmean(pos, axis=0)
+        axs[t].plot(avg[0], avg[1], marker="x", color="white", markeredgecolor="black", markersize=10)
+        axs[t].grid(True)
+
 def show_warnings(options, fig, infile: SynthFile, data: DataContainer, prepared_data, platform: str):
     ax = fig.subplots(1)
     ax.set_axis_off()
     ax.table(loc="top", colWidths=(1/20, 19/20), cellLoc="left", rowLabels=["123 5/6"], cellText=[["note:left", "placeholder, ie extreme peak in acceleration"]])
 
 TABS = [
     ("Notes", plot_notes),
     ("Walls", plot_walls),
+    ("Heatmap", plot_heatmap),
     # ("Warnings", show_warnings)
 ]
 PLATFORMS = ("PC", "Quest")
 
 def main(options):
     if not options.input.is_file():
         abort("Input file is not a file, is the path correct?")
```

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/rails.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/synth_format.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.1.1
+Version: 1.2.0
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

