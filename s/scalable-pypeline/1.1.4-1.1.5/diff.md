# Comparing `tmp/scalable-pypeline-1.1.4.tar.gz` & `tmp/scalable-pypeline-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalable-pypeline-1.1.4.tar", last modified: Tue Apr 11 15:11:42 2023, max compression
+gzip compressed data, was "scalable-pypeline-1.1.5.tar", last modified: Tue Apr 11 21:01:59 2023, max compression
```

## Comparing `scalable-pypeline-1.1.4.tar` & `scalable-pypeline-1.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.604842 scalable-pypeline-1.1.4/
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 15:11:42.605842 scalable-pypeline-1.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4270 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.598841 scalable-pypeline-1.1.4/pypeline/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11491 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10759 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/celery_beat.py
--rw-rw-rw-   0 root         (0) root         (0)     4185 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/extensions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.599841 scalable-pypeline-1.1.4/pypeline/flask/
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.600842 scalable-pypeline-1.1.4/pypeline/flask/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8325 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2327 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/schedules.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5842 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/flask/flask_sermos.py
--rw-rw-rw-   0 root         (0) root         (0)     6776 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     5503 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/logging_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6763 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/pipeline_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7385 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/schedule_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    29081 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/sermos_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.602842 scalable-pypeline-1.1.4/pypeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13029 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/config_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/graph_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/module_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    33793 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/pypeline/utils/task_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.604842 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      562 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-11 15:11:42.000000 scalable-pypeline-1.1.4/scalable_pypeline.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-11 15:11:42.605842 scalable-pypeline-1.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6428 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.592841 scalable-pypeline-1.1.4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:11:42.604842 scalable-pypeline-1.1.4/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2023-04-11 15:11:21.000000 scalable-pypeline-1.1.4/tests/fixtures/s3_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.854206 scalable-pypeline-1.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 21:01:59.854206 scalable-pypeline-1.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.847206 scalable-pypeline-1.1.5/pypeline/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11499 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10759 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/celery_beat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4191 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/extensions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.848206 scalable-pypeline-1.1.5/pypeline/flask/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.849206 scalable-pypeline-1.1.5/pypeline/flask/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8295 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/schedules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5791 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/flask_sermos.py
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/logging_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6763 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/pipeline_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7385 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/schedule_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    29081 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/sermos_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.851206 scalable-pypeline-1.1.5/pypeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13029 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/config_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/graph_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/module_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    33793 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/task_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.853206 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      541 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-11 21:01:59.855207 scalable-pypeline-1.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6355 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.841205 scalable-pypeline-1.1.5/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.854206 scalable-pypeline-1.1.5/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/tests/fixtures/s3_fixtures.py
```

### Comparing `scalable-pypeline-1.1.4/LICENSE` & `scalable-pypeline-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/PKG-INFO` & `scalable-pypeline-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.1.4
+Version: 1.1.5
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.1.4/README.md` & `scalable-pypeline-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/celery.py` & `scalable-pypeline-1.1.5/pypeline/celery.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,19 @@
         self.config = config if config else {}
         self.celery = celery_instance
 
     def _get_default_tasks(self) -> List[dict]:
         """ Sermos provides default tasks that all workers should know about.
         """
         return [{
-            'handler': 'sermos.celery.pipeline_retry'
+            'handler': 'pypeline.celery.pipeline_retry'
         }, {
-            'handler': 'sermos.celery.task_chain_regulator'
+            'handler': 'pypeline.celery.task_chain_regulator'
         }, {
-            'handler': 'sermos.celery.pipeline_success'
+            'handler': 'pypeline.celery.pipeline_success'
         }]
 
     def generate(self):
         """ Loads methods based on sermos config file and decorates them as
             celery tasks.
 
             Customer's methods:
@@ -211,15 +211,15 @@
     celery.Task = ChainedTask
 
     # Configure the broker and tasks
     celery.conf.broker_url = CELERY_BROKER_URL
 
     # Use our custom database scheduler for dynamic celery beat updates.
     celery.conf.beat_scheduler =\
-        'sermos.celery_beat:SermosScheduler'
+        'pypeline.celery_beat:SermosScheduler'
 
     # Reasonable defaults, override as necessary
     celery.conf.worker_redirect_stdouts = True
     celery.conf.worker_redirect_stdouts_level = LOG_LEVEL
     celery.conf.worker_hijack_root_logger = False
 
     if PIPELINE_CHORD_COMPRESSION:
```

### Comparing `scalable-pypeline-1.1.4/pypeline/celery_beat.py` & `scalable-pypeline-1.1.5/pypeline/celery_beat.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/constants.py` & `scalable-pypeline-1.1.5/pypeline/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 API_PATH_V1 = '/api/v1'
 
 DEFAULT_RESULT_TTL = 86400  # seconds (1 day)
 DEFAULT_TASK_TTL = 60  # seconds (1 minute)
 DEFAULT_RETRY_TASK_MAX_TTL = 300
 DEFAULT_MAX_RETRY = 10
-DEFAULT_REGULATOR_TASK = 'sermos.celery.task_chain_regulator'
-DEFAULT_SUCCESS_TASK = 'sermos.celery.pipeline_success'
-DEFAULT_RETRY_TASK = 'sermos.celery.pipeline_retry'
+DEFAULT_REGULATOR_TASK = 'pypeline.celery.task_chain_regulator'
+DEFAULT_SUCCESS_TASK = 'pypeline.celery.pipeline_success'
+DEFAULT_RETRY_TASK = 'pypeline.celery.pipeline_retry'
 
 CHAIN_SUCCESS_MSG = 'Chain built successfully ...'
 CHAIN_FAILURE_MSG = 'Chain failed to build ...'
 
 PIPELINE_RUN_WRAPPER_CACHE_KEY = 'sermos_{}_{}'  # pipeline_id + execution_id
 PIPELINE_RESULT_CACHE_KEY = 'sermos_result_{}'  # execution_id
```

### Comparing `scalable-pypeline-1.1.4/pypeline/extensions.py` & `scalable-pypeline-1.1.5/pypeline/extensions.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/flask/__init__.py` & `scalable-pypeline-1.1.5/pypeline/flask/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Sermos' Flask Implementation and Tooling. Convenience imports here.
 """
 import logging
 
 logger = logging.getLogger(__name__)
 
 try:
