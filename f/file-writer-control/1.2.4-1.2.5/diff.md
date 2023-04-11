# Comparing `tmp/file_writer_control-1.2.4.tar.gz` & `tmp/file_writer_control-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_writer_control-1.2.4.tar", last modified: Mon Feb 20 07:29:44 2023, max compression
+gzip compressed data, was "file_writer_control-1.2.5.tar", last modified: Tue Apr 11 12:27:51 2023, max compression
```

## Comparing `file_writer_control-1.2.4.tar` & `file_writer_control-1.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwx------   0 dd        (1000) dd        (1000)        0 2023-02-20 07:29:44.904058 file_writer_control-1.2.4/
--rw-------   0 dd        (1000) dd        (1000)     1374 2022-09-05 11:46:57.000000 file_writer_control-1.2.4/LICENSE
--rw-------   0 dd        (1000) dd        (1000)     2359 2023-02-20 07:29:44.904058 file_writer_control-1.2.4/PKG-INFO
--rw-------   0 dd        (1000) dd        (1000)     1991 2022-09-05 11:46:57.000000 file_writer_control-1.2.4/README.md
-drwx------   0 dd        (1000) dd        (1000)        0 2023-02-20 07:29:44.900058 file_writer_control-1.2.4/cli/
--rw-------   0 dd        (1000) dd        (1000)        0 2022-09-05 11:46:57.000000 file_writer_control-1.2.4/cli/__init__.py
--rw-------   0 dd        (1000) dd        (1000)     6882 2022-09-05 11:46:57.000000 file_writer_control-1.2.4/cli/start_file_writer.py
--rw-------   0 dd        (1000) dd        (1000)     4148 2022-09-05 11:46:57.000000 file_writer_control-1.2.4/cli/stop_file_writer.py
-drwx------   0 dd        (1000) dd        (1000)        0 2023-02-20 07:29:44.904058 file_writer_control-1.2.4/file_writer_control/
--rw-------   0 dd        (1000) dd        (1000)     8953 2023-02-19 15:51:31.000000 file_writer_control-1.2.4/file_writer_control/CommandChannel.py
--rw-------   0 dd        (1000) dd        (1000)     2244 2023-02-19 15:51:31.000000 file_writer_control-1.2.4/file_writer_control/CommandHandler.py
--rw-r--r--   0 dd        (1000) dd        (1000)     4517 2023-01-30 14:56:06.000000 file_writer_control-1.2.4/file_writer_control/CommandStatus.py
--rw-------   0 dd        (1000) dd        (1000)    10196 2023-02-20 07:28:39.000000 file_writer_control-1.2.4/file_writer_control/InThreadStatusTracker.py
--rw-------   0 dd        (1000) dd        (1000)     4296 2023-02-20 07:28:39.000000 file_writer_control-1.2.4/file_writer_control/JobHandler.py
--rw-------   0 dd        (1000) dd        (1000)     4343 2023-02-19 15:51:31.000000 file_writer_control-1.2.4/file_writer_control/JobStatus.py
--rw-------   0 dd        (1000) dd        (1000)      736 2023-02-19 15:51:31.000000 file_writer_control-1.2.4/file_writer_control/KafkaTopicUrl.py
--rw-r--r--   0 dd        (1000) dd        (1000)     2068 2023-01-30 14:56:06.000000 file_writer_control-1.2.4/file_writer_control/StateExtractor.py
--rw-------   0 dd        (1000) dd        (1000)     5979 2023-02-20 07:28:39.000000 file_writer_control-1.2.4/file_writer_control/WorkerFinder.py
--rw-r--r--   0 dd        (1000) dd        (1000)     2839 2023-01-30 14:56:06.000000 file_writer_control-1.2.4/file_writer_control/WorkerJobPool.py
--rw-r--r--   0 dd        (1000) dd        (1000)     2733 2023-01-30 14:56:06.000000 file_writer_control-1.2.4/file_writer_control/WorkerStatus.py
--rw-------   0 dd        (1000) dd        (1000)     2721 2023-02-19 15:51:31.000000 file_writer_control-1.2.4/file_writer_control/WriteJob.py
--rw-r--r--   0 dd        (1000) dd        (1000)      330 2023-01-30 14:56:06.000000 file_writer_control-1.2.4/file_writer_control/__init__.py
--rw-------   0 dd        (1000) dd        (1000)      180 2023-02-20 07:28:39.000000 file_writer_control-1.2.4/file_writer_control/_version.py
-drwx------   0 dd        (1000) dd        (1000)        0 2023-02-20 07:29:44.904058 file_writer_control-1.2.4/file_writer_control.egg-info/
--rw-------   0 dd        (1000) dd        (1000)     2359 2023-02-20 07:29:44.000000 file_writer_control-1.2.4/file_writer_control.egg-info/PKG-INFO
--rw-------   0 dd        (1000) dd        (1000)      856 2023-02-20 07:29:44.000000 file_writer_control-1.2.4/file_writer_control.egg-info/SOURCES.txt
--rw-------   0 dd        (1000) dd        (1000)        1 2023-02-20 07:29:44.000000 file_writer_control-1.2.4/file_writer_control.egg-info/dependency_links.txt
--rw-------   0 dd        (1000) dd        (1000)      126 2023-02-20 07:29:44.000000 file_writer_control-1.2.4/file_writer_control.egg-info/entry_points.txt
--rw-------   0 dd        (1000) dd        (1000)       51 2023-02-20 07:29:44.000000 file_writer_control-1.2.4/file_writer_control.egg-info/requires.txt
--rw-------   0 dd        (1000) dd        (1000)       24 2023-02-20 07:29:44.000000 file_writer_control-1.2.4/file_writer_control.egg-info/top_level.txt
--rw-------   0 dd        (1000) dd        (1000)       38 2023-02-20 07:29:44.904058 file_writer_control-1.2.4/setup.cfg
--rw-------   0 dd        (1000) dd        (1000)     1228 2022-09-05 11:46:57.000000 file_writer_control-1.2.4/setup.py
+drwx------   0 dd        (1000) dd        (1000)        0 2023-04-11 12:27:51.488841 file_writer_control-1.2.5/
+-rw-------   0 dd        (1000) dd        (1000)     1374 2022-09-05 11:46:57.000000 file_writer_control-1.2.5/LICENSE
+-rw-------   0 dd        (1000) dd        (1000)     2359 2023-04-11 12:27:51.488841 file_writer_control-1.2.5/PKG-INFO
+-rw-------   0 dd        (1000) dd        (1000)     1991 2022-09-05 11:46:57.000000 file_writer_control-1.2.5/README.md
+drwx------   0 dd        (1000) dd        (1000)        0 2023-04-11 12:27:51.488841 file_writer_control-1.2.5/cli/
+-rw-------   0 dd        (1000) dd        (1000)        0 2022-09-05 11:46:57.000000 file_writer_control-1.2.5/cli/__init__.py
+-rw-------   0 dd        (1000) dd        (1000)     6882 2022-09-05 11:46:57.000000 file_writer_control-1.2.5/cli/start_file_writer.py
+-rw-------   0 dd        (1000) dd        (1000)     4148 2022-09-05 11:46:57.000000 file_writer_control-1.2.5/cli/stop_file_writer.py
+drwx------   0 dd        (1000) dd        (1000)        0 2023-04-11 12:27:51.488841 file_writer_control-1.2.5/file_writer_control/
+-rw-------   0 dd        (1000) dd        (1000)     8953 2023-02-19 15:51:31.000000 file_writer_control-1.2.5/file_writer_control/CommandChannel.py
+-rw-------   0 dd        (1000) dd        (1000)     2244 2023-02-19 15:51:31.000000 file_writer_control-1.2.5/file_writer_control/CommandHandler.py
+-rw-r--r--   0 dd        (1000) dd        (1000)     4517 2023-01-30 14:56:06.000000 file_writer_control-1.2.5/file_writer_control/CommandStatus.py
+-rw-------   0 dd        (1000) dd        (1000)    10196 2023-02-20 07:28:39.000000 file_writer_control-1.2.5/file_writer_control/InThreadStatusTracker.py
+-rw-------   0 dd        (1000) dd        (1000)     4296 2023-02-20 07:28:39.000000 file_writer_control-1.2.5/file_writer_control/JobHandler.py
+-rw-------   0 dd        (1000) dd        (1000)     4417 2023-04-11 12:19:30.000000 file_writer_control-1.2.5/file_writer_control/JobStatus.py
+-rw-------   0 dd        (1000) dd        (1000)      736 2023-02-19 15:51:31.000000 file_writer_control-1.2.5/file_writer_control/KafkaTopicUrl.py
+-rw-r--r--   0 dd        (1000) dd        (1000)     2068 2023-01-30 14:56:06.000000 file_writer_control-1.2.5/file_writer_control/StateExtractor.py
+-rw-------   0 dd        (1000) dd        (1000)     5979 2023-02-20 07:28:39.000000 file_writer_control-1.2.5/file_writer_control/WorkerFinder.py
+-rw-r--r--   0 dd        (1000) dd        (1000)     2839 2023-01-30 14:56:06.000000 file_writer_control-1.2.5/file_writer_control/WorkerJobPool.py
+-rw-r--r--   0 dd        (1000) dd        (1000)     2827 2023-04-11 12:18:34.000000 file_writer_control-1.2.5/file_writer_control/WorkerStatus.py
+-rw-------   0 dd        (1000) dd        (1000)     2721 2023-02-19 15:51:31.000000 file_writer_control-1.2.5/file_writer_control/WriteJob.py
+-rw-r--r--   0 dd        (1000) dd        (1000)      330 2023-01-30 14:56:06.000000 file_writer_control-1.2.5/file_writer_control/__init__.py
+-rw-------   0 dd        (1000) dd        (1000)      180 2023-04-11 12:20:06.000000 file_writer_control-1.2.5/file_writer_control/_version.py
+drwx------   0 dd        (1000) dd        (1000)        0 2023-04-11 12:27:51.488841 file_writer_control-1.2.5/file_writer_control.egg-info/
+-rw-------   0 dd        (1000) dd        (1000)     2359 2023-04-11 12:27:51.000000 file_writer_control-1.2.5/file_writer_control.egg-info/PKG-INFO
+-rw-------   0 dd        (1000) dd        (1000)      856 2023-04-11 12:27:51.000000 file_writer_control-1.2.5/file_writer_control.egg-info/SOURCES.txt
+-rw-------   0 dd        (1000) dd        (1000)        1 2023-04-11 12:27:51.000000 file_writer_control-1.2.5/file_writer_control.egg-info/dependency_links.txt
+-rw-------   0 dd        (1000) dd        (1000)      126 2023-04-11 12:27:51.000000 file_writer_control-1.2.5/file_writer_control.egg-info/entry_points.txt
+-rw-------   0 dd        (1000) dd        (1000)       51 2023-04-11 12:27:51.000000 file_writer_control-1.2.5/file_writer_control.egg-info/requires.txt
+-rw-------   0 dd        (1000) dd        (1000)       24 2023-04-11 12:27:51.000000 file_writer_control-1.2.5/file_writer_control.egg-info/top_level.txt
+-rw-------   0 dd        (1000) dd        (1000)       38 2023-04-11 12:27:51.488841 file_writer_control-1.2.5/setup.cfg
+-rw-------   0 dd        (1000) dd        (1000)     1228 2022-09-05 11:46:57.000000 file_writer_control-1.2.5/setup.py
```

### Comparing `file_writer_control-1.2.4/LICENSE` & `file_writer_control-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/PKG-INFO` & `file_writer_control-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_writer_control
-Version: 1.2.4
+Version: 1.2.5
 Summary: A small Python library for controlling the ESS kafka-to-nexus file-writer.
 Home-page: https://github.com/ess-dmsc/file_writer_control
 Author: ScreamingUdder
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `file_writer_control-1.2.4/README.md` & `file_writer_control-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/cli/start_file_writer.py` & `file_writer_control-1.2.5/cli/start_file_writer.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/cli/stop_file_writer.py` & `file_writer_control-1.2.5/cli/stop_file_writer.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/CommandChannel.py` & `file_writer_control-1.2.5/file_writer_control/CommandChannel.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/CommandHandler.py` & `file_writer_control-1.2.5/file_writer_control/CommandHandler.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/CommandStatus.py` & `file_writer_control-1.2.5/file_writer_control/CommandStatus.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/InThreadStatusTracker.py` & `file_writer_control-1.2.5/file_writer_control/InThreadStatusTracker.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/JobHandler.py` & `file_writer_control-1.2.5/file_writer_control/JobHandler.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/JobStatus.py` & `file_writer_control-1.2.5/file_writer_control/JobStatus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime, timedelta
 from enum import Enum, auto
 from typing import Optional, Dict
 
-JOB_STATUS_TIMEOUT = timedelta(seconds=5)
+
+DEFAULT_TIMEOUT = timedelta(seconds=15)
 
 
 class JobState(Enum):
     """
     The state of a job.
     """
 
@@ -20,16 +21,17 @@
 
 
 class JobStatus:
     """
     Contains general information about the (execution) of a job.
     """
 
-    def __init__(self, job_id: str):
+    def __init__(self, job_id: str, timeout: Optional[timedelta] = DEFAULT_TIMEOUT):
         self._job_id = job_id
+        self._timeout = timeout
         self._service_id = ""
         self._file_name = ""
         self._last_update = datetime.now()
         self._state = JobState.WAITING
         self._metadata: Optional[Dict] = None
         self._message = ""
 
@@ -56,15 +58,15 @@
         Given the current time, state and the time of the last update: Have we lost the connection?
         :param current_time: The current time
         """
         if (
             self.state != JobState.DONE
             and self.state != JobState.ERROR
             and self.state != JobState.TIMEOUT
-            and current_time - self.last_update > JOB_STATUS_TIMEOUT
+            and current_time - self.last_update > self._timeout
         ):
             self._state = JobState.TIMEOUT
             self._last_update = current_time
 
     @property
     def job_id(self) -> str:
         """
```

