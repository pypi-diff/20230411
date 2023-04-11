# Comparing `tmp/heartfelt_tools-1.7.0.tar.gz` & `tmp/heartfelt_tools-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartfelt_tools-1.7.0.tar", max compression
+gzip compressed data, was "heartfelt_tools-1.8.0.tar", max compression
```

## Comparing `heartfelt_tools-1.7.0.tar` & `heartfelt_tools-1.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2022-10-21 01:09:12.000000 heartfelt_tools-1.7.0/LICENSE
--rw-r--r--   0        0        0     7303 2023-02-09 01:30:00.000000 heartfelt_tools-1.7.0/README.md
--rw-r--r--   0        0        0        0 2023-02-12 21:09:30.000000 heartfelt_tools-1.7.0/database_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/datastores/__init__.py
--rw-r--r--   0        0        0      938 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/datastores/records.py
--rw-r--r--   0        0        0     2520 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/datastores/signals.py
--rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/errors.py
--rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/__init__.py
--rw-r--r--   0        0        0      470 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/data.py
--rw-r--r--   0        0        0      224 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/utils.py
--rw-r--r--   0        0        0     6945 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/wfdb.py
--rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/__init__.py
--rw-r--r--   0        0        0     1228 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/cardiac.py
--rw-r--r--   0        0        0     2811 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/detect.py
--rw-r--r--   0        0        0     4765 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/metrics.py
--rw-r--r--   0        0        0     1859 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/modify.py
--rw-r--r--   0        0        0     5175 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/utils.py
--rw-r--r--   0        0        0    10403 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/DataEvaluator.py
--rw-r--r--   0        0        0     3080 2023-02-09 01:25:56.000000 heartfelt_tools-1.7.0/database_tools/tools/DataLocator.py
--rw-r--r--   0        0        0       82 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/__init__.py
--rw-r--r--   0        0        0    12151 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/dataset.py
--rw-r--r--   0        0        0     6884 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/records.py
--rw-r--r--   0        0        0      953 2023-04-09 21:24:33.784095 heartfelt_tools-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 heartfelt_tools-1.7.0/setup.py
--rw-r--r--   0        0        0     8342 1970-01-01 00:00:00.000000 heartfelt_tools-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-21 01:09:12.000000 heartfelt_tools-1.8.0/LICENSE
+-rw-r--r--   0        0        0     7303 2023-02-09 01:30:00.000000 heartfelt_tools-1.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-12 21:09:30.000000 heartfelt_tools-1.8.0/database_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/datastores/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/datastores/records.py
+-rw-r--r--   0        0        0     2520 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/datastores/signals.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/errors.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/io/__init__.py
+-rw-r--r--   0        0        0      470 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/io/data.py
+-rw-r--r--   0        0        0      224 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/io/utils.py
+-rw-r--r--   0        0        0     7102 2023-04-11 19:14:23.594087 heartfelt_tools-1.8.0/database_tools/io/wfdb.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/processing/__init__.py
+-rw-r--r--   0        0        0     1228 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/processing/cardiac.py
+-rw-r--r--   0        0        0     2811 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/processing/detect.py
+-rw-r--r--   0        0        0     4765 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/processing/metrics.py
+-rw-r--r--   0        0        0     1859 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/processing/modify.py
+-rw-r--r--   0        0        0     5175 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/processing/utils.py
+-rw-r--r--   0        0        0    10403 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/tools/DataEvaluator.py
+-rw-r--r--   0        0        0     3080 2023-02-09 01:25:56.000000 heartfelt_tools-1.8.0/database_tools/tools/DataLocator.py
+-rw-r--r--   0        0        0       82 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/tools/__init__.py
+-rw-r--r--   0        0        0    12151 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/tools/dataset.py
+-rw-r--r--   0        0        0     6884 2023-04-09 21:23:36.811381 heartfelt_tools-1.8.0/database_tools/tools/records.py
+-rw-r--r--   0        0        0      953 2023-04-11 19:15:44.707317 heartfelt_tools-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 heartfelt_tools-1.8.0/setup.py
+-rw-r--r--   0        0        0     8342 1970-01-01 00:00:00.000000 heartfelt_tools-1.8.0/PKG-INFO
```

### Comparing `heartfelt_tools-1.7.0/LICENSE` & `heartfelt_tools-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/README.md` & `heartfelt_tools-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/datastores/records.py` & `heartfelt_tools-1.8.0/database_tools/datastores/records.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/datastores/signals.py` & `heartfelt_tools-1.8.0/database_tools/datastores/signals.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/io/wfdb.py` & `heartfelt_tools-1.8.0/database_tools/io/wfdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,36 +5,40 @@
 import logging
 import requests
 import numpy as np
 import pandas as pd
 from typing import Union, List
 from alive_progress import alive_bar
 
