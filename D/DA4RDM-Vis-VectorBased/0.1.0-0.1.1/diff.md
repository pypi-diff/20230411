# Comparing `tmp/DA4RDM_Vis_VectorBased-0.1.0.tar.gz` & `tmp/DA4RDM_Vis_VectorBased-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DA4RDM_Vis_VectorBased-0.1.0.tar", last modified: Mon Apr 10 15:38:25 2023, max compression
+gzip compressed data, was "DA4RDM_Vis_VectorBased-0.1.1.tar", last modified: Tue Apr 11 15:20:15 2023, max compression
```

## Comparing `DA4RDM_Vis_VectorBased-0.1.0.tar` & `DA4RDM_Vis_VectorBased-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 15:38:25.444446 DA4RDM_Vis_VectorBased-0.1.0/
--rw-rw-rw-   0        0        0     1072 2023-04-10 15:36:51.000000 DA4RDM_Vis_VectorBased-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    10022 2023-04-10 15:38:25.443444 DA4RDM_Vis_VectorBased-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9423 2023-04-10 15:36:36.000000 DA4RDM_Vis_VectorBased-0.1.0/README.md
--rw-rw-rw-   0        0        0      653 2023-04-10 15:37:00.000000 DA4RDM_Vis_VectorBased-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 15:38:25.445446 DA4RDM_Vis_VectorBased-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 15:38:25.335915 DA4RDM_Vis_VectorBased-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 15:38:25.393447 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/
--rw-rw-rw-   0        0        0     8233 2023-04-10 15:03:00.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Evaluate.py
--rw-rw-rw-   0        0        0      834 2023-04-10 15:08:43.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Extract.py
--rw-rw-rw-   0        0        0      841 2023-04-10 15:08:35.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Timestamp.py
--rw-rw-rw-   0        0        0     1627 2023-04-10 15:03:04.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Visualize.py
--rw-rw-rw-   0        0        0        0 2023-04-10 14:45:21.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 15:38:25.438444 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased.egg-info/
--rw-rw-rw-   0        0        0    10022 2023-04-10 15:38:25.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-04-10 15:38:25.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 15:38:25.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-10 15:38:25.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-10 15:38:25.000000 DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-10 14:45:21.000000 DA4RDM_Vis_VectorBased-0.1.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:20:15.534898 DA4RDM_Vis_VectorBased-0.1.1/
+-rw-rw-rw-   0        0        0     1072 2023-04-10 15:36:51.000000 DA4RDM_Vis_VectorBased-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9239 2023-04-11 15:20:15.533895 DA4RDM_Vis_VectorBased-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8654 2023-04-11 15:13:28.000000 DA4RDM_Vis_VectorBased-0.1.1/README.md
+-rw-rw-rw-   0        0        0      653 2023-04-11 15:19:06.000000 DA4RDM_Vis_VectorBased-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:20:15.536410 DA4RDM_Vis_VectorBased-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 15:20:15.129499 DA4RDM_Vis_VectorBased-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:20:15.400092 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/
+-rw-rw-rw-   0        0        0     8233 2023-04-10 15:03:00.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Evaluate.py
+-rw-rw-rw-   0        0        0      834 2023-04-10 15:08:43.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Extract.py
+-rw-rw-rw-   0        0        0      841 2023-04-10 15:08:35.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Timestamp.py
+-rw-rw-rw-   0        0        0     1627 2023-04-10 15:03:04.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Visualize.py
+-rw-rw-rw-   0        0        0        0 2023-04-10 14:45:21.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:20:15.526572 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased.egg-info/
+-rw-rw-rw-   0        0        0     9239 2023-04-11 15:20:14.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-04-11 15:20:14.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:20:14.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-11 15:20:14.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-11 15:20:14.000000 DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-10 14:45:21.000000 DA4RDM_Vis_VectorBased-0.1.1/src/__init__.py
```

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/LICENSE` & `DA4RDM_Vis_VectorBased-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/PKG-INFO` & `DA4RDM_Vis_VectorBased-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: DA4RDM_Vis_VectorBased
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package that can be used to perform RDLC analysis by determining the correlations for the different phases of the development life cycle.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DA4RDM_Vis_VectorBased
 
 ## Description
-The DA4RDM_Vis_VectorBased is a python based package that allows extracting correlation data for to the different phases of Research Development Life Cycle process. The package can also be used to get vizualizations of the different correlation values for the different RDLC phases as obtained for a given Project Id and other related arguments.
+The DA4RDM_Vis_VectorBased is a python based package that allows extracting correlation data for to the different phases of Research Development Life Cycle process. The package can also be used to get radar vizualizations of the different correlation values for the different RDLC phases as obtained for a given Project Id and other related arguments.
 
 
 ## Installation
-The package is built using Python as a programming language and utilizes basic python packages. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
+The package is built using Python as a programming language and utilizes basic python packages. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the radar vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The package can be installed using the pip command provided below.
 
 **pip install DA4RDM_Vis_VectorBased**
 
 
 ## Importing the Modules 
-The package has two important modules **Evaluate** and **Vizualize** .The first module invokes the necessary functions that performs the task of data extraction, model creation and fitness evaluation and finally returns the correlation values. The second module uses the values retrieved from module Evaluate to provide the final visualization. The modules can be imported using the below command:
+The package has two important modules **Evaluate** and **Vizualize** .The first module invokes the necessary functions that performs the task of data extraction, model creation and fitness evaluation and finally returns the correlation values. The second module uses the values retrieved from module Evaluate to provide the final radar visualization. The modules can be imported using the below command:
 
 ```python
 from DA4RDM_Vis_VectorBased import Evaluate
 from DA4RDM_Vis_VectorBased import Vizualize
 ```
 
 ## Usage
-As mentioned above, the package has two major functionalities as listed below:
+As mentioned above, the package has two major functionalities as listed below:<br>
 **1.** Extracting correlation data for the project. the correlation data is returned as a dataframe consisting of the correlation values corresponding to each RDLC phase corresponding to the project. To use the package for retreiving the correlation data, the function **eval_corr** within the module **Evaluate** should be used. The function body along with parameter information is as shown below:
 
 ```python
 def eval_corr(data_path, project_id, start_date="", end_date="", operation_list_path="",
               eval_feature="pearson", eval_type="binary"):
  """
   :param data_path,: filepath to the input data as a csv file, a string is expected
-  :param project_id: the project for which fcorrelations are to be evaluated
+  :param project_id: the project for which correlations are to be evaluated
   :param start_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
   :param end_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
   :param operation_list_path: filepath to the json file containing list of operations and the vectors for each RDLC phase(default is defined in the function body)
   :param eval_feature: The distance feature to be used for similarity evaluation, either pearson(default) or cosine
   :param eval_type: The type of  distance feature to be used for similarity evaluation, either binary(default) or weighted
  """
 ```
@@ -89,66 +89,52 @@
 Below is an execution of the function with all parameters provided.
 ```python
 from DA4RDM_Vis_VectorBased import Evaluate
 
 correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "OperationalDatamodify.json", 'cosine', 'binary')
 print(correlation)
 ```
-Below is an execution of the function with only required parameters provided.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
-print(correlation)
-```
-Below is an example of function execution with no value passed for the parameter corresponding to the path of operational data json file. In order to skip a optional argument, the parameter value should be passed as an empty string at its position. Please refer below for example.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "", 'cosine', 'binary')
-print(correlation)
-```
 
 ## Output
 All the above executions invokes the function **eval_corr** with the passed parameter values.The correlation values are calculated and returned by the function. Finally, the results received will be printed as shown below.
 
 ```python
    RDLC_phase  Correlation_value
 0    Planning           0.966092
 1  Production           0.000000
 2    Analysis           0.000000
 3    Archival           0.188982
 4      Access           0.356348
 5       Reuse           0.000000
 ```
 
-**2.** Generating vizualizations or transforming the correlation data retreived using the eval_corr function as discussed in the sections above. To get a vizualization of the results the **visualize** function within the module Vizualize should be used. The function body along with parameter information is as shown below:
+**2.** Generating radar vizualizations or transforming the correlation data retreived using the eval_corr function as discussed in the sections above. To get a vizualization of the results the **visualize** function within the module Vizualize should be used. The function body along with parameter information is as shown below:
 
 ```python
 def visualize(corr_data, save_option):
  """
   :param corr_data: The correlation response data received as output from finction eval_corr
   :param save_option: the type of file to be saved(options are either png, jpeg, pdf or json)
  """
 ```
 
- This function accepts a dataframe with correlation data and a vizualization format as required parameters and provides relevant visualizazio. The user can choose from the various allowed formats such are jpeg, png, pdf and json.
+ This function accepts a dataframe with correlation data and a radar vizualization format as required parameters and provides relevant radar visualizazion. The user can choose from the various allowed formats such are jpeg, png, pdf and json.
 
 ## Example
 Below is an execution of the function with all parameters provided.
 ```python
 from DA4RDM_Vis_VectorBased import Evaluate
 from DA4RDM_Vis_VectorBased import Visualize
 
 correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
 Visualize.visualize(correlation, 'jpeg')
 ```
 
 ## Output
-If a user selects the format as jpeg, png or pdf, the result is a RadarChart vizualization of the correlation data.
+If a user selects the format as jpeg, png or pdf, the result is a radar vizualization of the correlation data.
 If json is the selected format the function outputs a json representation of the correlation values as shown below:
 ```python
 {"Similarity": {"corr_res": [0.9654746681256314, 0.3613249509436927, 0.2388835160664533, 0.5, 0.46176404435490637, 0.4037749551350624], "rdlc_phase": ["Planning", "Production", "Analysis", "Archival", "Access", "Reuse"]}}
 ```
 The generated files are saved onto the local repository of the program using the package.
```

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/README.md` & `DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,143 +1,140 @@
-# DA4RDM_Vis_VectorBased
-
-## Description
-The DA4RDM_Vis_VectorBased is a python based package that allows extracting correlation data for to the different phases of Research Development Life Cycle process. The package can also be used to get vizualizations of the different correlation values for the different RDLC phases as obtained for a given Project Id and other related arguments.
-
-
-## Installation
-The package is built using Python as a programming language and utilizes basic python packages. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
-
-**pip install DA4RDM_Vis_VectorBased**
-
-
-## Importing the Modules 
-The package has two important modules **Evaluate** and **Vizualize** .The first module invokes the necessary functions that performs the task of data extraction, model creation and fitness evaluation and finally returns the correlation values. The second module uses the values retrieved from module Evaluate to provide the final visualization. The modules can be imported using the below command:
-
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-from DA4RDM_Vis_VectorBased import Vizualize
-```
-
-## Usage
-As mentioned above, the package has two major functionalities as listed below:
-**1.** Extracting correlation data for the project. the correlation data is returned as a dataframe consisting of the correlation values corresponding to each RDLC phase corresponding to the project. To use the package for retreiving the correlation data, the function **eval_corr** within the module **Evaluate** should be used. The function body along with parameter information is as shown below:
-
-```python
-def eval_corr(data_path, project_id, start_date="", end_date="", operation_list_path="",
-              eval_feature="pearson", eval_type="binary"):
- """
-  :param data_path,: filepath to the input data as a csv file, a string is expected
-  :param project_id: the project for which fcorrelations are to be evaluated
-  :param start_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
-  :param end_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
-  :param operation_list_path: filepath to the json file containing list of operations and the vectors for each RDLC phase(default is defined in the function body)
-  :param eval_feature: The distance feature to be used for similarity evaluation, either pearson(default) or cosine
-  :param eval_type: The type of  distance feature to be used for similarity evaluation, either binary(default) or weighted
- """
-```
-
-The function **eval_corr** accepts two mandatory positional arguments namely the path for the event log and the Project Id. The project id must be provided to uniquely identify the projects.The optional arguments include start and end date, path for the operational data json file that will be used to build the operational list and RDLC phase identifier, the evaluation feature and type to be used for calculating the similarity. The operationa data is computed from a defalut json file if an external file path is not specified by the user. If the user wishes to provide a customized operational data file then the path must be provided at the arguments position while function invoking. Please refer to the file format as shown below.
-```python
-{
-"Operation_List": ["Add Project", "Edit Project", "Open Resource(RCV)", "Add Resource", "Edit Resource", "Delete Resource", "Upload File",  "Upload MD", "Download File", "View MD", "Delete File", "Update File", "Update MD", "Open User Management", "View Users", "Add Member", "Change Role", "Remove User", "Open Search", "View Search Results", "PID Enquiry", "Create Application Profile",  "Admin Project Quota Change", "Owner Project Quota Change", "Owner Resource Quota Change", "Invite External User", "Archive Resource", "Unarchive Resource", "Merge Request" ],
-"Planning": [
-        1,        1,        0,        1,        1,        1,        0,        0,        0,
-        0,        0,        0,        0,        1,        1,        1,        1,        1,
-        0,        0,        0,        1,        1,        1,        1,        1,        0,
-        0,        0    ],
-"Production": [
-        0,        0,        0,        0,        0,        0,        1,        1,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        1    ],
-"Analysis": [
-        0,        0,        0,        0,        0,        0,        0,        0,        1,
-        1,        1,        1,        1,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        1,        1    ],
-"Archival": [
-        0,        0,        0,        0,        1,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        1,
-        0,        0
-    ],
-"Access": [
-        0,        0,        1,        0,        0,        0,        0,        0,        1,
-        1,        0,        0,        0,        1,        1,        1,        0,        0,
-        1,        1,        0,        0,        0,        0,        0,        1,        0,
-        0,        0    ],
-"Reuse": [
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        1,        0,        0,        0,        0,        0,        0,
-        0,        1    ]
-}
-```
-
-## Example	
-Below is an execution of the function with all parameters provided.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "OperationalDatamodify.json", 'cosine', 'binary')
-print(correlation)
-```
-Below is an execution of the function with only required parameters provided.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
-print(correlation)
-```
-Below is an example of function execution with no value passed for the parameter corresponding to the path of operational data json file. In order to skip a optional argument, the parameter value should be passed as an empty string at its position. Please refer below for example.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "", 'cosine', 'binary')
-print(correlation)
-```
-
-## Output
-All the above executions invokes the function **eval_corr** with the passed parameter values.The correlation values are calculated and returned by the function. Finally, the results received will be printed as shown below.
-
-```python
-   RDLC_phase  Correlation_value
-0    Planning           0.966092
-1  Production           0.000000
-2    Analysis           0.000000
-3    Archival           0.188982
-4      Access           0.356348
-5       Reuse           0.000000
-```
-
-**2.** Generating vizualizations or transforming the correlation data retreived using the eval_corr function as discussed in the sections above. To get a vizualization of the results the **visualize** function within the module Vizualize should be used. The function body along with parameter information is as shown below:
-
-```python
-def visualize(corr_data, save_option):
- """
-  :param corr_data: The correlation response data received as output from finction eval_corr
-  :param save_option: the type of file to be saved(options are either png, jpeg, pdf or json)
- """
-```
-
- This function accepts a dataframe with correlation data and a vizualization format as required parameters and provides relevant visualizazio. The user can choose from the various allowed formats such are jpeg, png, pdf and json.
-
-## Example
-Below is an execution of the function with all parameters provided.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-from DA4RDM_Vis_VectorBased import Visualize
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
-Visualize.visualize(correlation, 'jpeg')
-```
-
-## Output
-If a user selects the format as jpeg, png or pdf, the result is a RadarChart vizualization of the correlation data.
-If json is the selected format the function outputs a json representation of the correlation values as shown below:
-```python
-{"Similarity": {"corr_res": [0.9654746681256314, 0.3613249509436927, 0.2388835160664533, 0.5, 0.46176404435490637, 0.4037749551350624], "rdlc_phase": ["Planning", "Production", "Analysis", "Archival", "Access", "Reuse"]}}
-```
-The generated files are saved onto the local repository of the program using the package.
-
-
+Metadata-Version: 2.1
+Name: DA4RDM-Vis-VectorBased
+Version: 0.1.1
+Summary: Package that can be used to perform RDLC analysis by determining the correlations for the different phases of the development life cycle.
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DA4RDM_Vis_VectorBased
+
+## Description
+The DA4RDM_Vis_VectorBased is a python based package that allows extracting correlation data for to the different phases of Research Development Life Cycle process. The package can also be used to get radar vizualizations of the different correlation values for the different RDLC phases as obtained for a given Project Id and other related arguments.
+
+
+## Installation
+The package is built using Python as a programming language and utilizes basic python packages. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the radar vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The package can be installed using the pip command provided below.
+
+**pip install DA4RDM_Vis_VectorBased**
+
+
+## Importing the Modules 
+The package has two important modules **Evaluate** and **Vizualize** .The first module invokes the necessary functions that performs the task of data extraction, model creation and fitness evaluation and finally returns the correlation values. The second module uses the values retrieved from module Evaluate to provide the final radar visualization. The modules can be imported using the below command:
+
+```python
+from DA4RDM_Vis_VectorBased import Evaluate
+from DA4RDM_Vis_VectorBased import Vizualize
+```
+
+## Usage
+As mentioned above, the package has two major functionalities as listed below:<br>
+**1.** Extracting correlation data for the project. the correlation data is returned as a dataframe consisting of the correlation values corresponding to each RDLC phase corresponding to the project. To use the package for retreiving the correlation data, the function **eval_corr** within the module **Evaluate** should be used. The function body along with parameter information is as shown below:
+
+```python
+def eval_corr(data_path, project_id, start_date="", end_date="", operation_list_path="",
+              eval_feature="pearson", eval_type="binary"):
+ """
+  :param data_path,: filepath to the input data as a csv file, a string is expected
+  :param project_id: the project for which correlations are to be evaluated
+  :param start_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
+  :param end_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
+  :param operation_list_path: filepath to the json file containing list of operations and the vectors for each RDLC phase(default is defined in the function body)
+  :param eval_feature: The distance feature to be used for similarity evaluation, either pearson(default) or cosine
+  :param eval_type: The type of  distance feature to be used for similarity evaluation, either binary(default) or weighted
+ """
+```
+
+The function **eval_corr** accepts two mandatory positional arguments namely the path for the event log and the Project Id. The project id must be provided to uniquely identify the projects.The optional arguments include start and end date, path for the operational data json file that will be used to build the operational list and RDLC phase identifier, the evaluation feature and type to be used for calculating the similarity. The operationa data is computed from a defalut json file if an external file path is not specified by the user. If the user wishes to provide a customized operational data file then the path must be provided at the arguments position while function invoking. Please refer to the file format as shown below.
+```python
+{
+"Operation_List": ["Add Project", "Edit Project", "Open Resource(RCV)", "Add Resource", "Edit Resource", "Delete Resource", "Upload File",  "Upload MD", "Download File", "View MD", "Delete File", "Update File", "Update MD", "Open User Management", "View Users", "Add Member", "Change Role", "Remove User", "Open Search", "View Search Results", "PID Enquiry", "Create Application Profile",  "Admin Project Quota Change", "Owner Project Quota Change", "Owner Resource Quota Change", "Invite External User", "Archive Resource", "Unarchive Resource", "Merge Request" ],
+"Planning": [
+        1,        1,        0,        1,        1,        1,        0,        0,        0,
+        0,        0,        0,        0,        1,        1,        1,        1,        1,
+        0,        0,        0,        1,        1,        1,        1,        1,        0,
+        0,        0    ],
+"Production": [
+        0,        0,        0,        0,        0,        0,        1,        1,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        1    ],
+"Analysis": [
+        0,        0,        0,        0,        0,        0,        0,        0,        1,
+        1,        1,        1,        1,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        1,        1    ],
+"Archival": [
+        0,        0,        0,        0,        1,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        1,
+        0,        0
+    ],
+"Access": [
+        0,        0,        1,        0,        0,        0,        0,        0,        1,
+        1,        0,        0,        0,        1,        1,        1,        0,        0,
+        1,        1,        0,        0,        0,        0,        0,        1,        0,
+        0,        0    ],
+"Reuse": [
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        1,        0,        0,        0,        0,        0,        0,
+        0,        1    ]
+}
+```
+
+## Example	
+Below is an execution of the function with all parameters provided.
+```python
+from DA4RDM_Vis_VectorBased import Evaluate
+
+correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "OperationalDatamodify.json", 'cosine', 'binary')
+print(correlation)
+```
+
+## Output
+All the above executions invokes the function **eval_corr** with the passed parameter values.The correlation values are calculated and returned by the function. Finally, the results received will be printed as shown below.
+
+```python
+   RDLC_phase  Correlation_value
+0    Planning           0.966092
+1  Production           0.000000
+2    Analysis           0.000000
+3    Archival           0.188982
+4      Access           0.356348
+5       Reuse           0.000000
+```
+
+**2.** Generating radar vizualizations or transforming the correlation data retreived using the eval_corr function as discussed in the sections above. To get a vizualization of the results the **visualize** function within the module Vizualize should be used. The function body along with parameter information is as shown below:
+
+```python
+def visualize(corr_data, save_option):
+ """
+  :param corr_data: The correlation response data received as output from finction eval_corr
+  :param save_option: the type of file to be saved(options are either png, jpeg, pdf or json)
+ """
+```
+
+ This function accepts a dataframe with correlation data and a radar vizualization format as required parameters and provides relevant radar visualizazion. The user can choose from the various allowed formats such are jpeg, png, pdf and json.
+
+## Example
+Below is an execution of the function with all parameters provided.
+```python
+from DA4RDM_Vis_VectorBased import Evaluate
+from DA4RDM_Vis_VectorBased import Visualize
+
+correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
+Visualize.visualize(correlation, 'jpeg')
+```
+
+## Output
+If a user selects the format as jpeg, png or pdf, the result is a radar vizualization of the correlation data.
+If json is the selected format the function outputs a json representation of the correlation values as shown below:
+```python
+{"Similarity": {"corr_res": [0.9654746681256314, 0.3613249509436927, 0.2388835160664533, 0.5, 0.46176404435490637, 0.4037749551350624], "rdlc_phase": ["Planning", "Production", "Analysis", "Archival", "Access", "Reuse"]}}
+```
+The generated files are saved onto the local repository of the program using the package.
+
+
```

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/pyproject.toml` & `DA4RDM_Vis_VectorBased-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DA4RDM_Vis_VectorBased"
-version = "0.1.0"
+version = "0.1.1"
 description = "Package that can be used to perform RDLC analysis by determining the correlations for the different phases of the development life cycle."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Evaluate.py` & `DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Evaluate.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Extract.py` & `DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Extract.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Timestamp.py` & `DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Timestamp.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased/Visualize.py` & `DA4RDM_Vis_VectorBased-0.1.1/src/DA4RDM_Vis_VectorBased/Visualize.py`

 * *Files identical despite different names*

### Comparing `DA4RDM_Vis_VectorBased-0.1.0/src/DA4RDM_Vis_VectorBased.egg-info/PKG-INFO` & `DA4RDM_Vis_VectorBased-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,154 +1,129 @@
-Metadata-Version: 2.1
-Name: DA4RDM-Vis-VectorBased
-Version: 0.1.0
-Summary: Package that can be used to perform RDLC analysis by determining the correlations for the different phases of the development life cycle.
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# DA4RDM_Vis_VectorBased
-
-## Description
-The DA4RDM_Vis_VectorBased is a python based package that allows extracting correlation data for to the different phases of Research Development Life Cycle process. The package can also be used to get vizualizations of the different correlation values for the different RDLC phases as obtained for a given Project Id and other related arguments.
-
-
-## Installation
-The package is built using Python as a programming language and utilizes basic python packages. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The test package can be installed using the pip command provided below.
-
-**pip install DA4RDM_Vis_VectorBased**
-
-
-## Importing the Modules 
-The package has two important modules **Evaluate** and **Vizualize** .The first module invokes the necessary functions that performs the task of data extraction, model creation and fitness evaluation and finally returns the correlation values. The second module uses the values retrieved from module Evaluate to provide the final visualization. The modules can be imported using the below command:
-
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-from DA4RDM_Vis_VectorBased import Vizualize
-```
-
-## Usage
-As mentioned above, the package has two major functionalities as listed below:
-**1.** Extracting correlation data for the project. the correlation data is returned as a dataframe consisting of the correlation values corresponding to each RDLC phase corresponding to the project. To use the package for retreiving the correlation data, the function **eval_corr** within the module **Evaluate** should be used. The function body along with parameter information is as shown below:
-
-```python
-def eval_corr(data_path, project_id, start_date="", end_date="", operation_list_path="",
-              eval_feature="pearson", eval_type="binary"):
- """
-  :param data_path,: filepath to the input data as a csv file, a string is expected
-  :param project_id: the project for which fcorrelations are to be evaluated
-  :param start_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
-  :param end_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
-  :param operation_list_path: filepath to the json file containing list of operations and the vectors for each RDLC phase(default is defined in the function body)
-  :param eval_feature: The distance feature to be used for similarity evaluation, either pearson(default) or cosine
-  :param eval_type: The type of  distance feature to be used for similarity evaluation, either binary(default) or weighted
- """
-```
-
-The function **eval_corr** accepts two mandatory positional arguments namely the path for the event log and the Project Id. The project id must be provided to uniquely identify the projects.The optional arguments include start and end date, path for the operational data json file that will be used to build the operational list and RDLC phase identifier, the evaluation feature and type to be used for calculating the similarity. The operationa data is computed from a defalut json file if an external file path is not specified by the user. If the user wishes to provide a customized operational data file then the path must be provided at the arguments position while function invoking. Please refer to the file format as shown below.
-```python
-{
-"Operation_List": ["Add Project", "Edit Project", "Open Resource(RCV)", "Add Resource", "Edit Resource", "Delete Resource", "Upload File",  "Upload MD", "Download File", "View MD", "Delete File", "Update File", "Update MD", "Open User Management", "View Users", "Add Member", "Change Role", "Remove User", "Open Search", "View Search Results", "PID Enquiry", "Create Application Profile",  "Admin Project Quota Change", "Owner Project Quota Change", "Owner Resource Quota Change", "Invite External User", "Archive Resource", "Unarchive Resource", "Merge Request" ],
-"Planning": [
-        1,        1,        0,        1,        1,        1,        0,        0,        0,
-        0,        0,        0,        0,        1,        1,        1,        1,        1,
-        0,        0,        0,        1,        1,        1,        1,        1,        0,
-        0,        0    ],
-"Production": [
-        0,        0,        0,        0,        0,        0,        1,        1,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        1    ],
-"Analysis": [
-        0,        0,        0,        0,        0,        0,        0,        0,        1,
-        1,        1,        1,        1,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        1,        1    ],
-"Archival": [
-        0,        0,        0,        0,        1,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        1,
-        0,        0
-    ],
-"Access": [
-        0,        0,        1,        0,        0,        0,        0,        0,        1,
-        1,        0,        0,        0,        1,        1,        1,        0,        0,
-        1,        1,        0,        0,        0,        0,        0,        1,        0,
-        0,        0    ],
-"Reuse": [
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        0,        0,        0,        0,        0,        0,        0,
-        0,        0,        1,        0,        0,        0,        0,        0,        0,
-        0,        1    ]
-}
-```
-
-## Example	
-Below is an execution of the function with all parameters provided.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "OperationalDatamodify.json", 'cosine', 'binary')
-print(correlation)
-```
-Below is an execution of the function with only required parameters provided.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
-print(correlation)
-```
-Below is an example of function execution with no value passed for the parameter corresponding to the path of operational data json file. In order to skip a optional argument, the parameter value should be passed as an empty string at its position. Please refer below for example.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "", 'cosine', 'binary')
-print(correlation)
-```
-
-## Output
-All the above executions invokes the function **eval_corr** with the passed parameter values.The correlation values are calculated and returned by the function. Finally, the results received will be printed as shown below.
-
-```python
-   RDLC_phase  Correlation_value
-0    Planning           0.966092
-1  Production           0.000000
-2    Analysis           0.000000
-3    Archival           0.188982
-4      Access           0.356348
-5       Reuse           0.000000
-```
-
-**2.** Generating vizualizations or transforming the correlation data retreived using the eval_corr function as discussed in the sections above. To get a vizualization of the results the **visualize** function within the module Vizualize should be used. The function body along with parameter information is as shown below:
-
-```python
-def visualize(corr_data, save_option):
- """
-  :param corr_data: The correlation response data received as output from finction eval_corr
-  :param save_option: the type of file to be saved(options are either png, jpeg, pdf or json)
- """
-```
-
- This function accepts a dataframe with correlation data and a vizualization format as required parameters and provides relevant visualizazio. The user can choose from the various allowed formats such are jpeg, png, pdf and json.
-
-## Example
-Below is an execution of the function with all parameters provided.
-```python
-from DA4RDM_Vis_VectorBased import Evaluate
-from DA4RDM_Vis_VectorBased import Visualize
-
-correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
-Visualize.visualize(correlation, 'jpeg')
-```
-
-## Output
-If a user selects the format as jpeg, png or pdf, the result is a RadarChart vizualization of the correlation data.
-If json is the selected format the function outputs a json representation of the correlation values as shown below:
-```python
-{"Similarity": {"corr_res": [0.9654746681256314, 0.3613249509436927, 0.2388835160664533, 0.5, 0.46176404435490637, 0.4037749551350624], "rdlc_phase": ["Planning", "Production", "Analysis", "Archival", "Access", "Reuse"]}}
-```
-The generated files are saved onto the local repository of the program using the package.
-
-
+# DA4RDM_Vis_VectorBased
+
+## Description
+The DA4RDM_Vis_VectorBased is a python based package that allows extracting correlation data for to the different phases of Research Development Life Cycle process. The package can also be used to get radar vizualizations of the different correlation values for the different RDLC phases as obtained for a given Project Id and other related arguments.
+
+
+## Installation
+The package is built using Python as a programming language and utilizes basic python packages. Noteworthy, it uses few visualization packages like plotly express and kaleido to get the radar vizualizations. Please make sure the necessary packages are installed before execution. Few other packages include scipy, json etc. The package can be installed using the pip command provided below.
+
+**pip install DA4RDM_Vis_VectorBased**
+
+
+## Importing the Modules 
+The package has two important modules **Evaluate** and **Vizualize** .The first module invokes the necessary functions that performs the task of data extraction, model creation and fitness evaluation and finally returns the correlation values. The second module uses the values retrieved from module Evaluate to provide the final radar visualization. The modules can be imported using the below command:
+
+```python
+from DA4RDM_Vis_VectorBased import Evaluate
+from DA4RDM_Vis_VectorBased import Vizualize
+```
+
+## Usage
+As mentioned above, the package has two major functionalities as listed below:<br>
+**1.** Extracting correlation data for the project. the correlation data is returned as a dataframe consisting of the correlation values corresponding to each RDLC phase corresponding to the project. To use the package for retreiving the correlation data, the function **eval_corr** within the module **Evaluate** should be used. The function body along with parameter information is as shown below:
+
+```python
+def eval_corr(data_path, project_id, start_date="", end_date="", operation_list_path="",
+              eval_feature="pearson", eval_type="binary"):
+ """
+  :param data_path,: filepath to the input data as a csv file, a string is expected
+  :param project_id: the project for which correlations are to be evaluated
+  :param start_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
+  :param end_date: the earliest timestamp to consider for filtering records, default is evaluated based on first ooccurence of the projectid
+  :param operation_list_path: filepath to the json file containing list of operations and the vectors for each RDLC phase(default is defined in the function body)
+  :param eval_feature: The distance feature to be used for similarity evaluation, either pearson(default) or cosine
+  :param eval_type: The type of  distance feature to be used for similarity evaluation, either binary(default) or weighted
+ """
+```
+
+The function **eval_corr** accepts two mandatory positional arguments namely the path for the event log and the Project Id. The project id must be provided to uniquely identify the projects.The optional arguments include start and end date, path for the operational data json file that will be used to build the operational list and RDLC phase identifier, the evaluation feature and type to be used for calculating the similarity. The operationa data is computed from a defalut json file if an external file path is not specified by the user. If the user wishes to provide a customized operational data file then the path must be provided at the arguments position while function invoking. Please refer to the file format as shown below.
+```python
+{
+"Operation_List": ["Add Project", "Edit Project", "Open Resource(RCV)", "Add Resource", "Edit Resource", "Delete Resource", "Upload File",  "Upload MD", "Download File", "View MD", "Delete File", "Update File", "Update MD", "Open User Management", "View Users", "Add Member", "Change Role", "Remove User", "Open Search", "View Search Results", "PID Enquiry", "Create Application Profile",  "Admin Project Quota Change", "Owner Project Quota Change", "Owner Resource Quota Change", "Invite External User", "Archive Resource", "Unarchive Resource", "Merge Request" ],
+"Planning": [
+        1,        1,        0,        1,        1,        1,        0,        0,        0,
+        0,        0,        0,        0,        1,        1,        1,        1,        1,
+        0,        0,        0,        1,        1,        1,        1,        1,        0,
+        0,        0    ],
+"Production": [
+        0,        0,        0,        0,        0,        0,        1,        1,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        1    ],
+"Analysis": [
+        0,        0,        0,        0,        0,        0,        0,        0,        1,
+        1,        1,        1,        1,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        1,        1    ],
+"Archival": [
+        0,        0,        0,        0,        1,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        1,
+        0,        0
+    ],
+"Access": [
+        0,        0,        1,        0,        0,        0,        0,        0,        1,
+        1,        0,        0,        0,        1,        1,        1,        0,        0,
+        1,        1,        0,        0,        0,        0,        0,        1,        0,
+        0,        0    ],
+"Reuse": [
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        0,        0,        0,        0,        0,        0,        0,
+        0,        0,        1,        0,        0,        0,        0,        0,        0,
+        0,        1    ]
+}
+```
+
+## Example	
+Below is an execution of the function with all parameters provided.
+```python
+from DA4RDM_Vis_VectorBased import Evaluate
+
+correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A', '2021-04-28', '2023-04-28', "OperationalDatamodify.json", 'cosine', 'binary')
+print(correlation)
+```
+
+## Output
+All the above executions invokes the function **eval_corr** with the passed parameter values.The correlation values are calculated and returned by the function. Finally, the results received will be printed as shown below.
+
+```python
+   RDLC_phase  Correlation_value
+0    Planning           0.966092
+1  Production           0.000000
+2    Analysis           0.000000
+3    Archival           0.188982
+4      Access           0.356348
+5       Reuse           0.000000
+```
+
+**2.** Generating radar vizualizations or transforming the correlation data retreived using the eval_corr function as discussed in the sections above. To get a vizualization of the results the **visualize** function within the module Vizualize should be used. The function body along with parameter information is as shown below:
+
+```python
+def visualize(corr_data, save_option):
+ """
+  :param corr_data: The correlation response data received as output from finction eval_corr
+  :param save_option: the type of file to be saved(options are either png, jpeg, pdf or json)
+ """
+```
+
+ This function accepts a dataframe with correlation data and a radar vizualization format as required parameters and provides relevant radar visualizazion. The user can choose from the various allowed formats such are jpeg, png, pdf and json.
+
+## Example
+Below is an execution of the function with all parameters provided.
+```python
+from DA4RDM_Vis_VectorBased import Evaluate
+from DA4RDM_Vis_VectorBased import Visualize
+
+correlation = Evaluate.eval_corr("RDM_lifecycle_analysis_-_28-04-2022.csv", 'BA1FD94A-CC71-4D32-80AE-67DD2C3BF19A')
+Visualize.visualize(correlation, 'jpeg')
+```
+
+## Output
+If a user selects the format as jpeg, png or pdf, the result is a radar vizualization of the correlation data.
+If json is the selected format the function outputs a json representation of the correlation values as shown below:
+```python
+{"Similarity": {"corr_res": [0.9654746681256314, 0.3613249509436927, 0.2388835160664533, 0.5, 0.46176404435490637, 0.4037749551350624], "rdlc_phase": ["Planning", "Production", "Analysis", "Archival", "Access", "Reuse"]}}
+```
+The generated files are saved onto the local repository of the program using the package.
+
+
```

