# Comparing `tmp/dominance_analysis-1.1.8.tar.gz` & `tmp/dominance_analysis-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\sajan.kumar\Projects\dominance_analysis\dist\.tmp-_tshhsv2\dominance_analysis-1.1.8.tar", last modified: Thu Dec  8 05:30:58 2022, max compression
+gzip compressed data, was "C:\Users\sajan.kumar\Projects\dominance_analysis\dist\.tmp-sb7bl266\dominance_analysis-1.1.9.tar", last modified: Tue Apr 11 19:12:10 2023, max compression
```

## Comparing `dominance_analysis-1.1.8.tar` & `dominance_analysis-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/
--rw-rw-rw-   0        0        0     1091 2018-12-04 06:51:59.000000 dominance_analysis-1.1.8/LICENSE
--rw-rw-rw-   0        0        0       16 2018-12-05 12:11:14.000000 dominance_analysis-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1524 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      489 2019-05-30 07:47:26.000000 dominance_analysis-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/dominance_analysis/
--rw-rw-rw-   0        0        0      114 2019-01-02 07:50:53.000000 dominance_analysis-1.1.8/dominance_analysis/__init__.py
--rw-rw-rw-   0        0        0    23321 2021-03-06 11:22:51.000000 dominance_analysis-1.1.8/dominance_analysis/dominance.py
--rw-rw-rw-   0        0        0    21057 2019-02-14 14:58:04.000000 dominance_analysis-1.1.8/dominance_analysis/dominance_old.py
--rw-rw-rw-   0        0        0      283 2018-12-05 13:57:16.000000 dominance_analysis-1.1.8/dominance_analysis/test.py
-drwxrwxrwx   0        0        0        0 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/dominance_analysis.egg-info/
--rw-rw-rw-   0        0        0     1524 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/dominance_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/dominance_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/dominance_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-12-27 13:44:22.000000 dominance_analysis-1.1.8/dominance_analysis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      118 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/dominance_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/dominance_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-08 05:30:58.000000 dominance_analysis-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1925 2022-12-08 05:30:57.000000 dominance_analysis-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/
+-rw-rw-rw-   0        0        0     1091 2018-12-04 06:51:59.000000 dominance_analysis-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       16 2018-12-05 12:11:14.000000 dominance_analysis-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1524 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2019-05-30 07:47:26.000000 dominance_analysis-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/dominance_analysis/
+-rw-rw-rw-   0        0        0      114 2019-01-02 07:50:53.000000 dominance_analysis-1.1.9/dominance_analysis/__init__.py
+-rw-rw-rw-   0        0        0    23632 2023-04-11 19:08:19.000000 dominance_analysis-1.1.9/dominance_analysis/dominance.py
+-rw-rw-rw-   0        0        0    21057 2019-02-14 14:58:04.000000 dominance_analysis-1.1.9/dominance_analysis/dominance_old.py
+-rw-rw-rw-   0        0        0      283 2018-12-05 13:57:16.000000 dominance_analysis-1.1.9/dominance_analysis/test.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/dominance_analysis.egg-info/
+-rw-rw-rw-   0        0        0     1524 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/dominance_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/dominance_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/dominance_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2018-12-27 13:44:22.000000 dominance_analysis-1.1.9/dominance_analysis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      118 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/dominance_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/dominance_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 19:12:10.000000 dominance_analysis-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1925 2023-04-11 18:53:10.000000 dominance_analysis-1.1.9/setup.py
```

### Comparing `dominance_analysis-1.1.8/LICENSE` & `dominance_analysis-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dominance_analysis-1.1.8/PKG-INFO` & `dominance_analysis-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominance_analysis
-Version: 1.1.8
+Version: 1.1.9
 Summary: Dominance Analysis
 Home-page: https://github.com/bhagatsajan0073/dominance_analysis
 Author: Sajan Kumar Bhagat, Kunjithapatham Sivakumar, Shashank Shekhar,Bala Koteshwar Kolluri
 Author-email: bhagat.sajan0073@gmail.com, s.vibish@gmail.com, quintshekhar@gmail.com, balakoteshwar@gmail.com
 Maintainer: Sajan Kumar Bhagat, Kunjithapatham Sivakumar, Shashank Shekhar, Bala Koteshwar Kolluri
 Maintainer-email: bhagat.sajan0073@gmail.com, s.vibish@gmail.com, quintshekhar@gmail.com, balakoteshwar@gmail.com
 License: MIT