-logging.basicConfig(
-     filename=f'{__name__}.log',
-     format= '[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
-     datefmt='%H:%M:%S'
-)
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
+try:
+    logging.basicConfig(
+        filename=f'{__name__}.log',
+        format= '[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
+        datefmt='%H:%M:%S'
+    )
+    logger = logging.getLogger(__name__)
+    logger.setLevel(logging.INFO)
+    LOG = True
+except OSError:
+    LOG = False
 
 MIMIC_DIR = 'mimic3wdb/1.0/'
 
 def generate_record_paths(name: str = None, shuffle: bool = True) -> str:
     if name is None:
         rec_dir = MIMIC_DIR + 'RECORDS'
     elif name == 'adults':
         rec_dir = MIMIC_DIR + 'RECORDS-adults'
     elif name == 'neonates':
         rec_dir = MIMIC_DIR + 'RECORDS-neonates'
     r = requests.get('https://physionet.org/files/' + rec_dir, stream=True)
     records = list(pd.read_csv(io.BytesIO(r.content), names=['records'])['records'])
     if shuffle:
         random.shuffle(records)
-    logger.info(f'Successfuly got records file from {rec_dir}')
+    if LOG: logger.info(f'Successfuly got records file from {rec_dir}')
     for path in records:
         yield path[:-1]  # remove trailing /
 
 def get_header_record(path: str, record_type: str) -> Union[wfdb.Record, wfdb.MultiRecord]:
     """Get data header or layout header record from MIMIC-III Waveforms database.
 
     Args:
@@ -51,38 +55,38 @@
         pn_dir = pn_dir.rsplit('/', 1)[0] if '_' in pn_dir else pn_dir  # remove file name from path if there
         hea_name = path.split('/')[-1]
     else:
         raise ValueError('record_type must be one of [\'layout\', \'data\']')
 
     try:
         hea = wfdb.rdheader(pn_dir=pn_dir, record_name=hea_name)
-        logger.info(f'Successfully got {record_type} record {hea_name}')
+        if LOG: logger.info(f'Successfully got {record_type} record {hea_name}')
         return hea
     except Exception as e:
-        logger.info(f'Failed to get {record_type} record {path} due to {e}')
+        if LOG: logger.info(f'Failed to get {record_type} record {path} due to {e}')
 
 def header_has_signals(hea: wfdb.Record, signals: List[str]) -> bool:
     """Check if a header record contains specified signals.
 
     Args:
         hea (wfdb.Record): Header file as wfdb.Record object.
         signals (List[str]): List of signals.
 
     Returns:
         bool: True if the record contains ALL signals provided.
     """
     try:
         if set(signals).difference(set(hea.sig_name)) == set():
-            logger.info(f'Record {hea.record_name}.hea contains {signals}')
+            if LOG: logger.info(f'Record {hea.record_name}.hea contains {signals}')
             return True
         else:
-            logger.info(f'Record {hea.record_name}.hea does not contain {signals}')
+            if LOG: logger.info(f'Record {hea.record_name}.hea does not contain {signals}')
             return False
     except TypeError:
-        logger.info(f'Error getting {signals} from {hea.record_name}.hea')
+        if LOG: logger.info(f'Error getting {signals} from {hea.record_name}.hea')
         return False
 
 def get_data_record(path: str, record_type: str = 'waveforms') -> wfdb.Record:
     """Get data record from MIMIC-III Waveforms database.
 
     Args:
         path (str): Path to data file.
