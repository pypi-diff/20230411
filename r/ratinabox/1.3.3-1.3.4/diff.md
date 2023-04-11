# Comparing `tmp/ratinabox-1.3.3.tar.gz` & `tmp/ratinabox-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.3.3.tar", last modified: Wed Mar 22 23:24:04 2023, max compression
+gzip compressed data, was "ratinabox-1.3.4.tar", last modified: Tue Apr 11 09:22:25 2023, max compression
```

## Comparing `ratinabox-1.3.3.tar` & `ratinabox-1.3.4.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-03-22 23:24:04.090312 ratinabox-1.3.3/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.3.3/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25262 2023-03-22 23:24:04.090435 ratinabox-1.3.3/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    24546 2023-03-22 13:51:11.000000 ratinabox-1.3.3/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.3.3/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-03-22 23:24:04.084466 ratinabox-1.3.3/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    38727 2023-03-22 15:29:07.000000 ratinabox-1.3.3/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    31696 2023-03-22 11:40:11.000000 ratinabox-1.3.3/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    76072 2023-03-22 12:41:55.000000 ratinabox-1.3.3/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.3.3/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2680 2023-03-22 23:23:54.000000 ratinabox-1.3.3/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-03-22 23:24:04.086344 ratinabox-1.3.3/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-03-22 11:40:11.000000 ratinabox-1.3.3/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.3.3/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.3.3/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.3.3/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.3.3/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    14973 2023-03-07 14:34:45.000000 ratinabox-1.3.3/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     6687 2023-03-21 18:01:51.000000 ratinabox-1.3.3/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.3.3/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-03-22 23:24:04.087181 ratinabox-1.3.3/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.3.3/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.3.3/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.3.3/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.3.3/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    26856 2023-03-22 15:14:55.000000 ratinabox-1.3.3/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-03-22 23:24:04.085199 ratinabox-1.3.3/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25262 2023-03-22 23:24:04.000000 ratinabox-1.3.3/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      844 2023-03-22 23:24:04.000000 ratinabox-1.3.3/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-03-22 23:24:04.000000 ratinabox-1.3.3/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      132 2023-03-22 23:24:04.000000 ratinabox-1.3.3/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-03-22 23:24:04.000000 ratinabox-1.3.3/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1033 2023-03-22 23:24:04.090750 ratinabox-1.3.3/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.3.3/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-03-22 23:24:04.090215 ratinabox-1.3.3/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-01-09 16:43:43.000000 ratinabox-1.3.3/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.3.3/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.3.3/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.3.3/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.715743 ratinabox-1.3.4/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.3.4/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:22:25.715871 ratinabox-1.3.4/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    24591 2023-04-11 09:20:54.000000 ratinabox-1.3.4/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.3.4/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.709092 ratinabox-1.3.4/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    41094 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    79913 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.3.4/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.711114 ratinabox-1.3.4/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.3.4/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.3.4/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.3.4/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.3.4/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.3.4/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    14973 2023-03-07 14:34:45.000000 ratinabox-1.3.4/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.3.4/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.3.4/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.712255 ratinabox-1.3.4/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.3.4/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.3.4/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.3.4/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.3.4/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    29721 2023-04-06 16:54:27.000000 ratinabox-1.3.4/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.709924 ratinabox-1.3.4/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      103 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-11 09:22:25.000000 ratinabox-1.3.4/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      996 2023-04-11 09:22:25.716185 ratinabox-1.3.4/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.3.4/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:22:25.715631 ratinabox-1.3.4/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-01-09 16:43:43.000000 ratinabox-1.3.4/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.3.4/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.3.4/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.3.4/tests/test_neurons.py
```

### Comparing `ratinabox-1.3.3/LICENSE` & `ratinabox-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/PKG-INFO` & `ratinabox-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.3.3
+Version: 1.3.4
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
@@ -15,15 +15,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: demos
 Provides-Extra: test
 License-File: LICENSE
 
 # RatInABox 
