# Comparing `tmp/cleanvision-0.1.1.tar.gz` & `tmp/cleanvision-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanvision-0.1.1.tar", last modified: Fri Mar 31 18:03:56 2023, max compression
+gzip compressed data, was "/Users/sanjana/cleanlab_home/cleanvision/dist/.tmp-pef1lbg3/cleanvision-0.2.0.tar", last modified: Tue Apr 11 03:03:25 2023, max compression
```

## Comparing `cleanvision-0.1.1.tar` & `cleanvision-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-31 18:03:56.384720 cleanvision-0.1.1/
--rw-r--r--   0 root         (0) staff       (20)     5373 2023-03-31 18:03:04.000000 cleanvision-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) staff       (20)     2911 2023-03-31 18:03:04.000000 cleanvision-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) staff       (20)     3901 2023-03-31 18:03:04.000000 cleanvision-0.1.1/DEVELOPMENT.md
--rw-r--r--   0 root         (0) staff       (20)    34523 2023-03-31 18:03:04.000000 cleanvision-0.1.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       58 2023-03-31 18:03:04.000000 cleanvision-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)    48936 2023-03-31 18:03:56.384395 cleanvision-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     7836 2023-03-31 18:03:04.000000 cleanvision-0.1.1/README.md
--rw-r--r--   0 root         (0) staff       (20)     1619 2023-03-31 18:03:04.000000 cleanvision-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)       38 2023-03-31 18:03:56.384813 cleanvision-0.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-31 18:03:56.372877 cleanvision-0.1.1/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-31 18:03:56.376542 cleanvision-0.1.1/src/cleanvision/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    25338 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/imagelab.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-31 18:03:56.380076 cleanvision-0.1.1/src/cleanvision/issue_managers/
--rw-r--r--   0 root         (0) staff       (20)     2069 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/issue_managers/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8232 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/issue_managers/duplicate_issue_manager.py
--rw-r--r--   0 root         (0) staff       (20)    10509 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/issue_managers/image_property.py
--rw-r--r--   0 root         (0) staff       (20)    12206 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/issue_managers/image_property_issue_manager.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-31 18:03:56.381691 cleanvision-0.1.1/src/cleanvision/utils/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/utils/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     2111 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/utils/base_issue_manager.py
--rw-r--r--   0 root         (0) staff       (20)      668 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/utils/constants.py
--rw-r--r--   0 root         (0) staff       (20)     3329 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/utils/utils.py
--rw-r--r--   0 root         (0) staff       (20)     1952 2023-03-31 18:03:04.000000 cleanvision-0.1.1/src/cleanvision/utils/viz_manager.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-31 18:03:56.378723 cleanvision-0.1.1/src/cleanvision.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    48936 2023-03-31 18:03:56.000000 cleanvision-0.1.1/src/cleanvision.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      920 2023-03-31 18:03:56.000000 cleanvision-0.1.1/src/cleanvision.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-03-31 18:03:56.000000 cleanvision-0.1.1/src/cleanvision.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      102 2023-03-31 18:03:56.000000 cleanvision-0.1.1/src/cleanvision.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2023-03-31 18:03:56.000000 cleanvision-0.1.1/src/cleanvision.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-31 18:03:56.383831 cleanvision-0.1.1/tests/
--rw-r--r--   0 root         (0) staff       (20)     8473 2023-03-31 18:03:04.000000 cleanvision-0.1.1/tests/test_duplicate_issue_manager.py
--rw-r--r--   0 root         (0) staff       (20)     4297 2023-03-31 18:03:04.000000 cleanvision-0.1.1/tests/test_image_property_helpers.py
--rw-r--r--   0 root         (0) staff       (20)     3594 2023-03-31 18:03:04.000000 cleanvision-0.1.1/tests/test_image_property_issue_manager.py
--rw-r--r--   0 root         (0) staff       (20)     6947 2023-03-31 18:03:04.000000 cleanvision-0.1.1/tests/test_run.py
--rw-r--r--   0 root         (0) staff       (20)      529 2023-03-31 18:03:04.000000 cleanvision-0.1.1/tests/test_utils.py
--rw-r--r--   0 root         (0) staff       (20)     1330 2023-03-31 18:03:04.000000 cleanvision-0.1.1/tests/test_viz_manager.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/
+-rw-r--r--   0 sanjana    (501) staff       (20)     5373 2023-04-10 14:40:45.000000 cleanvision-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 sanjana    (501) staff       (20)     2989 2023-04-11 02:44:57.000000 cleanvision-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 sanjana    (501) staff       (20)     3901 2023-04-10 14:40:45.000000 cleanvision-0.2.0/DEVELOPMENT.md
+-rw-r--r--   0 sanjana    (501) staff       (20)    34523 2023-04-10 14:40:45.000000 cleanvision-0.2.0/LICENSE
+-rw-r--r--   0 sanjana    (501) staff       (20)       58 2023-04-10 14:40:45.000000 cleanvision-0.2.0/MANIFEST.in
+-rw-r--r--   0 sanjana    (501) staff       (20)    49935 2023-04-11 03:03:25.000000 cleanvision-0.2.0/PKG-INFO
+-rw-r--r--   0 sanjana    (501) staff       (20)     8719 2023-04-11 02:44:57.000000 cleanvision-0.2.0/README.md
+-rw-r--r--   0 sanjana    (501) staff       (20)     1747 2023-04-11 02:44:57.000000 cleanvision-0.2.0/pyproject.toml
+-rw-r--r--   0 sanjana    (501) staff       (20)       38 2023-04-11 03:03:25.000000 cleanvision-0.2.0/setup.cfg
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/
+-rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/__init__.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/dataset/
+-rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/__init__.py
+-rw-r--r--   0 sanjana    (501) staff       (20)      978 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/base_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1044 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/folder_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1076 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/hf_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1019 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/torch_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1184 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/dataset/utils.py
+-rw-r--r--   0 sanjana    (501) staff       (20)    27008 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/imagelab.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/
+-rw-r--r--   0 sanjana    (501) staff       (20)     2069 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/__init__.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     8447 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/duplicate_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)    10509 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/image_property.py
+-rw-r--r--   0 sanjana    (501) staff       (20)    12346 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/issue_managers/image_property_issue_manager.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision/utils/
+-rw-r--r--   0 sanjana    (501) staff       (20)        0 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/utils/__init__.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     2155 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/utils/base_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)      668 2023-04-10 14:40:45.000000 cleanvision-0.2.0/src/cleanvision/utils/constants.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     3349 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/utils/utils.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1955 2023-04-11 02:44:57.000000 cleanvision-0.2.0/src/cleanvision/utils/viz_manager.py
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/
+-rw-r--r--   0 sanjana    (501) staff       (20)    49935 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/PKG-INFO
+-rw-r--r--   0 sanjana    (501) staff       (20)     1172 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjana    (501) staff       (20)        1 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjana    (501) staff       (20)      164 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/requires.txt
+-rw-r--r--   0 sanjana    (501) staff       (20)       12 2023-04-11 03:03:25.000000 cleanvision-0.2.0/src/cleanvision.egg-info/top_level.txt
+drwxr-xr-x   0 sanjana    (501) staff       (20)        0 2023-04-11 03:03:25.000000 cleanvision-0.2.0/tests/
+-rw-r--r--   0 sanjana    (501) staff       (20)     1969 2023-04-11 02:44:57.000000 cleanvision-0.2.0/tests/test_dataset.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     8473 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_duplicate_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     4297 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_image_property_helpers.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     3594 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_image_property_issue_manager.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     7528 2023-04-11 02:44:57.000000 cleanvision-0.2.0/tests/test_run.py
+-rw-r--r--   0 sanjana    (501) staff       (20)      529 2023-04-10 14:40:45.000000 cleanvision-0.2.0/tests/test_utils.py
+-rw-r--r--   0 sanjana    (501) staff       (20)     1064 2023-04-11 02:44:57.000000 cleanvision-0.2.0/tests/test_viz_manager.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cleanvision-0.1.1/CODE_OF_CONDUCT.md` & `cleanvision-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/CONTRIBUTING.md` & `cleanvision-0.2.0/CONTRIBUTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 All kinds of contributions to CleanVision are greatly appreciated. If you're not looking to write code, submitting a [feature request](#feature-requests) or
 [bug report](#bug-reports) is a great way to contribute. If you want to get
 your hands dirty, you can submit [Pull Requests](#pull-requests), either working on your
 own ideas or addressing [existing issues][issues].
 
 If you are unsure or confused about anything, please go ahead and submit your
 issue or pull request anyways! We appreciate all contributions, and we'll do
-our best to incorporate your feedback or code into CleanVision.
+our best to incorporate your feedback or code into CleanVision. 
+You can also chat with our developers in [Slack](https://cleanlab.ai/slack).
 
 Detailed contributing instructions can be found in the [Development Guide](DEVELOPMENT.md), please read this carefully!
 
 
 ## Feature Requests
 
 Do you have an idea for an awesome new feature for CleanVision? Let us know by
```

### Comparing `cleanvision-0.1.1/DEVELOPMENT.md` & `cleanvision-0.2.0/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/LICENSE` & `cleanvision-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/PKG-INFO` & `cleanvision-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.1.1
+Version: 0.2.0
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,14 +663,15 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Source, https://github.com/cleanlab/cleanvision
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanvision/issues
+Project-URL: Documentation, https://cleanvision.readthedocs.io/
 Keywords: computer_vision,cv,image_data,issue_detection,data_quality,image_quality,machine_learning,data_cleaning,image_deduplication
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -680,14 +681,16 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: huggingface
+Provides-Extra: pytorch
 License-File: LICENSE
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanvision_logo_open_source_transparent.png" width=50% height=50%>
 </p>
 
 <img width="1200" alt="Screen Shot 2023-03-10 at 10 23 33 AM" src="https://user-images.githubusercontent.com/10901697/224394144-bb0e1c85-6851-4828-bcd2-4ed234270a78.png">
@@ -697,61 +700,67 @@
 CleanVision is super simple -- run the same couple lines of Python code to audit any image dataset!
 
 [![Read the Docs](https://readthedocs.org/projects/cleanvision/badge/?version=latest)](https://cleanvision.readthedocs.io/en/latest/)
 [![pypi](https://img.shields.io/pypi/v/cleanvision?color=blue)](https://pypi.org/pypi/cleanvision/)
 [![os](https://img.shields.io/badge/platform-noarch-lightgrey)](https://pypi.org/pypi/cleanvision/)
 [![py\_versions](https://img.shields.io/badge/python-3.7%2B-blue)](https://pypi.org/pypi/cleanvision/)
 [![codecov](https://codecov.io/github/cleanlab/cleanvision/branch/main/graph/badge.svg?token=y1N6MluN9H)](https://codecov.io/gh/cleanlab/cleanvision)
+[![Slack Community](https://img.shields.io/static/v1?logo=slack&style=flat&color=white&label=slack&message=community)](https://cleanlab.ai/slack)
+[![Twitter](https://img.shields.io/twitter/follow/CleanlabAI?style=social)](https://twitter.com/CleanlabAI)
+[![Cleanlab Studio](https://raw.githubusercontent.com/cleanlab/assets/master/shields/cl-studio-shield.svg)](https://cleanlab.ai/studio/?utm_source=github&utm_medium=readme&utm_campaign=clostostudio)
 
 ## Installation
-
 ```shell
 pip install cleanvision
 ```
 
 ## Quickstart
 
 Download an example dataset (optional). Or just use any collection of image files you have.
 
 ```shell
 wget -nc 'https://cleanlab-public.s3.amazonaws.com/CleanVision/image_files.zip'
 ```
 
-Run CleanVision to audit the images.
+1. Run CleanVision to audit the images.
 
 ```python
 from cleanvision.imagelab import Imagelab
 
 # Specify path to folder containing the image files in your dataset
 imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
 
 # Automatically check for a predefined list of issues within your dataset
 imagelab.find_issues()
 
 # Produce a neat report of the issues found in your dataset
 imagelab.report()
 ```
 
-CleanVision diagnoses many types of issues, but you can also check for only specific issues.
+2. CleanVision diagnoses many types of issues, but you can also check for only specific issues.
 
 ```python
 issue_types = {"dark": {}, "blurry": {}}
 
 imagelab.find_issues(issue_types=issue_types)
 
 # Produce a report with only the specified issue_types
 imagelab.report(issue_types=issue_types)
 ```
 
+
 ## More resources on how to use CleanVision
 
 - [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
-- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py)
+- [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
+- [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
+- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
+- [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
 The quality of machine learning models hinges on the quality of the data used to train them, but it is hard to manually identify all of the low-quality data in a big dataset. CleanVision helps you automatically identify common types of data issues lurking in image datasets.
 
 This package currently detects issues in the raw images themselves, making it a useful tool for any computer vision
 task such as: classification, segmentation, object detection, pose estimation, keypoint detection, [generative modeling](https://openai.com/research/dall-e-2-pre-training-mitigations), etc.
```

### Comparing `cleanvision-0.1.1/README.md` & `cleanvision-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,61 +9,67 @@
 CleanVision is super simple -- run the same couple lines of Python code to audit any image dataset!
 
 [![Read the Docs](https://readthedocs.org/projects/cleanvision/badge/?version=latest)](https://cleanvision.readthedocs.io/en/latest/)
 [![pypi](https://img.shields.io/pypi/v/cleanvision?color=blue)](https://pypi.org/pypi/cleanvision/)
 [![os](https://img.shields.io/badge/platform-noarch-lightgrey)](https://pypi.org/pypi/cleanvision/)
 [![py\_versions](https://img.shields.io/badge/python-3.7%2B-blue)](https://pypi.org/pypi/cleanvision/)
 [![codecov](https://codecov.io/github/cleanlab/cleanvision/branch/main/graph/badge.svg?token=y1N6MluN9H)](https://codecov.io/gh/cleanlab/cleanvision)
+[![Slack Community](https://img.shields.io/static/v1?logo=slack&style=flat&color=white&label=slack&message=community)](https://cleanlab.ai/slack)
+[![Twitter](https://img.shields.io/twitter/follow/CleanlabAI?style=social)](https://twitter.com/CleanlabAI)
+[![Cleanlab Studio](https://raw.githubusercontent.com/cleanlab/assets/master/shields/cl-studio-shield.svg)](https://cleanlab.ai/studio/?utm_source=github&utm_medium=readme&utm_campaign=clostostudio)
 
 ## Installation
-
 ```shell
 pip install cleanvision
 ```
 
 ## Quickstart
 
 Download an example dataset (optional). Or just use any collection of image files you have.
 
 ```shell
 wget -nc 'https://cleanlab-public.s3.amazonaws.com/CleanVision/image_files.zip'
 ```
 
-Run CleanVision to audit the images.
+1. Run CleanVision to audit the images.
 
 ```python
 from cleanvision.imagelab import Imagelab
 
 # Specify path to folder containing the image files in your dataset
 imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
 
 # Automatically check for a predefined list of issues within your dataset
 imagelab.find_issues()
 
 # Produce a neat report of the issues found in your dataset
 imagelab.report()
 ```
 
-CleanVision diagnoses many types of issues, but you can also check for only specific issues.
+2. CleanVision diagnoses many types of issues, but you can also check for only specific issues.
 
 ```python
 issue_types = {"dark": {}, "blurry": {}}
 
 imagelab.find_issues(issue_types=issue_types)
 
 # Produce a report with only the specified issue_types
 imagelab.report(issue_types=issue_types)
 ```
 
+
 ## More resources on how to use CleanVision
 
 - [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
-- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py)
+- [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
+- [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
+- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
+- [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
 The quality of machine learning models hinges on the quality of the data used to train them, but it is hard to manually identify all of the low-quality data in a big dataset. CleanVision helps you automatically identify common types of data issues lurking in image datasets.
 
 This package currently detects issues in the raw images themselves, making it a useful tool for any computer vision
 task such as: classification, segmentation, object detection, pose estimation, keypoint detection, [generative modeling](https://openai.com/research/dall-e-2-pre-training-mitigations), etc.
```

### Comparing `cleanvision-0.1.1/pyproject.toml` & `cleanvision-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cleanvision"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     { name = "Cleanlab Inc.", email = "team@cleanlab.ai" },
 ]
 description = "Find issues in image datasets"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["computer_vision", "cv", "image_data", "issue_detection", "data_quality", "image_quality", "machine_learning", "data_cleaning", "image_deduplication"]
@@ -35,12 +35,16 @@
     "pandas>=1.1.5",
     "tabulate>=0.8.3", # pandas optional dependency for .to_markdown()
     "imagehash>=4.2.0",
     "tqdm>=4.53.0",
     "matplotlib>=3.4"
 ]
 
+[project.optional-dependencies]
+huggingface = ["datasets>=2.7.0"]
+pytorch = ["torchvision>=0.12.0"]
+
 [project.urls]
 "Source" = "https://github.com/cleanlab/cleanvision"
 "Bug Tracker" = "https://github.com/cleanlab/cleanvision/issues"
-#todo add documentation link
+"Documentation" = "https://cleanvision.readthedocs.io/"
```

### Comparing `cleanvision-0.1.1/src/cleanvision/imagelab.py` & `cleanvision-0.2.0/src/cleanvision/imagelab.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,58 +3,80 @@
 The methods in this module should suffice for most use-cases,
 but advanced users can get extra flexibility via the code in other CleanVision modules.
 """
 
 import os
 import pickle
 from typing import List, Dict, Any, Optional, Tuple, TypeVar, Type
+from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
+from PIL import Image
 
+from cleanvision.dataset.utils import build_dataset
 from cleanvision.issue_managers import (
     IssueType,
     IssueManagerFactory,
     ISSUE_MANAGER_REGISTRY,
 )
 from cleanvision.utils.base_issue_manager import IssueManager
 from cleanvision.utils.constants import (
     IMAGE_PROPERTY,
     DUPLICATE,
     IMAGE_PROPERTY_ISSUE_TYPES_LIST,
     DUPLICATE_ISSUE_TYPES_LIST,
     SETS,
 )
 from cleanvision.utils.utils import (
-    get_filepaths,
     deep_update_dict,
     get_is_issue_colname,
     get_score_colname,
     update_df,
 )
 from cleanvision.utils.viz_manager import VizManager
 
+if TYPE_CHECKING:  # pragma: no cover
+    import datasets
+    from torchvision.datasets.vision import VisionDataset
+
 __all__ = ["Imagelab"]
 
 OBJECT_FILENAME = "imagelab.pkl"
 TImagelab = TypeVar("TImagelab", bound="Imagelab")
 
 
 class Imagelab:
-    """A single class to find all types of issues in image datasets. Imagelab detects issues in the raw image files themselves and thus can be useful in most computer vision tasks.
+    """A single class to find all types of issues in image datasets.
+    Imagelab detects issues in any image dataset and thus can be useful in most computer vision tasks including
+    supervised and unsupervised training.
+    Imagelab supports various formats for datasets: local folder containing images, a list of image
+    filepaths, HuggingFace dataset and Torchvision dataset.
+    Specify only one of these arguments: `data_path`, `filepaths`, (`hf_dataset`, `image_key`), `torchvision_dataset`
+
+
 
     Parameters
     ----------
     data_path : str
         Path to image files.
         Imagelab will recursively retrieve all image files from the specified path
 
     filepaths: List[str], optional
         Issue checks will be run on this list of image paths specified in `filepaths`.
-        Specifying only one of `data_path` or `filepaths`.
+
+    hf_dataset: datasets.Dataset
+        Hugging Face dataset with images in PIL format accessible via some key in ``hf_dataset.features``.
+
+    image_key: str
+        Key used to access images within the Hugging Face `dataset.features` object. For many datasets, this key is just called "image".
+        This argument must be specified if you provide a Hugging Face dataset; for other types of dataset this argument has no effect.
+
+    torchvision_dataset: torchvision.datasets.vision.VisionDataset
+        torchvision dataset where each individual  example is a tuple containing exactly one image in PIL format.
 
     Attributes
     ----------
     issues : pd.DataFrame
         Dataframe where each row corresponds to an image and columns specify which issues were detected in this image.
         It has two types of columns for each issue type:
 
@@ -88,47 +110,39 @@
         imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
         imagelab.find_issues()
         imagelab.report()
 
     """
 
     def __init__(
-        self, data_path: Optional[str] = None, filepaths: Optional[List[str]] = None
+        self,
+        data_path: Optional[str] = None,
+        filepaths: Optional[List[str]] = None,
+        hf_dataset: Optional["datasets.Dataset"] = None,
+        image_key: Optional[str] = None,
+        torchvision_dataset: Optional["VisionDataset"] = None,
     ) -> None:
-        self._filepaths = self._get_filepaths(data_path, filepaths)
-        self._num_images: int = len(self._filepaths)
-        if self._num_images == 0:
-            raise ValueError("No images found in the specified path")
+        self._dataset = build_dataset(
+            data_path, filepaths, hf_dataset, image_key, torchvision_dataset
+        )
+        if len(self._dataset) == 0:
+            raise ValueError("No images found in the dataset specified")
         self.info: Dict[str, Any] = {"statistics": {}}
         self.issue_summary: pd.DataFrame = pd.DataFrame(
             columns=["issue_type", "num_images"]
         )
-        self.issues: pd.DataFrame = pd.DataFrame(index=self._filepaths)
+
+        self.issues: pd.DataFrame = pd.DataFrame(index=self._dataset.index)
         self._issue_types: List[str] = []
         self._issue_managers: Dict[str, IssueManager] = {}
+
         # can be loaded from a file later
         self._config: Dict[str, Any] = self._set_default_config()
         self._path = ""
 
-    def _get_filepaths(
-        self, data_path: Optional[str], filepaths: Optional[List[str]]
-    ) -> List[str]:
-        if (data_path is None and filepaths is None) or (
-            data_path is not None and filepaths is not None
-        ):
-            raise ValueError(
-                "Please specify one of data_path or filepaths to check for issues."
-            )
-        filepaths = []
-        if data_path:
-            filepaths = get_filepaths(data_path)
-        elif filepaths:
-            filepaths = filepaths
-        return filepaths
-
     def _set_default_config(self) -> Dict[str, Any]:
         """Sets default values for various config variables used in Imagelab class
         The naming convention for methods is {method_name}_{config_variable_name}
 
         Returns
         -------
         Dict[str, Any]
@@ -247,15 +261,15 @@
         self._set_issue_managers(issue_type_groups)
 
         # find issues
         for issue_type_group, params in issue_type_groups.items():
             issue_manager = self._issue_managers[issue_type_group]
             issue_manager.find_issues(
                 params=params,
-                filepaths=self._filepaths,
+                dataset=self._dataset,
                 imagelab_info=self.info,
                 n_jobs=n_jobs,
             )
 
             # update issues, issue_summary and info
             self._update_issues(issue_manager.issues)
             self._update_issue_summary(issue_manager.summary)
@@ -318,15 +332,15 @@
     ) -> List[str]:
         """Filters issues by max_prevalence in the dataset."""
         issue_summary = self.issue_summary[
             self.issue_summary["issue_type"].isin(issue_types)
         ]
         issue_to_report = []
         for row in issue_summary.itertuples(index=False):
-            if getattr(row, "num_images") / self._num_images < max_prevalence:
+            if getattr(row, "num_images") / len(self._dataset) < max_prevalence:
                 issue_to_report.append(getattr(row, "issue_type"))
             else:
                 print(
                     f"Removing {getattr(row, 'issue_type')} from potential issues in the dataset as it exceeds "
                     f"max_prevalence={max_prevalence} "
                 )
         return issue_to_report
@@ -463,37 +477,44 @@
             else:
                 print(
                     f"\nTop {num_images} {examples_str} with {issue_type} issue in the dataset."
                 )
 
             scores = sorted_df.head(num_images)[get_score_colname(issue_type)]
             titles = [f"score : {x:.4f}" for x in scores]
-            paths = scores.index.tolist()
-            if paths:
+            indices = scores.index.tolist()
+            images = [self._dataset[i] for i in indices]
+            if images:
                 VizManager.individual_images(
-                    filepaths=paths,
+                    images=images,
                     titles=titles,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
                 )
 
         elif viz_name == "image_sets":
-            image_sets = list(self.info[issue_type][SETS][:num_images])
+            image_set_indices = list(self.info[issue_type][SETS][:num_images])
+            image_sets = []
+            for indices in image_set_indices:
+                image_sets.append([self._dataset[index] for index in indices])
 
             sets_str = "sets" if len(image_sets) > 1 else "set"
             if len(image_sets) < num_images:
                 print(
                     f"Found {len(image_sets)} {sets_str} of images with {issue_type} issue in the dataset."
                 )
             else:
                 print(
                     f"\nTop {num_images} {sets_str} of images with {issue_type} issue"
                 )
 
-            title_sets = [[path.split("/")[-1] for path in s] for s in image_sets]
+            title_sets = [
+                [self._dataset.get_name(index) for index in s]
+                for s in image_set_indices
+            ]
 
             if image_sets:
                 VizManager.image_sets(
                     image_sets,
                     title_sets,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
@@ -563,29 +584,43 @@
 
         """
         if issue_types:
             if len(issue_types) == 0:
                 raise ValueError("issue_types list is empty")
             for issue_type in issue_types:
                 self._visualize(issue_type, num_images, cell_size)
+        elif image_files:
+            # todo: write test
+            if len(image_files) == 0:
+                raise ValueError("image_files list is empty.")
+            images = [Image.open(path) for path in image_files]
+            titles = [path.split("/")[-1] for path in image_files]
+            VizManager.individual_images(
+                images,
+                titles,
+                ncols=self._config["visualize_num_images_per_row"],
+                cell_size=cell_size,
+            )
         else:
+            # todo: write test
+            print("Sample images from the dataset")
             if image_files is None:
-                image_files = list(
+                image_indices = list(
                     np.random.choice(
-                        self._filepaths,
-                        min(num_images, self._num_images),
+                        self._dataset.index,
+                        min(
+                            num_images, len(self._dataset)
+                        ),  # in case the len(dataset) < 4
                         replace=False,
                     )
                 )
-            elif len(image_files) == 0:
-                raise ValueError("image_files list is empty.")
-            if image_files:
-                titles = [path.split("/")[-1] for path in image_files]
+                images = [self._dataset[i] for i in image_indices]
+                titles = [self._dataset.get_name(i) for i in image_indices]
                 VizManager.individual_images(
-                    image_files,
+                    images,
                     titles,
                     ncols=self._config["visualize_num_images_per_row"],
                     cell_size=cell_size,
                 )
 
     # Todo: Improve mypy dict typechecking so this does not return any
     def get_stats(self) -> Any:
@@ -657,15 +692,16 @@
         if not os.path.exists(path):
             raise ValueError(f"No folder found at specified path: {path}")
 
         object_file = os.path.join(path, OBJECT_FILENAME)
         with open(object_file, "rb") as f:
             imagelab: TImagelab = pickle.load(f)
 
-        if data_path is not None:
-            filepaths = get_filepaths(data_path)
-            if set(filepaths) != set(imagelab._filepaths):
-                raise ValueError(
-                    "Absolute path of image(s) has changed in the dataset. Cannot load Imagelab."
-                )
+        # todo: use hash for validating
+        # if data_path is not None:
+        #     filepaths = get_filepaths(data_path)
+        #     if set(filepaths) != set(imagelab._filepaths):
+        #         raise ValueError(
+        #             "Absolute path of image(s) has changed in the dataset. Cannot load Imagelab."
+        #         )
         print("Successfully loaded Imagelab")
         return imagelab
```

### Comparing `cleanvision-0.1.1/src/cleanvision/issue_managers/__init__.py` & `cleanvision-0.2.0/src/cleanvision/issue_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/src/cleanvision/issue_managers/duplicate_issue_manager.py` & `cleanvision-0.2.0/src/cleanvision/issue_managers/duplicate_issue_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import hashlib
 import multiprocessing
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import imagehash
 import numpy as np
 import pandas as pd
 from PIL import Image
 from tqdm import tqdm
 
+from cleanvision.dataset.base_dataset import Dataset
 from cleanvision.issue_managers import register_issue_manager, IssueType
 from cleanvision.utils.base_issue_manager import IssueManager
 from cleanvision.utils.constants import SETS, DUPLICATE, MAX_PROCS
 from cleanvision.utils.utils import get_max_n_jobs, get_is_issue_colname
 
 
 def get_hash(image: Image, params: Dict[str, Any]) -> str:
@@ -24,29 +25,28 @@
     elif hash_type == "phash":
         return str(imagehash.phash(image, hash_size=hash_size))
     else:
         raise ValueError("Hash type not supported")
 
 
 def compute_hash(
-    path: str, to_compute: List[str], params: Dict[str, Any]
-) -> Dict[str, Any]:
-    image = Image.open(path)
-    result = {}
-    result["path"] = path
+    index: int,
+    dataset: Dataset,
+    to_compute: List[str],
+    params: Dict[str, Any],
+) -> Dict[str, Union[str, int]]:
+    image = dataset[index]
+    result: Dict[str, Union[str, int]] = {"index": index}
     for issue_type in to_compute:
         result[issue_type] = get_hash(image, params[issue_type])
     return result
 
 
-def compute_hash_wrapper(arg: Dict[str, Any]) -> Dict[str, Any]:
-    path = arg["path"]
-    to_compute = arg["to_compute"]
-    params = arg["params"]
-    return compute_hash(path, to_compute, params)
+def compute_hash_wrapper(args: Dict[str, Any]) -> Dict[str, Union[str, int]]:
+    return compute_hash(**args)
 
 
 @register_issue_manager(DUPLICATE)
 class DuplicateIssueManager(IssueManager):
     issue_name: str = DUPLICATE
     visualization: str = "image_sets"
 
@@ -93,65 +93,73 @@
             to_compute.append(IssueType.NEAR_DUPLICATES.value)
         return to_compute
 
     def find_issues(
         self,
         *,
         params: Optional[Dict[str, Any]] = None,
-        filepaths: Optional[List[str]] = None,
+        dataset: Optional[Dataset] = None,
         imagelab_info: Optional[Dict[str, Any]] = None,
         n_jobs: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         super().find_issues(**kwargs)
         assert params is not None
         assert imagelab_info is not None
-        assert filepaths is not None
+        assert dataset is not None
 
         self.issue_types = list(params.keys())
         self.update_params(params)
 
         to_compute = self._get_issue_types_to_compute(self.issue_types, imagelab_info)
         issue_type_hash_mapping: Dict[str, Any] = {
             issue_type: {} for issue_type in to_compute
         }
 
         if n_jobs is None:
             n_jobs = get_max_n_jobs()
 
-        results: List[Any] = []
+        results: List[Dict[str, Union[str, int]]] = []
         if n_jobs == 1:
-            for path in tqdm(filepaths):
-                results.append(compute_hash(path, to_compute, self.params))
+            for idx in tqdm(dataset.index):
+                results.append(compute_hash(idx, dataset, to_compute, self.params))
         else:
             args = [
-                {"path": path, "to_compute": to_compute, "params": self.params}
-                for path in filepaths
+                {
+                    "index": idx,
+                    "dataset": dataset,
+                    "to_compute": to_compute,
+                    "params": self.params,
+                }
+                for idx in dataset.index
             ]
             chunksize = max(1, len(args) // MAX_PROCS)
             with multiprocessing.Pool(n_jobs) as p:
                 results = list(
                     tqdm(
                         p.imap_unordered(
                             compute_hash_wrapper, args, chunksize=chunksize
                         ),
-                        total=len(filepaths),
+                        total=len(dataset),
                     )
                 )
-            results = sorted(results, key=lambda r: r["path"])  # type:ignore
+
+            results = sorted(results, key=lambda r: r["index"])
 
         for result in results:
             for issue_type in to_compute:
                 hash_str = result[issue_type]
                 if hash_str in issue_type_hash_mapping[issue_type]:
-                    issue_type_hash_mapping[issue_type][hash_str].append(result["path"])
+                    issue_type_hash_mapping[issue_type][hash_str].append(
+                        result["index"]
+                    )
                 else:
-                    issue_type_hash_mapping[issue_type][hash_str] = [result["path"]]
+                    issue_type_hash_mapping[issue_type][hash_str] = [result["index"]]
 
-        self.issues = pd.DataFrame(index=filepaths)
+        self.issues = pd.DataFrame(index=dataset.index)
         self._update_info(self.issue_types, issue_type_hash_mapping, imagelab_info)
         self._update_issues()
         self._update_summary()
 
         return
 
     def _update_summary(self) -> None:
```

### Comparing `cleanvision-0.1.1/src/cleanvision/issue_managers/image_property.py` & `cleanvision-0.2.0/src/cleanvision/issue_managers/image_property.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/src/cleanvision/issue_managers/image_property_issue_manager.py` & `cleanvision-0.2.0/src/cleanvision/issue_managers/image_property_issue_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import multiprocessing
-from typing import Dict, Any, List, Set, Optional
+from typing import Dict, Any, List, Set, Optional, Union
 
 import pandas as pd
-from PIL import Image
 from tqdm import tqdm
 
+from cleanvision.dataset.base_dataset import Dataset
 from cleanvision.issue_managers import register_issue_manager, IssueType
 from cleanvision.issue_managers.image_property import (
     BrightnessProperty,
     AspectRatioProperty,
     EntropyProperty,
     BlurrinessProperty,
     ColorSpaceProperty,
@@ -25,29 +25,28 @@
     get_is_issue_colname,
     update_df,
     get_score_colname,
 )
 
 
 def compute_scores(
-    path: str, to_compute: List[str], properties: Dict[str, ImageProperty]
-) -> Dict[str, Any]:
-    image = Image.open(path)
-    results: Dict[str, Any] = {}
-    results["path"] = path
+    index: int,
+    dataset: Dataset,
+    to_compute: List[str],
+    image_properties: Dict[str, ImageProperty],
+) -> Dict[str, Union[str, int, float]]:
+    image = dataset[index]
+    result: Dict[str, Union[int, str, float]] = {"index": index}
     for issue_type in to_compute:
-        results = {**results, **properties[issue_type].calculate(image)}
-    return results
+        result = {**result, **image_properties[issue_type].calculate(image)}
+    return result
 
 
-def compute_scores_wrapper(arg: Dict[str, Any]) -> Dict[str, Any]:
-    to_compute = arg["to_compute"]
-    path = arg["path"]
-    properties = arg["image_properties"]
-    return compute_scores(path, to_compute, properties)
+def compute_scores_wrapper(args: Dict[str, Any]) -> Dict[str, Union[float, str, int]]:
+    return compute_scores(**args)
 
 
 # Combined all issues which are to be detected using image properties under one class to save time on loading image
 @register_issue_manager(IMAGE_PROPERTY)
 class ImagePropertyIssueManager(IssueManager):
     issue_name: str = IMAGE_PROPERTY
     visualization: str = "individual_images"
@@ -114,69 +113,75 @@
             additional_set.append(IssueType.DARK.value)
         return additional_set
 
     def find_issues(
         self,
         *,
         params: Optional[Dict[str, Any]] = None,
-        filepaths: Optional[List[str]] = None,
+        dataset: Optional[Dataset] = None,
         imagelab_info: Optional[Dict[str, Any]] = None,
         n_jobs: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         super().find_issues(**kwargs)
         assert params is not None
         assert imagelab_info is not None
-        assert filepaths is not None
+        assert dataset is not None
 
         self.issue_types = list(params.keys())
-        self.issues = pd.DataFrame(index=filepaths)
+        self.issues = pd.DataFrame(index=dataset.index)
         additional_set = self._get_additional_to_compute_set(self.issue_types)
         self.issue_types = self.issue_types + additional_set
 
         self.update_params(params)
 
-        agg_computations = self._get_prev_computations(filepaths, imagelab_info)
+        agg_computations = pd.DataFrame(index=dataset.index)
+        agg_computations = self._add_prev_computations(agg_computations, imagelab_info)
+
         defer_set = self._get_defer_set(self.issue_types, agg_computations)
 
         to_be_computed = list(set(self.issue_types).difference(defer_set))
-        new_computations = pd.DataFrame(index=filepaths)
+
+        new_computations = pd.DataFrame(index=dataset.index)
         if to_be_computed:
             if n_jobs is None:
                 n_jobs = get_max_n_jobs()
 
-            results: List[Any] = []
+            results: List[Dict[str, Union[int, float, str]]] = []
             if n_jobs == 1:
-                for path in tqdm(filepaths):
+                for idx in tqdm(dataset.index):
                     results.append(
-                        compute_scores(path, to_be_computed, self.image_properties)
+                        compute_scores(
+                            idx, dataset, to_be_computed, self.image_properties
+                        )
                     )
             else:
                 args = [
                     {
+                        "index": idx,
+                        "dataset": dataset,
                         "to_compute": to_be_computed,
-                        "path": path,
                         "image_properties": self.image_properties,
                     }
-                    for i, path in enumerate(filepaths)
+                    for idx in dataset.index
                 ]
                 chunksize = max(1, len(args) // MAX_PROCS)
                 with multiprocessing.Pool(n_jobs) as p:
                     results = list(
                         tqdm(
                             p.imap_unordered(
                                 compute_scores_wrapper, args, chunksize=chunksize
                             ),
-                            total=len(filepaths),
+                            total=len(dataset),
                         )
                     )
 
-                results = sorted(results, key=lambda r: r["path"])  # type:ignore
+                results = sorted(results, key=lambda r: r["index"])
 
-            new_computations = self.aggregate(results)
+            new_computations = self._aggregate(results)
 
         agg_computations = update_df(agg_computations, new_computations)
 
         ordered_issue_types = self._get_dependency_sorted(self.issue_types)
 
         self.update_issues(agg_computations, ordered_issue_types)
         self.update_info(agg_computations)
@@ -247,28 +252,27 @@
 
             is_issue = self.image_properties[issue_type].mark_issue(
                 issue_scores, self.params[issue_type].get("threshold"), issue_type
             )
             self.issues = self.issues.join(issue_scores)
             self.issues = self.issues.join(is_issue)
 
-    def _get_prev_computations(
-        self, filepaths: List[str], info: Dict[str, Any]
+    def _add_prev_computations(
+        self, agg_computations: pd.DataFrame, info: Dict[str, Any]
     ) -> pd.DataFrame:
-        agg_computations = pd.DataFrame(index=filepaths)
         for key in info.keys():
             if key in IMAGE_PROPERTY_ISSUE_TYPES_LIST + ["statistics"]:
                 for col in info[key]:
                     if col not in agg_computations:
                         agg_computations = agg_computations.join(info[key][col])
         return agg_computations
 
-    def aggregate(self, results: List[Dict[str, Any]]) -> pd.DataFrame:
+    def _aggregate(self, results: List[Dict[str, Any]]) -> pd.DataFrame:
         agg_computations = pd.DataFrame(results)
-        agg_computations = agg_computations.set_index("path")
+        agg_computations = agg_computations.set_index("index")
         return agg_computations
 
     def update_info(self, agg_computations: pd.DataFrame) -> None:
         """Updates `self.info` using computed properties
 
         Parameters
         ----------
```

### Comparing `cleanvision-0.1.1/src/cleanvision/utils/base_issue_manager.py` & `cleanvision-0.2.0/src/cleanvision/utils/base_issue_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import ABC, abstractmethod
-from typing import Dict, Any, List
+from typing import Dict, Any
 
 import pandas as pd
 
+from cleanvision.dataset.base_dataset import Dataset
+
 
 class IssueManager(ABC):
     """Base class for managing data issues of a particular type in Imagelab."""
 
     visualization: str
     issue_name: str
 
@@ -23,15 +25,15 @@
         class_name = self.__class__.__name__
         return class_name
 
     @staticmethod
     def check_params(**kwargs: Any) -> None:
         allowed_kwargs: Dict[str, Any] = {
             "params": Dict[str, Any],
-            "filepaths": List[str],
+            "dataset": Dataset,
             "imagelab_info": Dict[str, Any],
             "n_jobs": int,
         }
 
         for name, value in kwargs.items():
             if name not in allowed_kwargs:
                 raise ValueError(f"{name} is not a valid keyword argument.")
```

### Comparing `cleanvision-0.1.1/src/cleanvision/utils/constants.py` & `cleanvision-0.2.0/src/cleanvision/utils/constants.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/src/cleanvision/utils/utils.py` & `cleanvision-0.2.0/src/cleanvision/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     Returns
     -------
     List[str]
         Sorted list of image filepaths, note that all paths in this list are absolute paths
     """
 
-    abs_dir_path = os.path.abspath(dir_path)
+    abs_dir_path = os.path.abspath(os.path.expanduser(dir_path))
     print(f"Reading images from {abs_dir_path}")
     filepaths = []
     for ext in IMAGE_FILE_EXTENSIONS:
         filetype_images = glob.glob(
             os.path.join(abs_dir_path, "**", ext), recursive=True
         )
         if len(filetype_images) == 0:
```

### Comparing `cleanvision-0.1.1/src/cleanvision.egg-info/PKG-INFO` & `cleanvision-0.2.0/src/cleanvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanvision
-Version: 0.1.1
+Version: 0.2.0
 Summary: Find issues in image datasets
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -663,14 +663,15 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Source, https://github.com/cleanlab/cleanvision
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanvision/issues
+Project-URL: Documentation, https://cleanvision.readthedocs.io/
 Keywords: computer_vision,cv,image_data,issue_detection,data_quality,image_quality,machine_learning,data_cleaning,image_deduplication
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -680,14 +681,16 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: huggingface
+Provides-Extra: pytorch
 License-File: LICENSE
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanvision_logo_open_source_transparent.png" width=50% height=50%>
 </p>
 
 <img width="1200" alt="Screen Shot 2023-03-10 at 10 23 33 AM" src="https://user-images.githubusercontent.com/10901697/224394144-bb0e1c85-6851-4828-bcd2-4ed234270a78.png">
@@ -697,61 +700,67 @@
 CleanVision is super simple -- run the same couple lines of Python code to audit any image dataset!
 
 [![Read the Docs](https://readthedocs.org/projects/cleanvision/badge/?version=latest)](https://cleanvision.readthedocs.io/en/latest/)
 [![pypi](https://img.shields.io/pypi/v/cleanvision?color=blue)](https://pypi.org/pypi/cleanvision/)
 [![os](https://img.shields.io/badge/platform-noarch-lightgrey)](https://pypi.org/pypi/cleanvision/)
 [![py\_versions](https://img.shields.io/badge/python-3.7%2B-blue)](https://pypi.org/pypi/cleanvision/)
 [![codecov](https://codecov.io/github/cleanlab/cleanvision/branch/main/graph/badge.svg?token=y1N6MluN9H)](https://codecov.io/gh/cleanlab/cleanvision)
+[![Slack Community](https://img.shields.io/static/v1?logo=slack&style=flat&color=white&label=slack&message=community)](https://cleanlab.ai/slack)
+[![Twitter](https://img.shields.io/twitter/follow/CleanlabAI?style=social)](https://twitter.com/CleanlabAI)
+[![Cleanlab Studio](https://raw.githubusercontent.com/cleanlab/assets/master/shields/cl-studio-shield.svg)](https://cleanlab.ai/studio/?utm_source=github&utm_medium=readme&utm_campaign=clostostudio)
 
 ## Installation
-
 ```shell
 pip install cleanvision
 ```
 
 ## Quickstart
 
 Download an example dataset (optional). Or just use any collection of image files you have.
 
 ```shell
 wget -nc 'https://cleanlab-public.s3.amazonaws.com/CleanVision/image_files.zip'
 ```
 
-Run CleanVision to audit the images.
+1. Run CleanVision to audit the images.
 
 ```python
 from cleanvision.imagelab import Imagelab
 
 # Specify path to folder containing the image files in your dataset
 imagelab = Imagelab(data_path="FOLDER_WITH_IMAGES/")
 
 # Automatically check for a predefined list of issues within your dataset
 imagelab.find_issues()
 
 # Produce a neat report of the issues found in your dataset
 imagelab.report()
 ```
 
-CleanVision diagnoses many types of issues, but you can also check for only specific issues.
+2. CleanVision diagnoses many types of issues, but you can also check for only specific issues.
 
 ```python
 issue_types = {"dark": {}, "blurry": {}}
 
 imagelab.find_issues(issue_types=issue_types)
 
 # Produce a report with only the specified issue_types
 imagelab.report(issue_types=issue_types)
 ```
 
+
 ## More resources on how to use CleanVision
 
 - [Tutorial notebook](https://github.com/cleanlab/cleanvision-examples/blob/main/tutorial.ipynb)
-- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py)
+- [Notebook for running CleanVision on a HuggingFace Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/huggingface_dataset.ipynb)
+- [Notebook for running CleanVision on a Torchvision Dataset](https://github.com/cleanlab/cleanvision-examples/blob/main/torchvision_dataset.ipynb)
+- [Example script](https://github.com/cleanlab/cleanvision/blob/main/examples/run.py) that can be run with: `python examples/run.py --path <FOLDER_WITH_IMAGES>`
 - [Additional example notebooks](https://github.com/cleanlab/cleanvision-examples)
 - [Documentation](https://cleanvision.readthedocs.io/)
+- [Blog Post](https://cleanlab.ai/blog/cleanvision/)
 
 ## *Clean* your data for better Computer *Vision*
 
 The quality of machine learning models hinges on the quality of the data used to train them, but it is hard to manually identify all of the low-quality data in a big dataset. CleanVision helps you automatically identify common types of data issues lurking in image datasets.
 
 This package currently detects issues in the raw images themselves, making it a useful tool for any computer vision
 task such as: classification, segmentation, object detection, pose estimation, keypoint detection, [generative modeling](https://openai.com/research/dall-e-2-pre-training-mitigations), etc.
```

### Comparing `cleanvision-0.1.1/tests/test_duplicate_issue_manager.py` & `cleanvision-0.2.0/tests/test_duplicate_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/tests/test_image_property_helpers.py` & `cleanvision-0.2.0/tests/test_image_property_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/tests/test_image_property_issue_manager.py` & `cleanvision-0.2.0/tests/test_image_property_issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanvision-0.1.1/tests/test_run.py` & `cleanvision-0.2.0/tests/test_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,25 @@
-# to suppress plt.show()
-import matplotlib.pyplot as plt
-import numpy as np
+import os
+
 import pytest
-from PIL import Image
+import torchvision
+from datasets import load_dataset
 
+from cleanvision.dataset.folder_dataset import FolderDataset
 from cleanvision.imagelab import Imagelab
 from cleanvision.issue_managers.image_property import BrightnessProperty
 from cleanvision.issue_managers.image_property_issue_manager import (
     compute_scores_wrapper,
 )
 from examples.custom_issue_manager import CustomIssueManager
 
 
-def generate_image(arr=None):
-    if arr is None:
-        arr = np.random.randint(low=0, high=256, size=(300, 300, 3), dtype=np.uint8)
-    img = Image.fromarray(arr, mode="RGB")
-    return img
-
-
-@pytest.fixture(scope="session")
-def generate_single_image_file(tmpdir_factory, img_name="img.png", arr=None):
-    """Generates a single temporary image for testing"""
-    img = generate_image(arr)
-    fn = tmpdir_factory.mktemp("data").join(img_name)
-    img.save(str(fn))
-    return str(fn)
-
-
-@pytest.fixture(scope="session")
-def generate_n_image_files(tmpdir_factory, n=40):
-    """Generates n temporary images for testing and returns dir of images"""
-    filename_list = []
-    tmp_image_dir = tmpdir_factory.mktemp("data")
-    for i in range(n):
-        img = generate_image()
-        img_name = f"{i}.png"
-        fn = tmp_image_dir.join(img_name)
-        img.save(str(fn))
-        filename_list.append(str(fn))
-    return str(tmp_image_dir)
-
-
-@pytest.mark.usefixtures("generate_n_image_files")
-def test_example1(capsys, monkeypatch, generate_n_image_files):
-    monkeypatch.setattr(plt, "show", lambda: None)
-    imagelab = Imagelab(data_path=generate_n_image_files)  # initialize imagelab
+@pytest.mark.usefixtures("set_plt_show")
+def test_example1(capsys, generate_local_dataset):
+    imagelab = Imagelab(data_path=generate_local_dataset)  # initialize imagelab
     imagelab.list_default_issue_types()  # list default checks
 
     # ==== Test list_default_issue_types() lists all default isssue types====
     DEFAULT_ISSUE_TYPES = [
         "dark",
         "light",
         "odd_aspect_ratio",
@@ -94,43 +64,41 @@
 
     # === Test miscellaneous extra information about datasset
     assert set(imagelab.info.keys()) == set(DEFAULT_ISSUE_TYPES + ["statistics"])
     for key in ["color_space", "entropy", "brightness", "blurriness", "aspect_ratio"]:
         assert key in list(imagelab.info["statistics"].keys())
 
 
-@pytest.mark.usefixtures("generate_n_image_files")
-def test_example2(monkeypatch, generate_n_image_files):
-    monkeypatch.setattr(plt, "show", lambda: None)
-    imagelab = Imagelab(data_path=generate_n_image_files)  # initialize imagelab
+@pytest.mark.usefixtures("set_plt_show")
+def test_example2(generate_local_dataset, tmp_path):
+    imagelab = Imagelab(data_path=generate_local_dataset)  # initialize imagelab
     issue_types = {"near_duplicates": {}}
     imagelab.find_issues(issue_types)
     imagelab.report()
-    save_folder = generate_n_image_files + "/T_save_folder/"
+    save_folder = tmp_path / "T_save_folder/"
 
     imagelab.save(
         save_folder
     )  # optional, just included to show how to save/load this as a file
 
     # Check for additional types of issues using existing Imagelab
-    imagelab = Imagelab.load(save_folder, generate_n_image_files)
+    imagelab = Imagelab.load(save_folder, generate_local_dataset)
     issue_types = {"light": {}, "low_information": {}}
     imagelab.find_issues(issue_types)
     imagelab.report()
 
     # Check for an issue with a different threshold
     issue_types = {"dark": {"threshold": 0.2}}
     imagelab.find_issues(issue_types)
     imagelab.report(issue_types=issue_types.keys())  # report only specific issues
 
 
-@pytest.mark.usefixtures("generate_n_image_files")
-def test_example3(monkeypatch, generate_n_image_files):
-    monkeypatch.setattr(plt, "show", lambda: None)
-    imagelab = Imagelab(data_path=generate_n_image_files)
+@pytest.mark.usefixtures("set_plt_show")
+def test_example3(generate_local_dataset):
+    imagelab = Imagelab(data_path=generate_local_dataset)
     imagelab.find_issues()
     imagelab.report(["near_duplicates"])
 
     issue_types = {"near_duplicates": {"hash_type": "phash"}}
     imagelab.find_issues(issue_types)
     imagelab.report(issue_types=issue_types.keys())
 
@@ -143,54 +111,100 @@
     # Find top examples suffering from issues that are not present in more than 1% of the dataset
     imagelab.report(max_prevalence=0.01)
 
     # Increase cell_size in the grid
     imagelab.visualize(issue_types=["light"], num_images=8, cell_size=(3, 3))
 
 
-@pytest.mark.usefixtures("generate_n_image_files")
-def test_example4(monkeypatch, generate_n_image_files):
-    monkeypatch.setattr(plt, "show", lambda: None)
-    imagelab = Imagelab(data_path=generate_n_image_files)
+@pytest.mark.usefixtures("set_plt_show")
+def test_example4(generate_local_dataset):
+    imagelab = Imagelab(data_path=generate_local_dataset)
     issue_name = CustomIssueManager.issue_name
     imagelab.list_possible_issue_types()
 
     issue_types = {issue_name: {}}
     imagelab.find_issues(issue_types)  # check for custom issue type
 
     imagelab.find_issues()  # also check for default issue types
     imagelab.report()
 
 
-def test_jobs(monkeypatch, generate_n_image_files):
-    monkeypatch.setattr(plt, "show", lambda: None)
-    imagelab = Imagelab(data_path=generate_n_image_files)
+@pytest.mark.usefixtures("set_plt_show")
+def test_jobs(generate_local_dataset):
+    imagelab = Imagelab(data_path=generate_local_dataset)
     imagelab.find_issues(n_jobs=1)
 
 
-@pytest.mark.usefixtures("generate_single_image_file")
 def test_compute_scores(generate_single_image_file):
+    dataset = FolderDataset(filepaths=[generate_single_image_file])
     image_properties = {
         "dark": BrightnessProperty("dark"),
         "light": BrightnessProperty("light"),
     }
     args = {
         "to_compute": ["dark", "light"],
-        "path": generate_single_image_file,
+        "index": generate_single_image_file,
+        "dataset": dataset,
         "image_properties": image_properties,
     }
     _ = compute_scores_wrapper(args)
 
 
-@pytest.mark.usefixtures("generate_n_image_files")
-def test_example5(monkeypatch, generate_n_image_files):
-    monkeypatch.setattr(plt, "show", lambda: None)
-    imagelab = Imagelab(data_path=generate_n_image_files)
+@pytest.mark.usefixtures("set_plt_show")
+def test_example5(generate_local_dataset):
+    imagelab = Imagelab(data_path=generate_local_dataset)
     imagelab.find_issues({"blurry": {}})
     imagelab.find_issues({"dark": {}})
     imagelab.report()
     # Also test the reverse direction:
     # TODO: this direction maybe can be made faster since blurry-check depends on dark-score
-    imagelab = Imagelab(data_path=generate_n_image_files)
+    imagelab = Imagelab(data_path=generate_local_dataset)
     imagelab.find_issues({"dark": {}})
     imagelab.find_issues({"blurry": {}})
     imagelab.report()
+
+
+@pytest.mark.usefixtures("set_plt_show")
+def test_hf_dataset_run(generate_local_dataset, n_classes, images_per_class):
+    hf_dataset = load_dataset(
+        "imagefolder", data_dir=generate_local_dataset, split="train"
+    )
+    imagelab = Imagelab(hf_dataset=hf_dataset, image_key="image")
+    imagelab.find_issues()
+    imagelab.report()
+    assert len(imagelab.issues.columns) == 14
+    assert len(imagelab.issues) == n_classes * images_per_class
+
+
+@pytest.mark.usefixtures("set_plt_show")
+def test_torch_dataset_run(generate_local_dataset, n_classes, images_per_class):
+    torch_ds = torchvision.datasets.ImageFolder(root=generate_local_dataset)
+    imagelab = Imagelab(torchvision_dataset=torch_ds)
+    imagelab.find_issues()
+    imagelab.report()
+    assert len(imagelab.issues.columns) == 14
+    assert len(imagelab.issues) == n_classes * images_per_class
+
+
+@pytest.mark.usefixtures("set_plt_show")
+def test_visualize_sample_images(generate_local_dataset):
+    imagelab = Imagelab(data_path=generate_local_dataset)
+    imagelab.visualize()
+
+
+@pytest.mark.usefixtures("set_plt_show")
+def test_visualize_given_imagefiles(generate_local_dataset):
+    imagelab = Imagelab(data_path=generate_local_dataset)
+    files = os.listdir(generate_local_dataset / "class_0")
+    filepaths = [os.path.join(generate_local_dataset / "class_0", f) for f in files]
+    imagelab.visualize(image_files=filepaths)
+
+
+@pytest.mark.usefixtures("set_plt_show")
+def test_filepath_dataset_run(generate_local_dataset, images_per_class):
+    files = os.listdir(generate_local_dataset / "class_0")
+    filepaths = [os.path.join(generate_local_dataset / "class_0", f) for f in files]
+    imagelab = Imagelab(filepaths=filepaths)
+    imagelab.find_issues()
+    imagelab.report()
+    assert len(imagelab.issues.columns) == 14
+    assert len(imagelab.issues) == images_per_class
```

### Comparing `cleanvision-0.1.1/tests/test_utils.py` & `cleanvision-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

