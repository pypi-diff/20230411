# Comparing `tmp/opengeode-4.0.4.tar.gz` & `tmp/opengeode-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengeode-4.0.4.tar", last modified: Wed Mar  8 09:09:31 2023, max compression
+gzip compressed data, was "opengeode-4.0.6.tar", last modified: Tue Apr 11 08:52:31 2023, max compression
```

## Comparing `opengeode-4.0.4.tar` & `opengeode-4.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-03-08 09:09:31.966554 opengeode-4.0.4/
--rw-r--r--   0 taste     (1001) taste     (1001)     4673 2022-05-15 08:02:36.000000 opengeode-4.0.4/FONT-LICENCE.txt
--rw-r--r--   0 taste     (1001) taste     (1001)     7651 2022-05-15 08:02:36.000000 opengeode-4.0.4/LICENSE
--rw-r--r--   0 taste     (1001) taste     (1001)       54 2022-05-15 08:02:36.000000 opengeode-4.0.4/MANIFEST.in
--rw-r--r--   0 taste     (1001) taste     (1001)    43124 2023-03-08 09:09:31.966554 opengeode-4.0.4/PKG-INFO
--rw-r--r--   0 taste     (1001) taste     (1001)    33797 2023-03-08 09:09:18.000000 opengeode-4.0.4/README.md
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-03-08 09:09:31.966554 opengeode-4.0.4/opengeode/
--rw-r--r--   0 taste     (1001) taste     (1001)   155612 2023-02-01 06:37:47.000000 opengeode-4.0.4/opengeode/AdaGenerator.py
--rwxr-xr-x   0 taste     (1001) taste     (1001)    13962 2022-09-04 10:24:18.000000 opengeode-4.0.4/opengeode/Asn1scc.py
--rw-r--r--   0 taste     (1001) taste     (1001)   116013 2022-11-13 15:59:02.000000 opengeode-4.0.4/opengeode/CGenerator.py
--rw-r--r--   0 taste     (1001) taste     (1001)    11635 2022-09-18 13:58:55.000000 opengeode-4.0.4/opengeode/Clipboard.py
--rw-r--r--   0 taste     (1001) taste     (1001)    29689 2022-12-08 11:28:57.000000 opengeode-4.0.4/opengeode/Connectors.py
--rw-r--r--   0 taste     (1001) taste     (1001)    38631 2022-11-26 14:13:17.000000 opengeode-4.0.4/opengeode/Helper.py
--rw-r--r--   0 taste     (1001) taste     (1001)     9978 2022-05-15 08:02:36.000000 opengeode-4.0.4/opengeode/Lander.py
--rw-r--r--   0 taste     (1001) taste     (1001)    82924 2023-01-22 14:09:04.000000 opengeode-4.0.4/opengeode/LlvmGenerator.py
--rw-r--r--   0 taste     (1001) taste     (1001)    16987 2023-01-03 11:07:49.000000 opengeode-4.0.4/opengeode/Pr.py
--rw-r--r--   0 taste     (1001) taste     (1001)     2462 2022-05-15 08:02:36.000000 opengeode-4.0.4/opengeode/QGenSDL.py
--rw-r--r--   0 taste     (1001) taste     (1001)    15873 2023-01-03 10:27:29.000000 opengeode-4.0.4/opengeode/Renderer.py
--rw-r--r--   0 taste     (1001) taste     (1001)    36467 2022-08-25 09:25:42.000000 opengeode-4.0.4/opengeode/Statechart.py
--rw-r--r--   0 taste     (1001) taste     (1001)    73348 2022-07-25 21:01:25.000000 opengeode-4.0.4/opengeode/StgBackend.py
--rw-r--r--   0 taste     (1001) taste     (1001)    18658 2022-11-04 15:55:28.000000 opengeode-4.0.4/opengeode/TextInteraction.py
--rw-r--r--   0 taste     (1001) taste     (1001)     1058 2022-05-15 08:02:36.000000 opengeode-4.0.4/opengeode/__init__.py
--rw-r--r--   0 taste     (1001) taste     (1001)    57538 2022-12-30 23:55:15.000000 opengeode-4.0.4/opengeode/genericSymbols.py
--rw-r--r--   0 taste     (1001) taste     (1001) 21475752 2023-02-01 06:37:57.000000 opengeode-4.0.4/opengeode/icons.py
--rw-r--r--   0 taste     (1001) taste     (1001)    44341 2023-01-03 15:35:13.000000 opengeode-4.0.4/opengeode/ogAST.py
--rw-r--r--   0 taste     (1001) taste     (1001)   334820 2023-03-08 09:09:18.000000 opengeode-4.0.4/opengeode/ogParser.py
--rw-r--r--   0 taste     (1001) taste     (1001)   147716 2023-01-22 14:13:21.000000 opengeode-4.0.4/opengeode/opengeode.py
--rw-r--r--   0 taste     (1001) taste     (1001)   182007 2022-12-30 16:37:58.000000 opengeode-4.0.4/opengeode/sdl92Lexer.py
--rw-r--r--   0 taste     (1001) taste     (1001)  4596689 2022-12-30 16:37:58.000000 opengeode-4.0.4/opengeode/sdl92Parser.py
--rw-r--r--   0 taste     (1001) taste     (1001)     2077 2022-10-06 09:09:20.000000 opengeode-4.0.4/opengeode/sdlHelp.py
--rw-r--r--   0 taste     (1001) taste     (1001)    64288 2023-02-01 06:37:47.000000 opengeode-4.0.4/opengeode/sdlSymbols.py
--rw-r--r--   0 taste     (1001) taste     (1001)     9445 2022-07-25 21:01:25.000000 opengeode-4.0.4/opengeode/undoCommands.py
--rw-r--r--   0 taste     (1001) taste     (1001)      358 2023-03-08 09:09:18.000000 opengeode-4.0.4/opengeode/version.py
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-03-08 09:09:31.966554 opengeode-4.0.4/opengeode.egg-info/
--rw-r--r--   0 taste     (1001) taste     (1001)    43124 2023-03-08 09:09:31.000000 opengeode-4.0.4/opengeode.egg-info/PKG-INFO
--rw-r--r--   0 taste     (1001) taste     (1001)      818 2023-03-08 09:09:31.000000 opengeode-4.0.4/opengeode.egg-info/SOURCES.txt
--rw-r--r--   0 taste     (1001) taste     (1001)        1 2023-03-08 09:09:31.000000 opengeode-4.0.4/opengeode.egg-info/dependency_links.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       61 2023-03-08 09:09:31.000000 opengeode-4.0.4/opengeode.egg-info/entry_points.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       10 2023-03-08 09:09:31.000000 opengeode-4.0.4/opengeode.egg-info/top_level.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       38 2023-03-08 09:09:31.966554 opengeode-4.0.4/setup.cfg
--rwxr-xr-x   0 taste     (1001) taste     (1001)     1220 2023-01-22 14:13:21.000000 opengeode-4.0.4/setup.py
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-04-11 08:52:31.713609 opengeode-4.0.6/
+-rw-r--r--   0 taste     (1001) taste     (1001)     4673 2022-05-15 08:02:36.000000 opengeode-4.0.6/FONT-LICENCE.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)     7651 2022-05-15 08:02:36.000000 opengeode-4.0.6/LICENSE
+-rw-r--r--   0 taste     (1001) taste     (1001)       54 2022-05-15 08:02:36.000000 opengeode-4.0.6/MANIFEST.in
+-rw-r--r--   0 taste     (1001) taste     (1001)    43330 2023-04-11 08:52:31.713609 opengeode-4.0.6/PKG-INFO
+-rw-r--r--   0 taste     (1001) taste     (1001)    33955 2023-04-11 08:52:18.000000 opengeode-4.0.6/README.md
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-04-11 08:52:31.713609 opengeode-4.0.6/opengeode/
+-rw-r--r--   0 taste     (1001) taste     (1001)   155612 2023-02-01 06:37:47.000000 opengeode-4.0.6/opengeode/AdaGenerator.py
+-rwxr-xr-x   0 taste     (1001) taste     (1001)    13962 2022-09-04 10:24:18.000000 opengeode-4.0.6/opengeode/Asn1scc.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   116013 2022-11-13 15:59:02.000000 opengeode-4.0.6/opengeode/CGenerator.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    11635 2022-09-18 13:58:55.000000 opengeode-4.0.6/opengeode/Clipboard.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    29689 2022-12-08 11:28:57.000000 opengeode-4.0.6/opengeode/Connectors.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    38631 2022-11-26 14:13:17.000000 opengeode-4.0.6/opengeode/Helper.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    10781 2023-04-11 08:52:18.000000 opengeode-4.0.6/opengeode/Lander.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    82924 2023-01-22 14:09:04.000000 opengeode-4.0.6/opengeode/LlvmGenerator.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    16987 2023-01-03 11:07:49.000000 opengeode-4.0.6/opengeode/Pr.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     2462 2022-05-15 08:02:36.000000 opengeode-4.0.6/opengeode/QGenSDL.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    15873 2023-01-03 10:27:29.000000 opengeode-4.0.6/opengeode/Renderer.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    36467 2022-08-25 09:25:42.000000 opengeode-4.0.6/opengeode/Statechart.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    73348 2022-07-25 21:01:25.000000 opengeode-4.0.6/opengeode/StgBackend.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    18658 2022-11-04 15:55:28.000000 opengeode-4.0.6/opengeode/TextInteraction.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     1058 2022-05-15 08:02:36.000000 opengeode-4.0.6/opengeode/__init__.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    57538 2022-12-30 23:55:15.000000 opengeode-4.0.6/opengeode/genericSymbols.py
+-rw-r--r--   0 taste     (1001) taste     (1001) 21475752 2023-02-01 06:37:57.000000 opengeode-4.0.6/opengeode/icons.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    44341 2023-01-03 15:35:13.000000 opengeode-4.0.6/opengeode/ogAST.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   335946 2023-04-11 08:52:18.000000 opengeode-4.0.6/opengeode/ogParser.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   147717 2023-04-11 08:52:18.000000 opengeode-4.0.6/opengeode/opengeode.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   182007 2022-12-30 16:37:58.000000 opengeode-4.0.6/opengeode/sdl92Lexer.py
+-rw-r--r--   0 taste     (1001) taste     (1001)  4596689 2022-12-30 16:37:58.000000 opengeode-4.0.6/opengeode/sdl92Parser.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     2077 2022-10-06 09:09:20.000000 opengeode-4.0.6/opengeode/sdlHelp.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    64273 2023-03-18 10:17:58.000000 opengeode-4.0.6/opengeode/sdlSymbols.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     9445 2022-07-25 21:01:25.000000 opengeode-4.0.6/opengeode/undoCommands.py
+-rw-r--r--   0 taste     (1001) taste     (1001)      358 2023-04-11 08:52:18.000000 opengeode-4.0.6/opengeode/version.py
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-04-11 08:52:31.713609 opengeode-4.0.6/opengeode.egg-info/
+-rw-r--r--   0 taste     (1001) taste     (1001)    43330 2023-04-11 08:52:31.000000 opengeode-4.0.6/opengeode.egg-info/PKG-INFO
+-rw-r--r--   0 taste     (1001) taste     (1001)      818 2023-04-11 08:52:31.000000 opengeode-4.0.6/opengeode.egg-info/SOURCES.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)        1 2023-04-11 08:52:31.000000 opengeode-4.0.6/opengeode.egg-info/dependency_links.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       61 2023-04-11 08:52:31.000000 opengeode-4.0.6/opengeode.egg-info/entry_points.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       10 2023-04-11 08:52:31.000000 opengeode-4.0.6/opengeode.egg-info/top_level.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       38 2023-04-11 08:52:31.713609 opengeode-4.0.6/setup.cfg
+-rwxr-xr-x   0 taste     (1001) taste     (1001)     1220 2023-01-22 14:13:21.000000 opengeode-4.0.6/setup.py
```

### Comparing `opengeode-4.0.4/FONT-LICENCE.txt` & `opengeode-4.0.6/FONT-LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/LICENSE` & `opengeode-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/PKG-INFO` & `opengeode-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengeode
-Version: 4.0.4
+Version: 4.0.6
 Summary: A free SDL editor for TASTE
 Home-page: http://opengeode.net
 Author: Maxime Perrotin
 Author-email: maxime.perrotin@esa.int
 License: UNKNOWN
 Description: ![OpenGEODE Logo](icons/opengeode4.png)
         
