# Comparing `tmp/PyComplexHeatmap-1.4.tar.gz` & `tmp/PyComplexHeatmap-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.4.tar", last modified: Tue Apr 11 15:37:13 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.4.1.tar", last modified: Tue Apr 11 20:53:50 2023, max compression
```

## Comparing `PyComplexHeatmap-1.4.tar` & `PyComplexHeatmap-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,40 @@
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.921894 PyComplexHeatmap-1.4/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       31 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/.gitattributes
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.908264 PyComplexHeatmap-1.4/.github/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      810 2023-03-30 00:58:12.000000 PyComplexHeatmap-1.4/.github/FUNDING.yml
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       13 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/.gitignore
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1067 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/LICENSE
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      105 2023-04-11 15:37:05.000000 PyComplexHeatmap-1.4/MANIFEST.in
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11662 2023-04-11 15:37:13.921373 PyComplexHeatmap-1.4/PKG-INFO
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.917384 PyComplexHeatmap-1.4/PyComplexHeatmap/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      373 2023-04-11 15:34:50.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/__init__.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    65860 2023-04-11 02:21:02.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/annotations.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    70043 2023-04-11 02:05:07.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     5495 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/colors.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    21247 2023-04-08 14:53:33.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6766 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/example.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    17814 2023-04-10 00:47:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6753 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/tools.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    25810 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.920740 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11662 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      519 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        1 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       17 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11055 2023-04-10 19:33:30.000000 PyComplexHeatmap-1.4/README.md
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      670 2023-04-11 15:34:20.000000 PyComplexHeatmap-1.4/pyproject.toml
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       38 2023-04-11 15:37:13.921954 PyComplexHeatmap-1.4/setup.cfg
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1042 2023-04-11 15:34:30.000000 PyComplexHeatmap-1.4/setup.py
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.827531 PyComplexHeatmap-1.4.1/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       31 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/.gitattributes
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.759863 PyComplexHeatmap-1.4.1/.github/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      810 2023-03-30 00:58:12.000000 PyComplexHeatmap-1.4.1/.github/FUNDING.yml
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       13 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/.gitignore
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1067 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/LICENSE
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      105 2023-04-11 15:37:05.000000 PyComplexHeatmap-1.4.1/MANIFEST.in
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11667 2023-04-11 20:53:50.826660 PyComplexHeatmap-1.4.1/PKG-INFO
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.767924 PyComplexHeatmap-1.4.1/PyComplexHeatmap/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      375 2023-04-11 20:49:25.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    65860 2023-04-11 02:21:02.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    70631 2023-04-11 20:43:59.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     5495 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/colors.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    21247 2023-04-08 14:53:33.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6766 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/example.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    17814 2023-04-10 00:47:13.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6753 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/tools.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    25810 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.771625 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11667 2023-04-11 20:53:49.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      818 2023-04-11 20:53:50.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        1 2023-04-11 20:53:49.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       17 2023-04-11 20:53:49.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11058 2023-04-11 16:07:29.000000 PyComplexHeatmap-1.4.1/README.md
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.825889 PyComplexHeatmap-1.4.1/comparison/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    88559 2023-04-11 15:48:21.000000 PyComplexHeatmap-1.4.1/comparison/ComplexHeatmap.pdf
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   319414 2023-04-11 16:01:23.000000 PyComplexHeatmap-1.4.1/comparison/ComplexHeatmap.png
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   159732 2023-04-11 15:48:48.000000 PyComplexHeatmap-1.4.1/comparison/PyComplexHeatmap.pdf
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   666164 2023-04-11 16:01:43.000000 PyComplexHeatmap-1.4.1/comparison/PyComplexHeatmap.png
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1434 2023-04-11 16:30:23.000000 PyComplexHeatmap-1.4.1/comparison/README.md
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755) 15584021 2023-04-11 14:18:01.000000 PyComplexHeatmap-1.4.1/comparison/beta.csv
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      205 2023-04-11 15:29:17.000000 PyComplexHeatmap-1.4.1/comparison/compare.sh
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1236 2023-04-11 14:30:03.000000 PyComplexHeatmap-1.4.1/comparison/df_col.csv
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)  2909164 2023-04-11 14:21:19.000000 PyComplexHeatmap-1.4.1/comparison/df_row.csv
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     2469 2023-04-11 15:46:41.000000 PyComplexHeatmap-1.4.1/comparison/heatmap.R
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   182760 2023-04-11 20:48:31.000000 PyComplexHeatmap-1.4.1/comparison/heatmap.ipynb
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     2159 2023-04-11 15:43:20.000000 PyComplexHeatmap-1.4.1/comparison/heatmap.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      672 2023-04-11 20:49:16.000000 PyComplexHeatmap-1.4.1/pyproject.toml
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       38 2023-04-11 20:53:50.827631 PyComplexHeatmap-1.4.1/setup.cfg
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1044 2023-04-11 20:49:31.000000 PyComplexHeatmap-1.4.1/setup.py
```

### Comparing `PyComplexHeatmap-1.4/.github/FUNDING.yml` & `PyComplexHeatmap-1.4.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/LICENSE` & `PyComplexHeatmap-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PKG-INFO` & `PyComplexHeatmap-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4
+Version: 1.4.1
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -131,27 +131,27 @@
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
                 <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.1-Plot-clustermap-using-seaborn-brain-networks-dataset">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Plot-clustermap-using-seaborn-brain-networks-dataset">
                 <img src="docs/images/gallery11.png" title="Dot heatmap for correlation matrix" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
                 <img src="docs/images/gallery3.jpg" title="Combine two heatmap horizontally" align="center" width="250px">
             </a>
         </td>
     </tr>
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#4.-Annotations">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Only-plot-the-annotations">
                 <img src="docs/images/gallery5.png" title="Only plot annotations" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/clustermap.html#3.3-Top,-bottom,-left-,right-annotations">
                 <img src="docs/images/gallery6.png" title="cluster heatmap" align="center" width="250px">
             </a>
