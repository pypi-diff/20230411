# Comparing `tmp/donatellopyzza-1.6.3.tar.gz` & `tmp/donatellopyzza-1.6.4.tar.gz`

## Comparing `donatellopyzza-1.6.3.tar` & `donatellopyzza-1.6.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/__init__.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/assessor.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/envBuilder.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/game.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/main_assessor.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/main_generate.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/mazeGenerator.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/turtleAgent.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/environments/assessment_maze.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/environments/assessment_maze.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/environments/hard_maze.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/environments/maze.txt
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/environments/test.png
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/environments/test.txt
--rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/images/pizza.png
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/images/turtle.png
--rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/data/images/turtle_small.png
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/agent.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/careTaker.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/constants.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/grid.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/gui.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/map.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/memento.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/orientation.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/originator.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/parser.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/square.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/donatellopyzza/grid/turn.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/LICENSE
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 donatellopyzza-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/__init__.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/assessor.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/envBuilder.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/game.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/main_assessor.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/main_generate.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/mazeGenerator.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/turtleAgent.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/environments/assessment_maze.png
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/environments/assessment_maze.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/environments/hard_maze.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/environments/maze.txt
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/environments/test.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/environments/test.txt
+-rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/images/pizza.png
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/images/turtle.png
+-rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/data/images/turtle_small.png
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/__init__.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/agent.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/careTaker.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/constants.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/grid.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/gui.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/map.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/mazeParser.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/memento.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/orientation.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/originator.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/square.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/donatellopyzza/grid/turn.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/.gitignore
+-rw-r--r--   0        0        0    22304 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/LICENSE
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/README.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 donatellopyzza-1.6.4/PKG-INFO
```

### Comparing `donatellopyzza-1.6.3/donatellopyzza/assessor.py` & `donatellopyzza-1.6.4/donatellopyzza/assessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from random import randint
 from tqdm import tqdm
 import os, sys
 import time
 
-sys.path.insert(0, 'donatellopyzza/')
+#sys.path.insert(0, os.path.abspath('donatellopyzza/'))
 
 from .mazeGenerator import MazeGenerator
 from .game import Feedback
 from .game import Game
 
 
 class Assessor:
```

### Comparing `donatellopyzza-1.6.3/donatellopyzza/envBuilder.py` & `donatellopyzza-1.6.4/donatellopyzza/envBuilder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os, sys, inspect
 import pkg_resources
 from pathlib import Path
 from pkg_resources import resource_string
 
-sys.path.insert(0, 'donatellopyzza/grid')
+sys.path.insert(0, os.path.abspath("donatellopyzza/grid/"))
 
-from parser import Parser
 from grid import Grid
+from mazeParser import Parser
 
 
 class EnvBuilder:
     def __init__(self, name: str, gui: bool):
         self.name = name
         self.gui = gui
```

### Comparing `donatellopyzza-1.6.3/donatellopyzza/game.py` & `donatellopyzza-1.6.4/donatellopyzza/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from .turtleAgent import Turtle
 from .envBuilder import *
-# @DEBUG from .turtleAgent import Turtle
-# @DEBUG from .envBuilder import *
-# @DEBUG from .generator import *
+
 import time
 import random
 from enum import Enum
 
 class Action(Enum):
     MOVE_FORWARD = 0, "Move_forward"
     TURN_RIGHT = 1, "Turn_right"
```

### Comparing `donatellopyzza-1.6.3/donatellopyzza/main_assessor.py` & `donatellopyzza-1.6.4/donatellopyzza/main_assessor.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/main_generate.py` & `donatellopyzza-1.6.4/donatellopyzza/main_generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .mazeGenerator import MazeGenerator
 from .assessor import Assessor
 import random
 
 if __name__ == '__main__':
     # generate and save a new random maze
     generator = MazeGenerator()
-    maze = generator.create_maze(20, 20)
+    maze = generator.create_maze(12, 12)
     fn = "test"
     maze.save(maze, filename=fn)
 
     # load the new maze
     __ENVIRONMENT__ = "test"
     # display the interface (or not)
     __GUI__ = True
```

### Comparing `donatellopyzza-1.6.3/donatellopyzza/mazeGenerator.py` & `donatellopyzza-1.6.4/donatellopyzza/mazeGenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 from matplotlib import colors
 from numpy.random import random_integers as rand
 import os, sys, inspect
 import pkg_resources
 from pkg_resources import resource_string
 from random import randint
 
-#Pour inclure les fichiers de l'environnement
-cmd_subfolder_grid = os.path.realpath(os.path.abspath(os.path.join(os.path.split(inspect.getfile( inspect.currentframe() ))[0],"grid")))
-if cmd_subfolder_grid not in sys.path:
-    sys.path.insert(0, cmd_subfolder_grid)
+sys.path.insert(0, os.path.abspath('donatellopyzza/grid'))
 
 from constants import *
 
 
 class Maze:
     def __init__(self, rows, columns):
         assert rows >= 1 and columns >= 1