-![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox)
+![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
 
 [**Install**](#installing-and-importing) | [**Demos**](#get-started) | [**Features**](#feature-run-down) | [**Contributions and Questions**](#contribute) | [**Cite**](#cite)
 
 <img src=".images/readme/ratinabox.gif" width=850>
 
@@ -84,15 +84,15 @@
 import ratinabox
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import PlaceCells, GridCells #...
 ```
 
 ## Feature run-down
-Here is a list of features loosely organised into three categories: those pertaining to 
+Here is a list of features loosely organised into those pertaining to 
 
 (i) the [`Environment`](#i-environment-features)
 * [Adding walls](#walls)
 * [Polygon-shaped Environments](#polygon-shaped-environments)
 * [Holes](#holes)
 * [Boundary conditions](#boundary-conditions)
 * [1- or 2-dimensions](#1--or-2-dimensions) 
@@ -310,61 +310,53 @@
 #### Geometry of `PlaceCells` 
 Choose how you want `PlaceCells` to interact with walls in the `Environment`. We provide three types of geometries.  
 
 <img src=".images/readme/wall_geometry.png" width=900>
 
 
 #### Egocentric encodings
-Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric however `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. 
+Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric. `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. With an adequately defined field of view these can make, for example, "whisker cells". 
 
 ```python
 FoV_BVCs = FieldOfViewNeurons(Ag)
 FoV_OVCs = FieldOfViewNeurons(Ag,params={
     'cell_type':'OVC',
-    #other params defining the field of view area (see source code),
     })
+FoV_whiskers = FieldOfViewNeurons(Ag,params={
+    "FoV_angles":[75,105],
+    "FoV_distance":[0.1,0.2],
+    "spatial_resolution":0.02,})
 ```
 
 <img src=".images/readme/field_of_view.gif" width=600>
 
 
 
 #### More complex Neuron types and networks of Neurons
 We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here](./demos/path_integration_example.ipynb) and [here](./demos/reinforcement_learning_example.ipynb). 
 
 
 
 ### (iv) Figures and animations 
+`RatInABox` is built to be highly visual. It is easy to plot or animate data and save these plots/animations. Here are some tips
 
-#### Styling and saving
-`RatInABox` is built to be highly visual. It is easy to plot or animate data. Two functions have been written to help with this: 
+#### Saving
+* `ratinabox.figure_directory` a global variable specifying the directory into which figures/animations will be saved 
+* `ratinabox.utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within the figure directory  as both `".svg"` and `".png"` (`".mp4"` or `".gif"`). The current time will be appended to the `fig_name` so you won't ever overwrite. 
 
-* `ratinabox.stylize_plots()` sets some global rcParams to make plots look pretty 
-* `ratinabox.figure_directory` a global variable specifying the directory figures/animations will be saved into 
-* `utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within `ratinabox.figure_directory` as both `".svg"` and `".png"` (`".mp4"` or `".gif"`) for easy access later.
 
-```python
-import ratinabox
-from ratinabox import utils
-
-# (optional) stylize plots() sets some global rcParams to make plots look nice
-ratinabox.stylize_plots() 
+#### Saving (but automatically)
+* Setting `ratinabox.autosave_plots = True` means RatInABox figure will be automatically saved in the figure directory without having to indvidually call the `utils` function above. 
 
-# set the figure directory where figs and animations will be saved
-ratinabox.figure_directory = "./figures/"
+#### Styling
+* `ratinabox.stylize_plots()` this call sets some global matplotlib rcParams to make plots look pretty/exactly like they do in this repo
 
-#make a figure (many ays to do this)
-fig, ax = Ag.plot_trajectory() #for example
-
-# save it, will be saved in a date-specific folder with current time so you can find it later
-utils.save_figure(fig,"figure_name") #works for animations too
-```
 
 #### Most important plotting functions
-There most important plotting functions are (see source code for the available arguments/kwargs):
+The most important plotting functions are (see source code for the available arguments/kwargs):
 
 ```python
 Environment.plot_environment() #visualises current environment with walls and objects
 Agent.plot_trajectory() #plots trajectory
 Agent.animate_trajectory() #animate trajectory
 Neurons.plot_rate_map() # plots the rate map of the neurons at all positions
 Neurons.plot_rate_timeseries() # plots activities of the neurons over time
```

### Comparing `ratinabox-1.3.3/README.md` & `ratinabox-1.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # RatInABox 
-![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox)
+![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
 
 [**Install**](#installing-and-importing) | [**Demos**](#get-started) | [**Features**](#feature-run-down) | [**Contributions and Questions**](#contribute) | [**Cite**](#cite)
 
 <img src=".images/readme/ratinabox.gif" width=850>
 
@@ -64,15 +64,15 @@
 import ratinabox
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import PlaceCells, GridCells #...
 ```
 
 ## Feature run-down
-Here is a list of features loosely organised into three categories: those pertaining to 
+Here is a list of features loosely organised into those pertaining to 
 
 (i) the [`Environment`](#i-environment-features)
 * [Adding walls](#walls)
 * [Polygon-shaped Environments](#polygon-shaped-environments)
 * [Holes](#holes)
 * [Boundary conditions](#boundary-conditions)
 * [1- or 2-dimensions](#1--or-2-dimensions) 
@@ -290,61 +290,53 @@
 #### Geometry of `PlaceCells` 
 Choose how you want `PlaceCells` to interact with walls in the `Environment`. We provide three types of geometries.  
 
 <img src=".images/readme/wall_geometry.png" width=900>
 
 
 #### Egocentric encodings
-Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric however `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. 
+Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric. `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. With an adequately defined field of view these can make, for example, "whisker cells". 
 
 ```python
 FoV_BVCs = FieldOfViewNeurons(Ag)
 FoV_OVCs = FieldOfViewNeurons(Ag,params={
     'cell_type':'OVC',
-    #other params defining the field of view area (see source code),
     })
+FoV_whiskers = FieldOfViewNeurons(Ag,params={
+    "FoV_angles":[75,105],
+    "FoV_distance":[0.1,0.2],
+    "spatial_resolution":0.02,})
 ```
 
 <img src=".images/readme/field_of_view.gif" width=600>
 
 
 
 #### More complex Neuron types and networks of Neurons
 We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here](./demos/path_integration_example.ipynb) and [here](./demos/reinforcement_learning_example.ipynb). 
 
 
 
 ### (iv) Figures and animations 
+`RatInABox` is built to be highly visual. It is easy to plot or animate data and save these plots/animations. Here are some tips
 
-#### Styling and saving
-`RatInABox` is built to be highly visual. It is easy to plot or animate data. Two functions have been written to help with this: 
+#### Saving
+* `ratinabox.figure_directory` a global variable specifying the directory into which figures/animations will be saved 
+* `ratinabox.utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within the figure directory  as both `".svg"` and `".png"` (`".mp4"` or `".gif"`). The current time will be appended to the `fig_name` so you won't ever overwrite. 
 
-* `ratinabox.stylize_plots()` sets some global rcParams to make plots look pretty 
-* `ratinabox.figure_directory` a global variable specifying the directory figures/animations will be saved into 
-* `utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within `ratinabox.figure_directory` as both `".svg"` and `".png"` (`".mp4"` or `".gif"`) for easy access later.
 
-```python
-import ratinabox
-from ratinabox import utils
-
-# (optional) stylize plots() sets some global rcParams to make plots look nice
-ratinabox.stylize_plots() 
+#### Saving (but automatically)
+* Setting `ratinabox.autosave_plots = True` means RatInABox figure will be automatically saved in the figure directory without having to indvidually call the `utils` function above. 
 
-# set the figure directory where figs and animations will be saved
-ratinabox.figure_directory = "./figures/"
+#### Styling
+* `ratinabox.stylize_plots()` this call sets some global matplotlib rcParams to make plots look pretty/exactly like they do in this repo
 
-#make a figure (many ays to do this)
-fig, ax = Ag.plot_trajectory() #for example
-
-# save it, will be saved in a date-specific folder with current time so you can find it later
-utils.save_figure(fig,"figure_name") #works for animations too
-```
 
 #### Most important plotting functions
-There most important plotting functions are (see source code for the available arguments/kwargs):
+The most important plotting functions are (see source code for the available arguments/kwargs):
 
 ```python
 Environment.plot_environment() #visualises current environment with walls and objects
 Agent.plot_trajectory() #plots trajectory
 Agent.animate_trajectory() #animate trajectory
 Neurons.plot_rate_map() # plots the rate map of the neurons at all positions
 Neurons.plot_rate_timeseries() # plots activities of the neurons over time
```

### Comparing `ratinabox-1.3.3/ratinabox/Agent.py` & `ratinabox-1.3.4/ratinabox/Agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ratinabox
 
 import numpy as np
+import os
 import matplotlib
 from matplotlib import pyplot as plt
 
 
 from ratinabox import utils
 
 """AGENT"""
@@ -140,14 +141,17 @@
         6) Store new position and time in history data frame
         """
         if dt == None:
             dt = self.dt
         self.dt = dt
         self.t += dt
         self.velocity = self.velocity.astype(float)
+        self.pos = np.array(
+            self.pos
+        )  # check pos is an array (may have external been set as a list)
 
         if self.use_imported_trajectory == False:  # use random motion model
             if self.Environment.dimensionality == "2D":
                 # UPDATE VELOCITY there are a number of contributing factors
                 # 1 Stochastically update the direction
                 self.rotational_velocity += utils.ornstein_uhlenbeck(
                     dt=dt,
@@ -421,15 +425,15 @@
             self.history["rot_vel"].append(self.rotational_velocity)
         return
 
     def reset_history(self):
         for key in self.history.keys():
             self.history[key] = []
         return
-    
+
     def import_trajectory(
         self, times=None, positions=None, dataset=None, interpolate=True
     ):
         """Import trajectory data into the agent by passing a list or array of timestamps and a list or array of positions.
         These will used for moting rather than the random motion model. The data is interpolated using cubic splines.
         This means imported data can be low resolution and smoothly upsampled (aka "augmented" with artificial data). Interpolation can be turned off, in which case each time Ag.update() is called the Agent just moves one count along the imported trajectory (no matter how coarse this is), this may be a lot quicker in cases when your imported behaviour data is high resolution.
 
@@ -550,19 +554,20 @@
         framerate=10,
         fig=None,
         ax=None,
         point_size=15,
         decay_point_size=False,
         decay_point_timescale=10,
         plot_agent=True,
-        color='#7b699a',
+        color="#7b699a",
         alpha=0.7,
         xlim=None,
         background_color=None,
         axis_labels=True,
+        autosave=None,
         **kwargs,
     ):
 
         """Plots the trajectory between t_start (seconds) and t_end (defaulting to the last time available)
         Args:
             • t_start: start time in seconds
             • t_end: end time in seconds (default = self.history["t"][-1])
@@ -574,14 +579,15 @@
             • decay_point_timescale: if decay_point_size is True, this is the timescale over which sizes decay
             • plot_agent: dedicated point show agent current position
             • color: plot point color, if color == 'changing' will smoothly change trajectory color from start to finish
             • alpha: plot point opaqness
             • xlim: In 1D, forces the xlim to be a certain time (minutes) (useful if animating this function)
             • background_color: color of the background if not matplotlib default, only for 1D (probably white)
             • axis_labels: whether to show axes labels
+            • autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
 
         Returns:
             fig, ax
         """
 
         dt = self.dt
         t, pos = np.array(self.history["t"]), np.array(self.history["pos"])
@@ -593,44 +599,55 @@
             skiprate = max(1, int((1 / framerate) / dt))
             trajectory = pos[startid:endid, :][::skiprate]
         if self.Environment.dimensionality == "1D":
             skiprate = max(1, int((1 / framerate) / dt))
             trajectory = pos[startid:endid][::skiprate]
         time = t[startid:endid][::skiprate]
         if color is None:
-            color = ["C0"]*len(time)
-        elif color == 'changing':
-            trajectory_cmap = matplotlib.cm.get_cmap('viridis_r')
-            color = [trajectory_cmap(t/len(time)) for t in range(len(time))]
-            decay_point_size = False #if changing colour, may as well show WHOLE trajectory 
+            color = ["C0"] * len(time)
+        elif color == "changing":
+            trajectory_cmap = matplotlib.colormaps["viridis_r"]
+            color = [trajectory_cmap(t / len(time)) for t in range(len(time))]
+            decay_point_size = (
+                False  # if changing colour, may as well show WHOLE trajectory
+            )
         else:
-            color = [color]*len(time)
-
-
+            color = [color] * len(time)
 
         if self.Environment.dimensionality == "2D":
-            fig, ax = self.Environment.plot_environment(fig=fig, ax=ax)
+            fig, ax = self.Environment.plot_environment(fig=fig, ax=ax, autosave=False)
             s = point_size * np.ones_like(time)
             if decay_point_size == True:
                 s = point_size * np.exp((time - time[-1]) / decay_point_timescale)
                 s[(time[-1] - time) > (1.5 * decay_point_timescale)] *= 0
-            
+
             if plot_agent == True:
                 s[-1] = 40
                 color[-1] = "r"
 
             ax.scatter(
                 trajectory[:, 0],
                 trajectory[:, 1],
                 s=s,
                 alpha=alpha,
                 zorder=0,
                 c=color,
                 linewidth=0,
             )
+            # #plot the rat? TODO haha
+            # ratpath = os.path.join(
+            #     os.path.abspath(os.path.join(ratinabox.__file__, os.pardir)),
+            #         "data/rat.png",
+            #     )
+            # rat = plt.imread(ratpath)
+            # rect = 0.5, 0.4, 0.4, 0.4 # What should these values be?
+            # newax = fig.add_axes(rect, anchor='NE', zorder=1)
+            # newax.axis('off')
+            # newax.imshow(rat)
+
         if self.Environment.dimensionality == "1D":
             if fig is None and ax is None:
                 fig, ax = plt.subplots(figsize=(3, 1.5))
             ax.scatter(time / 60, trajectory, alpha=alpha, linewidth=0, c=color, s=5)
             ax.spines["left"].set_position(("data", t_start / 60))
             if axis_labels == True:
                 ax.set_xlabel("Time / min")
@@ -644,97 +661,113 @@
             ax.spines["top"].set_color(None)
             ax.set_xticks([t_start / 60, t_end / 60])
             ex = self.Environment.extent
             ax.set_yticks([ex[1]])
             if background_color is not None:
                 ax.set_facecolor(background_color)
                 fig.patch.set_facecolor(background_color)
+
+        ratinabox.utils.save_figure(fig, "trajectory", save=autosave)
+
         return fig, ax
 
     def animate_trajectory(
-        self, t_start=None, t_end=None, fps=15, speed_up=1, **kwargs
+        self, t_start=None, t_end=None, fps=15, speed_up=1, autosave=None, **kwargs
     ):
         """Returns an animation (anim) of the trajectory, 25fps.
         Should be saved using command like
             >>> anim.save("./where_to_save/animations.gif",dpi=300)
         To display in jupyter notebook, call it:
             >>> anim
 
         Args:
             t_start: Agent time at which to start animation
             t_end (_type_, optional): _description_. Defaults to None.
             fps: frames per second of end video
             speed_up: #times real speed animation should come out at
+            autosave (bool): whether to automatical try and save this. Defaults to None in which case looks for global constant ratinabox.autosave_plots
             kwargs: passed to trajectory plotting function (chuck anything you wish in here). A particularly useful kwarg is 'additional_plot_func': any function which takes a fig, ax and t as input. The animation wll be passed through this each time after plotting the trajectory, use it to modify your animations however you like
 
         Returns:
             animation
         """
         plt.rcParams["animation.html"] = "jshtml"  # for animation rendering in juypter
 
         dt = 1 / fps
         if t_start == None:
             t_start = self.history["t"][0]
         if t_end == None:
             t_end = self.history["t"][-1]
 
-        def animate_(
-            i, fig, ax, t_start, t_max, speed_up, dt, kwargs
-        ):
+        def animate_(i, fig, ax, t_start, t_max, speed_up, dt, kwargs):
             t_end = t_start + (i + 1) * speed_up * dt
             ax.clear()
             if self.Environment.dimensionality == "2D":
-                fig, ax = self.Environment.plot_environment(fig=fig, ax=ax)
+                fig, ax = self.Environment.plot_environment(
+                    fig=fig, ax=ax, autosave=False
+                )
             fig, ax = self.plot_trajectory(
                 t_start=t_start,
                 t_end=t_end,
                 fig=fig,
                 ax=ax,
                 decay_point_size=True,
                 xlim=t_max / 60,
+                autosave=False,
                 **kwargs,
             )
-            if 'additional_plot_func' in kwargs.keys():
-                fig, ax = kwargs['additional_plot_func'](
+            if "additional_plot_func" in kwargs.keys():
+                fig, ax = kwargs["additional_plot_func"](
                     fig=fig, ax=ax, t=t_end, **kwargs  # the current time
                 )
 
             plt.close()
             return
 
         fig, ax = self.plot_trajectory(
-            t_start=0, t_end=10 * self.dt, xlim=t_end / 60, **kwargs
+            t_start=0, t_end=10 * self.dt, xlim=t_end / 60, autosave=False, **kwargs
         )
 
         from matplotlib import animation
 
         anim = matplotlib.animation.FuncAnimation(
             fig,
             animate_,
             interval=1000 * dt,
             frames=int((t_end - t_start) / (dt * speed_up)),
             blit=False,
             fargs=(fig, ax, t_start, t_end, speed_up, dt, kwargs),
         )
+
+        ratinabox.utils.save_animation(anim, "trajectory", save=autosave)
+
         return anim
 
-    def plot_position_heatmap(self, dx=None, weights=None, fig=None, ax=None):
+    def plot_position_heatmap(
+        self,
+        dx=None,
+        fig=None,
+        ax=None,
+        autosave=None,
+    ):
         """Plots a heatmap of postions the agent has been in.
         vmin is always set to zero, so the darkest colormap color (if seen) represents locations which have never been visited
         Args:
             dx (float, optional): The heatmap bin size. Defaults to 5cm in 2D or 1cm in 1D.
             fig, ax: if provided, will plot onto this
+            autosave (bool, optional): If True, will try to save the figure into `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
+
         """
         if self.Environment.dimensionality == "1D":
             if dx is None:
                 dx = 0.01
             pos = np.array(self.history["pos"])
             ex = self.Environment.extent
             if fig is None and ax is None:
-                fig, ax = self.Environment.plot_environment(height=1)
+                fig, ax = self.Environment.plot_environment(autosave=False)
             heatmap, centres = utils.bin_data_for_histogramming(
                 data=pos, extent=ex, dx=dx
             )
             # maybe do smoothing?
             ax.plot(centres, heatmap)
             ax.fill_between(centres, 0, heatmap, alpha=0.3)
             ax.set_ylim(top=np.max(heatmap) * 1.2)
@@ -756,23 +789,32 @@
                 heatmap,
                 extent=ex,
                 interpolation="bicubic",
                 vmin=vmin,
                 vmax=vmax,
                 zorder=0,
             )
+        ratinabox.utils.save_figure(fig, "position_heatmap", save=autosave)
+
         return fig, ax
 
     def plot_histogram_of_speeds(
-        self, fig=None, ax=None, color="C1", return_data=False
+        self,
+        fig=None,
+        ax=None,
+        color="C1",
+        return_data=False,
+        autosave=None,
     ):
         """Plots a histogram of the observed speeds of the agent.
         args:
             fig, ax: not required. the ax object to be drawn onto.
             color: optional. the color.
+            return_data: if True, will return the histogram data (bins and patches)
+            autosave: if True, will try to save the figure into `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
         Returns:
             fig, ax: the figure
         """
         velocities = np.array(self.history["vel"])
         speeds = np.linalg.norm(velocities, axis=1)
         # exclude speeds above 3sigma
         mu, std = np.mean(speeds), np.std(speeds)
@@ -785,26 +827,35 @@
         ax.set_xlabel(r"Speed  / $ms^{-1}$")
         ax.set_yticks([])
         ax.set_xlim(left=0, right=8 * std)
         ax.spines["left"].set_color(None)
         ax.spines["right"].set_color(None)
         ax.spines["top"].set_color(None)
 
+        ratinabox.utils.save_figure(fig, "speed_histogram", save=autosave)
+
         if return_data == True:
             return fig, ax, n, bins, patches
         else:
             return fig, ax
 
     def plot_histogram_of_rotational_velocities(
-        self, fig=None, ax=None, color="C1", return_data=False
+        self,
+        fig=None,
+        ax=None,
+        color="C1",
+        return_data=False,
+        autosave=None,
     ):
         """Plots a histogram of the observed speeds of the agent.
         args:
             fig, ax: not required. the ax object to be drawn onto.
             color: optional. the color.
+            return_data: if True, will return the histogram data (bins and patches)
+            auto_save: if True, will try to save the figure into `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
         Returns:
             fig, ax: the figure
         """
         rot_vels = np.array(self.history["rot_vel"]) * 180 / np.pi
         # exclude rotational velocities above/below 3sigma
         mu, std = np.mean(rot_vels), np.std(rot_vels)
         rot_vels = rot_vels[rot_vels < mu + 3 * std]
@@ -820,10 +871,13 @@
         )
         ax.set_yticks([])
         ax.set_xlim(-5 * std, 5 * std)
         ax.spines["left"].set_color(None)
         ax.spines["right"].set_color(None)
         ax.spines["top"].set_color(None)
         ax.set_xlabel(r"Rotational velocity / $^{\circ} s^{-1}$")
+
+        ratinabox.utils.save_figure(fig, "rotational_velocity_histogram", save=autosave)
+
         if return_data == True:
             return fig, ax, n, bins, patches
         return fig, ax
```

### Comparing `ratinabox-1.3.3/ratinabox/Environment.py` & `ratinabox-1.3.4/ratinabox/Environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,28 +200,26 @@
         self.objects["objects"] = np.append(self.objects["objects"], object, axis=0)
         self.objects["object_types"] = np.append(
             self.objects["object_types"], type, axis=0
         )
         self.n_object_types = len(np.unique(self.objects["object_types"]))
         return
 
-    def plot_environment(self, fig=None, ax=None, height=1):
+    def plot_environment(self, fig=None, ax=None, autosave=None):
         """Plots the environment on the x axis, dark grey lines show the walls
         Args:
             fig,ax: the fig and ax to plot on (can be None)
-            height: if 1D, how many line plots will be stacked (5.5mm per line)
+            autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
         Returns:
             fig, ax: the environment figures, can be used for further downstream plotting.
         """
 
         if self.dimensionality == "1D":
             extent = self.extent
-            fig, ax = plt.subplots(
-                figsize=(2 * (extent[1] - extent[0]), height * (5.5 / 25))
-            )
+            fig, ax = plt.subplots(figsize=(2 * (extent[1] - extent[0]), (5.5 / 25)))
             ax.set_xlim(left=extent[0], right=extent[1])
             ax.spines["left"].set_color("none")
             ax.spines["right"].set_color("none")
             ax.spines["bottom"].set_position("zero")
             ax.spines["top"].set_color("none")
             ax.set_yticks([])
             ax.set_xticks([extent[0], extent[1]])
@@ -292,15 +290,15 @@
                     linewidth=4.0,
                     solid_capstyle="round",
                     zorder=2,
                 )
 
             # plot objects
             if self.plot_objects == True:
