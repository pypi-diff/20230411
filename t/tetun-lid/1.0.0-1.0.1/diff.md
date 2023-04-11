# Comparing `tmp/tetun_lid-1.0.0.tar.gz` & `tmp/tetun_lid-1.0.1.tar.gz`

## Comparing `tetun_lid-1.0.0.tar` & `tetun_lid-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/.DS_Store
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/Pipfile
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/tetunlid/__init__.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/tetunlid/lid.py
--rw-r--r--   0        0        0 20889678 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/tetunlid/model/tetun_lid_model.pkl
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/LICENSE
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/README.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 tetun_lid-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/.DS_Store
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/Pipfile
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/tetunlid/__init__.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/tetunlid/lid.py
+-rw-r--r--   0        0        0 20889678 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/tetunlid/model/tetun_lid_model.pkl
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/README.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/PKG-INFO
```

### Comparing `tetun_lid-1.0.0/.DS_Store` & `tetun_lid-1.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.0/Pipfile.lock` & `tetun_lid-1.0.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.0/tetunlid/lid.py` & `tetun_lid-1.0.1/tetunlid/lid.py`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.0/tetunlid/model/tetun_lid_model.pkl` & `tetun_lid-1.0.1/tetunlid/model/tetun_lid_model.pkl`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.0/LICENSE` & `tetun_lid-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.0/README.md` & `tetun_lid-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ### Dependecies
 
 Tetun LID depends on the following packages:
 
 * joblib
 * scikit-learn
-* Unicode
+* Unidecode
 
 To install the dependencies packages, run these commands in your console:
 
 ```
 pip install joblib
 pip install scikit-learn
 pip install Unidecode
@@ -207,10 +207,10 @@
 ```
 
 There are a few more ways to read file contents that you can use to achieve the same output.
 
 
 ### Additional notes
 
-1. Please follow the instruction as it is and try to understand how it works. All the dependencies need to be installed accordingly.
+1. Please follow the instruction carefully and try to understand how it works. All the dependencies need to be installed properly.
 2. If you encountered an `AttributeError: 'list' object has no attribute 'predict_proba'`, you might have some issues while installing the package. Please send me an email, and I will guide you on how to handle the error.
 3. Please make sure that you use the latest version of Tetun LID. To get the latest version, run this command in your console: `pip install --upgrade tetun-lid`.
```

### Comparing `tetun_lid-1.0.0/PKG-INFO` & `tetun_lid-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tetun_lid
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tetun Language Identification Model
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -26,15 +26,15 @@
 
 ### Dependecies
 
 Tetun LID depends on the following packages:
 
 * joblib
 * scikit-learn
-* Unicode
+* Unidecode
 
 To install the dependencies packages, run these commands in your console:
 
 ```
 pip install joblib
 pip install scikit-learn
 pip install Unidecode
@@ -219,10 +219,10 @@
 ```
 
 There are a few more ways to read file contents that you can use to achieve the same output.
 
 
 ### Additional notes
 
-1. Please follow the instruction as it is and try to understand how it works. All the dependencies need to be installed accordingly.
+1. Please follow the instruction carefully and try to understand how it works. All the dependencies need to be installed properly.
 2. If you encountered an `AttributeError: 'list' object has no attribute 'predict_proba'`, you might have some issues while installing the package. Please send me an email, and I will guide you on how to handle the error.
 3. Please make sure that you use the latest version of Tetun LID. To get the latest version, run this command in your console: `pip install --upgrade tetun-lid`.
```

