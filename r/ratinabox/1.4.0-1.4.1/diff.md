# Comparing `tmp/ratinabox-1.4.0.tar.gz` & `tmp/ratinabox-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.4.0.tar", last modified: Tue Apr 11 09:24:48 2023, max compression
+gzip compressed data, was "ratinabox-1.4.1.tar", last modified: Tue Apr 11 17:41:30 2023, max compression
```

## Comparing `ratinabox-1.4.0.tar` & `ratinabox-1.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.313537 ratinabox-1.4.0/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.4.0/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:24:48.313729 ratinabox-1.4.0/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    24591 2023-04-11 09:20:54.000000 ratinabox-1.4.0/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.4.0/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.306439 ratinabox-1.4.0/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    41094 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    79913 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.4.0/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.308395 ratinabox-1.4.0/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.4.0/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.4.0/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.4.0/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.4.0/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.4.0/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    14973 2023-03-07 14:34:45.000000 ratinabox-1.4.0/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.4.0/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.4.0/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.309725 ratinabox-1.4.0/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.4.0/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.4.0/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.4.0/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.4.0/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    29721 2023-04-06 16:54:27.000000 ratinabox-1.4.0/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.307183 ratinabox-1.4.0/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25307 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      103 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-11 09:24:48.000000 ratinabox-1.4.0/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      996 2023-04-11 09:24:48.314080 ratinabox-1.4.0/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.4.0/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 09:24:48.313392 ratinabox-1.4.0/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-01-09 16:43:43.000000 ratinabox-1.4.0/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.4.0/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.4.0/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.4.0/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.257229 ratinabox-1.4.1/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.4.1/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25185 2023-04-11 17:41:30.257382 ratinabox-1.4.1/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    24491 2023-04-11 13:27:49.000000 ratinabox-1.4.1/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.4.1/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.250123 ratinabox-1.4.1/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    41124 2023-04-11 16:33:06.000000 ratinabox-1.4.1/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.4.1/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    80087 2023-04-11 15:07:26.000000 ratinabox-1.4.1/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.4.1/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.4.1/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.251946 ratinabox-1.4.1/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.4.1/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.4.1/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.4.1/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.4.1/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.4.1/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15009 2023-04-11 17:03:00.000000 ratinabox-1.4.1/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.4.1/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.4.1/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.252972 ratinabox-1.4.1/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.4.1/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.4.1/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.4.1/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.4.1/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.4.1/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    30579 2023-04-11 17:15:32.000000 ratinabox-1.4.1/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.250855 ratinabox-1.4.1/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25185 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-11 17:41:30.257745 ratinabox-1.4.1/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.4.1/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.257054 ratinabox-1.4.1/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-01-09 16:43:43.000000 ratinabox-1.4.1/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.4.1/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.4.1/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.4.1/tests/test_neurons.py
```

### Comparing `ratinabox-1.4.0/LICENSE` & `ratinabox-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/PKG-INFO` & `ratinabox-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.4.0
+Version: 1.4.1
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: demos
 Provides-Extra: test
 License-File: LICENSE
 
 # RatInABox 
 ![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
@@ -67,21 +66,21 @@
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically. 
 
 **Install** the latest, stable version using `pip` at the command line with
 ```console
 $ pip install ratinabox
 ```
-Alternatively, in particular if you would like to edit `RatInABox` code, install locally using  
+Alternatively, in particular if you would like to develop `RatInABox` code or if you want the bleeding edge (may occasioanlly break), install from this repo using  
 ```console
 $ git clone --depth 1 https://github.com/TomGeorge1234/RatInABox.git
 $ cd RatInABox
 $ pip install -e .
 ```
-n.b. the `-e` (`--editable`) handle means this install points *directly* to the cloned repository itself. Any changes made here will be reflected when you next import `RatInABox` into your code. If you want to run the demo jupyter scripts please replace the last call with `pip install -e .[demos]`.
+n.b. the "editable" `-e` handle means changes made to your clone will be reflected when you next import `RatInABox` into your code.
 
 **Import** into your python project with  
 ```python
 import ratinabox
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import PlaceCells, GridCells #...
```

### Comparing `ratinabox-1.4.0/README.md` & `ratinabox-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically. 
 
 **Install** the latest, stable version using `pip` at the command line with
 ```console
 $ pip install ratinabox
 ```
-Alternatively, in particular if you would like to edit `RatInABox` code, install locally using  
+Alternatively, in particular if you would like to develop `RatInABox` code or if you want the bleeding edge (may occasioanlly break), install from this repo using  
 ```console
 $ git clone --depth 1 https://github.com/TomGeorge1234/RatInABox.git
 $ cd RatInABox
 $ pip install -e .
 ```
-n.b. the `-e` (`--editable`) handle means this install points *directly* to the cloned repository itself. Any changes made here will be reflected when you next import `RatInABox` into your code. If you want to run the demo jupyter scripts please replace the last call with `pip install -e .[demos]`.
+n.b. the "editable" `-e` handle means changes made to your clone will be reflected when you next import `RatInABox` into your code.
 
 **Import** into your python project with  
 ```python
 import ratinabox
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import PlaceCells, GridCells #...
```

### Comparing `ratinabox-1.4.0/ratinabox/Agent.py` & `ratinabox-1.4.1/ratinabox/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,15 +562,14 @@
         alpha=0.7,
         xlim=None,
         background_color=None,
         axis_labels=True,
         autosave=None,
         **kwargs,
     ):
