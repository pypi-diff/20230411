# Comparing `tmp/PyComplexHeatmap-1.3.9.tar.gz` & `tmp/PyComplexHeatmap-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.3.9.tar", last modified: Sun Apr  9 03:54:05 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.4.tar", last modified: Tue Apr 11 15:37:13 2023, max compression
```

## Comparing `PyComplexHeatmap-1.3.9.tar` & `PyComplexHeatmap-1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.699920 PyComplexHeatmap-1.3.9/
--rw-r--r--   0 dingw1   (1300322987) 1768498755       31 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/.gitattributes
-drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.676953 PyComplexHeatmap-1.3.9/.github/
--rw-r--r--   0 dingw1   (1300322987) 1768498755      810 2023-03-30 00:58:12.000000 PyComplexHeatmap-1.3.9/.github/FUNDING.yml
--rw-r--r--   0 dingw1   (1300322987) 1768498755       13 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/.gitignore
--rw-r--r--   0 dingw1   (1300322987) 1768498755     1067 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/LICENSE
--rw-r--r--   0 dingw1   (1300322987) 1768498755       89 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/MANIFEST.in
--rw-r--r--   0 dingw1   (1300322987) 1768498755     7981 2023-04-09 03:54:05.699393 PyComplexHeatmap-1.3.9/PKG-INFO
-drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.688483 PyComplexHeatmap-1.3.9/PyComplexHeatmap/
--rw-r--r--   0 dingw1   (1300322987) 1768498755      375 2023-04-09 03:51:12.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/__init__.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755    65705 2023-04-08 23:51:07.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/annotations.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755    70043 2023-04-09 02:17:50.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755     5495 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/colors.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755    21247 2023-04-08 14:53:33.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755     6766 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/example.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755    17624 2023-04-09 03:11:44.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755     6753 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/tools.py
--rw-r--r--   0 dingw1   (1300322987) 1768498755    25810 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.698369 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/
--rw-r--r--   0 dingw1   (1300322987) 1768498755     7981 2023-04-09 03:54:04.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 dingw1   (1300322987) 1768498755      519 2023-04-09 03:54:05.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 dingw1   (1300322987) 1768498755        1 2023-04-09 03:54:04.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 dingw1   (1300322987) 1768498755       17 2023-04-09 03:54:04.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 dingw1   (1300322987) 1768498755     7372 2023-04-09 03:50:27.000000 PyComplexHeatmap-1.3.9/README.md
--rw-r--r--   0 dingw1   (1300322987) 1768498755      672 2023-04-09 03:51:24.000000 PyComplexHeatmap-1.3.9/pyproject.toml
--rw-r--r--   0 dingw1   (1300322987) 1768498755       38 2023-04-09 03:54:05.700000 PyComplexHeatmap-1.3.9/setup.cfg
--rw-r--r--   0 dingw1   (1300322987) 1768498755     1044 2023-04-09 03:51:35.000000 PyComplexHeatmap-1.3.9/setup.py
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.921894 PyComplexHeatmap-1.4/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       31 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/.gitattributes
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.908264 PyComplexHeatmap-1.4/.github/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      810 2023-03-30 00:58:12.000000 PyComplexHeatmap-1.4/.github/FUNDING.yml
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       13 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/.gitignore
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1067 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/LICENSE
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      105 2023-04-11 15:37:05.000000 PyComplexHeatmap-1.4/MANIFEST.in
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11662 2023-04-11 15:37:13.921373 PyComplexHeatmap-1.4/PKG-INFO
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.917384 PyComplexHeatmap-1.4/PyComplexHeatmap/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      373 2023-04-11 15:34:50.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    65860 2023-04-11 02:21:02.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    70043 2023-04-11 02:05:07.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     5495 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/colors.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    21247 2023-04-08 14:53:33.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6766 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/example.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    17814 2023-04-10 00:47:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6753 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/tools.py
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    25810 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 15:37:13.920740 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11662 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      519 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        1 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       17 2023-04-11 15:37:13.000000 PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11055 2023-04-10 19:33:30.000000 PyComplexHeatmap-1.4/README.md
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      670 2023-04-11 15:34:20.000000 PyComplexHeatmap-1.4/pyproject.toml
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       38 2023-04-11 15:37:13.921954 PyComplexHeatmap-1.4/setup.cfg
+-rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1042 2023-04-11 15:34:30.000000 PyComplexHeatmap-1.4/setup.py
```

### Comparing `PyComplexHeatmap-1.3.9/.github/FUNDING.yml` & `PyComplexHeatmap-1.4/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/LICENSE` & `PyComplexHeatmap-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/PKG-INFO` & `PyComplexHeatmap-1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.3.9
+Version: 1.4
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -64,15 +64,15 @@
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
 ## **Usage**
 ----------------------
