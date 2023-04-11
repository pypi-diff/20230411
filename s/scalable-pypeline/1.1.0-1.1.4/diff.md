# Comparing `tmp/scalable-pypeline-1.1.0.tar.gz` & `tmp/scalable-pypeline-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalable-pypeline-1.1.0.tar", last modified: Mon Apr 10 16:07:28 2023, max compression
+gzip compressed data, was "scalable-pypeline-1.1.4.tar", last modified: Tue Apr 11 15:11:42 2023, max compression
```

## Comparing `scalable-pypeline-1.1.0.tar` & `scalable-pypeline-1.1.4.tar`

### file list

```diff
@@ -1,69 +1,45 @@
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.873737 scalable-pypeline-1.1.0/
--rw-r--r--   0 santiago   (501) staff       (20)    10174 2023-03-07 16:04:45.000000 scalable-pypeline-1.1.0/LICENSE
--rw-r--r--   0 santiago   (501) staff       (20)       90 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/MANIFEST.in
--rw-r--r--   0 santiago   (501) staff       (20)     4735 2023-04-10 16:07:28.873862 scalable-pypeline-1.1.0/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)     4270 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/README.md
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.858676 scalable-pypeline-1.1.0/pypeline/
--rw-r--r--   0 santiago   (501) staff       (20)       22 2023-04-10 15:29:50.000000 scalable-pypeline-1.1.0/pypeline/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)    11491 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/celery.py
--rw-r--r--   0 santiago   (501) staff       (20)    10759 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/celery_beat.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.860196 scalable-pypeline-1.1.0/pypeline/cli/
--rw-r--r--   0 santiago   (501) staff       (20)        0 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/cli/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)     1744 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/cli/config_server.py
--rw-r--r--   0 santiago   (501) staff       (20)     1097 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/cli/core.py
--rw-r--r--   0 santiago   (501) staff       (20)     5323 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/cli/deploy.py
--rw-r--r--   0 santiago   (501) staff       (20)     3031 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/cloud.py
--rw-r--r--   0 santiago   (501) staff       (20)     5589 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/constants.py
--rw-r--r--   0 santiago   (501) staff       (20)     6636 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/deploy.py
--rw-r--r--   0 santiago   (501) staff       (20)      599 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/extensions.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.861247 scalable-pypeline-1.1.0/pypeline/flask/
--rw-r--r--   0 santiago   (501) staff       (20)      782 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/flask/__init__.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.862573 scalable-pypeline-1.1.0/pypeline/flask/api/
--rw-r--r--   0 santiago   (501) staff       (20)        0 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/flask/api/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)     8325 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/flask/api/pipelines.py
--rw-r--r--   0 santiago   (501) staff       (20)     2327 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/flask/api/schedules.py
--rw-r--r--   0 santiago   (501) staff       (20)     1389 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/flask/api/utils.py
--rw-r--r--   0 santiago   (501) staff       (20)     2811 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/flask/decorators.py
--rw-r--r--   0 santiago   (501) staff       (20)     8729 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/flask/flask_sermos.py
--rw-r--r--   0 santiago   (501) staff       (20)     6776 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/generators.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.863183 scalable-pypeline-1.1.0/pypeline/lib/
--rw-r--r--   0 santiago   (501) staff       (20)        0 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/lib/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)     5303 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/lib/config_server.py
--rw-r--r--   0 santiago   (501) staff       (20)     5503 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/logging_config.py
--rw-r--r--   0 santiago   (501) staff       (20)     6763 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/pipeline_config_schema.py
--rw-r--r--   0 santiago   (501) staff       (20)     7385 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/schedule_config_schema.py
--rw-r--r--   0 santiago   (501) staff       (20)    29081 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/sermos_yaml.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.864822 scalable-pypeline-1.1.0/pypeline/utils/
--rw-r--r--   0 santiago   (501) staff       (20)        0 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/utils/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)    13092 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/utils/config_utils.py
--rw-r--r--   0 santiago   (501) staff       (20)     4642 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/utils/graph_utils.py
--rw-r--r--   0 santiago   (501) staff       (20)     4166 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/utils/module_utils.py
--rw-r--r--   0 santiago   (501) staff       (20)    33793 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/pypeline/utils/task_utils.py
--rw-r--r--   0 santiago   (501) staff       (20)      448 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/requirements.txt
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.866991 scalable-pypeline-1.1.0/scalable_pypeline.egg-info/
--rw-r--r--   0 santiago   (501) staff       (20)     4735 2023-04-10 16:07:28.000000 scalable-pypeline-1.1.0/scalable_pypeline.egg-info/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)     1546 2023-04-10 16:07:28.000000 scalable-pypeline-1.1.0/scalable_pypeline.egg-info/SOURCES.txt
--rw-r--r--   0 santiago   (501) staff       (20)        1 2023-04-10 16:07:28.000000 scalable-pypeline-1.1.0/scalable_pypeline.egg-info/dependency_links.txt
--rw-r--r--   0 santiago   (501) staff       (20)       56 2023-04-10 16:07:28.000000 scalable-pypeline-1.1.0/scalable_pypeline.egg-info/entry_points.txt
--rw-r--r--   0 santiago   (501) staff       (20)      613 2023-04-10 16:07:28.000000 scalable-pypeline-1.1.0/scalable_pypeline.egg-info/requires.txt
--rw-r--r--   0 santiago   (501) staff       (20)       15 2023-04-10 16:07:28.000000 scalable-pypeline-1.1.0/scalable_pypeline.egg-info/top_level.txt
--rw-r--r--   0 santiago   (501) staff       (20)      100 2023-04-10 16:07:28.874392 scalable-pypeline-1.1.0/setup.cfg
--rw-r--r--   0 santiago   (501) staff       (20)     6649 2023-04-10 16:07:23.000000 scalable-pypeline-1.1.0/setup.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.872692 scalable-pypeline-1.1.0/tests/
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2023-04-10 16:07:28.873465 scalable-pypeline-1.1.0/tests/fixtures/
--rw-r--r--   0 santiago   (501) staff       (20)       41 2023-03-07 16:04:45.000000 scalable-pypeline-1.1.0/tests/fixtures/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)     1694 2023-03-07 16:04:45.000000 scalable-pypeline-1.1.0/tests/fixtures/s3_fixtures.py
--rw-r--r--   0 santiago   (501) staff       (20)      290 2023-03-07 16:04:45.000000 scalable-pypeline-1.1.0/tests/test_celery.py
--rw-r--r--   0 santiago   (501) staff       (20)     3709 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_flask_decorators.py
--rw-r--r--   0 santiago   (501) staff       (20)      626 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_flask_sermos.py
--rw-r--r--   0 santiago   (501) staff       (20)     1459 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_pipelines.py
--rw-r--r--   0 santiago   (501) staff       (20)     2040 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_schedule_config.py
--rw-r--r--   0 santiago   (501) staff       (20)      984 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_sermos_cli_tools.py
--rw-r--r--   0 santiago   (501) staff       (20)     8180 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_sermos_deploy.py
--rw-r--r--   0 santiago   (501) staff       (20)     2104 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_sermos_utils.py
--rw-r--r--   0 santiago   (501) staff       (20)    12838 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_sermos_yaml.py
--rw-r--r--   0 santiago   (501) staff       (20)     2139 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_utils_api.py
--rw-r--r--   0 santiago   (501) staff       (20)     9363 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_utils_config.py
--rw-r--r--   0 santiago   (501) staff       (20)     4940 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_utils_graph.py
--rw-r--r--   0 santiago   (501) staff       (20)     2675 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_utils_module.py
--rw-r--r--   0 santiago   (501) staff       (20)    17173 2023-04-10 14:55:06.000000 scalable-pypeline-1.1.0/tests/test_utils_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.604842 scalable-pypeline-1.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 15:11:42.605842 scalable-pypeline-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.598841 scalable-pypeline-1.1.4/pypeline/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10759 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/celery_beat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/extensions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.599841 scalable-pypeline-1.1.4/pypeline/flask/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.600842 scalable-pypeline-1.1.4/pypeline/flask/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8325 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2327 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/schedules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5842 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/flask_sermos.py
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/logging_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6763 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/pipeline_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7385 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/schedule_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    29081 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/sermos_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.602842 scalable-pypeline-1.1.4/pypeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13029 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/config_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/graph_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/module_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    33793 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/task_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.604842 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      562 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-11 15:11:42.605842 scalable-pypeline-1.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6428 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.592841 scalable-pypeline-1.1.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.604842 scalable-pypeline-1.1.4/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/tests/fixtures/s3_fixtures.py
```

### Comparing `scalable-pypeline-1.1.0/LICENSE` & `scalable-pypeline-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/PKG-INFO` & `scalable-pypeline-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.1.0
+Version: 1.1.4
 Summary: PypeLine - Python pipelines for the Real World
