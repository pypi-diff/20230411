# Comparing `tmp/rapidpredict-0.0.0.5.tar.gz` & `tmp/rapidpredict-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpredict-0.0.0.5.tar", last modified: Tue Apr 11 02:45:13 2023, max compression
+gzip compressed data, was "rapidpredict-0.0.0.6.tar", last modified: Tue Apr 11 02:51:21 2023, max compression
```

## Comparing `rapidpredict-0.0.0.5.tar` & `rapidpredict-0.0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 02:45:13.552792 rapidpredict-0.0.0.5/
--rw-rw-rw-   0        0        0     4574 2023-04-11 02:45:13.552713 rapidpredict-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 02:45:13.530576 rapidpredict-0.0.0.5/rapidpredict/
--rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.5/rapidpredict/__init__.py
--rw-rw-rw-   0        0        0    21564 2023-04-11 02:42:51.000000 rapidpredict-0.0.0.5/rapidpredict/supervised.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:45:13.551210 rapidpredict-0.0.0.5/rapidpredict.egg-info/
--rw-rw-rw-   0        0        0     4574 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 02:45:13.000000 rapidpredict-0.0.0.5/rapidpredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 02:45:13.552792 rapidpredict-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1810 2023-04-11 02:45:05.000000 rapidpredict-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:51:21.598665 rapidpredict-0.0.0.6/
+-rw-rw-rw-   0        0        0     4574 2023-04-11 02:51:21.598665 rapidpredict-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 02:51:21.587363 rapidpredict-0.0.0.6/rapidpredict/
+-rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.6/rapidpredict/__init__.py
+-rw-rw-rw-   0        0        0    20349 2023-04-11 02:51:08.000000 rapidpredict-0.0.0.6/rapidpredict/supervised.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:51:21.597661 rapidpredict-0.0.0.6/rapidpredict.egg-info/
+-rw-rw-rw-   0        0        0     4574 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:51:21.598665 rapidpredict-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1810 2023-04-11 02:51:15.000000 rapidpredict-0.0.0.6/setup.py
```

### Comparing `rapidpredict-0.0.0.5/PKG-INFO` & `rapidpredict-0.0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rapidpredict-0.0.0.5/README.md` & `rapidpredict-0.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rapidpredict-0.0.0.5/rapidpredict/supervised.py` & `rapidpredict-0.0.0.6/rapidpredict/supervised.py`

 * *Files 6% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 #         ax.set_ylabel('Model')
 
 #         ax.invert_yaxis()
 
 #         plt.show()
 
 
-class CompareModel_bargraph:
+class compareModels_bargraph:
     def __init__(self, model_names, model_accuracies):
         self.model_names = model_names.to_list()
         self.model_accuracies = model_accuracies.to_list()
         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_accuracies})
         self.plot()
 
     def plot(self):
@@ -446,62 +446,26 @@
              # Add model accuracies at the end of each bar
         for i, bar in enumerate(bars):
             width = bar.get_width()
             label = f'{width:.2f}'
             ax.text(width, bar.get_y() + bar.get_height() / 2, label, ha='left', va='center')
 
 
-        plt.show()
+        plt.show();
 
 
 
-import matplotlib.pyplot as plt
-import pandas as pd
-import numpy as np
 
-class CompareModel_boxplot:
-    def __init__(self, model_names, model_accuracies):
-        self.model_names = model_names.to_list()
-        self.model_accuracies = model_accuracies.to_list()
-        self.df = pd.DataFrame({'Model': self.model_names, self.metric_name: self.model_accuracies})
-        self.plot()
-
-    def plot(self):
-        df_sorted = self.df.sort_values(self.metric_name, ascending=True)
-
-        fig, ax = plt.subplots(figsize=(16, 8))
-
-        # Generate an array of 26 different colors using a colormap
-        colormap = plt.cm.get_cmap("tab20", 26)
-        colors = colormap(np.arange(26))
-
-        # Create a box plot
-        boxplots = ax.boxplot(df_sorted[self.metric_name], vert=False, patch_artist=True)
-
-        # Set colors for each box
-        for i, box in enumerate(boxplots['boxes']):
-            box.set_facecolor(colors[i])
-
-        ax.set_title('Model Accuracies')
-        ax.set_xlabel(self.metric_name)
-        ax.set_ylabel('Model')
-
-        ax.invert_yaxis()
-
-        # Set y-tick labels to model names
-        ax.set_yticklabels(df_sorted['Model'])
-
-        plt.show()
 
 # import matplotlib.pyplot as plt
 # import pandas as pd
 # import numpy as np
 import seaborn as sns
 
-class CompareModel_boxplot:
+class compareModels_boxplot:
     def __init__(self, model_names, model_accuracies):
         self.model_names = model_names.to_list()
         self.model_accuracies = model_accuracies.to_list()
         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_accuracies})
         self.plot()
 
     def plot(self):
@@ -519,15 +483,15 @@
         ax.set_title('Model Accuracies')
         ax.set_xlabel('F1 Score')
         ax.set_ylabel('Model')
         # ax.set_xticklabels(ax.get_yticklabels())
         ax.xaxis.set_tick_params(rotation=90)
 
 
-        plt.show()
+        plt.show();
 
 # import matplotlib.pyplot as plt
 # import pandas as pd
 # import numpy as np
 # import seaborn as sns
 
 # class CompareModel_boxplot:
```

### Comparing `rapidpredict-0.0.0.5/rapidpredict.egg-info/PKG-INFO` & `rapidpredict-0.0.0.6/rapidpredict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rapidpredict-0.0.0.5/setup.py` & `rapidpredict-0.0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.0.5'
+VERSION = '0.0.0.6'
 DESCRIPTION = 'rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.'
 LONG_DESCRIPTION = 'This repository contains a Python-based framework for rapid prediction of machine learning models\
       that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn.\
           It''s designed to provide a quick way to test various algorithms on a given dataset and compare their performance.'
 
 # Setting up
 setup(
```