-                object_cmap = matplotlib.cm.get_cmap(self.object_colormap)
+                object_cmap = matplotlib.colormaps[self.object_colormap]
                 for (i, object) in enumerate(self.objects["objects"]):
                     object_color = object_cmap(
                         self.objects["object_types"][i]
                         / (self.n_object_types - 1 + 1e-8)
                     )
                     ax.scatter(
                         object[0],
@@ -313,14 +311,17 @@
                     )
 
             ax.set_aspect("equal")
             ax.grid(False)
             ax.axis("off")
             ax.set_xlim(left=extent[0] - 0.03, right=extent[1] + 0.03)
             ax.set_ylim(bottom=extent[2] - 0.03, top=extent[3] + 0.03)
+        
+        ratinabox.utils.save_figure(fig, "Environment", save=autosave)
+
         return fig, ax
 
     def sample_positions(self, n=10, method="uniform_jitter"):
         """Scatters 'n' locations across the environment which can act as, for example, the centres of gaussian place fields, or as a random starting position.
         If method == "uniform" an evenly spaced grid of locations is returned.  If method == "uniform_jitter" these locations are jittered slightly (i.e. random but span the space). Note; if n doesn't uniformly divide the size (i.e. n is not a square number in a square environment) then the largest number that can be scattered uniformly are found, the remaining are randomly placed.
         Args:
             n (int): number of features
@@ -481,15 +482,15 @@
 
             if wall_geometry == "geodesic":
                 assert (
                     boundary_conditions == "solid"
                 ), "geodesic geometry is not available for periodic boundary conditions"
                 assert (
                     len(walls) <= 5
-                ), """unfortunately geodesic geomtry is only defined in closed rooms with one additional wall
+                ), """unfortunately geodesic geometry is only defined in closed rooms with one additional wall
                 (efficient geometry calculations with more than 1 wall are super hard I have discovered!)"""
                 distances = utils.get_distances_between(vectors=vectors)
                 if len(walls) == 4:
                     pass
                 else:
                     wall = walls[4]
                     via_wall_distances = []