-    from rho_web.smorest import Blueprint, Api
-    from rho_web.response import abort
+    from flask_smorest import Blueprint, Api
+    from flask import abort
 except Exception as e:
     logger.error("Unable to import Web services (Blueprint, API, abort)"
                  f" ... {e}")
 
 try:
     from pypeline.flask.flask_sermos import FlaskSermos
 except Exception as e:
```

### Comparing `scalable-pypeline-1.1.4/pypeline/flask/api/pipelines.py` & `scalable-pypeline-1.1.5/pypeline/flask/api/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """ Pipeline APIs
 """
 import logging
 
 from celery.canvas import _chain
 from celery_dyrygent.workflows import Workflow
-from flask import jsonify, request
+from flask import jsonify, request, abort
+from flask_smorest import Blueprint
 from flask.views import MethodView
-from rho_web.smorest import Blueprint
-from rho_web.response import abort
 from marshmallow import Schema, fields
 from marshmallow.exceptions import ValidationError
 from pypeline.constants import API_DOC_RESPONSES, API_DOC_PARAMS, API_PATH_V1
 from pypeline.flask.decorators import require_accesskey
 from pypeline.flask.api.utils import chain_helper
 from pypeline.utils.task_utils import PipelineResult
 from pypeline.utils.config_utils import retrieve_latest_pipeline_config