@@ -165,15 +165,15 @@
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
                 <img src="docs/images/gallery8.png" title="OncoPrint with columns split" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.2-Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
                 <img src="docs/images/gallery7.png" title="Dot clustermap to show enrichment result" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
                 <img src="docs/images/gallery4.png" title="OncoPrint with mroe annotations" align="center" width="250px">
             </a>
```

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/annotations.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/clustermap.py`

 * *Files 2% similar despite different names*

```diff
@@ -999,17 +999,20 @@
             #index=self.dendrogram_row.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.row_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.row_split, pd.Series):
                 self.row_split = self.row_split.to_frame(name=self.row_split.name)
             cols = self.row_split.columns.tolist()
             row_clusters = self.row_split.groupby(cols).apply(lambda x: x.index.tolist())
-            if self.row_split_order:
-                row_clusters=row_clusters.loc[self.row_split_order]
-            self.row_clusters=row_clusters.to_dict()
+            if self.row_split_order is None:
+                # calculate row_split_order using the mean across all samples in this group of
+                # values of mean values across all samples
+                self.row_split_order = row_clusters.apply(lambda x: self.data2d.loc[x].mean(axis=1).mean())\
+                    .sort_values(ascending=False).index.tolist()
+            self.row_clusters = row_clusters.loc[self.row_split_order].to_dict()
         elif not self.row_cluster:
             self.row_order = [self.data2d.index.tolist()]
             return None
         else:
             raise TypeError("row_split must be integar or dataframe or series")
 
         self.row_order = []
@@ -1043,17 +1046,20 @@
             #index=self.dendrogram_col.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.col_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.col_split, pd.Series):
                 self.col_split = self.col_split.to_frame(name=self.col_split.name)
             cols = self.col_split.columns.tolist()
             col_clusters = self.col_split.groupby(cols).apply(lambda x: x.index.tolist())
-            if self.col_split_order:
-                col_clusters=col_clusters.loc[self.col_split_order]
-            self.col_clusters=col_clusters.to_dict()
+            if self.col_split_order is None:
+                # calculate col_split_order using the mean across all samples in this group of
+                # values of mean values across all samples
+                self.col_split_order = col_clusters.apply(lambda x: self.data2d.loc[:,x].mean().mean())\
+                    .sort_values(ascending=False).index.tolist()
+            self.col_clusters = col_clusters.loc[self.col_split_order].to_dict()
         elif not self.col_cluster:
             self.col_order = [self.data2d.columns.tolist()]
             return None
         else:
             raise TypeError("row_split must be integar or dataframe or series")
 
         self.col_order = []
```

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/tools.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4
+Version: 1.4.1
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -131,27 +131,27 @@
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
                 <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.1-Plot-clustermap-using-seaborn-brain-networks-dataset">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Plot-clustermap-using-seaborn-brain-networks-dataset">
                 <img src="docs/images/gallery11.png" title="Dot heatmap for correlation matrix" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
                 <img src="docs/images/gallery3.jpg" title="Combine two heatmap horizontally" align="center" width="250px">
             </a>
         </td>
     </tr>
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#4.-Annotations">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Only-plot-the-annotations">
                 <img src="docs/images/gallery5.png" title="Only plot annotations" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/clustermap.html#3.3-Top,-bottom,-left-,right-annotations">
                 <img src="docs/images/gallery6.png" title="cluster heatmap" align="center" width="250px">
             </a>
