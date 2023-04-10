# Comparing `tmp/plantuml_sequence-0.2.0.tar.gz` & `tmp/plantuml_sequence-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantuml_sequence-0.2.0.tar", max compression
+gzip compressed data, was "plantuml_sequence-0.2.1.tar", max compression
```

## Comparing `plantuml_sequence-0.2.0.tar` & `plantuml_sequence-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-06 10:03:16.416578 plantuml_sequence-0.2.0/LICENSE
--rw-r--r--   0        0        0     2410 2023-04-10 15:28:49.331488 plantuml_sequence-0.2.0/README.md
--rw-r--r--   0        0        0       52 2023-04-10 15:36:43.909170 plantuml_sequence-0.2.0/plantuml_sequence/__init__.py
--rw-r--r--   0        0        0    15464 2023-04-10 17:07:01.248505 plantuml_sequence-0.2.0/plantuml_sequence/diagram.py
--rw-r--r--   0        0        0        0 2023-04-10 10:02:31.709709 plantuml_sequence-0.2.0/plantuml_sequence/py.typed
--rw-r--r--   0        0        0     4783 2023-04-10 10:12:37.459284 plantuml_sequence-0.2.0/plantuml_sequence/utils.py
--rw-r--r--   0        0        0     2280 2023-04-10 17:07:39.827583 plantuml_sequence-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 plantuml_sequence-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-06 10:03:16.416578 plantuml_sequence-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2410 2023-04-10 15:28:49.331488 plantuml_sequence-0.2.1/README.md
+-rw-r--r--   0        0        0       52 2023-04-10 15:36:43.909170 plantuml_sequence-0.2.1/plantuml_sequence/__init__.py
+-rw-r--r--   0        0        0    15461 2023-04-10 22:38:30.196747 plantuml_sequence-0.2.1/plantuml_sequence/diagram.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:02:31.709709 plantuml_sequence-0.2.1/plantuml_sequence/py.typed
+-rw-r--r--   0        0        0     4783 2023-04-10 10:12:37.459284 plantuml_sequence-0.2.1/plantuml_sequence/utils.py
+-rw-r--r--   0        0        0     2280 2023-04-10 22:40:51.315252 plantuml_sequence-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 plantuml_sequence-0.2.1/PKG-INFO
```

### Comparing `plantuml_sequence-0.2.0/LICENSE` & `plantuml_sequence-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plantuml_sequence-0.2.0/README.md` & `plantuml_sequence-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `plantuml_sequence-0.2.0/plantuml_sequence/diagram.py` & `plantuml_sequence-0.2.1/plantuml_sequence/diagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         :type participant: Participant | str
         :param color: Color of the active lifeline, defaults to ""
         :type color: str, optional
         :return: Sequence diagram instance
         :rtype: Self
         """
         alias = participant_to_string(participant)
-        self._line_writer.writeline(f"deactivate {alias}")
+        self._line_writer.writeline(f"destroy {alias}")
         return self
 
     def delay(self, msg: str | None = None) -> Self:
         """
         Indicate a delay in the diagram
 
         :param msg: Message to add to the delay, defaults to None
```

### Comparing `plantuml_sequence-0.2.0/plantuml_sequence/utils.py` & `plantuml_sequence-0.2.1/plantuml_sequence/utils.py`

 * *Files identical despite different names*

### Comparing `plantuml_sequence-0.2.0/pyproject.toml` & `plantuml_sequence-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plantuml-sequence"
-version = "0.2.0"
+version = "0.2.1"
 description = "Create PlantUML sequence charts programmatically from Python"
 authors = ["Jonas Ehrlich <jonas.ehrlich@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/jonasehrlich/plantuml-sequence"
 repository = "https://github.com/jonasehrlich/plantuml-sequence"
 keywords = ["plantuml", "charts"]
```

### Comparing `plantuml_sequence-0.2.0/PKG-INFO` & `plantuml_sequence-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-sequence
-Version: 0.2.0
+Version: 0.2.1
 Summary: Create PlantUML sequence charts programmatically from Python
 Home-page: https://github.com/jonasehrlich/plantuml-sequence
 License: MIT
 Keywords: plantuml,charts
 Author: Jonas Ehrlich
 Author-email: jonas.ehrlich@gmail.com
 Requires-Python: >=3.10
```

