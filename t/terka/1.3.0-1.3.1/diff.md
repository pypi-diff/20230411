# Comparing `tmp/terka-1.3.0.tar.gz` & `tmp/terka-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.3.0.tar", last modified: Sat Apr  8 10:40:32 2023, max compression
+gzip compressed data, was "terka-1.3.1.tar", last modified: Tue Apr 11 15:41:37 2023, max compression
```

## Comparing `terka-1.3.0.tar` & `terka-1.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.736535 terka-1.3.0/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.3.0/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-08 10:40:32.736535 terka-1.3.0/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.3.0/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-08 10:40:32.736535 terka-1.3.0/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-08 10:39:03.000000 terka-1.3.0/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.732535 terka-1.3.0/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.0/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.732535 terka-1.3.0/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.0/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    13439 2023-04-08 10:39:03.000000 terka-1.3.0/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.3.0/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.732535 terka-1.3.0/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.0/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.3.0/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    32573 2023-04-08 10:39:03.000000 terka-1.3.0/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)      827 2023-03-06 19:56:41.000000 terka-1.3.0/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.3.0/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.3.0/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.3.0/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.3.0/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.3.0/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.3.0/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.3.0/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.3.0/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.3.0/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.3.0/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.3.0/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.732535 terka-1.3.0/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.3.0/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     3978 2023-04-08 10:39:03.000000 terka-1.3.0/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.732535 terka-1.3.0/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.0/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    26342 2023-04-08 10:39:03.000000 terka-1.3.0/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2283 2023-01-26 19:46:39.000000 terka-1.3.0/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.3.0/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.3.0/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     6764 2023-04-08 10:39:03.000000 terka-1.3.0/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.732535 terka-1.3.0/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-08 10:40:32.000000 terka-1.3.0/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-08 10:40:32.000000 terka-1.3.0/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-08 10:40:32.000000 terka-1.3.0/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-08 10:40:32.000000 terka-1.3.0/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-08 10:40:32.000000 terka-1.3.0/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-08 10:40:32.000000 terka-1.3.0/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-08 10:40:32.732535 terka-1.3.0/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.0/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.3.0/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.3.0/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.3.0/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.3.0/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.3.0/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.3.0/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.3.1/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:41:37.595610 terka-1.3.1/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.3.1/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-11 15:41:37.595610 terka-1.3.1/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-11 15:39:33.000000 terka-1.3.1/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.591610 terka-1.3.1/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.591610 terka-1.3.1/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    13439 2023-04-08 10:39:03.000000 terka-1.3.1/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.3.1/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.3.1/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    32550 2023-04-08 19:16:35.000000 terka-1.3.1/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)      827 2023-03-06 19:56:41.000000 terka-1.3.1/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.3.1/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.3.1/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.3.1/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.3.1/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.3.1/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.3.1/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.3.1/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.3.1/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.3.1/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.3.1/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.3.1/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.3.1/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.3.1/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    26661 2023-04-11 15:37:18.000000 terka-1.3.1/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.3.1/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.3.1/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.3.1/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     6764 2023-04-08 10:39:03.000000 terka-1.3.1/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-11 15:41:37.000000 terka-1.3.1/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-11 15:41:37.595610 terka-1.3.1/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.3.1/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.3.1/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.3.1/tests/test_utils.py
```

### Comparing `terka-1.3.0/LICENSE` & `terka-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/PKG-INFO` & `terka-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.3.0
+Version: 1.3.1
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.3.0/README.md` & `terka-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/setup.py` & `terka-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.3.0",
+    version="1.3.1",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.3.0/src/adapters/orm.py` & `terka-1.3.1/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/adapters/repository.py` & `terka-1.3.1/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/collaborators.py` & `terka-1.3.1/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/commands.py` & `terka-1.3.1/src/domain/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from src.domain.time_tracker import TimeTrackerEntry
 from src.domain.epic import Epic, EpicTask
 from src.domain.story import Story, StoryTask
 
 from src.service_layer import services, printer
 from src.service_layer.ui import TerkaTask
 from src.adapters.repository import AbsRepository
