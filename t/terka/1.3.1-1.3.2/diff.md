# Comparing `tmp/terka-1.3.1.tar.gz` & `tmp/terka-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.3.1.tar", last modified: Tue Apr 11 15:41:37 2023, max compression
+gzip compressed data, was "terka-1.3.2.tar", last modified: Tue Apr 11 15:45:08 2023, max compression
```

## Comparing `terka-1.3.1.tar` & `terka-1.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.3.1/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:41:37.595610 terka-1.3.1/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.3.1/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-11 15:41:37.595610 terka-1.3.1/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-11 15:39:33.000000 terka-1.3.1/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.591610 terka-1.3.1/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.591610 terka-1.3.1/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    13439 2023-04-08 10:39:03.000000 terka-1.3.1/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.3.1/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.3.1/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    32550 2023-04-08 19:16:35.000000 terka-1.3.1/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)      827 2023-03-06 19:56:41.000000 terka-1.3.1/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.3.1/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.3.1/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.3.1/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.3.1/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.3.1/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.3.1/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.3.1/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.3.1/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.3.1/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.3.1/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.3.1/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.3.1/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.3.1/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    26661 2023-04-11 15:37:18.000000 terka-1.3.1/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.3.1/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.3.1/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.3.1/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     6764 2023-04-08 10:39:03.000000 terka-1.3.1/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.3.1/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.344066 terka-1.3.2/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.3.2/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:45:08.344066 terka-1.3.2/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.3.2/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-11 15:45:08.344066 terka-1.3.2/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-11 15:45:04.000000 terka-1.3.2/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.340066 terka-1.3.2/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.2/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.340066 terka-1.3.2/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.2/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    13439 2023-04-08 10:39:03.000000 terka-1.3.2/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.3.2/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.344066 terka-1.3.2/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.2/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.3.2/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    32550 2023-04-08 19:16:35.000000 terka-1.3.2/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)      827 2023-03-06 19:56:41.000000 terka-1.3.2/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.3.2/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.3.2/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.3.2/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.3.2/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.3.2/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.3.2/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.3.2/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.3.2/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.3.2/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.3.2/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.3.2/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.344066 terka-1.3.2/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.3.2/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.3.2/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.344066 terka-1.3.2/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.2/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    26691 2023-04-11 15:44:06.000000 terka-1.3.2/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.3.2/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.3.2/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.3.2/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     6764 2023-04-08 10:39:03.000000 terka-1.3.2/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.344066 terka-1.3.2/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:45:08.000000 terka-1.3.2/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-11 15:45:08.000000 terka-1.3.2/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-11 15:45:08.000000 terka-1.3.2/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-11 15:45:08.000000 terka-1.3.2/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-11 15:45:08.000000 terka-1.3.2/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-11 15:45:08.000000 terka-1.3.2/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:45:08.344066 terka-1.3.2/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.2/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.3.2/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.3.2/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.3.2/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.3.2/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.3.2/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.3.2/tests/test_utils.py
```

### Comparing `terka-1.3.1/LICENSE` & `terka-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/PKG-INFO` & `terka-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.3.1
+Version: 1.3.2
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.3.1/README.md` & `terka-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/setup.py` & `terka-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.3.1",
+    version="1.3.2",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.3.1/src/adapters/orm.py` & `terka-1.3.2/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/adapters/repository.py` & `terka-1.3.2/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/collaborators.py` & `terka-1.3.2/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/commands.py` & `terka-1.3.2/src/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/commentary.py` & `terka-1.3.2/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/epic.py` & `terka-1.3.2/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/event_history.py` & `terka-1.3.2/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/project.py` & `terka-1.3.2/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/sprint.py` & `terka-1.3.2/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/story.py` & `terka-1.3.2/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/tag.py` & `terka-1.3.2/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/task.py` & `terka-1.3.2/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/time_tracker.py` & `terka-1.3.2/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/domain/user.py` & `terka-1.3.2/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/entrypoints/cli.py` & `terka-1.3.2/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/service_layer/printer.py` & `terka-1.3.2/src/service_layer/printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,16 @@
                 if not value:
                     continue
                 elif name in ("created_by", "assignee"):
                     attributes.append(
                         (name, services.lookup_user_name(value, self.repo)))
                 elif name == "project":
                     attributes.append(
-                        (name, services.lookup_project_name(value, self.repo)))
+                        (name,
+                         str(services.lookup_project_name(value, self.repo))))
                 elif hasattr(value, "name"):
                     attributes.append((name, value.name))
                 elif isinstance(value, datetime):
                     attributes.append((name, value.strftime("%Y-%m-%d %H:%M")))
                 elif isinstance(value, set):
                     values = value.pop()
                     attributes.append((name, str(values)))
```

### Comparing `terka-1.3.1/src/service_layer/services.py` & `terka-1.3.2/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/service_layer/ui.py` & `terka-1.3.2/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/service_layer/vertical_layout.css` & `terka-1.3.2/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/src/utils.py` & `terka-1.3.2/src/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/terka.egg-info/PKG-INFO` & `terka-1.3.2/terka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.3.1
+Version: 1.3.2
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.3.1/terka.egg-info/SOURCES.txt` & `terka-1.3.2/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/tests/test_orm.py` & `terka-1.3.2/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/tests/test_task.py` & `terka-1.3.2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.1/tests/test_user.py` & `terka-1.3.2/tests/test_user.py`

 * *Files identical despite different names*

