# Comparing `tmp/energyplus_launch-3.5.7.tar.gz` & `tmp/energyplus_launch-3.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.5.7.tar", last modified: Thu Apr  6 19:45:44 2023, max compression
+gzip compressed data, was "energyplus_launch-3.5.8.tar", last modified: Tue Apr 11 17:59:25 2023, max compression
```

## Comparing `energyplus_launch-3.5.7.tar` & `energyplus_launch-3.5.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:44.401949 energyplus_launch-3.5.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-04-06 19:45:44.401949 energyplus_launch-3.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:44.397949 energyplus_launch-3.5.7/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-04-06 19:45:44.000000 energyplus_launch-3.5.7/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-06 19:45:44.000000 energyplus_launch-3.5.7/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 19:45:44.000000 energyplus_launch-3.5.7/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-06 19:45:44.000000 energyplus_launch-3.5.7/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-06 19:45:44.000000 energyplus_launch-3.5.7/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-06 19:45:44.000000 energyplus_launch-3.5.7/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:44.397949 energyplus_launch-3.5.7/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:44.401949 energyplus_launch-3.5.7/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8728 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     6469 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    57229 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5813 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     4808 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:44.401949 energyplus_launch-3.5.7/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10882 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:44.401949 energyplus_launch-3.5.7/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:44.401949 energyplus_launch-3.5.7/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)     9790 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-06 19:45:44.401949 energyplus_launch-3.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-06 19:45:38.000000 energyplus_launch-3.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.841486 energyplus_launch-3.5.8/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 17:59:25.000000 energyplus_launch-3.5.8/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.841486 energyplus_launch-3.5.8/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8727 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6648 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63951 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5813 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4808 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9936 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-11 17:59:25.845486 energyplus_launch-3.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-11 17:59:20.000000 energyplus_launch-3.5.8/setup.py
```

### Comparing `energyplus_launch-3.5.7/LICENSE` & `energyplus_launch-3.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/PKG-INFO` & `energyplus_launch-3.5.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.5.7
+Version: 3.5.8
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
@@ -29,14 +29,15 @@
         
         ## Releases
         
         [![Releases](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/pypi.yml?label=Releases&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/pypi.yml)
         
         When a tag is created in the GitHub Repo, Github Actions builds a Python wheel and uploads it to PyPi: https://pypi.org/project/ep-launch/.
         The packages can be downloaded using standard `pip install energyplus-launch` commands.
+        Once Pip installed, desktop shortcuts and launchers can be configured using the `energyplus-launch-configure` command from the same Python environment.
         
         ## Development
         
         Basic development dependencies are installed with `pip install -r requirements.txt`.
         This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
         The application can be run by executing the module as `python -m eplaunch` file.
         To run the unit test suite, simply execute `nosetests`.
```

### Comparing `energyplus_launch-3.5.7/README.md` & `energyplus_launch-3.5.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 ## Releases
 
 [![Releases](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/pypi.yml?label=Releases&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/pypi.yml)
 
 When a tag is created in the GitHub Repo, Github Actions builds a Python wheel and uploads it to PyPi: https://pypi.org/project/ep-launch/.
 The packages can be downloaded using standard `pip install energyplus-launch` commands.
+Once Pip installed, desktop shortcuts and launchers can be configured using the `energyplus-launch-configure` command from the same Python environment.
 
 ## Development
 
 Basic development dependencies are installed with `pip install -r requirements.txt`.
 This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
 The application can be run by executing the module as `python -m eplaunch` file.
 To run the unit test suite, simply execute `nosetests`.
```

### Comparing `energyplus_launch-3.5.7/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.5.8/energyplus_launch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.5.7
+Version: 3.5.8
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
@@ -29,14 +29,15 @@
         
         ## Releases
         
         [![Releases](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/pypi.yml?label=Releases&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/pypi.yml)
         
         When a tag is created in the GitHub Repo, Github Actions builds a Python wheel and uploads it to PyPi: https://pypi.org/project/ep-launch/.
         The packages can be downloaded using standard `pip install energyplus-launch` commands.
+        Once Pip installed, desktop shortcuts and launchers can be configured using the `energyplus-launch-configure` command from the same Python environment.
         
         ## Development
         
         Basic development dependencies are installed with `pip install -r requirements.txt`.
         This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
         The application can be run by executing the module as `python -m eplaunch` file.
         To run the unit test suite, simply execute `nosetests`.
```

### Comparing `energyplus_launch-3.5.7/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.5.8/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/config.py` & `energyplus_launch-3.5.8/eplaunch/interface/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def __init__(self):
         # specify configuration settings here
         self.keep_dialog_open: bool = True
         self.cur_workflow_name: str = ''
         self.cur_workflow_context: str = ''
         self.directory: Path = Path.home()  # default to the home directory
-        self.file_selection: List[Path] = []
+        self.file_selection: List[str] = []
         self.welcome_shown: bool = False
         self.latest_welcome_shown: str = ''
         self.height: int = -1
         self.width: int = -1
         self.x: int = -1
         self.y: int = -1
         self.workflow_directories: List[Path] = []
```

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.5.8/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.5.8/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.5.8/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.5.8/eplaunch/interface/dialog_weather.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from pathlib import Path
 from tkinter import Tk, Toplevel, Frame, LabelFrame, StringVar, Radiobutton, TOP, W, Button, EW, NSEW, Entry, \
-    ALL, ACTIVE, DISABLED, filedialog, Label, OptionMenu, E, messagebox
+    ALL, ACTIVE, DISABLED, filedialog, Label, OptionMenu, E, messagebox, CENTER
 from typing import List, Optional
 
 
 class TkWeatherDialog(Toplevel):
     CLOSE_SIGNAL_OK = 0
     CLOSE_SIGNAL_CANCEL = 1
     WEATHER_TYPE_DD = "DD"
     WEATHER_TYPE_EPW = "EPW"
 
-    def __init__(self, parent_window, recent_files: List[Path], favorite_files: List[Path]):
+    def __init__(self, parent_window, recent_files: List[Path], favorite_files: List[Path], text: Optional[str] = None):
         super().__init__()
+        self.alt_text = text
         self.title("Choose Weather Configuration")
         # assume cancel to allow for closing the dialog with the X
         self.exit_code = self.CLOSE_SIGNAL_CANCEL
         self.selected_weather_file: Optional[Path] = None
         # build the gui and call required modal methods
         self._define_tk_variables()
         self._epw_set = False
@@ -28,14 +29,16 @@
         self._tk_var_weather_type.trace('w', self._weather_type_changed)
         self._tk_var_recent = StringVar(value="")
         self._tk_var_favorite = StringVar(value="")
         self._tk_var_epw_path = StringVar(value="<epw path>")
 
     def _build_gui(self, recent_files: List[Path], favorite_files: List[Path]):
         lf = LabelFrame(self, text="Choose a Weather File Configuration Option")
+        if self.alt_text:
+            Label(lf, text=self.alt_text).pack(side=TOP, anchor=CENTER, padx=3, pady=3)
         Radiobutton(
             lf, text="Design Days (Use Design Days Only; No Weather File)",
             value=self.WEATHER_TYPE_DD, variable=self._tk_var_weather_type
         ).pack(
             side=TOP, anchor=W, padx=3, pady=3
         )
         Radiobutton(
```

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.5.8/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/frame_main.py` & `energyplus_launch-3.5.8/eplaunch/interface/frame_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from mimetypes import guess_type
 from pathlib import Path
 from platform import system
 from queue import Queue
 
 from subprocess import Popen
 from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, OptionMenu, Frame, Label, Button, NSEW, \
-    SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, ACTIVE, LabelFrame, RIGHT, EW, PanedWindow, NS, filedialog
+    SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, ACTIVE, LabelFrame, RIGHT, EW, PanedWindow, NS, filedialog, ALL
 from tkinter.ttk import Combobox
 from typing import Dict, List, Optional, Tuple
 from uuid import uuid4
 from webbrowser import open as open_web
 from plan_tools.runtime import fixup_taskbar_icon_on_windows
 
 from eplaunch import VERSION, DOCS_URL, NAME
@@ -24,27 +24,28 @@
 from eplaunch.interface.widget_file_list import FileListScrollableFrame
 from eplaunch.interface.dialog_external_viewers import TkViewerDialog
 from eplaunch.interface.dialog_weather import TkWeatherDialog
 from eplaunch.interface.dialog_workflow_dirs import TkWorkflowsDialog
 from eplaunch.interface.dialog_output import TkOutputDialog
 from eplaunch.workflows.workflow_thread import WorkflowThread
 from eplaunch.utilities.cache import CacheFile
-from eplaunch.workflows.base import EPLaunchWorkflowResponse1
+from eplaunch.workflows.base import BaseEPLaunchWorkflow1, EPLaunchWorkflowResponse1
 from eplaunch.workflows.manager import WorkflowManager
 from eplaunch.workflows.workflow import Workflow
 
 
 class EPLaunchWindow(Tk):
 
     # region Construction and GUI building functions
 
     def __init__(self):
         super().__init__(className=NAME)
         # set the form title and icon, basic stuff
         self.title("EnergyPlus Launch")
+        self.option_add('*Dialog.msg.font', 'Helvetica 12')
         if system() == 'Darwin':
             self.icon_path = Path(__file__).resolve().parent.parent / 'icons' / 'icon.icns'
             if self.icon_path.exists():
                 self.iconbitmap(str(self.icon_path))
             else:
                 print(f"Could not set icon for Mac, expecting to find it at {self.icon_path}")
         elif system() == 'Windows':
@@ -72,21 +73,22 @@
 
         # create a config manager and load up the saved, or default, configuration
         self.conf = ConfigManager()
         self.conf.load()
 
         # initialize some dir/file selection variables
         self.previous_selected_directory: Optional[Path] = None
-        self.current_cache: Optional[CacheFile] = None
 
-        # create a workflow manager, it will initialize (EnergyPlus) workflows in predetermined locations
+        # create a workflow manager, it will initialize workflows in predetermined locations
         self.workflow_manager = WorkflowManager()
+
         # but now, if the saved configuration exists, use that as the list of directories to use moving forward
         if self.conf.workflow_directories:
             self.workflow_manager.workflow_directories = self.conf.workflow_directories
+
         # now that we have a list of workflows, instantiate any/all of them
         self.workflow_manager.instantiate_all_workflows()
         if len(self.workflow_manager.warnings) > 0:
             self.generic_dialogs.display(
                 self, 'Workflow Processing Errors', '\n'.join(self.workflow_manager.warnings)
             )
 
@@ -126,14 +128,19 @@
         # bind key presses for the app
         self.bind('<Key>', self._handle_keyboard_press)
 
     def _define_tk_variables(self):
         self._tk_var_workflow_context = StringVar(value='<context>')
         self._tk_var_workflow_instance = StringVar(value='<instance>')
         self._tk_var_output_suffix = StringVar(value='<output')
+        self._tk_var_output_1 = StringVar(value='--')
+        self._tk_var_output_2 = StringVar(value='--')
+        self._tk_var_output_3 = StringVar(value='--')
+        self._tk_var_output_4 = StringVar(value='--')
+        self._tk_var_output_5 = StringVar(value='--')
         self._tk_var_status_dir = StringVar(value="Selected dir")
         self._tk_var_status_workflow = StringVar(value="Selected workflow")
         self._tk_var_status_message = StringVar(value="Status Message")
         self._tk_var_weather_recent = StringVar(value="<recent>")
 
     def _build_gui(self):
         self._build_top_menu()
@@ -159,49 +166,46 @@
         y = max(self.conf.y, 128)
         self.wm_geometry(f"{width}x{height}+{x}+{y}")
 
     def _build_top_menu(self):
         menubar = Menu(self)
 
         menu_file = Menu(menubar, tearoff=False)
-        menu_file.add_command(label="Run Current Workflow on Selection", command=self._run_workflow)
+        menu_file.add_command(label="Run Current Workflow on Selection", command=self._run_workflow_on_selection)
+        menu_file.add_command(label="Run Current Workflow on Current Group", command=self._run_workflow_on_group)
         menu_file.add_command(label="Quit", command=self.window_close)
         menubar.add_cascade(label="File", menu=menu_file)
 
         menu_nav = Menu(menubar, tearoff=False)
         self.menu_nav_recent = Menu(menu_nav, tearoff=False)
         menu_nav.add_cascade(label="Recent", menu=self.menu_nav_recent)
         menu_nav.add_command(label="Navigate to previous folder", command=self._navigate_to_previous_folder)
         menu_nav.add_separator()
         self.menu_nav_favorites = Menu(menu_nav, tearoff=False)
         menu_nav.add_cascade(label="Favorites", menu=self.menu_nav_favorites)
         menu_nav.add_command(label="Add Current Folder to Favorites", command=self.add_folder_to_favorites)
         menu_nav.add_command(label="Remove Current Folder from Favorites", command=self.remove_folder_from_favorites)
-        menu_nav.add_separator()
-        self.menu_nav_group = Menu(menu_nav, tearoff=False)
-        menu_nav.add_cascade(label="Current Group", menu=self.menu_nav_group)
-        menu_nav.add_command(label="Clear Current Group", command=self._clear_group)
-        menu_nav.add_command(label="Load new Group file...", command=self._load_new_group_file)
-        menu_nav.add_command(label="Save Current Group to file...", command=self._save_group_file)
-        menu_nav.add_command(
-            label="Add current folder to current group", command=self._add_current_dir_to_group
-        )
-        menu_nav.add_command(
-            label="Add current file selection to current group", command=self._add_current_files_to_group
-        )
-        menu_nav.add_command(
-            label="Remove current folder from current group", command=self._remove_current_dir_from_group
+        menubar.add_cascade(label="Navigation", menu=menu_nav)
+
+        menu_group = Menu(menubar, tearoff=False)
+        self.menu_group_current = Menu(menu_group, tearoff=False)
+        menu_group.add_cascade(label="Current Group", menu=self.menu_group_current)
+        menu_group.add_command(label="Clear Current Group", command=self._clear_group)
+        menu_group.add_command(label="Load new Group file...", command=self._load_new_group_file)
+        menu_group.add_command(label="Save Current Group to file...", command=self._save_group_file)
+        menu_group.add_command(
+            label="Add selected files to current group", command=self._add_current_files_to_group
         )
-        menu_nav.add_command(
-            label="Remove current file selection from current group", command=self._remove_current_files_from_group
+        menu_group.add_command(
+            label="Remove selected files from current group", command=self._remove_current_files_from_group
         )
-        menu_nav.add_command(
+        menu_group.add_command(
             label="Cycle through current group entries", command=self._cycle_through_group
         )
-        menubar.add_cascade(label="Navigation", menu=menu_nav)
+        menubar.add_cascade(label="Group", menu=menu_group)
 
         menu_settings = Menu(menubar, tearoff=False)
         menu_settings.add_command(label="Workflow Directories", command=self._open_workflow_dir_dialog)
         self._tk_var_keep_dialogs_open = BooleanVar(value=True)
         menu_settings.add_checkbutton(
             label="Keep Output Dialog Open", onvalue=True, offvalue=False, variable=self._tk_var_keep_dialogs_open
         )
@@ -219,55 +223,89 @@
         menu_help.add_command(label="About...", command=self._open_about)
         menubar.add_cascade(label="Help", menu=menu_help)
 
         self.config(menu=menubar)
 
     # noinspection SqlNoDataSourceInspection
     def _build_top_icon_bar(self, container: Frame):
-        lf = LabelFrame(container, text="Workflow Operations")
+        lf = LabelFrame(container, text="Workflow Selection")
         Label(lf, text="Context:", justify=RIGHT).grid(row=0, column=0, **self.pad)
         self.option_workflow_context = OptionMenu(lf, self._tk_var_workflow_context, '<context>')
         self.option_workflow_context.grid(row=0, column=1, sticky=EW, **self.pad)
         Label(lf, text="Workflow: ", justify=RIGHT).grid(row=1, column=0, **self.pad)
         self.option_workflow_instance = OptionMenu(lf, self._tk_var_workflow_instance, '<instance>')
         self.option_workflow_instance.grid(row=1, column=1, sticky=EW, **self.pad)
+        lf.grid(row=0, column=0, sticky=NS, **self.pad)
+
+        lf = LabelFrame(container, text="Workflow Execution")
         Button(
-            lf, text=u"\U000025B6 Run Workflow on Current File(s)", command=self._run_workflow
-        ).grid(row=2, column=0, columnspan=2, sticky=EW, **self.pad)
-        lf.grid(row=0, column=0, **self.pad)
-
-        lf = LabelFrame(container, text="Weather")
-        Label(lf, text="Set Weather from Recent or from File").grid(row=0, column=0, columnspan=3, **self.pad)
-        Label(lf, text="Recent: ", justify=RIGHT).grid(row=1, column=0, **self.pad)
+            lf, text=u"\U000025B6 Run Workflow on Current File(s)", command=self._run_workflow_on_selection
+        ).grid(row=0, column=0, sticky=EW, **self.pad)
+        Button(
+            lf, text=u"\U000025B6 Run Workflow on Current Group", command=self._run_workflow_on_group
+        ).grid(row=1, column=0, sticky=EW, **self.pad)
+        lf.grid(row=0, column=1, sticky=NS, **self.pad)
+
+        lf = LabelFrame(container, text="Weather Selection")
+        Label(lf, text="Recent: ", justify=RIGHT).grid(row=0, column=0, **self.pad)
         self.option_weather_recent = Combobox(lf, textvariable=self._tk_var_weather_recent)
-        self.option_weather_recent.grid(row=1, column=1, **self.pad)
+        self.option_weather_recent.grid(row=0, column=1, **self.pad)
         self.option_weather_recent['state'] = 'readonly'
         self.button_weather_set = Button(lf, text=u"\U00002713 Set", command=self._set_weather_from_recent)
-        self.button_weather_set.grid(row=1, column=2, **self.pad)
+        self.button_weather_set.grid(row=0, column=2, **self.pad)
         self.button_weather_select = Button(
             lf, text=u"\U0001f325 Select Weather From Disk...", command=self._open_weather_dialog
         )
-        self.button_weather_select.grid(row=2, column=0, columnspan=3, sticky=EW, **self.pad)
-        lf.grid(row=0, column=1, sticky=NS, **self.pad)
+        self.button_weather_select.grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+        lf.grid(row=0, column=2, sticky=NS, **self.pad)
 
-        lf = LabelFrame(container, text="File/Folder Actions")
-        Label(lf, text="Open Output: ", justify=RIGHT).grid(row=0, column=0, **self.pad)
-        self.option_workflow_outputs = Combobox(lf, textvariable=self._tk_var_output_suffix)
-        self.option_workflow_outputs.grid(row=0, column=1, **self.pad)
-        self.option_workflow_outputs['state'] = 'readonly'
-        self.button_open_output_file = Button(lf, text=u"\U0001f325 Open", command=self._open_output_file)
-        self.button_open_output_file.grid(row=0, column=2, **self.pad)
+        lf = LabelFrame(container, text="Quicklinks")
         self.button_open_in_text = Button(
             lf, text=u"\U0001F5B9 Open Selected File in Text Editor", command=self._open_text_editor, state=DISABLED
         )
-        self.button_open_in_text.grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+        self.button_open_in_text.grid(row=0, column=0, columnspan=3, sticky=EW, **self.pad)
         Button(
             lf, text=u"\U0001F5C0 Open Dir in File Browser", command=self._open_file_browser
-        ).grid(row=2, column=0, columnspan=3, sticky=EW, **self.pad)
-        lf.grid(row=0, column=2, **self.pad)
+        ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+        lf.grid(row=0, column=3, sticky=NS, **self.pad)
+
+        lf = LabelFrame(container, text="Open Outputs")
+        sub_frame = Frame(lf)
+        self.button_open_output_1 = Button(
+            sub_frame, textvariable=self._tk_var_output_1, command=self._open_output_1, state=DISABLED
+        )
+        self.button_open_output_1.grid(row=0, column=0, sticky=EW, **self.pad)
+        self.button_open_output_2 = Button(
+            sub_frame, textvariable=self._tk_var_output_2, command=self._open_output_2, state=DISABLED
+        )
+        self.button_open_output_2.grid(row=0, column=1, sticky=EW, **self.pad)
+        self.button_open_output_3 = Button(
+            sub_frame, textvariable=self._tk_var_output_3, command=self._open_output_3, state=DISABLED
+        )
+        self.button_open_output_3.grid(row=0, column=2, sticky=EW, **self.pad)
+        self.button_open_output_4 = Button(
+            sub_frame, textvariable=self._tk_var_output_4, command=self._open_output_4, state=DISABLED
+        )
+        self.button_open_output_4.grid(row=0, column=3, sticky=EW, **self.pad)
+        self.button_open_output_5 = Button(
+            sub_frame, textvariable=self._tk_var_output_5, command=self._open_output_5, state=DISABLED
+        )
+        self.button_open_output_5.grid(row=0, column=4, sticky=EW, **self.pad)
+        sub_frame.grid_columnconfigure(ALL, weight=1)
+        sub_frame.grid_rowconfigure(ALL, weight=1)
+        sub_frame.grid(row=0, column=0, columnspan=3, sticky=EW, **self.pad)
+        Label(lf, text="Full List: ", justify=RIGHT).grid(row=1, column=0, **self.pad)
+        self.option_workflow_outputs = Combobox(lf, textvariable=self._tk_var_output_suffix)
+        self.option_workflow_outputs.grid(row=1, column=1, **self.pad)
+        self.option_workflow_outputs['state'] = 'readonly'
+        self.button_open_output_file = Button(lf, text=u"\U0001f325 Open", command=self._open_output_file)
+        self.button_open_output_file.grid(row=1, column=2, **self.pad)
+        lf.grid_columnconfigure(ALL, weight=1)
+        lf.grid_rowconfigure(ALL, weight=1)
+        lf.grid(row=0, column=4, sticky=NS, **self.pad)
 
     def _build_listings(self, container: Frame):
         pw = PanedWindow(container)  # default horizontal
         self.dir_tree = DirListScrollableFrame(pw, on_select=self._new_dir_selected, on_root_changed=self._new_root_dir)
         pw.add(self.dir_tree)
         self.file_list = FileListScrollableFrame(container, on_selection_changed=self._callback_file_selection_changed)
         pw.add(self.file_list)
@@ -348,15 +386,17 @@
         mod_control = 0x4
         # mod_alt = 0x20000
         if event.keysym == 'F5':
             self._update_file_list()
         elif event.keysym == 'w' and mod_control & event.state:
             self._open_weather_dialog()
         elif event.keysym == 'r' and mod_control & event.state:
-            self._run_workflow()
+            self._run_workflow_on_selection()
+        elif event.keysym == 'g' and mod_control & event.state:
+            self._run_workflow_on_group()
         elif event.keysym == 'm' and mod_control & event.state:
             self._cycle_through_group()
         elif event.keysym == 'z' and mod_control & event.state:
             self._navigate_to_previous_folder()
 
     # endregion
 
@@ -366,15 +406,15 @@
         self.conf.group_locations.clear()
         self._rebuild_group_menu()
 
     def _load_new_group_file(self):
         group_file_path = filedialog.askopenfilename(
             title="Load a new EPLaunch Group File",
             initialdir=self.conf.directory,
-            filetypes=(("EP-Launch Group Files", "*.epg"),)
+            filetypes=(("EP-Launch Group Files", "*.epg3"),)
         )
         if not group_file_path:
             return
         group_file_path_object = Path(group_file_path)
         entries = group_file_path_object.read_text().splitlines()
         self.conf.group_locations = []
         for e in sorted(entries):
@@ -382,32 +422,25 @@
                 self.conf.group_locations.append(Path(e))
         self._rebuild_group_menu()
 
     def _save_group_file(self):
         group_file_path = filedialog.asksaveasfilename(
             title="Save EPLaunch Group File",
             initialdir=self.conf.directory,
-            filetypes=(("EP-Launch Group Files", "*.epg"),)
+            filetypes=(("EP-Launch Group Files", "*.epg3"),)
         )
         if not group_file_path:
             return
         group_file_path_object = Path(group_file_path)
         try:
             group_file_path_object.write_text('\n'.join([str(p) for p in self.conf.group_locations]))
         except Exception as e:  # could be permission or just about anything
             messagebox.showerror("Error", f"Could not save group file, error message:\n{str(e)}")
             return
 
-    def _add_current_dir_to_group(self):
-        if self.conf.directory in self.conf.group_locations:
-            messagebox.showwarning("Warning", "This folder already exists in this group, skipping")
-            return
-        self.conf.group_locations.append(self.conf.directory)
-        self._rebuild_group_menu()
-
     def _add_current_files_to_group(self):
         if len(self.conf.file_selection) == 0:
             messagebox.showwarning("Warning", "No files selected, so none added to current group")
             return
         issue_warning = False
         for f in self.conf.file_selection:
             potential_path = self.conf.directory / f
@@ -415,21 +448,14 @@
                 issue_warning = True
             else:
                 self.conf.group_locations.append(potential_path)
         if issue_warning:
             messagebox.showwarning("Warning", "At least one file path was already in the group and skipped")
         self._rebuild_group_menu()
 
-    def _remove_current_dir_from_group(self):
-        if self.conf.directory not in self.conf.group_locations:
-            messagebox.showwarning("Warning", "This folder isn't in the current group, not doing anything")
-            return
-        self.conf.group_locations.remove(self.conf.directory)
-        self._rebuild_group_menu()
-
     def _remove_current_files_from_group(self):
         issue_warning = False
         for f in self.conf.file_selection:
             potential_path = self.conf.directory / f
             if potential_path in self.conf.group_locations:
                 self.conf.group_locations.remove(potential_path)
             else:
@@ -445,30 +471,29 @@
         self._handle_group_selection(self.group_cycle_next_index)
         self.group_cycle_next_index += 1
         if self.group_cycle_next_index + 1 > len(self.conf.group_locations):
             self.group_cycle_next_index = 0
 
     def _rebuild_group_menu(self):
         self.group_cycle_next_index = 0
-        self.menu_nav_group.delete(0, END)
+        self.menu_group_current.delete(0, END)
         for index, entry in enumerate(self.conf.group_locations):
-            self.menu_nav_group.add_command(
+            self.menu_group_current.add_command(
                 label=str(entry), command=lambda i=index: self._handle_group_selection(i)
             )
 
     def _handle_group_selection(self, index: int):
         entry = self.conf.group_locations[index]
         if not entry.exists():
             messagebox.showerror("Error", f"Could not navigate to group entry, it doesn't exist: {entry}")
             return
-        self.conf.directory = entry if entry.is_dir() else entry.parent
+        self.conf.directory = entry.parent
         self.dir_tree.dir_list.refresh_listing(self.conf.directory)
         self._update_file_list()
-        if entry.is_file():
-            self.file_list.tree.try_to_reselect([entry.name])
+        self.file_list.tree.try_to_reselect([entry.name])
 
     # endregion
 
     # region handling file/folder navigation
 
     def _repopulate_control_list_columns(self):
         """Rebuilds the file list columns based on the current workflow status and column headers"""
@@ -556,15 +581,14 @@
 
     def _new_dir_selected(self, _: bool, selected_path: Path):
         self.previous_selected_directory = self.conf.directory
         self.conf.directory = selected_path
         if len(self.conf.folders_recent) > 0 and self.conf.folders_recent[0] != selected_path:
             self.conf.folders_recent.appendleft(selected_path)
         self._rebuild_recent_folder_menu()
-        self.current_cache = CacheFile(self.conf.directory)
         try:
             self._update_status_bar(f"Selected directory: {self.conf.directory}")
             self._update_file_list()
         except Exception as e:  # noqa -- status_bar and things may not exist during initialization, just ignore
             print(str(e))  # log it to the console for fun
 
     def _new_root_dir(self, new_root_path: Path):
@@ -588,15 +612,16 @@
             previous_selected_files = []
 
         # there should be a cache file there, so get the cached data for the current workflow if it exists
         files_in_current_workflow = {}
         workflow_file_patterns = []
         workflow_columns = []
         if self.workflow_manager.current_workflow:
-            files_in_current_workflow = self.current_cache.get_files_for_workflow(
+            cache = CacheFile(self.conf.directory)
+            files_in_current_workflow = cache.get_files_for_workflow(
                 self.workflow_manager.current_workflow.name
             )
             workflow_file_patterns = self.workflow_manager.current_workflow.file_types
             workflow_columns = self.workflow_manager.current_workflow.columns
 
         # then get the entire list of files in the current directory to build up the listview items
         # if they happen to match the filename in the workflow cache, then add that info to the row structure
@@ -703,15 +728,16 @@
         else:
             self.option_weather_recent['values'] = []
 
     def _set_weather_from_recent(self) -> None:
         current_index = self.option_weather_recent.current()
         selected_recent_weather_string = str(self.conf.weathers_recent[current_index])
         for selected_file_name in self.conf.file_selection:
-            self.current_cache.add_config(
+            cache = CacheFile(self.conf.directory)
+            cache.add_config(
                 self.workflow_manager.current_workflow.name,
                 selected_file_name,
                 {'weather': selected_recent_weather_string}
             )
         self._update_file_list()
 
     def _open_weather_dialog(self) -> None:
@@ -725,15 +751,16 @@
             weather_file_to_use = self.dd_only_string
         else:
             weather_file_to_use = dialog_weather.selected_weather_file
             if weather_file_to_use not in self.conf.weathers_recent:
                 self.conf.weathers_recent.appendleft(weather_file_to_use)
                 self._repopulate_recent_weather_list(weather_file_to_use)
         for selected_file_name in self.conf.file_selection:
-            self.current_cache.add_config(
+            workflow_directory_cache = CacheFile(self.conf.directory)
+            workflow_directory_cache.add_config(
                 self.workflow_manager.current_workflow.name,
                 selected_file_name,
                 {'weather': str(weather_file_to_use)}
             )
         self._update_file_list()
 
     # endregion
@@ -810,31 +837,44 @@
         # clear the output menu entirely, and set status conditionally
         self._repopulate_output_suffix_options()
         # now that the workflow has been set, repopulate the file list columns and the file list itself
         self._repopulate_control_list_columns()
         self._update_file_list()
 
     def _repopulate_output_suffix_options(self):
-        suffixes = sorted(self.workflow_manager.current_workflow.output_suffixes)
-        combobox_output_enabled = 'readonly' if len(suffixes) > 0 else 'disabled'
-        output_enabled = ACTIVE if len(suffixes) > 0 else DISABLED
+        suffixes = self.workflow_manager.current_workflow.output_suffixes
+        sorted_suffixes = sorted(suffixes)
+        combobox_output_enabled = 'readonly' if len(sorted_suffixes) > 0 else 'disabled'
+        output_enabled = ACTIVE if len(sorted_suffixes) > 0 else DISABLED
         self.option_workflow_outputs.configure(state=combobox_output_enabled)
         self.button_open_output_file.configure(state=output_enabled)
 
         # rebuild the option menu if applicable
         current_selection = self._tk_var_output_suffix.get()
         if output_enabled == ACTIVE:
-            self.option_workflow_outputs['values'] = suffixes
-            if current_selection not in suffixes:
-                self._tk_var_output_suffix.set(suffixes[0])
+            self.option_workflow_outputs['values'] = sorted_suffixes
+            if current_selection not in sorted_suffixes:
+                self._tk_var_output_suffix.set(sorted_suffixes[0])
         else:
             self.option_workflow_outputs['values'] = []
             self._tk_var_output_suffix.set('')
         self.option_workflow_outputs.selection_clear()
 
+        # update the output file buttons too
+        self.button_open_output_1.configure(state=ACTIVE if len(suffixes) > 0 else DISABLED)
+        self._tk_var_output_1.set(suffixes[0] if len(suffixes) > 0 else '--')
+        self.button_open_output_2.configure(state=ACTIVE if len(suffixes) > 1 else DISABLED)
+        self._tk_var_output_2.set(suffixes[1] if len(suffixes) > 1 else '--')
+        self.button_open_output_3.configure(state=ACTIVE if len(suffixes) > 2 else DISABLED)
+        self._tk_var_output_3.set(suffixes[2] if len(suffixes) > 2 else '--')
+        self.button_open_output_4.configure(state=ACTIVE if len(suffixes) > 3 else DISABLED)
+        self._tk_var_output_4.set(suffixes[3] if len(suffixes) > 3 else '--')
+        self.button_open_output_5.configure(state=ACTIVE if len(suffixes) > 4 else DISABLED)
+        self._tk_var_output_5.set(suffixes[4] if len(suffixes) > 4 else '--')
+
     def _open_workflow_dir_dialog(self):
         if len(self.workflow_manager.threads) > 0:
             messagebox.showerror("Workflow Selection Error", 'Cannot change workflows while threads are running')
             return  # will leave the window open
         # refresh the list of workflows auto-found on the machine
         self.workflow_manager.auto_find_workflow_directories()
         # pass the newly found folders in, as well as the current active list of workflow directories
@@ -850,85 +890,128 @@
             self.generic_dialogs.display(
                 self, 'Workflow Processing Errors', '\n'.join(self.workflow_manager.warnings)
             )
         self.conf.workflow_directories = self.workflow_manager.workflow_directories
         self._repopulate_workflow_context_menu()
         self._repopulate_workflow_instance_menu()
 
-    def _run_workflow(self) -> None:
-        if self.conf.directory and self.conf.file_selection and self.workflow_manager.current_workflow:
-            pass
-        else:
-            messagebox.showerror(
-                title='Selection Error', message='ERROR: Make sure you select a workflow, directory and a file'
-            )
-            return
-
-        files_in_current_workflow = self.current_cache.get_files_for_workflow(
-            self.workflow_manager.current_workflow.name
-        )
+    def get_or_set_weather_for_file(self,
+                                    cur_workflow: Optional[BaseEPLaunchWorkflow1],
+                                    directory: Path,
+                                    selected_file: str,
+                                    backup_weather_file_to_use: str,
+                                    ) -> Tuple[bool, str, str]:
+        """
+        cur_workflow is "None" at init time, so it is marked technically optional
+        """
         weather_file_to_use: Optional[str] = None
-        if self.workflow_manager.current_workflow.uses_weather:
-            for selected_file_name in self.conf.file_selection:
-                if selected_file_name in files_in_current_workflow:
-                    cached_file_info = files_in_current_workflow[selected_file_name]
-                    if CacheFile.ParametersKey in cached_file_info:
-                        if CacheFile.WeatherFileKey in cached_file_info[CacheFile.ParametersKey]:
-                            weather_file_to_use = cached_file_info[CacheFile.ParametersKey][CacheFile.WeatherFileKey]
-            if not weather_file_to_use:
+        # if we find this file in the current folder cache
+        cache = CacheFile(directory)
+        files_in_current_workflow = cache.get_files_for_workflow(cur_workflow.name)
+        if selected_file in files_in_current_workflow:
+            # and if we find a weather file key for that file, for that workflow, just use the weather file
+            cached_file_info = files_in_current_workflow[selected_file]
+            if CacheFile.ParametersKey in cached_file_info:
+                if CacheFile.WeatherFileKey in cached_file_info[CacheFile.ParametersKey]:
+                    weather_file_to_use = cached_file_info[CacheFile.ParametersKey][CacheFile.WeatherFileKey]
+        # if we didn't find a weather file anywhere, we need to ask
+        if not weather_file_to_use:
+            # since we could be asking for many files, we don't want to ask for each
+            # get a backup file to use only once, and apply that to any missing ones as needed
+            if backup_weather_file_to_use:
+                weather_file_to_use = backup_weather_file_to_use
+            else:
+                # if we need weather, didn't find one in the cache, and didn't have a backup, ask for one now
                 recent_files = list(self.conf.weathers_recent)
                 favorite_files = self.conf.weathers_favorite
-                w = TkWeatherDialog(self, recent_files, favorite_files)
+                w = TkWeatherDialog(
+                    self, recent_files, favorite_files, "*At least one file is missing a weather configuration*"
+                )
                 self.wait_window(w)
                 if w.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
-                    return  # might need to do some other clean up
+                    return False, '', ''
                 else:  # a valid response was encountered
                     if not w.selected_weather_file:
                         weather_file_to_use = self.dd_only_string
                     else:
                         weather_file_to_use = str(w.selected_weather_file)
                         if w.selected_weather_file not in self.conf.weathers_recent:
                             self.conf.weathers_recent.appendleft(w.selected_weather_file)
-            for selected_file_name in self.conf.file_selection:
-                self.current_cache.add_config(
-                    self.workflow_manager.current_workflow.name,
-                    selected_file_name,
-                    {'weather': weather_file_to_use}
-                )
-            self._update_file_list()
+            # save the current selected one as the new backup for subsequent files
+            backup_weather_file_to_use = weather_file_to_use
+        # add the weather configuration to the cache regardless of how it was retrieved, and update file listing
+        cache.add_config(cur_workflow.name, selected_file, {'weather': weather_file_to_use})
+        return True, weather_file_to_use, backup_weather_file_to_use
+
+    def _run_workflow_on_selection(self) -> None:
+        cur_files = self.conf.file_selection
+        file_paths = [self.conf.directory / f for f in cur_files]
+        self._run_workflow_on_list_of_file_paths(file_paths)
+
+    def _run_workflow_on_group(self) -> None:
+        file_paths = self.conf.group_locations
+        self._run_workflow_on_list_of_file_paths(file_paths)
 
-        sel_dir = self.conf.directory
-        cur_wf = self.workflow_manager.current_workflow.name
-        for selected_file_name in self.conf.file_selection:
+    def _run_workflow_on_list_of_file_paths(self, file_paths: List[Path]):
+
+        # error out early
+        if self.conf.directory and self.conf.file_selection and self.workflow_manager.current_workflow:
+            pass
+        else:
+            messagebox.showerror(title='Selection', message='ERROR: Select a workflow, directory and a file')
+            return
+
+        already_running_instances = []
+        cur_workflow = self.workflow_manager.current_workflow
+        w_name = cur_workflow.name
+        backup_weather_file_to_use: Optional[str] = None
+
+        # loop over all the selected files and try to run the current workflow on each of them
+        for path in file_paths:
+            # if the current workflow uses weather, we need to determine what to pass into it
+            weather_file_to_use: Optional[str] = None
+            if cur_workflow.uses_weather:
+                success, weather_file_to_use, backup_weather_file_to_use = self.get_or_set_weather_for_file(
+                    cur_workflow, path.parent, path.name, backup_weather_file_to_use
+                )
+                if not success:
+                    return  # TODO: probably shouldn't just return blindly here
+            this_wea = '' if weather_file_to_use == self.dd_only_string else weather_file_to_use
+
+            # now we actually need to run this current file
+            this_file_good_to_go = True
+            # first check to see if the current file/dir/workflow combination is already running
             for thread_id, t in self.workflow_manager.threads.items():
-                if t.file_name == selected_file_name and t.run_directory == sel_dir and \
-                        t.workflow_instance.name() == cur_wf:
-                    # self.show_error_message('ERROR: This workflow/dir/file combination is already running')
-                    return
+                t_path = Path(t.run_directory) / t.file_name
+                if t_path == path and t.workflow_instance.name() == w_name:
+                    # save it in a list and wait to issue error message until the end
+                    already_running_instances.append(f"{w_name}: {path}")
+                    this_file_good_to_go = False
+                    break
+            # if this file isn't good, just continue the file loop
+            if not this_file_good_to_go:
+                continue
+            # otherwise, continue to instantiate a workflow thread instance to let it run
             new_uuid = str(uuid4())
-            self._update_status_bar('Starting workflow')
-            new_instance = self.workflow_manager.current_workflow.workflow_class()
-            new_instance.register_standard_output_callback(
-                new_uuid,
-                self._callback_workflow_stdout
-            )
-            this_weather = ''
-            if weather_file_to_use != self.dd_only_string:
-                this_weather = weather_file_to_use
+            new_instance = cur_workflow.workflow_class()
+            new_instance.register_standard_output_callback(new_uuid, self._callback_workflow_stdout)
             self.workflow_manager.threads[new_uuid] = WorkflowThread(
-                new_uuid, new_instance, self.conf.directory, selected_file_name,
-                {
-                    'weather': this_weather,
-                    'workflow location': self.workflow_manager.current_workflow.workflow_directory
-                },
+                new_uuid, new_instance, path.parent, path.name,
+                {'weather': this_wea, 'workflow location': cur_workflow.workflow_directory},
                 self._callback_workflow_done
             )
             self.output_dialogs[new_uuid] = self._create_output_dialog(new_uuid)
             self.output_dialogs[new_uuid].add_output("*** STARTING WORKFLOW ***")
 
+        # emit an error dialog if needed
+        if len(already_running_instances) > 0:
+            out = '\n'.join(already_running_instances)
+            messagebox.showerror("Run Error", f"Some configurations were already running, and were skipped: {out}")
+
+        self._update_file_list()  # do one update once all threads are spawned to update for weather selection, etc.
         self._update_status_bar("Currently %s processes running" % len(self.workflow_manager.threads))
 
     def _create_output_dialog(self, workflow_id: str) -> TkOutputDialog:
         """Generates an output dialog with the specified ID, updating dialog counter and setting dialog position"""
         max_dialog_vertical_increments = 5.0
         self.dialog_counter += 1
         if self.dialog_counter == max_dialog_vertical_increments:
@@ -1075,36 +1158,65 @@
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
 EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         """ % VERSION
         self.generic_dialogs.display(self, "About EP-Launch", text)
 
-    def _open_output_file(self):
+    def _open_output_file_generic(self, suffix_to_open: str):
         if len(self.conf.file_selection) > 2:
             message = """More than 2 files were selected when choosing to open workflow outputs.
-This could generate many output windows and is usually not intentional.  Select up to 2 input files."""
+        This could generate many output windows and is usually not intentional.  Select up to 2 input files."""
             messagebox.showerror("File Selection Issue", message)
             return
         for f in self.conf.file_selection:
             original_path = self.conf.directory / f
-            new_path_str = str(original_path.with_suffix('')) + self._tk_var_output_suffix.get()
-            new_path = Path(new_path_str)
-            if not new_path.exists():
+            filename_no_ext = original_path.with_suffix('').name
+            new_path = self.conf.directory / (filename_no_ext + suffix_to_open)
+            new_path_str = str(new_path)
+            eplus_sub_dir = f"EPLaunchRun_{filename_no_ext}"
+            eplus_specific_output_path = self.conf.directory / eplus_sub_dir / f"{filename_no_ext}{suffix_to_open}"
+            eplus_specific_output_file = str(eplus_specific_output_path)
+            if new_path.exists():
+                if suffix_to_open in self.conf.viewer_overrides:
+                    if self.conf.viewer_overrides[suffix_to_open] is not None:
+                        # then the viewer override was found, and not None, so use it
+                        Popen([str(self.conf.viewer_overrides[suffix_to_open]), new_path_str])
+                # if we make it this far, we didn't open it with a custom viewer, try to use the default
+                self._open_file_or_dir_with_default(new_path)
+            elif eplus_specific_output_path.exists():
+                if suffix_to_open in self.conf.viewer_overrides:
+                    if self.conf.viewer_overrides[suffix_to_open] is not None:
+                        # then the viewer override was found, and not None, so use it
+                        Popen([str(self.conf.viewer_overrides[suffix_to_open]), eplus_specific_output_file])
+                # if we make it this far, we didn't open it with a custom viewer, try to use the default
+                self._open_file_or_dir_with_default(eplus_specific_output_path)
+            else:
                 message = """At least some of the output files were not found.
 Make sure that the workflow has run on the selected input file(s), and that the runs
 actually generated the requested outputs.  Any found output files are being opened now."""
                 messagebox.showwarning("Missing Output Files", message)
-            if self._tk_var_output_suffix.get() in self.conf.viewer_overrides:
-                if self.conf.viewer_overrides[self._tk_var_output_suffix.get()] is not None:
-                    # then the viewer override was found, and not None, so use it
-                    Popen([str(self.conf.viewer_overrides[self._tk_var_output_suffix.get()]), new_path_str])
-                    return
-            # if we make it this far, we didn't open it with a custom viewer, try to use the default
-            self._open_file_or_dir_with_default(new_path)
+
+    def _open_output_file(self):
+        self._open_output_file_generic(self._tk_var_output_suffix.get())
+
+    def _open_output_1(self):
+        self._open_output_file_generic(self._tk_var_output_1.get())
+
+    def _open_output_2(self):
+        self._open_output_file_generic(self._tk_var_output_2.get())
+
+    def _open_output_3(self):
+        self._open_output_file_generic(self._tk_var_output_3.get())
+
+    def _open_output_4(self):
+        self._open_output_file_generic(self._tk_var_output_4.get())
+
+    def _open_output_5(self):
+        self._open_output_file_generic(self._tk_var_output_5.get())
 
     @staticmethod
     def _open_file_or_dir_with_default(full_path_obj: Path) -> None:
         full_path = str(full_path_obj)
         if system() == 'Windows':
             from os import startfile
             startfile(full_path)
```

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.5.8/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.5.8/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.5.7/eplaunch/utilities/cache.py` & `energyplus_launch-3.5.8/eplaunch/utilities/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import json
-import os
+from json import dumps, loads
+from os import path
 from pathlib import Path
-import time
-from typing import List
+from time import sleep
+from typing import Dict, List
 
 from eplaunch.utilities.exceptions import EPLaunchFileException
 
 # I'm trying to be good and catch specific exceptions, but the json library makes it difficult like this :-D
 try:
     from json.decoder import JSONDecodeError
 except ImportError:  # pragma: no cover
     JSONDecodeError = ValueError
 
 #: This is used as the mutex queue, the list of unique directories being altered at a given time
 cache_files_currently_updating_or_writing: List[Path] = []
 
 
-class CacheFile(object):
+class CacheFile:
     """
     Represents the file that is kept in each folder where workflows have been started
     Keeps track of the most recent state of the file, with some metadata that is workflow dependent
 
     Usage:
 
     To ensure thread-safety, this class employs a form of a mutex, where the unique id is the current directory
@@ -39,36 +39,36 @@
     FilesKey = 'files'
     ParametersKey = 'config'
     ResultsKey = 'result'
     WeatherFileKey = 'weather'
     QueueCheckInterval = 0.1  # seconds
     QueueTotalCheckTime = 5  # seconds
 
-    def _print(self, message):
+    def _print(self, message) -> None:
         """
         Utility function for printing diagnostic messages -- useful for when debugging synchronous alterations
 
         :param message: The message to print
         :return: None
         """
         debug = False
         if debug:  # pragma: no cover
-            print("%s: %s" % (self.file_path, message))
+            print(f"{self.file_path}: {message}")
 
     def __init__(self, working_directory: Path):
         """
         Constructor for this class, stores the local file path and initializes the workflow_state
 
         :param working_directory:
         """
         self.file_path = working_directory / self.FileName
         self._print("Created cache file")
         self.workflow_state = None
 
-    def _add_file_attribute(self, workflow_name, file_name, attribute, data, replace):
+    def _add_file_attribute(self, workflow_name, file_name, attribute, data, replace) -> None:
         """
         This function generically updates some attribute of a file within a given workflow context
         The hierarchy is:
          workflows
           - workflow_name
            - files
             - file_name
@@ -82,15 +82,15 @@
         :param data: A map of data to write to this attribute
         :param replace: A flag for whether this data should replace all prior data or just append to it
         :return: None
         """
 
         # if there is already a config for this workflow/file, update it
         # if something is missing from the structure, initialize it on each stage
-        self._print("Adding file attribute for workflow: %s, file: %s" % (workflow_name, file_name))
+        self._print(f"Adding file attribute for workflow: {workflow_name}, file: {file_name}")
         root = self.workflow_state[self.RootKey]
         if workflow_name in root:
             this_workflow = root[workflow_name]
             if self.FilesKey in this_workflow:
                 these_files = this_workflow[self.FilesKey]
                 if file_name in these_files:
                     this_file = these_files[file_name]
@@ -107,116 +107,116 @@
                     these_files[file_name] = {attribute: data}
             else:  # pragma: no cover
                 # There's really no way to get here...but I feel like I should leave this in
                 this_workflow[self.FilesKey] = {file_name: {attribute: data}}
         else:
             root[workflow_name] = {self.FilesKey: {file_name: {attribute: data}}}
 
-    def ok_to_continue(self):
+    def ok_to_continue(self) -> bool:
         """
         This function does the check-and-wait part of the mutex.  If the current directory is not blocked, it
         immediately returns.  If the current directory is blocked, it will attempt to check over a certain amount of
         time, at a tight interval, to wait on the mutex to be unlocked.  Ultimately if it can't pass, it returns False.
 
         :return: True or False, whether it is safe to write to this cache
         """
         self._print("Checking if its ok to continue")
         if self.file_path not in cache_files_currently_updating_or_writing:
             return True
         self._print("Found this file in the writing data, trying to sleep through it")
         for i in range(int(self.QueueTotalCheckTime / self.QueueCheckInterval)):
-            time.sleep(self.QueueCheckInterval)
+            sleep(self.QueueCheckInterval)
             if self.file_path not in cache_files_currently_updating_or_writing:
                 self._print("Managed to sleep long enough, continuing!")
                 return True
         else:
             self._print("Sleep didn't last long enough, aborting")
             return False
         # there is an **incredibly** small chance we could have a new file pop in between the check above and later code
         # I will have to noodle on whether we want to worry about that possibility
 
-    def add_config(self, workflow_name, file_name, config_data):
+    def add_config(self, workflow_name, file_name, config_data) -> None:
         """
         This function is used to add a config data block for a workflow.  A config data block contains data that is
         generally thought of as "input data" for a workflow, such as a weather file for a simulation run.
 
         :param workflow_name: The name of the workflow to alter, as given by the workflow's name() method
         :param file_name: The file name of the file to alter
         :param config_data: A map of data to write to this config section
         :return: None
         """
-        self._print("About to add a config attribute for workflow %s; file %s" % (workflow_name, file_name))
+        self._print(f"About to add a config attribute for workflow {workflow_name}; file {file_name}")
         if not self.ok_to_continue():
             pass  # somehow return an error...?
         cache_files_currently_updating_or_writing.append(self.file_path)
         self._print("Cache file locked")
         self.read()
         self._add_file_attribute(workflow_name, file_name, self.ParametersKey, config_data, False)
         self.write()
         cache_files_currently_updating_or_writing.remove(self.file_path)
         self._print("Cache file UN-locked")
 
-    def add_result(self, workflow_name, file_name, column_data):
+    def add_result(self, workflow_name, file_name, column_data) -> None:
         """
         This function is used to add a result data block for a workflow.  A result data block contains data that is
         generally thought of as "output data" for a workflow, such as energy usage for a simulation run.
 
         :param workflow_name: The name of the workflow to alter, as given by the workflow's name() method
         :param file_name: The file name of the file to alter
         :param column_data: A map of data to write to this result section, the keys are expected to be defined by
                             the workflow itself as given by the get_interface_columns() method
         :return: None
         """
-        self._print("About to add a result attribute for workflow %s; file %s" % (workflow_name, file_name))
+        self._print(f"About to add a result attribute for workflow {workflow_name}; file {file_name}")
         if not self.ok_to_continue():
             pass  # somehow return an error...?
         cache_files_currently_updating_or_writing.append(self.file_path)
         self._print("Cache file locked")
         self.read()
         self._add_file_attribute(workflow_name, file_name, self.ResultsKey, column_data, True)
         self.write()
         cache_files_currently_updating_or_writing.remove(self.file_path)
         self._print("Cache file UN-locked")
 
-    def read(self):
+    def read(self) -> None:
         """
         Reads the existing cache file, if it exists, and stores the data in the workflow_state instance variable.
         If the cache file doesn't exist, this simply initializes the workflow_state instance variable.
 
         :return: None
         """
-        if os.path.exists(self.file_path):
+        if path.exists(self.file_path):
             try:
                 with open(self.file_path, 'r') as f:
                     body_text = f.read()
             except IOError:  # pragma: no cover  -- would be difficult to mock up this weird case
                 raise EPLaunchFileException(self.file_path, 'Could not open or read text from file')
             try:
-                self.workflow_state = json.loads(body_text)
+                self.workflow_state = loads(body_text)
             except JSONDecodeError:
                 raise EPLaunchFileException(self.file_path, 'Could not parse cache file JSON text')
         else:
             self.workflow_state = {self.RootKey: {}}
 
-    def write(self):
+    def write(self) -> None:
         """
         Writes out the workflow state to the previously determined cache file location
         Note that this function does not protect for thread-safety!  It is expected that functions who are
         altering the state of the cache should call write() within their own blocking structure
 
         :return: None
         """
-        body_text = json.dumps(self.workflow_state, indent=2)
+        body_text = dumps(self.workflow_state, indent=2)
         try:
             with open(self.file_path, 'w') as f:
                 f.write(body_text)
         except IOError:  # pragma: no cover  -- would be difficult to mock up this weird case
             raise EPLaunchFileException(self.file_path, 'Could not write cache file')
 
-    def get_files_for_workflow(self, current_workflow_name):
+    def get_files_for_workflow(self, current_workflow_name) -> Dict:
         """
         Gets a list of files that are found in this cache inside the given workflow name
 
         :param current_workflow_name: The name of a workflow (as determined by the name() function on the workflow)
         :return: A map with keys that are file names found in this workflow
         """
         self.read()
```

### Comparing `energyplus_launch-3.5.7/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.5.8/eplaunch/utilities/crossplatform.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import platform
+from platform import system
 
 
 class Platform:
     WINDOWS = 1
     LINUX = 2
     MAC = 3
     UNKNOWN = 4
 
     @staticmethod
-    def get_current_platform(test_name=None):
+    def get_current_platform(test_name: str = None) -> int:
         if test_name:
             platform_name = test_name
         else:  # pragma: no cover -- can't know ahead of time which system we will test on
-            platform_name = platform.system()
+            platform_name = system()
         if platform_name == 'Windows':
             return Platform.WINDOWS
         elif platform_name == 'Linux':
             return Platform.LINUX
         elif platform_name == 'Darwin':
             return Platform.MAC
         else:
```

### Comparing `energyplus_launch-3.5.7/eplaunch/utilities/version.py` & `energyplus_launch-3.5.8/eplaunch/utilities/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
 from typing import Tuple
 
-# TODO: this built in eplaunch/utilities/version module should be removed, workflows should manage this themselves
+# TODO: this built-in eplaunch/utilities/version module should be removed, workflows should manage this themselves
 
 
 class Version:
 
     @staticmethod
     def check_energyplus_version(file_path: str) -> Tuple[bool, str, int]:
         """Gets the version number information for a given EnergyPlus input file"""
```

### Comparing `energyplus_launch-3.5.7/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.5.8/eplaunch/workflows/default/file_details.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import os
+from pathlib import Path
+from typing import Dict, List
 
 from eplaunch import NAME, VERSION
 from eplaunch.workflows.base import BaseEPLaunchWorkflow1, EPLaunchWorkflowResponse1
 
 
 class ColumnNames:
     FileType = 'File Type'
     FileSize = 'File Size [kB]'
 
 
 class FileDetailsWorkflow1(BaseEPLaunchWorkflow1):
 
-    def name(self):
+    def name(self) -> str:
         return "Get File Details"
 
-    def context(self):
+    def context(self) -> str:
         return f"{NAME} {VERSION}"
 
-    def description(self):
+    def description(self) -> str:
         return "Retrieves details about the file"
 
-    def get_file_types(self):
+    def get_file_types(self) -> List[str]:
         return ["*"]
 
-    def get_output_suffixes(self):
+    def get_output_suffixes(self) -> List[str]:
         return []
 
-    def get_interface_columns(self):
+    def get_interface_columns(self) -> List[str]:
         return [ColumnNames.FileType, ColumnNames.FileSize]
 
-    def main(self, run_directory, file_name, args):  # pragma: no cover; unit tests can't execute this
+    def main(self, run_directory: Path, file_name: str, args: Dict) -> EPLaunchWorkflowResponse1:  # pragma: no cover
         self.callback(f"In {type(self).__name__}, about to process file: {file_name}")
         file_path = os.path.join(run_directory, file_name)
         info = os.stat(file_path)
         file_type = os.path.splitext(file_path)[1]
         file_size = round(info.st_size / 1024)
         self.callback(f"Completed {type(self).__name__}")
         return EPLaunchWorkflowResponse1(
```

### Comparing `energyplus_launch-3.5.7/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.5.8/eplaunch/workflows/default/idf_details.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import os
+from pathlib import Path
+from typing import Dict, List
 
 from eplaunch import NAME, VERSION
 from eplaunch.workflows.base import BaseEPLaunchWorkflow1, EPLaunchWorkflowResponse1
 
 
 class ColumnNames:
     Version = 'Version'
     NumDesignDays = '# Design Days'
     NumRunPeriods = '# Run Periods'
     NumZones = '# Zones'
 
 
 class IDFDetailsWorkflow1(BaseEPLaunchWorkflow1):
 
-    def name(self):
+    def name(self) -> str:
         return "IDF Details"
 
-    def context(self):
+    def context(self) -> str:
         return f"{NAME} {VERSION}"
 
-    def description(self):
+    def description(self) -> str:
         return "Retrieves IDF Details"
 
-    def get_file_types(self):
+    def get_file_types(self) -> List[str]:
         return ["*.idf"]
 
-    def get_output_suffixes(self):
+    def get_output_suffixes(self) -> List[str]:
         return []
 
-    def get_interface_columns(self):
+    def get_interface_columns(self) -> List[str]:
         return [
             ColumnNames.Version,
             ColumnNames.NumDesignDays,
             ColumnNames.NumRunPeriods,
             ColumnNames.NumZones
         ]
 
-    def main(self, run_directory, file_name, args):  # pragma: no cover; unit tests can't execute this
+    def main(self, run_directory: Path, file_name: str, args: Dict) -> EPLaunchWorkflowResponse1:  # pragma: no cover
         self.callback(f"In {type(self).__name__}, about to process file: {file_name}")
         file_path = os.path.join(run_directory, file_name)
         content = open(file_path).read()
         new_lines = []
         try:
             for line in content.split('\n'):
                 if line.strip() == '':
```

### Comparing `energyplus_launch-3.5.7/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.5.8/eplaunch/workflows/default/site_location.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import os
+from pathlib import Path
+from typing import Dict, List
 
 from eplaunch import NAME, VERSION
 from eplaunch.workflows.base import BaseEPLaunchWorkflow1, EPLaunchWorkflowResponse1
 
 
 class ColumnNames:
     Location = 'Site:Location []'
 
 
 class SiteLocationWorkflow(BaseEPLaunchWorkflow1):
 
-    def name(self):
+    def name(self) -> str:
         return "Get Site:Location"
 
-    def context(self):
+    def context(self) -> str:
         return f"{NAME} {VERSION}"
 
-    def description(self):
+    def description(self) -> str:
         return "Retrieves the Site:Location name"
 
-    def get_file_types(self):
+    def get_file_types(self) -> List[str]:
         return ["*.idf"]
 
-    def get_output_suffixes(self):
+    def get_output_suffixes(self) -> List[str]:
         return []
 
-    def get_interface_columns(self):
+    def get_interface_columns(self) -> List[str]:
         return [ColumnNames.Location]
 
-    def main(self, run_directory, file_name, args):  # pragma: no cover; unit tests can't execute this
+    def main(self, run_directory: Path, file_name: str, args: Dict) -> EPLaunchWorkflowResponse1:  # pragma: no cover
         self.callback(f"In {type(self).__name__}, about to process file: {file_name}")
-        file_path = os.path.join(run_directory, file_name)
-        content = open(file_path).read()
+        content = (run_directory / file_name).read_text()
         new_lines = []
         for line in content.split('\n'):
             if line.strip() == '':
                 continue
             if '!' not in line:
                 new_lines.append(line.strip())
             else:
```

### Comparing `energyplus_launch-3.5.7/eplaunch/workflows/manager.py` & `energyplus_launch-3.5.8/eplaunch/workflows/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from string import ascii_uppercase
-from typing import Dict, List, Optional, Set
+from typing import Dict, List, Optional, Set, Tuple, Type
 from importlib import util as import_util
 from inspect import getmembers, isclass
 
 from eplaunch.utilities.crossplatform import Platform
+from eplaunch.workflows.base import BaseEPLaunchWorkflow1
 from eplaunch.workflows.workflow import Workflow
 from eplaunch.workflows.workflow_thread import WorkflowThread
 
 
 class WorkflowManager:
     def __init__(self):
         self.current_workflow: Optional[Workflow] = None
@@ -98,29 +99,29 @@
                     continue
                 except Exception as e:  # pragma: no cover
                     # there's always the potential of some other unforeseen thing going on when a workflow is executed
                     self.warnings.append(f"Unexpected error importing workflow: {str(this_file_path)}: {str(e)}")
                     continue
 
             for module_file_path, this_module in modules:
-                class_members = getmembers(this_module, isclass)
+                class_members: List[Tuple[str, Type[BaseEPLaunchWorkflow1]]] = getmembers(this_module, isclass)
                 for this_class in class_members:
                     this_class_name, this_class_type = this_class
                     # so right here, we could check issubclass, but this also matches the BaseEPLaunchWorkflow1, which
                     # is imported in each workflow class.  No need to do that.  For now, I'm going to check the direct
                     # parent class of this class to verify we only get direct descendants.  We can evaluate this later.
                     # if issubclass(this_class_type, BaseEPLaunchWorkflow1):
                     num_inheritance = len(this_class_type.__bases__)
                     base_class_name = this_class_type.__bases__[0].__name__
                     workflow_base_class_name = 'BaseEPLaunchWorkflow1'
                     if num_inheritance == 1 and workflow_base_class_name in base_class_name:
                         try:
                             # we've got a good match, grab more data and get ready to load this into the Detail class
-                            workflow_instance = this_class_type()
-                            workflow_name = workflow_instance.name()
+                            workflow_instance: BaseEPLaunchWorkflow1 = this_class_type()
+                            workflow_name: str = workflow_instance.name()
                             workflow_file_types = workflow_instance.get_file_types()
                             workflow_output_suffixes = workflow_instance.get_output_suffixes()
                             workflow_columns = workflow_instance.get_interface_columns()
                             workflow_context = workflow_instance.context()
                             workflow_weather = workflow_instance.uses_weather()
 
                             file_type_string = "("
```

### Comparing `energyplus_launch-3.5.7/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.5.8/eplaunch/workflows/workflow_thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from pathlib import Path
-import threading
+from threading import Thread
+from typing import Dict, Callable
 
 from eplaunch.workflows.base import EPLaunchWorkflowResponse1
 
 
-class WorkflowThread(threading.Thread):
+class WorkflowThread(Thread):
     """Worker Thread Class."""
 
     def __init__(self, identifier: str, workflow_instance,
-                 run_directory: Path, file_name, main_args, done_callback):
+                 run_directory: Path, file_name: str, main_args: Dict, done_callback: Callable):
         super().__init__()
         self._want_abort = 0
         self.id = identifier
         self.workflow_instance = workflow_instance
         self.workflow_directory = main_args['workflow location']
         self.run_directory = run_directory
         self.file_name = file_name
```

### Comparing `energyplus_launch-3.5.7/setup.py` & `energyplus_launch-3.5.8/setup.py`

 * *Files identical despite different names*