-
         """Plots the trajectory between t_start (seconds) and t_end (defaulting to the last time available)
         Args:
             • t_start: start time in seconds
             • t_end: end time in seconds (default = self.history["t"][-1])
             • framerate: how many scatter points / per second of motion to display
             • fig, ax: the fig, ax to plot on top of, optional, if not provided used self.Environment.plot_Environment().
               This can be used to plot trajectory on top of receptive fields etc.
@@ -625,19 +624,19 @@
                 color[-1] = "r"
 
             ax.scatter(
                 trajectory[:, 0],
                 trajectory[:, 1],
                 s=s,
                 alpha=alpha,
-                zorder=0,
+                zorder=1.1,
                 c=color,
                 linewidth=0,
             )
-            # #plot the rat? TODO haha
+            # #plot the rat? TODO haha probably never gonna do this
             # ratpath = os.path.join(
             #     os.path.abspath(os.path.join(ratinabox.__file__, os.pardir)),
             #         "data/rat.png",
             #     )
             # rat = plt.imread(ratpath)
             # rect = 0.5, 0.4, 0.4, 0.4 # What should these values be?
             # newax = fig.add_axes(rect, anchor='NE', zorder=1)
```

### Comparing `ratinabox-1.4.0/ratinabox/Environment.py` & `ratinabox-1.4.1/ratinabox/Environment.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/Neurons.py` & `ratinabox-1.4.1/ratinabox/Neurons.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,37 +358,41 @@
                 axes = np.array([ax]).reshape(-1)
                 if method in ["groundtruth", "history"]:
                     if colorbar == True:
                         from mpl_toolkits.axes_grid1 import make_axes_locatable
 
                         divider = make_axes_locatable(axes[-1])
                         cax = divider.append_axes("right", size="5%", pad=0.05)
-            for (i, ax_) in enumerate(axes):
+            for i, ax_ in enumerate(axes):
                 _, ax_ = self.Agent.Environment.plot_environment(
                     fig, ax_, autosave=False
                 )
             if len(chosen_neurons) != axes.size:
                 print(
                     f"You are trying to plot a different number of neurons {len(chosen_neurons)} than the number of axes provided {axes.size}. Some might be missed. Either change this with the chosen_neurons argument or pass in a list of axes to plot on"
                 )
 
             vmin, vmax = 0, 0
             ims = []
             if method in ["groundtruth", "history"]:
-                for (i, ax_) in enumerate(axes):
+                for i, ax_ in enumerate(axes):
                     ex = self.Agent.Environment.extent
                     if method == "groundtruth":
                         rate_map = rate_maps[chosen_neurons[i], :].reshape(
                             self.Agent.Environment.discrete_coords.shape[:2]
                         )
                         im = ax_.imshow(rate_map, extent=ex, zorder=0, cmap="inferno")
                     elif method == "history":
                         rate_timeseries_ = rate_timeseries[chosen_neurons[i], :]
                         rate_map = utils.bin_data_for_histogramming(
-                            data=pos, extent=ex, dx=0.05, weights=rate_timeseries_
+                            data=pos,
+                            extent=ex,
+                            dx=0.05,
+                            weights=rate_timeseries_,
+                            norm_by_bincount=True,
                         )
                         im = ax_.imshow(
                             rate_map,
                             extent=ex,
                             cmap="inferno",
                             interpolation="bicubic",
                             zorder=1,
@@ -404,15 +408,15 @@
                     cbar = plt.colorbar(ims[-1], cax=cax)
                     lim_v = vmax if vmax > -vmin else vmin
                     cbar.set_ticks([0, lim_v])
                     cbar.set_ticklabels([0, round(lim_v, 1)])
                     cbar.outline.set_visible(False)
 
             if spikes is True:
-                for (i, ax_) in enumerate(axes):
+                for i, ax_ in enumerate(axes):
                     pos_where_spiked = pos[spike_data[chosen_neurons[i], :]]
                     ax_.scatter(
                         pos_where_spiked[:, 0],
                         pos_where_spiked[:, 1],
                         s=2,
                         linewidth=0,
                         alpha=0.7,
@@ -429,14 +433,15 @@
                 rate_maps = []
                 for neuron_id in chosen_neurons:
                     rate_map, x = utils.bin_data_for_histogramming(
                         data=pos_,
                         extent=ex,
                         dx=0.01,
                         weights=rate_timeseries[neuron_id, :],
+                        norm_by_bincount=True,
                     )
                     x, rate_map = utils.interpolate_and_smooth(x, rate_map, sigma=0.03)
                     rate_maps.append(rate_map)
                 rate_maps = np.array(rate_maps)
 
             if fig is None and ax is None:
                 fig, ax = self.Agent.Environment.plot_environment(
@@ -1221,15 +1226,14 @@
         "beta": 12,
         "max_fr":1, # likely max firing rate of an OVC
         "min_fr":0, # likely min firing rate
     }
     """
 
     def __init__(self, Agent, params={}):
