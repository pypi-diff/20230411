# Comparing `tmp/tkreform-0.3.3.tar.gz` & `tmp/tkreform-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkreform-0.3.3.tar", last modified: Mon Apr 10 16:49:41 2023, max compression
+gzip compressed data, was "tkreform-0.3.4.tar", last modified: Tue Apr 11 18:17:24 2023, max compression
```

## Comparing `tkreform-0.3.3.tar` & `tkreform-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:49:41.970293 tkreform-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 16:49:36.000000 tkreform-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:49:41.970293 tkreform-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 16:49:36.000000 tkreform-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:49:41.970293 tkreform-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-10 16:49:36.000000 tkreform-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:49:41.970293 tkreform-0.3.3/tkreform/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/declarative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/linguist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-10 16:49:36.000000 tkreform-0.3.3/tkreform/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:49:41.970293 tkreform-0.3.3/tkreform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 16:49:41.000000 tkreform-0.3.3/tkreform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:17:24.202396 tkreform-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 18:17:21.000000 tkreform-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-11 18:17:24.202396 tkreform-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 18:17:21.000000 tkreform-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:17:24.202396 tkreform-0.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-11 18:17:21.000000 tkreform-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:17:24.198395 tkreform-0.3.4/tkreform/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/linguist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-11 18:17:21.000000 tkreform-0.3.4/tkreform/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:17:24.202396 tkreform-0.3.4/tkreform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 18:17:24.000000 tkreform-0.3.4/tkreform.egg-info/top_level.txt
```

### Comparing `tkreform-0.3.3/LICENSE` & `tkreform-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/PKG-INFO` & `tkreform-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.3
+Version: 0.3.4
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tkreform-0.3.3/setup.py` & `tkreform-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/tkreform/__init__.py` & `tkreform-0.3.4/tkreform/__init__.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/tkreform/base.py` & `tkreform-0.3.4/tkreform/base.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/tkreform/declarative.py` & `tkreform-0.3.4/tkreform/declarative.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,18 @@
 class MenuBinder:
     win: Optional["Window"] = None
 
 
 @dataclass
 class NotebookAdder:
     state: Literal["normal", "disabled", "hidden"] = "normal"
-    sticky: Optional[Direction] = None
+    sticky: Literal[Direction, "center", ""] = ""
     padding: Padding = (0, 0)
     text: str = ""
-    image: Any = None
+    image: Any = ""
     compound: Compound = "none"
     underline: int = 0
 
 
 class W:
     """Widget data pre-storage."""
     def __init__(self, widget: Type[WidgetType], **kwargs: Any) -> None:
```

### Comparing `tkreform-0.3.3/tkreform/events.py` & `tkreform-0.3.4/tkreform/events.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/tkreform/groups.py` & `tkreform-0.3.4/tkreform/groups.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/tkreform/linguist.py` & `tkreform-0.3.4/tkreform/linguist.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/tkreform/menu.py` & `tkreform-0.3.4/tkreform/menu.py`

 * *Files identical despite different names*

### Comparing `tkreform-0.3.3/tkreform.egg-info/PKG-INFO` & `tkreform-0.3.4/tkreform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkreform
-Version: 0.3.3
+Version: 0.3.4
 Summary: Reformed tkinter coding tool.
 Home-page: https://github.com/tkinguist/tkreform
 Author: HivertMoZara
 Author-email: worldmozara@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

