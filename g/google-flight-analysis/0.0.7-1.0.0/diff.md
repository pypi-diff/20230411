# Comparing `tmp/google-flight-analysis-0.0.7.tar.gz` & `tmp/google-flight-analysis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-flight-analysis-0.0.7.tar", last modified: Thu Apr  6 02:16:04 2023, max compression
+gzip compressed data, was "google-flight-analysis-1.0.0.tar", last modified: Tue Apr 11 05:25:37 2023, max compression
```

## Comparing `google-flight-analysis-0.0.7.tar` & `google-flight-analysis-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.095262 google-flight-analysis-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.091262 google-flight-analysis-0.0.7/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.087262 google-flight-analysis-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.091262 google-flight-analysis-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/.github/workflows/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.091262 google-flight-analysis-0.0.7/.github/workflows/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/.github/workflows/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.091262 google-flight-analysis-0.0.7/API/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/API/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-06 02:16:04.095262 google-flight-analysis-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.091262 google-flight-analysis-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.091262 google-flight-analysis-0.0.7/forecasting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/forecasting/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-06 02:16:04.095262 google-flight-analysis-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.087262 google-flight-analysis-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.091262 google-flight-analysis-0.0.7/src/google_flight_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/src/google_flight_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/src/google_flight_analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/src/google_flight_analysis/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/src/google_flight_analysis/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.095262 google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-06 02:16:04.000000 google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-06 02:16:04.000000 google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:16:04.000000 google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-06 02:16:04.000000 google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-06 02:16:04.000000 google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 02:16:04.000000 google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.095262 google-flight-analysis-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:16:04.095262 google-flight-analysis-0.0.7/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/tests/test_data/test1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-06 02:15:56.000000 google-flight-analysis-0.0.7/tests/test_data/test2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.852778 google-flight-analysis-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.844778 google-flight-analysis-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.github/workflows/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/.github/workflows/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.github/workflows/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-11 05:25:37.852778 google-flight-analysis-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-11 05:25:37.852778 google-flight-analysis-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.844778 google-flight-analysis-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/src/google_flight_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/src/google_flight_analysis/scrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 05:25:37.000000 google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:25:37.848778 google-flight-analysis-1.0.0/tests/test_data/.access/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/.access/CDG-IST.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/.access/LGA-RDU.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/CDG-IST.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/LGA-RDU.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/test1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-11 05:25:27.000000 google-flight-analysis-1.0.0/tests/test_data/test2.csv
```

### Comparing `google-flight-analysis-0.0.7/.circleci/config.yml` & `google-flight-analysis-1.0.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-0.0.7/.github/workflows/scripts/release.py` & `google-flight-analysis-1.0.0/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-0.0.7/LICENSE` & `google-flight-analysis-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-0.0.7/PKG-INFO` & `google-flight-analysis-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: google-flight-analysis
-Version: 0.0.7
+Version: 1.0.0
 Summary: Scraping flight data from Google Flights and analyzing.
 Home-page: https://github.com/kcelebi/flight_analysis
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/flight_analysis/issues
 Project-URL: Changelog, https://github.com/kcelebi/flight_analysis/releases
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![kcelebi](https://circleci.com/gh/kcelebi/flight-analysis.svg?style=svg)](https://circleci.com/gh/kcelebi/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://github.com/kcelebi/flight-analysis/actions/workflows/publish.yml/badge.svg?branch=main)](https://github.com/kcelebi/flight-analysis/actions/workflows/publish.yml)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-0.0.7-brightgreen)](https://img.shields.io/endpoint?url=img.shields.io/badge/PyPI-0.0.7-brightgreen)
 
 # Flight Analysis
 
-This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 8/29/22) are:
+This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
 
 - Scraping tools for Google Flights
 - Base analytical tools/methods for price forecasting/summary