-### **1. Simple Guide To Get started.**
+### **1. [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html).**
 ```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
 df['CD'] = ['C'] * 3 + ['D'] * 3 + ['G'] * 4
 df['EF'] = ['E'] * 6 + ['F'] * 2 + ['H'] * 2
@@ -89,23 +89,25 @@
 df_heatmap.iloc[1, 2] = np.nan
 
 #Annotate the rows with sample4 > 0.5
 df_rows = df_heatmap.apply(lambda x:x.name if x.sample4 > 0.5 else None,axis=1)
 df_rows=df_rows.to_frame(name='Selected')
 df_rows['XY']=df_rows.index.to_series().apply(lambda x:'A' if int(x.replace('Fea',''))>=15 else 'B')
 
+#Create row annotations
 row_ha = HeatmapAnnotation(
                            Scatter=anno_scatterplot(df_heatmap.sample4.apply(lambda x:round(x,2)),
                                             height=12,cmap='jet',legend=False),
                            Bar=anno_barplot(df_heatmap.sample4.apply(lambda x:round(x,2)),
                                             height=16,cmap='rainbow',legend=False),
                            selected=anno_label(df_rows,colors='red',relpos=(-0.05,0.4)),
                            label_kws={'rotation':30,'horizontalalignment':'left','verticalalignment':'bottom'},
                             axis=0,verbose=0)
 
+#Create column annotations
 col_ha = HeatmapAnnotation(label=anno_label(df.AB, merge=True,rotation=10),
                            AB=anno_simple(df.AB,add_text=True),axis=1,
                            CD=anno_simple(df.CD,add_text=True),
                            EF=anno_simple(df.EF,add_text=True,
                                             legend_kws={'frameon':True}),
                            G=anno_boxplot(df_box, cmap='jet',legend=False),
                            verbose=0)
@@ -119,50 +121,86 @@
                        show_rownames=False,show_colnames=True,
                        tree_kws={'row_cmap': 'Set1'},verbose=0,legend_gap=5,
                        cmap='RdYlBu_r',xticklabels_kws={'labelrotation':-45,'labelcolor':'blue'})
 #plt.savefig("example0.pdf", bbox_inches='tight')
 plt.show()
 ```
 ### Example output