```

### Comparing `ratinabox-1.3.3/ratinabox/Neurons.py` & `ratinabox-1.3.4/ratinabox/Neurons.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 """NEURONS"""
 """Parent Class"""
 
 
 class Neurons:
     """The Neuron class defines a population of Neurons. All Neurons have firing rates which depend on the state of the Agent. As the Agent moves the firing rate of the cells adjust accordingly.
 
-    All Neuron classes must be initalised with the Agent (to whom these cells belong) since the Agent determines the firingrates through its position and velocity. The Agent class will itself contain the Environment. Both the Agent (position/velocity) and the Environment (geometry, walls etc.) determine the firing rates. Optionally (but likely) an input dictionary 'params' specifying other params will be given.
+    All Neuron classes must be initalised with the Agent (to whom these cells belong) since the Agent determines the firingrates through its position and velocity. The Agent class will itself contain the Environment. Both the Agent (position/velocity) and the Environment (geometry, walls, objects etc.) determine the firing rates. Optionally (but likely) an input dictionary 'params' specifying other params will be given.
 
     This is a generic Parent class. We provide several SubClasses of it. These include:
     • PlaceCells()
     • GridCells()
     • BoundaryVectorCells()
+    • ObjectVectorCells()
     • VelocityCells()
     • HeadDirectionCells()
     • SpeedCells()
     • FeedForwardLayer()
+    as well as (in  the contribs)
+    • ValueNeuron()
+    • FieldOfViewNeurons()
 
-    The unique function in each child classes is get_state(). Whenever Neurons.update() is called Neurons.get_state() is then called to calculate and returns the firing rate of the cells at the current moment in time. This is then saved. In order to make your own Neuron subclass you will need to write a class with the following mandatory structure:
+    The unique function in each child classes is get_state(). Whenever Neurons.update() is called Neurons.get_state() is then called to calculate and return the firing rate of the cells at the current moment in time. This is then saved. In order to make your own Neuron subclass you will need to write a class with the following mandatory structure:
 
     ============================================================================================
     MyNeuronClass(Neurons):
         def __init__(self,
                      Agent,
                      params={}): #<-- do not change these
 
@@ -45,15 +49,15 @@
                       **kwargs) #<-- do not change these
 
             firingrate = .....
             ###
                 Insert here code which calculates the firing rate.
                 This may work differently depending on what you set evaluate_at as. For example, evaluate_at == 'agent' should means that the position or velocity (or whatever determines the firing rate) will by evaluated using the agents current state. You might also like to have an option like evaluate_at == "all" (all positions across an environment are tested simultaneously - plot_rate_map() tries to call this, for example) or evaluate_at == "last" (in a feedforward layer just look at the last firing rate saved in the input layers saves time over recalculating them.). **kwargs allows you to pass position or velocity in manually.
 
-                By default, the Neurons.update() calls Neurons.get_state() rwithout passing any arguments. So write the default behaviour of get_state() to be what you want it to do in the main training loop.
+                By default, the Neurons.update() calls Neurons.get_state() rwithout passing any arguments. So write the default behaviour of get_state() to be what you want it to do in the main training loop, .
             ###
 
             return firingrate
 
         def any_other_functions_you_might_want(self):...
     ============================================================================================
 
@@ -139,14 +143,15 @@
         chosen_neurons="all",
         spikes=False,
         imshow=False,
         fig=None,
         ax=None,
         xlim=None,
         background_color=None,
+        autosave=None,
         **kwargs,
     ):
         """Plots a timeseries of the firing rate of the neurons between t_start and t_end
 
         Args:
             • t_start (int, optional): _description_. Defaults to start of data, probably 0.
             • t_end (int, optional): _description_. Defaults to end of data.
@@ -154,14 +159,15 @@
             chosen_neurons (str, optional): Which neurons to plot. string "10" will plot 10 of them, "all" will plot all of them, a list like [1,4,5] will plot cells indexed 1, 4 and 5. Defaults to "10".
             • spikes (bool, optional): If True, scatters exact spike times underneath each curve of firing rate. Defaults to True.
             the below params I just added for help with animations
             • imshow - if True will not dispaly as mountain plot but as an image (plt.imshow)
             • fig, ax: the figure, axis to plot on (can be None)
             xlim: fix xlim of plot irrespective of how much time you're plotting
             • background_color: color of the background if not matplotlib default (probably white)
