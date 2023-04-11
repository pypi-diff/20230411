# Comparing `tmp/rapidpredict-0.0.0.6.tar.gz` & `tmp/rapidpredict-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpredict-0.0.0.6.tar", last modified: Tue Apr 11 02:51:21 2023, max compression
+gzip compressed data, was "rapidpredict-0.0.0.7.tar", last modified: Tue Apr 11 03:34:33 2023, max compression
```

## Comparing `rapidpredict-0.0.0.6.tar` & `rapidpredict-0.0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 02:51:21.598665 rapidpredict-0.0.0.6/
--rw-rw-rw-   0        0        0     4574 2023-04-11 02:51:21.598665 rapidpredict-0.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 02:51:21.587363 rapidpredict-0.0.0.6/rapidpredict/
--rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.6/rapidpredict/__init__.py
--rw-rw-rw-   0        0        0    20349 2023-04-11 02:51:08.000000 rapidpredict-0.0.0.6/rapidpredict/supervised.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:51:21.597661 rapidpredict-0.0.0.6/rapidpredict.egg-info/
--rw-rw-rw-   0        0        0     4574 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 02:51:21.000000 rapidpredict-0.0.0.6/rapidpredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 02:51:21.598665 rapidpredict-0.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1810 2023-04-11 02:51:15.000000 rapidpredict-0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:34:33.977957 rapidpredict-0.0.0.7/
+-rw-rw-rw-   0        0        0     4574 2023-04-11 03:34:33.977957 rapidpredict-0.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 03:34:33.963206 rapidpredict-0.0.0.7/rapidpredict/
+-rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.7/rapidpredict/__init__.py
+-rw-rw-rw-   0        0        0    21678 2023-04-11 03:32:56.000000 rapidpredict-0.0.0.7/rapidpredict/supervised.py
+drwxrwxrwx   0        0        0        0 2023-04-11 03:34:33.975460 rapidpredict-0.0.0.7/rapidpredict.egg-info/
+-rw-rw-rw-   0        0        0     4574 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 03:34:33.977957 rapidpredict-0.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1810 2023-04-11 03:34:25.000000 rapidpredict-0.0.0.7/setup.py
```

### Comparing `rapidpredict-0.0.0.6/PKG-INFO` & `rapidpredict-0.0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rapidpredict-0.0.0.6/README.md` & `rapidpredict-0.0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rapidpredict-0.0.0.6/rapidpredict/supervised.py` & `rapidpredict-0.0.0.7/rapidpredict/supervised.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 ##                       Load Libraries!                       ##
 #################################################################
 import numpy as np
 import pandas as pd
 import datetime
 import time
 import warnings
+import matplotlib.pyplot as plt
+import pandas as pd
+import numpy as np
+import seaborn as sns
 
 from tqdm import tqdm
 from sklearn.pipeline import Pipeline
 from sklearn.impute import SimpleImputer, MissingIndicator
 from sklearn.preprocessing import StandardScaler, OneHotEncoder, OrdinalEncoder
 from sklearn.compose import ColumnTransformer
 from sklearn.utils import all_estimators
@@ -388,110 +392,147 @@
         if len(self.models.keys()) == 0:
             self.fit(X_train, X_test, y_train, y_test) 
 
         return self.models
     
 
 
-# import matplotlib.pyplot as plt
-# import pandas as pd
-
-# class CompareModel:
-#     def __init__(self, model_names, model_accuracies):
-#         self.model_names = model_names.to_list()
-#         self.model_accuracies = model_accuracies.to_list()
-#         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_accuracies})
+# class plot_target:
+#     def __init__(self, dataset, target = "target"):
+#         self.dataset = dataset
+#         self.target = target
 #         self.plot()
 
-    
 #     def plot(self):
-#         df_sorted = self.df.sort_values('F1 Score', ascending=True)
+#         # Create a DataFrame containing the target column
+#         target_df = pd.DataFrame({self.target: self.dataset})
+#         fig, ax = plt.subplots(figsize=(4, 8))
+#         ax = sns.countplot(x=self.target, data=target_df)
+#         ax.set_title("Target Distribution")
+#         ax.set_xlabel("Target")
+#         ax.set_ylabel("Count")
+#         plt.show()
+
+#     def __repr__(self):
+#         return ''
+
+
+class plot_target:
+    def __init__(self, dataset, target="target"):
+        self.dataset = dataset
+        self.target = target
+        self.plot()
+
+    def plot(self):
+        # Create a DataFrame containing the target column
+        target_df = pd.DataFrame({self.target: self.dataset})
+        counts = target_df[self.target].value_counts()
+
+        # Create a subplot with 1 row and 2 columns
+        fig, ax = plt.subplots(1, 2, figsize=(10, 4))
+
+        # Create the countplot in the first subplot
+        sns.countplot(x=self.target, data=target_df, ax=ax[0])
+        ax[0].set_title("Target Distribution (Countplot)")
+        ax[0].set_xlabel("Target")
+        ax[0].set_ylabel("Count")
+
+        # Create the pie chart in the second subplot
+        ax[1].pie(counts, labels=counts.index, autopct='%1.1f%%', startangle=90)
+        ax[1].set_title("Target Distribution (Pie Chart)")
+        ax[1].axis('equal')  # Equal aspect ratio ensures the pie chart is circular
+
+        plt.show()
+
+    def __repr__(self):
+        return ''
+    
 
