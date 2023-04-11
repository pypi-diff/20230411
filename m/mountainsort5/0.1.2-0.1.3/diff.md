# Comparing `tmp/mountainsort5-0.1.2.tar.gz` & `tmp/mountainsort5-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountainsort5-0.1.2.tar", last modified: Wed Mar 29 00:03:58 2023, max compression
+gzip compressed data, was "mountainsort5-0.1.3.tar", last modified: Tue Apr 11 19:16:36 2023, max compression
```

## Comparing `mountainsort5-0.1.2.tar` & `mountainsort5-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:58.916819 mountainsort5-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-29 00:03:58.916819 mountainsort5-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:58.908819 mountainsort5-0.1.2/mountainsort5/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:58.912819 mountainsort5-0.1.2/mountainsort5/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/SnippetClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/cluster_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/compute_pca_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/compute_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/detect_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/extract_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/get_block_recording_for_scheme3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/get_sampled_recording_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/get_times_labels_from_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/core/pairwise_merge_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:58.916819 mountainsort5-0.1.2/mountainsort5/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/schemes/Scheme1SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/schemes/Scheme2SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/schemes/Scheme3SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/schemes/sorting_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/schemes/sorting_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/mountainsort5/schemes/sorting_scheme3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:58.912819 mountainsort5-0.1.2/mountainsort5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-29 00:03:58.000000 mountainsort5-0.1.2/mountainsort5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-29 00:03:58.000000 mountainsort5-0.1.2/mountainsort5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 00:03:58.000000 mountainsort5-0.1.2/mountainsort5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 00:03:58.000000 mountainsort5-0.1.2/mountainsort5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 00:03:58.000000 mountainsort5-0.1.2/mountainsort5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 00:03:58.916819 mountainsort5-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 00:03:58.916819 mountainsort5-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/tests/test_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/tests/test_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-29 00:03:02.000000 mountainsort5-0.1.2/tests/test_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.012350 mountainsort5-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/SnippetClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/cluster_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/compute_pca_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/compute_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/detect_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/extract_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/get_block_recording_for_scheme3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/get_sampled_recording_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/get_times_labels_from_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/core/pairwise_merge_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/Scheme1SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/Scheme2SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/Scheme3SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/mountainsort5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-11 19:16:35.000000 mountainsort5-0.1.3/mountainsort5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 19:16:36.000000 mountainsort5-0.1.3/mountainsort5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:16:36.012350 mountainsort5-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:16:36.008350 mountainsort5-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-11 19:15:36.000000 mountainsort5-0.1.3/tests/test_scheme3.py
```

### Comparing `mountainsort5-0.1.2/LICENSE` & `mountainsort5-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/PKG-INFO` & `mountainsort5-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.1.2
+Version: 0.1.3
 Summary: MountainSort 5 spike sorting algorithm
 Home-page: https://github.com/magland/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,19 +13,17 @@
 [![latest-release](https://img.shields.io/pypi/v/mountainsort5.svg)](https://pypi.org/project/mountainsort5)
 ![tests](https://github.com/magland/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/magland/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/magland/mountainsort5)
 
 This is the most recent version of the [MountainSort](https://www.sciencedirect.com/science/article/pii/S0896627317307456) spike sorting algorithm. An implementation of the previous version of this algorithm can be [found here](https://github.com/magland/mountainsort4).
 
 * Uses [Isosplit clustering](https://github.com/magland/isosplit6)
-* Runs much faster than previous versions
-* Works well on large datasets
+* Runs faster than previous versions, especially for large channel counts
 * Better handles time-overlapping events and drifting waveforms
-* Designed to be easy to use and to work well out of the box
-* Runs fast on a CPU
+* Runs fast on CPU
 * Uses SpikeInterface for I/O and preprocessing
 * Supports multiple sorting schemes, each suited for different experimental setups
 
 ![image](https://user-images.githubusercontent.com/3679296/227960322-0723b527-4356-45fb-a045-5ecd6a8269b7.png)
 
 ## Installation
 
@@ -35,17 +33,17 @@
 
 **Dependencies**:
 
 Python, SpikeInterface, scikit-learn, isosplit6
 
 ## Usage
 
-MountainSort5 utilizes [SpikeInterface](https://github.com/spikeinterface/spikeinterface) recording and sorting objects. You can get started by reading the [SpikeInterface documentation](https://spikeinterface.readthedocs.io/en/latest/).
+MountainSort5 utilizes [SpikeInterface](https://github.com/spikeinterface/spikeinterface) recording and sorting objects. See the [SpikeInterface documentation](https://spikeinterface.readthedocs.io/en/latest/) to learn how you can load and preprocess your ephys data.
 
-Once you have a recording object, you can run MountainSort5 using the following code:
+Once you have loaded a SpikeInterface recording object, you can run MountainSort5 using the following code:
 
 ```python
 import spikeinterface as si
 import spikeinterface.preprocessing as spre
 import mountainsort5 as ms5
 
 recording = ... # load your recording using SpikeInterface
@@ -82,43 +80,43 @@
 
 Scheme 2: [examples/scheme2/toy_example.py](./examples/scheme2/toy_example.py)
 
 Scheme 3: [examples/scheme3/toy_example.py](./examples/scheme3/toy_example.py)
 
 ## Preprocessing
 
-MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html), so that intermediate files do not need to be stored to disk.
+MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html) so that intermediate files do not need to be stored to disk.
 
 ## Sorting schemes
 
-MountainSort5 is organized into multiple *sorting schemes*. Different experimental setups will be best served by using different schemes.
+MountainSort5 is organized into three *sorting schemes*. Different schemes are appropriate for different experimental setups.
 
 ### Sorting scheme 1
 
-This is the simplest sorting scheme and is useful for quick tests. The entire recording is loaded into memory, and clustering is performed in a single pass. In general, scheme 2 should be used intead since it has better handling of events that overlap in time, and works with larger datasets on limited RAM systems. Nevertheless, scheme 1 can be useful for testing and debugging, and is used as the first pass in scheme 2.
+This is the simplest sorting scheme and is useful for quick tests. The entire recording is loaded into memory, and clustering is performed in a single pass. In general, scheme 1 should only be used for testing and debugging as scheme 2 does a better job handling events that overlap in time, and works with larger datasets on limited RAM systems. Scheme 1 is used as a first pass in scheme 2, so reading about the parameters of scheme 1 will help you understand the other schemes better.
 
 [Read more about scheme 1](./docs/scheme1.md)
 
 ### Sorting scheme 2
 
 The second sorting scheme is generally preferred over scheme 1 because it can handle larger datasets that cannot be fully loaded into memory, and also has other advantages in terms of accurately detecting and labeling spikes.
 
-In phase 1, the first scheme is used as a training step, performing unsupervised clustering on a subset of the dataset. Then in phase 2, a set of classifiers are trained based on the labels of the training step. The classifiers are then used to label the remaining data.
+In phase 1, the first scheme is used as a training step, performing unsupervised clustering on a subset of the dataset. Then in phase 2, a set of classifiers are trained based on the labels of the training step. The classifiers are then used to label the spikes in the entire recording.
 
 [Read more about scheme 2](./docs/scheme2.md)
 
 ### Sorting scheme 3
 
-Sorting scheme 3 is designed to handle long recordings that may involve waveform drift. The recording is divided into blocks, and each is spike sorted using scheme 2. Then the snippet classifiers are used to associate matching units between blocks.
+Sorting scheme 3 is designed to handle long recordings that may involve waveform drift. The recording is divided into blocks, and each block is spike sorted using scheme 2. Then the snippet classifiers for the blocks are used to associate matching units between blocks.
 
 [Read more about scheme 3](./docs/scheme3.md)
 
 ## Citing MountainSort
 
-Until there is a new publication, please cite the original MountainSort paper:
+For now, please cite the original MountainSort paper:
 
 ```bitex
 @article{chung2017fully,
   title={A fully automated approach to spike sorting},
   author={Chung, Jason E and Magland, Jeremy F and Barnett, Alex H and Tolosa, Vanessa M and Tooker, Angela C and Lee, Kye Y and Shah, Kedar G and Felix, Sarah H and Frank, Loren M and Greengard, Leslie F},
   journal={Neuron},
   volume={95},
@@ -153,18 +151,18 @@
 
 Jeremy Magland, Center for Computational Mathematics, Flatiron Institute
 
 ## Acknowledgements
 
 Thank you to Loren Frank and members of his lab for their support of this project at all stages of development.
 
-Thank you to Alex Barnett and Leslie Greengard for their work on the original Isosplit and MountainSort algorithms.
+Thank you to Alex Barnett, Leslie Greengard, and Jason Chung for their work on the original Isosplit and MountainSort algorithms.
 
 Thank you to the [SpikeInterface team](https://spikeinterface.readthedocs.io/en/latest/authors.html), especially Alessio Buccino and Samuel Garcia, for their work on the SpikeInterface framework, which supports pre- and post-processing and makes it easy to use MountainSort5 with a variety of file formats.
 
-Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it easy to inspect the results of MountainSort5.
+Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it possible to inspect the results of MountainSort5 and other algorithms.
 
 Finally, thank you to all the users of the previous version of MountainSort who have provided feedback and suggestions.
 
 ## License
 
 Apache-2.0
```

### Comparing `mountainsort5-0.1.2/README.md` & `mountainsort5-0.1.3/mountainsort5.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+Metadata-Version: 2.1
+Name: mountainsort5
+Version: 0.1.3
+Summary: MountainSort 5 spike sorting algorithm
+Home-page: https://github.com/magland/mountainsort5
+Author: Jeremy Magland
+Author-email: jmagland@flatironinstitute.org
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MountainSort 5
 
 [![latest-release](https://img.shields.io/pypi/v/mountainsort5.svg)](https://pypi.org/project/mountainsort5)
 ![tests](https://github.com/magland/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/magland/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/magland/mountainsort5)
 
 This is the most recent version of the [MountainSort](https://www.sciencedirect.com/science/article/pii/S0896627317307456) spike sorting algorithm. An implementation of the previous version of this algorithm can be [found here](https://github.com/magland/mountainsort4).
 
 * Uses [Isosplit clustering](https://github.com/magland/isosplit6)
-* Runs much faster than previous versions
-* Works well on large datasets
+* Runs faster than previous versions, especially for large channel counts
 * Better handles time-overlapping events and drifting waveforms
-* Designed to be easy to use and to work well out of the box
-* Runs fast on a CPU
+* Runs fast on CPU
 * Uses SpikeInterface for I/O and preprocessing
 * Supports multiple sorting schemes, each suited for different experimental setups
 
 ![image](https://user-images.githubusercontent.com/3679296/227960322-0723b527-4356-45fb-a045-5ecd6a8269b7.png)
 
 ## Installation
 
@@ -25,17 +33,17 @@
 
 **Dependencies**:
 
 Python, SpikeInterface, scikit-learn, isosplit6
 
 ## Usage
 
-MountainSort5 utilizes [SpikeInterface](https://github.com/spikeinterface/spikeinterface) recording and sorting objects. You can get started by reading the [SpikeInterface documentation](https://spikeinterface.readthedocs.io/en/latest/).
+MountainSort5 utilizes [SpikeInterface](https://github.com/spikeinterface/spikeinterface) recording and sorting objects. See the [SpikeInterface documentation](https://spikeinterface.readthedocs.io/en/latest/) to learn how you can load and preprocess your ephys data.
 
-Once you have a recording object, you can run MountainSort5 using the following code:
+Once you have loaded a SpikeInterface recording object, you can run MountainSort5 using the following code:
 
 ```python
 import spikeinterface as si
 import spikeinterface.preprocessing as spre
 import mountainsort5 as ms5
 
 recording = ... # load your recording using SpikeInterface
@@ -72,43 +80,43 @@
 
 Scheme 2: [examples/scheme2/toy_example.py](./examples/scheme2/toy_example.py)
 
 Scheme 3: [examples/scheme3/toy_example.py](./examples/scheme3/toy_example.py)
 
 ## Preprocessing
 
-MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html), so that intermediate files do not need to be stored to disk.
+MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html) so that intermediate files do not need to be stored to disk.
 
 ## Sorting schemes
 
-MountainSort5 is organized into multiple *sorting schemes*. Different experimental setups will be best served by using different schemes.
+MountainSort5 is organized into three *sorting schemes*. Different schemes are appropriate for different experimental setups.
 
 ### Sorting scheme 1
 
-This is the simplest sorting scheme and is useful for quick tests. The entire recording is loaded into memory, and clustering is performed in a single pass. In general, scheme 2 should be used intead since it has better handling of events that overlap in time, and works with larger datasets on limited RAM systems. Nevertheless, scheme 1 can be useful for testing and debugging, and is used as the first pass in scheme 2.
+This is the simplest sorting scheme and is useful for quick tests. The entire recording is loaded into memory, and clustering is performed in a single pass. In general, scheme 1 should only be used for testing and debugging as scheme 2 does a better job handling events that overlap in time, and works with larger datasets on limited RAM systems. Scheme 1 is used as a first pass in scheme 2, so reading about the parameters of scheme 1 will help you understand the other schemes better.
 
 [Read more about scheme 1](./docs/scheme1.md)
 
 ### Sorting scheme 2
 
 The second sorting scheme is generally preferred over scheme 1 because it can handle larger datasets that cannot be fully loaded into memory, and also has other advantages in terms of accurately detecting and labeling spikes.
 
-In phase 1, the first scheme is used as a training step, performing unsupervised clustering on a subset of the dataset. Then in phase 2, a set of classifiers are trained based on the labels of the training step. The classifiers are then used to label the remaining data.
+In phase 1, the first scheme is used as a training step, performing unsupervised clustering on a subset of the dataset. Then in phase 2, a set of classifiers are trained based on the labels of the training step. The classifiers are then used to label the spikes in the entire recording.
 
 [Read more about scheme 2](./docs/scheme2.md)
 
 ### Sorting scheme 3
 
-Sorting scheme 3 is designed to handle long recordings that may involve waveform drift. The recording is divided into blocks, and each is spike sorted using scheme 2. Then the snippet classifiers are used to associate matching units between blocks.
+Sorting scheme 3 is designed to handle long recordings that may involve waveform drift. The recording is divided into blocks, and each block is spike sorted using scheme 2. Then the snippet classifiers for the blocks are used to associate matching units between blocks.
 
 [Read more about scheme 3](./docs/scheme3.md)
 
 ## Citing MountainSort
 
-Until there is a new publication, please cite the original MountainSort paper:
+For now, please cite the original MountainSort paper:
 
 ```bitex
 @article{chung2017fully,
   title={A fully automated approach to spike sorting},
   author={Chung, Jason E and Magland, Jeremy F and Barnett, Alex H and Tolosa, Vanessa M and Tooker, Angela C and Lee, Kye Y and Shah, Kedar G and Felix, Sarah H and Frank, Loren M and Greengard, Leslie F},
   journal={Neuron},
   volume={95},
@@ -143,18 +151,18 @@
 
 Jeremy Magland, Center for Computational Mathematics, Flatiron Institute
 
 ## Acknowledgements
 
 Thank you to Loren Frank and members of his lab for their support of this project at all stages of development.
 
-Thank you to Alex Barnett and Leslie Greengard for their work on the original Isosplit and MountainSort algorithms.
+Thank you to Alex Barnett, Leslie Greengard, and Jason Chung for their work on the original Isosplit and MountainSort algorithms.
 
 Thank you to the [SpikeInterface team](https://spikeinterface.readthedocs.io/en/latest/authors.html), especially Alessio Buccino and Samuel Garcia, for their work on the SpikeInterface framework, which supports pre- and post-processing and makes it easy to use MountainSort5 with a variety of file formats.
 
-Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it easy to inspect the results of MountainSort5.
+Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it possible to inspect the results of MountainSort5 and other algorithms.
 
 Finally, thank you to all the users of the previous version of MountainSort who have provided feedback and suggestions.
 
 ## License
 
 Apache-2.0
```

### Comparing `mountainsort5-0.1.2/mountainsort5/core/SnippetClassifier.py` & `mountainsort5-0.1.3/mountainsort5/core/SnippetClassifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,34 @@
 import numpy.typing as npt
 from dataclasses import dataclass
 from sklearn import decomposition
 from sklearn.neighbors import NearestNeighbors
 
 
 class SnippetClassifier:
-    def __init__(self, npca: int) -> None:
+    def __init__(self, npca: Union[int, None]) -> None:
         self.npca = npca
         self.training_batches: List[TrainingBatch] = []
         self.pca_model = None
     def add_training_snippets(self, snippets: npt.NDArray[np.float32], label: int, offset: int):
         self.training_batches.append(TrainingBatch(snippets=snippets, label=label, offset=offset))
     def fit(self):
         if len(self.training_batches) == 0:
             raise Exception('No training batches added for classifier.') # pragma: no cover
         all_training_snippets = np.concatenate([b.snippets for b in self.training_batches], axis=0)
         L = all_training_snippets.shape[0]
         self.T = all_training_snippets.shape[1]
         self.M = all_training_snippets.shape[2]
         self.all_training_labels = np.concatenate([np.ones((b.num_snippets,), dtype=np.int32) * b.label for b in self.training_batches])
         self.all_training_offsets = np.concatenate([np.ones((b.num_snippets,), dtype=np.int32) * b.offset for b in self.training_batches])
-        self.pca_model = decomposition.PCA(n_components=min(self.npca, L))
+        if self.npca is not None:
+            effective_npca = self.npca
+        else:
+            effective_npca = max(12, self.M * 3)
+        self.pca_model = decomposition.PCA(n_components=min(effective_npca, L))
         self.pca_model.fit(all_training_snippets.reshape(L, self.T * self.M))
         X = self.pca_model.transform(all_training_snippets.reshape(L, self.T * self.M))
         self.nearest_neighbor_model = NearestNeighbors(n_neighbors=2)
         self.nearest_neighbor_model.fit(X)
     def classify_snippets(self, snippets: npt.NDArray[np.float32]) -> Tuple[Union[npt.NDArray[np.int32], None], Union[npt.NDArray[np.int32], None]]:
         if self.pca_model is None:
             raise Exception('self.pca_model is None, which probably means that fit() was not called.') # pragma: no cover
```

### Comparing `mountainsort5-0.1.2/mountainsort5/core/cluster_snippets.py` & `mountainsort5-0.1.3/mountainsort5/core/cluster_snippets.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/core/detect_spikes.py` & `mountainsort5-0.1.3/mountainsort5/core/detect_spikes.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/core/extract_snippets.py` & `mountainsort5-0.1.3/mountainsort5/core/extract_snippets.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/core/get_block_recording_for_scheme3.py` & `mountainsort5-0.1.3/mountainsort5/core/get_block_recording_for_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/core/get_sampled_recording_for_training.py` & `mountainsort5-0.1.3/mountainsort5/core/get_sampled_recording_for_training.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/core/get_times_labels_from_sorting.py` & `mountainsort5-0.1.3/mountainsort5/core/get_times_labels_from_sorting.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/core/pairwise_merge_step.py` & `mountainsort5-0.1.3/mountainsort5/core/pairwise_merge_step.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/schemes/Scheme1SortingParameters.py` & `mountainsort5-0.1.3/mountainsort5/schemes/Scheme1SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/schemes/Scheme2SortingParameters.py` & `mountainsort5-0.1.3/mountainsort5/schemes/Scheme2SortingParameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     - phase1_pairwise_merge_step: pairwise_merge_step in phase 1
     - detect_sign
     - detect_threshold: detect_threshold in phase 2
     - snippet_T1
     - snippet_T2
     - snippet_mask_radius
     - max_num_snippets_per_training_batch: the maximum number of snippets to use for training the classifier in each batch
-    - classifier_npca: the number of principal components to use for the classifier
+    - classifier_npca: the number of principal components to use for each neighborhood classifier
     - training_duration_sec: the duration of the training data (in seconds)
     - training_recording_sampling_mode: how to sample the training data. If 'initial', then the first training_duration_sec of the recording will be used. If 'uniform', then the training data will be sampled uniformly in 10-second chunks from the recording.
     """
     phase1_detect_channel_radius: Union[float, None]
     detect_channel_radius: Union[float, None]
     phase1_detect_threshold: float=5.5
     phase1_detect_time_radius_msec: float=1.5
@@ -36,15 +36,15 @@
     phase1_pairwise_merge_step: bool=True
     detect_sign: int=-1
     detect_threshold: float=5.5
     snippet_T1: int=20
     snippet_T2: int=20
     snippet_mask_radius: Union[float, None]=None
     max_num_snippets_per_training_batch: int=200
-    classifier_npca: Union[int, None]=60
+    classifier_npca: Union[int, None]=None
     training_duration_sec: Union[float, None]=None
     training_recording_sampling_mode: Literal['initial', 'uniform']='initial'
 
     def check_valid(self, *, M: int, N: int, sampling_frequency: float, channel_locations: npt.NDArray[np.float32]):
         """Internal function for checking validity of parameters"""
         assert channel_locations.shape[0] == M, 'Shape mismatch between traces and channel locations'
         D = channel_locations.shape[1]
```

### Comparing `mountainsort5-0.1.2/mountainsort5/schemes/Scheme3SortingParameters.py` & `mountainsort5-0.1.3/mountainsort5/schemes/Scheme3SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/mountainsort5/schemes/sorting_scheme1.py` & `mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme1.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,24 @@
         recording (si.BaseRecording): SpikeInterface recording object
         sorting_parameters (Scheme2SortingParameters): Sorting parameters
 
     Returns:
         si.BaseSorting: SpikeInterface sorting object
     """
 
+    ###################################################################
+    # Handle multi-segment recordings
     if recording.get_num_segments() > 1:
         print('Recording has multiple segments. Joining segments for sorting...')
         recording_joined = si.concatenate_recordings(recording_list=[recording])
         sorting_joined = sorting_scheme1(recording_joined, sorting_parameters=sorting_parameters)
         print('Splitting sorting into segments to match original multisegment recording...')
         sorting = si.split_sorting(sorting_joined, recording_joined)
         return sorting
+    ###################################################################
 
     M = recording.get_num_channels()
     N = recording.get_num_frames()
     sampling_frequency = recording.sampling_frequency
 
     channel_locations = recording.get_channel_locations()
```

### Comparing `mountainsort5-0.1.2/mountainsort5/schemes/sorting_scheme2.py` & `mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme2.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,35 @@
 from ..core.get_sampled_recording_for_training import get_sampled_recording_for_training
 from ..core.get_times_labels_from_sorting import get_times_labels_from_sorting
 
 
 def sorting_scheme2(
     recording: si.BaseRecording, *,
     sorting_parameters: Scheme2SortingParameters,
-    return_snippet_classifiers: bool = False,
-    reference_snippet_classifiers: Union[Dict[int, SnippetClassifier], None] = None,
-    label_offset: int = 0
+    return_snippet_classifiers: bool = False, # used in scheme 3
+    reference_snippet_classifiers: Union[Dict[int, SnippetClassifier], None] = None, # used in scheme 3
+    label_offset: int = 0 # used in scheme 3
 ) -> Union[si.BaseSorting, Tuple[si.BaseSorting, Dict[int, SnippetClassifier]]]:
     """MountainSort 5 sorting scheme 2
 
     Args:
         recording (si.BaseRecording): SpikeInterface recording object
         sorting_parameters (Scheme2SortingParameters): Sorting parameters
+        return_snippet_classifiers (bool): whether to return the snippet classifiers (used in scheme 3)
+        reference_snippet_classifiers: used in scheme 3
+        label_offset: used in scheme 3
 
     Returns:
         si.BaseSorting: SpikeInterface sorting object
+            or, if return_snippet_classifiers is True:
+        si.BaseSorting, snippet_classifiers
     """
 
+    ###################################################################
+    # Handle multi-segment recordings
     if recording.get_num_segments() > 1:
         print('Recording has multiple segments. Joining segments for sorting...')
         recording_joined = si.concatenate_recordings(recording_list=[recording])
         sorting_joined, snippet_classifiers = sorting_scheme2(
             recording_joined,
             sorting_parameters=sorting_parameters,
             return_snippet_classifiers=True,
@@ -43,20 +50,22 @@
         )
         print('Splitting sorting into segments to match original multisegment recording...')
         sorting = si.split_sorting(sorting_joined, recording_joined)
         if return_snippet_classifiers:
             return sorting, snippet_classifiers
         else:
             return sorting
+    ###################################################################
 
     M = recording.get_num_channels()
     N = recording.get_num_frames()
     sampling_frequency = recording.sampling_frequency
     channel_locations = recording.get_channel_locations()
 
+    # check that the sorting parameters are valid
     sorting_parameters.check_valid(M=M, N=N, sampling_frequency=sampling_frequency, channel_locations=channel_locations)
 
     # Subsample the recording for training
     if sorting_parameters.training_duration_sec is not None:
         training_recording = get_sampled_recording_for_training(
             recording=recording,
             training_duration_sec=sorting_parameters.training_duration_sec,
@@ -77,16 +86,16 @@
             snippet_T1=sorting_parameters.snippet_T1,
             snippet_T2=sorting_parameters.snippet_T2,
             npca_per_branch=sorting_parameters.phase1_npca_per_branch,
             pairwise_merge_step=sorting_parameters.phase1_pairwise_merge_step
         )
     )
     times, labels = get_times_labels_from_sorting(sorting1)
-    K = np.max(labels)
-    labels = labels + label_offset
+    K = np.max(labels) # number of clusters
+    labels = labels + label_offset # used in scheme 3
 
     print('Loading training traces')
     # Load the traces from the training recording
     training_traces = training_recording.get_traces()
     training_snippets = extract_snippets(
         traces=training_traces,
         channel_locations=None,
```

### Comparing `mountainsort5-0.1.2/mountainsort5/schemes/sorting_scheme3.py` & `mountainsort5-0.1.3/mountainsort5/schemes/sorting_scheme3.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,24 @@
         recording (si.BaseRecording): SpikeInterface recording object
         sorting_parameters (Scheme3SortingParameters): Sorting parameters
 
     Returns:
         si.BaseSorting: SpikeInterface sorting object
     """
 
+    ###################################################################
+    # Handle multi-segment recordings
     if recording.get_num_segments() > 1:
         print('Recording has multiple segments. Joining segments for sorting...')
         recording_joined = si.concatenate_recordings(recording_list=[recording])
         sorting_joined = sorting_scheme3(recording_joined, sorting_parameters=sorting_parameters)
         print('Splitting sorting into segments to match original multisegment recording...')
         sorting = si.split_sorting(sorting_joined, recording_joined)
         return sorting
+    ###################################################################
 
     M = recording.get_num_channels()
     N = recording.get_num_frames()
     sampling_frequency = recording.sampling_frequency
     channel_locations = recording.get_channel_locations()
 
     sorting_parameters.check_valid(M=M, N=N, sampling_frequency=sampling_frequency, channel_locations=channel_locations)
```

### Comparing `mountainsort5-0.1.2/mountainsort5.egg-info/PKG-INFO` & `mountainsort5-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-Metadata-Version: 2.1
-Name: mountainsort5
-Version: 0.1.2
-Summary: MountainSort 5 spike sorting algorithm
-Home-page: https://github.com/magland/mountainsort5
-Author: Jeremy Magland
-Author-email: jmagland@flatironinstitute.org
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MountainSort 5
 
 [![latest-release](https://img.shields.io/pypi/v/mountainsort5.svg)](https://pypi.org/project/mountainsort5)
 ![tests](https://github.com/magland/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/magland/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/magland/mountainsort5)
 
 This is the most recent version of the [MountainSort](https://www.sciencedirect.com/science/article/pii/S0896627317307456) spike sorting algorithm. An implementation of the previous version of this algorithm can be [found here](https://github.com/magland/mountainsort4).
 
 * Uses [Isosplit clustering](https://github.com/magland/isosplit6)
-* Runs much faster than previous versions
-* Works well on large datasets
+* Runs faster than previous versions, especially for large channel counts
 * Better handles time-overlapping events and drifting waveforms
-* Designed to be easy to use and to work well out of the box
-* Runs fast on a CPU
+* Runs fast on CPU
 * Uses SpikeInterface for I/O and preprocessing
 * Supports multiple sorting schemes, each suited for different experimental setups
 
 ![image](https://user-images.githubusercontent.com/3679296/227960322-0723b527-4356-45fb-a045-5ecd6a8269b7.png)
 
 ## Installation
 
@@ -35,17 +23,17 @@
 
 **Dependencies**:
 
 Python, SpikeInterface, scikit-learn, isosplit6
 
 ## Usage
 
-MountainSort5 utilizes [SpikeInterface](https://github.com/spikeinterface/spikeinterface) recording and sorting objects. You can get started by reading the [SpikeInterface documentation](https://spikeinterface.readthedocs.io/en/latest/).
+MountainSort5 utilizes [SpikeInterface](https://github.com/spikeinterface/spikeinterface) recording and sorting objects. See the [SpikeInterface documentation](https://spikeinterface.readthedocs.io/en/latest/) to learn how you can load and preprocess your ephys data.
 
-Once you have a recording object, you can run MountainSort5 using the following code:
+Once you have loaded a SpikeInterface recording object, you can run MountainSort5 using the following code:
 
 ```python
 import spikeinterface as si
 import spikeinterface.preprocessing as spre
 import mountainsort5 as ms5
 
 recording = ... # load your recording using SpikeInterface
@@ -82,43 +70,43 @@
 
 Scheme 2: [examples/scheme2/toy_example.py](./examples/scheme2/toy_example.py)
 
 Scheme 3: [examples/scheme3/toy_example.py](./examples/scheme3/toy_example.py)
 
 ## Preprocessing
 
-MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html), so that intermediate files do not need to be stored to disk.
+MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html) so that intermediate files do not need to be stored to disk.
 
 ## Sorting schemes
 
-MountainSort5 is organized into multiple *sorting schemes*. Different experimental setups will be best served by using different schemes.
+MountainSort5 is organized into three *sorting schemes*. Different schemes are appropriate for different experimental setups.
 
 ### Sorting scheme 1
 
-This is the simplest sorting scheme and is useful for quick tests. The entire recording is loaded into memory, and clustering is performed in a single pass. In general, scheme 2 should be used intead since it has better handling of events that overlap in time, and works with larger datasets on limited RAM systems. Nevertheless, scheme 1 can be useful for testing and debugging, and is used as the first pass in scheme 2.
+This is the simplest sorting scheme and is useful for quick tests. The entire recording is loaded into memory, and clustering is performed in a single pass. In general, scheme 1 should only be used for testing and debugging as scheme 2 does a better job handling events that overlap in time, and works with larger datasets on limited RAM systems. Scheme 1 is used as a first pass in scheme 2, so reading about the parameters of scheme 1 will help you understand the other schemes better.
 
 [Read more about scheme 1](./docs/scheme1.md)
 
 ### Sorting scheme 2
 
 The second sorting scheme is generally preferred over scheme 1 because it can handle larger datasets that cannot be fully loaded into memory, and also has other advantages in terms of accurately detecting and labeling spikes.
 
-In phase 1, the first scheme is used as a training step, performing unsupervised clustering on a subset of the dataset. Then in phase 2, a set of classifiers are trained based on the labels of the training step. The classifiers are then used to label the remaining data.
+In phase 1, the first scheme is used as a training step, performing unsupervised clustering on a subset of the dataset. Then in phase 2, a set of classifiers are trained based on the labels of the training step. The classifiers are then used to label the spikes in the entire recording.
 
 [Read more about scheme 2](./docs/scheme2.md)
 
 ### Sorting scheme 3
 
-Sorting scheme 3 is designed to handle long recordings that may involve waveform drift. The recording is divided into blocks, and each is spike sorted using scheme 2. Then the snippet classifiers are used to associate matching units between blocks.
+Sorting scheme 3 is designed to handle long recordings that may involve waveform drift. The recording is divided into blocks, and each block is spike sorted using scheme 2. Then the snippet classifiers for the blocks are used to associate matching units between blocks.
 
 [Read more about scheme 3](./docs/scheme3.md)
 
 ## Citing MountainSort
 
-Until there is a new publication, please cite the original MountainSort paper:
+For now, please cite the original MountainSort paper:
 
 ```bitex
 @article{chung2017fully,
   title={A fully automated approach to spike sorting},
   author={Chung, Jason E and Magland, Jeremy F and Barnett, Alex H and Tolosa, Vanessa M and Tooker, Angela C and Lee, Kye Y and Shah, Kedar G and Felix, Sarah H and Frank, Loren M and Greengard, Leslie F},
   journal={Neuron},
   volume={95},
@@ -153,18 +141,18 @@
 
 Jeremy Magland, Center for Computational Mathematics, Flatiron Institute
 
 ## Acknowledgements
 
 Thank you to Loren Frank and members of his lab for their support of this project at all stages of development.
 
-Thank you to Alex Barnett and Leslie Greengard for their work on the original Isosplit and MountainSort algorithms.
+Thank you to Alex Barnett, Leslie Greengard, and Jason Chung for their work on the original Isosplit and MountainSort algorithms.
 
 Thank you to the [SpikeInterface team](https://spikeinterface.readthedocs.io/en/latest/authors.html), especially Alessio Buccino and Samuel Garcia, for their work on the SpikeInterface framework, which supports pre- and post-processing and makes it easy to use MountainSort5 with a variety of file formats.
 
-Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it easy to inspect the results of MountainSort5.
+Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it possible to inspect the results of MountainSort5 and other algorithms.
 
 Finally, thank you to all the users of the previous version of MountainSort who have provided feedback and suggestions.
 
 ## License
 
 Apache-2.0
```

### Comparing `mountainsort5-0.1.2/mountainsort5.egg-info/SOURCES.txt` & `mountainsort5-0.1.3/mountainsort5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/setup.py` & `mountainsort5-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README.md
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 setup(
     name='mountainsort5',
     version=__version__,
     author="Jeremy Magland",
     author_email="jmagland@flatironinstitute.org",
     url="https://github.com/magland/mountainsort5",
```

### Comparing `mountainsort5-0.1.2/tests/test_core.py` & `mountainsort5-0.1.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/tests/test_scheme1.py` & `mountainsort5-0.1.3/tests/test_scheme1.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.2/tests/test_scheme2.py` & `mountainsort5-0.1.3/tests/test_scheme3.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,56 +2,43 @@
 import spikeinterface as si
 import spikeinterface.extractors as se
 import spikeinterface.preprocessing as spre
 import spikeinterface.comparison as sc
 import mountainsort5 as ms5
 
 
-def test_scheme2():
+def test_scheme3():
     recording, sorting_true = se.toy_example(
-        duration=40,
+        duration=20,
         num_channels=8,
         num_units=16,
         sampling_frequency=30000,
         num_segments=2,
         seed=0
     )
 
+    timer = time.time()
+
     # lazy preprocessing
     recording_filtered = spre.bandpass_filter(recording, freq_min=300, freq_max=6000)
     recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered)
 
     # sorting
-    print('Starting MountainSort5 (sorting1)')
-    timer = time.time()
-    sorting1 = ms5.sorting_scheme2(
-        recording_preprocessed,
-        sorting_parameters=ms5.Scheme2SortingParameters(
-            phase1_detect_channel_radius=150,
-            detect_channel_radius=50,
-            max_num_snippets_per_training_batch=3, # for improving test coverage
-            snippet_mask_radius=150,
-            training_duration_sec=15
-        )
-    )
-    elapsed_sec = time.time() - timer
-    duration_sec = recording.get_total_duration()
-    print(f'Elapsed time for sorting: {elapsed_sec:.2f} sec -- x{(duration_sec / elapsed_sec):.2f} speed compared with real time for {recording.get_num_channels()} channels')
-
-    print('Starting MountainSort5 (sorting2)')
-    timer = time.time()
-    sorting2 = ms5.sorting_scheme2(
+    print('Starting MountainSort5')
+    sorting = ms5.sorting_scheme3(
         recording_preprocessed,
-        sorting_parameters=ms5.Scheme2SortingParameters(
-            phase1_detect_channel_radius=150,
-            detect_channel_radius=50,
-            training_duration_sec=25,
-            training_recording_sampling_mode='uniform'
+        sorting_parameters=ms5.Scheme3SortingParameters(
+            block_sorting_parameters=ms5.Scheme2SortingParameters(
+                phase1_detect_channel_radius=150,
+                detect_channel_radius=50
+            ),
+            block_duration_sec=3
         )
     )
+    
     elapsed_sec = time.time() - timer
     duration_sec = recording.get_total_duration()
     print(f'Elapsed time for sorting: {elapsed_sec:.2f} sec -- x{(duration_sec / elapsed_sec):.2f} speed compared with real time for {recording.get_num_channels()} channels')
 
     # commenting out because this step takes a while
     # print('Comparing with truth')
     # comparison = sc.compare_sorter_to_ground_truth(gt_sorting=sorting_true, tested_sorting=sorting)
```