-from src.utils import format_command
+from src.utils import format_command, format_task_dict
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CurrentEntry:
     value: str
@@ -169,14 +169,15 @@
 
     def __init__(self, repo: AbsRepository):
         self.repo = repo
         self.handler = self._init_handlers()
         self.home_dir = os.path.expanduser('~')
         self.printer = printer.Printer(repo)
         self.console = Console()
+        self.config = self._read_config()
 
     def _init_handlers(self):
         handler_chain = BaseHandler(None)
         for handler in [
                 TaskHandler, ProjectHandler, UserHandler, TagHandler,
                 SprintHandler, SprintTaskHandler, TimeTrackerHandler,
                 EpicHandler, StoryHandler
@@ -362,44 +363,36 @@
             tail = head[-10:]
             for row in tail[::-1]:
                 info, message = row.split("] ")
                 date, source, level = info.split("][")
                 table.add_row(re.sub("\[", "", date), source, level, message)
             self.console.print(table)
         elif command == "focus":
-            with open(f"{self.home_dir}/.terka/config.yaml",
-                      "r",
-                      encoding="utf-8") as f:
-                config = yaml.safe_load(f)
             if entity_type == "tasks":
-                config["task_id"] = kwargs["id"]
-                if "project_name" in config.keys():
-                    del config["project_name"]
+                self.config["task_id"] = kwargs["id"]
+                if "project_name" in self.config.keys():
+                    del self.config["project_name"]
             if entity_type == "projects":
-                config["project_name"] = kwargs["id"]
-                if "task_id" in config.keys():
-                    del config["task_id"]
+                self.config["project_name"] = kwargs["id"]
+                if "task_id" in self.config.keys():
+                    del self.config["task_id"]
             with open(f"{self.home_dir}/.terka/config.yaml",
                       "w",
                       encoding="utf-8") as f:
-                yaml.dump(config, f)
+                yaml.dump(self.config, f)
             logger.info("<focus> %s: %s", entity_type, "")
         elif command == "unfocus":
-            with open(f"{self.home_dir}/.terka/config.yaml",
-                      "r",
-                      encoding="utf-8") as f:
-                config = yaml.safe_load(f)
-            if "task_id" in config.keys():
-                del config["task_id"]
-            if "project_name" in config.keys():
-                del config["project_name"]
+            if "task_id" in self.config.keys():
+                del self.config["task_id"]
+            if "project_name" in self.config.keys():
+                del self.config["project_name"]
             with open(f"{self.home_dir}/.terka/config.yaml",
                       "w",
                       encoding="utf-8") as f:
-                yaml.dump(config, f)
+                yaml.dump(self.config, f)
             logger.info("<unfocus> %s: %s", entity_type, "")
         elif command == "count":
             entities = self.repo.list(entity, kwargs)
             print(len(entities))
             logger.info("<count> tasks")
         elif command == "collaborate":
             if entity_type == "tasks":
@@ -574,16 +567,15 @@
                             "sprint": obj.sprint
                     }):
                         exit("task already added to sprint")
                     self.repo.add(obj)
             session.commit()
         elif command == "create":
             kwargs["created_by"] = services.lookup_user_id(
-                # config.get("user"),
-                "am",
+                self.config.get("user"),
                 self.repo)
             obj = entity(**kwargs)
             if entity in (Task, Project):
                 if (existing_obj := self.repo.list(entity,
                                                    {"name": obj.name})):
                     print("Found existing entity\n")
                     existing_id = str(existing_obj[0].id)
@@ -758,14 +750,21 @@
                 del kwargs["id"]
                 self.execute("create", "time_entry", kwargs)
             else:
                 exit("tracking missing -H (hours) or -M (minutes) value")
         else:
             raise ValueError(f"Uknown command: {command}")
 
