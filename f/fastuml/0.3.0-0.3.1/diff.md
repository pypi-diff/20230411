# Comparing `tmp/fastuml-0.3.0.tar.gz` & `tmp/fastuml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastuml-0.3.0.tar", last modified: Tue Apr 11 10:02:33 2023, max compression
+gzip compressed data, was "fastuml-0.3.1.tar", last modified: Tue Apr 11 10:32:23 2023, max compression
```

## Comparing `fastuml-0.3.0.tar` & `fastuml-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:33.154737 fastuml-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 10:02:23.000000 fastuml-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 10:02:33.154737 fastuml-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 10:02:23.000000 fastuml-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-11 10:02:23.000000 fastuml-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:02:33.154737 fastuml-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:33.150737 fastuml-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:33.150737 fastuml-0.3.0/src/fastuml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/class_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:33.150737 fastuml-0.3.0/src/fastuml/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/grammar/class_options.tx
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/grammar/class_uml.tx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:33.150737 fastuml-0.3.0/src/fastuml/grammar/components/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/grammar/components/base.tx
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/grammar/components/class_commons.tx
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/grammar/components/options.tx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:33.154737 fastuml-0.3.0/src/fastuml/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/class.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/connection.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/package.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/plantuml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/plantuml_class.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/plantuml_connection.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/plantuml_package.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/templates/uml.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-11 10:02:23.000000 fastuml-0.3.0/src/fastuml/uml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:02:33.150737 fastuml-0.3.0/src/fastuml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 10:02:33.000000 fastuml-0.3.0/src/fastuml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-11 10:02:33.000000 fastuml-0.3.0/src/fastuml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:02:33.000000 fastuml-0.3.0/src/fastuml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 10:02:33.000000 fastuml-0.3.0/src/fastuml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 10:02:33.000000 fastuml-0.3.0/src/fastuml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 10:02:33.000000 fastuml-0.3.0/src/fastuml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:23.265904 fastuml-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 10:32:12.000000 fastuml-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 10:32:23.265904 fastuml-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 10:32:12.000000 fastuml-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-11 10:32:12.000000 fastuml-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:32:23.265904 fastuml-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:23.261904 fastuml-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:23.261904 fastuml-0.3.1/src/fastuml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/class_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:23.265904 fastuml-0.3.1/src/fastuml/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/grammar/class_options.tx
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/grammar/class_uml.tx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:23.265904 fastuml-0.3.1/src/fastuml/grammar/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/grammar/components/base.tx
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/grammar/components/class_commons.tx
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/grammar/components/options.tx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:23.265904 fastuml-0.3.1/src/fastuml/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/class.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/connection.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/package.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/plantuml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/plantuml_class.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/plantuml_connection.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/plantuml_package.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/templates/uml.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-11 10:32:12.000000 fastuml-0.3.1/src/fastuml/uml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:32:23.265904 fastuml-0.3.1/src/fastuml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 10:32:23.000000 fastuml-0.3.1/src/fastuml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-11 10:32:23.000000 fastuml-0.3.1/src/fastuml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:32:23.000000 fastuml-0.3.1/src/fastuml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 10:32:23.000000 fastuml-0.3.1/src/fastuml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 10:32:23.000000 fastuml-0.3.1/src/fastuml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 10:32:23.000000 fastuml-0.3.1/src/fastuml.egg-info/top_level.txt
```

### Comparing `fastuml-0.3.0/LICENSE` & `fastuml-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/pyproject.toml` & `fastuml-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastuml"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Mathis Logemann" },
 ]
 dependencies = [
   'textx',
   'Jinja2',
   'click'
```

### Comparing `fastuml-0.3.0/src/fastuml/class_options.py` & `fastuml-0.3.1/src/fastuml/class_options.py`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/grammar/class_uml.tx` & `fastuml-0.3.1/src/fastuml/grammar/class_uml.tx`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/grammar/components/options.tx` & `fastuml-0.3.1/src/fastuml/grammar/components/options.tx`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/class.jinja` & `fastuml-0.3.1/src/fastuml/templates/class.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/connection.jinja` & `fastuml-0.3.1/src/fastuml/templates/connection.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/package.jinja` & `fastuml-0.3.1/src/fastuml/templates/package.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/plantuml.jinja` & `fastuml-0.3.1/src/fastuml/templates/plantuml.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/plantuml_class.jinja` & `fastuml-0.3.1/src/fastuml/templates/plantuml_class.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/plantuml_connection.jinja` & `fastuml-0.3.1/src/fastuml/templates/plantuml_connection.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/plantuml_package.jinja` & `fastuml-0.3.1/src/fastuml/templates/plantuml_package.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/templates/uml.jinja` & `fastuml-0.3.1/src/fastuml/templates/uml.jinja`

 * *Files identical despite different names*

### Comparing `fastuml-0.3.0/src/fastuml/uml.py` & `fastuml-0.3.1/src/fastuml/uml.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if not visible:
             return False
         return isModelVisible(model, "visibleConnections")
 
     jinja_env.filters["modelVisible"] = isModelVisibleEntry
     jinja_env.filters["edgeVisible"] = isEdgeVisible
 
-    template = jinja_env.get_template("plantuml.jinja")
+    template = jinja_env.get_template("uml.jinja")
 
     for f in file:
         logging.info("processing file {}".format(f))
         model = class_uml_meta.model_from_file(f)
         class_options.overrideDefaultOptions(model=model, option_model=options_model)
         if not model.options.direction:
             model.options.direction = "BT"
```

### Comparing `fastuml-0.3.0/src/fastuml.egg-info/SOURCES.txt` & `fastuml-0.3.1/src/fastuml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