@@ -165,15 +165,15 @@
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
                 <img src="docs/images/gallery8.png" title="OncoPrint with columns split" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.2-Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
                 <img src="docs/images/gallery7.png" title="Dot clustermap to show enrichment result" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
                 <img src="docs/images/gallery4.png" title="OncoPrint with mroe annotations" align="center" width="250px">
             </a>
```

### Comparing `PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/SOURCES.txt` & `PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -14,8 +14,20 @@
 PyComplexHeatmap/example.py
 PyComplexHeatmap/oncoPrint.py
 PyComplexHeatmap/tools.py
 PyComplexHeatmap/utils.py
 PyComplexHeatmap.egg-info/PKG-INFO
 PyComplexHeatmap.egg-info/SOURCES.txt
 PyComplexHeatmap.egg-info/dependency_links.txt
-PyComplexHeatmap.egg-info/top_level.txt
+PyComplexHeatmap.egg-info/top_level.txt
+comparison/ComplexHeatmap.pdf
+comparison/ComplexHeatmap.png
+comparison/PyComplexHeatmap.pdf
+comparison/PyComplexHeatmap.png
+comparison/README.md
+comparison/beta.csv
+comparison/compare.sh
+comparison/df_col.csv
+comparison/df_row.csv
+comparison/heatmap.R
+comparison/heatmap.ipynb
+comparison/heatmap.py
```

### Comparing `PyComplexHeatmap-1.4/README.md` & `PyComplexHeatmap-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,27 +115,27 @@
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
                 <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.1-Plot-clustermap-using-seaborn-brain-networks-dataset">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Plot-clustermap-using-seaborn-brain-networks-dataset">
                 <img src="docs/images/gallery11.png" title="Dot heatmap for correlation matrix" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
                 <img src="docs/images/gallery3.jpg" title="Combine two heatmap horizontally" align="center" width="250px">
             </a>
         </td>
     </tr>
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#4.-Annotations">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Only-plot-the-annotations">
                 <img src="docs/images/gallery5.png" title="Only plot annotations" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/clustermap.html#3.3-Top,-bottom,-left-,right-annotations">
                 <img src="docs/images/gallery6.png" title="cluster heatmap" align="center" width="250px">
             </a>
@@ -149,15 +149,15 @@
     <tr style="height: 500px">
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
                 <img src="docs/images/gallery8.png" title="OncoPrint with columns split" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
-            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.2-Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
                 <img src="docs/images/gallery7.png" title="Dot clustermap to show enrichment result" align="center" width="250px">
             </a>
         </td>
         <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
             <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
                 <img src="docs/images/gallery4.png" title="OncoPrint with mroe annotations" align="center" width="250px">
             </a>
```

### Comparing `PyComplexHeatmap-1.4/pyproject.toml` & `PyComplexHeatmap-1.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.4"
+version = "1.4.1"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.4/setup.py` & `PyComplexHeatmap-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.4',
+   version='1.4.1',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

