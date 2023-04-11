# Comparing `tmp/rcg-0.0.10.tar.gz` & `tmp/rcg-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcg-0.0.10.tar", last modified: Tue Apr 11 08:43:20 2023, max compression
+gzip compressed data, was "rcg-0.0.11.tar", last modified: Tue Apr 11 08:48:53 2023, max compression
```

## Comparing `rcg-0.0.10.tar` & `rcg-0.0.11.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:43:20.802222 rcg-0.0.10/
--rw-rw-rw-   0        0        0     1084 2023-04-07 03:51:45.000000 rcg-0.0.10/LICENSE
--rw-rw-rw-   0        0        0     7438 2023-04-11 08:43:20.801225 rcg-0.0.10/PKG-INFO
--rw-rw-rw-   0        0        0     6731 2023-04-11 08:33:36.000000 rcg-0.0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 08:43:20.764385 rcg-0.0.10/rcg/
--rw-rw-rw-   0        0        0        0 2023-04-07 06:43:05.000000 rcg-0.0.10/rcg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:43:20.788321 rcg-0.0.10/rcg/fuzzy/
--rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.10/rcg/fuzzy/__init__.py
--rw-rw-rw-   0        0        0    15199 2023-04-11 08:03:51.000000 rcg-0.0.10/rcg/fuzzy/categories.py
--rw-rw-rw-   0        0        0     3854 2023-04-11 08:01:10.000000 rcg-0.0.10/rcg/fuzzy/engine.py
--rw-rw-rw-   0        0        0     7981 2023-04-11 04:22:49.000000 rcg-0.0.10/rcg/fuzzy/memberships.py
--rw-rw-rw-   0        0        0    50253 2023-04-11 04:21:43.000000 rcg-0.0.10/rcg/fuzzy/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:43:20.796241 rcg-0.0.10/rcg/fuzzy/test_fuzzy/
--rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.10/rcg/fuzzy/test_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     9306 2023-04-11 04:22:49.000000 rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_categories.py
--rw-rw-rw-   0        0        0     3966 2023-04-11 04:13:47.000000 rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_engine.py
--rw-rw-rw-   0        0        0     3445 2023-04-11 04:21:43.000000 rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_memberships.py
--rw-rw-rw-   0        0        0     1119 2023-04-11 04:20:16.000000 rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:43:20.798232 rcg-0.0.10/rcg/inp_manage/
--rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.10/rcg/inp_manage/__init__.py
--rw-rw-rw-   0        0        0    18688 2023-04-11 03:46:03.000000 rcg-0.0.10/rcg/inp_manage/inp.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:43:20.800227 rcg-0.0.10/rcg/inp_manage/test_inp_manage/
--rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.10/rcg/inp_manage/test_inp_manage/__init__.py
--rw-rw-rw-   0        0        0    12465 2023-04-11 04:07:31.000000 rcg-0.0.10/rcg/inp_manage/test_inp_manage/test_inp.py
--rw-rw-rw-   0        0        0     1778 2023-04-09 10:37:37.000000 rcg-0.0.10/rcg/runner.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:43:20.780342 rcg-0.0.10/rcg.egg-info/
--rw-rw-rw-   0        0        0     7438 2023-04-11 08:43:20.000000 rcg-0.0.10/rcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-04-11 08:43:20.000000 rcg-0.0.10/rcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:43:20.000000 rcg-0.0.10/rcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-11 08:43:20.000000 rcg-0.0.10/rcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-11 08:43:20.000000 rcg-0.0.10/rcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 08:43:20.802222 rcg-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0     1729 2023-04-11 08:42:54.000000 rcg-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:48:53.438304 rcg-0.0.11/
+-rw-rw-rw-   0        0        0     1084 2023-04-07 03:51:45.000000 rcg-0.0.11/LICENSE
+-rw-rw-rw-   0        0        0     7361 2023-04-11 08:48:53.438304 rcg-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     6662 2023-04-11 08:48:29.000000 rcg-0.0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 08:48:53.409668 rcg-0.0.11/rcg/
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:43:05.000000 rcg-0.0.11/rcg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:48:53.426337 rcg-0.0.11/rcg/fuzzy/
+-rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.11/rcg/fuzzy/__init__.py
+-rw-rw-rw-   0        0        0    15199 2023-04-11 08:03:51.000000 rcg-0.0.11/rcg/fuzzy/categories.py
+-rw-rw-rw-   0        0        0     3854 2023-04-11 08:01:10.000000 rcg-0.0.11/rcg/fuzzy/engine.py
+-rw-rw-rw-   0        0        0     7981 2023-04-11 04:22:49.000000 rcg-0.0.11/rcg/fuzzy/memberships.py
+-rw-rw-rw-   0        0        0    50253 2023-04-11 04:21:43.000000 rcg-0.0.11/rcg/fuzzy/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:48:53.432320 rcg-0.0.11/rcg/fuzzy/test_fuzzy/
+-rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.11/rcg/fuzzy/test_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     9306 2023-04-11 04:22:49.000000 rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_categories.py
+-rw-rw-rw-   0        0        0     3966 2023-04-11 04:13:47.000000 rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_engine.py
+-rw-rw-rw-   0        0        0     3445 2023-04-11 04:21:43.000000 rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_memberships.py
+-rw-rw-rw-   0        0        0     1119 2023-04-11 04:20:16.000000 rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_rules.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:48:53.434315 rcg-0.0.11/rcg/inp_manage/
+-rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.11/rcg/inp_manage/__init__.py
+-rw-rw-rw-   0        0        0    18688 2023-04-11 03:46:03.000000 rcg-0.0.11/rcg/inp_manage/inp.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:48:53.437307 rcg-0.0.11/rcg/inp_manage/test_inp_manage/
+-rw-rw-rw-   0        0        0        0 2023-04-07 03:51:45.000000 rcg-0.0.11/rcg/inp_manage/test_inp_manage/__init__.py
+-rw-rw-rw-   0        0        0    12465 2023-04-11 04:07:31.000000 rcg-0.0.11/rcg/inp_manage/test_inp_manage/test_inp.py
+-rw-rw-rw-   0        0        0     1778 2023-04-09 10:37:37.000000 rcg-0.0.11/rcg/runner.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:48:53.419374 rcg-0.0.11/rcg.egg-info/
+-rw-rw-rw-   0        0        0     7361 2023-04-11 08:48:53.000000 rcg-0.0.11/rcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-04-11 08:48:53.000000 rcg-0.0.11/rcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:48:53.000000 rcg-0.0.11/rcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-11 08:48:53.000000 rcg-0.0.11/rcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-11 08:48:53.000000 rcg-0.0.11/rcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:48:53.439309 rcg-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      947 2023-04-11 08:48:38.000000 rcg-0.0.11/setup.py
```

### Comparing `rcg-0.0.10/LICENSE` & `rcg-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/PKG-INFO` & `rcg-0.0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 Metadata-Version: 2.1
 Name: rcg
