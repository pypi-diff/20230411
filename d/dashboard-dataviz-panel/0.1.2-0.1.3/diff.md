# Comparing `tmp/dashboard_dataviz_panel-0.1.2-py3-none-any.whl.zip` & `tmp/dashboard_dataviz_panel-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9667 bytes, number of entries: 9
+Zip file size: 9670 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Apr-10 15:09 dashboard_dataviz_panel/__init__.py
 -rw-rw-rw-  2.0 fat     1739 b- defN 23-Apr-02 21:05 dashboard_dataviz_panel/helpers.py
 -rw-rw-rw-  2.0 fat     4303 b- defN 23-Apr-07 04:26 dashboard_dataviz_panel/model.py
--rw-rw-rw-  2.0 fat    16052 b- defN 23-Apr-10 15:06 dashboard_dataviz_panel/plots.py
+-rw-rw-rw-  2.0 fat    16054 b- defN 23-Apr-11 04:00 dashboard_dataviz_panel/plots.py
 -rw-rw-rw-  2.0 fat     3840 b- defN 23-Apr-07 04:13 dashboard_dataviz_panel/tables.py
--rw-rw-rw-  2.0 fat      200 b- defN 23-Apr-10 16:37 dashboard_dataviz_panel-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 16:37 dashboard_dataviz_panel-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 23-Apr-10 16:37 dashboard_dataviz_panel-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      812 b- defN 23-Apr-10 16:37 dashboard_dataviz_panel-0.1.2.dist-info/RECORD
-9 files, 27608 bytes uncompressed, 8245 bytes compressed:  70.1%
+-rw-rw-rw-  2.0 fat      200 b- defN 23-Apr-11 15:06 dashboard_dataviz_panel-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 15:06 dashboard_dataviz_panel-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Apr-11 15:06 dashboard_dataviz_panel-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      812 b- defN 23-Apr-11 15:06 dashboard_dataviz_panel-0.1.3.dist-info/RECORD
+9 files, 27610 bytes uncompressed, 8248 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: dashboard_dataviz_panel/plots.py
 Comment: 
 
 Filename: dashboard_dataviz_panel/tables.py
 Comment: 
 
-Filename: dashboard_dataviz_panel-0.1.2.dist-info/METADATA
+Filename: dashboard_dataviz_panel-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: dashboard_dataviz_panel-0.1.2.dist-info/WHEEL
+Filename: dashboard_dataviz_panel-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: dashboard_dataviz_panel-0.1.2.dist-info/top_level.txt
+Filename: dashboard_dataviz_panel-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dashboard_dataviz_panel-0.1.2.dist-info/RECORD
+Filename: dashboard_dataviz_panel-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dashboard_dataviz_panel/plots.py

```diff
@@ -250,15 +250,15 @@
 def bivar_quanti_plot(df, quanti1, quanti2):
     fig = sns.jointplot(x=quanti1, y=quanti2, data=df, color='red', kind='kde').fig
     plt.close()
     return pn.pane.Matplotlib(fig, sizing_mode='stretch_both')
 
 def cross_heatmap(df,quali1, quali2, color):
 
-    crosstab = pd.crosstab(df[quali1], df[quali2], normalize='index')
+    crosstab = pd.crosstab(df[quali1], df[quali2], normalize='columns')
 
     # Create a Plotly heatmap
     fig = ff.create_annotated_heatmap(
         z=crosstab.values,
         x=list(crosstab.columns),
         y=list(crosstab.index),
         annotation_text=crosstab.round(2).values,
```

## Comparing `dashboard_dataviz_panel-0.1.2.dist-info/RECORD` & `dashboard_dataviz_panel-0.1.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 dashboard_dataviz_panel/__init__.py,sha256=IfTLDGV6yvRWPkFVE1XcTKmIJaPToV3lYMKC1Mrliuw,546
 dashboard_dataviz_panel/helpers.py,sha256=vKWrH-Qs81ET883r-yCjtMdRIH-57CMb1y4Dg7ocrns,1739
 dashboard_dataviz_panel/model.py,sha256=myr6z6yCd4OBLtRAjRw-K7Z6PiXaBTw_pBjyCQXO82E,4303
-dashboard_dataviz_panel/plots.py,sha256=KxNQPS8V9hAUcZZnARCC6MPoFMOzpvMLT4UJw-Wgn50,16052
+dashboard_dataviz_panel/plots.py,sha256=UJqMwObPdNb8JmrfoJM_TIcnbwJqygGkR3ptToJJ9xw,16054
 dashboard_dataviz_panel/tables.py,sha256=lzVieilldfJ6tojzqHY0oo0S6IM9N2YD2di0bBS0M9c,3840
-dashboard_dataviz_panel-0.1.2.dist-info/METADATA,sha256=Yn4x-N3XCCCsyStQQ5Py4ReT9njrquG7mEJfRm3c4CI,200
-dashboard_dataviz_panel-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-dashboard_dataviz_panel-0.1.2.dist-info/top_level.txt,sha256=NApPH9rQcpSER515QJjuUKWbx3kG8c39QEwylWxVRdA,24
-dashboard_dataviz_panel-0.1.2.dist-info/RECORD,,
+dashboard_dataviz_panel-0.1.3.dist-info/METADATA,sha256=6gN1slWwkyeuW12pv6I0ip08W2Iy7QRe9gvu9X8_gc0,200
+dashboard_dataviz_panel-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+dashboard_dataviz_panel-0.1.3.dist-info/top_level.txt,sha256=NApPH9rQcpSER515QJjuUKWbx3kG8c39QEwylWxVRdA,24
+dashboard_dataviz_panel-0.1.3.dist-info/RECORD,,
```