@@ -120,43 +117,49 @@
 class MazeGenerator():
     def create_maze(self, nrows, ncolumns, complexity=0, seed=None):
         if nrows <= 9 and ncolumns <= 9:
             print("WARNING: make a maze that have at least 10 rows and 10 columns. "
                 "The generated maze has been sized at 10x10")
             nrows = 10
             ncolumns = 10
-        r = nrows
-        c = ncolumns
-        deviation = (abs(c-(r+c)/2)/2)
-        nrows = int(min(r, c) + deviation)
-        ncolumns = int(max(r, c) - deviation)
-
+        elif nrows / 2 >= ncolumns or ncolumns / 2 >= nrows:
+            print("WARNING: this maze generator struggles making non-square mazes. One size of your maze is too large compared to other. The maze has been squarred a little bit.")
+            r = nrows
+            c = ncolumns
+            deviation = (abs(c-(r+c)/2)/2)
+            nrows = int(min(r, c) + deviation)
+            ncolumns = int(max(r, c) - deviation)
+
+        if nrows % 2 == 1:
+            nrows -= 1
+            ncolumns -= 1
+        
         startPosition = 1
         pizzaPosition = 1
-
-        rows = (nrows // 2) * 2 + 1
-        columns = (ncolumns // 2) * 2 + 1
+        
+        rows = int((nrows // 2) * 2 + 1)
+        columns = int((ncolumns // 2) * 2 + 1)
 
         if seed is not None:
             np.random.seed(seed)
 
         density = 1 - complexity
-        if nrows <= 10 or ncolumns <= 10:
+        if rows <= 10 or ncolumns <= 10:
             density = min(density + 0.5, 1)
 
         # Adjust complexity and density relative to maze size
         complexity = int((1-complexity) * (5 * (rows + columns)))
         density = int(density * ((rows // 2) * (columns // 2)))
 
         maze = Maze(rows, columns)
         maze.set_borders()
 
         # Make aisles
         for i in range(density):
-            x, y = rand(0, rows // 2) * 2, rand(0, columns // 2) * 2
+            x, y = randint(0, rows // 2) * 2, randint(0, columns // 2) * 2
             maze.set_wall(x, y)
 
             for j in range(complexity):
                 neighbours = []
 
                 if maze.in_maze(x - 2, y):
                     neighbours.append((x - 2, y))
@@ -167,15 +170,15 @@
                 if maze.in_maze(x, y - 2):
                     neighbours.append((x, y - 2))
 
                 if maze.in_maze(x, y + 2):
                     neighbours.append((x, y + 2))
 
                 if len(neighbours):
-                    next_x, next_y = neighbours[rand(0, len(neighbours) - 1)]
+                    next_x, next_y = neighbours[randint(0, len(neighbours) - 1)]
 
                     if not maze.is_wall(next_x, next_y):
                         maze.set_wall(next_x, next_y)
                         maze.set_wall(next_x + (x - next_x) // 2, next_y + (y - next_y) // 2)
                         x, y = next_x, next_y
 
         x, y = randint(0, rows), randint(0, columns)
```

### Comparing `donatellopyzza-1.6.3/donatellopyzza/data/environments/assessment_maze.png` & `donatellopyzza-1.6.4/donatellopyzza/data/environments/assessment_maze.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/data/environments/test.png` & `donatellopyzza-1.6.4/donatellopyzza/data/environments/test.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/data/images/pizza.png` & `donatellopyzza-1.6.4/donatellopyzza/data/images/pizza.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/data/images/turtle.png` & `donatellopyzza-1.6.4/donatellopyzza/data/images/turtle.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/data/images/turtle_small.png` & `donatellopyzza-1.6.4/donatellopyzza/data/images/turtle_small.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/grid/agent.py` & `donatellopyzza-1.6.4/donatellopyzza/grid/agent.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/grid/grid.py` & `donatellopyzza-1.6.4/donatellopyzza/grid/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 
         result = None
         if self._name == "env1":
             result = self.result_for_env1(square, squareTmp, square_touched, agent)
         else:
             result = self.result_generic_env(square, squareTmp, square_touched, agent, action)
 
-        if not self.foundPizza:
-            self.nbActions += 1
+        #if not self.foundPizza:
+        self.nbActions += 1
 
         return result
     
     def pizzaIsFound(self):
         return self.foundPizza
 
     def disableDisplay(self):
```

### Comparing `donatellopyzza-1.6.3/donatellopyzza/grid/gui.py` & `donatellopyzza-1.6.4/donatellopyzza/grid/gui.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/grid/map.py` & `donatellopyzza-1.6.4/donatellopyzza/grid/map.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/grid/parser.py` & `donatellopyzza-1.6.4/donatellopyzza/grid/mazeParser.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/donatellopyzza/grid/square.py` & `donatellopyzza-1.6.4/donatellopyzza/grid/square.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.3/README.md` & `donatellopyzza-1.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## DonatelloPyzza
 
-DonatelloPyzza is a simple and educational game to help beginners learn Python in high school and university.
+DonatelloPyzza is a simple and educational game to help beginners learn algorithmic in Python in high school and university.
 
 A turtle can move through a grid and touch each cells until it finds the pizza.
 This game can be used at several levels:
-- for young beginners: they can hard-code a path to help the turtle find its pizza and small mazes.
+- for young beginners: they can hard-code a path to help the turtle find its pizza in small mazes.
 - for beginners: they can develop intuitive heuristics to find the pizza
 - for intermediate or advanced developers: they can develop a complex path finding method or AI-based solutions.
 
 
 ![View of the game (please go to the homepage of the project to watch this gif)](https://github.com/MilowB/DonatelloPyzza/blob/master/views/example.gif)
 
 
@@ -44,15 +44,15 @@
 turtle = game.start()
 ```
 
 Once the game has started, you get a turtle instance which you can move around the board.
 To do this, the following instruction can be used:
 
 ```python
-feedback = turtle.execute(Action.FORWARD)
+feedback = turtle.execute(Action.MOVE_FORWARD)
 print(feedback)
 ```
 
 You can use the feedback from the `execute()` method to see what happened after your action.
 
 ## Learning the rules:  actions and feedbacks
 
@@ -108,10 +108,10 @@
 
 - make several tests for this package
 - make tutorials to help beginners use this package
 - make a more formal documentation
 - promote this game through a website
 - ~~adapt the GUI to resize it depending on the number of cells~~
 - ~~add a test infrastructure to validate users' algorithm on several mazes~~
-- ~~make possible to the user to select the difficulty its maze when generating it~~
+- ~~make possible to the user to select the difficulty of the maze when generating it~~
 - ~~debug the GUI~~
-- ~~add a gridworld generator~~
+- ~~add a gridworld generator~~
```

### Comparing `donatellopyzza-1.6.3/pyproject.toml` & `donatellopyzza-1.6.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DonatelloPyzza"
-version = "1.6.3"
+version = "1.6.4"
 authors = [
   { name="Mickaël Bettinelli", email="mickael.bettinelli@univ-smb.fr" },
 ]
-description = "A simple grid environment to learn Python"
+description = "A simple and educational game to learn algorithmic where you can develop the behavior of a turtle to move in a maze."
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: Free for non-commercial use",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/MilowB/Donatello"
 "Bug Tracker" = "https://github.com/MilowB/Donatello/pulls"
```

### Comparing `donatellopyzza-1.6.3/PKG-INFO` & `donatellopyzza-1.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: DonatelloPyzza
-Version: 1.6.3
-Summary: A simple grid environment to learn Python
+Version: 1.6.4
+Summary: A simple and educational game to learn algorithmic where you can develop the behavior of a turtle to move in a maze.
 Project-URL: Homepage, https://github.com/MilowB/Donatello
 Project-URL: Bug Tracker, https://github.com/MilowB/Donatello/pulls
 Author-email: Mickaël Bettinelli <mickael.bettinelli@univ-smb.fr>
 License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 
 ## DonatelloPyzza
 
-DonatelloPyzza is a simple and educational game to help beginners learn Python in high school and university.
+DonatelloPyzza is a simple and educational game to help beginners learn algorithmic in Python in high school and university.
 
 A turtle can move through a grid and touch each cells until it finds the pizza.
 This game can be used at several levels:
-- for young beginners: they can hard-code a path to help the turtle find its pizza and small mazes.
+- for young beginners: they can hard-code a path to help the turtle find its pizza in small mazes.
 - for beginners: they can develop intuitive heuristics to find the pizza
 - for intermediate or advanced developers: they can develop a complex path finding method or AI-based solutions.
 
 
 ![View of the game (please go to the homepage of the project to watch this gif)](https://github.com/MilowB/DonatelloPyzza/blob/master/views/example.gif)
 
 
@@ -58,15 +58,15 @@
 turtle = game.start()
 ```
 
 Once the game has started, you get a turtle instance which you can move around the board.
 To do this, the following instruction can be used:
 
 ```python
-feedback = turtle.execute(Action.FORWARD)
+feedback = turtle.execute(Action.MOVE_FORWARD)
 print(feedback)
 ```
 
 You can use the feedback from the `execute()` method to see what happened after your action.
 
 ## Learning the rules:  actions and feedbacks
 
@@ -122,10 +122,10 @@
 
 - make several tests for this package
 - make tutorials to help beginners use this package
 - make a more formal documentation
 - promote this game through a website
 - ~~adapt the GUI to resize it depending on the number of cells~~
 - ~~add a test infrastructure to validate users' algorithm on several mazes~~
-- ~~make possible to the user to select the difficulty its maze when generating it~~
+- ~~make possible to the user to select the difficulty of the maze when generating it~~
 - ~~debug the GUI~~
-- ~~add a gridworld generator~~
+- ~~add a gridworld generator~~
```