-Version: 0.0.10
+Version: 0.0.11
 Summary: Rapid catchment generator - is a tool for rapid prototyping of a hydraulic model catchments that can be read and edited with SWMM.
 Home-page: UNKNOWN
 Author: Rafał Buczyński
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/BuczynskiRafal/rapid-catchment-generator
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Rapid catchment generator
-Tool for rapid prototyping of a hydraulic model that can be read and edited with SWMM.
-The generator was created using feature analysis and surface runoff research from the literature. 
-Fuzzy logic controller rules were developed using parameterized categories of soil, slope, 
-and permeability. The catchment configuration procedure was simplified by mapping typical 
-storage and Manning's coefficients. The use of fuzzy logic rules allows the system to be modified 
-to adjust the categories to certain situations. The use of membership functions allows us to increase 
-computation accuracy and customize the tool to diverse applications. Following alteration 
-of the catchment in the SWMM GUI allows for accurate portrayal of the real condition of the catchment; 
-no issues were encountered in altering the *inp file.
+Tool for rapid prototyping of a hydraulic model that can be read and edited with SWMM. The generator was created using feature analysis and surface runoff research from the literature. Fuzzy logic controller rules were developed using parameterized categories of soil, slope, and permeability. The catchment configuration procedure was simplified by mapping typical storage and Manning's coefficients. The use of fuzzy logic rules allows the system to be modified to adjust the categories to certain situations. The use of membership functions allows us to increase computation accuracy and customize the tool to diverse applications. Following alteration of the catchment in the SWMM GUI allows for accurate portrayal of the real condition of the catchment.
 
 ## Requirements
 * Python 3
 
 ## Usage
 Create a virtual environment:
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: rcg Version: 0.0.10 Summary: Rapid catchment
+Metadata-Version: 2.1 Name: rcg Version: 0.0.11 Summary: Rapid catchment
 generator - is a tool for rapid prototyping of a hydraulic model catchments
 that can be read and edited with SWMM. Home-page: UNKNOWN Author: RafaÅ
 BuczyÅski License: UNKNOWN Project-URL: Homepage, https://github.com/
 BuczynskiRafal/rapid-catchment-generator Platform: UNKNOWN Description-Content-
 Type: text/markdown License-File: LICENSE # Rapid catchment generator Tool for
 rapid prototyping of a hydraulic model that can be read and edited with SWMM.
 The generator was created using feature analysis and surface runoff research
 from the literature. Fuzzy logic controller rules were developed using
 parameterized categories of soil, slope, and permeability. The catchment
 configuration procedure was simplified by mapping typical storage and Manning's
 coefficients. The use of fuzzy logic rules allows the system to be modified to
 adjust the categories to certain situations. The use of membership functions
 allows us to increase computation accuracy and customize the tool to diverse
 applications. Following alteration of the catchment in the SWMM GUI allows for
