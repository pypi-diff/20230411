# Comparing `tmp/rapidpredict-0.0.0.4.tar.gz` & `tmp/rapidpredict-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpredict-0.0.0.4.tar", last modified: Tue Apr 11 00:35:18 2023, max compression
+gzip compressed data, was "rapidpredict-0.0.0.5.tar", last modified: Tue Apr 11 02:45:13 2023, max compression
```

## Comparing `rapidpredict-0.0.0.4.tar` & `rapidpredict-0.0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 00:35:18.216823 rapidpredict-0.0.0.4/
--rw-rw-rw-   0        0        0     4574 2023-04-11 00:35:18.216823 rapidpredict-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 00:35:18.197087 rapidpredict-0.0.0.4/rapidpredict/
--rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.4/rapidpredict/__init__.py
--rw-rw-rw-   0        0        0    15653 2023-04-11 00:20:14.000000 rapidpredict-0.0.0.4/rapidpredict/supervised.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:35:18.215876 rapidpredict-0.0.0.4/rapidpredict.egg-info/
--rw-rw-rw-   0        0        0     4574 2023-04-11 00:35:17.000000 rapidpredict-0.0.0.4/rapidpredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-11 00:35:18.000000 rapidpredict-0.0.0.4/rapidpredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 00:35:17.000000 rapidpredict-0.0.0.4/rapidpredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-11 00:35:17.000000 rapidpredict-0.0.0.4/rapidpredict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 00:35:17.000000 rapidpredict-0.0.0.4/rapidpredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 00:35:18.216823 rapidpredict-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1798 2023-04-11 00:20:32.000000 rapidpredict-0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:45:13.552792 rapidpredict-0.0.0.5/
+-rw-rw-rw-   0        0        0     4574 2023-04-11 02:45:13.552713 rapidpredict-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 02:45:13.530576 rapidpredict-0.0.0.5/rapidpredict/
+-rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.5/rapidpredict/__init__.py
+-rw-rw-rw-   0        0        0    21564 2023-04-11 02:42:51.000000 rapidpredict-0.0.0.5/rapidpredict/supervised.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:45:13.551210 rapidpredict-0.0.0.5/rapidpredict.egg-info/
+-rw-rw-rw-   0        0        0     4574 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:45:13.552792 rapidpredict-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1810 2023-04-11 02:45:05.000000 rapidpredict-0.0.0.5/setup.py
```

### Comparing `rapidpredict-0.0.0.4/PKG-INFO` & `rapidpredict-0.0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rapidpredict-0.0.0.4/README.md` & `rapidpredict-0.0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rapidpredict-0.0.0.4/rapidpredict.egg-info/PKG-INFO` & `rapidpredict-0.0.0.5/rapidpredict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rapidpredict-0.0.0.4/setup.py` & `rapidpredict-0.0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.0.4'
+VERSION = '0.0.0.5'
 DESCRIPTION = 'rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.'
 LONG_DESCRIPTION = 'This repository contains a Python-based framework for rapid prediction of machine learning models\
       that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn.\
           It''s designed to provide a quick way to test various algorithms on a given dataset and compare their performance.'
 
 # Setting up
 setup(
@@ -20,15 +20,15 @@
     author="Synthetic Dataset AI Team",
     author_email="<nematiusa@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=["click", "scikit-learn", "pandas"  , "tqdm" , "joblib", \
-                       "lightgbm" ,  "xgboost"  , "itables" ,"catboost" , "colorlover"\
+                       "lightgbm" ,  "xgboost"  , "itables" ,"catboost" , "colorlover" , "seaborn"\
                           , "plotly" , "IPython"],
     keywords=['python', 'pandas', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'seaborn'],
     python_requires=">=3.8.1.7",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