+            • autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
             • kwargs sent to mountain plot function, you can ignore these
 
         Returns:
             fig, ax
         """
         t = np.array(self.history["t"])
         # times to plot
@@ -178,15 +184,15 @@
         # neurons to plot
         chosen_neurons = self.return_list_of_neurons(chosen_neurons)
         n_neurons_to_plot = len(chosen_neurons)
         if ("shift" not in kwargs.keys()) and ("overlap" not in kwargs.keys()):
             kwargs["shift"] = max(
                 1.5, min(4, 40 / n_neurons_to_plot)
             )  # scaled to make plots look nice and be ~constant size
-            # the height must be constant
+            kwargs["shift"] = 2
             kwargs["overlap"] = 2.2
         spike_data = spike_data[startid:endid, chosen_neurons]
         rate_timeseries = rate_timeseries[:, chosen_neurons]
 
         if imshow == False:
             firingrates = rate_timeseries.T
             fig, ax = utils.mountain_plot(
@@ -235,27 +241,29 @@
             ax.spines["left"].set_visible(False)
             ax.set_xlabel("Time / min")
             ax.set_xticks([0 - 0.5, len(t) + 0.5])
             ax.set_xticklabels([round(t_start / 60, 2), round(t_end / 60, 2)])
             ax.set_yticks([])
             ax.set_ylabel("Neurons")
 
+        ratinabox.utils.save_figure(fig, self.name + "_firingrate", save=autosave)
         return fig, ax
 
     def plot_rate_map(
         self,
         chosen_neurons="all",
         method="groundtruth",
         spikes=False,
         fig=None,
         ax=None,
         shape=None,
         colorbar=True,
         t_start=0,
         t_end=None,
+        autosave=None,
         **kwargs,
     ):
         """Plots rate maps of neuronal firing rates across the environment
         Args:
             •chosen_neurons: Which neurons to plot. string "10" will plot 10 of them, "all" will plot all of them, a list like [1,4,5] will plot cells indexed 1, 4 and 5. Defaults to "10".
 
             • method: "groundtruth" "history" "neither": which method to use. If "analytic" (default) tries to calculate rate map by evaluating firing rate at all positions across the environment (note this isn't always well defined. in which case...). If "history", plots ratemap by a weighting a histogram of positions visited by the firingrate observed at that position. If "neither" (or anything else), then neither.
@@ -263,14 +271,15 @@
             • spikes: True or False. Whether to display the occurence of spikes. If False (default) no spikes are shown. If True both ratemap and spikes are shown.
 
             • fig, ax (the fig and ax to draw on top of, optional)
 
             • shape is the shape of the multipanel figure, must be compatible with chosen neurons
             • colorbar: whether to show a colorbar
             • t_start, t_end: in the case where you are plotting spike, or using historical data to get rate map, this restricts the timerange of data you are using
+            • autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
             • kwargs are sent to get_state and utils.mountain_plot and can be ignore if you don't need to use them
 
         Returns:
             fig, ax
         """
         # GET DATA
         if method == "groundtruth":
@@ -350,39 +359,41 @@
                 if method in ["groundtruth", "history"]:
                     if colorbar == True:
                         from mpl_toolkits.axes_grid1 import make_axes_locatable
 
                         divider = make_axes_locatable(axes[-1])
                         cax = divider.append_axes("right", size="5%", pad=0.05)
             for (i, ax_) in enumerate(axes):
-                _, ax_ = self.Agent.Environment.plot_environment(fig, ax_)
+                _, ax_ = self.Agent.Environment.plot_environment(
+                    fig, ax_, autosave=False
+                )
             if len(chosen_neurons) != axes.size:
                 print(
                     f"You are trying to plot a different number of neurons {len(chosen_neurons)} than the number of axes provided {axes.size}. Some might be missed. Either change this with the chosen_neurons argument or pass in a list of axes to plot on"
                 )
 
             vmin, vmax = 0, 0
             ims = []
             if method in ["groundtruth", "history"]:
                 for (i, ax_) in enumerate(axes):
                     ex = self.Agent.Environment.extent
                     if method == "groundtruth":
                         rate_map = rate_maps[chosen_neurons[i], :].reshape(
                             self.Agent.Environment.discrete_coords.shape[:2]
                         )
-                        im = ax_.imshow(rate_map, extent=ex, zorder=0, cmap='inferno')
+                        im = ax_.imshow(rate_map, extent=ex, zorder=0, cmap="inferno")
                     elif method == "history":
                         rate_timeseries_ = rate_timeseries[chosen_neurons[i], :]
                         rate_map = utils.bin_data_for_histogramming(
                             data=pos, extent=ex, dx=0.05, weights=rate_timeseries_
                         )
                         im = ax_.imshow(
                             rate_map,
                             extent=ex,
-                            cmap='inferno',
+                            cmap="inferno",
                             interpolation="bicubic",
                             zorder=1,
                         )
                     ims.append(im)
                     vmin, vmax = (
                         min(vmin, np.min(rate_map)),
                         max(vmax, np.max(rate_map)),
@@ -403,18 +414,16 @@
                         pos_where_spiked[:, 0],
                         pos_where_spiked[:, 1],
                         s=2,
                         linewidth=0,
                         alpha=0.7,
                     )
 
-            return fig, axes
-
         # PLOT 1D
-        if self.Agent.Environment.dimensionality == "1D":
+        elif self.Agent.Environment.dimensionality == "1D":
             if method == "groundtruth":
                 rate_maps = rate_maps[chosen_neurons, :]
                 x = self.Agent.Environment.flattened_discrete_coords[:, 0]
             if method == "history":
                 ex = self.Agent.Environment.extent
                 pos_ = pos[:, 0]
                 rate_maps = []
@@ -427,18 +436,24 @@
                     )
                     x, rate_map = utils.interpolate_and_smooth(x, rate_map, sigma=0.03)
                     rate_maps.append(rate_map)
                 rate_maps = np.array(rate_maps)
 
             if fig is None and ax is None:
                 fig, ax = self.Agent.Environment.plot_environment(
-                    height=0.5 * len(chosen_neurons)
+                    autosave=False,
                 )
 
             if method != "neither":
+                kwargs = {}
+                kwargs["shift"] = max(
+                    1.5, min(4, 40 / len(chosen_neurons))
+                )  # scaled to make plots look nice and be ~constant size
+                kwargs["shift"] = 2
+                kwargs["overlap"] = 2.2
                 fig, ax = utils.mountain_plot(
                     X=x, NbyX=rate_maps, color=self.color, fig=fig, ax=ax, **kwargs
                 )
 
             if spikes is True:
                 for i in range(len(chosen_neurons)):
                     pos_ = pos[:, 0]
@@ -451,15 +466,18 @@
                         alpha=0.5,
                         s=2,
                         linewidth=0,
                     )
             ax.set_xlabel("Position / m")
             ax.set_ylabel("Neurons")
 
-        return fig, ax
+            axes = ax
+        ratinabox.utils.save_figure(fig, self.name + "_ratemaps", save=autosave)
+
+        return fig, axes
 
     def save_to_history(self):
         cell_spikes = np.random.uniform(0, 1, size=(self.n,)) < (
             self.Agent.dt * self.firingrate
         )
         self.history["t"].append(self.Agent.t)
         self.history["firingrate"].append(list(self.firingrate))
@@ -473,14 +491,15 @@
     def animate_rate_timeseries(
         self,
         t_start=None,
         t_end=None,
         chosen_neurons="all",
         fps=15,
         speed_up=1,
+        autosave=None,
         **kwargs,
     ):
         """Returns an animation (anim) of the firing rates, 25fps.
         Should be saved using command like:
             >>> anim.save("./where_to_save/animations.gif",dpi=300) #or ".mp4" etc...
         To display within jupyter notebook, just call it:
             >>> anim
@@ -512,37 +531,42 @@
             fig, ax = self.plot_rate_timeseries(
                 t_start=t_start,
                 t_end=t_end,
                 chosen_neurons=chosen_neurons,
                 fig=fig,
                 ax=ax,
                 xlim=t_max,
+                autosave=False,
                 **kwargs,
             )
             plt.close()
             return
 
         fig, ax = self.plot_rate_timeseries(
             t_start=0,
             t_end=10 * self.Agent.dt,
             chosen_neurons=chosen_neurons,
             xlim=t_end,
+            autosave=False,
             **kwargs,
         )
 
         from matplotlib import animation
 
         anim = matplotlib.animation.FuncAnimation(
             fig,
             animate_,
             interval=1000 * dt,
             frames=int((t_end - t_start) / (dt * speed_up)),
             blit=False,
             fargs=(fig, ax, chosen_neurons, t_start, t_end, dt, speed_up),
         )
+
+        ratinabox.utils.save_animation(anim, "rat_timeseries", save=autosave)
+
         return anim
 
     def return_list_of_neurons(self, chosen_neurons="all"):
         """Returns a list of indices corresponding to neurons.
 
         Args:
             which (_type_, optional): _description_. Defaults to "all".
@@ -659,15 +683,15 @@
                     f"{self.wall_geometry} wall geometry only possible in 2D when the boundary conditions are solid. Using 'euclidean' instead."
                 )
                 self.wall_geometry = "euclidean"
             if (self.wall_geometry == "geodesic") and (
                 len(self.Agent.Environment.walls) > 5
             ):
                 print(
-                    "'geodesic' wall geometry only supported for enivoronments with 1 additional wall (4 boundaing walls + 1 additional). Sorry. Using 'line_of_sight' instead."
+                    "'geodesic' wall geometry only supported for enivironments with 1 additional wall (4 bounding walls + 1 additional). Sorry. Using 'line_of_sight' instead."
                 )
                 self.wall_geometry = "line_of_sight"
 
         if ratinabox.verbose is True:
             print(
                 "PlaceCells successfully initialised. You can see where they are centred at using PlaceCells.plot_place_cell_locations()"
             )
@@ -716,36 +740,46 @@
             firingrate = 1 * (dist < self.widths)
 
         firingrate = (
             firingrate * (self.max_fr - self.min_fr) + self.min_fr
         )  # scales from being between [0,1] to [min_fr, max_fr]
         return firingrate
 
-    def plot_place_cell_locations(self, fig=None, ax=None):
+    def plot_place_cell_locations(
+        self,
+        fig=None,
+        ax=None,
+        autosave=None,
+    ):
         """Scatter plots where the centre of the place cells are
 
         Args:
             fig, ax: if provided, will plot fig and ax onto these instead of making new.
+            autosave (bool, optional): if True, will try to save the figure into `ratinabox.figure_directory`.Defaults to None in which case looks for global constant ratinabox.autosave_plots
 
         Returns:
             _type_: _description_
         """
         if fig is None and ax is None:
-            fig, ax = self.Agent.Environment.plot_environment()
+            fig, ax = self.Agent.Environment.plot_environment(autosave=False)
         else:
-            _, _ = self.Agent.Environment.plot_environment(fig=fig, ax=ax)
+            _, _ = self.Agent.Environment.plot_environment(
+                fig=fig, ax=ax, autosave=False
+            )
         place_cell_centres = self.place_cell_centres
         ax.scatter(
             place_cell_centres[:, 0],
             place_cell_centres[:, 1],
             c="C1",
             marker="x",
             s=15,
             zorder=2,
         )
+        ratinabox.utils.save_figure(fig, "place_cell_locations", save=autosave)
+
         return fig, ax
 
 
 class GridCells(Neurons):
     """The GridCells class defines a population of GridCells. This class is a subclass of Neurons() and inherits it properties/plotting functions.
 
     Must be initialised with an Agent and a 'params' dictionary.
@@ -1101,19 +1135,27 @@
                 -1,
                 -1,
                 -1,
             ),
         )
         return pref[..., 0]
 