### Comparing `file_writer_control-1.2.4/file_writer_control/KafkaTopicUrl.py` & `file_writer_control-1.2.5/file_writer_control/KafkaTopicUrl.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/StateExtractor.py` & `file_writer_control-1.2.5/file_writer_control/StateExtractor.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/WorkerFinder.py` & `file_writer_control-1.2.5/file_writer_control/WorkerFinder.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/WorkerJobPool.py` & `file_writer_control-1.2.5/file_writer_control/WorkerJobPool.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control/WorkerStatus.py` & `file_writer_control-1.2.5/file_writer_control/WorkerStatus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime, timedelta
 from enum import Enum, auto
+from typing import Optional
 
-STATUS_MESSAGE_TIMEOUT = timedelta(seconds=5)
+
+DEFAULT_TIMEOUT = timedelta(seconds=15)
 
 
 class WorkerState(Enum):
     """
     The state of a worker (i.e. a file-writer instance).
     """
 
@@ -16,17 +18,18 @@
 
 
 class WorkerStatus(object):
     """
     Contains general status information about a worker.
     """
 
-    def __init__(self, service_id: str):
+    def __init__(self, service_id: str, timeout: Optional[timedelta] = DEFAULT_TIMEOUT):
         self._last_update = datetime.now()
         self._service_id = service_id
