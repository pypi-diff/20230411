# Comparing `tmp/samshee-0.1.2.tar.gz` & `tmp/samshee-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samshee-0.1.2.tar", last modified: Tue Apr 11 06:37:27 2023, max compression
+gzip compressed data, was "samshee-0.1.3.tar", last modified: Tue Apr 11 09:40:14 2023, max compression
```

## Comparing `samshee-0.1.2.tar` & `samshee-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.268862 samshee-0.1.2/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.2/LICENSE
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 06:37:27.268862 samshee-0.1.2/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.2/README.md
--rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-04-11 06:37:05.000000 samshee-0.1.2/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-04-11 06:37:27.268862 samshee-0.1.2/setup.cfg
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.265529 samshee-0.1.2/src/
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.265529 samshee-0.1.2/src/samshee/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.2/src/samshee/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.2/src/samshee/samplesheetv2.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.2/src/samshee/sectionedsheet.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    25990 2023-04-11 06:36:13.000000 samshee-0.1.2/src/samshee/validation.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.268862 samshee-0.1.2/src/samshee.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/top_level.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.268862 samshee-0.1.2/tests/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.2/tests/test_validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.3/LICENSE
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 09:40:14.245348 samshee-0.1.3/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.3/README.md
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-04-11 09:40:08.000000 samshee-0.1.3/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-04-11 09:40:14.245348 samshee-0.1.3/setup.cfg
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/src/
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/src/samshee/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.3/src/samshee/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.3/src/samshee/samplesheetv2.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.3/src/samshee/sectionedsheet.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    26109 2023-04-11 09:39:21.000000 samshee-0.1.3/src/samshee/validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/src/samshee.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-04-11 09:40:14.000000 samshee-0.1.3/src/samshee.egg-info/top_level.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 09:40:14.245348 samshee-0.1.3/tests/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.3/tests/test_validation.py
```

### Comparing `samshee-0.1.2/LICENSE` & `samshee-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `samshee-0.1.2/PKG-INFO` & `samshee-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.2
+Version: 0.1.3
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.2/README.md` & `samshee-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `samshee-0.1.2/pyproject.toml` & `samshee-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samshee"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Jakob Simeth", email="jakob.simeth@ukr.de" }
 ]
 description="A schema-agnostic parser and writer for illumina sample sheets v2."
 readme = "README.md"
 license={file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `samshee-0.1.2/src/samshee/samplesheetv2.py` & `samshee-0.1.3/src/samshee/samplesheetv2.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.2/src/samshee/sectionedsheet.py` & `samshee-0.1.3/src/samshee/sectionedsheet.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.2/src/samshee/validation.py` & `samshee-0.1.3/src/samshee/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,20 +327,23 @@
                         )
                         for index in index2
                     ]
                 ):
                     raise Exception(
                         f"(At least some) Second indices of the samples have a different length than what is specified in OverrideCycles ({minindex2length})"
                     )
-            # indices may be equal if on separate lanes:
+            else:
+                index = index1
+
+            # indices may be equal if on separate lanes, so we add the lane as an additional identifier prefix:
             if "Lane" in convertdata[0]:
                 lane = [i["Lane"] for i in convertdata]
                 index = [str(l) + i for l, i in zip(lane, index)]
-            else:
-                index = index1
+
+            # finally, check if there are non-unique indices:
             if len(set(index)) != len(index):
                 raise Exception("Indices are not unique.")
 
 
 def basespacelogic(doc: SectionedSheet) -> None:
     if "Cloud_Data" not in doc:
         raise Exception("no Cloud_Data section")
```

### Comparing `samshee-0.1.2/src/samshee.egg-info/PKG-INFO` & `samshee-0.1.3/src/samshee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.2
+Version: 0.1.3
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.2/tests/test_validation.py` & `samshee-0.1.3/tests/test_validation.py`

 * *Files identical despite different names*

