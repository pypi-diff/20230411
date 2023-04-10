# Comparing `tmp/motion_python-0.1.29.tar.gz` & `tmp/motion_python-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.29.tar", max compression
+gzip compressed data, was "motion_python-0.1.30.tar", max compression
```

## Comparing `motion_python-0.1.29.tar` & `motion_python-0.1.30.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2819 2023-04-10 05:04:02.615301 motion_python-0.1.29/README.md
--rw-r--r--   0        0        0      641 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/api/__init__.py
--rw-r--r--   0        0        0     6702 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/api/models.py
--rw-r--r--   0        0        0     2582 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/cli.py
--rw-r--r--   0        0        0     9885 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/client.py
--rw-r--r--   0        0        0    21544 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/cursor.py
--rw-r--r--   0        0        0     8664 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1348 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/routing.py
--rw-r--r--   0        0        0     3477 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/schema.py
--rw-r--r--   0        0        0    14188 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/store.py
--rw-r--r--   0        0        0     3741 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/task.py
--rw-r--r--   0        0        0     5977 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/trigger.py
--rw-r--r--   0        0        0     1092 2023-04-10 05:04:02.619301 motion_python-0.1.29/motion/utils.py
--rw-r--r--   0        0        0     1416 2023-04-10 05:04:25.854976 motion_python-0.1.29/pyproject.toml
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0     2819 2023-04-10 22:08:18.695807 motion_python-0.1.30/README.md
+-rw-r--r--   0        0        0      641 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/api/__init__.py
+-rw-r--r--   0        0        0     6702 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/api/models.py
+-rw-r--r--   0        0        0     2618 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/cli.py
+-rw-r--r--   0        0        0     9885 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/client.py
+-rw-r--r--   0        0        0    21544 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/cursor.py
+-rw-r--r--   0        0        0     8664 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1348 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/routing.py
+-rw-r--r--   0        0        0     3477 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/schema.py
+-rw-r--r--   0        0        0    14188 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/store.py
+-rw-r--r--   0        0        0     3741 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/task.py
+-rw-r--r--   0        0        0     5977 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/trigger.py
+-rw-r--r--   0        0        0     1092 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/utils.py
+-rw-r--r--   0        0        0     1416 2023-04-10 22:08:38.351831 motion_python-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.30/PKG-INFO
```

### Comparing `motion_python-0.1.29/README.md` & `motion_python-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/__init__.py` & `motion_python-0.1.30/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/api/api.py` & `motion_python-0.1.30/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/api/models.py` & `motion_python-0.1.30/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/cli.py` & `motion_python-0.1.30/motion/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     """Creates a new application."""
     motion.create_app(name, author)
 
     click.echo("Created a project successfully.")
 
 
 @motioncli.command("serve")
-@click.argument("host", required=False, default="0.0.0.0")
-@click.argument("port", required=False, default=5000)
+@click.option("host", "--host", default="0.0.0.0", help="Host to serve on.")
+@click.option("port", "--port", default=5000, help="Port to serve on.")
 @click.option(
     "logging_level",
     "--logging-level",
     "-l",
     default="WARNING",
     help="Logging level for motion. Can be DEBUG, INFO, WARNING, ERROR, CRITICAL.",
 )
```

### Comparing `motion_python-0.1.29/motion/client.py` & `motion_python-0.1.30/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/cursor.py` & `motion_python-0.1.30/motion/cursor.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/entry.py` & `motion_python-0.1.30/motion/entry.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/examples/cooking/dashboard.py` & `motion_python-0.1.30/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/examples/cooking/test.py` & `motion_python-0.1.30/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.30/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.30/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/routing.py` & `motion_python-0.1.30/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/schema.py` & `motion_python-0.1.30/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/store.py` & `motion_python-0.1.30/motion/store.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/task.py` & `motion_python-0.1.30/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/trigger.py` & `motion_python-0.1.30/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/motion/utils.py` & `motion_python-0.1.30/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.29/pyproject.toml` & `motion_python-0.1.30/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.29"
+version = "0.1.30"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `motion_python-0.1.29/PKG-INFO` & `motion_python-0.1.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.29
+Version: 0.1.30
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