+        self._timeout = timeout
         self._state = WorkerState.UNAVAILABLE
 
     def __eq__(self, other_status: "WorkerStatus") -> bool:
         if not isinstance(other_status, WorkerStatus):
             raise NotImplementedError
         return (
             self.service_id == other_status.service_id
@@ -49,15 +52,15 @@
     def check_if_outdated(self, current_time: datetime):
         """
         Given the current time, state and the time of the last update: Have we lost the connection?
         :param current_time: The current time
         """
         if (
             self.state != WorkerState.UNAVAILABLE
-            and current_time - self.last_update > STATUS_MESSAGE_TIMEOUT
+            and current_time - self.last_update > self._timeout
         ):
             self._state = WorkerState.UNAVAILABLE
             self._last_update = current_time
 
     @property
     def state(self) -> WorkerState:
         """
```

### Comparing `file_writer_control-1.2.4/file_writer_control/WriteJob.py` & `file_writer_control-1.2.5/file_writer_control/WriteJob.py`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/file_writer_control.egg-info/PKG-INFO` & `file_writer_control-1.2.5/file_writer_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-writer-control
-Version: 1.2.4
+Version: 1.2.5
 Summary: A small Python library for controlling the ESS kafka-to-nexus file-writer.
 Home-page: https://github.com/ess-dmsc/file_writer_control
 Author: ScreamingUdder
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `file_writer_control-1.2.4/file_writer_control.egg-info/SOURCES.txt` & `file_writer_control-1.2.5/file_writer_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `file_writer_control-1.2.4/setup.py` & `file_writer_control-1.2.5/setup.py`

 * *Files identical despite different names*

