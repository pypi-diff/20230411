# Comparing `tmp/pygex-0.1.8.tar.gz` & `tmp/pygex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygex-0.1.8.tar", last modified: Tue Apr  4 02:51:45 2023, max compression
+gzip compressed data, was "pygex-0.1.9.tar", last modified: Tue Apr 11 00:30:01 2023, max compression
```

## Comparing `pygex-0.1.8.tar` & `pygex-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 02:51:45.252511 pygex-0.1.8/
--rw-rw-rw-   0        0        0     4352 2023-04-04 02:51:45.252511 pygex-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3615 2023-02-27 04:04:04.000000 pygex-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 02:51:45.218488 pygex-0.1.8/pygex/
--rw-rw-rw-   0        0        0       65 2023-03-21 02:22:05.000000 pygex-0.1.8/pygex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:51:45.238501 pygex-0.1.8/pygex/animation/
--rw-rw-rw-   0        0        0      178 2023-02-23 18:55:51.000000 pygex-0.1.8/pygex/animation/__init__.py
--rw-rw-rw-   0        0        0     1658 2023-02-23 18:47:34.000000 pygex-0.1.8/pygex/animation/animator.py
--rw-rw-rw-   0        0        0     1135 2023-02-23 18:18:49.000000 pygex-0.1.8/pygex/animation/curves.py
--rw-rw-rw-   0        0        0     1129 2023-02-23 19:00:54.000000 pygex-0.1.8/pygex/animation/target_animator.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:51:45.242517 pygex-0.1.8/pygex/core/
--rw-rw-rw-   0        0        0       35 2023-03-14 00:25:18.000000 pygex-0.1.8/pygex/core/__init__.py
--rw-rw-rw-   0        0        0     3306 2023-04-04 02:49:35.000000 pygex-0.1.8/pygex/core/application.py
--rw-rw-rw-   0        0        0     3022 2023-03-14 21:26:30.000000 pygex-0.1.8/pygex/core/game_object.py
--rw-rw-rw-   0        0        0     2706 2023-04-04 02:50:04.000000 pygex-0.1.8/pygex/core/input.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:51:45.251510 pygex-0.1.8/pygex/rendering/
--rw-rw-rw-   0        0        0      302 2023-03-25 17:49:54.000000 pygex-0.1.8/pygex/rendering/__init__.py
--rw-rw-rw-   0        0        0    18897 2023-03-16 02:08:18.000000 pygex-0.1.8/pygex/rendering/font.py
--rw-rw-rw-   0        0        0     8643 2023-03-01 23:10:41.000000 pygex-0.1.8/pygex/rendering/geometry.py
--rw-rw-rw-   0        0        0     3152 2023-03-10 02:50:04.000000 pygex-0.1.8/pygex/rendering/render_target.py
--rw-rw-rw-   0        0        0     2793 2023-03-14 00:36:47.000000 pygex-0.1.8/pygex/rendering/renderer.py
--rw-rw-rw-   0        0        0     2399 2023-03-16 02:08:18.000000 pygex-0.1.8/pygex/rendering/shader.py
--rw-rw-rw-   0        0        0     6031 2023-03-16 01:32:16.000000 pygex-0.1.8/pygex/rendering/texture.py
--rw-rw-rw-   0        0        0    11402 2023-03-16 02:08:18.000000 pygex-0.1.8/pygex/rendering/texture_generators.py
--rw-rw-rw-   0        0        0     5289 2023-03-10 11:44:52.000000 pygex-0.1.8/pygex/rendering/utils.py
--rw-rw-rw-   0        0        0    29413 2023-03-21 04:18:19.000000 pygex-0.1.8/pygex/vmath.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:51:45.234487 pygex-0.1.8/pygex.egg-info/
--rw-rw-rw-   0        0        0     4352 2023-04-04 02:51:45.000000 pygex-0.1.8/pygex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      664 2023-04-04 02:51:45.000000 pygex-0.1.8/pygex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 02:51:45.000000 pygex-0.1.8/pygex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-04 02:51:45.000000 pygex-0.1.8/pygex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-04 02:51:45.000000 pygex-0.1.8/pygex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 02:51:45.253515 pygex-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1742 2023-04-04 02:51:31.000000 pygex-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:30:01.030736 pygex-0.1.9/
+-rw-rw-rw-   0        0        0     4352 2023-04-11 00:30:01.030736 pygex-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3615 2023-02-27 04:04:04.000000 pygex-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 00:30:01.003865 pygex-0.1.9/pygex/
+-rw-rw-rw-   0        0        0       65 2023-03-21 02:22:05.000000 pygex-0.1.9/pygex/__init__.py
+-rw-rw-rw-   0        0        0     1975 2023-04-11 00:25:35.000000 pygex-0.1.9/pygex/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:30:01.015866 pygex-0.1.9/pygex/animation/
+-rw-rw-rw-   0        0        0      178 2023-02-23 18:55:51.000000 pygex-0.1.9/pygex/animation/__init__.py
+-rw-rw-rw-   0        0        0     1658 2023-02-23 18:47:34.000000 pygex-0.1.9/pygex/animation/animator.py
+-rw-rw-rw-   0        0        0     1135 2023-02-23 18:18:49.000000 pygex-0.1.9/pygex/animation/curves.py
+-rw-rw-rw-   0        0        0     1129 2023-02-23 19:00:54.000000 pygex-0.1.9/pygex/animation/target_animator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:30:01.019875 pygex-0.1.9/pygex/core/
+-rw-rw-rw-   0        0        0       35 2023-03-14 00:25:18.000000 pygex-0.1.9/pygex/core/__init__.py
+-rw-rw-rw-   0        0        0     3306 2023-04-04 02:49:35.000000 pygex-0.1.9/pygex/core/application.py
+-rw-rw-rw-   0        0        0     3022 2023-03-14 21:26:30.000000 pygex-0.1.9/pygex/core/game_object.py
+-rw-rw-rw-   0        0        0     2706 2023-04-04 02:50:04.000000 pygex-0.1.9/pygex/core/input.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:30:01.029724 pygex-0.1.9/pygex/rendering/
+-rw-rw-rw-   0        0        0      302 2023-03-25 17:49:54.000000 pygex-0.1.9/pygex/rendering/__init__.py
+-rw-rw-rw-   0        0        0    18897 2023-03-16 02:08:18.000000 pygex-0.1.9/pygex/rendering/font.py
+-rw-rw-rw-   0        0        0     8643 2023-03-01 23:10:41.000000 pygex-0.1.9/pygex/rendering/geometry.py
+-rw-rw-rw-   0        0        0     3152 2023-03-10 02:50:04.000000 pygex-0.1.9/pygex/rendering/render_target.py
+-rw-rw-rw-   0        0        0     2793 2023-03-14 00:36:47.000000 pygex-0.1.9/pygex/rendering/renderer.py
+-rw-rw-rw-   0        0        0     2399 2023-03-16 02:08:18.000000 pygex-0.1.9/pygex/rendering/shader.py
+-rw-rw-rw-   0        0        0     6031 2023-03-16 01:32:16.000000 pygex-0.1.9/pygex/rendering/texture.py
+-rw-rw-rw-   0        0        0    11402 2023-03-16 02:08:18.000000 pygex-0.1.9/pygex/rendering/texture_generators.py
+-rw-rw-rw-   0        0        0     5289 2023-03-10 11:44:52.000000 pygex-0.1.9/pygex/rendering/utils.py
+-rw-rw-rw-   0        0        0    29413 2023-03-21 04:18:19.000000 pygex-0.1.9/pygex/vmath.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:30:01.011868 pygex-0.1.9/pygex.egg-info/
+-rw-rw-rw-   0        0        0     4352 2023-04-11 00:30:00.000000 pygex-0.1.9/pygex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2023-04-11 00:30:00.000000 pygex-0.1.9/pygex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 00:30:00.000000 pygex-0.1.9/pygex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-11 00:30:00.000000 pygex-0.1.9/pygex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 00:30:00.000000 pygex-0.1.9/pygex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 00:30:01.031732 pygex-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1742 2023-04-11 00:28:31.000000 pygex-0.1.9/setup.py
```

### Comparing `pygex-0.1.8/PKG-INFO` & `pygex-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygex
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple Python game engine built around pygame and PyOpenGL.
 Home-page: https://github.com/DCubix/pyge
 Author: Diego Lopes
 Author-email: diego95lopes@gmail.com
 License: MIT
 Keywords: python,game,engine,3d,graphics,gamedev
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygex Version: 0.1.8 Summary: A simple Python game
+Metadata-Version: 2.1 Name: pygex Version: 0.1.9 Summary: A simple Python game
 engine built around pygame and PyOpenGL. Home-page: https://github.com/DCubix/
 pyge Author: Diego Lopes Author-email: diego95lopes@gmail.com License: MIT
 Keywords: python,game,engine,3d,graphics,gamedev Description-Content-Type:
 text/markdown
                                     &#xa0;
                               ****** PyGE ******
       [Github top language] [Github language count] [Repository size]