-    def plot_BVC_receptive_field(self, chosen_neurons="all", fig=None, ax=None):
+    def plot_BVC_receptive_field(
+        self,
+        chosen_neurons="all",
+        fig=None,
+        ax=None,
+        autosave=None,
+    ):
         """Plots the receptive field (in polar corrdinates) of the BVC cells. For allocentric BVCs "up" in this plot == "North", for egocentric BVCs, up == the head direction of the animals
 
         Args:
             chosen_neurons: Which neurons to plot. Can be int, list, array or "all". Defaults to "all".
+            fig, ax: the figure/ax object to plot onto (optional)
+            autosave (bool, optional): if True, will try to save the figure into `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
 
         Returns:
             fig, ax
         """
 
         if chosen_neurons == "all":
             chosen_neurons = np.arange(self.n)
@@ -1152,14 +1194,16 @@
             ax[i].grid(False)
             ax[i].pcolormesh(
                 theta, r, receptive_field, edgecolors="face", shading="nearest"
             )
             ax[i].set_xticks([])
             ax[i].set_yticks([])
 
+        ratinabox.utils.save_figure(fig, "BVC_receptive_fields", save=autosave)
+
         return fig, ax
 
 
 class ObjectVectorCells(Neurons):
     """Initialises ObjectVectorCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
 
     ObjectVectorCells respond to Objects inside the Environment (2D only). Add objects to the environment using the `Env.add_object()` method. Each OVC has a prefrerred type (which "type" of object it responds to), tuning angle, and tuning distance (direction and distance from object cell will preferentially fire at).
@@ -1370,15 +1414,15 @@
         """Initialise HeadDirectionCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
         Args:
             params (dict, optional). Defaults to {}."""
         default_params = {
             "min_fr": 0,
             "max_fr": 1,
             "n": 4,
-            "angular_spread_degrees": 30,  # width of HDC preference function (degrees)
+            "angular_spread_degrees": 45,  # width of HDC preference function (degrees)
             "name": "HeadDirectionCells",
         }
         self.Agent = Agent
         for key in params.keys():
             default_params[key] = params[key]
         self.params = default_params
 
@@ -1427,17 +1471,53 @@
         firingrate = (
             firingrate * (self.max_fr - self.min_fr) + self.min_fr
         )  # scales from being between [0,1] to [min_fr, max_fr]
 
         return firingrate
 
     def plot_HDC_receptive_field(
-        self,
+        self, chosen_neurons="all", fig=None, ax=None, autosave=None
     ):
-        return
+        """Plots the receptive fields, in polar coordinates, of hte head direction cells. The receptive field is a von mises function centred around the preferred direction of the cell.
+
+        Args:
+            chosen_neurons (str, optional): The neurons to plot. Defaults to "all".
+            fig, ax (_type_, optional): matplotlib fig, ax objects ot plot onto (optional).
+            autosave (bool, optional): if True, will try to save the figure into `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
+
+        Returns:
+            fig, ax
+        """
+        chosen_neurons = self.return_list_of_neurons(chosen_neurons=chosen_neurons)
+        if fig is None and ax is None:
+            fig, ax = plt.subplots(
+                1,
+                len(chosen_neurons),
+                figsize=(2 * len(chosen_neurons), 2),
+                subplot_kw={"projection": "polar"},
+            )
+
+        for i, n in enumerate(chosen_neurons):
+            theta = np.linspace(0, 2 * np.pi, 100)
+            pref_theta = self.preferred_angles[n]
+            sigma_theta = self.angular_tunings[n]
+            fr = utils.von_mises(theta, pref_theta, sigma_theta, norm=1)
+            fr = fr * (self.max_fr - self.min_fr) + self.min_fr
+            ax[i].plot(theta, fr, linewidth=2, color=self.color, zorder=11)
+            ax[i].set_yticks([])
+            ax[i].set_xticks([])
+            ax[i].set_xticks([0, np.pi / 2, np.pi, 3 * np.pi / 2])
+            ax[i].fill_between(theta, fr, 0, color=self.color, alpha=0.2)
+            ax[i].set_ylim([0, self.max_fr])
+            ax[i].tick_params(pad=-18)
+            ax[i].set_xticklabels(["E", "N", "W", "S"])
+
+        ratinabox.utils.save_figure(fig, self.name + "_ratemaps", save=autosave)
+
+        return fig, ax
 
 
 class VelocityCells(HeadDirectionCells):
     """The VelocityCells class defines a population of Velocity cells. This basically takes the output from a population of HeadDirectionCells and scales it proportional to the speed (dependence on speed and direction --> velocity).
 
     Must be initialised with an Agent and a 'params' dictionary. Initalise tehse cells as if they are HeadDirectionCells
```

