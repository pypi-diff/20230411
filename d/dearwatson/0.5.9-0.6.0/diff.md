# Comparing `tmp/dearwatson-0.5.9.tar.gz` & `tmp/dearwatson-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.5.9.tar", last modified: Tue Mar 28 09:34:36 2023, max compression
+gzip compressed data, was "dearwatson-0.6.0.tar", last modified: Tue Apr 11 10:28:50 2023, max compression
```

## Comparing `dearwatson-0.5.9.tar` & `dearwatson-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.356158 dearwatson-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 09:34:17.000000 dearwatson-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-28 09:34:17.000000 dearwatson-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-28 09:34:36.356158 dearwatson-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 09:34:17.000000 dearwatson-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 09:34:36.000000 dearwatson-0.5.9/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 09:34:36.356158 dearwatson-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-28 09:34:19.000000 dearwatson-0.5.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-28 09:34:19.000000 dearwatson-0.5.9/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.348158 dearwatson-0.5.9/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-03-28 09:34:19.000000 dearwatson-0.5.9/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.352158 dearwatson-0.5.9/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:20.000000 dearwatson-0.5.9/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-03-28 09:34:20.000000 dearwatson-0.5.9/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:34:36.356158 dearwatson-0.5.9/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:34:21.000000 dearwatson-0.5.9/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-03-28 09:34:21.000000 dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-03-28 09:34:21.000000 dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   109758 2023-03-28 09:34:20.000000 dearwatson-0.5.9/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.418296 dearwatson-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 10:28:35.000000 dearwatson-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 10:28:35.000000 dearwatson-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-11 10:28:50.418296 dearwatson-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-11 10:28:35.000000 dearwatson-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.414296 dearwatson-0.6.0/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-11 10:28:50.000000 dearwatson-0.6.0/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 10:28:50.000000 dearwatson-0.6.0/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:28:50.000000 dearwatson-0.6.0/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-11 10:28:50.000000 dearwatson-0.6.0/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 10:28:50.000000 dearwatson-0.6.0/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:28:50.418296 dearwatson-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-11 10:28:37.000000 dearwatson-0.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 10:28:37.000000 dearwatson-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.414296 dearwatson-0.6.0/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.414296 dearwatson-0.6.0/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.414296 dearwatson-0.6.0/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.414296 dearwatson-0.6.0/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.418296 dearwatson-0.6.0/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:28:50.418296 dearwatson-0.6.0/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:28:39.000000 dearwatson-0.6.0/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-04-11 10:28:39.000000 dearwatson-0.6.0/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-11 10:28:39.000000 dearwatson-0.6.0/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106233 2023-04-11 10:28:37.000000 dearwatson-0.6.0/watson/watson.py
```

### Comparing `dearwatson-0.5.9/LICENSE` & `dearwatson-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/PKG-INFO` & `dearwatson-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.5.9
+Version: 0.6.0
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.5.9/README.md` & `dearwatson-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.6.0/dearwatson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.5.9
+Version: 0.6.0
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.5.9/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.6.0/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/setup.py` & `dearwatson-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.5.9"
+version = "0.6.0"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
@@ -23,15 +23,15 @@
     python_requires='>=3.8',
     install_requires=[
                         "bokeh==2.4.2", # TPFPlotter dependency
                         'configparser==5.0.1',
                         "cython==0.29.21",
                         "extension-helpers==0.1",
                         "imageio==2.9.0",
-                        "lcbuilder==0.10.12",
+                        "lcbuilder==0.11.1",
                         "matplotlib==3.5.2",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "pyyaml==5.4.1",
                         "reportlab==3.5.59",
                         'setuptools>=41.0.0',
     ]
 )
