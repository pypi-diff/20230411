# Comparing `tmp/hyperactive-4.4.0-py3-none-any.whl.zip` & `tmp/hyperactive-4.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,30 @@
-Zip file size: 57567 bytes, number of entries: 68
--rw-rw-r--  2.0 unx      195 b- defN 23-Feb-01 18:21 hyperactive/__init__.py
--rw-rw-r--  2.0 unx     1057 b- defN 23-Feb-01 18:21 hyperactive/distribution.py
--rw-rw-r--  2.0 unx     4980 b- defN 23-Feb-01 18:21 hyperactive/hyperactive.py
+Zip file size: 60112 bytes, number of entries: 73
+-rw-rw-r--  2.0 unx      195 b- defN 23-Apr-11 05:43 hyperactive/__init__.py
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Mar-18 07:16 hyperactive/distribution.py
+-rw-rw-r--  2.0 unx     4980 b- defN 23-Apr-11 05:34 hyperactive/hyperactive.py
 -rw-rw-r--  2.0 unx     3749 b- defN 22-Dec-26 17:59 hyperactive/print_results.py
--rw-rw-r--  2.0 unx      754 b- defN 23-Feb-01 18:21 hyperactive/process.py
--rw-rw-r--  2.0 unx     2505 b- defN 23-Jan-04 13:10 hyperactive/results.py
+-rw-rw-r--  2.0 unx      754 b- defN 23-Mar-26 10:22 hyperactive/process.py
+-rw-rw-r--  2.0 unx     2505 b- defN 23-Apr-11 05:34 hyperactive/results.py
 -rw-rw-r--  2.0 unx     1416 b- defN 22-Dec-26 17:59 hyperactive/run_search.py
--rw-rw-r--  2.0 unx     3981 b- defN 22-Jan-02 09:48 hyperactive/search_space.py
+-rw-rw-r--  2.0 unx     3981 b- defN 23-Apr-11 05:34 hyperactive/search_space.py
 -rw-rw-r--  2.0 unx     1292 b- defN 23-Feb-01 18:21 hyperactive/optimizers/__init__.py
 -rw-rw-r--  2.0 unx      337 b- defN 23-Feb-26 07:03 hyperactive/optimizers/dictionary.py
--rw-rw-r--  2.0 unx     4816 b- defN 22-Nov-16 16:50 hyperactive/optimizers/hyper_gradient_conv.py
--rw-rw-r--  2.0 unx     5107 b- defN 23-Feb-01 18:21 hyperactive/optimizers/hyper_optimizer.py
--rw-rw-r--  2.0 unx     1456 b- defN 23-Feb-01 18:21 hyperactive/optimizers/objective_function.py
+-rw-rw-r--  2.0 unx     4816 b- defN 23-Apr-11 05:34 hyperactive/optimizers/hyper_gradient_conv.py
+-rw-rw-r--  2.0 unx     5107 b- defN 23-Apr-11 05:34 hyperactive/optimizers/hyper_optimizer.py
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Mar-30 10:15 hyperactive/optimizers/objective_function.py
 -rw-rw-r--  2.0 unx      825 b- defN 23-Feb-01 18:21 hyperactive/optimizers/optimizer_attributes.py
 -rw-rw-r--  2.0 unx     5103 b- defN 23-Feb-01 18:21 hyperactive/optimizers/optimizers.py
 -rw-rw-r--  2.0 unx      199 b- defN 23-Feb-01 18:21 hyperactive/optimizers/strategies/__init__.py
--rw-rw-r--  2.0 unx      573 b- defN 23-Feb-01 18:21 hyperactive/optimizers/strategies/custom_optimization_strategy.py
--rw-rw-r--  2.0 unx     3581 b- defN 23-Feb-01 18:21 hyperactive/optimizers/strategies/optimization_strategy.py
+-rw-rw-r--  2.0 unx      573 b- defN 23-Apr-11 05:34 hyperactive/optimizers/strategies/custom_optimization_strategy.py
+-rw-rw-r--  2.0 unx     3581 b- defN 23-Apr-11 05:34 hyperactive/optimizers/strategies/optimization_strategy.py
 -rw-rw-r--  2.0 unx     1741 b- defN 23-Feb-01 18:21 hyperactive/optimizers/strategies/optimizer_attributes.py
