# Comparing `tmp/rapidpredict-0.0.0.1.tar.gz` & `tmp/rapidpredict-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpredict-0.0.0.1.tar", last modified: Mon Apr 10 16:32:48 2023, max compression
+gzip compressed data, was "rapidpredict-0.0.0.2.tar", last modified: Mon Apr 10 22:33:06 2023, max compression
```

## Comparing `rapidpredict-0.0.0.1.tar` & `rapidpredict-0.0.0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 16:32:48.784701 rapidpredict-0.0.0.1/
--rw-rw-rw-   0        0        0     1028 2023-04-10 16:32:48.783725 rapidpredict-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-04-10 16:29:09.000000 rapidpredict-0.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 16:32:48.782778 rapidpredict-0.0.0.1/rapidpredict.egg-info/
--rw-rw-rw-   0        0        0     1028 2023-04-10 16:32:48.000000 rapidpredict-0.0.0.1/rapidpredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-10 16:32:48.000000 rapidpredict-0.0.0.1/rapidpredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 16:32:48.000000 rapidpredict-0.0.0.1/rapidpredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-10 16:32:48.000000 rapidpredict-0.0.0.1/rapidpredict.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 16:32:48.000000 rapidpredict-0.0.0.1/rapidpredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 16:32:48.784701 rapidpredict-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1689 2023-04-10 16:31:19.000000 rapidpredict-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:33:06.007966 rapidpredict-0.0.0.2/
+-rw-rw-rw-   0        0        0     4570 2023-04-10 22:33:06.007966 rapidpredict-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 22:33:05.987335 rapidpredict-0.0.0.2/rapidpredict/
+-rw-rw-rw-   0        0        0       19 2023-04-10 22:32:28.000000 rapidpredict-0.0.0.2/rapidpredict/Regression.py
+-rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.2/rapidpredict/__init__.py
+-rw-rw-rw-   0        0        0    16510 2023-04-10 22:16:02.000000 rapidpredict-0.0.0.2/rapidpredict/classification.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:33:06.006987 rapidpredict-0.0.0.2/rapidpredict.egg-info/
+-rw-rw-rw-   0        0        0     4570 2023-04-10 22:33:05.000000 rapidpredict-0.0.0.2/rapidpredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-04-10 22:33:05.000000 rapidpredict-0.0.0.2/rapidpredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:33:05.000000 rapidpredict-0.0.0.2/rapidpredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-10 22:33:05.000000 rapidpredict-0.0.0.2/rapidpredict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:33:05.000000 rapidpredict-0.0.0.2/rapidpredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:33:06.008909 rapidpredict-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1741 2023-04-10 22:32:41.000000 rapidpredict-0.0.0.2/setup.py
```

### Comparing `rapidpredict-0.0.0.1/setup.py` & `rapidpredict-0.0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.0.1'
+VERSION = '0.0.0.2'
 DESCRIPTION = 'rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.'
 LONG_DESCRIPTION = 'This repository contains a Python-based framework for rapid prediction of machine learning models\
       that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn.\
           It''s designed to provide a quick way to test various algorithms on a given dataset and compare their performance.'
 
 # Setting up
 setup(
     name="rapidpredict",
     version=VERSION,
     author="Synthetic Dataset AI Team",
-    author_email="<admin@syntheticdataset.ai>",
+    author_email="<nematiusa@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['python', 'pandas', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'seaborn', 'tqdm'],
+    install_requires=["click", "scikit-learn", "pandas"  , "tqdm" , "joblib",  "lightgbm" ,  "xgboost"  , "itables" ,"catboost" , "colorlover" , "plotly" , "IPython"],
     keywords=['python', 'pandas', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'seaborn'],
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