```

### Comparing `dearwatson-0.5.9/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.6.0/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/watson/neighbours.py` & `dearwatson-0.6.0/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/watson/report.py` & `dearwatson-0.6.0/watson/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 resources_dir = path.join(path.dirname(__file__))
 
 
 class Report:
     LOGO_IMAGE = resources_dir + "/resources/images/watson.png"
 
     def __init__(self, data_dir, file_name, object_id, ra, dec, t0, period, duration, depth, transit_t0s_list,
-                 summary_list_t0s_indexes, v, j, h, k, with_tpfs=True):
+                 summary_list_t0s_indexes, v, j, h, k, with_tpfs=True, is_summary=False):
         self.data_dir = data_dir
         self.file_name = file_name
         self.object_id = object_id
         self.ra = ra
         self.dec = dec
         self.t0 = t0
         self.period = period
@@ -36,14 +36,15 @@
         self.transit_t0s_list = transit_t0s_list
         self.summary_list_t0s_indexes = summary_list_t0s_indexes
         self.v = v
         self.j = j
         self.h = h
         self.k = k
         self.with_tpfs = with_tpfs
+        self.is_summary = is_summary
 
     @staticmethod
     def row_colors(df, table_object):
         data_len = len(df)
         for each in range(1, data_len + 1):
             if each % 2 == 1:
                 bg_color = colors.whitesmoke
@@ -255,24 +256,25 @@
                                                                                             'Middle right, the declination centroid shift with binning. ' \
                                                                                             'Bottom left, optical ghost diagnostic curve for core flux.' \
                                                                                             'Bottom right, optical ghost diagnostic curve for halo flux</font>'
             story.append(Spacer(1, 5))
             story.append(Paragraph(descripcion, styles["ParagraphAlignCenter"]))
             story.append(Spacer(1, 15))
             figure = figure + 1