```

### Comparing `scalable-pypeline-1.1.4/pypeline/flask/api/schedules.py` & `scalable-pypeline-1.1.5/pypeline/flask/api/schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ API Endpoints for Scheduled Tasks
 """
 import os
 import logging
 from flask import jsonify, request
 from flask.views import MethodView
 from marshmallow import Schema, fields
-from rho_web.smorest import Blueprint
-from rho_web.response import abort
+from flask_smorest import Blueprint
+from flask import abort
 from marshmallow.exceptions import ValidationError
 from pypeline.constants import API_DOC_RESPONSES, API_DOC_PARAMS,\
     API_PATH_V1
 from pypeline.utils.config_utils import retrieve_latest_schedule_config, \
     update_schedule_config
 from pypeline.schedule_config_schema import BaseScheduleSchema
 from pypeline.flask.decorators import require_accesskey
```

### Comparing `scalable-pypeline-1.1.4/pypeline/flask/api/utils.py` & `scalable-pypeline-1.1.5/pypeline/flask/api/utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/flask/decorators.py` & `scalable-pypeline-1.1.5/pypeline/flask/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import logging
 from http import HTTPStatus
 from functools import wraps
 import requests
 from rhodb.redis_conf import RedisConnector
 from flask import request
-from rho_web.response import abort
+from flask import abort
 from pypeline.constants import DEFAULT_AUTH_URL, AUTH_LOCK_KEY, \
     AUTH_LOCK_DURATION, USING_SERMOS_CLOUD
 
 logger = logging.getLogger(__name__)
 redis_conn = RedisConnector().get_connection()
```

### Comparing `scalable-pypeline-1.1.4/pypeline/flask/flask_sermos.py` & `scalable-pypeline-1.1.5/pypeline/flask/flask_sermos.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 if os.getenv('USE_GEVENT', 'false').lower() == 'true':
     import gevent.monkey
     gevent.monkey.patch_all()
 
 import logging
 from flask import Flask
 from werkzeug.middleware.proxy_fix import ProxyFix
-from rho_web.smorest import Api, Blueprint
-from pypeline.logging_config import setup_logging
+from flask_smorest import  Api, Blueprint
 from pypeline.extensions import sermos_config
 from pypeline.constants import DEFAULT_OPENAPI_CONFIG
 from pypeline import __version__
 
 logger = logging.getLogger(__name__)
```

### Comparing `scalable-pypeline-1.1.4/pypeline/generators.py` & `scalable-pypeline-1.1.5/pypeline/generators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/logging_config.py` & `scalable-pypeline-1.1.5/pypeline/logging_config.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/pipeline_config_schema.py` & `scalable-pypeline-1.1.5/pypeline/pipeline_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/schedule_config_schema.py` & `scalable-pypeline-1.1.5/pypeline/schedule_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/sermos_yaml.py` & `scalable-pypeline-1.1.5/pypeline/sermos_yaml.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/utils/config_utils.py` & `scalable-pypeline-1.1.5/pypeline/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/utils/graph_utils.py` & `scalable-pypeline-1.1.5/pypeline/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/utils/module_utils.py` & `scalable-pypeline-1.1.5/pypeline/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/pypeline/utils/task_utils.py` & `scalable-pypeline-1.1.5/pypeline/utils/task_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/scalable_pypeline.egg-info/PKG-INFO` & `scalable-pypeline-1.1.5/scalable_pypeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.1.4
+Version: 1.1.5
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.1.4/scalable_pypeline.egg-info/SOURCES.txt` & `scalable-pypeline-1.1.5/scalable_pypeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.4/scalable_pypeline.egg-info/requires.txt` & `scalable-pypeline-1.1.5/scalable_pypeline.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 honcho>=1.0.1
 awscli>=1.11
 pylint>=2.5.3
 pip-licenses
 
 [flask]
 Flask>=1.1.1
-rho-web[smorest]>=0.3.3
 flask-smorest>=0.23.0
 
 [test]
 pytest-cov<3,>=2.6.1
 tox<4,>=3.14.1
 mock<2,>=1
 moto<2,>=1.3.16
@@ -35,9 +34,9 @@
 importlib-metadata<5,>=4.12
 
 [web]
 gunicorn
 gevent
 
 [workers]
-celery[redis]==5.1.2
+celery[redis]<6,>=5.1.2
 networkx>=2.4
```

### Comparing `scalable-pypeline-1.1.4/setup.py` & `scalable-pypeline-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,20 +161,19 @@
     packages=packages,
     include_package_data=True,
     cmdclass=cmdclass,
     ext_modules=ext_modules,
     install_requires=install_requires,
     extras_require={
         'build': ['wheel', 'twine'],
-        # TODO: decouple rho-web & Flask-RhoAuth
         'flask':
-        ['Flask>=1.1.1', 'rho-web[smorest]>=0.3.3', 'flask-smorest>=0.23.0'],
+        ['Flask>=1.1.1', 'flask-smorest>=0.23.0'],
         'web': ['gunicorn', 'gevent'],
         'workers': [
-            'celery[redis]==5.1.2',
+            "celery[redis]>=5.1.2,<6",
             'networkx>=2.4',
         ],
         'dev':['honcho>=1.0.1', 'awscli>=1.11', 'pylint>=2.5.3', 'pip-licenses'],
         'test': [
             'pytest-cov>=2.6.1,<3',
             'tox>=3.14.1,<4',
             'mock>=1,<2',
```

### Comparing `scalable-pypeline-1.1.4/tests/fixtures/s3_fixtures.py` & `scalable-pypeline-1.1.5/tests/fixtures/s3_fixtures.py`

 * *Files identical despite different names*