+    def _read_config(self) -> Dict[str, Any]:
+        with open(f"{self.home_dir}/.terka/config.yaml",
+                  "r",
+                  encoding="utf-8") as f:
+            config = yaml.safe_load(f)
+        return config
+
 
 def get_ids(ids: Union[str, int]) -> List[Union[int, str]]:
     id_string = str(ids)
     if "," in id_string:
         ids = id_string.split(",")
     elif ".." in id_string:
         task_range = id_string.split("..")
```

### Comparing `terka-1.3.0/src/domain/commentary.py` & `terka-1.3.1/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/epic.py` & `terka-1.3.1/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/event_history.py` & `terka-1.3.1/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/project.py` & `terka-1.3.1/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/sprint.py` & `terka-1.3.1/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/story.py` & `terka-1.3.1/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/tag.py` & `terka-1.3.1/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/task.py` & `terka-1.3.1/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/time_tracker.py` & `terka-1.3.1/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/domain/user.py` & `terka-1.3.1/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/entrypoints/cli.py` & `terka-1.3.1/src/entrypoints/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from io import StringIO
 import re
 import os
 from operator import attrgetter
 import sys
 import yaml
 import logging
+from pprint import pprint
 
 import rich
 from rich.console import Console
 from rich.table import Table
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker, clear_mappers
 
 from src.adapters.orm import metadata, start_mappers
 from src.adapters.repository import SqlAlchemyRepository
 
 from src.domain.commands import CommandHandler
-from src.utils import format_task_dict, process_command, update_task_dict
+from src.utils import format_task_dict, process_command, update_task_dict, create_task_dict
+from src.service_layer import services
 
 
 def init_db(home_dir):
     engine = create_engine(f"sqlite:////{home_dir}/.terka/tasks.db")
     metadata.create_all(engine)
     return engine
 
@@ -45,14 +47,20 @@
     args = parser.parse_known_args()
     args, kwargs = args
     if args.version:
         import pkg_resources
         version = pkg_resources.require("terka")[0].version
         print(f"terka version {version}")
         exit()
+    if args.command == "config":
+        if "--show" in kwargs:
+            pprint(services.get_config())
+        else:
+            services.update_config(create_task_dict(kwargs))
+        exit()
     home_dir = os.path.expanduser('~')
     logger = logging.getLogger(__name__)
     console = Console()
 
     engine = init_db(home_dir)
     start_mappers()
     Session = sessionmaker(engine)
```

### Comparing `terka-1.3.0/src/service_layer/printer.py` & `terka-1.3.1/src/service_layer/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,21 @@
         if entity_type == "stories":
             if entities:
                 self.print_story(entities, repo)
             else:
                 exit(f"No story with id '{task}' found!")
         if entity_type == "projects":
             if entities:
-                self.print_project(
-                    entities, show_completed_tasks=show_completed)
+                self.print_project(entities,
+                                   show_completed_tasks=show_completed)
             else:
                 exit(f"No project '{task}' found!")
         if entity_type == "tasks":
             if entities:
-                self.print_task(
-                    entities,
-                    repo,
-                    show_completed=show_completed)
+                self.print_task(entities, repo, show_completed=show_completed)
             else:
                 print(f"No task with id '{task}' found!")
 
     def print_entities(self,
                        entities,
                        type,
                        repo,
@@ -144,16 +141,16 @@
                           entity.date.strftime("%Y-%m-%d %H:%M"), entity.text)
         self.console.print(table)
 
     def print_epic(self, entities, repo, show_tasks=True):
         table = Table(box=self.box, title="EPICS", expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
-        tasks = []
         for entity in entities:
+            tasks = []
             for epic_task in entity.epic_tasks:
                 task = epic_task.tasks
                 tasks.append(task)
             try:
                 project_obj = services.lookup_project_name(
                     entity.project, repo)
                 project = project_obj.name
@@ -168,16 +165,16 @@
                             show_completed=True,
                             show_window=False)
 
     def print_story(self, entities, repo, show_tasks=True):
         table = Table(box=self.box, title="STORIES", expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
-        tasks = []
         for entity in entities:
+            tasks = []
             for story_task in entity.story_tasks:
                 task = story_task.tasks
                 tasks.append(task)
             try:
                 project_obj = services.lookup_project_name(
                     entity.project, repo)
                 project = project_obj.name
@@ -194,18 +191,18 @@
 
     def print_sprint(self, entities, repo, show_tasks=True):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "start_date", "end_date", "goal", "status",
                        "open tasks", "tasks", "velocity", "collaborators",
                        "time_spent"):
             table.add_column(column)
