# Comparing `tmp/vdk-meta-jobs-0.1.824443273.tar.gz` & `tmp/vdk-meta-jobs-0.1.833741966.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-meta-jobs-0.1.824443273.tar", last modified: Fri Mar 31 14:25:59 2023, max compression
+gzip compressed data, was "vdk-meta-jobs-0.1.833741966.tar", last modified: Tue Apr 11 12:13:05 2023, max compression
```

## Comparing `vdk-meta-jobs-0.1.824443273.tar` & `vdk-meta-jobs-0.1.833741966.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.908502 vdk-meta-jobs-0.1.824443273/
--rw-r--r--   0 root         (0) root         (0)     6342 2023-03-31 14:25:59.908502 vdk-meta-jobs-0.1.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5769 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:59.908502 vdk-meta-jobs-0.1.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1457 2023-03-31 14:25:51.000000 vdk-meta-jobs-0.1.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.904502 vdk-meta-jobs-0.1.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.904502 vdk-meta-jobs-0.1.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.904502 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.904502 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.904502 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/api/
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/api/meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)     8151 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6485 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4522 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5635 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta_job_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/plugin_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1553 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.908502 vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6342 2023-03-31 14:25:59.000000 vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      859 2023-03-31 14:25:59.000000 vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:59.000000 vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-31 14:25:59.000000 vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-03-31 14:25:59.000000 vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:59.000000 vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.908502 vdk-meta-jobs-0.1.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/tests/test_meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)    13617 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/tests/test_meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-03-31 14:25:48.000000 vdk-meta-jobs-0.1.824443273/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2023-04-11 12:12:57.000000 vdk-meta-jobs-0.1.833741966/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.884825 vdk-meta-jobs-0.1.833741966/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.884825 vdk-meta-jobs-0.1.833741966/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.884825 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/api/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/api/meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     8320 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7948 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4522 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5710 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_job_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/plugin_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     9041 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-11 12:13:05.000000 vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:13:05.888825 vdk-meta-jobs-0.1.833741966/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    15107 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-11 12:12:53.000000 vdk-meta-jobs-0.1.833741966/tests/test_tracking_job_executor.py
```

### Comparing `vdk-meta-jobs-0.1.824443273/PKG-INFO` & `vdk-meta-jobs-0.1.833741966/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.824443273
+Version: 0.1.833741966
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -38,25 +38,27 @@
 ```python
 def run(job_input):
     jobs = [
         {
         "job_name": "name-of-job",
         "team_name": "team-of-job",
         "fail_meta_job_on_error": True or False,
+        "arguments": {"key1": value1, "key2": value2},
         "depends_on": [name-of-job1, name-of-job2]
         },
         ...
     ]
     MetaJobInput().run_meta_job(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
 * **job_name**: required, the name of the data job
 * **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team
-* **fail_meta_job_on_error**: optional, default is true. if true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **fail_meta_job_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
@@ -75,46 +77,52 @@
 from vdk.plugin.meta_jobs.meta_job_runner import MetaJobInput
 
 JOBS_RUN_ORDER = [
     {
         "job_name": "job1",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": []
     },
 
     {
         "job_name": "job2",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
     {
         "job_name": "job3",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
     {
         "job_name": "job4",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
 
     {
         "job_name": "job5",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job3"]
     },
     {
         "job_name": "job6",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job3"]
     },
 ]
 
 
 def run(job_input: IJobInput) - > None:
     MetaJobInput().run_meta_job(JOBS_RUN_ORDER)
```

### Comparing `vdk-meta-jobs-0.1.824443273/README.md` & `vdk-meta-jobs-0.1.833741966/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,25 +24,27 @@
 ```python
 def run(job_input):
     jobs = [
         {
         "job_name": "name-of-job",
         "team_name": "team-of-job",
         "fail_meta_job_on_error": True or False,
+        "arguments": {"key1": value1, "key2": value2},
         "depends_on": [name-of-job1, name-of-job2]
         },
         ...
     ]
     MetaJobInput().run_meta_job(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
 * **job_name**: required, the name of the data job
 * **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team
-* **fail_meta_job_on_error**: optional, default is true. if true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **fail_meta_job_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
@@ -61,46 +63,52 @@
 from vdk.plugin.meta_jobs.meta_job_runner import MetaJobInput
 
 JOBS_RUN_ORDER = [
     {
         "job_name": "job1",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": []
     },
 
     {
         "job_name": "job2",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
     {
         "job_name": "job3",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
     {
         "job_name": "job4",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
 
     {
         "job_name": "job5",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job3"]
     },
     {
         "job_name": "job6",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job3"]
     },
 ]
 
 
 def run(job_input: IJobInput) - > None:
     MetaJobInput().run_meta_job(JOBS_RUN_ORDER)
```

