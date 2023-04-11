# Comparing `tmp/napari-sam-0.2.3.tar.gz` & `tmp/napari-sam-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.2.3.tar", last modified: Mon Apr 10 10:23:44 2023, max compression
+gzip compressed data, was "napari-sam-0.2.5.tar", last modified: Tue Apr 11 10:19:13 2023, max compression
```

## Comparing `napari-sam-0.2.3.tar` & `napari-sam-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:23:44.384685 napari-sam-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 10:23:18.000000 napari-sam-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 10:23:18.000000 napari-sam-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-10 10:23:44.384685 napari-sam-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-10 10:23:18.000000 napari-sam-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-10 10:23:18.000000 napari-sam-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-10 10:23:44.384685 napari-sam-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:23:44.384685 napari-sam-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:23:44.384685 napari-sam-0.2.3/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 10:23:18.000000 napari-sam-0.2.3/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-04-10 10:23:18.000000 napari-sam-0.2.3/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 10:23:18.000000 napari-sam-0.2.3/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-10 10:23:18.000000 napari-sam-0.2.3/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:23:44.384685 napari-sam-0.2.3/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-10 10:23:44.000000 napari-sam-0.2.3/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-10 10:23:44.000000 napari-sam-0.2.3/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:23:44.000000 napari-sam-0.2.3/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 10:23:44.000000 napari-sam-0.2.3/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 10:23:44.000000 napari-sam-0.2.3/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 10:23:44.000000 napari-sam-0.2.3/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:19:13.200338 napari-sam-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 10:18:54.000000 napari-sam-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 10:18:54.000000 napari-sam-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-04-11 10:19:13.200338 napari-sam-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-11 10:18:54.000000 napari-sam-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-11 10:18:54.000000 napari-sam-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-11 10:19:13.200338 napari-sam-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:19:13.196338 napari-sam-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:19:13.196338 napari-sam-0.2.5/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 10:18:54.000000 napari-sam-0.2.5/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29400 2023-04-11 10:18:54.000000 napari-sam-0.2.5/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-11 10:18:54.000000 napari-sam-0.2.5/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-11 10:18:54.000000 napari-sam-0.2.5/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:19:13.200338 napari-sam-0.2.5/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-04-11 10:19:13.000000 napari-sam-0.2.5/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 10:19:13.000000 napari-sam-0.2.5/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:19:13.000000 napari-sam-0.2.5/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-11 10:19:13.000000 napari-sam-0.2.5/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 10:19:13.000000 napari-sam-0.2.5/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 10:19:13.000000 napari-sam-0.2.5/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.2.3/LICENSE` & `napari-sam-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.2.3/PKG-INFO` & `napari-sam-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.2.3
+Version: 0.2.5
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -34,17 +34,17 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-sam.svg?color=green)](https://python.org)
 [![tests](https://github.com/MIC-DKFZ/napari-sam/workflows/tests/badge.svg)](https://github.com/MIC-DKFZ/napari-sam/actions)
 [![codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)](https://napari-hub.org/plugins/napari-sam)
 
 Segment anything with our **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**!
 
-SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object** and now our plugin neatly integrates this into Napari.
+SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object**, and now, our plugin neatly integrates this into Napari.
 
-We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation**!
+We have already **extended** SAM's click-based foreground separation to full **click-based semantic segmentation and instance segmentation**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
 
@@ -60,25 +60,39 @@
 
 ----------------------------------
 
 ## Installation
 
 The plugin requires `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow the instructions here to install both PyTorch and TorchVision dependencies. Installing both PyTorch and TorchVision with CUDA support is strongly recommended.
 
+Install Napari via [pip]:
+    
+    pip install napari[all]
+
 You can install `napari-sam` via [pip]:
 
     pip install git+https://github.com/facebookresearch/segment-anything.git
     pip install napari-sam
 
 
 
 To install latest development version :
 
     pip install git+https://github.com/MIC-DKFZ/napari-sam.git
 
+## Usage
+
+Start Napari from the console with:
+
+    napari
+
+Then navigate to `Plugins -> Segment Anything (napari-sam)` and drag & drop an image into Napari. At last create, a labels layer that will be used for the SAM predictions, by clicking in the layer list on the third button.
+
+You can then auto-download one of the available SAM models (this can take 1-2 minutes),  activate one of the annotations & segmentation modes, and you are ready to go!
+
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.2.3 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.2.5 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -23,40 +23,47 @@
 workflows/tests/badge.svg)](https://github.com/MIC-DKFZ/napari-sam/actions) [!
 [codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/
 badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub](https://
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)]
 (https://napari-hub.org/plugins/napari-sam) Segment anything with our
 **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**! SAM
 is the new segmentation system from Meta AI capable of **one-click segmentation
-of any object** and now our plugin neatly integrates this into Napari. We
-already **extended** SAMs click-based foreground separation to full **click-
-based semantic segmentation & instance segmentation**! ------------------------
----------- Everything mode | Click-based semantic segmentation mode | Click-
-based instance segmentation mode :-------------------------:|:-----------------
---------:|:-------------------------: ![](cats_everything.png) | ![]
+of any object**, and now, our plugin neatly integrates this into Napari. We
+have already **extended** SAM's click-based foreground separation to full
+**click-based semantic segmentation and instance segmentation**! --------------
+-------------------- Everything mode | Click-based semantic segmentation mode |
+Click-based instance segmentation mode :-------------------------:|:-----------
+--------------:|:-------------------------: ![](cats_everything.png) | ![]
 (cats_semantic.png) | ![](cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
-recommended. You can install `napari-sam` via [pip]: pip install git+https://
-github.com/facebookresearch/segment-anything.git pip install napari-sam To
-install latest development version : pip install git+https://github.com/MIC-
-DKFZ/napari-sam.git ## Contributing Contributions are very welcome. Tests can
-be run with [tox], please ensure the coverage at least stays the same before
-you submit a pull request. ## License Distributed under the terms of the
-[Apache Software License 2.0] license, "napari-sam" is free and open source
-software ## Issues If you encounter any problems, please [file an issue] along
-with a detailed description. [napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter [@napari]: https://
-github.com/napari [MIT]: http://opensource.org/licenses/MIT [BSD-3]: http://
-opensource.org/licenses/BSD-3-Clause [GNU GPL v3.0]: http://www.gnu.org/
-licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-
-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-sam/issues [napari]:
-https://github.com/napari/napari [tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/ [PyPI]: https://pypi.org/
+recommended. Install Napari via [pip]: pip install napari[all] You can install
+`napari-sam` via [pip]: pip install git+https://github.com/facebookresearch/
+segment-anything.git pip install napari-sam To install latest development
+version : pip install git+https://github.com/MIC-DKFZ/napari-sam.git ## Usage
+Start Napari from the console with: napari Then navigate to `Plugins -> Segment
+Anything (napari-sam)` and drag & drop an image into Napari. At last create, a
+labels layer that will be used for the SAM predictions, by clicking in the
+layer list on the third button. You can then auto-download one of the available
+SAM models (this can take 1-2 minutes), activate one of the annotations &
+segmentation modes, and you are ready to go! ## Contributing Contributions are
+very welcome. Tests can be run with [tox], please ensure the coverage at least
+stays the same before you submit a pull request. ## License Distributed under
+the terms of the [Apache Software License 2.0] license, "napari-sam" is free
+and open source software ## Issues If you encounter any problems, please [file
+an issue] along with a detailed description. [napari]: https://github.com/
+napari/napari [Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari [MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause [GNU GPL v3.0]: http://
+www.gnu.org/licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/
+lgpl-3.0.txt [Apache Software License 2.0]: http://www.apache.org/licenses/
+LICENSE-2.0 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/
+2.0/index.txt [cookiecutter-napari-plugin]: https://github.com/napari/
+cookiecutter-napari-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-
+sam/issues [napari]: https://github.com/napari/napari [tox]: https://
+tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
+https://pypi.org/
```

### Comparing `napari-sam-0.2.3/README.md` & `napari-sam-0.2.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-sam.svg?color=green)](https://python.org)
 [![tests](https://github.com/MIC-DKFZ/napari-sam/workflows/tests/badge.svg)](https://github.com/MIC-DKFZ/napari-sam/actions)
 [![codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)](https://napari-hub.org/plugins/napari-sam)
 
 Segment anything with our **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**!
 
-SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object** and now our plugin neatly integrates this into Napari.
+SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object**, and now, our plugin neatly integrates this into Napari.
 
-We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation**!
+We have already **extended** SAM's click-based foreground separation to full **click-based semantic segmentation and instance segmentation**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
 
@@ -31,25 +31,39 @@
 
 ----------------------------------
 
 ## Installation
 
 The plugin requires `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow the instructions here to install both PyTorch and TorchVision dependencies. Installing both PyTorch and TorchVision with CUDA support is strongly recommended.
 
+Install Napari via [pip]:
+    
+    pip install napari[all]
+
 You can install `napari-sam` via [pip]:
 
     pip install git+https://github.com/facebookresearch/segment-anything.git
     pip install napari-sam
 
 
 
 To install latest development version :
 
     pip install git+https://github.com/MIC-DKFZ/napari-sam.git
 
+## Usage
+
+Start Napari from the console with:
+
+    napari
+
+Then navigate to `Plugins -> Segment Anything (napari-sam)` and drag & drop an image into Napari. At last create, a labels layer that will be used for the SAM predictions, by clicking in the layer list on the third button.
+
+You can then auto-download one of the available SAM models (this can take 1-2 minutes),  activate one of the annotations & segmentation modes, and you are ready to go!
+
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

#### html2text {}

```diff
@@ -7,40 +7,47 @@
 DKFZ/napari-sam/workflows/tests/badge.svg)](https://github.com/MIC-DKFZ/napari-
 sam/actions) [![codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/
 graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub]
 (https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-
 sam)](https://napari-hub.org/plugins/napari-sam) Segment anything with our
 **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**! SAM
 is the new segmentation system from Meta AI capable of **one-click segmentation
-of any object** and now our plugin neatly integrates this into Napari. We
-already **extended** SAMs click-based foreground separation to full **click-
-based semantic segmentation & instance segmentation**! ------------------------
----------- Everything mode | Click-based semantic segmentation mode | Click-
-based instance segmentation mode :-------------------------:|:-----------------
---------:|:-------------------------: ![](cats_everything.png) | ![]
+of any object**, and now, our plugin neatly integrates this into Napari. We
+have already **extended** SAM's click-based foreground separation to full
+**click-based semantic segmentation and instance segmentation**! --------------
+-------------------- Everything mode | Click-based semantic segmentation mode |
+Click-based instance segmentation mode :-------------------------:|:-----------
+--------------:|:-------------------------: ![](cats_everything.png) | ![]
 (cats_semantic.png) | ![](cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
-recommended. You can install `napari-sam` via [pip]: pip install git+https://
-github.com/facebookresearch/segment-anything.git pip install napari-sam To
-install latest development version : pip install git+https://github.com/MIC-
-DKFZ/napari-sam.git ## Contributing Contributions are very welcome. Tests can
-be run with [tox], please ensure the coverage at least stays the same before
-you submit a pull request. ## License Distributed under the terms of the
-[Apache Software License 2.0] license, "napari-sam" is free and open source
-software ## Issues If you encounter any problems, please [file an issue] along
-with a detailed description. [napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter [@napari]: https://
-github.com/napari [MIT]: http://opensource.org/licenses/MIT [BSD-3]: http://
-opensource.org/licenses/BSD-3-Clause [GNU GPL v3.0]: http://www.gnu.org/
-licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-
-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-sam/issues [napari]:
-https://github.com/napari/napari [tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/ [PyPI]: https://pypi.org/
+recommended. Install Napari via [pip]: pip install napari[all] You can install
+`napari-sam` via [pip]: pip install git+https://github.com/facebookresearch/
+segment-anything.git pip install napari-sam To install latest development
+version : pip install git+https://github.com/MIC-DKFZ/napari-sam.git ## Usage
+Start Napari from the console with: napari Then navigate to `Plugins -> Segment
+Anything (napari-sam)` and drag & drop an image into Napari. At last create, a
+labels layer that will be used for the SAM predictions, by clicking in the
+layer list on the third button. You can then auto-download one of the available
+SAM models (this can take 1-2 minutes), activate one of the annotations &
+segmentation modes, and you are ready to go! ## Contributing Contributions are
+very welcome. Tests can be run with [tox], please ensure the coverage at least
+stays the same before you submit a pull request. ## License Distributed under
+the terms of the [Apache Software License 2.0] license, "napari-sam" is free
+and open source software ## Issues If you encounter any problems, please [file
+an issue] along with a detailed description. [napari]: https://github.com/
+napari/napari [Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari [MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause [GNU GPL v3.0]: http://
+www.gnu.org/licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/
+lgpl-3.0.txt [Apache Software License 2.0]: http://www.apache.org/licenses/
+LICENSE-2.0 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/
+2.0/index.txt [cookiecutter-napari-plugin]: https://github.com/napari/
+cookiecutter-napari-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-
+sam/issues [napari]: https://github.com/napari/napari [tox]: https://
+tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
+https://pypi.org/
```

### Comparing `napari-sam-0.2.3/setup.cfg` & `napari-sam-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.2.3/src/napari_sam/_widget.py` & `napari-sam-0.2.5/src/napari_sam/_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,24 +69,26 @@
 
         self.g_annotation = QGroupBox("Annotation mode")
         self.l_annotation = QVBoxLayout()
 
         self.rb_click = QRadioButton("Click")
         self.rb_click.setChecked(True)
         self.l_annotation.addWidget(self.rb_click)
+        self.rb_click.clicked.connect(self.on_everything_mode_checked)
 
         self.rb_bbox = QRadioButton("Bounding Box (WIP)")
         self.rb_bbox.setEnabled(False)
         self.rb_bbox.setStyleSheet("color: gray")
         self.l_annotation.addWidget(self.rb_bbox)
 
         self.rb_auto = QRadioButton("Everything")
         # self.rb_auto.setEnabled(False)
         # self.rb_auto.setStyleSheet("color: gray")
         self.l_annotation.addWidget(self.rb_auto)
+        self.rb_auto.clicked.connect(self.on_everything_mode_checked)
 
         self.g_annotation.setLayout(self.l_annotation)
         self.layout().addWidget(self.g_annotation)
 
         self.g_segmentation = QGroupBox("Segmentation mode")
         self.l_segmentation = QVBoxLayout()
 
@@ -106,27 +108,61 @@
 
         self.btn_activate = QPushButton("Activate")
         self.btn_activate.clicked.connect(self._activate)
         self.btn_activate.setEnabled(False)
         self.is_active = False
         self.layout().addWidget(self.btn_activate)
 
-        self.l_info = QLabel("Info: \n \n"
-                             "Positive Click: Middle Mouse Button\n \n"
-                             "Negative Click: Control + Middle Mouse Button \n \n"
-                             "Undo: Control + Z \n \n"
-                             "Select Point: Left Click \n \n"
-                             "Delete Selected Point: Delete")
-        # self.l_info_positive = QLabel("Middle Mouse Button: Positive Click")
-        # self.l_info_negative = QLabel("Control + Middle Mouse Button: Negative Click")
-        # self.l_info_undo = QLabel("Undo: Control + Z")
-        self.layout().addWidget(self.l_info)
-        # self.layout().addWidget(self.l_info_positive)
-        # self.layout().addWidget(self.l_info_negative)
-        # self.layout().addWidget(self.l_info_undo)
+        self.g_info_click = QGroupBox("Click Mode")
+        self.l_info_click = QVBoxLayout()
+
+        self.label_info_click = QLabel("Positive Click: Middle Mouse Button\n \n"
+                                 "Negative Click: Control + Middle Mouse Button \n \n"
+                                 "Undo: Control + Z \n \n"
+                                 "Select Point: Left Click \n \n"
+                                 "Delete Selected Point: Delete")
+        self.l_info_click.addWidget(self.label_info_click)
+        self.g_info_click.setLayout(self.l_info_click)
+        self.layout().addWidget(self.g_info_click)
+
+        self.g_info_everything = QGroupBox("Everything Mode")
+        self.l_info_everything = QVBoxLayout()
+
+        self.label_info_everything = QLabel("Creates automatically an instance segmentation \n"
+                                            "of the entire image.\n"
+                                            "No user interaction possible.")
+        self.l_info_everything.addWidget(self.label_info_everything)
+        self.g_info_everything.setLayout(self.l_info_everything)
+        self.layout().addWidget(self.g_info_everything)
+
+        self.g_info_semantic = QGroupBox("Semantic Mode")
+        self.l_info_semantic = QVBoxLayout()
+
+        self.label_info_semantic = QLabel("Enables the user to create a \n"
+                                 "multi-label (semantic) segmentation of different classes.\n \n"
+                                 "All objects from the same class \n"
+                                 "should be given the same label by the user.\n \n"
+                                 "The current label can be changed by the user \n"
+                                 "on the labels layer pane after selecting the labels layer.")
+        self.l_info_semantic.addWidget(self.label_info_semantic)
+        self.g_info_semantic.setLayout(self.l_info_semantic)
+        self.layout().addWidget(self.g_info_semantic)
+
+        self.g_info_instance = QGroupBox("Instance Mode")
+        self.l_info_instance = QVBoxLayout()
+
+        self.label_info_instance = QLabel("Enables the user to create an \n"
+                                 "instance segmentation of different objects.\n \n"
+                                 "Objects can be from the same or different classes,\n"
+                                 "but each object should be given a unique label by the user. \n \n"
+                                 "The current label can be changed by the user \n"
+                                 "on the labels layer pane after selecting the labels layer.")
+        self.l_info_instance.addWidget(self.label_info_instance)
+        self.g_info_instance.setLayout(self.l_info_instance)
+        self.layout().addWidget(self.g_info_instance)
 
         self.image_name = None
         self.image_layer = None
         self.label_layer = None
         self.label_layer_changes = None
         self.label_color_mapping = None
         self.points_layer = None
@@ -140,14 +176,24 @@
         self.sam_logits = None
 
         self.points = defaultdict(list)
         self.point_label = None
 
         self.viewer.window.qt_viewer.layers.model().filterAcceptsRow = self._myfilter
 
+    def on_everything_mode_checked(self):
+        if self.rb_auto.isChecked():
+            self.rb_semantic.setEnabled(False)
+            self.rb_semantic.setChecked(False)
+            self.rb_semantic.setStyleSheet("color: gray")
+            self.rb_instance.setChecked(True)
+        else:
+            self.rb_semantic.setEnabled(True)
+            self.rb_semantic.setStyleSheet("")
+
     def init_model_type_combobox(self):
         model_types = list(sam_model_registry.keys())
         cached_weight_types = get_cached_weight_types(model_types)
         entries = []
         for name, is_cached in cached_weight_types.items():
             if is_cached:
                 entries.append("{} (Cached)".format(name))
@@ -343,20 +389,20 @@
         self.points_layer = None
         self.annotator_mode = AnnotatorMode.NONE
         self.points = defaultdict(list)
         self.point_label = None
         self.sam_logits = None
         self.rb_click.setEnabled(True)
         self.rb_auto.setEnabled(True)
-        self.rb_click.setStyleSheet("color: black")
-        self.rb_auto.setStyleSheet("color: black")
+        self.rb_click.setStyleSheet("")
+        self.rb_auto.setStyleSheet("")
         self.rb_semantic.setEnabled(True)
         self.rb_instance.setEnabled(True)
-        self.rb_semantic.setStyleSheet("color: black")
-        self.rb_instance.setStyleSheet("color: black")
+        self.rb_semantic.setStyleSheet("")
+        self.rb_instance.setStyleSheet("")
         self._reset_history()
 
     def create_label_color_mapping(self, num_labels=1000):
         if self.label_layer is not None:
             self.label_color_mapping = {"label_mapping": {}, "color_mapping": {}}
             for label in range(num_labels):
                 color = self.label_layer.get_color(label)
```

### Comparing `napari-sam-0.2.3/src/napari_sam/utils.py` & `napari-sam-0.2.5/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.2.3/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.2.5/src/napari_sam.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.2.3
+Version: 0.2.5
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -34,17 +34,17 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-sam.svg?color=green)](https://python.org)
 [![tests](https://github.com/MIC-DKFZ/napari-sam/workflows/tests/badge.svg)](https://github.com/MIC-DKFZ/napari-sam/actions)
 [![codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)](https://napari-hub.org/plugins/napari-sam)
 
 Segment anything with our **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**!
 
-SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object** and now our plugin neatly integrates this into Napari.
+SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object**, and now, our plugin neatly integrates this into Napari.
 
-We already **extended** SAMs click-based foreground separation to full **click-based semantic segmentation & instance segmentation**!
+We have already **extended** SAM's click-based foreground separation to full **click-based semantic segmentation and instance segmentation**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
 
@@ -60,25 +60,39 @@
 
 ----------------------------------
 
 ## Installation
 
 The plugin requires `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow the instructions here to install both PyTorch and TorchVision dependencies. Installing both PyTorch and TorchVision with CUDA support is strongly recommended.
 
+Install Napari via [pip]:
+    
+    pip install napari[all]
+
 You can install `napari-sam` via [pip]:
 
     pip install git+https://github.com/facebookresearch/segment-anything.git
     pip install napari-sam
 
 
 
 To install latest development version :
 
     pip install git+https://github.com/MIC-DKFZ/napari-sam.git
 
+## Usage
+
+Start Napari from the console with:
+
+    napari
+
+Then navigate to `Plugins -> Segment Anything (napari-sam)` and drag & drop an image into Napari. At last create, a labels layer that will be used for the SAM predictions, by clicking in the layer list on the third button.
+
+You can then auto-download one of the available SAM models (this can take 1-2 minutes),  activate one of the annotations & segmentation modes, and you are ready to go!
+
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.2.3 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.2.5 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -23,40 +23,47 @@
 workflows/tests/badge.svg)](https://github.com/MIC-DKFZ/napari-sam/actions) [!
 [codecov](https://codecov.io/gh/MIC-DKFZ/napari-sam/branch/main/graph/
 badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub](https://
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)]
 (https://napari-hub.org/plugins/napari-sam) Segment anything with our
 **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**! SAM
 is the new segmentation system from Meta AI capable of **one-click segmentation
-of any object** and now our plugin neatly integrates this into Napari. We
-already **extended** SAMs click-based foreground separation to full **click-
-based semantic segmentation & instance segmentation**! ------------------------
----------- Everything mode | Click-based semantic segmentation mode | Click-
-based instance segmentation mode :-------------------------:|:-----------------
---------:|:-------------------------: ![](cats_everything.png) | ![]
+of any object**, and now, our plugin neatly integrates this into Napari. We
+have already **extended** SAM's click-based foreground separation to full
+**click-based semantic segmentation and instance segmentation**! --------------
+-------------------- Everything mode | Click-based semantic segmentation mode |
+Click-based instance segmentation mode :-------------------------:|:-----------
+--------------:|:-------------------------: ![](cats_everything.png) | ![]
 (cats_semantic.png) | ![](cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
-recommended. You can install `napari-sam` via [pip]: pip install git+https://
-github.com/facebookresearch/segment-anything.git pip install napari-sam To
-install latest development version : pip install git+https://github.com/MIC-
-DKFZ/napari-sam.git ## Contributing Contributions are very welcome. Tests can
-be run with [tox], please ensure the coverage at least stays the same before
-you submit a pull request. ## License Distributed under the terms of the
-[Apache Software License 2.0] license, "napari-sam" is free and open source
-software ## Issues If you encounter any problems, please [file an issue] along
-with a detailed description. [napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter [@napari]: https://
-github.com/napari [MIT]: http://opensource.org/licenses/MIT [BSD-3]: http://
-opensource.org/licenses/BSD-3-Clause [GNU GPL v3.0]: http://www.gnu.org/
-licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-
-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-sam/issues [napari]:
-https://github.com/napari/napari [tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/ [PyPI]: https://pypi.org/
+recommended. Install Napari via [pip]: pip install napari[all] You can install
+`napari-sam` via [pip]: pip install git+https://github.com/facebookresearch/
+segment-anything.git pip install napari-sam To install latest development
+version : pip install git+https://github.com/MIC-DKFZ/napari-sam.git ## Usage
+Start Napari from the console with: napari Then navigate to `Plugins -> Segment
+Anything (napari-sam)` and drag & drop an image into Napari. At last create, a
+labels layer that will be used for the SAM predictions, by clicking in the
+layer list on the third button. You can then auto-download one of the available
+SAM models (this can take 1-2 minutes), activate one of the annotations &
+segmentation modes, and you are ready to go! ## Contributing Contributions are
+very welcome. Tests can be run with [tox], please ensure the coverage at least
+stays the same before you submit a pull request. ## License Distributed under
+the terms of the [Apache Software License 2.0] license, "napari-sam" is free
+and open source software ## Issues If you encounter any problems, please [file
+an issue] along with a detailed description. [napari]: https://github.com/
+napari/napari [Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari [MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause [GNU GPL v3.0]: http://
+www.gnu.org/licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/
+lgpl-3.0.txt [Apache Software License 2.0]: http://www.apache.org/licenses/
+LICENSE-2.0 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/
+2.0/index.txt [cookiecutter-napari-plugin]: https://github.com/napari/
+cookiecutter-napari-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-
+sam/issues [napari]: https://github.com/napari/napari [tox]: https://
+tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
+https://pypi.org/
```