+-rw-rw-r--  2.0 unx       79 b- defN 23-Mar-26 09:16 hyperactive/optimizers/strategies/layers/__init__.py
+-rw-rw-r--  2.0 unx     2328 b- defN 23-Mar-28 17:35 hyperactive/optimizers/strategies/layers/optimizer.py
+-rw-rw-r--  2.0 unx     1945 b- defN 23-Mar-30 10:16 hyperactive/optimizers/strategies/layers/search_space_pruning.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Jan-14 15:47 tests/__init__.py
 -rw-rw-r--  2.0 unx      686 b- defN 21-Dec-08 14:43 tests/_test_examples.py
 -rw-rw-r--  2.0 unx     1995 b- defN 22-May-03 10:56 tests/test_callbacks.py
 -rw-rw-r--  2.0 unx     2566 b- defN 22-May-03 10:56 tests/test_catch.py
 -rw-rw-r--  2.0 unx     4353 b- defN 23-Mar-01 11:28 tests/test_distribution.py
 -rw-rw-r--  2.0 unx     7035 b- defN 21-Dec-08 14:43 tests/test_early_stop.py
 -rw-rw-r--  2.0 unx     5196 b- defN 21-Dec-08 14:43 tests/test_hyper_gradient_trafo.py
@@ -48,23 +51,25 @@
 -rw-rw-r--  2.0 unx     5620 b- defN 23-Feb-01 18:21 tests/_local_test_timings/_test_shared_memory.py
 -rw-rw-r--  2.0 unx      743 b- defN 21-Dec-01 05:57 tests/_local_test_timings/_test_warm_start.py
 -rw-rw-r--  2.0 unx     3945 b- defN 21-Dec-01 05:57 tests/_local_test_timings/_test_warm_start_n_jobs.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-01 05:57 tests/test_issues/__init__.py
 -rw-rw-r--  2.0 unx     1580 b- defN 21-Dec-01 05:57 tests/test_issues/test_issue_25.py
 -rw-rw-r--  2.0 unx      987 b- defN 21-Dec-08 14:43 tests/test_issues/test_issue_29.py
 -rw-rw-r--  2.0 unx     1711 b- defN 21-Dec-01 05:57 tests/test_issues/test_issue_34.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Jan-14 15:47 tests/test_optimization_strategies/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Jan-14 15:47 tests/test_optimization_strategies/test_early_stopping.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Jan-14 15:47 tests/test_optimizers/__init__.py
 -rw-rw-r--  2.0 unx     1336 b- defN 23-Feb-01 18:21 tests/test_optimizers/_parametrize.py
 -rw-rw-r--  2.0 unx     2651 b- defN 21-Dec-08 14:43 tests/test_optimizers/test_best_results.py
--rw-rw-r--  2.0 unx     2615 b- defN 23-Feb-01 18:21 tests/test_optimizers/test_gfo_wrapper.py
+-rw-rw-r--  2.0 unx     2615 b- defN 23-Apr-11 05:34 tests/test_optimizers/test_gfo_wrapper.py
 -rw-rw-r--  2.0 unx      698 b- defN 23-Feb-01 18:21 tests/test_optimizers/test_memory.py
 -rw-rw-r--  2.0 unx     1380 b- defN 23-Mar-01 11:28 tests/test_optimizers/test_optimization_strategies.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-01 05:57 tests/test_warm_starts/__init__.py
 -rw-rw-r--  2.0 unx     2421 b- defN 21-Dec-08 14:43 tests/test_warm_starts/test_memory_warm_start.py
 -rw-rw-r--  2.0 unx     2413 b- defN 21-Dec-01 05:57 tests/test_warm_starts/test_warm_start.py
 -rw-rw-r--  2.0 unx     2896 b- defN 22-Dec-26 17:59 tests/test_warm_starts/test_warm_start_smbo.py
--rw-rw-r--  2.0 unx     1069 b- defN 23-Mar-01 11:36 hyperactive-4.4.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    40490 b- defN 23-Mar-01 11:36 hyperactive-4.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-01 11:36 hyperactive-4.4.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Mar-01 11:36 hyperactive-4.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6388 b- defN 23-Mar-01 11:36 hyperactive-4.4.0.dist-info/RECORD
-68 files, 208378 bytes uncompressed, 47179 bytes compressed:  77.4%
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Apr-11 05:43 hyperactive-4.4.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    40833 b- defN 23-Apr-11 05:43 hyperactive-4.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 05:43 hyperactive-4.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-11 05:43 hyperactive-4.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6937 b- defN 23-Apr-11 05:43 hyperactive-4.4.1.dist-info/RECORD
+73 files, 213622 bytes uncompressed, 48800 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -51,14 +51,23 @@
 
 Filename: hyperactive/optimizers/strategies/optimization_strategy.py
 Comment: 
 
 Filename: hyperactive/optimizers/strategies/optimizer_attributes.py
 Comment: 
 
