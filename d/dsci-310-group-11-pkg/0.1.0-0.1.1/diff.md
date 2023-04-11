# Comparing `tmp/dsci_310_group_11_pkg-0.1.0.tar.gz` & `tmp/dsci_310_group_11_pkg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsci_310_group_11_pkg-0.1.0.tar", max compression
+gzip compressed data, was "dsci_310_group_11_pkg-0.1.1.tar", max compression
```

## Comparing `dsci_310_group_11_pkg-0.1.0.tar` & `dsci_310_group_11_pkg-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1072 2023-04-10 23:48:36.419342 dsci_310_group_11_pkg-0.1.0/LICENSE
--rw-r--r--   0        0        0     3211 2023-04-11 00:30:57.536160 dsci_310_group_11_pkg-0.1.0/README.md
--rw-r--r--   0        0        0      683 2023-04-10 23:48:36.424990 dsci_310_group_11_pkg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      123 2023-04-10 23:48:36.425332 dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/__init__.py
--rw-r--r--   0        0        0     6935 2023-04-10 23:48:36.425531 dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/grapher.py
--rw-r--r--   0        0        0     3883 2023-04-10 23:48:36.425680 dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/optimize.py
--rw-r--r--   0        0        0     1963 2023-04-10 23:48:36.425876 dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/pipeline.py
--rw-r--r--   0        0        0     1266 2023-04-10 23:48:36.426032 dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/preprocess.py
--rw-r--r--   0        0        0     3988 1970-01-01 00:00:00.000000 dsci_310_group_11_pkg-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-04-10 23:48:36.419342 dsci_310_group_11_pkg-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3295 2023-04-11 02:04:50.841236 dsci_310_group_11_pkg-0.1.1/README.md
+-rw-r--r--   0        0        0      683 2023-04-11 02:06:19.692602 dsci_310_group_11_pkg-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-04-10 23:48:36.425332 dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/__init__.py
+-rw-r--r--   0        0        0     6824 2023-04-11 02:04:50.844426 dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/grapher.py
+-rw-r--r--   0        0        0     3883 2023-04-10 23:48:36.425680 dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/optimize.py
+-rw-r--r--   0        0        0     1963 2023-04-10 23:48:36.425876 dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/pipeline.py
+-rw-r--r--   0        0        0     1266 2023-04-10 23:48:36.426032 dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/preprocess.py
+-rw-r--r--   0        0        0     4072 1970-01-01 00:00:00.000000 dsci_310_group_11_pkg-0.1.1/PKG-INFO
```

### Comparing `dsci_310_group_11_pkg-0.1.0/LICENSE` & `dsci_310_group_11_pkg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsci_310_group_11_pkg-0.1.0/README.md` & `dsci_310_group_11_pkg-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 ```
 
 2. Navigate to the local repository through the terminal (this may differ based on your home directory setups):
 ```
 cd dsci-310-group-11-pkg
 ```
 
-3. Run pip to install the package locally:
+3. Run pip to install the package locally (from [pypi](https://pypi.org/project/dsci-310-group-11-pkg/)):
 ```
-pip install .
+pip install dsci-310-group-11-pkg
 ```
 
 You should now be able to import the package into relevant projects and notebooks.
 
 ## Usage
 
 The most basic usage of this package is to split the data into training or testing data:
@@ -51,31 +51,31 @@
 
 model = pipe_build(model_type, x, y)
 
 ```
 Another usage is to conduct hyperparameter tuning and return it as dataframe for different model as follows:
 
 ```python
-from dsci_310_group_11_pkg.optimizer import optimize
+from dsci_310_group_11_pkg.optimize import hy_optimizer
 
 x = X_training_data # training features data
 y = Y_training data # training label data
 model_name = 'lr' # types of model
 
-tuning_result = optimize(model_name, x, y)
+tuning_result = hp_optimize(model_name, x, y)
 ```
 
 This package can also be used to generate different graphs for the analysis report, for example: 
 
 ```python
 from dsci_310_group_11_pkg.grapher import correlation_table
 
 ctb = correlation_table(df) # this generate the correlation table for dataframe df
 ```