-accurate portrayal of the real condition of the catchment; no issues were
-encountered in altering the *inp file. ## Requirements * Python 3 ## Usage
-Create a virtual environment: ``` python3 -m venv venv ``` Download and install
-the required dependencies: ``` python3 pip install -r requirements ``` To run
-the script, use the following command: ``` python3 rcg.runner file path ```
-where `file path` is the path to the SWMM model file. Enter data into the
-terminal according to the instructions it displays. The file is automatically
-saved in the same directory. ## About For the construction of the catchment
-generator, the type of land use was divided according to Table 1, the land
-cover according to Table 2. The categories were determined on the basis of the
-data presented by (DoÅÄga, Rogala, 1973), given below in Table 3.
+accurate portrayal of the real condition of the catchment. ## Requirements *
+Python 3 ## Usage Create a virtual environment: ``` python3 -m venv venv ```
+Download and install the required dependencies: ``` python3 pip install -
+r requirements ``` To run the script, use the following command: ``` python3
+rcg.runner file path ``` where `file path` is the path to the SWMM model file.
+Enter data into the terminal according to the instructions it displays. The
+file is automatically saved in the same directory. ## About For the
+construction of the catchment generator, the type of land use was divided
+according to Table 1, the land cover according to Table 2. The categories were
+determined on the basis of the data presented by (DoÅÄga, Rogala, 1973),
+given below in Table 3.
 **** Table 1. Land use categories ****
 Number Land Use
 1      marshes and lowlands
 2      flats and plateaus
 3      flats and plateaus in combination with hills
 4      hills with gentle slopes
 5      steeper hills and foothills
```

### Comparing `rcg-0.0.10/README.md` & `rcg-0.0.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 # Rapid catchment generator
-Tool for rapid prototyping of a hydraulic model that can be read and edited with SWMM.
-The generator was created using feature analysis and surface runoff research from the literature. 
-Fuzzy logic controller rules were developed using parameterized categories of soil, slope, 
-and permeability. The catchment configuration procedure was simplified by mapping typical 
-storage and Manning's coefficients. The use of fuzzy logic rules allows the system to be modified 
-to adjust the categories to certain situations. The use of membership functions allows us to increase 
-computation accuracy and customize the tool to diverse applications. Following alteration 
-of the catchment in the SWMM GUI allows for accurate portrayal of the real condition of the catchment; 
-no issues were encountered in altering the *inp file.
+Tool for rapid prototyping of a hydraulic model that can be read and edited with SWMM. The generator was created using feature analysis and surface runoff research from the literature. Fuzzy logic controller rules were developed using parameterized categories of soil, slope, and permeability. The catchment configuration procedure was simplified by mapping typical storage and Manning's coefficients. The use of fuzzy logic rules allows the system to be modified to adjust the categories to certain situations. The use of membership functions allows us to increase computation accuracy and customize the tool to diverse applications. Following alteration of the catchment in the SWMM GUI allows for accurate portrayal of the real condition of the catchment.
 
 ## Requirements
 * Python 3
 
 ## Usage
 Create a virtual environment:
 ```
```

