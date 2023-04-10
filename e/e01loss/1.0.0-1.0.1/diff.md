# Comparing `tmp/e01loss-1.0.0.tar.gz` & `tmp/e01loss-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e01loss-1.0.0.tar", last modified: Mon Apr 10 21:44:36 2023, max compression
+gzip compressed data, was "e01loss-1.0.1.tar", last modified: Mon Apr 10 22:18:01 2023, max compression
```

## Comparing `e01loss-1.0.0.tar` & `e01loss-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:44:36.658772 e01loss-1.0.0/
--rw-rw-rw-   0        0        0     1988 2023-04-10 19:13:27.000000 e01loss-1.0.0/CITATION.cff
--rw-rw-rw-   0        0        0    35821 2023-04-10 17:54:01.000000 e01loss-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       97 2023-04-10 20:43:31.000000 e01loss-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8321 2023-04-10 21:44:36.657771 e01loss-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7982 2023-04-10 21:28:32.000000 e01loss-1.0.0/README.md
--rw-rw-rw-   0        0        0    29972 2023-04-06 11:24:29.000000 e01loss-1.0.0/complexity_analysis.png
-drwxrwxrwx   0        0        0        0 2023-04-10 21:44:36.644768 e01loss-1.0.0/e01loss/
--rw-rw-rw-   0        0        0        0 2023-04-10 09:41:36.000000 e01loss-1.0.0/e01loss/__init__.py
--rw-rw-rw-   0        0        0     2791 2023-04-10 19:08:17.000000 e01loss-1.0.0/e01loss/auxfuncs.py
--rw-rw-rw-   0        0        0     6265 2023-04-10 18:30:52.000000 e01loss-1.0.0/e01loss/classifylinear.py
--rw-rw-rw-   0        0        0    11239 2023-04-10 19:05:53.000000 e01loss-1.0.0/e01loss/exact_classify01loss.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:44:36.656770 e01loss-1.0.0/e01loss/test/
--rw-rw-rw-   0        0        0        0 2023-04-10 09:47:00.000000 e01loss-1.0.0/e01loss/test/__init__.py
--rw-rw-rw-   0        0        0      766 2023-04-10 18:32:31.000000 e01loss-1.0.0/e01loss/test/test_classify01loss_data.py
--rw-rw-rw-   0        0        0     1901 2023-04-10 19:21:51.000000 e01loss-1.0.0/e01loss/test/test_classify01loss_synth.py
--rw-rw-rw-   0        0        0    14648 2023-04-10 16:32:33.000000 e01loss-1.0.0/e01loss/test/voicepath_data.csv
-drwxrwxrwx   0        0        0        0 2023-04-10 21:44:36.651769 e01loss-1.0.0/e01loss.egg-info/
--rw-rw-rw-   0        0        0     8321 2023-04-10 21:44:36.000000 e01loss-1.0.0/e01loss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-04-10 21:44:36.000000 e01loss-1.0.0/e01loss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 21:44:36.000000 e01loss-1.0.0/e01loss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 21:44:36.000000 e01loss-1.0.0/e01loss.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-10 21:44:36.000000 e01loss-1.0.0/e01loss.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:44:36.658772 e01loss-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-04-10 21:44:30.000000 e01loss-1.0.0/setup.py
--rw-rw-rw-   0        0        0   179223 2023-04-06 11:41:53.000000 e01loss-1.0.0/voicepath.png
+drwxrwxrwx   0        0        0        0 2023-04-10 22:18:01.347090 e01loss-1.0.1/
+-rw-rw-rw-   0        0        0      445 2023-04-10 22:11:00.000000 e01loss-1.0.1/CITATION.cff
+-rw-rw-rw-   0        0        0    35821 2023-04-10 22:11:00.000000 e01loss-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       97 2023-04-10 22:11:00.000000 e01loss-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8309 2023-04-10 22:18:01.347090 e01loss-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7982 2023-04-10 22:11:00.000000 e01loss-1.0.1/README.md
+-rw-rw-rw-   0        0        0    29972 2023-04-10 22:11:00.000000 e01loss-1.0.1/complexity_analysis.png
+drwxrwxrwx   0        0        0        0 2023-04-10 22:18:01.333085 e01loss-1.0.1/e01loss/
+-rw-rw-rw-   0        0        0        0 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/__init__.py
+-rw-rw-rw-   0        0        0     2791 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/auxfuncs.py
+-rw-rw-rw-   0        0        0     6265 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/classifylinear.py
+-rw-rw-rw-   0        0        0    11239 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/exact_classify01loss.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:18:01.345088 e01loss-1.0.1/e01loss/test/
+-rw-rw-rw-   0        0        0        0 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/test/__init__.py
+-rw-rw-rw-   0        0        0      766 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/test/test_classify01loss_data.py
+-rw-rw-rw-   0        0        0     1901 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/test/test_classify01loss_synth.py
+-rw-rw-rw-   0        0        0    14648 2023-04-10 22:11:00.000000 e01loss-1.0.1/e01loss/test/voicepath_data.csv
+drwxrwxrwx   0        0        0        0 2023-04-10 22:18:01.340087 e01loss-1.0.1/e01loss.egg-info/
+-rw-rw-rw-   0        0        0     8309 2023-04-10 22:18:01.000000 e01loss-1.0.1/e01loss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-04-10 22:18:01.000000 e01loss-1.0.1/e01loss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:18:01.000000 e01loss-1.0.1/e01loss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:18:01.000000 e01loss-1.0.1/e01loss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 22:18:01.000000 e01loss-1.0.1/e01loss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:18:01.347090 e01loss-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-04-10 22:11:00.000000 e01loss-1.0.1/setup.py
+-rw-rw-rw-   0        0        0   179223 2023-04-10 22:11:00.000000 e01loss-1.0.1/voicepath.png
```

### Comparing `e01loss-1.0.0/LICENSE` & `e01loss-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/PKG-INFO` & `e01loss-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: e01loss
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for solving the exact 0-1 loss linear classification problem
-Home-page: https://github.com/XiHegrt/Exact-ML-Algorithms
+Home-page: https://github.com/XiHegrt/E01Loss
 Author: Xi He
 Author-email: xihegrt@gmail.com