-Home-page: https://gitlab.com/bravos2/pype-line
+Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
-Provides-Extra: cli
 Provides-Extra: flask
-Provides-Extra: flask_auth
 Provides-Extra: web
 Provides-Extra: workers
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # PypeLine
```

### Comparing `scalable-pypeline-1.1.0/README.md` & `scalable-pypeline-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/celery.py` & `scalable-pypeline-1.1.4/pypeline/celery.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/celery_beat.py` & `scalable-pypeline-1.1.4/pypeline/celery_beat.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/extensions.py` & `scalable-pypeline-1.1.4/pypeline/extensions.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/flask/api/pipelines.py` & `scalable-pypeline-1.1.4/pypeline/flask/api/pipelines.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/flask/api/schedules.py` & `scalable-pypeline-1.1.4/pypeline/flask/api/schedules.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/flask/api/utils.py` & `scalable-pypeline-1.1.4/pypeline/flask/api/utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/flask/decorators.py` & `scalable-pypeline-1.1.4/pypeline/flask/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,38 +2,23 @@
 """
 import os
 import logging
 from http import HTTPStatus
 from functools import wraps
 import requests
 from rhodb.redis_conf import RedisConnector
-from flask import current_app, request
+from flask import request
 from rho_web.response import abort
-from pypeline.flask import oidc
 from pypeline.constants import DEFAULT_AUTH_URL, AUTH_LOCK_KEY, \
     AUTH_LOCK_DURATION, USING_SERMOS_CLOUD
 
 logger = logging.getLogger(__name__)
 redis_conn = RedisConnector().get_connection()
 
 
-def require_login(fn):
-    """ Utilize Flask RhoAuth to secure a route with @require_login decorator
-    """
-    secure_fn = oidc.require_login(fn)
-
-    @wraps(fn)
-    def decorated(*args, **kwargs):
-        if str(current_app.config['RHOAUTH_ENABLED']).lower() == 'true':
-            return secure_fn(*args, **kwargs)
-        return fn(*args, **kwargs)
-
-    return decorated
-
-
 def validate_access_key(access_key: str = None):
     """ Verify whether an Access Key is valid according to Sermos Cloud.
 
     If deploying in 'local' mode, no validation is done. To deploy in local
     mode, set DEFAULT_BASE_URL=local in your environment.
     """
     # Always 'valid' in local mode
@@ -45,15 +30,14 @@
     access_key = os.environ.get('SERMOS_ACCESS_KEY', access_key)
 
     # Invalid if None, no need to ask.
     if access_key is None:
         return False
 
     # Ask cache first
-    # TODO update to remove Redis as a dependency, merely an optional feature.
     validated = redis_conn.get(AUTH_LOCK_KEY)
     if validated is not None:
         return True
 
     # Ask Sermos Cloud (Note: Sermos Cloud's API expects `apikey`)
     headers = {'apikey': access_key}
     r = requests.post(DEFAULT_AUTH_URL, headers=headers, verify=True)
```

### Comparing `scalable-pypeline-1.1.0/pypeline/flask/flask_sermos.py` & `scalable-pypeline-1.1.4/pypeline/flask/flask_sermos.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 """
 import os
 if os.getenv('USE_GEVENT', 'false').lower() == 'true':
     import gevent.monkey
     gevent.monkey.patch_all()
 
 import logging
