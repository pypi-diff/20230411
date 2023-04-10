# Comparing `tmp/pandacolumns-0.1.6.tar.gz` & `tmp/pandacolumns-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.6.tar", last modified: Mon Apr 10 21:48:10 2023, max compression
+gzip compressed data, was "pandacolumns-0.1.7.tar", last modified: Mon Apr 10 22:23:26 2023, max compression
```

## Comparing `pandacolumns-0.1.6.tar` & `pandacolumns-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:48:10.607488 pandacolumns-0.1.6/
--rw-rw-rw-   0        0        0      171 2023-04-10 21:48:10.606482 pandacolumns-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 21:48:10.589822 pandacolumns-0.1.6/pandacolumns/
--rw-rw-rw-   0        0        0     2111 2023-04-10 19:52:41.000000 pandacolumns-0.1.6/pandacolumns/PandaDrop.py
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.1.6/pandacolumns/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:48:10.605977 pandacolumns-0.1.6/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 21:48:10.000000 pandacolumns-0.1.6/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-04-10 21:48:10.000000 pandacolumns-0.1.6/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 21:48:10.000000 pandacolumns-0.1.6/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 21:48:10.000000 pandacolumns-0.1.6/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 21:48:10.000000 pandacolumns-0.1.6/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:48:10.607488 pandacolumns-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 21:48:02.000000 pandacolumns-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:23:26.921784 pandacolumns-0.1.7/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:23:26.920659 pandacolumns-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 22:23:26.897601 pandacolumns-0.1.7/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.1.7/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-04-10 22:22:44.000000 pandacolumns-0.1.7/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:23:26.919153 pandacolumns-0.1.7/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:23:26.921784 pandacolumns-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 22:23:21.000000 pandacolumns-0.1.7/setup.py
```

### Comparing `pandacolumns-0.1.6/pandacolumns/PandaDrop.py` & `pandacolumns-0.1.7/pandacolumns/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import ipywidgets as widgets
 from IPython.display import display
 
-def PandaDrop(df):
+def pandadrop(df):
   checkboxes = [widgets.Checkbox(value=False, description=column) for column in df.columns]
 
   for checkbox in checkboxes:
       checkbox.layout.width = 'auto'
       #checkbox.layout.margin = '10px'
       checkbox.style.description_width = 'initial'
       checkbox.style.font_weight = 'bold'
@@ -36,31 +36,30 @@
       button_style='', 
       tooltip='Submit',
       icon='')
 
 
   def on_submit_button_click_keep(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
-      global df
       df = df[selected_columns]
       return df
 
   def on_submit_button_click_drop(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
-      global df
       df = df.drop(selected_columns,axis = 1)
       return df
 
   def on_submit_button_click_rollback(b):
-      global df
       df = df1.copy()
       return df
     
   submit_button_keep.on_click(on_submit_button_click_keep)
   submit_button_drop.on_click(on_submit_button_click_drop)
   submit_button_rollback.on_click(on_submit_button_click_rollback)
 
   checkboxes_box = widgets.VBox(children=checkboxes)
   submit_box = widgets.VBox(children=[widgets.Label(value=''), submit_button_keep, submit_button_drop,submit_button_rollback])
   submit_box.layout.margin = '30px 0px 0px 20px'
   full_box = widgets.HBox(children=[checkboxes_box, submit_box])
-  display(full_box)
+  display(full_box)
+
+
```