-#         fig, ax = plt.subplots(figsize=(16, 8))
 
-#         ax.barh(df_sorted['F1 Score'] , df_sorted['Model'])
 
-#         ax.set_title('Model Accuracies')
-#         ax.set_xlabel('F1 Score')
-#         ax.set_ylabel('Model')
 
-#         ax.invert_yaxis()
 
-#         plt.show()
 
 
 class compareModels_bargraph:
-    def __init__(self, model_names, model_accuracies):
+    def __init__(self, model_names, model_metrics_flscore):
         self.model_names = model_names.to_list()
-        self.model_accuracies = model_accuracies.to_list()
-        self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_accuracies})
+        self.model_metrics_flscore = model_metrics_flscore.to_list()
+        self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_metrics_flscore})
         self.plot()
 
     def plot(self):
         df_sorted = self.df.sort_values('F1 Score', ascending=True)
 
         fig, ax = plt.subplots(figsize=(16, 8))
 
         # Generate an array of 26 different colors using a colormap
         colormap = plt.cm.get_cmap("tab20", 26)
         colors = colormap(np.arange(26))
 
         # Pass the colors array to the barh function
         bars = ax.barh(df_sorted['F1 Score'], df_sorted['Model'], color=colors)
 
-        ax.set_title('Model Accuracies')
+        ax.set_title('Model F1 Score')
         ax.set_xlabel('F1 Score')
         ax.set_ylabel('Model')
 
         ax.invert_yaxis()
              # Add model accuracies at the end of each bar
         for i, bar in enumerate(bars):
             width = bar.get_width()
             label = f'{width:.2f}'
             ax.text(width, bar.get_y() + bar.get_height() / 2, label, ha='left', va='center')
 
 
-        plt.show();
+        plt.show()
+        def __repr__(self):
+        # Return an empty string or a custom message
+            return ''
 
 
 
 
 
-# import matplotlib.pyplot as plt
-# import pandas as pd
-# import numpy as np
-import seaborn as sns
 
 class compareModels_boxplot:
-    def __init__(self, model_names, model_accuracies):
+    def __init__(self, model_names, model_metrics_flscore):
         self.model_names = model_names.to_list()
-        self.model_accuracies = model_accuracies.to_list()
-        self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_accuracies})
+        self.model_metrics_flscore = model_metrics_flscore.to_list()
+        self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_metrics_flscore})
         self.plot()
 
     def plot(self):
         df_sorted = self.df.sort_values('F1 Score', ascending=True)
 
         fig, ax =plt.subplots(figsize=(10, 4)) 
 
         # Generate an array of 26 different colors using a colormap
         colormap = plt.cm.get_cmap("tab20", 26)
         colors = colormap(np.arange(26))
 
         # Create a custom boxplot with seaborn
         sns.boxplot(x='F1 Score', y='Model', data=df_sorted, palette=colors[:len(self.model_names)], ax=ax )
 
-        ax.set_title('Model Accuracies')
+        ax.set_title('Model F1 Scores')
         ax.set_xlabel('F1 Score')
         ax.set_ylabel('Model')
-        # ax.set_xticklabels(ax.get_yticklabels())
         ax.xaxis.set_tick_params(rotation=90)
 
+        #     # Add model accuracies close to the model names
+        # for i, row in df_sorted.iterrows():
+        #     ax.text(row['F1 Score'] + 0.005, i, f"{row['F1 Score']:.3f}", va='center')
+
+
+        plt.show()
+        def __repr__(self):
+        # Return an empty string or a custom message
+            return ''
+
 
-        plt.show();
 
 # import matplotlib.pyplot as plt
 # import pandas as pd
 # import numpy as np
 # import seaborn as sns
 
 # class CompareModel_boxplot:
```

### Comparing `rapidpredict-0.0.0.6/rapidpredict.egg-info/PKG-INFO` & `rapidpredict-0.0.0.7/rapidpredict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rapidpredict-0.0.0.6/setup.py` & `rapidpredict-0.0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.0.6'
+VERSION = '0.0.0.7'
 DESCRIPTION = 'rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.'
 LONG_DESCRIPTION = 'This repository contains a Python-based framework for rapid prediction of machine learning models\
       that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn.\
           It''s designed to provide a quick way to test various algorithms on a given dataset and compare their performance.'
 
 # Setting up
 setup(
```