@@ -97,18 +101,18 @@
     elif record_type == 'numerics':
         pn_dir = MIMIC_DIR + path
         rcd_name = path.split('/')[-1] + 'n'
     else:
         raise ValueError('record_type must be one of [\'waveforms\', \'numerics\']')
     try:
         rcd = wfdb.rdrecord(pn_dir=pn_dir, record_name=rcd_name)
-        logger.info(f'Successfully got {record_type} record {rcd_name}')
+        if LOG: logger.info(f'Successfully got {record_type} record {rcd_name}')
         return rcd
     except Exception as e:
-        logger.info(f'Failed to get {record_type} record {path} due to {e}')
+        if LOG: logger.info(f'Failed to get {record_type} record {path} due to {e}')
 
 def get_signal(rec: wfdb.Record, sig: str, errors: str = 'ignore') -> np.ndarray:
     """Extract signal data from a record.
 
     Args:
         rec (wfdb.Record): MIMIC-III record.
         sig (str): Signal name. One of ['PLETH', 'ABP'].
@@ -116,19 +120,19 @@
 
     Returns:
         data (np.ndarray): 1D signal data or NoneType if errors is 'ignore'.
     """
     try:
         s = rec.sig_name  # list of signals in record
         data = rec.p_signal[:, s.index(sig)].astype(np.float64)
-        logger.info(f'Successfully extracted {sig} from {rec.record_name}')
+        if LOG: logger.info(f'Successfully extracted {sig} from {rec.record_name}')
         return data
     except Exception as e:
         if errors == 'ignore':