-License: MIT License
+License: GNU GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # E01Loss: A Python library for solving the exact 0-1 loss linear classification problem
 
 Algorithms for solving the **linear classification problem** [1] have a long history, dating back at least to 1936 with Ronald Fisher's *discriminant analysis*. For linearly separable data, many algorithms can obtain the exact solution to the corresponding *0-1 loss classification* problem efficiently, but for data which is not linearly separable, it has been shown that this problem, in full generality, is NP-hard [2]. Alternative approaches all involve approximations of some kind, including the use of *surrogates* for the 0-1 loss (for example, the *hinge* or *logistic loss*) or approximate combinatorial search, none of which can be guaranteed to solve the problem exactly. Finding efficient algorithms to obtain an *exact* i.e. *globally optimal* solution for the 0-1 loss linear classification problem with fixed dimension $D$, is a long-standing problem. The E01Loss library provides Python implementations of several novel polynomial-time algorithms (currently: incremental combinatorial generation, incremental combinatorial purging, cell enumeration) which are provably correct and practical for small to medium-sized problems.
```

### Comparing `e01loss-1.0.0/README.md` & `e01loss-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/complexity_analysis.png` & `e01loss-1.0.1/complexity_analysis.png`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/e01loss/auxfuncs.py` & `e01loss-1.0.1/e01loss/auxfuncs.py`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/e01loss/classifylinear.py` & `e01loss-1.0.1/e01loss/classifylinear.py`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/e01loss/exact_classify01loss.py` & `e01loss-1.0.1/e01loss/exact_classify01loss.py`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/e01loss/test/test_classify01loss_data.py` & `e01loss-1.0.1/e01loss/test/test_classify01loss_data.py`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/e01loss/test/test_classify01loss_synth.py` & `e01loss-1.0.1/e01loss/test/test_classify01loss_synth.py`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/e01loss/test/voicepath_data.csv` & `e01loss-1.0.1/e01loss/test/voicepath_data.csv`

 * *Files identical despite different names*

### Comparing `e01loss-1.0.0/e01loss.egg-info/PKG-INFO` & `e01loss-1.0.1/e01loss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: e01loss
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for solving the exact 0-1 loss linear classification problem
-Home-page: https://github.com/XiHegrt/Exact-ML-Algorithms
+Home-page: https://github.com/XiHegrt/E01Loss
 Author: Xi He
 Author-email: xihegrt@gmail.com
-License: MIT License
+License: GNU GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # E01Loss: A Python library for solving the exact 0-1 loss linear classification problem
 
 Algorithms for solving the **linear classification problem** [1] have a long history, dating back at least to 1936 with Ronald Fisher's *discriminant analysis*. For linearly separable data, many algorithms can obtain the exact solution to the corresponding *0-1 loss classification* problem efficiently, but for data which is not linearly separable, it has been shown that this problem, in full generality, is NP-hard [2]. Alternative approaches all involve approximations of some kind, including the use of *surrogates* for the 0-1 loss (for example, the *hinge* or *logistic loss*) or approximate combinatorial search, none of which can be guaranteed to solve the problem exactly. Finding efficient algorithms to obtain an *exact* i.e. *globally optimal* solution for the 0-1 loss linear classification problem with fixed dimension $D$, is a long-standing problem. The E01Loss library provides Python implementations of several novel polynomial-time algorithms (currently: incremental combinatorial generation, incremental combinatorial purging, cell enumeration) which are provably correct and practical for small to medium-sized problems.
```

### Comparing `e01loss-1.0.0/setup.py` & `e01loss-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name='e01loss',
-    version='1.0.0',
+    version='1.0.1',
     description='A Python library for solving the exact 0-1 loss linear classification problem',
-    url='https://github.com/XiHegrt/Exact-ML-Algorithms',
+    url='https://github.com/XiHegrt/E01Loss',
     author='Xi He',
     author_email='xihegrt@gmail.com',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    license='MIT License',
+    license='GNU GPL-3.0',
     packages=['e01loss','e01loss.test'],
     include_package_data=True,
     package_data={'e01loss': ['test/*.csv']},
     install_requires=['numpy','cvxopt'],
-)
+)
```

### Comparing `e01loss-1.0.0/voicepath.png` & `e01loss-1.0.1/voicepath.png`

 * *Files identical despite different names*

