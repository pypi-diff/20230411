# Comparing `tmp/gl-webhooks-1.1.8.tar.gz` & `tmp/gl-webhooks-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gl-webhooks-1.1.8.tar", last modified: Tue Apr  4 07:48:02 2023, max compression
+gzip compressed data, was "gl-webhooks-1.1.9.tar", last modified: Tue Apr  4 07:56:01 2023, max compression
```

## Comparing `gl-webhooks-1.1.8.tar` & `gl-webhooks-1.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.743638 gl-webhooks-1.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2497 2023-04-04 07:48:02.743638 gl-webhooks-1.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1655 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.736637 gl-webhooks-1.1.8/gl_webhooks/
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      889 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.740638 gl-webhooks-1.1.8/gl_webhooks/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.741638 gl-webhooks-1.1.8/gl_webhooks/api/badges/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/badges/static.py
--rw-rw-rw-   0 root         (0) root         (0)     3876 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/badges/static.yml
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/metrics.yml
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/openapi.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.732637 gl-webhooks-1.1.8/gl_webhooks/api/webhooks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.742638 gl-webhooks-1.1.8/gl_webhooks/api/webhooks/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)     2880 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/webhooks/gitlab/jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1398 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/webhooks/gitlab/jobs.yml
--rw-rw-rw-   0 root         (0) root         (0)     5042 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/api/x-responses.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.743638 gl-webhooks-1.1.8/gl_webhooks/models/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6319 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/gl_webhooks/models/badges.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:48:02.739637 gl-webhooks-1.1.8/gl_webhooks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2497 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/gl_webhooks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/gl_webhooks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/gl_webhooks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/gl_webhooks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/gl_webhooks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/gl_webhooks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/gl_webhooks.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)     6458 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-04 07:48:02.000000 gl-webhooks-1.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 07:48:02.743638 gl-webhooks-1.1.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1120 2023-04-04 07:47:17.000000 gl-webhooks-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.238925 gl-webhooks-1.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-04-04 07:56:01.237925 gl-webhooks-1.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1655 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.231925 gl-webhooks-1.1.9/gl_webhooks/
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      889 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.235925 gl-webhooks-1.1.9/gl_webhooks/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.235925 gl-webhooks-1.1.9/gl_webhooks/api/badges/
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/badges/static.py
+-rw-rw-rw-   0 root         (0) root         (0)     3876 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/badges/static.yml
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/metrics.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/openapi.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.227924 gl-webhooks-1.1.9/gl_webhooks/api/webhooks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.236925 gl-webhooks-1.1.9/gl_webhooks/api/webhooks/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)     2897 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/webhooks/gitlab/jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/webhooks/gitlab/jobs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5042 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/api/x-responses.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.237925 gl-webhooks-1.1.9/gl_webhooks/models/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6319 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/gl_webhooks/models/badges.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:56:01.233925 gl-webhooks-1.1.9/gl_webhooks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-04-04 07:56:01.000000 gl-webhooks-1.1.9/gl_webhooks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-04 07:56:01.000000 gl-webhooks-1.1.9/gl_webhooks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 07:56:01.000000 gl-webhooks-1.1.9/gl_webhooks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-04 07:56:01.000000 gl-webhooks-1.1.9/gl_webhooks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-04 07:56:01.000000 gl-webhooks-1.1.9/gl_webhooks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-04 07:56:01.000000 gl-webhooks-1.1.9/gl_webhooks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 07:56:01.000000 gl-webhooks-1.1.9/gl_webhooks.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)     6458 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-04 07:56:00.000000 gl-webhooks-1.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 07:56:01.238925 gl-webhooks-1.1.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1120 2023-04-04 07:55:15.000000 gl-webhooks-1.1.9/setup.py
```

### Comparing `gl-webhooks-1.1.8/LICENSE` & `gl-webhooks-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/PKG-INFO` & `gl-webhooks-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gl-webhooks
-Version: 1.1.8
+Version: 1.1.9
 Summary: GL Webhooks is a project that provides GitLab functionalities via webhook endpoints.
 Author-email: Julien Lecomte <julien@lecomte.at>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/jlecomte/python/gl-webhooks
 Project-URL: Documentation, https://jlecomte.gitlab.io/python/gl-webhooks/
 Project-URL: Source code, https://gitlab.com/jlecomte/python/gl-webhooks
 Project-URL: Bug tracker, https://gitlab.com/jlecomte/python/gl-webhooks/-/issues