-<p align="center"> 
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
-<img src="docs/images/1.jpg" width=700 align="center">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/clustermap.html#3.3-Top,-bottom,-left-,right-annotations">
-<img src="docs/images/2.png" width=600 align="middle">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Change-orentation-to-the-right">
-<img src="docs/images/3.png" width=700 align="middle">
-</a>
-</p>
-<!-- ![image](docs/images/4.png) -->
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/cpg_modules.html#Plotting-the-Dot-clustermap">
-<img src="docs/images/4.png" width=600 align="middle">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
-<img src="docs/images/5.jpg" width=500 align="middle">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
-<img src="docs/images/6.png" width=600 align="middle">
-</a>
-</p>
+Click picture to view the source code
+
+<table>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
+                <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.1-Plot-clustermap-using-seaborn-brain-networks-dataset">
+                <img src="docs/images/gallery11.png" title="Dot heatmap for correlation matrix" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
+                <img src="docs/images/gallery3.jpg" title="Combine two heatmap horizontally" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#4.-Annotations">
+                <img src="docs/images/gallery5.png" title="Only plot annotations" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/clustermap.html#3.3-Top,-bottom,-left-,right-annotations">
+                <img src="docs/images/gallery6.png" title="cluster heatmap" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/single_cell_methylation.html">
+                <img src="docs/images/gallery9.png" title="DNA methylation cell type specific signatures" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
+                <img src="docs/images/gallery8.png" title="OncoPrint with columns split" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.2-Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
+                <img src="docs/images/gallery7.png" title="Dot clustermap to show enrichment result" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
+                <img src="docs/images/gallery4.png" title="OncoPrint with mroe annotations" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/cpg_modules.html#Plotting-the-Dot-clustermap">
+                <img src="docs/images/gallery2.png" title="Dot clustermap with annotations" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Changing-the-size-of-point">
+                <img src="docs/images/gallery10.png" title="Dot heatmap using different dot size" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Change-orentation-to-the-left">
+                <img src="docs/images/gallery12.png" title="Plot only the annotation with different orientations" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+</table>
 
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
 
 ## Call for Contributions
 ----------------------
