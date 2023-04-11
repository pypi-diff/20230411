# Comparing `tmp/DA4RDM_Vis_ProcessBased-0.1.1.tar.gz` & `tmp/DA4RDM_Vis_ProcessBased-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DA4RDM_Vis_ProcessBased-0.1.1.tar", last modified: Thu Apr  6 16:02:36 2023, max compression
+gzip compressed data, was "DA4RDM_Vis_ProcessBased-0.1.6.tar", last modified: Tue Apr 11 15:23:37 2023, max compression
```

## Comparing `DA4RDM_Vis_ProcessBased-0.1.1.tar` & `DA4RDM_Vis_ProcessBased-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 16:02:36.424952 DA4RDM_Vis_ProcessBased-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-06 16:02:36.402390 DA4RDM_Vis_ProcessBased-0.1.1/DA4RDM_Vis_ProcessBased.egg-info/
--rw-rw-rw-   0        0        0     3503 2023-04-06 16:02:36.000000 DA4RDM_Vis_ProcessBased-0.1.1/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2023-04-06 16:02:36.000000 DA4RDM_Vis_ProcessBased-0.1.1/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 16:02:36.000000 DA4RDM_Vis_ProcessBased-0.1.1/DA4RDM_Vis_ProcessBased.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-06 16:02:36.000000 DA4RDM_Vis_ProcessBased-0.1.1/DA4RDM_Vis_ProcessBased.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1072 2023-04-05 06:47:24.000000 DA4RDM_Vis_ProcessBased-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       51 2023-04-05 15:44:42.000000 DA4RDM_Vis_ProcessBased-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3503 2023-04-06 16:02:36.425952 DA4RDM_Vis_ProcessBased-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3031 2023-04-06 16:01:43.000000 DA4RDM_Vis_ProcessBased-0.1.1/README.md
--rw-rw-rw-   0        0        0      483 2023-04-06 16:02:00.000000 DA4RDM_Vis_ProcessBased-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      303 2023-04-06 16:02:36.431952 DA4RDM_Vis_ProcessBased-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-04-06 16:02:15.000000 DA4RDM_Vis_ProcessBased-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 16:02:36.368360 DA4RDM_Vis_ProcessBased-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 16:02:36.411937 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/
--rw-rw-rw-   0        0        0     1764 2023-04-05 16:15:18.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py
--rw-rw-rw-   0        0        0     1351 2023-04-05 06:14:11.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/Extract.py
-drwxrwxrwx   0        0        0        0 2023-04-06 16:02:36.422959 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/
--rw-rw-rw-   0        0        0      581 2023-04-05 06:12:12.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv
--rw-rw-rw-   0        0        0      503 2023-04-05 06:12:12.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Analysis.csv
--rw-rw-rw-   0        0        0      619 2023-04-05 06:12:12.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv
--rw-rw-rw-   0        0        0      929 2023-04-05 06:12:12.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv
--rw-rw-rw-   0        0        0     1001 2023-04-05 06:12:12.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv
--rw-rw-rw-   0        0        0      687 2023-04-05 06:12:12.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv
--rw-rw-rw-   0        0        0     3586 2023-04-05 16:43:35.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/Visualize.py
--rw-rw-rw-   0        0        0        0 2023-04-05 06:50:44.000000 DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:23:37.756776 DA4RDM_Vis_ProcessBased-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:23:37.517227 DA4RDM_Vis_ProcessBased-0.1.6/DA4RDM_Vis_ProcessBased.egg-info/
+-rw-rw-rw-   0        0        0     4140 2023-04-11 15:23:37.000000 DA4RDM_Vis_ProcessBased-0.1.6/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2023-04-11 15:23:37.000000 DA4RDM_Vis_ProcessBased-0.1.6/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:23:37.000000 DA4RDM_Vis_ProcessBased-0.1.6/DA4RDM_Vis_ProcessBased.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-11 15:23:37.000000 DA4RDM_Vis_ProcessBased-0.1.6/DA4RDM_Vis_ProcessBased.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1072 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4140 2023-04-11 15:23:37.758225 DA4RDM_Vis_ProcessBased-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3678 2023-04-11 15:16:13.000000 DA4RDM_Vis_ProcessBased-0.1.6/README.md
+-rw-rw-rw-   0        0        0      473 2023-04-11 15:17:34.000000 DA4RDM_Vis_ProcessBased-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      303 2023-04-11 15:23:37.765709 DA4RDM_Vis_ProcessBased-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      999 2023-04-11 15:18:08.000000 DA4RDM_Vis_ProcessBased-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:23:37.445669 DA4RDM_Vis_ProcessBased-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:23:37.625092 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/
+-rw-rw-rw-   0        0        0     1764 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py
+-rw-rw-rw-   0        0        0     1351 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/Extract.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:23:37.755774 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/
+-rw-rw-rw-   0        0        0      581 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv
+-rw-rw-rw-   0        0        0      503 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Analysis.csv
+-rw-rw-rw-   0        0        0      619 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv
+-rw-rw-rw-   0        0        0      929 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv
+-rw-rw-rw-   0        0        0     1001 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv
+-rw-rw-rw-   0        0        0      687 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv
+-rw-rw-rw-   0        0        0     3586 2023-04-11 15:17:03.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/Visualize.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 11:58:19.000000 DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/__init__.py
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO` & `DA4RDM_Vis_ProcessBased-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
-Name: DA4RDM-Vis-ProcessBased
-Version: 0.1.1
-Summary: Package to get visualisation of fitness values evaluated for a given projectid analyzed on different RDLC phase process models
+Name: DA4RDM_Vis_ProcessBased
+Version: 0.1.6
+Summary: Test package to get visualisation for a given projectid as reference analyzed on different RDLC phase process models
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# DA4RDM_Vis_Processbased
+# DA4RDM_Vis_ProcessBased
 
 ## Description