```

### Comparing `gl-webhooks-1.1.8/README.md` & `gl-webhooks-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks/__main__.py` & `gl-webhooks-1.1.9/gl_webhooks/__main__.py`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/badges/static.py` & `gl-webhooks-1.1.9/gl_webhooks/api/badges/static.py`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/badges/static.yml` & `gl-webhooks-1.1.9/gl_webhooks/api/badges/static.yml`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/metrics.py` & `gl-webhooks-1.1.9/gl_webhooks/api/metrics.py`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/metrics.yml` & `gl-webhooks-1.1.9/gl_webhooks/api/metrics.yml`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/openapi.yml` & `gl-webhooks-1.1.9/gl_webhooks/api/openapi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 #
 # https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.0.md
 #
 openapi: "3.0.0"
 
 info:
-  version: "1.1.8"
+  version: "1.1.9"
   title: "GL Webhooks"
   description: |
     GL Webhooks is a project that provides GitLab functionalities via webhook endpoints.
 
 components:
   # ----------------------------------------------------------------------------
   parameters:
```

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/webhooks/gitlab/jobs.py` & `gl-webhooks-1.1.9/gl_webhooks/api/webhooks/gitlab/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,35 +31,38 @@
                 json.dump(data, fd, indent=2, sort_keys=True)
 
         return data or {}
 
 
 @endpoint
 def monitor_purge(app, body):
-    cfg = app.settings["gitlab"]
-
-    gl = gitlab.Gitlab(cfg["url"], private_token=cfg["token"])
-
-    def action1(data):
+    def action(data):
         # purge finished states
         data = {k: v for k, v in data.items() if v["status"] not in FINAL_STATES}
         return data
 
-    def action2(data):
+    data = action_jobs_file(app, action)
+    return data, 200
+
+
+@endpoint
+def monitor_update(app, body):
+    cfg = app.settings["gitlab"]
+    gl = gitlab.Gitlab(cfg["url"], private_token=cfg["token"])
+
+    def action(data):
         for k, v in data.items():
             try:
                 job = gl.projects.get(v["project_id"], lazy=True).jobs.get(v["build_id"])
                 v["status"] = job.status
             except:
                 pass
         return data
 
-    data = action_jobs_file(app, action1)
-    data = action_jobs_file(app, action2)
-    data = action_jobs_file(app, action1)
+    data = action_jobs_file(app, action)
     return data, 200
 
 
 @webhook([HookEvents.JOB_HOOK])
 def monitor(app, body):
     build_id = str(body["build_id"])
     build_status = body["build_status"]
```

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/webhooks/gitlab/jobs.yml` & `gl-webhooks-1.1.9/gl_webhooks/api/webhooks/gitlab/jobs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,29 @@
         200:
           $ref: "#/components/responses/200_ok"
         400:
           $ref: "#/components/responses/400_bad_request"
         500:
           $ref: "#/components/responses/500_internal_server_error"
 
+  /api/webhooks/gitlab/jobs/monitor/update:
+    post:
+      operationId: api.webhooks.gitlab.jobs.monitor_update
+      summary: "Update monitor job creations and destructions statuses"
+      tags:
+        - gitlab
+        - jobs
+      responses:
+        200:
+          $ref: "#/components/responses/200_ok"
+        400:
+          $ref: "#/components/responses/400_bad_request"
+        500:
+          $ref: "#/components/responses/500_internal_server_error"
+
   /api/webhooks/gitlab/jobs/monitor:
     post:
       operationId: api.webhooks.gitlab.jobs.monitor
       summary: "Monitor job creations and destructions"
       tags:
         - gitlab
         - jobs
```

### Comparing `gl-webhooks-1.1.8/gl_webhooks/api/x-responses.yml` & `gl-webhooks-1.1.9/gl_webhooks/api/x-responses.yml`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks/models/badges.py` & `gl-webhooks-1.1.9/gl_webhooks/models/badges.py`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/gl_webhooks.egg-info/PKG-INFO` & `gl-webhooks-1.1.9/gl_webhooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gl-webhooks
-Version: 1.1.8
+Version: 1.1.9
 Summary: GL Webhooks is a project that provides GitLab functionalities via webhook endpoints.
 Author-email: Julien Lecomte <julien@lecomte.at>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/jlecomte/python/gl-webhooks
 Project-URL: Documentation, https://jlecomte.gitlab.io/python/gl-webhooks/
 Project-URL: Source code, https://gitlab.com/jlecomte/python/gl-webhooks
 Project-URL: Bug tracker, https://gitlab.com/jlecomte/python/gl-webhooks/-/issues
```

### Comparing `gl-webhooks-1.1.8/gl_webhooks.egg-info/SOURCES.txt` & `gl-webhooks-1.1.9/gl_webhooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gl-webhooks-1.1.8/pyproject.toml` & `gl-webhooks-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # ------------------------------------------------------------------------------
 # Setup
 # ------------------------------------------------------------------------------
 [project]
 dynamic = ["dependencies"]
 
 name = "gl-webhooks"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   {name = "Julien Lecomte", email = "julien@lecomte.at"}
 ]
 readme  = "README.md"
 license = {text = "MIT"}
 description = "GL Webhooks is a project that provides GitLab functionalities via webhook endpoints."
```

### Comparing `gl-webhooks-1.1.8/setup.py` & `gl-webhooks-1.1.9/setup.py`

 * *Files identical despite different names*

