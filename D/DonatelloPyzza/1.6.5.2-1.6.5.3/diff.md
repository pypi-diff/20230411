# Comparing `tmp/donatellopyzza-1.6.5.2.tar.gz` & `tmp/donatellopyzza-1.6.5.3.tar.gz`

## Comparing `donatellopyzza-1.6.5.2.tar` & `donatellopyzza-1.6.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/__init__.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/assessor.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/envBuilder.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/game.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/main_assessor.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/main_generate.py
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/mazeGenerator.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/turtleAgent.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/environments/assessment_maze.png
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/environments/assessment_maze.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/environments/hard_maze.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/environments/maze.txt
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/environments/test.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/environments/test.txt
--rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/images/pizza.png
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/images/turtle.png
--rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/data/images/turtle_small.png
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/__init__.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/agent.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/careTaker.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/constants.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/grid.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/gui.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/map.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/mazeParser.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/memento.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/orientation.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/originator.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/square.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/donatellopyzza/grid/turn.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/.gitignore
--rw-r--r--   0        0        0    22304 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/LICENSE
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/README.md
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/pyproject.toml
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.2/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/__init__.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/assessor.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/envBuilder.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/game.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/main_assessor.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/main_generate.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/mazeGenerator.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/turtleAgent.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/environments/assessment_maze.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/environments/assessment_maze.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/environments/hard_maze.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/environments/maze.txt
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/environments/test.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/environments/test.txt
+-rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/images/pizza.png
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/images/turtle.png
+-rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/data/images/turtle_small.png
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/__init__.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/agent.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/careTaker.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/constants.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/grid.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/gui.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/map.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/mazeParser.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/memento.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/orientation.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/originator.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/square.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/donatellopyzza/grid/turn.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/.gitignore
+-rw-r--r--   0        0        0    22304 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/LICENSE
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 donatellopyzza-1.6.5.3/PKG-INFO
```

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/assessor.py` & `donatellopyzza-1.6.5.3/donatellopyzza/assessor.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/envBuilder.py` & `donatellopyzza-1.6.5.3/donatellopyzza/envBuilder.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/game.py` & `donatellopyzza-1.6.5.3/donatellopyzza/game.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/main_assessor.py` & `donatellopyzza-1.6.5.3/donatellopyzza/main_assessor.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/main_generate.py` & `donatellopyzza-1.6.5.3/donatellopyzza/main_generate.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/mazeGenerator.py` & `donatellopyzza-1.6.5.3/donatellopyzza/mazeGenerator.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/data/environments/assessment_maze.png` & `donatellopyzza-1.6.5.3/donatellopyzza/data/environments/assessment_maze.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/data/environments/test.png` & `donatellopyzza-1.6.5.3/donatellopyzza/data/environments/test.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/data/images/pizza.png` & `donatellopyzza-1.6.5.3/donatellopyzza/data/images/pizza.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/data/images/turtle.png` & `donatellopyzza-1.6.5.3/donatellopyzza/data/images/turtle.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/data/images/turtle_small.png` & `donatellopyzza-1.6.5.3/donatellopyzza/data/images/turtle_small.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/grid/agent.py` & `donatellopyzza-1.6.5.3/donatellopyzza/grid/agent.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/grid/grid.py` & `donatellopyzza-1.6.5.3/donatellopyzza/grid/grid.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/grid/gui.py` & `donatellopyzza-1.6.5.3/donatellopyzza/grid/gui.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/grid/map.py` & `donatellopyzza-1.6.5.3/donatellopyzza/grid/map.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/grid/mazeParser.py` & `donatellopyzza-1.6.5.3/donatellopyzza/grid/mazeParser.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/donatellopyzza/grid/square.py` & `donatellopyzza-1.6.5.3/donatellopyzza/grid/square.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/LICENSE` & `donatellopyzza-1.6.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/README.md` & `donatellopyzza-1.6.5.3/README.md`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.5.2/pyproject.toml` & `donatellopyzza-1.6.5.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "pygame ~= 2.1.2", "tqdm"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DonatelloPyzza"
-version = "1.6.5.2"
+version = "1.6.5.3"
 authors = [
   { name="Mickaël Bettinelli", email="mickael.bettinelli@univ-smb.fr" },
 ]
 description = "A simple and educational game to learn algorithmic where you can develop the behavior of a turtle to move in a maze."
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
@@ -20,8 +20,8 @@
 [project.urls]
 "Homepage" = "https://github.com/MilowB/Donatello"
 "Bug Tracker" = "https://github.com/MilowB/Donatello/pulls"
 
 [tool.hatch.build]
 include = [
   "donatellopyzza/*"
-]
+]
```

### Comparing `donatellopyzza-1.6.5.2/PKG-INFO` & `donatellopyzza-1.6.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DonatelloPyzza
-Version: 1.6.5.2
+Version: 1.6.5.3
 Summary: A simple and educational game to learn algorithmic where you can develop the behavior of a turtle to move in a maze.
 Project-URL: Homepage, https://github.com/MilowB/Donatello
 Project-URL: Bug Tracker, https://github.com/MilowB/Donatello/pulls
 Author-email: Mickaël Bettinelli <mickael.bettinelli@univ-smb.fr>
 License-File: LICENSE
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

