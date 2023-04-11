# Comparing `tmp/gmltools-0.0.40.tar.gz` & `tmp/gmltools-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.40.tar", last modified: Tue Apr  4 08:49:39 2023, max compression
+gzip compressed data, was "gmltools-0.0.41.tar", last modified: Tue Apr 11 09:53:19 2023, max compression
```

## Comparing `gmltools-0.0.40.tar` & `gmltools-0.0.41.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:39.310858 gmltools-0.0.40/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.40/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.40/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-04 08:49:39.309862 gmltools-0.0.40/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.40/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:38.964894 gmltools-0.0.40/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.40/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.40/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.40/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.40/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.40/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.40/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-04 08:49:05.000000 gmltools-0.0.40/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 08:49:39.310858 gmltools-0.0.40/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-04 08:48:55.000000 gmltools-0.0.40/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:38.792819 gmltools-0.0.40/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:38.999991 gmltools-0.0.40/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.40/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.40/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:39.092928 gmltools-0.0.40/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.40/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.40/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:39.208744 gmltools-0.0.40/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.40/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.40/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.40/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0    83848 2023-04-04 08:42:06.000000 gmltools-0.0.40/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.40/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.40/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:39.249894 gmltools-0.0.40/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.40/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    72039 2023-03-30 11:31:35.000000 gmltools-0.0.40/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.40/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:39.306695 gmltools-0.0.40/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.40/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.40/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.40/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.40/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:49:39.063616 gmltools-0.0.40/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-04 08:49:37.000000 gmltools-0.0.40/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-04 08:49:38.000000 gmltools-0.0.40/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 08:49:37.000000 gmltools-0.0.40/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-04 08:49:37.000000 gmltools-0.0.40/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-04 08:49:37.000000 gmltools-0.0.40/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.528497 gmltools-0.0.41/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.41/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.41/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-11 09:53:19.528497 gmltools-0.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.41/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.507324 gmltools-0.0.41/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.41/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.41/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.41/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.41/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.41/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.41/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-11 09:52:11.000000 gmltools-0.0.41/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:53:19.528497 gmltools-0.0.41/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-11 09:51:56.000000 gmltools-0.0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.495361 gmltools-0.0.41/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.509317 gmltools-0.0.41/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.41/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.41/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.517330 gmltools-0.0.41/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.41/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.41/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.521601 gmltools-0.0.41/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.41/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.41/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.41/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0    88338 2023-04-11 09:50:45.000000 gmltools-0.0.41/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.41/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0     3846 2023-03-19 22:48:47.000000 gmltools-0.0.41/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.525077 gmltools-0.0.41/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.41/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73495 2023-04-11 09:50:48.000000 gmltools-0.0.41/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.41/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.527460 gmltools-0.0.41/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.41/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.41/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.41/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.41/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:53:19.514805 gmltools-0.0.41/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 09:53:19.000000 gmltools-0.0.41/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.40/LICENSE` & `gmltools-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/Models.ipynb` & `gmltools-0.0.41/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/PKG-INFO` & `gmltools-0.0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.40
+Version: 0.0.41
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.40/README.md` & `gmltools-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.41/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.41/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.41/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.41/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/gmltools.yml` & `gmltools-0.0.41/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/mltools.yml` & `gmltools-0.0.41/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/pyproject.toml` & `gmltools-0.0.41/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.40"
+version = "0.0.41"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.40/setup.py` & `gmltools-0.0.41/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.40',
+    'version': '0.0.41',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.40/src/gmltools/To_Do.txt` & `gmltools-0.0.41/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/eda/eda.py` & `gmltools-0.0.41/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/models/bayes.py` & `gmltools-0.0.41/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.41/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/models/model.py` & `gmltools-0.0.41/src/gmltools/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,33 @@
 from sklearn.preprocessing import StandardScaler
 from sklearn.preprocessing import OrdinalEncoder
 #OPTIMIZERS
 from sklearn.model_selection import GridSearchCV
 from .bayes import ModelOptimizer
 from sklearn.model_selection import RandomizedSearchCV
 #INFO
