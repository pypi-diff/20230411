# Comparing `tmp/np-session-0.5.0.tar.gz` & `tmp/np-session-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.5.0.tar", last modified: Tue Apr  4 00:50:16 2023, max compression
+gzip compressed data, was "np-session-0.5.1.tar", last modified: Tue Apr 11 20:30:52 2023, max compression
```

## Comparing `np-session-0.5.0.tar` & `np-session-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2113 2023-04-04 00:49:02.091818 np-session-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.0/README.md
--rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.0/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.0/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     7781 2023-04-03 23:30:20.220124 np-session-0.5.0/src/np_session/components/info.py
--rw-r--r--   0        0        0     7708 2023-03-23 23:41:50.844242 np-session-0.5.0/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.0/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.0/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.0/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.0/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.0/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.0/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.0/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.0/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.0/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.0/src/np_session/databases/sql_alchemy.py
--rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.0/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.0/src/np_session/jobs/find_missing_files.py
--rw-r--r--   0        0        0        0 2023-03-19 18:03:04.930628 np-session-0.5.0/src/np_session/jobs/generate_session_summaries.py
--rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.0/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.0/src/np_session/jobs/probes.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.0/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.0/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0    25576 2023-03-29 21:44:41.257200 np-session-0.5.0/src/np_session/session.py
--rw-r--r--   0        0        0     8288 2023-03-17 05:14:59.167647 np-session-0.5.0/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.0/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.0/tests/test_platform_json.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2113 2023-04-11 20:30:41.750465 np-session-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.1/README.md
+-rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.1/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.1/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     7972 2023-04-11 20:30:10.239218 np-session-0.5.1/src/np_session/components/info.py
+-rw-r--r--   0        0        0     7708 2023-03-23 23:41:50.844242 np-session-0.5.1/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.1/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.1/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.1/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.1/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.1/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.1/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.1/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.1/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.1/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.1/src/np_session/databases/sql_alchemy.py
+-rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.1/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.1/src/np_session/jobs/find_missing_files.py
+-rw-r--r--   0        0        0        0 2023-03-19 18:03:04.930628 np-session-0.5.1/src/np_session/jobs/generate_session_summaries.py
+-rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.1/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.1/src/np_session/jobs/probes.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.1/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.1/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0    25576 2023-03-29 21:44:41.257200 np-session-0.5.1/src/np_session/session.py
+-rw-r--r--   0        0        0     8288 2023-03-17 05:14:59.167647 np-session-0.5.1/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.1/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.1/tests/test_platform_json.py
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.1/PKG-INFO
```

### Comparing `np-session-0.5.0/pyproject.toml` & `np-session-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.5.0"
+version = "0.5.1"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np-session-0.5.0/README.md` & `np-session-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/components/info.py` & `np-session-0.5.1/src/np_session/components/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import abc
 import datetime
 import enum
 import functools
 import time
-from typing import Any, MutableMapping, Optional
-
+from typing import Any, ClassVar, MutableMapping, Optional
 
+import np_config
 import np_logging
 from backports.cached_property import cached_property
 from typing_extensions import Literal
 
 from np_session.databases import State
 from np_session.databases.lims2 import (LIMS2MouseInfo, LIMS2ProjectInfo,
                                         LIMS2UserInfo)
@@ -182,52 +182,55 @@
             logger.error("Failed to load `%r.state`: %r", self, exc)
         return {}
     
 class Dye(WithState):
     """Info about a DiI or DiO dye.
     
     >>> dye = Dye(1)
-    >>> dye.dii_description
+    >>> dye.description
     'CM-DiI 100%'
     >>> dye.previous_uses = 0
     >>> dye.record_first_use(time.time())
     >>> dye.increment_uses()
     >>> dye.previous_uses
     1
     """
     
+    descriptions: ClassVar = ('CM-DiI 100%', 'DiO')
+    
     def __init__(self, dye_id: int) -> None:
         self.id = int(dye_id)
         
     @property
     def previous_uses(self) -> int:
         return self.state.setdefault('previous_uses', 0)
     
     @previous_uses.setter
     def previous_uses(self, value: int) -> None:
         self.state['previous_uses'] = int(value)
     
     @property
-    def dii_description(self) -> Literal['CM-DiI 100%', 'DiO']:
-        return self.state.setdefault('dii_description', 'CM-DiI 100%')
+    def description(self) -> Literal['CM-DiI` 100%', 'DiO']:
+        return self.state.setdefault('description', self.descriptions[0])
     
-    @dii_description.setter
-    def dii_description(self, value: Literal['CM-DiI 100%', 'DiO']) -> None:
-        self.state['dii_description'] = value
+    @description.setter
+    def description(self, value: Literal['CM-DiI 100%', 'DiO']) -> None:
+        self.state['description'] = value
     
     @property
     def first_use(self) -> datetime.datetime | None:
         first_use: float | None = self.state.get('first_use')
         return datetime.datetime.fromtimestamp(first_use) if first_use else None
     
-    def record_first_use(self, timestamp: Optional[float] = None) -> None:
+    def record_first_use(self, timestamp: Optional[datetime.datetime | float] = None) -> None:
         """Record the time this dye was first used.
         
         Supply a `time.time()`, else the current time will be recorded.
         """
+        timestamp = timestamp.timestamp() if isinstance(timestamp, datetime.datetime) else timestamp
         self.state['first_use'] = time.time() if timestamp is None else timestamp
     
     def increment_uses(self):
         """Increment the number of times this dye has been used."""
         previous_uses = self.previous_uses
         if previous_uses == 0:
             self.record_first_use()
```

### Comparing `np-session-0.5.0/src/np_session/components/lims_manifests.py` & `np-session-0.5.1/src/np_session/components/lims_manifests.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/components/paths.py` & `np-session-0.5.1/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/components/platform_json.py` & `np-session-0.5.1/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/components/settings_xml.py` & `np-session-0.5.1/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/databases/data_getters.py` & `np-session-0.5.1/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/databases/firebase_state.py` & `np-session-0.5.1/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/databases/lims2.py` & `np-session-0.5.1/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/databases/mtrain.py` & `np-session-0.5.1/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/databases/redis_state.py` & `np-session-0.5.1/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/databases/sql_alchemy.py` & `np-session-0.5.1/src/np_session/databases/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/jobs/lims_upload.py` & `np-session-0.5.1/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/jobs/probes.py` & `np-session-0.5.1/src/np_session/jobs/probes.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/jobs/sessions.json` & `np-session-0.5.1/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/jobs/sync_states.py` & `np-session-0.5.1/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/session.py` & `np-session-0.5.1/src/np_session/session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/src/np_session/utils.py` & `np-session-0.5.1/src/np_session/utils.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/tests/test_platform_json.py` & `np-session-0.5.1/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.0/PKG-INFO` & `np-session-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```

