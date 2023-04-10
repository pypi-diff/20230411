# Comparing `tmp/pandacolumns-0.1.9.tar.gz` & `tmp/pandacolumns-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.9.tar", last modified: Mon Apr 10 22:39:47 2023, max compression
+gzip compressed data, was "pandacolumns-0.2.0.tar", last modified: Mon Apr 10 22:46:45 2023, max compression
```

## Comparing `pandacolumns-0.1.9.tar` & `pandacolumns-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:39:47.878899 pandacolumns-0.1.9/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:39:47.877899 pandacolumns-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 22:39:47.848393 pandacolumns-0.1.9/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.1.9/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2209 2023-04-10 22:39:10.000000 pandacolumns-0.1.9/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:39:47.874920 pandacolumns-0.1.9/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 22:39:47.000000 pandacolumns-0.1.9/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:39:47.879897 pandacolumns-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 22:39:25.000000 pandacolumns-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:46:45.059256 pandacolumns-0.2.0/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:46:45.057079 pandacolumns-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 22:46:45.033032 pandacolumns-0.2.0/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.0/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2218 2023-04-10 22:45:08.000000 pandacolumns-0.2.0/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:46:45.055088 pandacolumns-0.2.0/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:46:44.000000 pandacolumns-0.2.0/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:46:45.059256 pandacolumns-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 22:46:38.000000 pandacolumns-0.2.0/setup.py
```

### Comparing `pandacolumns-0.1.9/pandacolumns/dynamic.py` & `pandacolumns-0.2.0/pandacolumns/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       button_style='', 
       tooltip='Submit',
       icon='')
 
   def on_submit_button_click_keep(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       global mydataframe
-      mydataframe = df[selected_columns]
+      mydataframe = mydataframe[selected_columns]
       return mydataframe
 
   def on_submit_button_click_drop(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       global mydataframe
       mydataframe = mydataframe.drop(selected_columns,axis = 1)
       return mydataframe
```

