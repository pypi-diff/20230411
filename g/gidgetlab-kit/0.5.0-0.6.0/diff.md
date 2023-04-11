# Comparing `tmp/gidgetlab-kit-0.5.0.tar.gz` & `tmp/gidgetlab_kit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gidgetlab-kit-0.5.0.tar", last modified: Thu Sep 15 14:35:33 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `gidgetlab-kit-0.5.0.tar` & `gidgetlab_kit-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 14:35:33.040759 gidgetlab-kit-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       99 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      956 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      444 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1079 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3095 2022-09-15 14:35:33.039759 gidgetlab-kit-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2381 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 14:35:33.037759 gidgetlab-kit-0.5.0/gidgetlab_kit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14700 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/api.py
--rw-rw-rw-   0 root         (0) root         (0)     3504 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/clone.py
--rw-rw-rw-   0 root         (0) root         (0)     6237 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/command.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/commits.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/get.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2658 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/producers.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/gidgetlab_kit/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 14:35:33.039759 gidgetlab-kit-0.5.0/gidgetlab_kit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3095 2022-09-15 14:35:32.000000 gidgetlab-kit-0.5.0/gidgetlab_kit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      627 2022-09-15 14:35:33.000000 gidgetlab-kit-0.5.0/gidgetlab_kit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 14:35:32.000000 gidgetlab-kit-0.5.0/gidgetlab_kit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2022-09-15 14:35:32.000000 gidgetlab-kit-0.5.0/gidgetlab_kit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      101 2022-09-15 14:35:32.000000 gidgetlab-kit-0.5.0/gidgetlab_kit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-09-15 14:35:32.000000 gidgetlab-kit-0.5.0/gidgetlab_kit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      188 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-15 14:35:33.040759 gidgetlab-kit-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1324 2022-09-15 14:35:20.000000 gidgetlab-kit-0.5.0/setup.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/.flake8
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/MANIFEST.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/__init__.py
+-rw-r--r--   0        0        0    14700 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/api.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/clone.py
+-rw-r--r--   0        0        0     6634 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/command.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/commits.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/exceptions.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/get.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/models.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/pipelines.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/producers.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/tasks.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/gidgetlab_kit/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/test_api.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/test_clone.py
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/test_command.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/test_commits.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/test_models.py
+-rw-r--r--   0        0        0    10980 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/test_pipelines.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/test_util.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/utils.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/groups_id.json
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/groups_id_subgroup.json
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/project_from_pipeline_event.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/project_from_tag_push_event.json
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/project_null_description.json
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/project_tags.json
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/projects_empty.json
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/projects_id_auth.json
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/projects_id_no_auth.json
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/projects_id_subgroup.json
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/tests/samples/subgroup.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/README.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 gidgetlab_kit-0.6.0/PKG-INFO
```

### Comparing `gidgetlab-kit-0.5.0/.gitlab-ci.yml` & `gidgetlab_kit-0.6.0/.gitlab-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -26,37 +26,29 @@
   script:
     - python -m build
   artifacts:
     expire_in: 1 day
     paths:
       - dist/
 
-.test:
+run-pytest:
   stage: test
+  image: python:$PYTHON_VERSION
   before_script:
     - pip install .[tests]
   script:
     - pytest -v --junitxml=report.xml --cov=gidgetlab_kit tests
+  parallel:
+    matrix:
+      - PYTHON_VERSION: ["3.8", "3.9", "3.10", "3.11"]
   artifacts:
     when: always
     reports:
       junit: report.xml
 
-test-python38:
-  extends: .test
-  image: python:3.8
-
-test-python39:
-  extends: .test
-  image: python:3.9
-
-test-python310:
-  extends: .test
-  image: python:3.10
-
 release-pypi-package:
   stage: release
   before_script:
     - pip install twine
   script:
     - twine upload dist/*
   only:
```

### Comparing `gidgetlab-kit-0.5.0/LICENSE` & `gidgetlab_kit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/README.md` & `gidgetlab_kit-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/api.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/api.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/clone.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/clone.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/command.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,26 +143,39 @@
         help="Number of projects to trigger. Set to 0 to trigger all projects from the group.",
     ),
     random: bool = typer.Option(
         False,
         help="Randomly pick the projects. Select the oldest that were triggered otherwise.",
     ),
     exclude: List[str] = typer.Option(
-        [],
-        help="Project to exclude (path with basename)",
+        None,
+        help=(
+            "Project to exclude (path with basename). "
+            "This is to exclude very specific project(s). To use regex, use include instead."
+        ),
+    ),
+    include: Optional[str] = typer.Option(
+        None,
+        help="regex that should match the name of projects to include (using re.search).",
     ),
     description: str = typer.Option(
         "gidgetlab",
         help="Pipeline trigger description",
     ),
 ):
     """Trigger the pipeline for all or a subset of projects from group"""
     asyncio.run(
         run_trigger_group_pipelines(
-            state["gl"], group, nb_projects, random, description, exclude
+            state["gl"],
+            group,
+            nb_projects,
+            is_random=random,
+            description=description,
+            exclude=exclude,
+            include=include,
         )
     )
 
 
 @app.command()
 def commit_file(
     filepath: Path = typer.Argument(..., help="Local file to add or update"),
```

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/commits.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/commits.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/get.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/get.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/models.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/models.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/pipelines.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import random
+import re
 import typer
 from operator import itemgetter
-from typing import List
+from typing import List, Optional
 from dateutil.parser import parse
 from dateutil.tz import UTC
 from gidgetlab.abc import GitLabAPI
 from .models import GitLabId, Project
 from . import api
 
 
@@ -40,29 +41,36 @@
 async def run_trigger_group_pipelines(
     gl: GitLabAPI,
     group: GitLabId,
     nb_projects: int,
     is_random: bool = False,
     description: str = "gidgetlab",
     exclude: List[str] = [],
+    include: Optional[str] = None,
 ) -> None:
     """Trigger the pipeline for the group projects
 
     When greater than 0, nb_projects allows to select a subset of the projects.
     If is_random is true, projects are picked randomly. If not, the ones with
     the oldest pipeline execution are selected.
     Some projects can be excluded based on the path with namespace.
+    You can also filter the projects based on the name using the include regex.
     """
     # Filter out empty project (default_branch is None) and excluded one
     projects = [
         project
         async for project in api.get_all_projects(gl, group)
         if project.default_branch is not None
         and project.path_with_namespace not in exclude
     ]
+    if include is not None:
+        pattern = re.compile(include)
+        projects = [
+            project for project in projects if pattern.search(project.name) is not None
+        ]
     if nb_projects == 0 or nb_projects >= len(projects):
         sampled = projects
     else:
         if is_random:
             sampled = random.sample(projects, nb_projects)
         else:
             sorted_projects = await sort_projects_by_pipeline_date(gl, projects)
```

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/producers.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/producers.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/tasks.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/tasks.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-kit-0.5.0/gidgetlab_kit/util.py` & `gidgetlab_kit-0.6.0/gidgetlab_kit/util.py`

 * *Files identical despite different names*