+Filename: hyperactive/optimizers/strategies/layers/__init__.py
+Comment: 
+
+Filename: hyperactive/optimizers/strategies/layers/optimizer.py
+Comment: 
+
+Filename: hyperactive/optimizers/strategies/layers/search_space_pruning.py
+Comment: 
+
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/_test_examples.py
 Comment: 
 
 Filename: tests/test_callbacks.py
@@ -153,14 +162,20 @@
 
 Filename: tests/test_issues/test_issue_29.py
 Comment: 
 
 Filename: tests/test_issues/test_issue_34.py
 Comment: 
 
+Filename: tests/test_optimization_strategies/__init__.py
+Comment: 
+
+Filename: tests/test_optimization_strategies/test_early_stopping.py
+Comment: 
+
 Filename: tests/test_optimizers/__init__.py
 Comment: 
 
 Filename: tests/test_optimizers/_parametrize.py
 Comment: 
 
 Filename: tests/test_optimizers/test_best_results.py
@@ -183,23 +198,23 @@
 
 Filename: tests/test_warm_starts/test_warm_start.py
 Comment: 
 
 Filename: tests/test_warm_starts/test_warm_start_smbo.py
 Comment: 
 
-Filename: hyperactive-4.4.0.dist-info/LICENSE
+Filename: hyperactive-4.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: hyperactive-4.4.0.dist-info/METADATA
+Filename: hyperactive-4.4.1.dist-info/METADATA
 Comment: 
 
-Filename: hyperactive-4.4.0.dist-info/WHEEL
+Filename: hyperactive-4.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: hyperactive-4.4.0.dist-info/top_level.txt
+Filename: hyperactive-4.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: hyperactive-4.4.0.dist-info/RECORD
+Filename: hyperactive-4.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hyperactive/__init__.py

```diff
@@ -1,12 +1,12 @@
 # Author: Simon Blanke
 # Email: simon.blanke@yahoo.com
 # License: MIT License
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 __license__ = "MIT"
 
 
 from .hyperactive import Hyperactive
 
 
 __all__ = [
```

## Comparing `hyperactive-4.4.0.dist-info/LICENSE` & `hyperactive-4.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hyperactive-4.4.0.dist-info/METADATA` & `hyperactive-4.4.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperactive
-Version: 4.4.0
+Version: 4.4.1
 Summary: A hyperparameter optimization toolbox for convenient and fast prototyping
 Home-page: https://github.com/SimonBlanke/Hyperactive
 Author: Simon Blanke
 Author-email: simon.blanke@yahoo.com
 License: MIT
 Keywords: machine learning,deep learning,optimization,data-science
 Classifier: Programming Language :: Python :: 3
@@ -23,17 +23,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy (>=1.18.1)
-Requires-Dist: tqdm (>=4.48.0)
-Requires-Dist: pandas
+Requires-Dist: numpy (<2.0.0,>=1.18.1)
+Requires-Dist: tqdm (<5.0.0,>=4.48.0)
+Requires-Dist: pandas (<2.0.0)
 Requires-Dist: gradient-free-optimizers (<2.0.0,>=1.2.4)
 Provides-Extra: distribution
 Requires-Dist: pathos ; extra == 'distribution'
 Requires-Dist: joblib ; extra == 'distribution'
 
 <p align="center">
   <a href="https://github.com/SimonBlanke/Hyperactive"><img src="./docs/images/logo.png" height="250"></a>
@@ -79,20 +79,26 @@
 - makes optimization [data collection](./examples/optimization_applications/meta_data_collection.py) simple
 
 - saves your [computation time](./examples/optimization_applications/memory.py)
 
 - supports [parallel computing](./examples/tested_and_supported_packages/multiprocessing_example.py)
 
 
+
+
 <br>
 <br>
 <br>
 