+
+The features in development are:
+
 - Models to demonstrate ML techniques on forecasting
 - API for access to previously collected data
 
 ## Table of Contents
 - [Overview](#Overview)
 - [Usage](#usage)
 - [Updates & New Features](#updates-&-new-features)
@@ -40,35 +43,51 @@
 
 ## Usage
 
 The web scraping tool is currently functional only for scraping round trip flights for a given origin, destination, and date range. It can be easily used in a script or a jupyter notebook.
 
 Note that the following packages are **absolutely required** as dependencies:
 - tqdm
-- selenium (make sure to update your [chromedriver](https://chromedriver.chromium.org)!)
-- json
+- selenium **(make sure to update your [ChromeDriver](https://chromedriver.chromium.org)!)**
+- pandas
+- numpy
+
+You can easily install this by running either installing the Python package `google-flight-analysis`:
+
+	pip install google-flight-analysis
+
+or forking/cloning this repository. Upon doing so, make sure to install the dependencies and update ChromeDriver to match your Google Chrome version.
+
+	pip install -r requirements.txt
+
 
-You can easily install this by running `pip install -r requirements.txt`.
+The main scraping function that makes up the backbone of most other functionalities is `Scrape()`. It serves also as a data object, preserving the flight information as well as meta-data from your query. For Python package users, import as follows:
 
-The main scraping function that makes up the backbone of most other functionalities is `scrape_data`. Note that the `cache` parameter refers to whether this output should be saved in a caching system. See further documentation on caching (to be available soon).
+	from google_flight_analysis.scrape import *
+
+For GitHub repository cloners, import as follows from the root of the repository:
+
+	from src.google_flight_analysis.scrape import *
+
+Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
-	# Parameter documentation
-	# scrape_data(origin : str, destination : str, date_leave : str, date_return : str, cache : bool = False) -> dict
 	# Try to keep the dates in format YYYY-mm-dd
-	
-	result = scrape_data('JFK', 'IST', '2022-05-20', '2022-06-10')
-	
-	# Can also input list of date strings for date_leave and date_return
-	
-	leave_dates = ['2022-05-20', '2022-05-21', '2022-05-22']
-	return_dates = ['2022-06-10', '2022-06-11', '2022-06-12']
-	range_result = scrape_data('JFK', 'IST', leave_dates, return_dates)
-	
+	result = Scrape('JFK', 'IST', '2022-05-20', '2022-06-10') # obtain our scrape object
+
+	dataframe = result.data # outputs a Pandas DF with flight prices/info
+	origin = result.origin # 'JFK'
+	dest = result.dest # 'IST'
+	date_leave = result.date_leave # '2022-05-20'
+	date_return = result.date_return # '2022-06-10'
+
+
 ## Updates & New Features
 
+Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
+
 
 <!--
 ## Cache Data
 
 The caching system for this application is mainly designed to make the loading of data more efficient. For the moment, this component of the application hasn't been designed well for the public to easily use so I would suggest that most people leave it alone, or fork the repository and modify some of the functions to create folders in the destinations that they would prefer. The key caching functions are:
 
 - `cache_data`
```

### Comparing `google-flight-analysis-0.0.7/README.md` & `google-flight-analysis-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [![kcelebi](https://circleci.com/gh/kcelebi/flight-analysis.svg?style=svg)](https://circleci.com/gh/kcelebi/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://github.com/kcelebi/flight-analysis/actions/workflows/publish.yml/badge.svg?branch=main)](https://github.com/kcelebi/flight-analysis/actions/workflows/publish.yml)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-0.0.7-brightgreen)](https://img.shields.io/endpoint?url=img.shields.io/badge/PyPI-0.0.7-brightgreen)
 
 # Flight Analysis
 
-This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 8/29/22) are:
+This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
 
 - Scraping tools for Google Flights
 - Base analytical tools/methods for price forecasting/summary
+
+The features in development are:
+
 - Models to demonstrate ML techniques on forecasting
 - API for access to previously collected data
 
 ## Table of Contents
 - [Overview](#Overview)
 - [Usage](#usage)
 - [Updates & New Features](#updates-&-new-features)
@@ -24,35 +27,51 @@
 
 ## Usage
 
 The web scraping tool is currently functional only for scraping round trip flights for a given origin, destination, and date range. It can be easily used in a script or a jupyter notebook.
 
 Note that the following packages are **absolutely required** as dependencies:
 - tqdm
-- selenium (make sure to update your [chromedriver](https://chromedriver.chromium.org)!)
-- json
+- selenium **(make sure to update your [ChromeDriver](https://chromedriver.chromium.org)!)**
+- pandas
+- numpy
+
+You can easily install this by running either installing the Python package `google-flight-analysis`:
+
+	pip install google-flight-analysis
+
+or forking/cloning this repository. Upon doing so, make sure to install the dependencies and update ChromeDriver to match your Google Chrome version.
+
+	pip install -r requirements.txt
+
 
-You can easily install this by running `pip install -r requirements.txt`.
+The main scraping function that makes up the backbone of most other functionalities is `Scrape()`. It serves also as a data object, preserving the flight information as well as meta-data from your query. For Python package users, import as follows:
 
-The main scraping function that makes up the backbone of most other functionalities is `scrape_data`. Note that the `cache` parameter refers to whether this output should be saved in a caching system. See further documentation on caching (to be available soon).
+	from google_flight_analysis.scrape import *
+
+For GitHub repository cloners, import as follows from the root of the repository:
+
+	from src.google_flight_analysis.scrape import *
+
+Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
-	# Parameter documentation
-	# scrape_data(origin : str, destination : str, date_leave : str, date_return : str, cache : bool = False) -> dict
 	# Try to keep the dates in format YYYY-mm-dd
-	
-	result = scrape_data('JFK', 'IST', '2022-05-20', '2022-06-10')
-	
-	# Can also input list of date strings for date_leave and date_return
-	
-	leave_dates = ['2022-05-20', '2022-05-21', '2022-05-22']
-	return_dates = ['2022-06-10', '2022-06-11', '2022-06-12']
-	range_result = scrape_data('JFK', 'IST', leave_dates, return_dates)
-	
+	result = Scrape('JFK', 'IST', '2022-05-20', '2022-06-10') # obtain our scrape object
+
+	dataframe = result.data # outputs a Pandas DF with flight prices/info
+	origin = result.origin # 'JFK'
+	dest = result.dest # 'IST'
+	date_leave = result.date_leave # '2022-05-20'
+	date_return = result.date_return # '2022-06-10'
+
+
 ## Updates & New Features
 
+Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
+
 
 <!--
 ## Cache Data
 
 The caching system for this application is mainly designed to make the loading of data more efficient. For the moment, this component of the application hasn't been designed well for the public to easily use so I would suggest that most people leave it alone, or fork the repository and modify some of the functions to create folders in the destinations that they would prefer. The key caching functions are:
 
 - `cache_data`
```

### Comparing `google-flight-analysis-0.0.7/setup.cfg` & `google-flight-analysis-1.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description_content_type = text/markdown
 url = https://github.com/kcelebi/flight_analysis
 project_urls = 
 	Bug Tracker = https://github.com/kcelebi/flight_analysis/issues
 	Changelog = https://github.com/kcelebi/flight_analysis/releases
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: BSD License
+	License :: OSI Approved :: MIT License
 	Intended Audience :: Developers
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
```

### Comparing `google-flight-analysis-0.0.7/src/google_flight_analysis/scrape.py` & `google-flight-analysis-1.0.0/src/google_flight_analysis/scrape.py`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-0.0.7/src/google_flight_analysis.egg-info/PKG-INFO` & `google-flight-analysis-1.0.0/src/google_flight_analysis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: google-flight-analysis
-Version: 0.0.7
+Version: 1.0.0
 Summary: Scraping flight data from Google Flights and analyzing.
 Home-page: https://github.com/kcelebi/flight_analysis
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/flight_analysis/issues
 Project-URL: Changelog, https://github.com/kcelebi/flight_analysis/releases
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![kcelebi](https://circleci.com/gh/kcelebi/flight-analysis.svg?style=svg)](https://circleci.com/gh/kcelebi/flight-analysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Live on PyPI](https://github.com/kcelebi/flight-analysis/actions/workflows/publish.yml/badge.svg?branch=main)](https://github.com/kcelebi/flight-analysis/actions/workflows/publish.yml)
+[![Live on PyPI](https://img.shields.io/badge/PyPI-0.0.7-brightgreen)](https://img.shields.io/endpoint?url=img.shields.io/badge/PyPI-0.0.7-brightgreen)
 
 # Flight Analysis
 
-This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 8/29/22) are:
+This project provides tools and models for users to analyze, forecast, and collect data regarding flights and prices. There are currently many features in initial stages and in development. The current features (as of 4/5/2023) are:
 
 - Scraping tools for Google Flights
 - Base analytical tools/methods for price forecasting/summary
+
+The features in development are:
+
 - Models to demonstrate ML techniques on forecasting
 - API for access to previously collected data
 
 ## Table of Contents
 - [Overview](#Overview)
 - [Usage](#usage)
 - [Updates & New Features](#updates-&-new-features)
@@ -40,35 +43,51 @@
 
 ## Usage
 
 The web scraping tool is currently functional only for scraping round trip flights for a given origin, destination, and date range. It can be easily used in a script or a jupyter notebook.
 
 Note that the following packages are **absolutely required** as dependencies:
 - tqdm
-- selenium (make sure to update your [chromedriver](https://chromedriver.chromium.org)!)
-- json
+- selenium **(make sure to update your [ChromeDriver](https://chromedriver.chromium.org)!)**
+- pandas
+- numpy
+
+You can easily install this by running either installing the Python package `google-flight-analysis`:
+
+	pip install google-flight-analysis
+
+or forking/cloning this repository. Upon doing so, make sure to install the dependencies and update ChromeDriver to match your Google Chrome version.
+
+	pip install -r requirements.txt
+
 
-You can easily install this by running `pip install -r requirements.txt`.
+The main scraping function that makes up the backbone of most other functionalities is `Scrape()`. It serves also as a data object, preserving the flight information as well as meta-data from your query. For Python package users, import as follows:
 
-The main scraping function that makes up the backbone of most other functionalities is `scrape_data`. Note that the `cache` parameter refers to whether this output should be saved in a caching system. See further documentation on caching (to be available soon).
+	from google_flight_analysis.scrape import *
+
+For GitHub repository cloners, import as follows from the root of the repository:
+
+	from src.google_flight_analysis.scrape import *
+
+Here is some quick starter code to accomplish the basic tasks. Find more in the [documentation](https://kcelebi.github.io/flight-analysis/).
 
-	# Parameter documentation
-	# scrape_data(origin : str, destination : str, date_leave : str, date_return : str, cache : bool = False) -> dict
 	# Try to keep the dates in format YYYY-mm-dd
-	
-	result = scrape_data('JFK', 'IST', '2022-05-20', '2022-06-10')
-	
-	# Can also input list of date strings for date_leave and date_return
-	
-	leave_dates = ['2022-05-20', '2022-05-21', '2022-05-22']
-	return_dates = ['2022-06-10', '2022-06-11', '2022-06-12']
-	range_result = scrape_data('JFK', 'IST', leave_dates, return_dates)
-	
+	result = Scrape('JFK', 'IST', '2022-05-20', '2022-06-10') # obtain our scrape object
+
+	dataframe = result.data # outputs a Pandas DF with flight prices/info
+	origin = result.origin # 'JFK'
+	dest = result.dest # 'IST'
+	date_leave = result.date_leave # '2022-05-20'
+	date_return = result.date_return # '2022-06-10'
+
+
 ## Updates & New Features
 
+Performing a complete revamp of this package, including new addition to PyPI. Documentation is being updated frequently, contact for any questions.
+
 
 <!--
 ## Cache Data
 
 The caching system for this application is mainly designed to make the loading of data more efficient. For the moment, this component of the application hasn't been designed well for the public to easily use so I would suggest that most people leave it alone, or fork the repository and modify some of the functions to create folders in the destinations that they would prefer. The key caching functions are:
 
 - `cache_data`
```

### Comparing `google-flight-analysis-0.0.7/tests/test_data/test1.csv` & `google-flight-analysis-1.0.0/tests/test_data/test1.csv`

 * *Files identical despite different names*

### Comparing `google-flight-analysis-0.0.7/tests/test_data/test2.csv` & `google-flight-analysis-1.0.0/tests/test_data/test2.csv`

 * *Files identical despite different names*

