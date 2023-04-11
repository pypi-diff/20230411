# Comparing `tmp/stackingNT-0.0.1.tar.gz` & `tmp/stackingNT-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackingNT-0.0.1.tar", last modified: Mon Apr 10 02:40:50 2023, max compression
+gzip compressed data, was "stackingNT-0.0.2.tar", last modified: Tue Apr 11 05:19:11 2023, max compression
```

## Comparing `stackingNT-0.0.1.tar` & `stackingNT-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 02:40:50.468114 stackingNT-0.0.1/
--rw-rw-rw-   0        0        0    57719 2023-04-10 02:40:50.468114 stackingNT-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-10 02:40:50.469111 stackingNT-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-04-10 02:35:46.000000 stackingNT-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:40:50.448167 stackingNT-0.0.1/stackingNT/
--rw-rw-rw-   0        0        0       78 2023-04-07 06:24:54.000000 stackingNT-0.0.1/stackingNT/__init__.py
--rw-rw-rw-   0        0        0     3463 2023-04-07 06:32:03.000000 stackingNT-0.0.1/stackingNT/stackingnonlineartransformations.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:40:50.466119 stackingNT-0.0.1/stackingNT.egg-info/
--rw-rw-rw-   0        0        0    57719 2023-04-10 02:40:50.000000 stackingNT-0.0.1/stackingNT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-04-10 02:40:50.000000 stackingNT-0.0.1/stackingNT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 02:40:50.000000 stackingNT-0.0.1/stackingNT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-10 02:40:50.000000 stackingNT-0.0.1/stackingNT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 05:19:11.762627 stackingNT-0.0.2/
+-rw-rw-rw-   0        0        0     3347 2023-04-11 05:19:11.761630 stackingNT-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2688 2023-04-11 05:06:28.000000 stackingNT-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:19:11.762627 stackingNT-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-04-11 05:18:19.000000 stackingNT-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:19:11.742681 stackingNT-0.0.2/stackingNT/
+-rw-rw-rw-   0        0        0       78 2023-04-07 06:24:54.000000 stackingNT-0.0.2/stackingNT/__init__.py
+-rw-rw-rw-   0        0        0     3462 2023-04-11 05:17:23.000000 stackingNT-0.0.2/stackingNT/stackingnonlineartransformations.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:19:11.760633 stackingNT-0.0.2/stackingNT.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-04-11 05:19:11.000000 stackingNT-0.0.2/stackingNT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-04-11 05:19:11.000000 stackingNT-0.0.2/stackingNT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:19:11.000000 stackingNT-0.0.2/stackingNT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-11 05:19:11.000000 stackingNT-0.0.2/stackingNT.egg-info/top_level.txt
```

### Comparing `stackingNT-0.0.1/setup.py` & `stackingNT-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 
 # these things are needed for the README.md show on pypi
 here = os.path.abspath(os.path.dirname(__file__))
 
-with codecs.open(os.path.join(here, "3.md"), encoding="utf-8") as fh:
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Stacking algorithm optimisation'
 LONG_DESCRIPTION = 'Stacking algorithm optimisation'
 
 # Setting up
 setup(
     name="stackingNT",
     version=VERSION,
```

### Comparing `stackingNT-0.0.1/stackingNT/stackingnonlineartransformations.py` & `stackingNT-0.0.2/stackingNT/stackingnonlineartransformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         elif NT == "softmax":
             exps = np.exp(x - np.max(x, axis=-1, keepdims=True))
             return exps/np.sum(exps, axis=-1, keepdims=True)
         elif NT == "softplus":
             return np.log(1 + np.exp(x))
 
 
-    def base_model_fit(self, train_X, train_y, test_X, test_y,cv=10):
+    def base_model_fit(self, train_X, train_y, test_X, test_y, NT, cv=10):
         best_models = dict()
         for name in self.base_models.keys():
             model = self.base_models[name]
             cv_results = cross_validate(model, train_X, train_y.values, cv=cv, return_estimator=True, return_train_score=True)
             test_results = []
             for m in cv_results['estimator']:
                 test_results.append(m.score(test_X, test_y.values))
@@ -56,23 +56,23 @@
         test_[:,0:len(test_X.columns)] = test_X
 
         for i, name in enumerate(best_models):
             model = best_models[name]
             train_pred = model.predict(train_X)
             test_pred = model.predict(test_X)
 
-            train_[:, len(train_X.columns)+i] = self.NonlinearTransformations(train_pred,"sigmoid")
-            test_[:,len(test_X.columns)+i] = self.NonlinearTransformations(test_pred,"sigmoid")
+            train_[:, len(train_X.columns)+i] = self.NonlinearTransformations(train_pred,NT)
+            test_[:,len(test_X.columns)+i] = self.NonlinearTransformations(test_pred,NT)
 
             
         return train_, test_
 
-    def fit(self, train_X, train_y, test_X, test_y, cv=10):
+    def fit(self, train_X, train_y, test_X, test_y,NT, cv=10):
 
-        new_train, new_test = self.base_model_fit(train_X, train_y, test_X, test_y,cv)
+        new_train, new_test = self.base_model_fit(train_X, train_y, test_X, test_y, NT, cv)
         model = list(self.meta_model.values())[0]
         cv_results = cross_validate(model, new_train, train_y.values, cv=cv, return_estimator=True, return_train_score=True)
         test_results = []
         for m in cv_results['estimator']:
             test_results.append(m.score(new_test, test_y.values))
         ind = np.argmax(test_results)
         new_best_models = cv_results['estimator'][ind]
```