+
 As its name suggests Hyperactive started as a hyperparameter optimization package, but it has been generalized to solve expensive gradient-free optimization problems. It uses the [Gradient-Free-Optimizers](https://github.com/SimonBlanke/Gradient-Free-Optimizers) package as an optimization-backend and expands on it with additional features and tools.
 
+
+<br>
+
 ---
 
 <div align="center"><a name="menu"></a>
   <h3>
     <a href="https://github.com/SimonBlanke/Hyperactive#overview">Overview</a> •
     <a href="https://github.com/SimonBlanke/Hyperactive#installation">Installation</a> •
     <a href="https://github.com/SimonBlanke/Hyperactive#hyperactive-api-reference">API reference</a> •
@@ -103,14 +109,15 @@
 </div>
 
 ---
 
 <br>
 
 ## What's new?
+  - ### 01.03.2023 v4.4.0 add new feature: "Optimization Strategies"
   - ### 18.11.2022 v4.3.0 with three new optimization algorithms (Spiral Optimization, Lipschitz Optimizer, DIRECT Optimizer)
   - ### 04.05.2022 v4.2.0 with support of handling Exceptions and Callbacks
 
 <br>
 
 ## Overview
 
@@ -234,80 +241,34 @@
     </tr>
   </tbody>
 </table>
 
 The examples above are not necessarily done with realistic datasets or training procedures. 
 The purpose is fast execution of the solution proposal and giving the user ideas for interesting usecases.
 
-<br>
-
-
-### Hyperactive is very easy to use:
-
-<table>
-<tbody>
-<tr>
-<th> Regular training </th>
-<th> Hyperactive </th>
-</tr>
-<tr>
-<td>
-
-```python
-from sklearn.model_selection import cross_val_score
-from sklearn.tree import DecisionTreeRegressor
-from sklearn.datasets import fetch_california_housing
-
-
-data = fetch_california_housing()
-X, y = data.data, data.target
-
-
-gbr = DecisionTreeRegressor(max_depth=10)
-score = cross_val_score(gbr, X, y, cv=3).mean()
-
-
 
+<br>
 
+## Sideprojects and Tools
 
+The following packages are designed to support Hyperactive and expand its use cases. 
 
+| Package                                                                       | Description                                                                          |
+|-------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
+| [Search-Data-Collector](https://github.com/SimonBlanke/search-data-collector) | Simple tool to save search-data during or after the optimization run into csv-files. |
+| [Search-Data-Explorer](https://github.com/SimonBlanke/search-data-explorer)   | Visualize search-data with plotly inside a streamlit dashboard.
 
+If you want news about Hyperactive and related projects you can follow me on [twitter](https://twitter.com/blanke_simon).
 
 
-```
-
-</td>
-<td>
-
-```python
-from sklearn.model_selection import cross_val_score
-from sklearn.tree import DecisionTreeRegressor
-from sklearn.datasets import fetch_california_housing
-from hyperactive import Hyperactive
-
-data = fetch_california_housing()
-X, y = data.data, data.target
-
-def model(opt):
-    gbr = DecisionTreeRegressor(max_depth=opt["max_depth"])
-    return cross_val_score(gbr, X, y, cv=3).mean()
-
-
-search_space = {"max_depth": list(range(3, 25))}
-
-hyper = Hyperactive()
-hyper.add_search(model, search_space, n_iter=50)
-hyper.run()
-```
+<br>
 
-</td>
-</tr>
-</tbody>
-</table>
+## Notebooks and Tutorials
 
+- [Introduction to Hyperactive](https://nbviewer.org/github/SimonBlanke/hyperactive-tutorial/blob/main/notebooks/hyperactive_tutorial.ipynb)
 
 
 <br>
 
 ## Installation
 
 The most recent version of Hyperactive is available on PyPi:
@@ -316,14 +277,16 @@
 [![PyPI version](https://img.shields.io/pypi/v/hyperactive?style=for-the-badge&logo=pypi&color=green&logoColor=white)](https://pypi.org/project/hyperactive/)
 [![PyPI version](https://img.shields.io/pypi/dm/hyperactive?style=for-the-badge&color=red)](https://pypi.org/project/hyperactive/)
 
 ```console
 pip install hyperactive
 ```
 
+
+
 <br>
 
 ## Example
 
 ```python
 from sklearn.model_selection import cross_val_score
 from sklearn.ensemble import GradientBoostingRegressor
@@ -884,18 +847,20 @@
       </tbody>
     </table>
 
 </details>
 
 
 
+
 <br>
 
 ## Roadmap
 
+
 <details>
 <summary><b>v2.0.0</b> :heavy_check_mark:</summary>
 
   - [x] Change API
 </details>
 
 <details>
@@ -999,29 +964,42 @@
     - [x] add Lipschitz Optimizer
     - [x] add DIRECT Optimizer
     - [x] print the random seed for reproducibility
 
 </details>
 
 <details>
-<summary><b>v4.4.0</b> </summary>
+<summary><b>v4.4.0</b> :heavy_check_mark: </summary>
 
   - [ ] add Optimization-Strategies
   - [ ] redesign progress-bar
 
 </details>
 
+<details>
+<summary><b>v4.5.0</b> </summary>
+
+  - [ ] add early stopping feature to custom optimization strategies
+  - [ ] add "prune_search_space"-method to custom optimization strategy class
+  - [ ] display additional outputs from objective-function in results in command-line
+  - [ ] add type hints to hyperactive-api
+  
+</details>
+
+
+
+
+
+
 
 
 <details>
 <summary><b>Ideas for the Future</b></summary>
    
-  - [ ] Data collector tool to store data (from inside the objective function) into csv-files
   - [ ] Experiment-tracking for search-data storage and usage
-  - [ ] Dashboard for visualization of stored search-data
   - [ ] Meta-Learning tool for hyperparameter optimization
 
 </details>
 
 
 
 <br>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hyperactive Version: 4.4.0 Summary: A
+Metadata-Version: 2.1 Name: hyperactive Version: 4.4.1 Summary: A
 hyperparameter optimization toolbox for convenient and fast prototyping Home-
 page: https://github.com/SimonBlanke/Hyperactive Author: Simon Blanke Author-
 email: simon.blanke@yahoo.com License: MIT Keywords: machine learning,deep
 learning,optimization,data-science Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -12,18 +12,18 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis Classifier:
 Topic :: Scientific/Engineering :: Mathematics Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Requires-Python: >=3.5 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: numpy
-(>=1.18.1) Requires-Dist: tqdm (>=4.48.0) Requires-Dist: pandas Requires-Dist:
-gradient-free-optimizers (<2.0.0,>=1.2.4) Provides-Extra: distribution
-Requires-Dist: pathos ; extra == 'distribution' Requires-Dist: joblib ; extra
-== 'distribution'
+(<2.0.0,>=1.18.1) Requires-Dist: tqdm (<5.0.0,>=4.48.0) Requires-Dist: pandas
+(<2.0.0) Requires-Dist: gradient-free-optimizers (<2.0.0,>=1.2.4) Provides-
+Extra: distribution Requires-Dist: pathos ; extra == 'distribution' Requires-
+Dist: joblib ; extra == 'distribution'
                            [./docs/images/logo.png]
 
 ---
 [img_not_loaded:_try_F5_:)] [img_not_loaded:_try_F5_:)] [img_not_loaded:_try_F5
  :)] [img_not_loaded:_try_F5_:)] [img_not_loaded:_try_F5_:)] [img_not_loaded:
                                   try_F5_:)]
    ***** An optimization and data collection toolbox for convenient and fast
@@ -40,19 +40,21 @@
 examples/tested_and_supported_packages/multiprocessing_example.py)
 
 
 As its name suggests Hyperactive started as a hyperparameter optimization
 package, but it has been generalized to solve expensive gradient-free
 optimization problems. It uses the [Gradient-Free-Optimizers](https://
 github.com/SimonBlanke/Gradient-Free-Optimizers) package as an optimization-
-backend and expands on it with additional features and tools. ---
+backend and expands on it with additional features and tools.
+---
  **** Overview â¢ Installation â¢ API_reference â¢ Roadmap â¢ Citation â¢
                                  License ****
 ---
-## What's new? - ### 18.11.2022 v4.3.0 with three new optimization algorithms
+## What's new? - ### 01.03.2023 v4.4.0 add new feature: "Optimization
+Strategies" - ### 18.11.2022 v4.3.0 with three new optimization algorithms
 (Spiral Optimization, Lipschitz Optimizer, DIRECT Optimizer) - ### 04.05.2022
 v4.2.0 with support of handling Exceptions and Callbacks
 ## Overview
  **** Hyperactive features a collection of optimization algorithms that can be
 used for a variety of optimization problems. The following table shows examples
                            of its capabilities: ****
 
@@ -93,32 +95,27 @@
     * Tree_of_Parzen
       Estimators
     * Forest_Optimizer
       [dto]
 The examples above are not necessarily done with realistic datasets or training
 procedures. The purpose is fast execution of the solution proposal and giving
 the user ideas for interesting usecases.
-### Hyperactive is very easy to use:
-Regular training                       Hyperactive
-                                       ```python from sklearn.model_selection
-                                       import cross_val_score from sklearn.tree
-```python from sklearn.model_selection import DecisionTreeRegressor from
-import cross_val_score from            sklearn.datasets import
-sklearn.tree import                    fetch_california_housing from
-DecisionTreeRegressor from             hyperactive import Hyperactive data =
-sklearn.datasets import                fetch_california_housing() X, y =
-fetch_california_housing data =        data.data, data.target def model(opt):
-fetch_california_housing() X, y =      gbr = DecisionTreeRegressor
-data.data, data.target gbr =           (max_depth=opt["max_depth"]) return
-DecisionTreeRegressor(max_depth=10)    cross_val_score(gbr, X, y, cv=3).mean()
-score = cross_val_score(gbr, X, y,     search_space = {"max_depth": list(range
-cv=3).mean() ```                       (3, 25))} hyper = Hyperactive()
-                                       hyper.add_search(model, search_space,
-                                       n_iter=50) hyper.run() ```
-
+## Sideprojects and Tools The following packages are designed to support
+Hyperactive and expand its use cases. | Package | Description | |--------------
+-----------------------------------------------------------------|-------------
+-------------------------------------------------------------------------| |
+[Search-Data-Collector](https://github.com/SimonBlanke/search-data-collector) |
+Simple tool to save search-data during or after the optimization run into csv-
+files. | | [Search-Data-Explorer](https://github.com/SimonBlanke/search-data-
+explorer) | Visualize search-data with plotly inside a streamlit dashboard. If
+you want news about Hyperactive and related projects you can follow me on
+[twitter](https://twitter.com/blanke_simon).
+## Notebooks and Tutorials - [Introduction to Hyperactive](https://
+nbviewer.org/github/SimonBlanke/hyperactive-tutorial/blob/main/notebooks/
+hyperactive_tutorial.ipynb)
 ## Installation The most recent version of Hyperactive is available on PyPi: [!
 [pyversions](https://img.shields.io/pypi/pyversions/hyperactive.svg?style=for-
 the-badge&logo=python&color=blue&logoColor=white)](https://pypi.org/project/
 hyperactive) [![PyPI version](https://img.shields.io/pypi/v/
 hyperactive?style=for-the-badge&logo=pypi&color=green&logoColor=white)](https:/
 /pypi.org/project/hyperactive/) [![PyPI version](https://img.shields.io/pypi/
 dm/hyperactive?style=for-the-badge&color=red)](https://pypi.org/project/
@@ -366,20 +363,22 @@
 learn, ...) from separate repositories - [x] separate progress board into
 separate repository   v4.1.0 :heavy_check_mark: - [x] add python 3.9 to testing
 - [x] add pass_through-parameter - [x] add v1 GFO optimization algorithms
 v4.2.0 :heavy_check_mark: - [x] add callbacks-parameter - [x] add catch-
 parameter - [x] add option to add eval- and iter- times to search-data   v4.3.0
 :heavy_check_mark: - [x] add new features from GFO - [x] add Spiral
 Optimization - [x] add Lipschitz Optimizer - [x] add DIRECT Optimizer - [x]
-print the random seed for reproducibility   v4.4.0  - [ ] add Optimization-
-Strategies - [ ] redesign progress-bar   Ideas for the Future - [ ] Data
-collector tool to store data (from inside the objective function) into csv-
-files - [ ] Experiment-tracking for search-data storage and usage - [ ]
-Dashboard for visualization of stored search-data - [ ] Meta-Learning tool for
-hyperparameter optimization
+print the random seed for reproducibility   v4.4.0 :heavy_check_mark:  - [ ]
+add Optimization-Strategies - [ ] redesign progress-bar   v4.5.0  - [ ] add
+early stopping feature to custom optimization strategies - [ ] add
+"prune_search_space"-method to custom optimization strategy class - [ ] display
+additional outputs from objective-function in results in command-line - [ ] add
+type hints to hyperactive-api   Ideas for the Future - [ ] Experiment-tracking
+for search-data storage and usage - [ ] Meta-Learning tool for hyperparameter
+optimization
 ## Experimental algorithms The following algorithms are of my own design and,
 to my knowledge, do not yet exist in the technical literature. If any of these
 algorithms already exist I would like you to share it with me in an issue. ####
 Random Annealing A combination between simulated annealing and random search.
 ## FAQ #### Known Errors + Solutions  Read this before opening a bug-issue
 - Are you sure the bug is located in Hyperactive? The error might be located in
 the optimization-backend. Look at the error message from the command line. If
```

## Comparing `hyperactive-4.4.0.dist-info/RECORD` & `hyperactive-4.4.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-hyperactive/__init__.py,sha256=PpMe9E9qAUO5pd3PoI13uOsQG6rV60bZC7dNaMQu59Y,195
+hyperactive/__init__.py,sha256=g32vrxGIv8yeRjhs3QWrrOEbxXC_0IUJalMaTOQF0sU,195
 hyperactive/distribution.py,sha256=pmiJcJ3MgzduAaPJq7ze3Jw2_Od1CHUUSY_24vhUqZY,1057
 hyperactive/hyperactive.py,sha256=JTSlzsLQWmNXpiIoB0bo4JV1fdE6ZST6pJhxg1XpAPg,4980
 hyperactive/print_results.py,sha256=bMHB9s3PIezDdeZbeLTDpwAn8oOTXKHOTXa7hvio23o,3749
 hyperactive/process.py,sha256=-eWKSKUJpPElc85r5gdHQ28MIMnfxLBw3QJvuFVHRok,754
 hyperactive/results.py,sha256=Se2CQCVKUJ07UVdCu92vtUHmroDUclm4T2m8SEpDPhg,2505
 hyperactive/run_search.py,sha256=sECQFoX0tO3hby8u-febVrjo-Owuk2el_3klRusBFcQ,1416
 hyperactive/search_space.py,sha256=9j1acKdOy_TiIqa_BTlY9K4c9sdUOqVq8blC1ygBJCU,3981
@@ -13,14 +13,17 @@
 hyperactive/optimizers/objective_function.py,sha256=FWINdUMC4WFhKKV_xPN0N1EEcBlLktDVBRJrVk1y8Vo,1456
 hyperactive/optimizers/optimizer_attributes.py,sha256=YQiAsXk2Ag3ez9Fe0HZ1bq858Q21ADBRbnYpts8Bwg0,825
 hyperactive/optimizers/optimizers.py,sha256=SrSeTPi2t9AZMOfLx43J9s5a0Fb9dQvxJqfaHI9vZYE,5103
 hyperactive/optimizers/strategies/__init__.py,sha256=-XSIY9W45p81E6wLB98DkqZcUwZYK7aPFtFSK35-6Kw,199
 hyperactive/optimizers/strategies/custom_optimization_strategy.py,sha256=RCE-YM3OyNg37UFTnXLsKXdUyuZGXNMLtXnSMxczcgE,573
 hyperactive/optimizers/strategies/optimization_strategy.py,sha256=QSV2huEew7cEbXEj8jMLP5REXbFcPQ29ZoDNJlO2qCY,3581
 hyperactive/optimizers/strategies/optimizer_attributes.py,sha256=4JQyZapCAKs6ruvEfknd0oh2v7WBgFmWf1FGREG3viY,1741
+hyperactive/optimizers/strategies/layers/__init__.py,sha256=5Ceb7BOEy-kdg2D98p_WeIJelkxT3CeboTA9ZqT-MPs,79
+hyperactive/optimizers/strategies/layers/optimizer.py,sha256=IHFu7opbSJ_XhBUjbG7F-uwK0ja7-Bnj13GOw6B03Xs,2328
+hyperactive/optimizers/strategies/layers/search_space_pruning.py,sha256=Z3XMRvWfD_2vtQ3aTyjdJ0l-rsT3hS7kI7DE5JuQKZk,1945
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/_test_examples.py,sha256=7QRuve6FWx7oiw39NU2Lzx1eAA3cN_Hn2POBDYpl2ig,686
 tests/test_callbacks.py,sha256=U_djPJTHztY-XtLEhmPtjOG-DDZEDs0vFYSywTLmdtM,1995
 tests/test_catch.py,sha256=Bsd_9tvSPzZU0TxVjhpVYY96_QhiDWjXQVZsbsLd5A4,2566
 tests/test_distribution.py,sha256=N0OXWPeMhz9C6yqEu6gDeWOtD_wTOqg5Mghqr8Vu8yM,4353
 tests/test_early_stop.py,sha256=apwDIOAFaczChs7M3c4YFlirX1oe1NbRjak1eTVTrbA,7035
 tests/test_hyper_gradient_trafo.py,sha256=U-So-BFqAkqEbEEljPgwduopZ-0y9Eye2p1CtVxnFJo,5196
@@ -47,22 +50,24 @@
 tests/_local_test_timings/_test_shared_memory.py,sha256=anbDOHBaBVeuO_pedFrF9PCc_K1NpGxvynG_WTGR0Tk,5620
 tests/_local_test_timings/_test_warm_start.py,sha256=YKmYVDjv8uH0RW156yDd7di2BYSdmawYtUK8sLrRI18,743
 tests/_local_test_timings/_test_warm_start_n_jobs.py,sha256=8buGbyc4AOjCoLdntjV0bJZQFXR3qjPySA2FSwWzB2c,3945
 tests/test_issues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_issues/test_issue_25.py,sha256=TTOxFjqUWodHm9Fw3W72lwFGRLQjL4pIYtD2oPqa8z0,1580
 tests/test_issues/test_issue_29.py,sha256=Z5haa34Ja0y9iBkaOz6PYAqptWPu4ic8J-z0fbvWfUQ,987
 tests/test_issues/test_issue_34.py,sha256=7joD-gCmB77-xmDG2KFSiKc_aBAHCPdvi68QMcug4lU,1711
+tests/test_optimization_strategies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/test_optimization_strategies/test_early_stopping.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_optimizers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_optimizers/_parametrize.py,sha256=_qYSVlOq_gSfx6e5U65e-UiqPZ5BKrBXW786yWkusS0,1336
 tests/test_optimizers/test_best_results.py,sha256=F8qSOY5VJp6KlntO9Qq36yib3Mfkky-_M6QBOXnbP3U,2651
 tests/test_optimizers/test_gfo_wrapper.py,sha256=fjxOTB6-mMJq6Bh2S5P1ZnnF6YW3QeaxZEs7XCPPPrU,2615
 tests/test_optimizers/test_memory.py,sha256=hjxotqtn29li7y__J1GbheEw01IYjhvq86YN-97y1jc,698
 tests/test_optimizers/test_optimization_strategies.py,sha256=qTVFU-5EdfxEYNMW7Rnsy611P82S4fVucQ54M-qaoHI,1380
 tests/test_warm_starts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_warm_starts/test_memory_warm_start.py,sha256=CJLAKHAYFPUtuEQjHw8JtIpuxOvuYOuZQ596Z0ZUuT4,2421
 tests/test_warm_starts/test_warm_start.py,sha256=U7Digok8gyvKs0tuYIqCmkl2cLS3UA1sVm8a1SSH2ec,2413
 tests/test_warm_starts/test_warm_start_smbo.py,sha256=0ic7V-11QOVEplno_jQVdhmiw1DQGSU7rBLs-s5bOk0,2896
-hyperactive-4.4.0.dist-info/LICENSE,sha256=DA9r_H29OB7cmPO-wKWJ44gP2Zok54f08pBMqivlbwE,1069
-hyperactive-4.4.0.dist-info/METADATA,sha256=Q4ns-fiVe1kFk6F5aeEDyZ7fFkozIafHnwX0A4h-koY,40490
-hyperactive-4.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-hyperactive-4.4.0.dist-info/top_level.txt,sha256=eKxBf3Mh-LzqGdk_eza4VBHt6My6tMtEljMI9hupE-8,18
-hyperactive-4.4.0.dist-info/RECORD,,
+hyperactive-4.4.1.dist-info/LICENSE,sha256=DA9r_H29OB7cmPO-wKWJ44gP2Zok54f08pBMqivlbwE,1069
+hyperactive-4.4.1.dist-info/METADATA,sha256=IxktZp-QKru7NF3vKcH3tJzy8T50-6iwGY8MgMuMZy4,40833
+hyperactive-4.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+hyperactive-4.4.1.dist-info/top_level.txt,sha256=eKxBf3Mh-LzqGdk_eza4VBHt6My6tMtEljMI9hupE-8,18
+hyperactive-4.4.1.dist-info/RECORD,,
```

