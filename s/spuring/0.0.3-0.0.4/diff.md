# Comparing `tmp/spuring-0.0.3.tar.gz` & `tmp/spuring-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spuring-0.0.3.tar", last modified: Mon Jan 23 20:40:49 2023, max compression
+gzip compressed data, was "spuring-0.0.4.tar", last modified: Tue Apr 11 18:36:09 2023, max compression
```

## Comparing `spuring-0.0.3.tar` & `spuring-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-01-23 20:40:49.182905 spuring-0.0.3/
--rw-rw-rw-   0        0        0     1103 2023-01-12 19:45:14.000000 spuring-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0       34 2023-01-21 19:23:55.000000 spuring-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2891 2023-01-23 20:40:49.181881 spuring-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2023-01-23 20:40:33.000000 spuring-0.0.3/README.md
--rw-rw-rw-   0        0        0      437 2023-01-23 20:28:21.000000 spuring-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-23 20:40:49.182905 spuring-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-23 20:40:49.146976 spuring-0.0.3/spuring/
--rw-rw-rw-   0        0        0       68 2023-01-23 19:40:23.000000 spuring-0.0.3/spuring/__init__.py
--rw-rw-rw-   0        0        0       90 2023-01-23 19:41:00.000000 spuring-0.0.3/spuring/__main__.py
--rw-rw-rw-   0        0        0     2172 2023-01-21 12:07:55.000000 spuring-0.0.3/spuring/creation.py
--rw-rw-rw-   0        0        0     2260 2023-01-23 19:46:52.000000 spuring-0.0.3/spuring/main.py
-drwxrwxrwx   0        0        0        0 2023-01-23 20:40:49.172906 spuring-0.0.3/spuring/scripts/
--rw-rw-rw-   0        0        0      687 2023-01-23 19:41:51.000000 spuring-0.0.3/spuring/scripts/pip.py
--rw-rw-rw-   0        0        0      378 2023-01-23 19:42:01.000000 spuring-0.0.3/spuring/scripts/venv.py
--rw-rw-rw-   0        0        0     2249 2023-01-23 19:25:22.000000 spuring-0.0.3/spuring/template.py
-drwxrwxrwx   0        0        0        0 2023-01-23 20:40:49.177892 spuring-0.0.3/spuring/templates/
--rw-rw-rw-   0        0        0      684 2023-01-23 20:18:49.000000 spuring-0.0.3/spuring/templates/base.toml
--rw-rw-rw-   0        0        0      282 2023-01-23 20:21:40.000000 spuring-0.0.3/spuring/templates/default.toml
--rw-rw-rw-   0        0        0      542 2023-01-23 19:08:18.000000 spuring-0.0.3/spuring/templates/flask.toml
-drwxrwxrwx   0        0        0        0 2023-01-23 20:40:49.169912 spuring-0.0.3/spuring.egg-info/
--rw-rw-rw-   0        0        0     2891 2023-01-23 20:40:49.000000 spuring-0.0.3/spuring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-01-23 20:40:49.000000 spuring-0.0.3/spuring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 20:40:49.000000 spuring-0.0.3/spuring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-01-23 20:40:49.000000 spuring-0.0.3/spuring.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-01-23 20:40:49.000000 spuring-0.0.3/spuring.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-23 20:40:49.000000 spuring-0.0.3/spuring.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-23 20:40:49.180884 spuring-0.0.3/test/
--rw-rw-rw-   0        0        0      176 2023-01-12 18:38:47.000000 spuring-0.0.3/test/TestCreation.py
--rw-rw-rw-   0        0        0      787 2023-01-23 20:21:21.000000 spuring-0.0.3/test/TestMain.py
--rw-rw-rw-   0        0        0     1688 2023-01-23 19:08:18.000000 spuring-0.0.3/test/TestTemplate.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:36:09.246105 spuring-0.0.4/
+-rw-rw-rw-   0        0        0     1103 2023-01-12 19:45:14.000000 spuring-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0       34 2023-01-21 19:23:55.000000 spuring-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2891 2023-04-11 18:36:09.246105 spuring-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2023-01-23 20:40:33.000000 spuring-0.0.4/README.md
+-rw-rw-rw-   0        0        0      439 2023-04-11 18:35:52.000000 spuring-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 18:36:09.247104 spuring-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 18:36:09.212523 spuring-0.0.4/spuring/
+-rw-rw-rw-   0        0        0       68 2023-01-23 19:40:23.000000 spuring-0.0.4/spuring/__init__.py
+-rw-rw-rw-   0        0        0       90 2023-01-23 19:41:00.000000 spuring-0.0.4/spuring/__main__.py
+-rw-rw-rw-   0        0        0     2172 2023-01-21 12:07:55.000000 spuring-0.0.4/spuring/creation.py
+-rw-rw-rw-   0        0        0     2260 2023-01-23 19:46:52.000000 spuring-0.0.4/spuring/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:36:09.237590 spuring-0.0.4/spuring/scripts/
+-rw-rw-rw-   0        0        0      686 2023-04-11 18:27:30.000000 spuring-0.0.4/spuring/scripts/pip.py
+-rw-rw-rw-   0        0        0      313 2023-04-11 17:53:07.000000 spuring-0.0.4/spuring/scripts/venv.py
+-rw-rw-rw-   0        0        0     2249 2023-01-23 19:25:22.000000 spuring-0.0.4/spuring/template.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:36:09.241104 spuring-0.0.4/spuring/templates/
+-rw-rw-rw-   0        0        0      684 2023-01-23 20:18:49.000000 spuring-0.0.4/spuring/templates/base.toml
+-rw-rw-rw-   0        0        0      281 2023-04-11 18:09:16.000000 spuring-0.0.4/spuring/templates/default.toml
+-rw-rw-rw-   0        0        0      541 2023-04-11 18:09:16.000000 spuring-0.0.4/spuring/templates/flask.toml
+drwxrwxrwx   0        0        0        0 2023-04-11 18:36:09.229541 spuring-0.0.4/spuring.egg-info/
+-rw-rw-rw-   0        0        0     2891 2023-04-11 18:36:09.000000 spuring-0.0.4/spuring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2023-04-11 18:36:09.000000 spuring-0.0.4/spuring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 18:36:09.000000 spuring-0.0.4/spuring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-11 18:36:09.000000 spuring-0.0.4/spuring.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 18:36:09.000000 spuring-0.0.4/spuring.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 18:36:09.000000 spuring-0.0.4/spuring.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 18:36:09.245105 spuring-0.0.4/test/
+-rw-rw-rw-   0        0        0      176 2023-01-12 18:38:47.000000 spuring-0.0.4/test/TestCreation.py
+-rw-rw-rw-   0        0        0      787 2023-01-23 20:21:21.000000 spuring-0.0.4/test/TestMain.py
+-rw-rw-rw-   0        0        0     1688 2023-01-23 19:08:18.000000 spuring-0.0.4/test/TestTemplate.py
```

### Comparing `spuring-0.0.3/LICENSE.md` & `spuring-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/PKG-INFO` & `spuring-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spuring
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create a project folder. It can be self configurated
 Author-email: Tobias Baumgarten <Tobias.b.baumgarten@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Welcome to spuring documentation