```

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
         width and other arguments passed to plt.boxplot.
 
     Parameters
     ----------
     """
 
     def _height(self, height):
-        return 8 if height is None else height
+        return 10 if height is None else height
 
     def _set_default_plot_kws(self, plot_kws):
         self.plot_kws = plot_kws if plot_kws is not None else {}
         self.plot_kws.setdefault('showfliers', False)
         self.plot_kws.setdefault('edgecolor', 'black')
         self.plot_kws.setdefault('medianlinecolor', 'black')
         self.plot_kws.setdefault('grid', True)
@@ -920,15 +920,15 @@
     Class HeatmapAnnotation.
 
     """
 
     def __init__(self, df=None, axis=1, cmap='auto', colors=None, label_side=None, label_kws=None,
                  ticklabels_kws=None, plot_kws=None, plot=False, legend=True, legend_side='right',
                  legend_gap=5, legend_width=4.5, legend_hpad=2, legend_vpad=5, orientation=None,
-                 wspace=0, hspace=0,
+                 wgap=0.1,hgap=0.1,
                  plot_legend=True, rasterized=False, verbose=1, **args):
         if df is None and len(args) == 0:
             raise ValueError("Please specify either df or other args")
         if not df is None and len(args) > 0:
             raise ValueError("df and Name-value pairs can only be given one, not both.")
         if not df is None:
             self._check_df(df)
@@ -938,14 +938,16 @@
         self.verbose = verbose
         self.label_side = label_side
         self.plot_kws = plot_kws if not plot_kws is None else {}
         self.args = args
         self._check_legend(legend)
         self.legend_side = legend_side
         self.legend_gap = legend_gap
+        self.wgap=wgap
+        self.hgap = hgap
         self.legend_width = legend_width
         self.legend_hpad = legend_hpad
         self.legend_vpad = legend_vpad
         self.plot_legend = plot_legend
         self.rasterized = rasterized
         self.orientation = orientation
         self.plot = plot
@@ -956,15 +958,15 @@
         else:
             self._check_colors(colors)
         self._process_data()
         self._heights()
         self._nrows()
         self.label_kws,self.ticklabels_kws = label_kws, ticklabels_kws
         if self.plot:
-            self.plot_annotations(wspace=wspace, hspace=hspace)
+            self.plot_annotations()
 
     def _check_df(self, df):
         if type(df) == list or isinstance(df, np.ndarray):
             df = pd.Series(df).to_frame(name='df')
         elif isinstance(df, pd.Series):
             name = df.name if not df.name is None else 'df'
             df = df.to_frame(name=name)
@@ -1218,29 +1220,27 @@
                 legend_kws.setdefault('vmax', round(vmax, 2))
                 self.legend_list.append([annotation.cmap, annotation.label, legend_kws, 4,'cmap'])
         if len(self.legend_list) > 1:
             self.legend_list = sorted(self.legend_list, key=lambda x: x[3])
         self.label_max_width = max([ann.get_max_label_width() for ann in self.annotations])
         # self.label_max_height = max([ann.ax.yaxis.label.get_window_extent().height for ann in self.annotations])
 
-    def plot_annotations(self, ax=None, subplot_spec=None, idxs=None, gap=0.5,
+    def plot_annotations(self, ax=None, subplot_spec=None, idxs=None,
                          wspace=None, hspace=None):
         """
         Plot annotations
 
         Parameters
         ----------
         ax : ax
             axes to plot the annotations.
         subplot_spec : ax.figure.add_gridspec
             object from ax.figure.add_gridspec or matplotlib.gridspec.GridSpecFromSubplotSpec.
         idxs : list
             index to reorder df and df of annotation class.
-        gap : float
-            gap to calculate wspace and hspace for gridspec.
         wspace : float
             if wspace not is None, use wspace, else wspace would be calculated based on gap.
         hspace : float
             if hspace not is None, use hspace, else hspace would be calculated based on gap.
 
         Returns
         -------
@@ -1257,25 +1257,27 @@
         if idxs is None:
             idxs = [self.annotations[0].plot_data.index.tolist()]
         if self.axis == 1:
             nrows = len(self.heights)
             ncols = len(idxs)
             height_ratios = self.heights
             width_ratios = [len(idx) for idx in idxs]
-            wspace = gap * mm2inch * self.ax.figure.dpi / (
+            wspace = self.wgap * mm2inch * self.ax.figure.dpi / (
                     self.ax.get_window_extent().width / ncols) if wspace is None else wspace  # 1mm=mm2inch inch
-            hspace = 0 if hspace is None else hspace  # fraction of height
+            hspace = self.hgap * mm2inch * self.ax.figure.dpi / (
+                    self.ax.get_window_extent().height / nrows) if hspace is None else hspace  # fraction of height
         else:
             nrows = len(idxs)
             ncols = len(self.heights)
             width_ratios = self.heights
             height_ratios = [len(idx) for idx in idxs]
-            hspace = gap * mm2inch * self.ax.figure.dpi / (
+            hspace = self.hgap * mm2inch * self.ax.figure.dpi / (
                     self.ax.get_window_extent().height / nrows) if hspace is None else hspace
-            wspace = 0 if wspace is None else wspace  # The amount of width reserved for space between subplots, expressed as a fraction of the average axis width
+            wspace = self.wgap * mm2inch * self.ax.figure.dpi / (
+                    self.ax.get_window_extent().width / ncols) if wspace is None else wspace  # The amount of width reserved for space between subplots, expressed as a fraction of the average axis width
         if subplot_spec is None:
             self.gs = self.ax.figure.add_gridspec(nrows, ncols, hspace=hspace, wspace=wspace,
                                                   height_ratios=height_ratios,
                                                   width_ratios=width_ratios)
         else: #this ax is a subplot of another bigger figure.
             self.gs = matplotlib.gridspec.GridSpecFromSubplotSpec(nrows, ncols, hspace=hspace, wspace=wspace,
                                                                   subplot_spec=subplot_spec,
```

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/clustermap.py`

 * *Files 0% similar despite different names*

```diff
@@ -691,15 +691,15 @@
                  top_annotation=None, bottom_annotation=None, left_annotation=None, right_annotation=None,
                  row_cluster=True, col_cluster=True, row_cluster_method='average', row_cluster_metric='correlation',
                  col_cluster_method='average', col_cluster_metric='correlation',
                  show_rownames=False, show_colnames=False, row_names_side='right', col_names_side='bottom',
                  row_dendrogram=False, col_dendrogram=False, row_dendrogram_size=10, col_dendrogram_size=10,
                  row_split=None, col_split=None, dendrogram_kws=None, tree_kws=None,
                  row_split_order=None, col_split_order=None, row_split_gap=0.5, col_split_gap=0.2, mask=None,