-        for file in sorted(list(pathlib.Path(self.data_dir).glob('folded_tpf_*.png'))):
-            story.append(Image(str(file), width=14 * cm, height=22 * cm))
-            descripcion = '<font name="HELVETICA" size="9"><strong>Figure ' + str(figure) + '' \
-                                                                                            ': </strong>Above, the TPF and per-pixel BLS SNR best fits. Bottom left, the per-pixel BLS SNR for each' \
-                                                                                            ' pixel. Bottom right, the differential images SNR for each pixel. The target position is represented ' \
-                                                                                            'by a red star and the TPF independent source offset is represented by a white plus.</font>'
-            story.append(Spacer(1, 5))
-            story.append(Paragraph(descripcion, styles["ParagraphAlignCenter"]))
-            figure = figure + 1
-        story.append(PageBreak())
+        if not self.is_summary:
+            for file in sorted(list(pathlib.Path(self.data_dir).glob('folded_tpf_*.png'))):
+                story.append(Image(str(file), width=14 * cm, height=22 * cm))
+                descripcion = '<font name="HELVETICA" size="9"><strong>Figure ' + str(figure) + '' \
+                                                                                                ': </strong>Above, the TPF and per-pixel BLS SNR best fits. Bottom left, the per-pixel BLS SNR for each' \
+                                                                                                ' pixel. Bottom right, the differential images SNR for each pixel. The target position is represented ' \
+                                                                                                'by a red star and the TPF independent source offset is represented by a white plus.</font>'
+                story.append(Spacer(1, 5))
+                story.append(Paragraph(descripcion, styles["ParagraphAlignCenter"]))
+                figure = figure + 1
+            story.append(PageBreak())
         introduction = '<font name="HELVETICA" size="9">The next pages will contain each of the single-transits ' \
                        'vetting sheets with the next information: </font>'
         story.append(Paragraph(introduction, styles["ParagraphAlignJustify"]))
         story.append(ListFlowable(
             [Paragraph(s, styles["ParagraphAlignJustify"]) for s in [
                 "<b>TOP-LEFT</b>: Plot with single transit photometry found in the analyzed curve (with momentum dumps, if any).",
                 "<b>TOP-CENTER</b>: Plot with X-axis data drift (X-axis motion vs X-axis centroid offset) around the transit times.",
```

### Comparing `dearwatson-0.5.9/watson/resources/images/sherlock3.png` & `dearwatson-0.6.0/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/watson/resources/images/watson.png` & `dearwatson-0.6.0/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/watson/tests/test_watson.py` & `dearwatson-0.6.0/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.6.0/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.6.0/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.5.9/watson/watson.py` & `dearwatson-0.6.0/watson/watson.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 # from __future__ import print_function, absolute_import, division
 
 import logging
 import multiprocessing
 import traceback
-import lcbuilder.eleanor
 import sys
 
 from watson.data_validation_report.DvrPreparer import DvrPreparer
 
-sys.modules['eleanor'] = sys.modules['lcbuilder.eleanor']
-import eleanor
-from lcbuilder.eleanor.targetdata import TargetData
-from lcbuilder.eleanor_manager import EleanorManager
 import warnings
 from itertools import chain
 import PIL
 import batman
-import scipy
 import foldedleastsquares
 import lcbuilder
 import lightkurve
-from lightkurve.periodogram import BoxLeastSquaresPeriodogram
 from lightkurve import MPLSTYLE
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import wotan
 import yaml
 from astropy.timeseries.periodograms import BoxLeastSquares
 from astropy.wcs import WCS
 from astropy.coordinates import SkyCoord
 from astropy import units as u
-from lcbuilder.constants import CUTOUT_SIZE, LIGHTKURVE_CACHE_DIR, ELEANOR_CACHE_DIR
+from lcbuilder.constants import CUTOUT_SIZE, LIGHTKURVE_CACHE_DIR
 from lcbuilder.helper import LcbuilderHelper
 from lcbuilder.lcbuilder_class import LcBuilder
 from lcbuilder.objectinfo.MissionObjectInfo import MissionObjectInfo
 from lcbuilder.objectinfo.preparer.MissionLightcurveBuilder import MissionLightcurveBuilder
 from lcbuilder.photometry.aperture_extractor import ApertureExtractor
 from lcbuilder.star.EpicStarCatalog import EpicStarCatalog
 from lcbuilder.star.HabitabilityCalculator import HabitabilityCalculator
@@ -50,16 +43,14 @@
 import astropy.visualization as stretching
 from scipy import stats, ndimage
 
 from watson import constants
 import watson.tpfplotterSub.tpfplotter as tpfplotter
 import pandas as pd
 import os
-from math import ceil, floor
-from copy import deepcopy
 
 from watson.neighbours import CreateStarCsvInput, create_star_csv, NeighbourInput, get_neighbour_lc
 from watson.report import Report
 
 
 class Watson:
     """
@@ -163,15 +154,15 @@
         logging.info("Creating complete report")
         report = Report(self.data_dir, file_name, id, ra, dec, t0, period, duration, depth, transits_list, None,
                         v, j, h, k, with_tpfs)
         report.create_report()
         file_name = "transits_validation_report_summary.pdf"
         logging.info("Creating summary report")
         report = Report(self.data_dir, file_name, id, ra, dec, t0, period, duration, depth, transits_list,
-                        summary_list_t0s_indexes, v, j, h, k, with_tpfs)
+                        summary_list_t0s_indexes, v, j, h, k, with_tpfs, is_summary=True)
         report.create_report()
 
 
     def vetting_with_data(self, candidate_df, star, transits_df, cpus, create_fov_plots=False, cadence_fov=None,
                           transits_mask=None):
         """
         Same than vetting but receiving a candidate dataframe and a star dataframe with one row each.
@@ -268,23 +259,17 @@
                 summary_t0s_indexes = np.append(summary_t0s_indexes, np.argmin(closest_depths_to_mean))
         else:
             transit_t0s_list = LcbuilderHelper.compute_t0s(lc.time.value, period, t0, duration / 60 / 24)
         mission, mission_prefix, target_id = MissionLightcurveBuilder().parse_object_id(id)
         metrics_df = pd.DataFrame(columns=['metric', 'score', 'passed'])
         snrs = Watson.plot_all_folded_cadences(self.data_dir, mission_prefix, mission, target_id, lc, sectors, period,
                                                t0, duration, depth / 1000, rp_rstar, a_rstar, transits_mask, cpus)
-        folded_cadences_snrs = [snr for snr in snrs.values()]
-        if len(folded_cadences_snrs) > 0:
+        if len(snrs.values()) > 0:
             for cadence, snr in snrs.items():
                 metrics_df = metrics_df.append({'metric': cadence + '_snr', 'score': snr, 'passed': snr > 3}, ignore_index=True)
-            folded_cadences_snrs_mean = np.nanmean(folded_cadences_snrs)
-            folded_cadences_snrs_std = np.nanstd(folded_cadences_snrs)
-            folded_cadences_snr_significance = folded_cadences_snrs_std / folded_cadences_snrs_mean
-            metrics_df = metrics_df.append({'metric': 'folded_cadences_snr', 'score': folded_cadences_snr_significance,
-                               'passed': folded_cadences_snr_significance < 0.3}, ignore_index=True)
         snr_p_t0, snr_p_2t0, snr_2p_t0, snr_2p_2t0, snr_p2_t0, snr_p2_t02 = \
             self.plot_folded_curve(self.data_dir, id, lc, period, t0, duration, depth / 1000, rp_rstar, a_rstar)
         metrics_df = metrics_df.append({'metric': 'snr_p_t0', 'score': snr_p_t0, 'passed': snr_p_t0 > 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_p_2t0', 'score': snr_p_2t0, 'passed': snr_p_2t0 < 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_2p_t0', 'score': snr_2p_t0, 'passed': snr_2p_t0 > 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_2p_2t0', 'score': snr_2p_2t0, 'passed': snr_2p_2t0 > 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_p2_t0', 'score': snr_p2_t0, 'passed': snr_p2_t0 < 3}, ignore_index=True)
@@ -301,15 +286,15 @@
                                         tpfs, lc_file, lc_data_file, tpfs_dir, sectors, period, t0, duration, depth / 1000,
                                         rp_rstar, a_rstar, transits_mask, transit_t0s_list, apertures, cpus)
                 pixel_size = LcbuilderHelper.mission_pixel_size(mission)
                 pixel_size_degrees = pixel_size / 3600
                 offset_test = np.sqrt((offset_ra - ra_fov) ** 2 + (offset_dec - dec_fov) ** 2) < pixel_size / 3600
                 metrics_df = metrics_df.append({'metric': 'transit_offset_ra', 'score': offset_ra, 'passed': np.abs(offset_ra - ra_fov) < pixel_size_degrees}, ignore_index=True)
                 metrics_df = metrics_df.append({'metric': 'transit_offset_dec', 'score': offset_dec, 'passed': np.abs(offset_dec - dec_fov) < pixel_size_degrees}, ignore_index=True)
-                metrics_df = metrics_df.append({'metric': 'transit_offset_err', 'score': offset_err, 'passed': offset_err < pixel_size * 3 / 3600}, ignore_index=True)
+                metrics_df = metrics_df.append({'metric': 'transit_offset_err', 'score': offset_err, 'passed': True if offset_err < pixel_size * 3 / 3600 else np.nan}, ignore_index=True)
                 target_dist = np.sqrt((offset_ra - ra_fov) ** 2 + (offset_dec - dec_fov) ** 2)
                 metrics_df = metrics_df.append({'metric': 'transit_offset_pos', 'score': target_dist, 'passed': target_dist < offset_err}, ignore_index=True)
                 metrics_df = metrics_df.append({'metric': 'core_flux_snr', 'score': core_flux_snr, 'passed': True if core_flux_snr > 3 else np.nan }, ignore_index=True)
                 metrics_df = metrics_df.append({'metric': 'halo_flux_snr', 'score': halo_flux_snr, 'passed': True if halo_flux_snr > 3 else np.nan }, ignore_index=True)
                 metrics_df = metrics_df.append({'metric': 'og_score', 'score': og_score, 'passed': og_score < 1 if core_flux_snr > 3 else np.nan }, ignore_index=True)
                 metrics_df = metrics_df.append({'metric': 'centroids_ra_snr', 'score': centroids_ra_snr, 'passed': np.abs(centroids_ra_snr) < 3 }, ignore_index=True)
                 metrics_df = metrics_df.append({'metric': 'centroids_dec_snr', 'score': centroids_dec_snr, 'passed': np.abs(centroids_dec_snr) < 3 }, ignore_index=True)
@@ -331,22 +316,23 @@
         mission, mission_prefix, mission_int_id = LcBuilder().parse_object_info(id)
         lc = pd.read_csv(lc_file, header=0)
         lc_data = None
         lc_data_norm = None
         if os.path.exists(lc_data_file):
             lc_data = pd.read_csv(lc_data_file, header=0)
             lc_data_norm = Watson.normalize_lc_data(lc_data)
+            if 'quality' in lc_data.columns:
+                lc_data = lc_data.drop('quality', axis='columns')
         time, flux, flux_err = lc["#time"].values, lc["flux"].values, lc["flux_err"].values
         for transit_mask in transits_mask:
             logging.info('* Transit mask with P=%.2f d, T0=%.2f d, Dur=%.2f min *', transit_mask["P"],
                          transit_mask["T0"], transit_mask["D"])
             time, flux, flux_err = LcbuilderHelper.mask_transits(time, flux,  transit_mask["P"],
                                                                  transit_mask["D"] / 60 / 24, transit_mask["T0"])
         lc = TessLightCurve(time=time, flux=flux, flux_err=flux_err, quality=np.zeros(len(time)))
-        lc.extra_columns = []
         tpfs = []
         if os.path.exists(tpfs_dir):
             for tpf_file in sorted(os.listdir(tpfs_dir)):
                 tpf = TessTargetPixelFile(tpfs_dir + "/" + tpf_file) if mission == lcbuilder.constants.MISSION_TESS else \
                     KeplerTargetPixelFile(tpfs_dir + "/" + tpf_file)
                 for transit_mask in transits_mask:
                     mask = foldedleastsquares.transit_mask(tpf.time.value, transit_mask["P"], transit_mask["D"] / 60 / 24,
@@ -362,21 +348,21 @@
         time = lc_data_copy["time"].to_numpy()
         dif = time[1:] - time[:-1]
         jumps = np.where(np.abs(dif) > 0.2)[0]
         jumps = np.append(jumps, len(lc_data_copy))
         previous_jump_index = 0
         for jumpIndex in jumps:
             token = lc_data_copy["centroids_x"][previous_jump_index:jumpIndex]
-            lc_data_copy["centroids_x"][previous_jump_index:jumpIndex] = token - np.nanmedian(token)
+            lc_data_copy.iloc[previous_jump_index:jumpIndex]["centroids_x"] = token - np.nanmedian(token)
             token = lc_data_copy["centroids_y"][previous_jump_index:jumpIndex]
-            lc_data_copy["centroids_y"][previous_jump_index:jumpIndex] = token - np.nanmedian(token)
+            lc_data_copy.iloc[previous_jump_index:jumpIndex]["centroids_y"] = token - np.nanmedian(token)
             token = lc_data_copy["motion_x"][previous_jump_index:jumpIndex]
-            lc_data_copy["motion_x"][previous_jump_index:jumpIndex] = token - np.nanmedian(token)
+            lc_data_copy.iloc[previous_jump_index:jumpIndex]["motion_x"] = token - np.nanmedian(token)
             token = lc_data_copy["motion_y"][previous_jump_index:jumpIndex]
-            lc_data_copy["motion_y"][previous_jump_index:jumpIndex] = token - np.nanmedian(token)
+            lc_data_copy.iloc[previous_jump_index:jumpIndex]["motion_y"] = token - np.nanmedian(token)
             previous_jump_index = jumpIndex
         return lc_data_copy
 
     @staticmethod
     def plot_transits_statistics(data_dir, id, epoch, period, transits_list):
         fig, axs = plt.subplots(1, 1, figsize=(12, 6), constrained_layout=True)
         fig.suptitle(str(id) + ' Transits depth analysis T0=' + str(round(epoch, 2)) + ' P=' + str(round(period, 2)) + 'd', size=18)
@@ -665,15 +651,14 @@
         fig.clf()
         plt.close(fig)
         return snr_p_t0, snr_p_2t0, snr_2p_t0, snr_2p_2t0, snr_p2_t0, snr_p2_t02
 
     @staticmethod
     def plot_all_folded_cadences(file_dir, mission_prefix, mission, id, lc, sectors, period, epoch, duration, depth, rp_rstar,
                                  a_rstar, transits_mask, cpus=os.cpu_count() - 1):
-        updated_eleanor = False
         bins = 100
         fig, axs = plt.subplots(3, 1, figsize=(10, 15))
         duration = duration / 60 / 24
         duration_to_period = duration / period
         cadences = ['fast', 'short', 'long']
         epoch = LcbuilderHelper.correct_epoch(mission, epoch)
         snrs = {}
@@ -685,96 +670,48 @@
                 author = "TESS-SPOC"
             elif mission == lcbuilder.constants.MISSION_TESS and cadence != 'long':
                 author = "SPOC"
             elif mission == lcbuilder.constants.MISSION_KEPLER:
                 author = "Kepler"
             elif mission == lcbuilder.constants.MISSION_K2:
                 author = "K2"
-            if mission == "TESS" and cadence == 'long':
-                lcs = lightkurve.search_lightcurve(
-                    mission_prefix + " " + str(id),
-                    mission=mission,
-                    sector=sectors,
-                    campaign=sectors,
-                    quarter=sectors,
-                    author=author,
-                    cadence=cadence
-                ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
-                if lcs is None:
-                    if not updated_eleanor:
-                        EleanorManager.update()
-                        updated_eleanor = True
-                    star = eleanor.multi_sectors(tic=round(id), sectors='all',
-                                                 post_dir=os.path.expanduser('~') + '/' + ELEANOR_CACHE_DIR,
-                                                 metadata_path=os.path.expanduser('~') + '/' + ELEANOR_CACHE_DIR)
-                    data = []
-                    for s in star:
-                        datum = TargetData(s, height=CUTOUT_SIZE, width=CUTOUT_SIZE, do_pca=True)
-                        data.append(datum)
-                    lc = data[0].to_lightkurve(data[0].pca_flux).remove_nans().flatten()
-                    if len(data) > 1:
-                        for datum in data[1:]:
-                            lc = lc.append(datum.to_lightkurve(datum.pca_flux).remove_nans().flatten())
-                    lc = lc.remove_nans()
-                else:
-                    matching_objects = []
-                    for i in range(0, len(lcs.data)):
-                        if lcs.data[i].label == "TIC " + str(id):
-                            if lc is None:
-                                lc = lcs.data[i].normalize()
-                            else:
-                                lc = lc.append(lcs.data[i].normalize())
-                        else:
-                            matching_objects.append(lcs.data[i].label)
+            lcs = lightkurve.search_lightcurve(
+                mission_prefix + " " + str(id),
+                mission=mission,
+                sector=sectors,
+                campaign=sectors,
+                quarter=sectors,
+                author=author,
+                cadence=cadence
+            ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
+            if lcs is None:
+                continue
+            matching_objects = []
+            for i in range(0, len(lcs.data)):
+                if lcs.data[i].label == mission_prefix + " " + str(id):
                     if lc is None:
-                        continue
-                    else:
-                        if mission == lcbuilder.constants.MISSION_TESS:
-                            found_sectors = lcs.sector
-                        elif mission == lcbuilder.constants.MISSION_KEPLER:
-                            found_sectors = lcs.quarter
-                        elif mission == lcbuilder.constants.MISSION_K2:
-                            found_sectors = lcs.campaign
-                    lc = lc.remove_nans()
-                    if mission == lcbuilder.constants.MISSION_K2:
-                        lc = lc.to_corrector("sff").correct(windows=20)
-            else:
-                lcs = lightkurve.search_lightcurve(
-                    mission_prefix + " " + str(id),
-                    mission=mission,
-                    sector=sectors,
-                    campaign=sectors,
-                    quarter=sectors,
-                    author=author,
-                    cadence=cadence
-                ).download_all(download_dir=os.path.expanduser('~') + '/' + LIGHTKURVE_CACHE_DIR)
-                if lcs is None:
-                    continue
-                matching_objects = []
-                for i in range(0, len(lcs.data)):
-                    if lcs.data[i].label == mission_prefix + " " + str(id):
-                        if lc is None:
-                            lc = lcs.data[i].normalize()
-                        else:
-                            lc = lc.append(lcs.data[i].normalize())
+                        lc = lcs.data[i].normalize()
                     else:
-                        matching_objects.append(lcs.data[i].label)
-                if lc is None:
-                    continue
+                        lc = lc.append(lcs.data[i].normalize())
                 else:
-                    if mission == lcbuilder.constants.MISSION_TESS:
-                        found_sectors = lcs.sector
-                    elif mission == lcbuilder.constants.MISSION_KEPLER:
-                        found_sectors = lcs.quarter
-                    elif mission == lcbuilder.constants.MISSION_K2:
-                        found_sectors = lcs.campaign
-                lc = lc.remove_nans()
-                lc = lc.remove_outliers(sigma_lower=float('inf'), sigma_upper=3)
-                if mission == lcbuilder.constants.MISSION_K2:
-                    lc = lc.to_corrector("sff").correct(windows=20)
+                    matching_objects.append(lcs.data[i].label)
+            if lc is None:
+                continue
+            else:
+                if mission == lcbuilder.constants.MISSION_TESS:
+                    found_sectors = lcs.sector
+                elif mission == lcbuilder.constants.MISSION_KEPLER:
+                    found_sectors = lcs.quarter
+                elif mission == lcbuilder.constants.MISSION_K2:
+                    found_sectors = lcs.campaign
+            lc = lc.remove_nans()
+            lc = lc.remove_outliers(sigma_lower=float('inf'), sigma_upper=3)
+            if mission == lcbuilder.constants.MISSION_K2:
+                lc = lc.to_corrector("sff").correct(windows=20)
+            lc.flux = wotan.flatten(lc.time.value, lc.flux.value, window_length=duration * 4, method="biweight")
             lc = LcbuilderHelper.mask_transits_dict(lc, transits_mask)
             snr = Watson.compute_snr(lc.time.value, lc.flux.value, duration, period, epoch)
             snrs[cadence] = snr
             Watson.compute_phased_values_and_fill_plot(id, axs[index], lc, period, epoch, depth, duration,
                                                        rp_rstar, a_rstar, bins=bins)
             axs[index].set_title(mission_prefix + " " + str(id) + " " + str(found_sectors) + ": " + cadence + ". SNR=" + str(np.round(snr, 2)))
         file = file_dir + '/folded_cadences.png'
@@ -1488,16 +1425,14 @@
         fig, axs = plt.subplots(plot_grid_size, plot_grid_size, figsize=(16, 16))
         stars_df = pd.read_csv(star_csv_file)
         stars_df = stars_df.loc[~np.isnan(stars_df['id'])]
         stars_df = stars_df.sort_values(by=['dist_arcsec'], ascending=True)
         page = 0
         file = file_dir + '/star_nb_' + str(page) + '.png'
         duration = duration / 60 / 60
-        if mission == "TESS":
-            EleanorManager.update()
         neighbour_inputs = []
         for index, star_row in stars_df.iterrows():
             neighbour_inputs.append(
                 NeighbourInput(index, mission, author, round(star_row['id']), period, epoch, duration))
         with multiprocessing.Pool(processes=1) as pool:
             lc_dfs = pool.map(get_neighbour_lc, neighbour_inputs)
         for index, neighbour_input in enumerate(neighbour_inputs):
@@ -1750,15 +1685,15 @@
         :param indir: the data source directory
         :param mission: the mission of the target
         :param tic: the target id
         :param cadence: the exposure time between measurements in seconds
         :param ra: the right ascension of the target
         :param dec: the declination of the target
         :param sectors: the sectors where the target was observed
-        :param source: the source where the aperture was generated [tpf, tesscut, eleanor]
+        :param source: the source where the aperture was generated [tpf, tesscut]
         :param apertures: a dict mapping sectors to boolean apertures
         :param cpus: cores to be used
         :return: the directory where resulting data is stored
         """
         try:
             sectors = [sectors] if isinstance(sectors, int) else sectors
             sectors_search = None if sectors is not None and len(sectors) == 0 else sectors
```