-from .models_info import *
+from .models_info import (
+    rf_default_params_clf,
+    rf_default_params_reg,
+    xgb_default_params_clf,
+    xgb_default_params_reg,
+    lr_default_params_clf,
+    lr_default_params_reg,
+    mlp_default_params_clf,
+    mlp_default_params_reg,
+    knn_default_params_clf,
+    knn_default_params_reg,
+    dt_default_params_clf,
+    dt_default_params_reg
+)
 #import compute_sample_weight
 from sklearn.utils.class_weight import compute_sample_weight
+import joblib
+import os
+from openpyxl import load_workbook
 
 
 
 #---------------------------------------------------------------------------
 
 def automatic_preprocessor(X_train,ordinal_cat_cols):
     #Arguments assertion not needed because they are already checked in the model method of the classes that are the ones that call this function
@@ -189,16 +205,17 @@
     RandomForest_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     XGBoost_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     LogisticRegression_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     DecisionTree_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     KNN_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     MLP_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
 
-    def __init__(self):
-        pass
+    def __init__(self, model_name):
+        self.model = None
+        self.model_name = model_name
 
     def RandomForest_Classifier(self, X_train, y_train, ordinal_cat_cols=None,
                                 scoring='accuracy', class_weight=None,
                                 grid_params={'RFC__n_estimators': [100, 200],
                                             'RFC__max_depth': [None, 10, 20],
                                             'RFC__min_samples_split': [2, 5],
                                             'RFC__max_features': ['sqrt', None]},
@@ -285,17 +302,18 @@
             ('RF', RandomForestClassifier(
                 criterion = criterion,
                 bootstrap = True,
                 n_jobs = n_jobs,
                 random_state = random_state,
                 class_weight = class_weight))])
 
-        model_=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        
 
-        return model_
+        return self.model
     
     def XGBoost_Classifier( self, X_train, y_train, ordinal_cat_cols=None,
                             scoring='accuracy', eval_metric='merror',
                             objective='multi:softmax', grid_params={},
                             cv=10, random_params=None, random_n_iter=10,
                             bayes_pbounds=None,bayes_int_params=None, 
                             bayes_n_iter=30, random_state=None,
@@ -377,16 +395,16 @@
             ('XGB', XGBClassifier(
                                 random_state=random_state,
                                 n_jobs=n_jobs, 
                                 verbosity=0,
                                 eval_metric=eval_metric,
                                 objective=objective))])
                                 
-        model_=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
-        return model_
+        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        return self.model
     
     def LogisticRegression_Classifier(self, X_train, y_train,  
                                       ordinal_cat_cols=None, scoring='accuracy',
                                     grid_params = {'LR__C': [0.1, 1, 10],
                                     'LR__penalty': ['l1', 'l2', 'elasticnet'],
                                     'LR__multi_class': ['ovr', 'multinomial'],   
                                     'LR__solver': ['newton-cg', 'lbfgs', 'liblinear', 'sag', 'saga']},
@@ -487,17 +505,17 @@
                                     n_jobs=n_jobs, 
                                     verbose=0,
                                     warm_start=False,
                                     fit_intercept=True,
                                     intercept_scaling=1,
                                     dual=False))])
 
-        model_=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,cv=cv,random_n_iter=random_n_iter,sample_weight=sample_weight)
+        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,cv=cv,random_n_iter=random_n_iter,sample_weight=sample_weight)
         
-        return model_
+        return self.model
     
     def MLP_Classifier(self,X_train,y_train,ordinal_cat_cols=None, scoring='accuracy',
                        grid_params={'MLP__alpha': [1e-9,1e-7,1e-5,0.001,0.01],
                         'MLP__hidden_layer_sizes':[(5,),(10,),(15,),(20,),(25,)]},
                         cv=10, random_params=None, random_n_iter=10,
                         bayes_pbounds=None, bayes_int_params=None, bayes_n_iter=30, 
                         random_state=None, n_jobs=-1, solver='lbfgs',
@@ -611,16 +629,16 @@
                                                     verbose = verbose,
                                                     early_stopping=early_stopping,
                                                     learning_rate=learning_rate,
                                                     learning_rate_init=learning_rate_init
                                                     ))]) # For replication
 
 