-                 subplot_gap=3, legend=True, legend_kws=None, plot=True, plot_legend=True,
+                 subplot_gap=1, legend=True, legend_kws=None, plot=True, plot_legend=True,
                  legend_anchor='auto', legend_gap=5, legend_width=4.5, legend_hpad=2, legend_vpad=5,
                  legend_side='right', cmap='jet', label=None, xticklabels_kws=None, yticklabels_kws=None,
                  rasterized=False, legend_delta_x=None, verbose=1, **kwargs):
         self.kwargs = kwargs if not kwargs is None else {}
         self.data2d = self.format_data(data, mask, z_score, standard_scale)
         self.verbose=verbose
         self._define_kws(xticklabels_kws, yticklabels_kws)
```

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/oncoPrint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 # !/usr/bin/env python3
 import os, sys
 import pandas as pd
 import numpy as np
+from scipy.cluster import hierarchy
 import matplotlib
 import matplotlib.pylab as plt
 from .utils import _draw_figure,mm2inch,plot_legend_list,despine,_index_to_ticklabels
 from .clustermap import ClusterMapPlotter
 from .annotations import HeatmapAnnotation, anno_barplot
 from matplotlib.ticker import MultipleLocator, FormatStrFormatter
 # =============================================================================
@@ -196,15 +197,15 @@
                                                              criterion='maxclust'),
                                           index=self.data2d.index.tolist()).to_frame(name='cluster')\
                 .groupby('cluster').apply(lambda x: x.index.tolist()).to_dict()
             #index=self.dendrogram_row.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.row_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.row_split, pd.Series):
-                self.row_split = self.row_split.to_frame(name=self.row_split.name)
+                self.row_split = self.row_split.to_frame(name=self.row_split.name).loc[self.data2d.index.tolist()]
             cols = self.row_split.columns.tolist()
             row_clusters = self.row_split.groupby(cols).apply(lambda x: x.index.tolist())
             if self.row_split_order:
                 row_clusters=row_clusters.loc[self.row_split_order]
             self.row_clusters=row_clusters.to_dict()
         elif not self.row_cluster:
             self.row_order = [self.data2d.index.tolist()]
@@ -217,42 +218,49 @@
         for i, cluster in enumerate(self.row_clusters):
             rows = self.row_clusters[cluster]
             if len(rows) <= 1:
                 self.row_order.append(rows)
                 self.dendrogram_rows.append(None)
                 continue
             if self.row_cluster:
-                self.calculate_row_dendrograms(self.data2d.loc[rows])
-                self.dendrogram_rows.append(self.dendrogram_row)
-                self.row_order.append(self.dendrogram_row.dendrogram['ivl'])
+                row_order=self.row_vc.loc[rows].sum(axis=1).sort_values(ascending=False).index.tolist()
+                self.row_order.append(row_order)
             else:
                 self.row_order.append(rows)
 
+    def get_samples_order(self,data,row_order):
+        """
+        data is a dataframe, row_order is a list ([[],[]]).
+        """
+        nrows = data.shape[0]
+        row_orders = list(np.array(row_order).flatten())
+        # https://gist.github.com/armish/564a65ab874a770e2c26
+        col_order = data.apply(
+            lambda x: x.apply(lambda y: 0 if np.sum(y) == 0 else 2 ** (nrows - row_orders.index(x.name) - 1)), axis=1) \
+            .sum().sort_values(ascending=False).index.tolist()
+        return col_order
+
     def _reorder_cols(self):
         if self.verbose >= 1:
             print("Reordering cols..")
         if self.col_split is None and self.col_cluster:
-            nrows=self.data2d.shape[0]
-            row_orders=list(np.array(self.row_order).flatten())
-            #https://gist.github.com/armish/564a65ab874a770e2c26
-            col_order=self.data2d.apply(lambda x:x.apply(lambda y:0 if np.sum(y)==0 else 2**(nrows-row_orders.index(x.name)-1)),axis=1)\
-                .sum().sort_values(ascending=False).index.tolist()
+            col_order=self.get_samples_order(self.data2d,self.row_order)
             self.col_order = [col_order]  # self.data2d.iloc[:, xind].columns.tolist()
             return None
         elif isinstance(self.col_split, int) and self.col_cluster:
             self.calculate_col_dendrograms(self.data2d.applymap(lambda x:np.sum(x)))
             self.col_clusters = pd.Series(hierarchy.fcluster(self.dendrogram_col.linkage, t=self.col_split,
                                                              criterion='maxclust'),
                                           index=self.data2d.columns.tolist()).to_frame(name='cluster')\
                 .groupby('cluster').apply(lambda x: x.index.tolist()).to_dict()
             #index=self.dendrogram_col.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.col_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.col_split, pd.Series):
-                self.col_split = self.col_split.to_frame(name=self.col_split.name)
+                self.col_split = self.col_split.to_frame(name=self.col_split.name).loc[self.data2d.columns.tolist()]
             cols = self.col_split.columns.tolist()
             col_clusters = self.col_split.groupby(cols).apply(lambda x: x.index.tolist())
             if self.col_split_order:
                 col_clusters=col_clusters.loc[self.col_split_order]
             self.col_clusters=col_clusters.to_dict()
         elif not self.col_cluster:
             self.col_order = [self.data2d.columns.tolist()]
@@ -265,17 +273,16 @@
         for i, cluster in enumerate(self.col_clusters):
             cols = self.col_clusters[cluster]
             if len(cols) <= 1:
                 self.col_order.append(cols)
                 self.dendrogram_cols.append(None)
                 continue
             if self.col_cluster:
-                self.calculate_col_dendrograms(self.data2d.loc[:, cols])
-                self.dendrogram_cols.append(self.dendrogram_col)
-                self.col_order.append(self.dendrogram_col.dendrogram['ivl'])
+                col_order=self.get_samples_order(self.data2d.loc[:,cols],self.row_order)
+                self.col_order.append(col_order)
             else:
                 self.col_order.append(cols)
 
     def plot_matrix(self, row_order, col_order):
         if self.verbose >= 1:
             print("Plotting matrix..")
         nrows = len(row_order)
```

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/tools.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.4/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.3.9
+Version: 1.4
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -64,15 +64,15 @@
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
 ## **Usage**
 ----------------------