-Other functions and more detailed usage can be found in docs/example or in the [website documentation of group 11 package](https://dsci-310-group11-pkg.readthedocs.io/en/latest/index.html) 
+Other functions and more detailed usage can be found in docs/example or in the [website documentation of the package](https://dsci-310-group11-pkg.readthedocs.io/en/latest/index.html).
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
```

### Comparing `dsci_310_group_11_pkg-0.1.0/pyproject.toml` & `dsci_310_group_11_pkg-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dsci_310_group_11_pkg"
-version = "0.1.0"
+version = "0.1.1"
 description = "package for dsci310 report"
 authors = ["Anthony Huang"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/grapher.py` & `dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/grapher.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     table = alt.Chart(cor_data).mark_rect().encode(
         alt.X('Variable 1:O'),
         alt.Y('Variable 2:O'),
         alt.Color('correlation'),
         alt.Tooltip(['correlation_label']),
     ).interactive().properties(width=300, height=300)
 
-    xy = table.to_json('corrtab.json')
-    return xy
+   
+    return table
 
 def bar_chart(df):
     """DESCRIPTION: Displays a simple bar chart of the count of the quality variable.
     
     ACTION: Inputs a dataframe and displays the bar chart.
     
     INPUTS: df - A dataframe object
@@ -51,16 +51,16 @@
     
     TODO: 1. Modularize the variables that you can input into the chart
     2. Move from altair to matplotlib
     """
     x = alt.Chart(df).mark_bar().encode(alt.X('quality:O'),
                                         alt.Y('count()')).properties(width=200,
                                                                      height=100)
-    xyy = x.to_json('bar.json')
-    return xyy
+    
+    return x
 
 def class_report(pipe, X_test, y_test):
     """DESCRIPTION: Displays a heatmap of the count of the predicted case.
     
     ACTION: Inputs a model, testing data and displays the heatmap.
     
     INPUTS: pipe - a model
@@ -68,16 +68,16 @@
             y_test - testing label data
     
     RETURNS: The heatmap as figure
     
     """
     clf_report = classification_report(y_test, pipe.predict(X_test), output_dict=True)
     report = sns.heatmap(pd.DataFrame(clf_report).iloc[:-1, :].T, annot=True, linewidth=.5, cmap="crest")
-    fig = report.get_figure()
-    return fig
+    
+    return report
 
 def vis_tree(X_train, y_train):
     """DESCRIPTION: Displays a visual example of a decision tree for conceptual
     purposes. The max_depth variable is limited to 3 so that the visualization
     is interpretable.
     
     INPUTS: X_train - a dataframe object containing prediction features
@@ -125,15 +125,15 @@
         alt.datum.Score == max(
             report['Score']),  # If the year is 1810 this test returns True,
         alt.value('red'),  # which sets the bar orange.
         alt.value(
             'steelblue')  # And if it's not true it sets the bar steelblue.
     )).properties(width=500, height=200).configure(background='lightgrey')
 
-    y = y.to_json('scores.json')
+    
     return y
 
 def show_coefficients(pipe, X_train):
     """DESCRIPTION: Displays a dataframe with the coefficients of the Logistic
     Regression model.
     
     INPUTS: pipe - a pipeline object containing scikit-learn model transformers, and a scikit-learn model.
```

### Comparing `dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/optimize.py` & `dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/optimize.py`

 * *Files identical despite different names*

### Comparing `dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/pipeline.py` & `dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/pipeline.py`

 * *Files identical despite different names*

### Comparing `dsci_310_group_11_pkg-0.1.0/src/dsci_310_group_11_pkg/preprocess.py` & `dsci_310_group_11_pkg-0.1.1/src/dsci_310_group_11_pkg/preprocess.py`

 * *Files identical despite different names*

### Comparing `dsci_310_group_11_pkg-0.1.0/PKG-INFO` & `dsci_310_group_11_pkg-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsci-310-group-11-pkg
-Version: 0.1.0
+Version: 0.1.1
 Summary: package for dsci310 report
 License: MIT
 Author: Anthony Huang
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -39,17 +39,17 @@
 ```
 
 2. Navigate to the local repository through the terminal (this may differ based on your home directory setups):
 ```
 cd dsci-310-group-11-pkg
 ```
 
-3. Run pip to install the package locally:
+3. Run pip to install the package locally (from [pypi](https://pypi.org/project/dsci-310-group-11-pkg/)):
 ```
-pip install .
+pip install dsci-310-group-11-pkg
 ```
 
 You should now be able to import the package into relevant projects and notebooks.
 
 ## Usage
 
 The most basic usage of this package is to split the data into training or testing data:
@@ -73,31 +73,31 @@
 
 model = pipe_build(model_type, x, y)
 
 ```
 Another usage is to conduct hyperparameter tuning and return it as dataframe for different model as follows:
 
 ```python
-from dsci_310_group_11_pkg.optimizer import optimize
+from dsci_310_group_11_pkg.optimize import hy_optimizer
 
 x = X_training_data # training features data
 y = Y_training data # training label data
 model_name = 'lr' # types of model
 
-tuning_result = optimize(model_name, x, y)
+tuning_result = hp_optimize(model_name, x, y)
 ```
 
 This package can also be used to generate different graphs for the analysis report, for example: 
 
 ```python
 from dsci_310_group_11_pkg.grapher import correlation_table
 
 ctb = correlation_table(df) # this generate the correlation table for dataframe df
 ```
-Other functions and more detailed usage can be found in docs/example or in the [website documentation of group 11 package](https://dsci-310-group11-pkg.readthedocs.io/en/latest/index.html) 
+Other functions and more detailed usage can be found in docs/example or in the [website documentation of the package](https://dsci-310-group11-pkg.readthedocs.io/en/latest/index.html).
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
 ## License
```