@@ -129,15 +129,21 @@
         There is no runtime, and the generated code is not subject to any license.
         
         The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
         The background pattern was downloaded from www.subtlepatterns.com
         
         Changelog
         =========
-        **4.0.3 (03/2023)**
+        **4.0.6 (04/2023)**
+        - Bugfix: type checking when mixing octet strings and integers
+        
+        **4.0.5 (03/2023)**
+        - Bugfix: alternative symbol could not follow labels
+        
+        **4.0.4 (03/2023)**
         - Improve type checking of raw SEQUENCE expressions
         
         **4.0.3 (01/2023)**
         - Better support for optional fields in sequences
         - Improve synonym parsing
         - Improve checks on ground expressions
```

### Comparing `opengeode-4.0.4/README.md` & `opengeode-4.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,21 @@
 There is no runtime, and the generated code is not subject to any license.
 
 The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
 The background pattern was downloaded from www.subtlepatterns.com
 
 Changelog
 =========
-**4.0.3 (03/2023)**
+**4.0.6 (04/2023)**
+- Bugfix: type checking when mixing octet strings and integers
+
+**4.0.5 (03/2023)**
+- Bugfix: alternative symbol could not follow labels
+
+**4.0.4 (03/2023)**
 - Improve type checking of raw SEQUENCE expressions
 
 **4.0.3 (01/2023)**
 - Better support for optional fields in sequences
 - Improve synonym parsing
 - Improve checks on ground expressions