-The DA4RDM_Vis_Processbased is a python based package that can be used to evaluate fitness scores based on process mining alignment algorithm applied on different RDLC phase models.     The package provides a vizualizations of the evaluated scores for the different RDLC phases as obtained for a given Project Id and other related arguments such as start and end timestamps.
+The DA4RDM_Vis_ProcessBased is a python based package that can be used to evaluate fitness scores for the RDLC phases namely Planning, Production, Analysis, Archival, Access and Reuse for a reference projectid. The fitness scores are evaluated by generating a meaningful log based on the records associated with the reference projectid, converting them into a format accepted by the pm4py process mining algorithm and then evaluating alighment based fitness values by replaying the log on models defined for each RDLC phase separately. The package finally provides a radar vizualization of the evaluated fitness scores.
 
 
 ## Installation
-The package is built using Python as a programming language and utilizes basic python packages. The package also uses the pm4py process mining package for fitness evaluations. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
+The package is built using Python as a programming language and utilizes basic python packages. The package also uses the pm4py process mining package for fitness evaluations. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the radar vizualization. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
 
-**pip install DA4RDM_Vis_Processbased**
+**pip install DA4RDM_Vis_ProcessBased**
 
 
 ## Importing the Module 
 The package has one important module **Vizualize**. This modules invokes the necessary functions from other modules that perform the tasks of data extraction, model creation, fitness evaluation and plotting. The module can be imported using the below command:
 
 ```python
-from DA4RDM_Vis_Processbased import Vizualize
+from DA4RDM_Vis_ProcessBased import Vizualize
 ```
 
 ## Usage