-### **1. Simple Guide To Get started.**
+### **1. [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html).**
 ```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
 df['CD'] = ['C'] * 3 + ['D'] * 3 + ['G'] * 4
 df['EF'] = ['E'] * 6 + ['F'] * 2 + ['H'] * 2
@@ -89,23 +89,25 @@
 df_heatmap.iloc[1, 2] = np.nan
 
 #Annotate the rows with sample4 > 0.5
 df_rows = df_heatmap.apply(lambda x:x.name if x.sample4 > 0.5 else None,axis=1)
 df_rows=df_rows.to_frame(name='Selected')
 df_rows['XY']=df_rows.index.to_series().apply(lambda x:'A' if int(x.replace('Fea',''))>=15 else 'B')
 
+#Create row annotations
 row_ha = HeatmapAnnotation(
                            Scatter=anno_scatterplot(df_heatmap.sample4.apply(lambda x:round(x,2)),
                                             height=12,cmap='jet',legend=False),
                            Bar=anno_barplot(df_heatmap.sample4.apply(lambda x:round(x,2)),
                                             height=16,cmap='rainbow',legend=False),
                            selected=anno_label(df_rows,colors='red',relpos=(-0.05,0.4)),
                            label_kws={'rotation':30,'horizontalalignment':'left','verticalalignment':'bottom'},
                             axis=0,verbose=0)
 
+#Create column annotations
 col_ha = HeatmapAnnotation(label=anno_label(df.AB, merge=True,rotation=10),
                            AB=anno_simple(df.AB,add_text=True),axis=1,
                            CD=anno_simple(df.CD,add_text=True),
                            EF=anno_simple(df.EF,add_text=True,
                                             legend_kws={'frameon':True}),
                            G=anno_boxplot(df_box, cmap='jet',legend=False),
                            verbose=0)
@@ -119,50 +121,86 @@
                        show_rownames=False,show_colnames=True,
                        tree_kws={'row_cmap': 'Set1'},verbose=0,legend_gap=5,
                        cmap='RdYlBu_r',xticklabels_kws={'labelrotation':-45,'labelcolor':'blue'})
 #plt.savefig("example0.pdf", bbox_inches='tight')
 plt.show()
 ```
 ### Example output
