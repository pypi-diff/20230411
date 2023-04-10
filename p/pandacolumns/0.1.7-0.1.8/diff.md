# Comparing `tmp/pandacolumns-0.1.7.tar.gz` & `tmp/pandacolumns-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.7.tar", last modified: Mon Apr 10 22:23:26 2023, max compression
+gzip compressed data, was "pandacolumns-0.1.8.tar", last modified: Mon Apr 10 22:28:50 2023, max compression
```

## Comparing `pandacolumns-0.1.7.tar` & `pandacolumns-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:23:26.921784 pandacolumns-0.1.7/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:23:26.920659 pandacolumns-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 22:23:26.897601 pandacolumns-0.1.7/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.1.7/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-04-10 22:22:44.000000 pandacolumns-0.1.7/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:23:26.919153 pandacolumns-0.1.7/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 22:23:26.000000 pandacolumns-0.1.7/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:23:26.921784 pandacolumns-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 22:23:21.000000 pandacolumns-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:28:50.649787 pandacolumns-0.1.8/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:28:50.649787 pandacolumns-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 22:28:50.630730 pandacolumns-0.1.8/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.1.8/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2076 2023-04-10 22:28:21.000000 pandacolumns-0.1.8/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:28:50.647533 pandacolumns-0.1.8/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:28:50.000000 pandacolumns-0.1.8/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:28:50.649787 pandacolumns-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 22:28:42.000000 pandacolumns-0.1.8/setup.py
```

### Comparing `pandacolumns-0.1.7/pandacolumns/dynamic.py` & `pandacolumns-0.1.8/pandacolumns/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,25 +34,25 @@
       description='Rollback',
       disabled=False,
       button_style='', 
       tooltip='Submit',
       icon='')
 
 
-  def on_submit_button_click_keep(b):
+  def on_submit_button_click_keep(b,df):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       df = df[selected_columns]
       return df
 
-  def on_submit_button_click_drop(b):
+  def on_submit_button_click_drop(b,df):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       df = df.drop(selected_columns,axis = 1)
       return df
 
-  def on_submit_button_click_rollback(b):
+  def on_submit_button_click_rollback(b,df1):
       df = df1.copy()
       return df
     
   submit_button_keep.on_click(on_submit_button_click_keep)
   submit_button_drop.on_click(on_submit_button_click_drop)
   submit_button_rollback.on_click(on_submit_button_click_rollback)
```