### Comparing `ratinabox-1.3.3/ratinabox/README.md` & `ratinabox-1.3.4/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.3.4/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.3.4/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.3.4/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/contribs/README.md` & `ratinabox-1.3.4/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.3.4/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.3.4/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.3.4/ratinabox/contribs/ValueNeuron.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,31 +32,32 @@
     """
 
     def __init__(self, Agent, params={}):
         default_params = {
             "input_layer": None,  # the features it is using as inputs
             "tau": 2,  # discount time horizon (equivalent to gamma in discrete RL)
             "tau_e": None,  # eligibility trace timescale, must be <= tau (defaults to tau/2)
-            "eta": 0.1,  # learning rate
-            "L2": 0.01,  # L2 regularisation
+            "eta": 0.001,  # learning rate
+            "L2": 0.001,  # L2 regularisation
             "activation_params": {"activation": "relu"},  # non-linearity for
             "n": 1,  # how many rewards there will be and thus how many Values function (each represented by one ValueNeuron) there are
         }
 
         default_params.update(params)
         self.params = default_params
 
         self.params["input_layers"] = [self.params["input_layer"]]
         super().__init__(Agent, self.params)  # initialise parent class
 
         if self.tau_e == None:
             self.tau_e = self.tau / 2
-        self.et = np.zeros(params["input_layer"].n)  # initialise eligibility trace
-        self.firingrate = np.zeros(1)  # initialise firing rate
-        self.firingrate_deriv = np.zeros(1)  # initialise firing rate derivative
+        self.et = np.zeros(self.n)  # initialise eligibility trace
+        self.firingrate = np.zeros(self.n)  # initialise firing rate
+        self.firingrate_deriv = np.zeros(self.n)  # initialise firing rate derivative
+        self.td_error = np.zeros(self.n)  # initialise td error
 
     def update(self):
         """Updates firing rate as weighted linear sum of feature inputs"""
         firingrate_last = self.firingrate
         # update the firing rate
         super().update()  # FeedForwardLayer builtin function. this sums the inputs from the input features over the weight matrix and saves the firingrate.
         # calculate temporal derivative of the firing rate
@@ -86,17 +87,30 @@
         )  # this is the continuous analog of the TD error
         dw = (
             self.Agent.dt
             * self.eta
             * (np.outer(self.td_error * self.firingrate_prime, self.et))
             - self.eta * self.Agent.dt * self.L2 * w
         )  # note L2 regularisation
+        if np.linalg.norm(dw) > 10:
+            print(np.linalg.norm(dw))
         self.inputs[self.input_layer.name]["w"] += dw
         return
 
+    def reset(
+        self,
+    ):
+        """Resets the value neuron by wiping the current eligibility trace and firing rate"""
+        self.et = np.zeros(self.n)  # reinitialise eligibility trace
+        self.firingrate = np.zeros(self.n)  # reinitialise firing rate
+        self.firingrate_deriv = np.zeros(self.n)  # reinitialise firing rate derivative
+        self.td_error = np.zeros(self.n)  # reinitialise td error
+
+        return
+
 
 if __name__ == "__main__":
     """Example use.
     A reward is placed in the middle of the environment. Agent explores and learns "value" as linear sum of 100 place cells. Afterwarrd, the results are plotted. (If successful the value function should be higher in the centre of the environment (near reward) and lower at the edges))
     """
     from ratinabox.contribs.ValueNeuron import ValueNeuron
     from tqdm import tqdm
```

### Comparing `ratinabox-1.3.3/ratinabox/data/README.md` & `ratinabox-1.3.4/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/data/sargolini.npz` & `ratinabox-1.3.4/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/data/tanni.npz` & `ratinabox-1.3.4/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/ratinabox/utils.py` & `ratinabox-1.3.4/ratinabox/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     Each element of vector_list_a gives a line segment of the form [[x_a_0,y_a_0],[x_a_1,y_a_1]], or, in vector notation [p_a_0,p_a_1]
     (same goes for vector vector_list_b). Thus
         vector_list_A.shape = (N_a,2,2)
         vector_list_B.shape = (N_b,2,2)
     where N_a is the number of vectors defined in vector_list_a
 
-    Each line segments define an (infinite) line, parameterised by line_a = p_a_0 + l_a.(p_a_1-p_a_0).
+    Each line segments defines an (infinite) line, parameterised by line_a = p_a_0 + l_a.(p_a_1-p_a_0).
     We want to find the intersection between these lines in terms of the parameters l_a and l_b.
     Iff l_a and l_b are BOTH between 0 and 1 then the line segments intersect. Thus the goal is to return an array, I,  of shape
         I.shape = (N_a,N_b,2)
     where, if I[n_a,n_b][0] and I[n_a,n_b][1] are both between 0 and 1 then it means line segments vector_list_a[n_a] and vector_list_b[n_b] intersect.
 
     To do this we consider solving the equation line_a = line_b. The solution to this is:
         l_a = dot((p_b_0 - p_a_0) , (p_b_1 - p_b_0)_p) / dot((p_a_1 - p_a_0) , (p_b_1 - p_b_0)_p)
@@ -490,17 +490,17 @@
     fc = 0.3 * c + (1 - 0.3) * np.array([1, 1, 1])  # convert rgb+alpha to rgb
 
     if norm_by == "max":
         NbyX = overlap * NbyX / np.max(np.abs(NbyX))
     else:
         NbyX = overlap * NbyX / norm_by
     if fig is None and ax is None:
-        fig, ax = plt.subplots(
-            figsize=(4, len(NbyX) * shift / 25)
-        )  # ~<shift>mm gap between lines
+        fig, ax = plt.subplots()
+
+    fig.set_size_inches(4, len(NbyX) * shift / 25)
     zorder = 1
     for i in range(len(NbyX)):
         ax.plot(X, NbyX[i] + i + 1, c=c, zorder=zorder)
         zorder -= 0.01
         ax.fill_between(
             X, NbyX[i] + i + 1, i + 1, color=fc, zorder=zorder, alpha=0.8, linewidth=0
         )
@@ -520,69 +520,126 @@
     ax.set_ylim()
     if xlim is not None:
         ax.set_xlim(right=xlim)
 
     return fig, ax
 
 
-def save_figure(fig,
-                save_title="",
-                fig_save_types=['svg','png'],
-                anim_save_types=['gif','mp4']
+def save_figure(
+    fig,
+    save_title="",
+    fig_save_types=["svg", "png"],
+    anim_save_types=["gif", "mp4"],
+    save=True,
 ):
     """
-    Saves a figures and animations by date (folder) and time (name) as both '.png' and '.svg'
+    Saves a figure in a dated-folder with the current time appended to save_title, as both '.png' and '.svg'. Same for animations but as ".gif" and ".mp4".
+    This function can be used by anyone...just pass a fig object and it will be saved in the right place.
+
     Args:
         fig (matplotlib fig object): the matplotlib figure or animation object to be saved
         save_title (str, optional): name to be saved as. Current time will be appended to this so you won't overwrite old figures, defaults to no name "".
         fig_file_types: what file types to save figure as ['svg','png']
-        fig_file_types: what file types to save figure as ['gif','mp4']
+        anim_file_types: what file types to save figure as ['gif','mp4']
+        save: whether to save or not, i.e. this function can be called but if save is not True, nothing will happen (expect some warnings). Mostly ignore this.
 
     """
-    figure_directory = ratinabox.figure_directory  
-    assert figure_directory is not None, print('A figure directory has not been set. Set one using command `ratinabox.figure_directory = "path/to/my/figs/"')
+    if save is None:  # take ratinabox default
+        save = ratinabox.autosave_plots
+        # print a hint to the first-time user
+        if (
+            (ratinabox._save_plot_warnings_on)
+            and (save == "undefined")
+            and (save != False)
+        ):
+            # None is the default for ratinabox.autosave_plots which is the default for many internal functions that call this function
+            print("WARNING: This figure has not been saved.")
+            print(
+                "    • To AUTOMATICALLY save all plots (recommended), set  `ratinabox.autosave_plots = True`"
+            )
+            print(
+                "    • To MANUALLY save plots, call                        `ratinabox.utils.save_figure(figure_object, save_title)."
+            )
+            print("      This warning will not be shown again")
+            ratinabox._save_plot_warnings_on = False
+
+        if (ratinabox._stylize_plot_warnings_on) and (
+            ratinabox._stylized_plots == False
+        ):
+            print(
+                "HINT: You can stylize plots to make them look like repo/paper by calling `ratinabox.stylize_plots()`"
+            )
+
+            print("      This hint will not be shown again")
+            ratinabox._stylize_plot_warnings_on = False
+
+    if save != True:
+        return
+
+    figure_directory = ratinabox.figure_directory
+    if (figure_directory == "undefined") or (figure_directory is None):
+        print(
+            "This figure cannot be saved because a figure directory has not been set."
+        )
+        print(
+            '    Set a default figure directory `ratinabox.figure_directory = "path/to/my/figs/"`'
+        )
+        print(f"       (the current working directory is {os.getcwd()})")
+        return
+
+    if figure_directory[-1] != "/":
+        figure_directory += "/"
+
     if not os.path.isdir(figure_directory):
         os.mkdir(figure_directory)
 
-    #make today-specific directory inside figure directory  
-    today =  datetime.strftime(datetime.now(),'%y%m%d')
+    # make today-specific directory inside figure directory
+    today = datetime.strftime(datetime.now(), "%d_%m_%y")
     if not os.path.isdir(figure_directory + f"{today}/"):
         os.mkdir(figure_directory + f"{today}/")
-    
+
     figdir = figure_directory + f"{today}/"
-    now = datetime.strftime(datetime.now(),'%H%M')
+    now = datetime.strftime(datetime.now(), "%H%M")
     path_ = f"{figdir}{save_title}_{now}"
     path = path_
 
     if type(fig) == matplotlib.figure.Figure:
         for filetype in fig_save_types:
-            i=1
-            while True: #checks there isn't an existing figure with this name 
-                if os.path.isfile(path+"." + filetype):
-                    path = path_+"_"+str(i)
-                    i+=1
-                elif i >= 100: break
-                else: break
-            fig.savefig(path+"."+filetype,bbox_inches='tight')
-    
+            i = 1
+            while True:  # checks there isn't an existing figure with this name
+                if os.path.isfile(path + "." + filetype):
+                    path = path_ + "_" + str(i)
+                    i += 1
+                elif i >= 100:
+                    break
+                else:
+                    break
+            fig.savefig(path + "." + filetype, bbox_inches="tight")
+
     elif type(fig) == matplotlib.animation.FuncAnimation:
         for filetype in anim_save_types:
-            i=1
+            i = 1
             while True:
-                if os.path.isfile(path+"." + filetype):
-                    path = path_+"_"+str(i)
-                    i+=1
-                elif i >= 100: break
-                else: break
-            fig.save(path+"."+filetype)
-
+                if os.path.isfile(path + "." + filetype):
+                    path = path_ + "_" + str(i)
+                    i += 1
+                elif i >= 100:
+                    break
+                else:
+                    break
+            fig.save(path + "." + filetype)
 
     return path
 
 
+def save_animation(*args, **kwargs):
+    """Saves an animation. This function just passes the animation object to utils.save_figure() where it is then saved. We only include this function for semantic consistency (you could just use save_figure directly. Takes exactly the same args are save_figure() and just passes the animation over there"""
+    return save_figure(*args, **kwargs)
+
+
 """Other"""
 
 
 def update_class_params(Class, params: dict):
     """Updates parameters from a dictionary.
     All parameters found in params will be updated to new value
     Args:
@@ -622,14 +679,15 @@
 
     assert name in [
         "linear",
         "sigmoid",
         "relu",
         "tanh",
         "retanh",
+        "softmax",
     ]
 
     if name == "linear":
         if deriv == False:
             return x
         elif deriv == True:
             return np.ones(x.shape)
@@ -686,7 +744,17 @@
             )
         elif deriv == True:
             return (
                 other_args["gain"]
                 * (1 - np.tanh(x) ** 2)
                 * ((x - other_args["threshold"]) > 0)
             )