-            logger.info(f'Failed to extract {sig} from {rec.record_name} due to {e}')
+            if LOG: logger.info(f'Failed to extract {sig} from {rec.record_name} due to {e}')
         elif errors == 'raise':
             raise ValueError(f'Signal name {sig} is not in the provided record')
         else:
             raise ValueError('errors must be one of [\'ignore\', \'raise\']')
 
 def locate_valid_records(signals: List[str], min_length: int, n_segments: int, shuffle: bool = True) -> List[str]:
     """Locate valid data records. Exclusion is performed based on a list of signals
```

### Comparing `heartfelt_tools-1.7.0/database_tools/processing/cardiac.py` & `heartfelt_tools-1.8.0/database_tools/processing/cardiac.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/processing/detect.py` & `heartfelt_tools-1.8.0/database_tools/processing/detect.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/processing/metrics.py` & `heartfelt_tools-1.8.0/database_tools/processing/metrics.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/processing/modify.py` & `heartfelt_tools-1.8.0/database_tools/processing/modify.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/processing/utils.py` & `heartfelt_tools-1.8.0/database_tools/processing/utils.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/tools/DataEvaluator.py` & `heartfelt_tools-1.8.0/database_tools/tools/DataEvaluator.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/tools/DataLocator.py` & `heartfelt_tools-1.8.0/database_tools/tools/DataLocator.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/tools/dataset.py` & `heartfelt_tools-1.8.0/database_tools/tools/dataset.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/database_tools/tools/records.py` & `heartfelt_tools-1.8.0/database_tools/tools/records.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-1.7.0/pyproject.toml` & `heartfelt_tools-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heartfelt-tools"
-version = "1.7.0"
+version = "1.8.0"
 description = "Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb."
 authors = ["Cameron Johnson"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "database_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `heartfelt_tools-1.7.0/setup.py` & `heartfelt_tools-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'tensorflow==2.9.2',
  'tqdm>=4.64.1,<5.0.0',
  'vitaldb>=1.2.10,<2.0.0',
  'wfdb>=4.0.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'heartfelt-tools',
-    'version': '1.7.0',
+    'version': '1.8.0',
     'description': 'Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb.',
     'long_description': '<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->\n<a name="readme-top"></a>\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n      \n            \n <img src="images/heartfelt-logo.png"  width="300em" height="300em"> \n\n  \n  <h1 align="center">MIMIC-III Database Tools</h1>\n\n  <p align="center">\n    For extracting and cleaning ppg and abp data from the MIMIC-III Waveforms Database.\n    <br />\n  </p>\n</div>\n\n\n\n<!-- TABLE OF CONTENTS -->\n<details>\n  <summary>Table of Contents</summary>\n  <ol>\n    <li>\n      <a href="#introduction">Introduction</a>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n      <ul>\n        <li><a href="#poetry">Poetry</a></li>\n        <li><a href="#get-valid-records">Get Valid Records</a></li>\n        <li><a href="#build-database">Build Database</a></li>\n        <li><a href="#evaluate-dataset">Evaluate Dataset</a></li>\n        <li><a href="#generate-records">Generate Records</a></li>\n        <li><a href="#read-records">Read Records</a></li>\n      </ul>\n    <li><a href="#license">License</a></li>\n  </ol>\n</details>\n\n\n\n<!-- Introduction -->\n## Introduction\n\nThis repo contains a set of tools for extracting and cleaning photoplethysmography (ppg) and artial blood pressure (abp) waveforms from the [MIMIC-III Waveforms Database](https://physionet.org/content/mimic3wdb/1.0/) for the purpose of blood pressure estimation via deep learning. \n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n<!-- GETTING STARTED -->\n## Getting Started\n\nThis sections details the requirements to start using this library. Links are for Ubuntu installation.\n\n### Prerequisites\n\n1. Python\n```shell\nsudo apt install python3.8 -y\nsudo apt install python3.8-dev python3.8-venv -y\n\necho \'export PATH="$PATH:/home/ubuntu/.local/bin"\' >> ~/.bashrc\nsource ~/.bashrc\n\ncurl -sS https://bootstrap.pypa.io/get-pip.py | python3.8\npython3.8 -m pip install virtualenv\npython3.8 -m venv .venv/base-env\necho \'alias base-env="source ~/.venv/base-env/bin/activate"\' >> ~/.bashrc\nbase-env\n\npython3.8 -m pip install --upgrade pip\n```\n2. Poetry\n```shell\ncurl -sSL https://install.python-poetry.org | python3 -\necho \'export PATH="$PATH:$HOME/.local/bin"\' >> ~/.bashrc\nsource ~/.bashrc\n\n# Verify installation\npoetry --version\n```\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\n### Poetry\nThe commands below can be used to install the poetry environment, build the project, and activate the environment.\n```shell\ncd database-tools\npoetry lock\npoetry install\npoetry build\npoetry shell\n```\n\n### Create Data Directory\nThe functions in this library rely on a data folder named with the convention `data-YYYY-MM-DD`. This directory contains two additional folders, `mimic3/` and `figures/`. The `mimic3/lines/` folder is intended to hold the jsonlines files the data will initially saved to. The `mimic3/records/` folder will hold the TFRecords files generated from these jsonlines files. This will be discussed in greater depth in the <a href="#generate-records">Generate Records</a> section.\n\n### Get Valid Records\nThe class DataLocator (located in `database_tools/tools/`) is specifically written to find valid data files in the MIMIC-III Waveforms subset and create a csv of the html links for these data files. Performing this task prior to downloading is done to improve runtime and the usability of this workflow. Valid records refers to data files that contain both PPG and ABP recordings and are at least 10 minutes in length. Currently this code is only intended for the MIMIC-III Waveforms subset but will likely be adapated to allow for valid segments to be identified in the MIMIC-III Matched Subset (records are linked to clinical data). To perform an extraction the file `scripts/get-valid-segs.py` can be run (data directory and repository path must be configured manually). This function will output a csv called `valid-segments.csv` to the data directory provided. The figure below shows how these signals are located.\n\nAdd mimic3 valid segs logic figure.\n\n### Build Database\nThe class `BuildDatabase` (located in `database_tools/tools/`) downloads data from `valid-segments.csv`, extracts PPG and ABP data, and then processed it by leveraging the `SignalProcessor` class (located in `database_tools/preprocessing/`). A database can be build by running `scripts/build_database.py` (be sure to configure the paths). BuildDatabase takes a few important parameters which modify how signals are excluded and how the signals are divided prior to processing. The `win_len` parameter controls the length of each window, `fs` is the sampling rate of the data (125 Hz in the case of MIMIC-III), while `samples_per_file`, `samples_per_patient`, and `max_samples` control the size of the dataset (how many files the data is spread across, how many samples a patient can contribute, and the total number of samples in the dataset. The final parameter `config` controls the various constants of the SignalProcessor that determine the quality threshold for accepting signals. The SignalProcessor filters signals according to the figure chart below. The functions used for this filtering can be found in `database_tools/preprocessing/`. Data exctracted with this script is saved directly to the `mimic3/lines/` folder in the data directory. A file named `mimic3_stats.csv` containing the stats of every processed waveform (not just the valid ones) will also be saved to the data directory.\n\nAdd data preprocessing figure.\n\n### Evaluate Dataset\nThe class `DataEvaluator` (located in `database_tools/tools/`) reads the `mimic3_stats.csv` file from the provided data directory and outputs figures to visualize the statistics. These figures are saved directly to the `figures/` folder in the data directory in addition to be output such that they can be viewed in a Jupyter notebook. The 3D histogram are generated using the fuction `histogram3d` located in `database_tools/plotting/`.\n\n### Generate Records\nOnce data has been extracted TFRecords can be generated for training a Tensorflow model. The class `RecordsHandler` contains the method `GenerateRecords` which is used to create the TFRecords. This can be done using `scripts/generate_records.py` (paths must be configured). When calling `GenerateRecords` the size of the train, validation, and test splits, as well as the max number of samples per file and a boolean to control whether or not the data is standardized must be specified (using `sklearn.preprocessing.StandardScaler()`.\n\n### Read Records\nThe class `RecordsHandler` also contains the function `ReadRecords` which can be used to read the TFRecords into a Tensorflow `TFRecordsDataset` object. This function can be used to inspect the integrity of the dataset or for loading the dataset for model training. The number of cores and a TensorFlow `AUTOTUNE` object must be provided.\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the MIT License. See `LICENSE.txt` for more information.\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n',
     'author': 'Cameron Johnson',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 'database_tools.processing', 'database_tools.tools'] package_data = \ {'':
 ['*']} install_requires = \ ['alive-progress>=3.0.1,<4.0.0',
 'heartpy>=1.2.7,<2.0.0', 'neurokit2>=0.2.1,<0.3.0', 'numpy>=1.23.4,<2.0.0',
 'openpyxl>=3.0.10,<4.0.0', 'pandas>=1.5.1,<2.0.0', 'plotly>=5.10.0,<6.0.0',
 'pytest>=7.2.1,<8.0.0', 'scikit-learn>=1.1.2,<2.0.0', 'scipy>=1.9.3,<2.0.0',
 'tabulate>=0.9.0,<0.10.0', 'tensorflow==2.9.2', 'tqdm>=4.64.1,<5.0.0',
 'vitaldb>=1.2.10,<2.0.0', 'wfdb>=4.0.0,<5.0.0'] setup_kwargs = { 'name':
-'heartfelt-tools', 'version': '1.7.0', 'description': 'Extract and process
+'heartfelt-tools', 'version': '1.8.0', 'description': 'Extract and process
 photoplethysmography and arterial blood pressure data from mimic3-waveforms and
 vitaldb.', 'long_description': '\n\n\n\n
 \n
                  \n \n \n [images/heartfelt-logo.png] \n\n \n
                     ****** MIMIC-III Database Tools ******
                                      \n\n
  \n For extracting and cleaning ppg and abp data from the MIMIC-III Waveforms
```

### Comparing `heartfelt_tools-1.7.0/PKG-INFO` & `heartfelt_tools-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartfelt-tools
-Version: 1.7.0
+Version: 1.8.0
 Summary: Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb.
 License: MIT
 Author: Cameron Johnson
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: heartfelt-tools Version: 1.7.0 Summary: Extract and
+Metadata-Version: 2.1 Name: heartfelt-tools Version: 1.8.0 Summary: Extract and
 process photoplethysmography and arterial blood pressure data from mimic3-
 waveforms and vitaldb. License: MIT Author: Cameron Johnson Requires-Python:
 >=3.9,<3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Requires-Dist: alive-progress (>=3.0.1,<4.0.0) Requires-Dist: heartpy
 (>=1.2.7,<2.0.0) Requires-Dist: neurokit2 (>=0.2.1,<0.3.0) Requires-Dist: numpy
 (>=1.23.4,<2.0.0) Requires-Dist: openpyxl (>=3.0.10,<4.0.0) Requires-Dist:
```