#### html2text {}

```diff
@@ -4,25 +4,24 @@
 controller rules were developed using parameterized categories of soil, slope,
 and permeability. The catchment configuration procedure was simplified by
 mapping typical storage and Manning's coefficients. The use of fuzzy logic
 rules allows the system to be modified to adjust the categories to certain
 situations. The use of membership functions allows us to increase computation
 accuracy and customize the tool to diverse applications. Following alteration
 of the catchment in the SWMM GUI allows for accurate portrayal of the real
-condition of the catchment; no issues were encountered in altering the *inp
-file. ## Requirements * Python 3 ## Usage Create a virtual environment: ```
-python3 -m venv venv ``` Download and install the required dependencies: ```
-python3 pip install -r requirements ``` To run the script, use the following
-command: ``` python3 rcg.runner file path ``` where `file path` is the path to
-the SWMM model file. Enter data into the terminal according to the instructions
-it displays. The file is automatically saved in the same directory. ## About
-For the construction of the catchment generator, the type of land use was
-divided according to Table 1, the land cover according to Table 2. The
-categories were determined on the basis of the data presented by (DoÅÄga,
-Rogala, 1973), given below in Table 3.
+condition of the catchment. ## Requirements * Python 3 ## Usage Create a
+virtual environment: ``` python3 -m venv venv ``` Download and install the
+required dependencies: ``` python3 pip install -r requirements ``` To run the
+script, use the following command: ``` python3 rcg.runner file path ``` where
+`file path` is the path to the SWMM model file. Enter data into the terminal
+according to the instructions it displays. The file is automatically saved in
+the same directory. ## About For the construction of the catchment generator,
+the type of land use was divided according to Table 1, the land cover according
+to Table 2. The categories were determined on the basis of the data presented
+by (DoÅÄga, Rogala, 1973), given below in Table 3.
 **** Table 1. Land use categories ****
 Number Land Use
 1      marshes and lowlands
 2      flats and plateaus
 3      flats and plateaus in combination with hills
 4      hills with gentle slopes
 5      steeper hills and foothills
```

### Comparing `rcg-0.0.10/rcg/fuzzy/categories.py` & `rcg-0.0.11/rcg/fuzzy/categories.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/fuzzy/engine.py` & `rcg-0.0.11/rcg/fuzzy/engine.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/fuzzy/memberships.py` & `rcg-0.0.11/rcg/fuzzy/memberships.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/fuzzy/rules.py` & `rcg-0.0.11/rcg/fuzzy/rules.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_categories.py` & `rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_categories.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_engine.py` & `rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_engine.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_memberships.py` & `rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_memberships.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/fuzzy/test_fuzzy/test_rules.py` & `rcg-0.0.11/rcg/fuzzy/test_fuzzy/test_rules.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/inp_manage/inp.py` & `rcg-0.0.11/rcg/inp_manage/inp.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/inp_manage/test_inp_manage/test_inp.py` & `rcg-0.0.11/rcg/inp_manage/test_inp_manage/test_inp.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg/runner.py` & `rcg-0.0.11/rcg/runner.py`

 * *Files identical despite different names*

### Comparing `rcg-0.0.10/rcg.egg-info/PKG-INFO` & `rcg-0.0.11/rcg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 Metadata-Version: 2.1
 Name: rcg