+
+    if name == "softmax":
+        other_args_default = {"gain": 1, "threshold": 0}
+        for key in other_args.keys():
+            other_args_default[key] = other_args[key]
+        other_args = other_args_default
+        if deriv == False:
+            return other_args["gain"] * np.log(1 + np.exp(x - other_args["threshold"]))
+        elif deriv == True:
+            return other_args["gain"] / (1 + np.exp(-(x - other_args["threshold"])))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ratinabox-1.3.3/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.3.4/ratinabox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.3.3
+Version: 1.3.4
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
@@ -15,15 +15,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: demos
 Provides-Extra: test
 License-File: LICENSE
 
 # RatInABox 
-![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox)
+![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
 
 [**Install**](#installing-and-importing) | [**Demos**](#get-started) | [**Features**](#feature-run-down) | [**Contributions and Questions**](#contribute) | [**Cite**](#cite)
 
 <img src=".images/readme/ratinabox.gif" width=850>
 
@@ -84,15 +84,15 @@
 import ratinabox
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import PlaceCells, GridCells #...
 ```
 
 ## Feature run-down
-Here is a list of features loosely organised into three categories: those pertaining to 
+Here is a list of features loosely organised into those pertaining to 
 
 (i) the [`Environment`](#i-environment-features)
 * [Adding walls](#walls)
 * [Polygon-shaped Environments](#polygon-shaped-environments)
 * [Holes](#holes)
 * [Boundary conditions](#boundary-conditions)
 * [1- or 2-dimensions](#1--or-2-dimensions) 
@@ -310,61 +310,53 @@
 #### Geometry of `PlaceCells` 
 Choose how you want `PlaceCells` to interact with walls in the `Environment`. We provide three types of geometries.  
 
 <img src=".images/readme/wall_geometry.png" width=900>
 
 
 #### Egocentric encodings
-Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric however `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. 
+Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric. `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. With an adequately defined field of view these can make, for example, "whisker cells". 
 
 ```python
 FoV_BVCs = FieldOfViewNeurons(Ag)
 FoV_OVCs = FieldOfViewNeurons(Ag,params={
     'cell_type':'OVC',
-    #other params defining the field of view area (see source code),
     })
+FoV_whiskers = FieldOfViewNeurons(Ag,params={
+    "FoV_angles":[75,105],
+    "FoV_distance":[0.1,0.2],
+    "spatial_resolution":0.02,})
 ```
 
 <img src=".images/readme/field_of_view.gif" width=600>
 
 
 
 #### More complex Neuron types and networks of Neurons
 We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here](./demos/path_integration_example.ipynb) and [here](./demos/reinforcement_learning_example.ipynb). 
 
 
 
 ### (iv) Figures and animations 
+`RatInABox` is built to be highly visual. It is easy to plot or animate data and save these plots/animations. Here are some tips
 
-#### Styling and saving
-`RatInABox` is built to be highly visual. It is easy to plot or animate data. Two functions have been written to help with this: 
+#### Saving
+* `ratinabox.figure_directory` a global variable specifying the directory into which figures/animations will be saved 
+* `ratinabox.utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within the figure directory  as both `".svg"` and `".png"` (`".mp4"` or `".gif"`). The current time will be appended to the `fig_name` so you won't ever overwrite. 
 
-* `ratinabox.stylize_plots()` sets some global rcParams to make plots look pretty 
-* `ratinabox.figure_directory` a global variable specifying the directory figures/animations will be saved into 
-* `utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within `ratinabox.figure_directory` as both `".svg"` and `".png"` (`".mp4"` or `".gif"`) for easy access later.
 
-```python
-import ratinabox
-from ratinabox import utils
-
-# (optional) stylize plots() sets some global rcParams to make plots look nice
-ratinabox.stylize_plots() 
+#### Saving (but automatically)
+* Setting `ratinabox.autosave_plots = True` means RatInABox figure will be automatically saved in the figure directory without having to indvidually call the `utils` function above. 
 
-# set the figure directory where figs and animations will be saved
-ratinabox.figure_directory = "./figures/"
+#### Styling
+* `ratinabox.stylize_plots()` this call sets some global matplotlib rcParams to make plots look pretty/exactly like they do in this repo
 
-#make a figure (many ays to do this)
-fig, ax = Ag.plot_trajectory() #for example
-
-# save it, will be saved in a date-specific folder with current time so you can find it later
-utils.save_figure(fig,"figure_name") #works for animations too
-```
 
 #### Most important plotting functions
-There most important plotting functions are (see source code for the available arguments/kwargs):
+The most important plotting functions are (see source code for the available arguments/kwargs):
 
 ```python
 Environment.plot_environment() #visualises current environment with walls and objects
 Agent.plot_trajectory() #plots trajectory
 Agent.animate_trajectory() #animate trajectory
 Neurons.plot_rate_map() # plots the rate map of the neurons at all positions
 Neurons.plot_rate_timeseries() # plots activities of the neurons over time
```

### Comparing `ratinabox-1.3.3/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.3.4/ratinabox.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 ratinabox/contribs/README.md
 ratinabox/contribs/STDPFeedForwardLayer.py
 ratinabox/contribs/ThetaSequenceAgent.py
 ratinabox/contribs/ValueNeuron.py
 ratinabox/contribs/__init__.py
 ratinabox/data/README.md
 ratinabox/data/__init__.py
+ratinabox/data/rat.png
 ratinabox/data/sargolini.npz
 ratinabox/data/tanni.npz
 tests/test_advanced.py
 tests/test_agent.py
 tests/test_environment.py
 tests/test_neurons.py
```

### Comparing `ratinabox-1.3.3/setup.cfg` & `ratinabox-1.3.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.3.3
+version = 1.3.4
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
@@ -17,18 +17,18 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 install_requires = 
-	numpy ~= 1.24.2
-	matplotlib ~= 3.7.1
-	scipy ~= 1.9.3
-	shapely ~= 2.0.1
+	numpy
+	matplotlib
+	scipy
+	shapely
 python_requires = >=3.7
 include_package_data = False
 
 [options.extras_require]
 demos = 
 	jupyter ~= 1.0.0
 	tqdm ~= 4.62.3
```

### Comparing `ratinabox-1.3.3/tests/test_advanced.py` & `ratinabox-1.3.4/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.3.3/tests/test_environment.py` & `ratinabox-1.3.4/tests/test_environment.py`

 * *Files identical despite different names*

