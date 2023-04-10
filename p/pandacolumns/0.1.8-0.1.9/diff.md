# Comparing `tmp/pandacolumns-0.1.8.tar.gz` & `tmp/pandacolumns-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.8.tar", last modified: Mon Apr 10 22:28:50 2023, max compression
+gzip compressed data, was "pandacolumns-0.1.9.tar", last modified: Mon Apr 10 22:39:47 2023, max compression
```

## Comparing `pandacolumns-0.1.8.tar` & `pandacolumns-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:28:50.649787 pandacolumns-0.1.8/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:28:50.649787 pandacolumns-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 22:28:50.630730 pandacolumns-0.1.8/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.1.8/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2076 2023-04-10 22:28:21.000000 pandacolumns-0.1.8/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:28:50.647533 pandacolumns-0.1.8/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:28:50.649787 pandacolumns-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 22:28:42.000000 pandacolumns-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:39:47.878899 pandacolumns-0.1.9/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:39:47.877899 pandacolumns-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 22:39:47.848393 pandacolumns-0.1.9/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.1.9/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2209 2023-04-10 22:39:10.000000 pandacolumns-0.1.9/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:39:47.874920 pandacolumns-0.1.9/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:39:47.879897 pandacolumns-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 22:39:25.000000 pandacolumns-0.1.9/setup.py
```

### Comparing `pandacolumns-0.1.8/pandacolumns/dynamic.py` & `pandacolumns-0.1.9/pandacolumns/dynamic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import pandas as pd
 import ipywidgets as widgets
 from IPython.display import display
-
-def pandadrop(df):
-  checkboxes = [widgets.Checkbox(value=False, description=column) for column in df.columns]
-
+def pandadrop(mydataframe):
+  checkboxes = [widgets.Checkbox(value=False, description=column) for column in mydataframe.columns]
   for checkbox in checkboxes:
       checkbox.layout.width = 'auto'
       #checkbox.layout.margin = '10px'
       checkbox.style.description_width = 'initial'
       checkbox.style.font_weight = 'bold'
       checkbox.style.font_size = '16px'
       checkbox.style.description_color = '#333333'
       checkbox.style.background_color = 'lightblue'
 
-  df1 = df.copy()
+  
+  df1 = mydataframe.copy()
+  
 
   submit_button_keep = widgets.Button(
       description='Keep selected',
       disabled=False,
       button_style='', 
       tooltip='Submit',
       icon='')
@@ -33,33 +32,33 @@
   submit_button_rollback = widgets.Button(
       description='Rollback',
       disabled=False,
       button_style='', 
       tooltip='Submit',
       icon='')
 
-
-  def on_submit_button_click_keep(b,df):
+  def on_submit_button_click_keep(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
-      df = df[selected_columns]
-      return df
+      global mydataframe
+      mydataframe = df[selected_columns]
+      return mydataframe
 
-  def on_submit_button_click_drop(b,df):
+  def on_submit_button_click_drop(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
-      df = df.drop(selected_columns,axis = 1)
-      return df
-
-  def on_submit_button_click_rollback(b,df1):
-      df = df1.copy()
-      return df
+      global mydataframe
+      mydataframe = mydataframe.drop(selected_columns,axis = 1)
+      return mydataframe
+
+  def on_submit_button_click_rollback(b):
+      global mydataframe
+      mydataframe = df1.copy()
+      return mydataframe
     
   submit_button_keep.on_click(on_submit_button_click_keep)
   submit_button_drop.on_click(on_submit_button_click_drop)
   submit_button_rollback.on_click(on_submit_button_click_rollback)
 
   checkboxes_box = widgets.VBox(children=checkboxes)
   submit_box = widgets.VBox(children=[widgets.Label(value=''), submit_button_keep, submit_button_drop,submit_button_rollback])
   submit_box.layout.margin = '30px 0px 0px 20px'
   full_box = widgets.HBox(children=[checkboxes_box, submit_box])
-  display(full_box)
-
-
+  display(full_box)
```

