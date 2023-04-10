# Comparing `tmp/pandacolumns-0.2.0.tar.gz` & `tmp/pandacolumns-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.2.0.tar", last modified: Mon Apr 10 22:46:45 2023, max compression
+gzip compressed data, was "pandacolumns-0.2.1.tar", last modified: Mon Apr 10 22:56:17 2023, max compression
```

## Comparing `pandacolumns-0.2.0.tar` & `pandacolumns-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:46:45.059256 pandacolumns-0.2.0/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:46:45.057079 pandacolumns-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 22:46:45.033032 pandacolumns-0.2.0/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.0/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2218 2023-04-10 22:45:08.000000 pandacolumns-0.2.0/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:46:45.055088 pandacolumns-0.2.0/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:46:45.059256 pandacolumns-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 22:46:38.000000 pandacolumns-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:56:17.144163 pandacolumns-0.2.1/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:56:17.143153 pandacolumns-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 22:56:17.123878 pandacolumns-0.2.1/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.1/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2155 2023-04-10 22:55:37.000000 pandacolumns-0.2.1/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:56:17.141995 pandacolumns-0.2.1/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:56:16.000000 pandacolumns-0.2.1/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:56:17.144163 pandacolumns-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 22:55:48.000000 pandacolumns-0.2.1/setup.py
```

### Comparing `pandacolumns-0.2.0/pandacolumns/dynamic.py` & `pandacolumns-0.2.1/pandacolumns/dynamic.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,26 +36,26 @@
       tooltip='Submit',
       icon='')
 
   def on_submit_button_click_keep(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       global mydataframe
       mydataframe = mydataframe[selected_columns]
-      return mydataframe
+   
 
   def on_submit_button_click_drop(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       global mydataframe
       mydataframe = mydataframe.drop(selected_columns,axis = 1)
-      return mydataframe
+    
 
   def on_submit_button_click_rollback(b):
       global mydataframe
       mydataframe = df1.copy()
-      return mydataframe
+  
     
   submit_button_keep.on_click(on_submit_button_click_keep)
   submit_button_drop.on_click(on_submit_button_click_drop)
   submit_button_rollback.on_click(on_submit_button_click_rollback)
 
   checkboxes_box = widgets.VBox(children=checkboxes)
   submit_box = widgets.VBox(children=[widgets.Label(value=''), submit_button_keep, submit_button_drop,submit_button_rollback])
```