-
         default_params = {
             "n": 10,
             "name": "ObjectVectorCell",
             "walls_occlude": True,
             "reference_frame": "allocentric",
             "angle_spread_degrees": 15,
             "pref_object_dist": 0.25,
@@ -1709,15 +1713,15 @@
                     f"There already exists a layer called {name}. Overwriting it now."
                 )
         self.inputs[name] = {}
         self.inputs[name]["layer"] = input_layer
         self.inputs[name]["w"] = w
         self.inputs[name]["w_init"] = w.copy()
         self.inputs[name]["I"] = I
-        for (key, value) in kwargs.items():
+        for key, value in kwargs.items():
             self.inputs[name][key] = value
         if ratinabox.verbose is True:
             print(
                 f'An input layer called {name} was added. The weights can be accessed with "self.inputs[{name}]["w"]"'
             )
 
     def get_state(self, evaluate_at="last", **kwargs):
```

### Comparing `ratinabox-1.4.0/ratinabox/README.md` & `ratinabox-1.4.1/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/__init__.py` & `ratinabox-1.4.1/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.4.1/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.4.1/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.4.1/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/contribs/README.md` & `ratinabox-1.4.1/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.4.1/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.4.1/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,14 +258,15 @@
         )  # decays sequences fast if animated
         kwargs_["framerate"] = (
             self.v_sequence / 0.02
         )  # 2cm point seperation for sequences
         kwargs_["color"] = "C1"
         kwargs_["alpha"] = 0.4
         kwargs_["plot_agent"] = False