```

### Comparing `spuring-0.0.3/README.md` & `spuring-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/spuring/creation.py` & `spuring-0.0.4/spuring/creation.py`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/spuring/main.py` & `spuring-0.0.4/spuring/main.py`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/spuring/scripts/pip.py` & `spuring-0.0.4/spuring/scripts/pip.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import sys
 from spuring import Template
 
 
 def process(template: Template, wd: Path):
     if "pip" not in template.scripts:
         return
-    # pip dependencie installation
+    # pip dependencies installation
     exe = sys.executable
     if "venv" in template.scripts:
         dir = wd / template.scripts["venv"]
         # setup the path - windows and linux path are different
         dir /= "Scripts" if os.name == "nt" else "bin"
-        exe = dir / "python.exe"
+        exe = dir / "python"
     # update pip
+
     os.system(f"{exe} -m pip install -U pip")
     # load the value from the pip attribute and run
     req = wd / template.scripts['pip']
     os.system(f"{exe} -m pip install -r {req}")
```

### Comparing `spuring-0.0.3/spuring/template.py` & `spuring-0.0.4/spuring/template.py`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/spuring/templates/base.toml` & `spuring-0.0.4/spuring/templates/base.toml`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/spuring/templates/flask.toml` & `spuring-0.0.4/spuring/templates/flask.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "base.toml" %}
 {% block base %}
 name = "flask"
 description = "creates a default flask project"
 narrative = "A simple project setup with flask and autopep8"
 
 [scripts]
-venv = ".venv"
+venv = "venv"
 pip = "requirements.txt"
 {% endblock %}
 
 {% block files %}
 pyinit.content = "_obj:init"
 req = {path="requirements.txt", content="flask"}
 {% endblock %}
```

### Comparing `spuring-0.0.3/spuring.egg-info/PKG-INFO` & `spuring-0.0.4/spuring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spuring
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create a project folder. It can be self configurated
 Author-email: Tobias Baumgarten <Tobias.b.baumgarten@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Welcome to spuring documentation
```

### Comparing `spuring-0.0.3/spuring.egg-info/SOURCES.txt` & `spuring-0.0.4/spuring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/test/TestMain.py` & `spuring-0.0.4/test/TestMain.py`

 * *Files identical despite different names*

### Comparing `spuring-0.0.3/test/TestTemplate.py` & `spuring-0.0.4/test/TestTemplate.py`

 * *Files identical despite different names*