```

### Comparing `pygex-0.1.8/README.md` & `pygex-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/animation/animator.py` & `pygex-0.1.9/pygex/animation/animator.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/animation/curves.py` & `pygex-0.1.9/pygex/animation/curves.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/animation/target_animator.py` & `pygex-0.1.9/pygex/animation/target_animator.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/core/application.py` & `pygex-0.1.9/pygex/core/application.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/core/game_object.py` & `pygex-0.1.9/pygex/core/game_object.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/core/input.py` & `pygex-0.1.9/pygex/core/input.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/font.py` & `pygex-0.1.9/pygex/rendering/font.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/geometry.py` & `pygex-0.1.9/pygex/rendering/geometry.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/render_target.py` & `pygex-0.1.9/pygex/rendering/render_target.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/renderer.py` & `pygex-0.1.9/pygex/rendering/renderer.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/shader.py` & `pygex-0.1.9/pygex/rendering/shader.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/texture.py` & `pygex-0.1.9/pygex/rendering/texture.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/texture_generators.py` & `pygex-0.1.9/pygex/rendering/texture_generators.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/rendering/utils.py` & `pygex-0.1.9/pygex/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex/vmath.py` & `pygex-0.1.9/pygex/vmath.py`

 * *Files identical despite different names*

### Comparing `pygex-0.1.8/pygex.egg-info/PKG-INFO` & `pygex-0.1.9/pygex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygex
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple Python game engine built around pygame and PyOpenGL.
 Home-page: https://github.com/DCubix/pyge
 Author: Diego Lopes
 Author-email: diego95lopes@gmail.com
 License: MIT
 Keywords: python,game,engine,3d,graphics,gamedev
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygex Version: 0.1.8 Summary: A simple Python game
+Metadata-Version: 2.1 Name: pygex Version: 0.1.9 Summary: A simple Python game
 engine built around pygame and PyOpenGL. Home-page: https://github.com/DCubix/
 pyge Author: Diego Lopes Author-email: diego95lopes@gmail.com License: MIT
 Keywords: python,game,engine,3d,graphics,gamedev Description-Content-Type:
 text/markdown
                                     &#xa0;
                               ****** PyGE ******
       [Github top language] [Github language count] [Repository size]
```

### Comparing `pygex-0.1.8/pygex.egg-info/SOURCES.txt` & `pygex-0.1.9/pygex.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 pygex/__init__.py
+pygex/__main__.py
 pygex/vmath.py
 pygex.egg-info/PKG-INFO
 pygex.egg-info/SOURCES.txt
 pygex.egg-info/dependency_links.txt
 pygex.egg-info/requires.txt
 pygex.egg-info/top_level.txt
 pygex/animation/__init__.py
```

### Comparing `pygex-0.1.8/setup.py` & `pygex-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 from setuptools import setup, find_packages, Command
 import shutil, glob, os
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
```