-        model_=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
-        return model_
+        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        return self.model
         
 
 
     #do the same for knn_classifier
     def KNN_Classifier(self,X_train,y_train,ordinal_cat_cols=None, scoring='accuracy',
                         grid_params={'KNN__n_neighbors': [3,10,25,60]},
                         cv=10, random_params=None, random_n_iter=10,  bayes_pbounds=None,
@@ -703,107 +721,156 @@
             assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
             assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
 
         preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
         pipe = Pipeline(steps=[('Prep', preprocessor),
                             ('KNN', KNeighborsClassifier(n_jobs=n_jobs, random_state=random_state))])
         
-        model_=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        self.model=train_bayes_or_grid_search(X_train,y_train,bayes_pbounds,grid_params,random_params,n_jobs,pipe,scoring,bayes_int_params,bayes_n_iter,sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
 
-        return model_
+        return self.model
 
 
     
 
     #do the same for a decision tree
     def DecisionTree_Classifier(self,X_train,y_train, ordinal_cat_cols=None, scoring='accuracy',
                             grid_params={'DT__max_depth': [3,5,7,10],
                                 'DT__min_samples_split': [2,3,4],
                                 'DT__min_samples_leaf': [4,5,6],
                                 'DT__max_features': ['auto','sqrt','log2',None]},
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None, 
                             bayes_int_params=None, bayes_n_iter=30, class_weight=None, sample_weight=None, random_state=None, n_jobs=-1):
             
-            """
-            This method performs a Decision Tree classification model with grid search or bayesian optimization.
-    
-            Parameters
-            ----------
-            X_train : pandas dataframe
-                Training set.
-    
-            y_train : pandas dataframe
-                Training set labels.
-    
-            ordinal_cat_cols : list, optional
-                List of ordinal categorical variables. The default is None.
-    
-            scoring : str, optional
-                Evaluation metric. The default is 'accuracy'.
-    
-            grid_params : dict, optional
-                Dictionary of parameters for grid search. The default is
-            
-            cv : int, optional
-                Number of folds for cross validation. The default is 10.
+        """
+        This method performs a Decision Tree classification model with grid search or bayesian optimization.
 
-            random_params : dict, optional
-                Dictionary of parameters for random search. The default is None.
+        Parameters
+        ----------
+        X_train : pandas dataframe
+            Training set.
 
-            random_n_iter : int, optional
-                Number of iterations for random search. The default is 10.
-            
-            bayes_pbounds : dict, optional
-                Dictionary of parameters for bayesian optimization. The default is None.
-            
-            bayes_int_params : list, optional
-                List of parameters for bayesian optimization that are integers. The default is None.
+        y_train : pandas dataframe
+            Training set labels.
 
-            bayes_n_iter : int, optional
-                Number of iterations for bayesian optimization. The default is 30.
-            
-            random_state : int, optional
-                Random state. The default is None.
-            
-            n_jobs : int, optional
-                Number of jobs. The default is -1.
-            
-            Returns
-            -------
-            model_ : sklearn model
-                Trained model.
-            
-            """
+        ordinal_cat_cols : list, optional
+            List of ordinal categorical variables. The default is None.
 
-            print(" INFO: Agurments params must start as 'DT__param'" + '\n' "INFO: Default params in Documentation for Decision Tree are: ", dt_default_params_clf)
-            print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
-            f'bayes_n_iter = {bayes_n_iter}', f'class_weigth = {class_weight}', f'bayes_pbounds = {bayes_pbounds}', 
-            f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
-            assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
-            assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter values"
-            assert random_params is None or isinstance(random_params, dict), "In case of random search, random_param_grid must be a dictionary of parameter values"
-            assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
-            assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
-            assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
-            #DT__ is the prefix for every hyperparameter in the Decision Tree model
-            if grid_params is not None and random_params is None and bayes_pbounds is None:
-                assert all('DT__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'DT__'"
-            elif random_params is not None:
-                assert all('DT__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'DT__'"
-            elif bayes_pbounds is not None:
-                assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
-                assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
+        scoring : str, optional
+            Evaluation metric. The default is 'accuracy'.
 
-            preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
-            pipe = Pipeline(steps=[('Prep', preprocessor),
-                                ('DT', DecisionTreeClassifier(random_state=random_state,class_weight=class_weight))])
-            
-            model_=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params,n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+        grid_params : dict, optional
+            Dictionary of parameters for grid search. The default is
+        
+        cv : int, optional
+            Number of folds for cross validation. The default is 10.
+
+        random_params : dict, optional
+            Dictionary of parameters for random search. The default is None.
 
-            return model_
+        random_n_iter : int, optional
+            Number of iterations for random search. The default is 10.
+        
+        bayes_pbounds : dict, optional
+            Dictionary of parameters for bayesian optimization. The default is None.
+        
+        bayes_int_params : list, optional
+            List of parameters for bayesian optimization that are integers. The default is None.
+
+        bayes_n_iter : int, optional
+            Number of iterations for bayesian optimization. The default is 30.
+        
+        random_state : int, optional
+            Random state. The default is None.
+        
+        n_jobs : int, optional
+            Number of jobs. The default is -1.
+        
+        Returns
+        -------
+        model_ : sklearn model
+            Trained model.
+        
+        """
+
+        print(" INFO: Agurments params must start as 'DT__param'" + '\n' "INFO: Default params in Documentation for Decision Tree are: ", dt_default_params_clf)
+        print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
+        f'bayes_n_iter = {bayes_n_iter}', f'class_weigth = {class_weight}', f'bayes_pbounds = {bayes_pbounds}', 
+        f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+        assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
+        assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter values"
+        assert random_params is None or isinstance(random_params, dict), "In case of random search, random_param_grid must be a dictionary of parameter values"
+        assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
+        assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
+        assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
+        #DT__ is the prefix for every hyperparameter in the Decision Tree model
+        if grid_params is not None and random_params is None and bayes_pbounds is None:
+            assert all('DT__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'DT__'"
+        elif random_params is not None:
+            assert all('DT__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'DT__'"
+        elif bayes_pbounds is not None:
+            assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
+            assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
+
+        preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
+        pipe = Pipeline(steps=[('Prep', preprocessor),
+                            ('DT', DecisionTreeClassifier(random_state=random_state,class_weight=class_weight))])
+        
+        self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params,n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter)
+
+        return self.model
+    #save model
+    def save(self):
+        """
+        Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
+
+        Parameters
+        ----------
+        model_name : str
+            Name of the model.
+            The model is stored in the models folder. with the model name provided
+
+        Returns
+        -------
+        None.
+
+        """
+        assert self._model is not None , "Model not trained yet"
+        #create folder if not exists where the model will be saved
+        path = f'./models/{self.model_name}'
+        if not os.path.exists(path):
+            os.makedirs(path)
+
+        joblib.dump(self._model, os.path.join(path, self.model_name+'.joblib'))
+        #save cv results if exists grid search or random search
+        if hasattr(self._model, 'cv_results_'):
+            df = pd.DataFrame(self._model.cv_results_)
+            df.sort_values('rank_test_score', inplace=True)
+            df.to_excel(os.path.join(path, self.model_name+'_cv_results.xlsx'), index=False)
+    #load model
+    def load(self):
+
+        """
+        Loads a model from a file.
+
+        Parameters
+        ----------
+        model_name : str
+            Name of the model.
+            The model is stored in the models folder. with the model name provided
+
+        Returns
+        -------
+        None.
+
+        """
+        assert self.model_name+'.joblib' in os.listdir('./models'), "Model not found"
+        path = f'./models/{self.model_name}/{self.model_name}'+'.joblib'
+        self.model = joblib.load(path)
+        return self.model
     
 #-------------------------------------------------------------------------------------------------------------------REGRESSION-------------------------------------------------------------------------------------------------------------#
 class Regression:
     """
     This class contains all regression models that are considered relevant.
     Its up to add more models in the future thta could be suggested by the user.
     """
@@ -811,16 +878,17 @@
     RandomForest_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     XGBoost_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     LogisticRegression_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     DecisionTree_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     KNN_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     MLP_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
 
-    def __init__(self):
-        pass
+    def __init__(self,model_name:str):
+        self.model = None
+        self.model_name = model_name
 
     def RandomForest_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error', criterion="friedman_mse",
                             grid_params={'RF__n_estimators': [100, 200, 300, 400, 500],
                                 'RF__max_depth': [3,5,7,10],
                                 'RF__min_samples_split': [2,3,4],
                                 'RF__min_samples_leaf': [4,5,6],
                                 'RF__max_features': ['auto','sqrt','log2',None]}, 
@@ -900,18 +968,18 @@
                 assert all('RF__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'RF__'"
                 assert all('RF__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'RF__'"
 
             preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('RF', RandomForestRegressor(criterion=criterion,random_state=random_state,n_jobs=n_jobs))])
             
-            model_=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter, X_prev=X_prev
+            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter, X_prev=X_prev
                                               ,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
-            return model_
+            return self.model
     
     def XGB_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'XGB__n_estimators': [100, 200, 300, 400, 500],
                                 'XGB__max_depth': [3,5,7,10],
                                 'XGB__learning_rate': [0.01,0.05,0.1,0.15,0.2],
                                 'XGB__min_child_weight': [1,3,5,7],
                                 'XGB__gamma': [0.0,0.1,0.2,0.3,0.4],
@@ -991,18 +1059,18 @@
                 assert all('XGB__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'XGB__'"
                 assert all('XGB__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'XGB__'"
             
             preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('XGB', XGBRegressor(random_state=random_state,n_jobs=n_jobs))])
             
-            model_=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter, X_prev=X_prev,
+            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv,random_n_iter=random_n_iter, X_prev=X_prev,
                                               columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
-            return model_
+            return self.model
     
     def Linear_Regression(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'LR__fit_intercept': [True, False],
                                 'LR__normalize': [True, False],
                                 'LR__copy_X': [True, False]}, 
                             cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1, X_prev=None,
@@ -1079,18 +1147,18 @@
                 assert all('LR__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LR__'"
                 assert all('LR__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LR__'"
             
             preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('LR', LinearRegression())])
             
-            model_=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight, cv=cv, random_n_iter=random_n_iter,
+            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight, cv=cv, random_n_iter=random_n_iter,
                                               X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
-            return model_
+            self.model
     
     def KNN_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'KNN__n_neighbors': [3,5,7,9,11,13,15,17,19,21,23,25,27,29,31,33,35,37,39,41,43,45,47,49,51,53,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,87,89,91,93,95,97,99],
                                 'KNN__weights': ['uniform', 'distance'],
                                 'KNN__algorithm': ['auto', 'ball_tree', 'kd_tree', 'brute'],
                                 'KNN__leaf_size': [10,20,30,40,50,60,70,80,90,100],
                                 'KNN__p': [1,2]}, 
@@ -1169,18 +1237,18 @@
                 assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
                 assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
 
             preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('KNN', KNeighborsRegressor())])
             