-<p align="center"> 
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
-<img src="docs/images/1.jpg" width=700 align="center">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/clustermap.html#3.3-Top,-bottom,-left-,right-annotations">
-<img src="docs/images/2.png" width=600 align="middle">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Change-orentation-to-the-right">
-<img src="docs/images/3.png" width=700 align="middle">
-</a>
-</p>
-<!-- ![image](docs/images/4.png) -->
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/cpg_modules.html#Plotting-the-Dot-clustermap">
-<img src="docs/images/4.png" width=600 align="middle">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
-<img src="docs/images/5.jpg" width=500 align="middle">
-</a>
-</p>
-
-<p align="center">
-<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
-<img src="docs/images/6.png" width=600 align="middle">
-</a>
-</p>
+Click picture to view the source code
+
+<table>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#3.-Test-the-row-/-col-orders-&-add-selected-rows-labels">
+                <img src="docs/images/gallery1.jpg" title="Heatmap with annotations" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.1-Plot-clustermap-using-seaborn-brain-networks-dataset">
+                <img src="docs/images/gallery11.png" title="Dot heatmap for correlation matrix" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
+                <img src="docs/images/gallery3.jpg" title="Combine two heatmap horizontally" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#4.-Annotations">
+                <img src="docs/images/gallery5.png" title="Only plot annotations" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/clustermap.html#3.3-Top,-bottom,-left-,right-annotations">
+                <img src="docs/images/gallery6.png" title="cluster heatmap" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/single_cell_methylation.html">
+                <img src="docs/images/gallery9.png" title="DNA methylation cell type specific signatures" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
+                <img src="docs/images/gallery8.png" title="OncoPrint with columns split" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#4.2-Visualize-up-to-five-dimension-data-using-DotClustermapPlotter">
+                <img src="docs/images/gallery7.png" title="Dot clustermap to show enrichment result" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
+                <img src="docs/images/gallery4.png" title="OncoPrint with mroe annotations" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+    <tr style="height: 500px">
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/cpg_modules.html#Plotting-the-Dot-clustermap">
+                <img src="docs/images/gallery2.png" title="Dot clustermap with annotations" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/dotHeatmap.html#Changing-the-size-of-point">
+                <img src="docs/images/gallery10.png" title="Dot heatmap using different dot size" align="center" width="250px">
+            </a>
+        </td>
+        <td style="width:33%; background-color:white;text-align:center; vertical-align:middle">
+            <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html#Change-orentation-to-the-left">
+                <img src="docs/images/gallery12.png" title="Plot only the annotation with different orientations" align="center" width="250px">
+            </a>
+        </td>
+    </tr>
+</table>
 
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
 
 ## Call for Contributions
 ----------------------
```

### Comparing `PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/SOURCES.txt` & `PyComplexHeatmap-1.4/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.9/pyproject.toml` & `PyComplexHeatmap-1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.3.9"
+version = "1.4"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.3.9/setup.py` & `PyComplexHeatmap-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.3.9',
+   version='1.4',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