-As mentioned earlier, the package can be used to extract fitness values and plot them for a reference ProjectId. The fitness values corresponding to the different RDLC phase data models is evaluated for a model created for the reference ProjectId. Finally, a vizualization of the same can be generated and the path of the vizualization image file is returned. To use the package for generating the vizualization, the function **process_vis** within the module **Vizualize** should be used. The function body along with parameter information is as shown below:
+As mentioned earlier, the package can be used to extract fitness values and plot them for a reference ProjectId. The fitness value corresponding to the each RDLC phase is evaluated separately by replaying the log extracted for the reference projectid on the predefined model of the respective RDLC phase. The overall process thus evaluates 6 fitness score corresponsing to the previously mentioned RDLC phases. Finally, a radar vizualization of the same can be generated and the file is saved onto the local disk and the path of the radar vizualization image file is returned. To use the package for generating the radar vizualization, the function **process_vis** within the module **Vizualize** should be used. This method is the entry point and invokes the necessary functions that perform the evaluations and render the radar vizualization. The function body along with parameter information is as shown below:
 
 ```python
 def process_vis(dataset_user_interactions, project_id, earliest_timestamp, last_timestamp):
  """
   :param dataset_user_interactions: filepath to the csv file, a string is expected
   :param project_id: the project for which fitness are to be evaluated
   :param earliest_timestamp: the earliest timestamp to consider for filtering records 
@@ -46,13 +46,13 @@
 ```python
 from DA4RDM_Vis_ProcessBased import Visualize
 path = Visualize.process_vis('17-02-2023.csv', "f5c043a1-82bc-4c61-bce6-0acbc0062948", '2023-02-14 08:57:44.315', '2021-05-03 02:31:54.652')
 print(path)
 ```
 
 ## Output
-All the above executions invokes the function **process_vis** with the passed parameter values.The fitness values are calculated and returned by the function. The generated vizualization is saved onto the local repository of the program using the package. Finally a path is returned for the saved image.
+All the above executions invokes the function **process_vis** with the passed parameter values. The fitness values are calculated and returned by the function. The radar vizualization is generated and saved onto the local repository of the program using the package. The function finally returns the path for the saved image file as shown below:
 
 ```python
 C:\Users\avina\anaconda3\lib\site-packages\DA4RDM_Vis_ProcessBased\Radarchart.png
 ```
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt` & `DA4RDM_Vis_ProcessBased-0.1.6/DA4RDM_Vis_ProcessBased.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/LICENSE` & `DA4RDM_Vis_ProcessBased-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/PKG-INFO` & `DA4RDM_Vis_ProcessBased-0.1.6/DA4RDM_Vis_ProcessBased.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
-Name: DA4RDM_Vis_ProcessBased
-Version: 0.1.1
-Summary: Package to get visualisation of fitness values evaluated for a given projectid analyzed on different RDLC phase process models
+Name: DA4RDM-Vis-ProcessBased
+Version: 0.1.6
+Summary: Test package to get visualisation for a given projectid as reference analyzed on different RDLC phase process models
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# DA4RDM_Vis_Processbased
+# DA4RDM_Vis_ProcessBased
 
 ## Description
-The DA4RDM_Vis_Processbased is a python based package that can be used to evaluate fitness scores based on process mining alignment algorithm applied on different RDLC phase models.     The package provides a vizualizations of the evaluated scores for the different RDLC phases as obtained for a given Project Id and other related arguments such as start and end timestamps.
+The DA4RDM_Vis_ProcessBased is a python based package that can be used to evaluate fitness scores for the RDLC phases namely Planning, Production, Analysis, Archival, Access and Reuse for a reference projectid. The fitness scores are evaluated by generating a meaningful log based on the records associated with the reference projectid, converting them into a format accepted by the pm4py process mining algorithm and then evaluating alighment based fitness values by replaying the log on models defined for each RDLC phase separately. The package finally provides a radar vizualization of the evaluated fitness scores.
 
 
 ## Installation
-The package is built using Python as a programming language and utilizes basic python packages. The package also uses the pm4py process mining package for fitness evaluations. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
+The package is built using Python as a programming language and utilizes basic python packages. The package also uses the pm4py process mining package for fitness evaluations. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the radar vizualization. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
 
-**pip install DA4RDM_Vis_Processbased**
+**pip install DA4RDM_Vis_ProcessBased**
 
 
 ## Importing the Module 
 The package has one important module **Vizualize**. This modules invokes the necessary functions from other modules that perform the tasks of data extraction, model creation, fitness evaluation and plotting. The module can be imported using the below command:
 
 ```python