### Comparing `vdk-meta-jobs-0.1.824443273/setup.py` & `vdk-meta-jobs-0.1.833741966/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.824443273"
+__version__ = "0.1.833741966"
 
 setuptools.setup(
     name="vdk-meta-jobs",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/api/meta_job.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/api/meta_job.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     """
     TODO
     """
 
     job_name: str
     team_name: str = None
     fail_meta_job_on_error: bool = True
+    arguments: dict = None
     depends_on: List[str] = field(default_factory=list)
 
 
 @dataclass
 class MetaJob(SingleJob):
     """
     TODO
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/cached_data_job_executor.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/cached_data_job_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import logging
-import os
 import time
 from typing import Dict
 from typing import Optional
 
 import urllib3.exceptions as url_exception
+from vdk.api.job_input import IJobArguments
 from vdk.internal.core.errors import ErrorMessage
 from vdk.internal.core.errors import UserCodeError
 from vdk.plugin.meta_jobs.meta import IDataJobExecutor
 from vdk.plugin.meta_jobs.meta import TrackableJob
 from vdk.plugin.meta_jobs.remote_data_job import JobStatus
 
 log = logging.getLogger(__name__)
@@ -40,15 +40,15 @@
     def start_job(self, job_name: str) -> None:
         """
         :param job_name: the job to start and track
         """
         job = self.__get_job(job_name)
         job.start_attempt += 1
         execution_id = self.start_new_job_execution(
-            job_name=job.job_name, team_name=job.team_name
+            job_name=job.job_name, team_name=job.team_name, arguments=job.arguments
         )
         log.info(f"Starting new data job execution with id {execution_id}")
         job.execution_id = execution_id
         job.status = JobStatus.SUBMITTED.value
         job.details = self._executor.details_job(
             job.job_name, job.team_name, job.execution_id
         )
@@ -131,15 +131,17 @@
 
     def get_all_jobs(self):
         return list(self._jobs_cache.values())
 
     def get_currently_running_jobs(self):
         return [j for j in self._jobs_cache.values() if j.status in ACTIVE_JOB_STATUSES]
 
-    def start_new_job_execution(self, job_name: str, team_name: str) -> str:
+    def start_new_job_execution(
+        self, job_name: str, team_name: str, arguments: IJobArguments = None
+    ) -> str:
         """
         Start a new data job execution.
         The stages of the process are:
             1) Get the latest available execution_id before any new
                executions have been started.
             2) Start a new execution.
             3) In case of a Timeout exception, check if a new execution
@@ -148,26 +150,27 @@
         NOTE: A loop is used to handle situations, where due to some
         network instability, a socket timeout happens. The execution of
         the data job may have started, but we don't know because an execution
         id was not returned due to the exception.
 
         :param job_name: name of the data job to be executed
         :param team_name: name of the owning team
+        :param arguments: arguments of the data job
         :return: id of the started job execution
         """
         current_retries = 0
         execution_id = None
 
         latest_available_execution_id = self.get_latest_available_execution_id(
             job_name=job_name, team=team_name
         )
 
         while current_retries < ALLOWED_RETRIES:
             try:
-                execution_id = self._executor.start_job(job_name, team_name)
+                execution_id = self._executor.start_job(job_name, team_name, arguments)
                 return execution_id
             except url_exception.TimeoutError as e:
                 log.info(
                     f"A timeout exception occurred while starting the {job_name} data job. "
                     f"Exception was: {e}"
                 )
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/dag_validator.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/dag_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # Copyright 2023-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import graphlib
+import json
 import logging
 from collections import namedtuple
 from typing import Dict
 from typing import List
 
 from vdk.internal.core.errors import ErrorMessage
 from vdk.internal.core.errors import UserCodeError
 
 log = logging.getLogger(__name__)
 Error = namedtuple("Error", ["TYPE", "PERMISSION", "REQUIREMENT", "CONFLICT"])
 ERROR = Error(
     TYPE="type", PERMISSION="permission", REQUIREMENT="requirement", CONFLICT="conflict"
 )
-allowed_job_keys = {"job_name", "team_name", "fail_meta_job_on_error", "depends_on"}
+allowed_job_keys = {
+    "job_name",
+    "team_name",
+    "fail_meta_job_on_error",
+    "depends_on",
+    "arguments",
+}
 required_job_keys = {"job_name", "depends_on"}
 
 
 class DagValidator:
     """
     The purpose of this class is to validate the DAG structure and jobs.
     It is being used right before the DAG is built.