-            model_=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight, cv=cv, random_n_iter=random_n_iter,
+            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight, cv=cv, random_n_iter=random_n_iter,
                                               X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
-            return model_
+            self.model
     
     def DecisionTree_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'DT__criterion': ["squared_error", "friedman_mse", "absolute_error", "poisson"],
                                 'DT__max_depth': [None,2,3,4,5],
                                 'DT__min_samples_split': [2,3,4,],
                                 'DT__max_features': ['auto', 'sqrt', 'log2'],
                                 'DT__min_impurity_decrease': [0.0,0.1,0.2]}, 
@@ -1259,18 +1327,18 @@
                 assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
                 assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
             
             preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('DT', DecisionTreeRegressor(random_state=random_state))])
             
-            model_=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv, random_n_iter=random_n_iter,
+            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv, random_n_iter=random_n_iter,
                                               X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
-            return model_
+            self.model
     
     def MLP_Regressor(self, X_train, y_train, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'MLP__hidden_layer_sizes': [(3,),(5,)],
                                 'MLP__activation': ['identity', 'logistic', 'tanh', 'relu'],
                                 'MLP__solver': ['lbfgs', 'sgd', 'adam'],
                                 'MLP__alpha': [0.0001,0.001,0.01,0.1,1,10,100],
                                 'MLP__max_iter': [200]},