+        kwargs_["autosave"] = False
 
         if sequences_ontop == False:
             fig, ax = super(ThetaSequenceAgent, self).plot_trajectory(**kwargs_)
             kwargs["fig"] = fig
             kwargs["ax"] = ax
             kwargs["alpha"] = 0.4
             fig, ax = self.TrueAgent.plot_trajectory(**kwargs)
```

### Comparing `ratinabox-1.4.0/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.4.1/ratinabox/contribs/ValueNeuron.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/data/README.md` & `ratinabox-1.4.1/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/data/rat.png` & `ratinabox-1.4.1/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/data/sargolini.npz` & `ratinabox-1.4.1/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/data/tanni.npz` & `ratinabox-1.4.1/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/ratinabox/utils.py` & `ratinabox-1.4.1/ratinabox/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -413,42 +413,51 @@
     v = v * norm
     return v
 
 
 """Plotting functions"""
 
 
-def bin_data_for_histogramming(data, extent, dx, weights=None):
+def bin_data_for_histogramming(data, extent, dx, weights=None, norm_by_bincount=False):
     """Bins data ready for plotting.
     So for example if the data is 1D the extent is broken up into bins (leftmost edge = extent[0], rightmost edge = extent[1]) and then data is
     histogrammed into these bins.
     weights weights the histogramming process so the contribution of each data point to a bin count is the weight, not 1.
-
+    norm_by_bincount divides the histogram by the number of data points in each bin. This is useful if you want to plot just the average of the wegihts normalising out any contribution from the number of data points in each bin.
     Args:
         data (array): (2,N) for 2D or (N,) for 1D)
         extent (_type_): _description_
         dx (_type_): _description_
         weights (_type_, optional): _description_. Defaults to None.
 
     Returns:
         (heatmap,bin_centres): if 1D
         (heatmap): if 2D
     """
     if len(extent) == 2:  # dimensionality = "1D"
         bins = np.arange(extent[0], extent[1] + dx, dx)
         heatmap, xedges = np.histogram(data, bins=bins, weights=weights)
+        if norm_by_bincount:
+            bincount = np.histogram(data, bins=bins)[0]
+            heatmap = heatmap / bincount
         centres = (xedges[1:] + xedges[:-1]) / 2
         return (heatmap, centres)
 
     elif len(extent) == 4:  # dimensionality = "2D"
         bins_x = np.arange(extent[0], extent[1] + dx, dx)
         bins_y = np.arange(extent[2], extent[3] + dx, dx)
         heatmap, xedges, yedges = np.histogram2d(
             data[:, 0], data[:, 1], bins=[bins_x, bins_y], weights=weights
         )