```

### Comparing `opengeode-4.0.4/opengeode/AdaGenerator.py` & `opengeode-4.0.6/opengeode/AdaGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Asn1scc.py` & `opengeode-4.0.6/opengeode/Asn1scc.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/CGenerator.py` & `opengeode-4.0.6/opengeode/CGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Clipboard.py` & `opengeode-4.0.6/opengeode/Clipboard.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Connectors.py` & `opengeode-4.0.6/opengeode/Connectors.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Helper.py` & `opengeode-4.0.6/opengeode/Helper.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Lander.py` & `opengeode-4.0.6/opengeode/Lander.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,30 @@
 
     SDL is the Specification and Description Language (Z100 standard from ITU)
 
     Copyright (c) 2012-2013 European Space Agency
 
     Designed and implemented by Maxime Perrotin
 
-    This module is an easter egg.
-
-    Credits:
-    Rendering algorithm to transform graphviz b-splines to to Qt bezier curves
-    was developed by Steve Dodier-Lazaro (www.mupuf.org)
+    This module is an easter egg, inspired by an old DOS basic game (LANDER.BAS).
 
     Contact: maxime.perrotin@esa.int
 """
 import logging
 import math
 import random
 
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 from PySide6.QtUiTools import QUiLoader
 
 try:
-    from PySide import phonon
+    from PySide6.QtMultimedia import *
 except ImportError:
-    # In some distributions, phonon cannot be installed properly
-    # Discard - but sound will not work.
-    # alternative to be checked for pyside2
     pass
 
 from . import genericSymbols, icons
 
 LOG = logging.getLogger(__name__)
 
 
@@ -45,49 +38,54 @@
     _unique_followers = []
     _insertable_followers = []
     _terminal_followers = []
 
     def __init__(self):
         ''' Initialization: compute the polygon shape '''
         super().__init__(parent=None)
-        self.set_shape(30, 60)
-        self.setBrush(QtGui.QBrush(QtGui.QColor(255, 255, 202)))
+        self.set_shape(30, 40)
+        self.setBrush(QBrush(QColor(255, 255, 255)))
         # Set the rotation origin point
         self.setTransformOriginPoint(self.boundingRect().center())
 
     def set_shape(self, width, height):
         ''' Define the polygon shape from width and height '''
-        path = QtGui.QPainterPath()
+        path = QPainterPath()
         path.moveTo(width / 2, 0)
         path.lineTo(width / 3, height / 6)
         path.lineTo(width / 3, height - height / 6)
         path.lineTo(width - width / 3, height - height / 6)
         path.lineTo(width - width / 3, height / 6)
         path.lineTo(width / 2, 0)
+
+        # left booster
         path.moveTo(width / 3, height / 2)
-        path.lineTo(0, height / 2)
-        path.lineTo(0, height)
-        path.lineTo(width / 6, height - height / 6)
+        path.lineTo(width / 6, height / 2)
+        path.lineTo(width / 6, height)
+        path.lineTo(width / 4, height - height / 6)
         path.lineTo(width / 3, height)
         path.lineTo(width / 3, height - height / 6)
+        # right booster
         path.moveTo(width - width / 3, height / 2)
-        path.lineTo(width, height / 2)
-        path.lineTo(width, height)
-        path.lineTo(width - width / 6, height - height / 6)
+        path.lineTo(width-(width/6), height / 2)
+        path.lineTo(width-(width/6), height)
+        path.lineTo(width - width / 4, height - height / 6)
         path.lineTo(width - width / 3, height)
         path.lineTo(width - width / 3, height - height / 6)
         self.setPath(path)
         super().set_shape(width, height)
 
     def _rotation(self):
         ''' Qt Property that can be used in animations '''
         return self.rotation()
 
     def _set_rotation(self, value):
         ''' Qt Property that can be used in animations '''
+        if value == 360:
+            value = 0
         self.setRotation(value)
 
     angle = Property(float, _rotation, _set_rotation)
 
     def resize_item(self, _):
         ''' Redefine the resizing function - forbid resizing '''
         pass
@@ -102,160 +100,192 @@
         pass
 
     def mouse_release(self, _):
         ''' Mouse has no effect on the rocket '''
         pass
 
 
-class Lander(object):
+class Lander:
     ''' Rocket Lander '''
     def __init__(self, scene):
         ''' Initialize the game '''
         self.scene = scene
         scene.scene_left.connect(self.quit_scene)
         self.rocket = Rocket()
         self.width = self.scene.sceneRect().width()
         self.height = self.scene.sceneRect().height()
 
         self.screen_bottom = self.height - self.rocket.boundingRect().height()
         scene.addItem(self.rocket)
 
-        # Compute random land points
+        # Compute random land field
+        lp = 150
+        lx = [0] * lp
+        ly = [0] * lp
+        lax = [0] * lp
+        lay = [0] * lp
+        lx[0] = 0
+        ly[0] = 40
+        for i in range (1, lp):
+            lx[i] = i * self.width / lp
+
         random.seed()
-        p1 = QPointF(0.0, random.uniform(0.0, self.height))
-        p2 = QPointF(random.uniform(0.0, self.width / 4.0),
-                    random.uniform(0.0, self.height))
-        p3 = QPointF(random.uniform(p2.x(), 2 * self.width / 3.0), self.height)
-        p4 = QPointF(p3.x() + 40.0, self.height)
-        p5 = QPointF(self.width, random.uniform(0.0, self.height))
+        p1 = QPointF(0, 0)
         path = QPainterPath(p1)
-        slope = (p2.y() - p1.y()) / (p2.x() - p1.x())
-        sign = 3
-        for point in range(int((p2.x() - p1.x()) / 5)):
-            sign = -sign
-            x = p1.x() + point * 5
-            path.lineTo(x, slope * x + sign)
-        path.lineTo(p2)
-        path.lineTo(p3)
-        path.lineTo(p4)
-        path.lineTo(p5)
-        scene.addPath(path)
+        # Define coordinates of the landing area
+        bot = self.width * random.uniform(0, 1)
+        for i in range(1, lp):
+            # Determine the angle between the current x-coordinate and the landing field
+            angle = math.pi * (lx[i] - bot - 15) / (self.width * 1.5)
+            # Determine the y-coordinate based on the cosine of the angle
+            ly[i] = ly[0] + (self.height - ly[0]) * abs(math.cos(angle))
+            # Add some random noise to the y-coordinate to make the land contour look more realistic
+            ly[i] += math.sqrt(ly[i]) * (0.5 - random.uniform(0, 1))
+            # If the point falls within the landing field, set its y-coordinate to the height of the landing field
+            if bot < lx[i] < bot + 30:
+                ly[i] = self.height - 2
+            # Prevent overflow of the screen
+            if ly[i] > self.height - 2:
+                ly[i] = self.height - 2
+            # Draw a line segment connecting the current point to the previous point
+            path.lineTo(lx[i], ly[i])
+        path.lineTo(lx[i], self.height)
+        path.lineTo(0, self.height)
+        path.lineTo(0,0)
+        brush = QBrush(QColor(246, 241, 213))
+        self.landscape = scene.addPath(path, brush=brush)
+
+        # Define parameters used to control the physics
+        self.thrust = 10
+        self.tilt = 0  # used to index "ang" hich is the angle in degree
+        self.speed_x = 30
+        self.speed_y = 0
+        self.x = 0
+        self.y = 0
+        self.gravity = 10
+        self.fuel = 4000
+        # these are the possible angles (0 = vertical)
+        # the arrows allow to go from one to the next
+        self.ang = [0, 15, 30, 45, 60, 90, 180, 270, 285, 300, 315, 330, 345]
+        self.nang = len(self.ang)    # number of angles
+
+        # landing pad
+        brush = QBrush(QColor(228, 48, 32)) # red from Tintin's rocket
+        path=QPainterPath()
+        x1, y1 = bot, self.height - 15
+        x2, y2 = bot + 30, self.height
+        path.addRect(x1, y1, x2-x1, y2-y1)
+        self.pad = scene.addPath(path, brush=brush)
 
         # Initialize the music
         try:
-            self.music = phonon.Phonon.createPlayer(
-                    phonon.Phonon.MusicCategory,
-                    phonon.Phonon.MediaSource(':/lander.mp3'))
+            self.music = QMediaPlayer()
+            audioOutput = QAudioOutput()
+            self.music.setAudioOutput(audioOutput)
+            self.music.setSource(QUrl.fromLocalFile('lander.mp3'))
         except NameError:
-            LOG.warning('Could not initialise phonon')
+            LOG.warning('Could not initialise QtMultimedia')
         # Initialize the animation for the translation of the rocket
-        self.animation = QPropertyAnimation(self.rocket, "position")
-        self.rocket_position = None
+        self.animation = QPropertyAnimation(self.rocket, b"position")
         # Initialize the animation for the rotation of the rocket
-        self.rotation = QPropertyAnimation(self.rocket, "angle")
+        self.rotation = QPropertyAnimation(self.rocket, b"angle")
 
         # Catch the key events to add user interaction:
         self.scene.keyPressEvent = lambda x: self.key(x)
 
         # updateCurrentTime is called by Qt when time changes
         self.animation.updateCurrentTime = lambda x: self.time_progress(x)
         # Connect signal sent at end of animation
         self.animation.finished.connect(self.animation_finished)
 
     def time_progress(self, time_value):
-        ''' Called when time changes - used to estimate rocket speed '''
+        ''' Called when time changes - not used '''
         # Call super function - it computes the new position
         super(QPropertyAnimation,
                 self.animation).updateCurrentTime(time_value)
-        if self.rocket.pos().y() - self.rocket_position.y() > 0.1:
-            self.rocket.speed = 'high'
-        else:
-            self.rocket.speed = 'low'
-        self.rocket_position = self.rocket.pos()
 
     def key(self, evt):
         ''' Handling of key press event '''
         # Discard keys if there is a running rotation animation
         if self.rotation.state() != QAbstractAnimation.Stopped:
             return
-        self.rotation.setDuration(500)
-        self.rotation.setStartValue(self.rocket.angle)
+        self.rotation.setDuration(200)
         self.rotation.setEasingCurve(QEasingCurve.Linear)
         if evt.key() == Qt.Key_Right:
-            self.rotation.setEndValue(self.rocket.angle + 30.0)
+            self.tilt = self.tilt + 1 if self.tilt < self.nang - 1 else 0
+            end_value = self.ang[self.tilt] if self.tilt != 0 else 360
+            self.rotation.setStartValue(self.rocket.angle)
+            self.rotation.setEndValue(end_value)
             self.rotation.start()
         elif evt.key() == Qt.Key_Left:
-            self.rotation.setEndValue(self.rocket.angle - 30.0)
+            if self.tilt == 0:
+                self.rocket.setRotation(360)
+                self.tilt = self.nang - 1
+            else:
+                self.tilt -= 1
+            end_value = self.ang[self.tilt]
+            self.rotation.setStartValue(self.rocket.angle)
+            self.rotation.setEndValue(end_value)
             self.rotation.start()
         elif evt.key() == Qt.Key_Up:
-            # Up key action depends on current speed and angle
-            self.animation.stop()
-            end_value = self.animation.endValue()
-            remaining_time = (self.animation.totalDuration() -
-                             self.animation.currentTime())
-            if 90 < abs(self.rocket.angle) < 270:
-                # If the rocket nose is towards Earth
-                nose = 'down'
-                delta_y = -(self.screen_bottom - self.rocket.y())
-                hypo = delta_y / math.cos(math.radians(self.rocket.angle))
-                delta_x = hypo * math.sin(math.radians(self.rocket.angle))
-            else:
-                nose = 'up'
-                delta_x = 70.0 * math.sin(math.radians(self.rocket.angle))
-                delta_y = 70.0 * math.cos(math.radians(-self.rocket.angle))
-            if(nose == 'up' and end_value.y() > self.rocket.y() and
-                    self.rocket.speed == 'high'):
-                # Delay impact time by 2 seconds if going down at high speed
-                self.animation.setDuration(remaining_time + 2000)
-                self.animation.setStartValue(self.rocket.pos())
-                self.animation.start()
-                return
-            elif end_value.y() > self.rocket.y() and (
-                    self.rocket.speed == 'low' or nose == 'down'):
-                end_value.setX(self.rocket.x() + delta_x)
-                end_value.setY(self.rocket.y() - delta_y)
-            else:
-                end_value.setX(end_value.x() + delta_x)
-                end_value.setY(end_value.y() - delta_y)
-            self.animation.setDuration(2000)
-            self.animation.setEasingCurve(QEasingCurve.InOutExpo)
-            self.animation.setStartValue(self.rocket.pos())
-            self.animation.setEndValue(end_value)
-            self.animation.start()
-
+            self.thrust = self.thrust + 1 if self.thrust < 19 else 19
         elif evt.key() == Qt.Key_Down:
-            # Down key has no effect
-            pass
+            # Reduce thrust
+            self.thrust = self.thrust - 1 if self.thrust > 0 else 0
         else:
             pass
 
     def play(self):
         ''' Run the game '''
-        self.rocket.setPos(0, 0)
+        self.rocket.setPos(self.x, self.y)
         try:
             self.music.play()
         except AttributeError:
             pass
-        self.animation.setDuration(20000)
+        self.animation.setDuration(200)
         self.animation.setStartValue(self.rocket.pos())
-        # Store initial position - used to compute rocket speed
-        self.rocket_position = self.rocket.pos()
-        self.animation.setEndValue(QPointF(350, self.screen_bottom))
+        self.update_control()   # compute next position
+        self.animation.setEndValue(QPointF(self.x, self.y))
         self.animation.setEasingCurve(QEasingCurve.InCirc)
         self.animation.start()
 
+    def update_control(self):
+        ''' Compute position and speed based on thrust and tilt '''
+        # Update control
+        self.speed_y += self.gravity - self.thrust * math.cos(math.pi * self.ang[self.tilt] / 180)
+        self.speed_x = 0.9 * self.speed_x + self.thrust * math.sin(math.pi * self.ang[self.tilt] / 180)
+        if self.speed_y < -10:
+            self.speed_y = -10
+        self.x += self.speed_x * 0.05
+        self.y += self.speed_y * 0.05
+        if self.y < 0:
+            self.y = 0
+        self.fuel = self.fuel - self.thrust
+        if self.fuel < 0:
+            self.fuel = 0
+
     def animation_finished(self):
         ''' When animation is finished, check if another one is needed '''
+        for item in self.rocket.collidingItems():
+            if item == self.landscape:
+                print("CRASH - GAME OVER")
+                return
+            elif item == self.pad:
+                if self.speed_y < 100:
+                    print ("CONGRATULATIONS")
+                else:
+                    print ("TOO FAST ! GAME OVER")
+                    print (self.speed_y)
+                return
         if self.rocket.y() < self.screen_bottom:
-            end_value = self.animation.endValue()
-            end_value.setY(self.screen_bottom)
+            self.update_control()
+            self.animation.setEndValue(QPointF(self.x, self.y))
             self.animation.setStartValue(self.rocket.pos())
-            self.animation.setEndValue(end_value)
             self.animation.setEasingCurve(QEasingCurve.InCirc)
-            self.animation.setDuration(abs(self.rocket.y()) * 500)
+            self.animation.setDuration(200)
             self.animation.start()
         else:
             print('GAME OVER')
 
     def quit_scene(self):
         ''' Redefinition of the quit_scene: Stop the game and the music '''
         try:
```

### Comparing `opengeode-4.0.4/opengeode/LlvmGenerator.py` & `opengeode-4.0.6/opengeode/LlvmGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Pr.py` & `opengeode-4.0.6/opengeode/Pr.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/QGenSDL.py` & `opengeode-4.0.6/opengeode/QGenSDL.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Renderer.py` & `opengeode-4.0.6/opengeode/Renderer.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/Statechart.py` & `opengeode-4.0.6/opengeode/Statechart.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/StgBackend.py` & `opengeode-4.0.6/opengeode/StgBackend.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/TextInteraction.py` & `opengeode-4.0.6/opengeode/TextInteraction.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/__init__.py` & `opengeode-4.0.6/opengeode/__init__.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/genericSymbols.py` & `opengeode-4.0.6/opengeode/genericSymbols.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/icons.py` & `opengeode-4.0.6/opengeode/icons.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/ogAST.py` & `opengeode-4.0.6/opengeode/ogAST.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/ogParser.py` & `opengeode-4.0.6/opengeode/ogParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1516,28 +1516,37 @@
                     and not (is_number(type_a) or is_number(type_b)):
                 raise TypeError("Signed vs Unsigned type mismatch " +
                         mismatch)
             elif mismatch:
                 warnings.append(mismatch)
         elif mismatch:
             warnings.append(mismatch)
-        #print traceback.print_stack()
         return warnings
     elif is_string(type_a) and is_string(type_b):
         return warnings
     elif is_integer(type_a) and is_integer(type_b):
         if mismatch:
             warnings.append(mismatch)
         return warnings
     elif is_real(type_a) and is_real(type_b):
         if mismatch:
             warnings.append(mismatch)
         return warnings
     elif is_integer(type_a) and type_b.kind == 'OctetStringType' \
             or is_integer(type_b) and type_a.kind == 'OctetStringType':
+        # Here we have an octet string and a number. This is usually
+        # a type mismatch (e.g. octStr // 5 is wrong, usser must use
+        # mkstring to convert the integer to an appendable string).
+        # However there is one exception, if the octet string is a
+        # raw string: 'FF'H + 1 is valid.
+        if (is_integer(type_a) and type_b.__name__ != 'PrStr') or \
+            (is_integer(type_b) and type_a.__name__ != 'PrStr'):
+            #traceback.print_stack()
+            #breakpoint()
+            raise TypeError(f'Try using mkstring')
         if mismatch:
             warnings.append(mismatch)
         return warnings
 
     else:
         raise TypeError('Incompatible types {} and {}'.format(
             type_name(type_a),
@@ -3751,15 +3760,17 @@
             if proc.exported:
                 # Exported procedures are called from remotely: update SENDER
                 get_sender, _, e1, w1, t1 = parseSingleElement('procedure_call',
                     'call get_sender(sender);', proc)
                 get_sender.no_render = True
                 if not e1:
                     # No error means the function is defined => insert the call
-                    proc.content.start.transition.actions.insert(0, get_sender)
+                    if hasattr(proc.content.start, 'transition') and \
+                            proc.content.start.transition is not None:
+                        proc.content.start.transition.actions.insert(0, get_sender)
             errors.extend(err)
             warnings.extend(warn)
         elif child.type == lexer.FLOATING_LABEL:
             lab, err, warn = floating_label(child, parent=None, context=proc)
             errors.extend(err)
             warnings.extend(warn)
             proc.content.floating_labels.append(lab)
@@ -5946,20 +5957,31 @@
                           lexer.OPEN_RANGE, lexer.INFORMAL_TEXT):
             #ans.inputString = get_input_string(child)
             ans.inputString = token_stream(child).toString(startIndex, stopIndex)
             ans.line = child.getLine()
             ans.charPositionInLine = child.getCharPositionInLine()
             # Report errors with symbol coordinates
             x, y = (ans.pos_x or 0, ans.pos_y or 0)
-            errors = [[e, [x, y], []] for e in errors]
-            warnings = [[w, [x, y], []] for w in warnings]
+            # there can be multiple answers (we are in a loop) so we must
+            # make sure that we don't process the same error/warnings
+            # multiple times when adding the coordinates
+            errs, warns = [], []
             for e in errors:
-                ans.errors.append(e[0])
+                if isinstance(e, str):
+                    errs.append([e, [x, y], []])
+                    ans.errors.append(e)
+                else:
+                    errs.append(e)
             for w in warnings:
-                ans.warnings.append(w[0])
+                if isinstance(w, str):
+                    warns.append([w, [x, y], []])
+                    ans.warnings.append(w)
+                else:
+                    warns.append(w)
+            errors, warnings = errs, warns
     return ans, errors, warnings
 
 def alternative(root, parent, context):
     return decision(root, parent, context)
 
 def decision(root, parent, context):
     ''' Parse a DECISION '''
```

### Comparing `opengeode-4.0.4/opengeode/opengeode.py` & `opengeode-4.0.6/opengeode/opengeode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1773,15 +1773,15 @@
         elif event.key() == Qt.Key_F5:
             self.refresh()
         elif event.matches(QKeySequence.Open):
             self.open_diagram()
         elif event.matches(QKeySequence.New):
             self.new_diagram()
         elif (event.key() == Qt.Key_F12 and
-                event.modifiers() == Qt.ControlModifier and
+                #event.modifiers() == Qt.ControlModifier and
                 self.scene() != self.lander_scene):
             self.lander_scene.setSceneRect(0, 0, self.width(), self.height())
             if not self.lander:
                 self.lander = Lander.Lander(self.lander_scene)
             horpos = self.horizontalScrollBar().value()
             verpos = self.verticalScrollBar().value()
             self.scene_stack.append((self.scene(), horpos, verpos))
```

### Comparing `opengeode-4.0.4/opengeode/sdl92Lexer.py` & `opengeode-4.0.6/opengeode/sdl92Lexer.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/sdl92Parser.py` & `opengeode-4.0.6/opengeode/sdl92Parser.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/sdlHelp.py` & `opengeode-4.0.6/opengeode/sdlHelp.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode/sdlSymbols.py` & `opengeode-4.0.6/opengeode/sdlSymbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,17 +713,17 @@
         return 'STOP'
 
 
 # pylint: disable=R0904
 class Label(VerticalSymbol):
     ''' LABEL symbol '''
     _insertable_followers = ['Create',
-            'Task', 'ProcedureCall', 'Output', 'Decision', 'Label']
-    _terminal_followers = ['Join', 'State', 'ProcedureStop', 'ProcessStop',
-                           'Alternative']
+            'Task', 'ProcedureCall', 'Output', 'Decision', 'Label',
+            'Alternative']
+    _terminal_followers = ['Join', 'State', 'ProcedureStop', 'ProcessStop']
     needs_parent = False
     # Define reserved keywords for the syntax highlighter
     blackbold = SDL_BLACKBOLD
     redbold = SDL_REDBOLD
     # Symbol must not use antialiasing, otherwise the middle line is too thick
     _antialiasing = False
```

### Comparing `opengeode-4.0.4/opengeode/undoCommands.py` & `opengeode-4.0.6/opengeode/undoCommands.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/opengeode.egg-info/PKG-INFO` & `opengeode-4.0.6/opengeode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengeode
-Version: 4.0.4
+Version: 4.0.6
 Summary: A free SDL editor for TASTE
 Home-page: http://opengeode.net
 Author: Maxime Perrotin
 Author-email: maxime.perrotin@esa.int
 License: UNKNOWN
 Description: ![OpenGEODE Logo](icons/opengeode4.png)
         
@@ -129,15 +129,21 @@
         There is no runtime, and the generated code is not subject to any license.
         
         The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
         The background pattern was downloaded from www.subtlepatterns.com
         
         Changelog
         =========
-        **4.0.3 (03/2023)**
+        **4.0.6 (04/2023)**
+        - Bugfix: type checking when mixing octet strings and integers
+        
+        **4.0.5 (03/2023)**
+        - Bugfix: alternative symbol could not follow labels
+        
+        **4.0.4 (03/2023)**
         - Improve type checking of raw SEQUENCE expressions
         
         **4.0.3 (01/2023)**
         - Better support for optional fields in sequences
         - Improve synonym parsing
         - Improve checks on ground expressions
```

### Comparing `opengeode-4.0.4/opengeode.egg-info/SOURCES.txt` & `opengeode-4.0.6/opengeode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengeode-4.0.4/setup.py` & `opengeode-4.0.6/setup.py`

 * *Files identical despite different names*