```

### Comparing `dominance_analysis-1.1.8/dominance_analysis/dominance.py` & `dominance_analysis-1.1.9/dominance_analysis/dominance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from itertools import combinations
 import sklearn
 from sklearn.linear_model import LinearRegression
 from sklearn.datasets import load_breast_cancer
-from sklearn.datasets import load_boston
+# from sklearn.datasets import load_boston
 from tqdm import tqdm
 from sklearn.feature_selection import SelectKBest,chi2,f_regression
 import pandas as pd
 from plotly import offline
 from plotly.offline import init_notebook_mode,iplot
 import cufflinks as cf
 from sklearn.linear_model import LogisticRegression
@@ -549,13 +549,18 @@
 		breast_cancer_data['target_names']=breast_cancer_data['target'].map(target_dict)
 		return breast_cancer_data.iloc[:,:-1]
 
 	@classmethod
 	def get_boston(cls):
 		print("""The copy of Boston Housing Dataset is downloaded from: https://www.cs.toronto.edu/~delve/data/boston/bostonDetail.html""")
 		print("""Internally using load_boston function from sklearn.datasets """)
-		boston_data=pd.DataFrame(data=load_boston()['data'],columns=load_boston()['feature_names'])
-		boston_data['House_Price']=load_boston()['target']
+		# boston_data=pd.DataFrame("./data/boston_dataset.csv")
+		data_url = "http://lib.stat.cmu.edu/datasets/boston"
+		raw_df = pd.read_csv(data_url, sep="\s+", skiprows=22, header=None)
+		data = np.hstack([raw_df.values[::2, :], raw_df.values[1::2, :2]])
+		target = raw_df.values[1::2, 2]
+		boston_data = pd.DataFrame(data=data,columns=['CRIM','ZN','INDUS','CHAS','NOX','RM','AGE','DIS','RAD','TAX','PTRATIO','B','LSTAT'])
+		boston_data['House_Price']=target
 		return boston_data
 
 	def __init__(self):
 		print("Datasets for Dominance Analysis")
```

### Comparing `dominance_analysis-1.1.8/dominance_analysis/dominance_old.py` & `dominance_analysis-1.1.9/dominance_analysis/dominance_old.py`

 * *Files identical despite different names*

### Comparing `dominance_analysis-1.1.8/dominance_analysis.egg-info/PKG-INFO` & `dominance_analysis-1.1.9/dominance_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominance-analysis
-Version: 1.1.8
+Version: 1.1.9
 Summary: Dominance Analysis
 Home-page: https://github.com/bhagatsajan0073/dominance_analysis
 Author: Sajan Kumar Bhagat, Kunjithapatham Sivakumar, Shashank Shekhar,Bala Koteshwar Kolluri
 Author-email: bhagat.sajan0073@gmail.com, s.vibish@gmail.com, quintshekhar@gmail.com, balakoteshwar@gmail.com
 Maintainer: Sajan Kumar Bhagat, Kunjithapatham Sivakumar, Shashank Shekhar, Bala Koteshwar Kolluri
 Maintainer-email: bhagat.sajan0073@gmail.com, s.vibish@gmail.com, quintshekhar@gmail.com, balakoteshwar@gmail.com
 License: MIT
```

### Comparing `dominance_analysis-1.1.8/setup.py` & `dominance_analysis-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dominance_analysis",
-    version="1.1.8",
+    version="1.1.9",
     author="Sajan Kumar Bhagat, Kunjithapatham Sivakumar, Shashank Shekhar,Bala Koteshwar Kolluri",
     author_email='bhagat.sajan0073@gmail.com, s.vibish@gmail.com, quintshekhar@gmail.com, balakoteshwar@gmail.com',
     maintainer="Sajan Kumar Bhagat, Kunjithapatham Sivakumar, Shashank Shekhar, Bala Koteshwar Kolluri",
     maintainer_email='bhagat.sajan0073@gmail.com, s.vibish@gmail.com, quintshekhar@gmail.com, balakoteshwar@gmail.com',
     description='Dominance Analysis',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