-        story_points = []
-        tasks = []
-        collaborators = []
         for entity in entities:
+            story_points = []
+            tasks = []
+            collaborators = []
             collaborators_dict = defaultdict(int)
             for sprint_task in entity.sprint_tasks:
                 story_points.append(sprint_task.story_points)
                 task = sprint_task.tasks
                 tasks.append(task)
                 if task_collaborators := task.collaborators:
                     for collaborator in task.collaborators:
@@ -215,30 +212,30 @@
                     collaborators_dict["Unknown"] += sprint_task.story_points
 
             for user, story_point in sorted(collaborators_dict.items(),
                                             key=lambda x: x[1],
                                             reverse=True):
                 collaborators.append(f"{user} ({story_point})")
 
-            collaborators = ", ".join(collaborators)
+            collaborators_string = ", ".join(collaborators)
             open_tasks = [
                 task for task in tasks
                 if task.status.name not in ("DONE", "DELETED")
             ]
             time_spent_sum = sum([
                 entry.time_spent_minutes for task in tasks
                 for entry in task.time_spent
             ])
 
             time_spent = self._format_time_spent(time_spent_sum)
             table.add_row(str(entity.id), str(entity.start_date),
                           str(entity.end_date), entity.goal,
                           entity.status.name, str(len(open_tasks)),
                           str(len(tasks)), str(sum(story_points)),
-                          collaborators, str(time_spent))
+                          collaborators_string, str(time_spent))
         self.console.print(table)
         if show_tasks:
             self.print_sprint_task(entities=tasks,
                                    repo=repo,
                                    show_completed=True,
                                    story_points=story_points)
 
@@ -545,14 +542,20 @@
     def _get_attributes(self, obj) -> List[Tuple[str, str]]:
         import inspect
         attributes = []
         for name, value in inspect.getmembers(obj):
             if not name.startswith("_") and not inspect.ismethod(value):
                 if not value:
                     continue
+                elif name in ("created_by", "assignee"):
+                    attributes.append(
+                        (name, services.lookup_user_name(value, self.repo)))
+                elif name == "project":
+                    attributes.append(
+                        (name, services.lookup_project_name(value, self.repo)))
                 elif hasattr(value, "name"):
                     attributes.append((name, value.name))
                 elif isinstance(value, datetime):
                     attributes.append((name, value.strftime("%Y-%m-%d %H:%M")))
                 elif isinstance(value, set):
                     values = value.pop()
                     attributes.append((name, str(values)))
```

### Comparing `terka-1.3.0/src/service_layer/ui.py` & `terka-1.3.1/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/service_layer/vertical_layout.css` & `terka-1.3.1/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/src/utils.py` & `terka-1.3.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/terka.egg-info/PKG-INFO` & `terka-1.3.1/terka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.3.0
+Version: 1.3.1
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.3.0/terka.egg-info/SOURCES.txt` & `terka-1.3.1/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/tests/test_orm.py` & `terka-1.3.1/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/tests/test_task.py` & `terka-1.3.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.3.0/tests/test_user.py` & `terka-1.3.1/tests/test_user.py`

 * *Files identical despite different names*