-Version: 0.0.10
+Version: 0.0.11
 Summary: Rapid catchment generator - is a tool for rapid prototyping of a hydraulic model catchments that can be read and edited with SWMM.
 Home-page: UNKNOWN
 Author: Rafał Buczyński
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/BuczynskiRafal/rapid-catchment-generator
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Rapid catchment generator
-Tool for rapid prototyping of a hydraulic model that can be read and edited with SWMM.
-The generator was created using feature analysis and surface runoff research from the literature. 
-Fuzzy logic controller rules were developed using parameterized categories of soil, slope, 
-and permeability. The catchment configuration procedure was simplified by mapping typical 
-storage and Manning's coefficients. The use of fuzzy logic rules allows the system to be modified 
-to adjust the categories to certain situations. The use of membership functions allows us to increase 
-computation accuracy and customize the tool to diverse applications. Following alteration 
-of the catchment in the SWMM GUI allows for accurate portrayal of the real condition of the catchment; 
-no issues were encountered in altering the *inp file.
+Tool for rapid prototyping of a hydraulic model that can be read and edited with SWMM. The generator was created using feature analysis and surface runoff research from the literature. Fuzzy logic controller rules were developed using parameterized categories of soil, slope, and permeability. The catchment configuration procedure was simplified by mapping typical storage and Manning's coefficients. The use of fuzzy logic rules allows the system to be modified to adjust the categories to certain situations. The use of membership functions allows us to increase computation accuracy and customize the tool to diverse applications. Following alteration of the catchment in the SWMM GUI allows for accurate portrayal of the real condition of the catchment.
 
 ## Requirements
 * Python 3
 
 ## Usage
 Create a virtual environment:
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: rcg Version: 0.0.10 Summary: Rapid catchment
+Metadata-Version: 2.1 Name: rcg Version: 0.0.11 Summary: Rapid catchment
 generator - is a tool for rapid prototyping of a hydraulic model catchments
 that can be read and edited with SWMM. Home-page: UNKNOWN Author: RafaÅ
 BuczyÅski License: UNKNOWN Project-URL: Homepage, https://github.com/
 BuczynskiRafal/rapid-catchment-generator Platform: UNKNOWN Description-Content-
 Type: text/markdown License-File: LICENSE # Rapid catchment generator Tool for
 rapid prototyping of a hydraulic model that can be read and edited with SWMM.
 The generator was created using feature analysis and surface runoff research
 from the literature. Fuzzy logic controller rules were developed using
 parameterized categories of soil, slope, and permeability. The catchment
 configuration procedure was simplified by mapping typical storage and Manning's
 coefficients. The use of fuzzy logic rules allows the system to be modified to
 adjust the categories to certain situations. The use of membership functions
 allows us to increase computation accuracy and customize the tool to diverse
 applications. Following alteration of the catchment in the SWMM GUI allows for
-accurate portrayal of the real condition of the catchment; no issues were
-encountered in altering the *inp file. ## Requirements * Python 3 ## Usage
-Create a virtual environment: ``` python3 -m venv venv ``` Download and install
-the required dependencies: ``` python3 pip install -r requirements ``` To run
-the script, use the following command: ``` python3 rcg.runner file path ```
-where `file path` is the path to the SWMM model file. Enter data into the
-terminal according to the instructions it displays. The file is automatically
-saved in the same directory. ## About For the construction of the catchment
-generator, the type of land use was divided according to Table 1, the land
-cover according to Table 2. The categories were determined on the basis of the
-data presented by (DoÅÄga, Rogala, 1973), given below in Table 3.
+accurate portrayal of the real condition of the catchment. ## Requirements *
+Python 3 ## Usage Create a virtual environment: ``` python3 -m venv venv ```
+Download and install the required dependencies: ``` python3 pip install -
+r requirements ``` To run the script, use the following command: ``` python3
+rcg.runner file path ``` where `file path` is the path to the SWMM model file.
+Enter data into the terminal according to the instructions it displays. The
+file is automatically saved in the same directory. ## About For the
+construction of the catchment generator, the type of land use was divided
+according to Table 1, the land cover according to Table 2. The categories were
+determined on the basis of the data presented by (DoÅÄga, Rogala, 1973),
+given below in Table 3.
 **** Table 1. Land use categories ****
 Number Land Use
 1      marshes and lowlands
 2      flats and plateaus
 3      flats and plateaus in combination with hills
 4      hills with gentle slopes
 5      steeper hills and foothills
```

### Comparing `rcg-0.0.10/rcg.egg-info/SOURCES.txt` & `rcg-0.0.11/rcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