@@ -1356,18 +1424,87 @@
 
             
             preprocessor=automatic_preprocessor(X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor), 
                                       ('MLP', MLPRegressor(random_state=random_state))])
             
 
-            model_=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv, random_n_iter=random_n_iter,
+            self.model=train_bayes_or_grid_search(X_train, y_train, bayes_pbounds, grid_params, random_params, n_jobs, pipe, scoring, bayes_int_params, bayes_n_iter, sample_weight=sample_weight,cv=cv, random_n_iter=random_n_iter,
                                               X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            return self.model
+    
+
+    def save(self):
+        """
+        Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
+
+        Parameters
+        ----------
+        model_name : str
+            Name of the model.
+            The model is stored in the models folder. with the model name provided
+
+        Returns
+        -------
+        None.
+
+        """
+        assert self.model is not None , "Model not trained yet"
+        #create folder if not exists where the model will be saved
+        path = f'./models/{self.model_name}'
+        if not os.path.exists(path):
+            os.makedirs(path)
+
+        joblib.dump(self.model, os.path.join(path, self.model_name+'.joblib'))
+        #save cv results if exists grid search or random search
+        if hasattr(self.model, 'cv_results_'):
+            df = pd.DataFrame(self.model.cv_results_)
+            df.sort_values('rank_test_score', inplace=True)
+            df.to_excel(os.path.join(path, self.model_name+'_cv_results.xlsx'), index=False)
+
+            #save the best register of the cv_results in a second sheet of excel file called summary_models.xlsx
+            df_best = pd.DataFrame(df.iloc[0]).T
+            df_best['model_name'] = self.model_name
+            #set the model_name as the firts column
+            cols = df_summary.columns.tolist()
+            cols = cols[-1:] + cols[:-1]
+            df_best = df_best[cols]
+
+            # save in the second sheet
+            file_path = './models/summary_models.xlsx'
+            if os.path.exists(file_path):
+                df_summary = pd.read_excel(file_path, sheet_name='Sheet2')
+                df_summary = pd.concat([df_summary, df_best], axis=0,ignore_index=True)
+                df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
+            else:
+                df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
+
+
+    def load(self):
+
+        """
+        Loads a model from a file.
+
+        Parameters
+        ----------
+        model_name : str
+            Name of the model.
+            The model is stored in the models folder. with the model name provided
+
+        Returns
+        -------
+        None.
 
-            return model_
+        """
+        assert self.model_name+'.joblib' in os.listdir('./models'), "Model not found"
+        path = f'./models/{self.model_name}/{self.model_name}'+'.joblib'
+        self.model = joblib.load(path)
+        return self.model
+
+
```

### Comparing `gmltools-0.0.40/src/gmltools/models/models_info.py` & `gmltools-0.0.41/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.41/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.41/src/gmltools/models_analysis/classification_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pandas.api.types import is_datetime64_any_dtype as is_datetime
 import math
 from sklearn.linear_model import LinearRegression
 import statsmodels.api as sm
 from sklearn.pipeline import Pipeline
 from scipy import stats
 from sklearn.calibration import calibration_curve
+import os
 from sklearn.metrics import (
     confusion_matrix,
     f1_score,
     brier_score_loss,
     precision_score,
     recall_score,
     accuracy_score,
@@ -998,15 +999,16 @@
 
 
 
 class Ranalysis:
     """
     Class to perform analysis of regression models.
     """
-    def __init__(self,model, X_train, y_train, X_test = None, y_test = None,X_val=None, y_val=None, X_prev = None):
+    def __init__(self,model_name:str, model, X_train, y_train, X_test = None, y_test = None,X_val=None, y_val=None, X_prev = None):
+        self.model_name = model_name
         self.model = model
         self.X_train = X_train
         self.y_train = y_train
         if X_test is not None and y_test is not None:
             assert isinstance(X_test, pd.core.frame.DataFrame), 'X_test must be a pandas DataFrame'
             assert isinstance(y_test, pd.core.series.Series), 'y_test must be a pandas Series'
             self.X_test = X_test
@@ -1015,15 +1017,16 @@
             assert isinstance(X_val, pd.core.frame.DataFrame), 'X_val must be a pandas DataFrame'
             assert isinstance(y_val, pd.core.series.Series), 'y_val must be a pandas Series'
             self.X_val = X_val
             self.y_val = y_val
         if X_prev is not None:
             assert isinstance(X_prev,pd.core.frame.DataFrame)
             self.X_prev = X_prev
-    def residual_analysis(self, train_or_test_or_val:str, remove_vars=None, figsize=(20, 10), bins=30, smooth_order=5):
+    #residual analysis of the models
+    def residual_analysis(self, train_or_test_or_val:str, remove_vars:list=None, figsize=(20, 10), bins:int=30, smooth_order:int=5, save:bool=True):
         """
         Generate a residual analysis plot. Is used to determine if the model is overfitting or underfitting.
         Studying the variance and the bias of the residuals.
 
         Parameters
         ----------
         train_or_test : str
@@ -1040,14 +1043,17 @@
         
         Returns
         -------
         None.
             Plot is generated.
         """
         sns.set()
+        #assertions
+        if save:
+            assert os.path.exists(f'./models/{self.model_name})'), f'./models/{self.model_name} does not exist. Please create the directory and try again.'
         assert train_or_test_or_val.lower() in ['train', 'test','val'], "train_or_test must be either 'train' or 'test'"
         assert isinstance(figsize, tuple) and len(figsize) == 2, "figsize must be a tuple and figsize must be a tuple of length 2"
         assert isinstance(bins, int) and bins > 0, "bins must be an integer greater than 0"
         assert isinstance(smooth_order, int) and smooth_order > 0, "smooth_order must be an integer greater than 0"
         # Create the residuals
         assert train_or_test_or_val.lower() in ['train','test','val'], "train_or_test must be 'train', 'test' or 'val'"
         assert remove_vars is None or isinstance(remove_vars, list), "remove_vars must be a list"
@@ -1109,16 +1115,19 @@
                     else:
                         sns.regplot(x=df.columns.values.tolist()[input_num], y='residuals', data=df, ax=ax, order=smooth_order, ci=None, line_kws={'color':'navy'})
                         ax.set_title(df.columns.values.tolist()[input_num] + ' vs ' + 'residuals')
 
                 input_num += 1
             else:
                 ax.axis('off')
+        plt.suptitle(self.model_name + train_or_test_or_val.capitalize() + ' Residual Analysis', fontsize=18)
         plt.show()
-        return fig
+        self.fig_residual_analysis = fig
+        if save:
+            fig.savefig(f'./models/{self.model_name}/residual_analysis_{train_or_test_or_val.lower()}.png')
 
 
 
     def summaryLinReg(self, use_old:bool= True):
         """
         Summary of scikit 'LinearRegression' models.
         
@@ -1264,15 +1273,15 @@
             den_f = RSS / (n - k - 1)
             f = num_f / den_f
             p_f = 1 - stats.f.cdf(f, k, (n - k - 1)) 
             print(f'F-statistic: {round(f, 3)} on {k} and {n - k - 1} DOF, P(F-statistic): {round(p_f, 3)}')
             return 
         
 
-    def permutation_importance(self,n_repeats:int=10,random_state=None,figsize=(12, 4),title='Permutation Importance'):
+    def permutation_importance(self,n_repeats:int=10,random_state=None,figsize=(12, 4),title='Permutation Importance',rotation:int=90, save:bool = True):
         """
         Generate a permutation importance plot. Is used
         to determine the importance of each feature in the model.
 
         Parameters
         ----------
         n_repeats : int, optional
@@ -1285,35 +1294,39 @@
             Size of the figure. The default is (12, 4).
 
         Returns
         -------
         None.
             Plot is generated.
         """
+        if save:
+            assert os.path.exists(f'./models/{self.model_name})'), f'./models/{self.model_name} does not exist. Please create the directory and try again.'
         assert not isinstance(self.model, list), 'model must be a single model, not a list. Comparison of models is only supported for plot_roc_curve(), plot_calibration_curve() and plot_accuracy_across_thresholds()'
         assert n_repeats > 0, "n_repeats must be greater than 0 for permutation importance"
         assert random_state is None or isinstance(random_state, int), "random_state must be an integer or None"
         assert isinstance(figsize, tuple) and len(figsize) == 2, "figsize must be a tuple and figsize must be a tuple of length 2"
         importances = permutation_importance(self.model, 
                                     self.X_train, self.y_train,
                                     n_repeats=n_repeats,
                                     random_state=random_state)
         
         fig = plt.figure(2, figsize=figsize) 
         plt.bar(self.X_train.columns, importances.importances_mean, yerr=importances.importances_std,color='black', alpha=0.5)
         plt.xlabel('Feature')
         plt.ylabel('Permutation Importance')
-        plt.title(title)
-        plt.xticks(rotation=90)
+        plt.title(self.model_name + " " + title)
+        plt.xticks(rotation=rotation)
         plt.grid()
         plt.show()
-        return fig
+        self.fig_permutation_importance = fig
+        if save:
+            fig.savefig(f'./models/{self.model_name}/permutation_importance.png')
 
 
-    def get_metrics_summary(self, model_name:str, sample_weight=None, multioutput='uniform_average')-> pd.DataFrame:
+    def get_metrics_summary(self, sample_weight:str=None, multioutput='uniform_average', save:bool = True)-> pd.DataFrame:
         """
         Prints a summary of the metrics of a model for a given threshold
         and returns them in a DataFrame
 
         Parameters
         ------------
         model_name : str
@@ -1354,35 +1367,32 @@
         sample_weight = {
             'train': train_weights,
             'test': test_weights,
             'validation': val_weights
 
         """
         assert not isinstance(self.model, list), 'model must be a single model, not a list. Comparison of models is only supported for plot_roc_curve(), plot_calibration_curve() and plot_accuracy_across_thresholds()'
-        assert isinstance(model_name,str), "model_name must be a string"
         assert multioutput in ['uniform_average','raw_values']
         assert sample_weight is None or isinstance(sample_weight, dict), "sample_weight must be None or a dictionary"
         
-        data_dict={'Train': {'data': self.X_train,'target': self.y_train},
-            'Test': {'data': self.X_test, 'target': self.y_test} }
-        #add validation if it exists
-        if hasattr(self, 'X_val') and hasattr(self, 'y_val'):
-            data_dict['Val']={'data': self.X_val, 'target': self.y_val}
-
+        data_dict={'Train': {'data': self.X_train,'target': self.y_train}}
+        #add test and validation  if it exists
         if hasattr(self,'X_test') and hasattr(self,'y_test'):
             data_dict['Test']={'data': self.X_test, 'target': self.y_test}
+        if hasattr(self, 'X_val') and hasattr(self, 'y_val'):
+            data_dict['Val']={'data': self.X_val, 'target': self.y_val}
             
         # Get the predicted probabilities and predictions
         predictions_dict = {}
         for dataset_type in data_dict.keys():
             predictions_dict[dataset_type] = self.model.predict(data_dict[dataset_type]['data'])
         # Calculate and print the metrics for each set
         metrics_dict = {
-            'Model': model_name,
-            'Weights': [True if sample_weight is not None else "None"]
+            'Model': self.model_name,
+            'Weights': sample_weight,
         }
         # Iterate over the metrics
         for metric in REG_METRIC_FUNCS_SUMMARY.keys():
             # Print a separator
             #if multi_class print ("multiclass")
             # Iterate over the sets
             for dataset_type, predictions in predictions_dict.items():
@@ -1419,15 +1429,31 @@
                 metrics_dict["Search"] = 'Random' + str(self.model.param_distributions)
 
         except:
             metrics_dict["best_params"] = None
             metrics_dict["Search"] = None
         
         # Return the metrics as a DataFrame
-        return pd.DataFrame(metrics_dict,index=[0])
+        summary=pd.DataFrame(metrics_dict,index=[0])
+
+        self.metrics_summary = summary
+        if save:
+            if not os.path.exists('./models'):
+                os.makedirs('./models')
+
+            if not os.path.isfile('./models/summary_models.xlsx'):
+                df=pd.DataFrame(columns=summary.columns)
+                #save the summary data to the excel
+                df.to_excel('./models/summary_models.xlsx',index=False)
+            else:
+                df=pd.read_excel('./models/summary_models.xlsx')
+                #concat the summary data to the excel
+                df=pd.concat([df,summary],axis=0,ignore_index=True)
+    
+        return  self.metrics_summary
```

### Comparing `gmltools-0.0.40/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.41/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.41/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.41/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.41/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.40/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.41/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.40
+Version: 0.0.41
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.40/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.41/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