-from DA4RDM_Vis_Processbased import Vizualize
+from DA4RDM_Vis_ProcessBased import Vizualize
 ```
 
 ## Usage
-As mentioned earlier, the package can be used to extract fitness values and plot them for a reference ProjectId. The fitness values corresponding to the different RDLC phase data models is evaluated for a model created for the reference ProjectId. Finally, a vizualization of the same can be generated and the path of the vizualization image file is returned. To use the package for generating the vizualization, the function **process_vis** within the module **Vizualize** should be used. The function body along with parameter information is as shown below:
+As mentioned earlier, the package can be used to extract fitness values and plot them for a reference ProjectId. The fitness value corresponding to the each RDLC phase is evaluated separately by replaying the log extracted for the reference projectid on the predefined model of the respective RDLC phase. The overall process thus evaluates 6 fitness score corresponsing to the previously mentioned RDLC phases. Finally, a radar vizualization of the same can be generated and the file is saved onto the local disk and the path of the radar vizualization image file is returned. To use the package for generating the radar vizualization, the function **process_vis** within the module **Vizualize** should be used. This method is the entry point and invokes the necessary functions that perform the evaluations and render the radar vizualization. The function body along with parameter information is as shown below:
 
 ```python
 def process_vis(dataset_user_interactions, project_id, earliest_timestamp, last_timestamp):
  """
   :param dataset_user_interactions: filepath to the csv file, a string is expected
   :param project_id: the project for which fitness are to be evaluated
   :param earliest_timestamp: the earliest timestamp to consider for filtering records 
@@ -46,13 +46,13 @@
 ```python
 from DA4RDM_Vis_ProcessBased import Visualize
 path = Visualize.process_vis('17-02-2023.csv', "f5c043a1-82bc-4c61-bce6-0acbc0062948", '2023-02-14 08:57:44.315', '2021-05-03 02:31:54.652')
 print(path)
 ```
 
 ## Output
-All the above executions invokes the function **process_vis** with the passed parameter values.The fitness values are calculated and returned by the function. The generated vizualization is saved onto the local repository of the program using the package. Finally a path is returned for the saved image.
+All the above executions invokes the function **process_vis** with the passed parameter values. The fitness values are calculated and returned by the function. The radar vizualization is generated and saved onto the local repository of the program using the package. The function finally returns the path for the saved image file as shown below:
 
 ```python
 C:\Users\avina\anaconda3\lib\site-packages\DA4RDM_Vis_ProcessBased\Radarchart.png
 ```
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/README.md` & `DA4RDM_Vis_ProcessBased-0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# DA4RDM_Vis_Processbased
+# DA4RDM_Vis_ProcessBased
 
 ## Description
-The DA4RDM_Vis_Processbased is a python based package that can be used to evaluate fitness scores based on process mining alignment algorithm applied on different RDLC phase models.     The package provides a vizualizations of the evaluated scores for the different RDLC phases as obtained for a given Project Id and other related arguments such as start and end timestamps.
+The DA4RDM_Vis_ProcessBased is a python based package that can be used to evaluate fitness scores for the RDLC phases namely Planning, Production, Analysis, Archival, Access and Reuse for a reference projectid. The fitness scores are evaluated by generating a meaningful log based on the records associated with the reference projectid, converting them into a format accepted by the pm4py process mining algorithm and then evaluating alighment based fitness values by replaying the log on models defined for each RDLC phase separately. The package finally provides a radar vizualization of the evaluated fitness scores.
 
 
 ## Installation
-The package is built using Python as a programming language and utilizes basic python packages. The package also uses the pm4py process mining package for fitness evaluations. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
+The package is built using Python as a programming language and utilizes basic python packages. The package also uses the pm4py process mining package for fitness evaluations. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the radar vizualization. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
 
-**pip install DA4RDM_Vis_Processbased**
+**pip install DA4RDM_Vis_ProcessBased**
 
 
 ## Importing the Module 
 The package has one important module **Vizualize**. This modules invokes the necessary functions from other modules that perform the tasks of data extraction, model creation, fitness evaluation and plotting. The module can be imported using the below command:
 
 ```python
-from DA4RDM_Vis_Processbased import Vizualize
+from DA4RDM_Vis_ProcessBased import Vizualize
 ```
 
 ## Usage
-As mentioned earlier, the package can be used to extract fitness values and plot them for a reference ProjectId. The fitness values corresponding to the different RDLC phase data models is evaluated for a model created for the reference ProjectId. Finally, a vizualization of the same can be generated and the path of the vizualization image file is returned. To use the package for generating the vizualization, the function **process_vis** within the module **Vizualize** should be used. The function body along with parameter information is as shown below:
+As mentioned earlier, the package can be used to extract fitness values and plot them for a reference ProjectId. The fitness value corresponding to the each RDLC phase is evaluated separately by replaying the log extracted for the reference projectid on the predefined model of the respective RDLC phase. The overall process thus evaluates 6 fitness score corresponsing to the previously mentioned RDLC phases. Finally, a radar vizualization of the same can be generated and the file is saved onto the local disk and the path of the radar vizualization image file is returned. To use the package for generating the radar vizualization, the function **process_vis** within the module **Vizualize** should be used. This method is the entry point and invokes the necessary functions that perform the evaluations and render the radar vizualization. The function body along with parameter information is as shown below:
 
 ```python
 def process_vis(dataset_user_interactions, project_id, earliest_timestamp, last_timestamp):
  """
   :param dataset_user_interactions: filepath to the csv file, a string is expected
   :param project_id: the project for which fitness are to be evaluated
   :param earliest_timestamp: the earliest timestamp to consider for filtering records 