@@ -33,15 +40,15 @@
         self._validate_no_duplicates(jobs)
         for job in jobs:
             self._validate_job(job)
         self._check_dag_cycles(jobs)
         log.info("Successfully validated the DAG!")
 
     def _raise_error(
-        self, jobs: List[Dict], error_type: str, reason: str, countermeasures: str
+        self, error_type: str, reason: str, countermeasures: str, jobs: List[str] = ""
     ):
         raise UserCodeError(
             ErrorMessage(
                 "",
                 "Meta Job failed due to a Data Job validation failure.",
                 f"There is a {error_type} error with job(s) {jobs}. " + reason,
                 "The DAG will not be built and the Meta Job will fail.",
@@ -49,110 +56,145 @@
             )
         )
 
     def _validate_no_duplicates(self, jobs: List[Dict]):
         duplicated_jobs = list({job["job_name"] for job in jobs if jobs.count(job) > 1})
         if duplicated_jobs:
             self._raise_error(
-                duplicated_jobs,
                 ERROR.CONFLICT,
                 f"There are some duplicated jobs: {duplicated_jobs}.",
                 f"Remove the duplicated jobs from the list - each job can appear in the jobs list at most once. "
                 f"Duplicated jobs: {duplicated_jobs}.",
+                duplicated_jobs,
             )
 
     def _validate_job(self, job: Dict):
+        self._validate_job_type(job)
         self._validate_allowed_and_required_keys(job)
         self._validate_job_name(job)
-        self._validate_dependencies(job)
-        self._validate_team_name(job)
-        self._validate_fail_meta_job_on_error(job)
-        log.info(f"Successfully validated job: {job['job_name']}")
+        job_name = job.get("job_name")
+        self._validate_dependencies(job_name, job["depends_on"])
+        if "team_name" in job:
+            self._validate_team_name(job_name, job["team_name"])
+        if "fail_meta_job_on_error" in job:
+            self._validate_fail_meta_job_on_error(
+                job_name, job["fail_meta_job_on_error"]
+            )
+        if "arguments" in job:
+            self._validate_arguments(job_name, job["arguments"])
+        log.info(f"Successfully validated job: {job_name}")
+
+    def _validate_job_type(self, job: Dict):
+        if not isinstance(job, dict):
+            self._raise_error(
+                ERROR.TYPE,
+                "The job type is not dict.",
+                f"Change the Data Job type. Current type is {type(job)}. Expected type is dict.",
+                ["".join(list(job))],
+            )
 
     def _validate_allowed_and_required_keys(self, job: Dict):
-        forbidden_keys = [key for key in job.keys() if key not in allowed_job_keys]
-        if forbidden_keys:
+        disallowed_keys = [key for key in job.keys() if key not in allowed_job_keys]
+        if disallowed_keys:
             self._raise_error(
-                list(job),
                 ERROR.PERMISSION,
                 "One or more job dict keys are not allowed.",
-                f"Remove the forbidden Data Job Dict keys. "
-                f"Keys {forbidden_keys} are forbidden. Allowed keys: {allowed_job_keys}.",
+                f"Remove the disallowed Data Job Dict keys. "
+                f"Keys {disallowed_keys} are not allowed. Allowed keys: {allowed_job_keys}.",
             )
         missing_keys = [key for key in required_job_keys if key not in job]
         if missing_keys:
             self._raise_error(
-                list(job),
                 ERROR.REQUIREMENT,
                 "One or more job dict required keys are missing.",
                 f"Add the missing required Data Job Dict keys. Keys {missing_keys} "
                 f"are missing. Required keys: {required_job_keys}.",
             )
 
     def _validate_job_name(self, job: Dict):
         if not isinstance(job["job_name"], str):
             self._raise_error(
-                list(job),
                 ERROR.TYPE,
                 "The type of the job dict key job_name is not string.",
                 f"Change the Data Job Dict value of job_name. "
                 f"Current type is {type(job['job_name'])}. Expected type is string.",
+                ["".join(list(job))],
             )
 