+        if norm_by_bincount:
+            bincount, xedges, yedges = np.histogram2d(
+                data[:, 0], data[:, 1], bins=[bins_x, bins_y]
+            )
+            bincount[bincount == 0] = 1
+            heatmap = heatmap / bincount
         heatmap = heatmap.T[::-1, :]
         return heatmap
 
 
 def mountain_plot(
     X,
     NbyX,
@@ -491,16 +500,16 @@
 
     if norm_by == "max":
         NbyX = overlap * NbyX / np.max(np.abs(NbyX))
     else:
         NbyX = overlap * NbyX / norm_by
     if fig is None and ax is None:
         fig, ax = plt.subplots()
+        fig.set_size_inches(4, len(NbyX) * shift / 25)
 
-    fig.set_size_inches(4, len(NbyX) * shift / 25)
     zorder = 1
     for i in range(len(NbyX)):
         ax.plot(X, NbyX[i] + i + 1, c=c, zorder=zorder)
         zorder -= 0.01
         ax.fill_between(
             X, NbyX[i] + i + 1, i + 1, color=fc, zorder=zorder, alpha=0.8, linewidth=0
         )
@@ -523,16 +532,16 @@
 
     return fig, ax
 
 
 def save_figure(
     fig,
     save_title="",
-    fig_save_types=["svg", "png"],
-    anim_save_types=["gif", "mp4"],
+    fig_save_types=["png", "svg"],
+    anim_save_types=["mp4", "gif"],
     save=True,
 ):
     """
     Saves a figure in a dated-folder with the current time appended to save_title, as both '.png' and '.svg'. Same for animations but as ".gif" and ".mp4".
     This function can be used by anyone...just pass a fig object and it will be saved in the right place.
 
     Args:
@@ -599,39 +608,45 @@
 
     figdir = figure_directory + f"{today}/"
     now = datetime.strftime(datetime.now(), "%H%M")
     path_ = f"{figdir}{save_title}_{now}"
     path = path_
 
     if type(fig) == matplotlib.figure.Figure:
+        file_type = "Figure"
+        save_types = "  & .".join(fig_save_types)
         for filetype in fig_save_types:
             i = 1
             while True:  # checks there isn't an existing figure with this name
                 if os.path.isfile(path + "." + filetype):
                     path = path_ + "_" + str(i)
                     i += 1
                 elif i >= 100:
                     break
                 else:
                     break
             fig.savefig(path + "." + filetype, bbox_inches="tight")
 
     elif type(fig) == matplotlib.animation.FuncAnimation:
+        file_type = "Animation"
+        save_types = "  & .".join(anim_save_types)
         for filetype in anim_save_types:
             i = 1
             while True:
                 if os.path.isfile(path + "." + filetype):
                     path = path_ + "_" + str(i)
                     i += 1
                 elif i >= 100:
                     break
                 else:
                     break
             fig.save(path + "." + filetype)
 
+    print(f"{file_type} saved to {os.path.abspath(path)}.{save_types}")
+
     return path
 
 
 def save_animation(*args, **kwargs):
     """Saves an animation. This function just passes the animation object to utils.save_figure() where it is then saved. We only include this function for semantic consistency (you could just use save_figure directly. Takes exactly the same args are save_figure() and just passes the animation over there"""
     return save_figure(*args, **kwargs)
```

### Comparing `ratinabox-1.4.0/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.4.1/ratinabox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.4.0
+Version: 1.4.1
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: demos
 Provides-Extra: test
 License-File: LICENSE
 
 # RatInABox 
 ![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
@@ -67,21 +66,21 @@
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically. 
 
 **Install** the latest, stable version using `pip` at the command line with
 ```console
 $ pip install ratinabox
 ```
-Alternatively, in particular if you would like to edit `RatInABox` code, install locally using  
+Alternatively, in particular if you would like to develop `RatInABox` code or if you want the bleeding edge (may occasioanlly break), install from this repo using  
 ```console
 $ git clone --depth 1 https://github.com/TomGeorge1234/RatInABox.git
 $ cd RatInABox
 $ pip install -e .
 ```
-n.b. the `-e` (`--editable`) handle means this install points *directly* to the cloned repository itself. Any changes made here will be reflected when you next import `RatInABox` into your code. If you want to run the demo jupyter scripts please replace the last call with `pip install -e .[demos]`.
+n.b. the "editable" `-e` handle means changes made to your clone will be reflected when you next import `RatInABox` into your code.
 
 **Import** into your python project with  
 ```python
 import ratinabox
 from ratinabox.Environment import Environment
 from ratinabox.Agent import Agent
 from ratinabox.Neurons import PlaceCells, GridCells #...
```

### Comparing `ratinabox-1.4.0/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.4.1/ratinabox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/setup.cfg` & `ratinabox-1.4.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.4.0
+version = 1.4.1
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
@@ -25,18 +25,14 @@
 	matplotlib
 	scipy
 	shapely
 python_requires = >=3.7
 include_package_data = False
 
 [options.extras_require]
-demos = 
-	jupyter ~= 1.0.0
-	tqdm ~= 4.62.3
-	scikit-learn ~= 1.2.0
 test = 
 	pytest
 
 [options.package_data]
 ratinabox = data/*
 * = README.md
```

### Comparing `ratinabox-1.4.0/tests/test_advanced.py` & `ratinabox-1.4.1/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.0/tests/test_environment.py` & `ratinabox-1.4.1/tests/test_environment.py`

 * *Files identical despite different names*