-from functools import partial
 from flask import Flask
 from werkzeug.middleware.proxy_fix import ProxyFix
 from rho_web.smorest import Api, Blueprint
-from pypeline.utils.task_utils import TaskRunner, PipelineResult
 from pypeline.logging_config import setup_logging
 from pypeline.extensions import sermos_config
-from pypeline.flask import oidc
-from pypeline.constants import DEFAULT_OPENAPI_CONFIG, DEFAULT_RHOAUTH_CONFIG
+from pypeline.constants import DEFAULT_OPENAPI_CONFIG
 from pypeline import __version__
 
 logger = logging.getLogger(__name__)
 
 
 class FlaskSermos:
     """ Sermos Flask extension.
@@ -34,15 +31,14 @@
 
     def init_app(self, app: Flask, init_api: bool = False):
         """ Sermos bootstrapping process.
 
         Application config variables to set include:
 
             SERMOS_CLIENT_VERSION (default: v?.?.?)
-            RHOAUTH_ENABLED (default: True)
             SERMOS_HIJACK_ROOT_LOGGER (default: False)
 
         Optional, if `init_api` is True:
 
             API_DOCUMENTATION_TITLE
             API_DOCUMENTATION_DESCRIPTION
             OPENAPI_VERSION
@@ -66,79 +62,29 @@
                 documentation for additional configuration options.
         """
         # Ensure there's a SERMOS_CLIENT_VERSION on app config
         app.config.setdefault(
             'SERMOS_CLIENT_VERSION',
             app.config.get("SERMOS_CLIENT_VERSION", "v?.?.?"))
 
-        # Bootstrap logging if app requests
-        self._bootstrap_logging(app)
-
         app.wsgi_app = ProxyFix(app.wsgi_app)
         app.url_map.strict_slashes = False
 
         # Create and register the sermos blueprint
         bp = Blueprint('sermos',
                        __name__,
                        template_folder='../templates',
                        static_folder='../static',
                        url_prefix='/sermos')
         app.register_blueprint(bp)
 
-        # Bootstrap RhoAuth if app requests
-        self._bootstrap_rhoauth(app)
-
         # Bootstrap api if app requests
         if init_api is True:
             self._bootstrap_api(app)
 
-    def _bootstrap_rhoauth(self, app: Flask):
-        """ If RHOAUTH_ENABLED is True, bootstrap the application with default
-            configuration, precedent given to the provide app.
-        """
-        # TODO Remove rhoauth by default and/or entirely in future release.
-        rhoauth_enabled = str(app.config.get('RHOAUTH_ENABLED',
-                                             True)).lower() == 'true'
-        app.config.setdefault('RHOAUTH_ENABLED', rhoauth_enabled)
-        if rhoauth_enabled is True:
-            # Set useful defaults so users don't need to request.
-            for rhoauth_config in DEFAULT_RHOAUTH_CONFIG:
-                app.config.setdefault(
-                    rhoauth_config[0],
-                    app.config.get(rhoauth_config[0], rhoauth_config[1]))
-
-        # Initialize open id connect for authentication
-        if rhoauth_enabled is True:
-            logger.info("Initializing using RhoAuth ...")
-            self.oidc = oidc
-            self.oidc.init_app(app)
-
-            @app.route('/logout')
-            def logout():
-                return self.oidc.logout("/")
-
-    @staticmethod
-    def _bootstrap_logging(app: Flask):
-        """ If application requests Sermos logging, enable here
-
-            Main reason to do this is to have clear versioning in each log
-            and to supress the elasticsearch log level by default, which is
-            extremely verbose if using elasticsearch-py. There is no dependency
-            on elasticsearch - we simply create the logger and upgrade level
-            because it's extremely annoying if you do need to use ES.
-        """
-        if app.config.get('SERMOS_HIJACK_ROOT_LOGGER', False):
-            overload_es = app.config.get('OVERLOAD_ES_LOGGING', True)
-            logger.info("Initializing using Sermos logging ...")
-            setup_logging(app_version=__version__,
-                          client_version=app.config['SERMOS_CLIENT_VERSION'],
-                          default_level=app.config.get("LOG_LEVEL", "INFO"),
-                          overload_elasticsearch=overload_es,
-                          establish_logging_config=True)
-
     def _bootstrap_api(self, app: Flask):
         """ If initializing the API, we will create the core Sermos API paths
             and initialize the default Swagger documentation.
         """
         # Set sensible defaults for Swagger docs. Provided `app` will
         # take precedent.
         for swagger_config in DEFAULT_OPENAPI_CONFIG:
@@ -183,23 +129,15 @@
             'title': app.config['API_DOCUMENTATION_TITLE'],
             'version': f"Sermos: {__version__} - "
             f"Client: {app.config['SERMOS_CLIENT_VERSION']}",
             'description': app.config['API_DOCUMENTATION_DESCRIPTION'],
             'tags': tags
         }
         try:
-            # Initialize the API documentation and ensure RhoAuth validates
-            # correct `role`
-            if str(app.config['RHOAUTH_ENABLED']).lower() == 'true':
-                decorator = partial(self.oidc.require_login,
-                                    roles=['sermos-client-api-docs'])
-                api = Api(auth_decorator=decorator)
-            else:
-                api = Api()
-
+            api = Api()
             api.init_app(app, spec_kwargs=spec_kwargs)
 
             # Register available Sermos API Namespaces
             self._register_api_namespaces(api)
 
         except Exception as e:
             api = None
```

### Comparing `scalable-pypeline-1.1.0/pypeline/generators.py` & `scalable-pypeline-1.1.4/pypeline/generators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/logging_config.py` & `scalable-pypeline-1.1.4/pypeline/logging_config.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/pipeline_config_schema.py` & `scalable-pypeline-1.1.4/pypeline/pipeline_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/schedule_config_schema.py` & `scalable-pypeline-1.1.4/pypeline/schedule_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/sermos_yaml.py` & `scalable-pypeline-1.1.4/pypeline/sermos_yaml.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/utils/config_utils.py` & `scalable-pypeline-1.1.4/pypeline/utils/config_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from urllib.parse import urljoin
 import requests
 from rhodb.redis_conf import RedisConnector
 from pypeline.constants import DEFAULT_BASE_URL, PIPELINE_CONFIG_CACHE_KEY, \
     SCHEDULE_CONFIG_CACHE_KEY, CONFIG_REFRESH_RATE, USING_SERMOS_CLOUD, \
     LOCAL_DEPLOYMENT_VALUE, DEFAULT_CONFIG_RETRIEVAL_PAGE_SIZE
 from pypeline.sermos_yaml import load_sermos_config
-from pypeline.pipeline_config_schema import BasePipelineSchema
 from pypeline.schedule_config_schema import BaseScheduleSchema
 
 logger = logging.getLogger(__name__)
 redis_conn = RedisConnector().get_connection()
 
 
 def get_access_key(access_key: Union[str, None] = None,
```

### Comparing `scalable-pypeline-1.1.0/pypeline/utils/graph_utils.py` & `scalable-pypeline-1.1.4/pypeline/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/utils/module_utils.py` & `scalable-pypeline-1.1.4/pypeline/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/pypeline/utils/task_utils.py` & `scalable-pypeline-1.1.4/pypeline/utils/task_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.0/scalable_pypeline.egg-info/PKG-INFO` & `scalable-pypeline-1.1.4/scalable_pypeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.1.0
+Version: 1.1.4
 Summary: PypeLine - Python pipelines for the Real World
-Home-page: https://gitlab.com/bravos2/pype-line
+Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
-Provides-Extra: cli
 Provides-Extra: flask
-Provides-Extra: flask_auth
 Provides-Extra: web
 Provides-Extra: workers
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # PypeLine
```

### Comparing `scalable-pypeline-1.1.0/scalable_pypeline.egg-info/SOURCES.txt` & `scalable-pypeline-1.1.4/scalable_pypeline.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,56 +3,34 @@
 README.md
 requirements.txt
 setup.cfg
 setup.py
 pypeline/__init__.py
 pypeline/celery.py
 pypeline/celery_beat.py
-pypeline/cloud.py
 pypeline/constants.py
-pypeline/deploy.py
 pypeline/extensions.py
 pypeline/generators.py
 pypeline/logging_config.py
 pypeline/pipeline_config_schema.py
 pypeline/schedule_config_schema.py
 pypeline/sermos_yaml.py
-pypeline/cli/__init__.py
-pypeline/cli/config_server.py
-pypeline/cli/core.py
-pypeline/cli/deploy.py
 pypeline/flask/__init__.py
 pypeline/flask/decorators.py
 pypeline/flask/flask_sermos.py
 pypeline/flask/api/__init__.py
 pypeline/flask/api/pipelines.py
 pypeline/flask/api/schedules.py
 pypeline/flask/api/utils.py
-pypeline/lib/__init__.py
-pypeline/lib/config_server.py
 pypeline/utils/__init__.py
 pypeline/utils/config_utils.py
 pypeline/utils/graph_utils.py
 pypeline/utils/module_utils.py
 pypeline/utils/task_utils.py
 scalable_pypeline.egg-info/PKG-INFO
 scalable_pypeline.egg-info/SOURCES.txt
 scalable_pypeline.egg-info/dependency_links.txt
 scalable_pypeline.egg-info/entry_points.txt
 scalable_pypeline.egg-info/requires.txt
 scalable_pypeline.egg-info/top_level.txt
-tests/test_celery.py
-tests/test_flask_decorators.py
-tests/test_flask_sermos.py
-tests/test_pipelines.py
-tests/test_schedule_config.py
-tests/test_sermos_cli_tools.py
-tests/test_sermos_deploy.py
-tests/test_sermos_utils.py
-tests/test_sermos_yaml.py
-tests/test_utils_api.py
-tests/test_utils_config.py
-tests/test_utils_graph.py
-tests/test_utils_module.py
-tests/test_utils_task.py
 tests/fixtures/__init__.py
 tests/fixtures/s3_fixtures.py
```

### Comparing `scalable-pypeline-1.1.0/scalable_pypeline.egg-info/requires.txt` & `scalable-pypeline-1.1.4/scalable_pypeline.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 PyYAML<6,>=5.2
+click==8.0.4
 marshmallow<4,>=3.2.1
-click
 requests>=2.24.0
-redis==3.3.11
+redis<5,>=4.5.4
 rhodb[redis]<6,>=5.1.1
 attrs<20,>=19
 boto3<2,>=1.11
 croniter<2,>=1.0.15
 celery-dyrygent==0.8.0
 itsdangerous==2.0.1
 
 [build]
 wheel
 twine
 
-[cli]
-celery==5.1.2
-
 [dev]
 honcho>=1.0.1
 awscli>=1.11
 pylint>=2.5.3
 pip-licenses
 
 [flask]
 Flask>=1.1.1
 rho-web[smorest]>=0.3.3
 flask-smorest>=0.23.0
 
-[flask_auth]
-Flask-RhoAuth[openid]>=2.2.1
-
 [test]
 pytest-cov<3,>=2.6.1
 tox<4,>=3.14.1
 mock<2,>=1
 moto<2,>=1.3.16
 responses<0.11,>=0.10.16
-fakeredis==1.0.5
+fakeredis<3,>=2.10.3
 importlib-metadata<5,>=4.12
 
 [web]
 gunicorn
 gevent
 
 [workers]
```

### Comparing `scalable-pypeline-1.1.0/setup.py` & `scalable-pypeline-1.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -153,44 +153,38 @@
     name='scalable-pypeline',
     version=__version__,
     description="PypeLine - Python pipelines for the Real World",
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     author="Bravos Power Corporation",
     license="Apache License 2.0",
-    url="https://gitlab.com/bravos2/pype-line",
+    url="https://gitlab.com/bravos2/pypeline",
     packages=packages,
     include_package_data=True,
     cmdclass=cmdclass,
     ext_modules=ext_modules,
     install_requires=install_requires,
     extras_require={
         'build': ['wheel', 'twine'],
-        'cli': [
-            # TODO Need to address celery dependency, same as under `deploy`
-            # and `workers` extras
-            'celery==5.1.2'
-        ],
         # TODO: decouple rho-web & Flask-RhoAuth
         'flask':
         ['Flask>=1.1.1', 'rho-web[smorest]>=0.3.3', 'flask-smorest>=0.23.0'],
-        'flask_auth': ['Flask-RhoAuth[openid]>=2.2.1'],
         'web': ['gunicorn', 'gevent'],
         'workers': [
             'celery[redis]==5.1.2',
             'networkx>=2.4',
         ],
         'dev':['honcho>=1.0.1', 'awscli>=1.11', 'pylint>=2.5.3', 'pip-licenses'],
         'test': [
             'pytest-cov>=2.6.1,<3',
             'tox>=3.14.1,<4',
             'mock>=1,<2',
             'moto>=1.3.16,<2',
             'responses>=0.10.16,<0.11',
-            'fakeredis==1.0.5',
+            'fakeredis>=2.10.3,<3',
             'importlib-metadata>=4.12,<5'
         ]
     },
     entry_points="""
     [console_scripts]
     pypeline=pypeline.cli.core:pypeline
     """,
```

### Comparing `scalable-pypeline-1.1.0/tests/fixtures/s3_fixtures.py` & `scalable-pypeline-1.1.4/tests/fixtures/s3_fixtures.py`

 * *Files identical despite different names*