-    def _validate_dependencies(self, job: Dict):
-        if not (isinstance(job["depends_on"], List)):
+    def _validate_dependencies(self, job_name: str, dependencies: List[str]):
+        if not (isinstance(dependencies, List)):
             self._raise_error(
-                list(job),
                 ERROR.TYPE,
                 "The type of the job dict depends_on key is not list.",
                 f"Check the Data Job Dict type of the depends_on key. Current type "
-                f"is {type(job['depends_on'])}. Expected type is list.",
+                f"is {type(dependencies)}. Expected type is list.",
+                [job_name],
             )
         non_string_dependencies = [
-            pred for pred in job["depends_on"] if not isinstance(pred, str)
+            pred for pred in dependencies if not isinstance(pred, str)
         ]
         if non_string_dependencies:
             self._raise_error(
-                list(job),
                 ERROR.TYPE,
                 "One or more items of the job dependencies list are not strings.",
                 f"Check the Data Job Dict values of the depends_on list. "
                 f"There are some non-string values: {non_string_dependencies}. Expected type is string.",
+                [job_name],
             )
 
-    def _validate_team_name(self, job: Dict):
-        if "team_name" in job and not isinstance(job["team_name"], str):
+    def _validate_team_name(self, job_name: str, team_name: str):
+        if not isinstance(team_name, str):
             self._raise_error(
-                list(job),
                 ERROR.TYPE,
                 "The type of the job dict key job_name is not string.",
                 f"Change the Data Job Dict value of team_name. "
-                f"Current type is {type(job['team_name'])}. Expected type is string.",
+                f"Current type is {type(team_name)}. Expected type is string.",
+                [job_name],
             )
 
-    def _validate_fail_meta_job_on_error(self, job: Dict):
-        if "fail_meta_job_on_error" in job and not isinstance(
-            (job["fail_meta_job_on_error"]), bool
-        ):
+    def _validate_fail_meta_job_on_error(
+        self, job_name: str, fail_meta_job_on_error: bool
+    ):
+        if not isinstance(fail_meta_job_on_error, bool):
             self._raise_error(
-                list(job),
                 ERROR.TYPE,
                 "The type of the job dict key fail_meta_job_on_error is not bool (True/False).",
                 f"Change the Data Job Dict value of fail_meta_job_on_error. Current type"
-                f" is {type(job['fail_meta_job_on_error'])}. Expected type is bool.",
+                f" is {type(fail_meta_job_on_error)}. Expected type is bool.",
+                [job_name],
+            )
+
+    def _validate_arguments(self, job_name: str, job_args: dict):
+        if not isinstance(job_args, dict):
+            self._raise_error(
+                ERROR.TYPE,
+                "The type of the job dict key arguments is not dict.",
+                f"Change the Data Job Dict value of arguments. "
+                f"Current type is {type(job_args)}. Expected type is dict.",
+                [job_name],
+            )
+        try:
+            json.dumps(job_args)
+        except TypeError as e:
+            self._raise_error(
+                ERROR.TYPE,
+                str(e),
+                f"Change the Data Job Dict value of arguments. "
+                f"Current type is {type(job_args)} but not serializable as JSON.",
+                [job_name],
             )
 
     def _check_dag_cycles(self, jobs: List[Dict]):
         topological_sorter = graphlib.TopologicalSorter()
         for job in jobs:
             topological_sorter.add(job["job_name"], *job["depends_on"])
 
         try:
             # Preparing the sorter raises CycleError if cycles exist
             topological_sorter.prepare()
         except graphlib.CycleError as e:
             self._raise_error(
-                e.args[1][:-1],
                 ERROR.CONFLICT,
                 "There is a cycle in the DAG.",
                 f"Change the depends_on list of the jobs that participate in the detected cycle: {e.args[1]}.",
+                e.args[1][:-1],
             )
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 # SPDX-License-Identifier: Apache-2.0
 import abc
 from dataclasses import dataclass
 from typing import List
 from typing import Optional
 
 from taurus_datajob_api import DataJobExecution
+from vdk.api.job_input import IJobArguments
 from vdk.plugin.meta_jobs.api import meta_job
 
 
 class IDataJobExecutor(abc.ABC):
     @abc.abstractmethod