@@ -36,13 +36,13 @@
 ```python
 from DA4RDM_Vis_ProcessBased import Visualize
 path = Visualize.process_vis('17-02-2023.csv', "f5c043a1-82bc-4c61-bce6-0acbc0062948", '2023-02-14 08:57:44.315', '2021-05-03 02:31:54.652')
 print(path)
 ```
 
 ## Output
-All the above executions invokes the function **process_vis** with the passed parameter values.The fitness values are calculated and returned by the function. The generated vizualization is saved onto the local repository of the program using the package. Finally a path is returned for the saved image.
+All the above executions invokes the function **process_vis** with the passed parameter values. The fitness values are calculated and returned by the function. The radar vizualization is generated and saved onto the local repository of the program using the package. The function finally returns the path for the saved image file as shown below:
 
 ```python
 C:\Users\avina\anaconda3\lib\site-packages\DA4RDM_Vis_ProcessBased\Radarchart.png
 ```
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/setup.py` & `DA4RDM_Vis_ProcessBased-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from setuptools import setup, find_packages
-
-
-def readme():
-    with open('README.md') as f:
-        return f.read()
-
-
-setup(name='DA4RDM_Vis_ProcessBased',
-      version='0.1.1',
-      description='Package to get visualisation of fitness values evaluated for a given projectid analyzed '
-                  'on different RDLC phase process models',
-      long_description=readme(),
-      classifiers=[
-          "Programming Language :: Python :: 3.9",
-          "License :: OSI Approved :: MIT License",
-          "Operating System :: OS Independent",	
-      ],
-      packages = ['DA4RDM_Vis_ProcessBased'],
-      package_dir = {'DA4RDM_Vis_ProcessBased': 'src/DA4RDM_Vis_ProcessBased'},
-      package_data={'DA4RDM_Vis_ProcessBased': ['PhaseData/*.csv']},
-      dependencies=[
-        'plotly-express>==0.4.1',
-        'numpy >= 1.18.1',
-        'pandas >= 1.5.3',
-        'python_dateutil >= 2.8.2',
-        'pm4py >= 2.7.0',
-        'kaleido >= 0.2.1',
-        ],
-      include_package_data=True,
-      )
+from setuptools import setup, find_packages
+
+
+def readme():
+    with open('README.md') as f:
+        return f.read()
+
+
+setup(name='DA4RDM_Vis_ProcessBased',
+      version='0.1.6',
+      description='Test package to get visualisation for a given projectid as reference analyzed '
+                  'on different RDLC phase process models',
+      long_description=readme(),
+      classifiers=[
+          "Programming Language :: Python :: 3.9",
+          "License :: OSI Approved :: MIT License",
+          "Operating System :: OS Independent",	
+      ],
+      packages = ['DA4RDM_Vis_ProcessBased'],
+      package_dir = {'DA4RDM_Vis_ProcessBased': 'src/DA4RDM_Vis_ProcessBased'},
+      package_data={'DA4RDM_Vis_ProcessBased': ['PhaseData/*.csv']},
+      dependencies=[
+        'plotly-express>==0.4.1',
+        'numpy >= 1.18.1',
+        'pandas >= 1.5.3',
+        'python_dateutil >= 2.8.2',
+        'pm4py >= 2.7.0',
+        'kaleido >= 0.2.1',
+        ],
+      include_package_data=True,
+      )
```

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/Evaluate_Fitness.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/Extract.py` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/Extract.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Access.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Archival.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Planning.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Production.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/PhaseData/Reuse.csv`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_ProcessBased-0.1.1/src/DA4RDM_Vis_ProcessBased/Visualize.py` & `DA4RDM_Vis_ProcessBased-0.1.6/src/DA4RDM_Vis_ProcessBased/Visualize.py`

 * *Files identical despite different names*