-    def start_job(self, job_name: str, team_name: str):
+    def start_job(self, job_name: str, team_name: str, arguments: IJobArguments = None):
         """
         Start an execution of a data job and returns its execution id
+        :param arguments:
         :param job_name:
         :param team_name:
         :return: execution id
         """
         pass
 
     @abc.abstractmethod
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta_configuration.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta_dag.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 from vdk.plugin.meta_jobs.remote_data_job_executor import RemoteDataJobExecutor
 from vdk.plugin.meta_jobs.time_based_queue import TimeBasedQueue
 
 log = logging.getLogger(__name__)
 
 
 class MetaJobsDag:
-    def __init__(self, team_name: str, meta_config: MetaPluginConfiguration):
+    def __init__(
+        self,
+        team_name: str,
+        meta_config: MetaPluginConfiguration,
+    ):
         self._team_name = team_name
         self._topological_sorter = TopologicalSorter()
         self._delayed_starting_jobs = TimeBasedQueue(
             min_ready_time_seconds=meta_config.meta_jobs_delayed_jobs_min_delay_seconds(),
             randomize_delay_seconds=meta_config.meta_jobs_delayed_jobs_randomized_added_delay_seconds(),
         )
         self._max_concurrent_running_jobs = (
@@ -45,14 +49,15 @@
     def build_dag(self, jobs: List[Dict]):
         self._dag_validator.validate(jobs)
         for job in jobs:
             trackable_job = TrackableJob(
                 job["job_name"],
                 job.get("team_name", self._team_name),
                 job.get("fail_meta_job_on_error", True),
+                job.get("arguments", None),
             )
             self._job_executor.register_job(trackable_job)
             self._topological_sorter.add(trackable_job.job_name, *job["depends_on"])
 
     def execute_dag(self):
         self._topological_sorter.prepare()
         while self._topological_sorter.is_active():
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/meta_job_runner.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/meta_job_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/plugin_entry.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/plugin_entry.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/remote_data_job.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from taurus_datajob_api import ApiClient
 from taurus_datajob_api import Configuration
 from taurus_datajob_api import DataJobExecution
 from taurus_datajob_api import DataJobExecutionRequest
 from taurus_datajob_api import DataJobsExecutionApi
 from urllib3 import Retry
+from vdk.api.job_input import IJobArguments
 from vdk.plugin.control_api_auth.authentication import Authentication
 
 log = logging.getLogger(__name__)
 
 
 # This is mostly copy pasted from
 # https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/airflow-provider-vdk/vdk_provider/hooks/vdk.py
@@ -45,20 +46,22 @@
     """
 
     def __init__(
         self,
         job_name: str,
         team_name: str,
         rest_api_url: str,
+        arguments: IJobArguments = None,
         timeout: int = 5,  # TODO: Set reasonable default
         **kwargs,
     ) -> None:
-        self.job_name = job_name
-        self.team_name = team_name
-        self._rest_api_url = rest_api_url
+        self.__job_name = job_name
+        self.__team_name = team_name
+        self.__rest_api_url = rest_api_url
+        self.__arguments = arguments
         self.timeout = timeout
         self.deployment_id = "production"  # currently multiple deployments are not supported so this remains hardcoded
         self.auth: Optional[Authentication] = kwargs.pop("auth", None)
 
         # setting these manually to avoid using VDKConfig
         # TODO: set op ID from current job
         self.op_id = f"{uuid.uuid4().hex}"[:16]
@@ -74,27 +77,27 @@
         self.http_connect_retries = int(
             os.getenv("VDK_CONTROL_HTTP_CONNECT_RETRIES", "6")
         )
         self.http_read_retries = int(os.getenv("VDK_CONTROL_HTTP_READ_RETRIES", "6"))
 
         self.__execution_api = self._get_execution_api()
 
-    def start_job_execution(self, **request_kwargs) -> str:
+    def start_job_execution(self) -> str:
         """
         Triggers a manual Datajob execution.
 
         :param: request_kwargs: Request arguments to be included with the HTTP request
         """
         execution_request = DataJobExecutionRequest(
             started_by="meta-job",  # TODO: specify name of meta job
-            args=request_kwargs,
+            args=self.__arguments,
         )
         _, _, headers = self.__execution_api.data_job_execution_start_with_http_info(
-            team_name=self.team_name,
-            job_name=self.job_name,
+            team_name=self.__team_name,
+            job_name=self.__job_name,
             deployment_id=self.deployment_id,
             data_job_execution_request=execution_request,
             _request_timeout=self.timeout,
         )
         log.debug(f"Received headers: {headers}")
 
         job_execution_id = os.path.basename(headers["Location"])
@@ -103,52 +106,56 @@
     def cancel_job_execution(self, execution_id: str) -> None:
         """
         Cancels a Datajob execution.
 
         :param execution_id: ID of the job execution
         """
         self.__execution_api.data_job_execution_cancel(
-            team_name=self.team_name,
-            job_name=self.job_name,
+            team_name=self.__team_name,
+            job_name=self.__job_name,
             execution_id=execution_id,
             _request_timeout=self.timeout,
         )
 
     def get_job_execution_log(self, execution_id: str) -> str:
         """
         Returns the stored execution logs for a particular job execution.
 
         :param execution_id: ID of the job execution
         :return: job execution logs
         """
         return self.__execution_api.data_job_logs_download(
-            team_name=self.team_name, job_name=self.job_name, execution_id=execution_id
+            team_name=self.__team_name,
+            job_name=self.__job_name,
+            execution_id=execution_id,
         ).logs
 
     def get_job_execution_status(self, execution_id: str) -> DataJobExecution:
         """
         Returns the execution status for a particular job execution.
 
         :param execution_id: ID of the job execution
         :return: The execution status object listing details about the status of this particular execution
         """
         job_execution: DataJobExecution = self.__execution_api.data_job_execution_read(
-            team_name=self.team_name, job_name=self.job_name, execution_id=execution_id
+            team_name=self.__team_name,
+            job_name=self.__job_name,
+            execution_id=execution_id,
         )
         return job_execution
 
     def get_job_executions(self) -> Optional[List[DataJobExecution]]:
         """
         Returns a list of all executions for a specific data job. The list
         is sorted and the last element is the latest available execution.
 
         :return: A list of DataJobExecution objects for the available executions.
         """
         job_execution_list = self.__execution_api.data_job_execution_list(
-            team_name=self.team_name, job_name=self.job_name
+            team_name=self.__team_name, job_name=self.__job_name
         )
         return job_execution_list
 
     def wait_for_job(
         self,
         execution_id,
         wait_seconds: float = 3,
@@ -196,15 +203,15 @@
             else:
                 log.info(
                     f"Encountered unexpected status `{job_status}` for job execution `{execution_id}`"
                 )
             return job_status
 
     def _get_execution_api(self):
-        rest_api_url = self._rest_api_url
+        rest_api_url = self.__rest_api_url
 
         config = Configuration(host=rest_api_url, api_key=None)
         config.connection_pool_maxsize = self.http_connection_pool_maxsize
         config.retries = Retry(
             total=self.http_total_retries,
             connect=self.http_connect_retries,
             read=self.http_read_retries,
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/remote_data_job_executor.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/remote_data_job_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 from typing import Optional
 
 from taurus_datajob_api import DataJobExecution
+from vdk.api.job_input import IJobArguments
 from vdk.internal.control.configuration.vdk_config import VDKConfig
 from vdk.plugin.meta_jobs.meta import IDataJobExecutor
 from vdk.plugin.meta_jobs.remote_data_job import RemoteDataJob
 
 
 class RemoteDataJobExecutor(IDataJobExecutor):
-    def start_job(self, job_name: str, team_name: str):
+    def start_job(self, job_name: str, team_name: str, arguments: IJobArguments = None):
         vdk_cfg = VDKConfig()
-        job = RemoteDataJob(job_name, team_name, vdk_cfg.control_service_rest_api_url)
+        job = RemoteDataJob(
+            job_name, team_name, vdk_cfg.control_service_rest_api_url, arguments
+        )
         return job.start_job_execution()
         # catch error on 409
 
     def status_job(self, job_name: str, team_name: str, execution_id: str) -> str:
         vdk_cfg = VDKConfig()
         job = RemoteDataJob(job_name, team_name, vdk_cfg.control_service_rest_api_url)
         status = job.get_job_execution_status(execution_id)
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk/plugin/meta_jobs/time_based_queue.py` & `vdk-meta-jobs-0.1.833741966/src/vdk/plugin/meta_jobs/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/PKG-INFO` & `vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.824443273
+Version: 0.1.833741966
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -38,25 +38,27 @@
 ```python
 def run(job_input):
     jobs = [
         {
         "job_name": "name-of-job",
         "team_name": "team-of-job",
         "fail_meta_job_on_error": True or False,
+        "arguments": {"key1": value1, "key2": value2},
         "depends_on": [name-of-job1, name-of-job2]
         },
         ...
     ]
     MetaJobInput().run_meta_job(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
 * **job_name**: required, the name of the data job
 * **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team
-* **fail_meta_job_on_error**: optional, default is true. if true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **fail_meta_job_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
+* **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
@@ -75,46 +77,52 @@
 from vdk.plugin.meta_jobs.meta_job_runner import MetaJobInput
 
 JOBS_RUN_ORDER = [
     {
         "job_name": "job1",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": []
     },
 
     {
         "job_name": "job2",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
     {
         "job_name": "job3",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
     {
         "job_name": "job4",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job1"]
     },
 
     {
         "job_name": "job5",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job3"]
     },
     {
         "job_name": "job6",
         "team_name": "team-awesome",
         "fail_meta_job_on_error": True,
+        "arguments": {},
         "depends_on": ["job3"]
     },
 ]
 
 
 def run(job_input: IJobInput) - > None:
     MetaJobInput().run_meta_job(JOBS_RUN_ORDER)
```

### Comparing `vdk-meta-jobs-0.1.824443273/src/vdk_meta_jobs.egg-info/SOURCES.txt` & `vdk-meta-jobs-0.1.833741966/src/vdk_meta_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.824443273/tests/test_meta_dag.py` & `vdk-meta-jobs-0.1.833741966/tests/test_meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.824443273/tests/test_meta_job.py` & `vdk-meta-jobs-0.1.833741966/tests/test_meta_job.py`

 * *Files 14% similar despite different names*

```diff
@@ -123,15 +123,18 @@
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             # CliEntryBasedTestRunner (provided by vdk-test-utils) gives a away to simulate vdk command
             # and mock large parts of it - e.g passed our own plugins
             result: Result = self.runner.invoke(
-                ["run", jobs_path_from_caller_directory(meta_job_name)]
+                [
+                    "run",
+                    jobs_path_from_caller_directory(meta_job_name),
+                ]
             )
 
             return result
 
     def _assert_meta_job_fails_with_error(self, result, error):
         with mock.patch.dict(
             os.environ,
@@ -323,15 +326,54 @@
 
     def test_meta_job_duplicate_jobs(self):
         self._test_meta_job_validation("meta-job-duplicate-jobs")
 
     def test_meta_job_not_allowed_job_key(self):
         self._test_meta_job_validation("meta-job-not-allowed-job-key")
 
+    def test_meta_job_wrong_job_arguments_type(self):
+        self._test_meta_job_validation("dag-wrong-job-arguments-type")
+
+    def test_meta_job_arguments(self):
+        self._set_up()
+        with mock.patch.dict(
+            os.environ,
+            self.env_vars,
+        ):
+            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            result = self._run_meta_job("dag-arguments")
+            cli_assert_equal(0, result)
+            job2_arguments = self._get_job_arguments("job2")
+            assert len(job2_arguments) == 2
+            assert job2_arguments == {"table_name": "test_table", "counter": 123}
+            self.httpserver.stop()
+
+    def test_meta_job_empty_arguments(self):
+        self._set_up()
+        with mock.patch.dict(
+            os.environ,
+            self.env_vars,
+        ):
+            self.runner = CliEntryBasedTestRunner(plugin_entry)
+            result = self._run_meta_job("dag-empty-arguments")
+            cli_assert_equal(0, result)
+            job2_arguments = self._get_job_arguments("job2")
+            assert len(job2_arguments) == 0
+            self.httpserver.stop()
+
     def test_meta_job_wrong_job_key_type(self):
         self._test_meta_job_validation("meta-job-wrong-job-key-type")
 
     def test_meta_job_wrong_job_type(self):
         self._test_meta_job_validation("meta-job-wrong-job-type")
 
     def test_meta_job_wrong_topological_order(self):
         self._test_meta_job_validation("meta-job-wrong-topological-order")
+
+    def _get_job_arguments(self, job_name: str):
+        job_post_req = [
+            req
+            for req, res in self.httpserver.log
+            if req.method == "POST"
+            and req.path.split("/jobs/")[1].split("/")[0] == job_name
+        ]
+        return job_post_req[0].json["args"]
```

### Comparing `vdk-meta-jobs-0.1.824443273/tests/test_time_based_queue.py` & `vdk-meta-jobs-0.1.833741966/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.824443273/tests/test_tracking_job_executor.py` & `vdk-meta-jobs-0.1.833741966/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

