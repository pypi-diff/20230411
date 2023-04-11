# Comparing `tmp/samshee-0.1.1.tar.gz` & `tmp/samshee-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samshee-0.1.1.tar", last modified: Mon Mar 20 07:44:57 2023, max compression
+gzip compressed data, was "samshee-0.1.2.tar", last modified: Tue Apr 11 06:37:27 2023, max compression
```

## Comparing `samshee-0.1.1.tar` & `samshee-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-20 07:44:57.696167 samshee-0.1.1/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.1/LICENSE
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-03-20 07:44:57.696167 samshee-0.1.1/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.1/README.md
--rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-03-20 07:43:27.000000 samshee-0.1.1/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-03-20 07:44:57.696167 samshee-0.1.1/setup.cfg
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-20 07:44:57.696167 samshee-0.1.1/src/
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-20 07:44:57.696167 samshee-0.1.1/src/samshee/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.1/src/samshee/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.1/src/samshee/samplesheetv2.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.1/src/samshee/sectionedsheet.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    25229 2023-02-25 05:45:57.000000 samshee-0.1.1/src/samshee/validation.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-20 07:44:57.696167 samshee-0.1.1/src/samshee.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-03-20 07:44:57.000000 samshee-0.1.1/src/samshee.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-03-20 07:44:57.000000 samshee-0.1.1/src/samshee.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-03-20 07:44:57.000000 samshee-0.1.1/src/samshee.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-03-20 07:44:57.000000 samshee-0.1.1/src/samshee.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-03-20 07:44:57.000000 samshee-0.1.1/src/samshee.egg-info/top_level.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-20 07:44:57.696167 samshee-0.1.1/tests/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.1/tests/test_validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.268862 samshee-0.1.2/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.2/LICENSE
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 06:37:27.268862 samshee-0.1.2/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.2/README.md
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-04-11 06:37:05.000000 samshee-0.1.2/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-04-11 06:37:27.268862 samshee-0.1.2/setup.cfg
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.265529 samshee-0.1.2/src/
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.265529 samshee-0.1.2/src/samshee/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.2/src/samshee/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.2/src/samshee/samplesheetv2.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.2/src/samshee/sectionedsheet.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    25990 2023-04-11 06:36:13.000000 samshee-0.1.2/src/samshee/validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.268862 samshee-0.1.2/src/samshee.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-04-11 06:37:27.000000 samshee-0.1.2/src/samshee.egg-info/top_level.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-04-11 06:37:27.268862 samshee-0.1.2/tests/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.2/tests/test_validation.py
```

### Comparing `samshee-0.1.1/LICENSE` & `samshee-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `samshee-0.1.1/PKG-INFO` & `samshee-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.1
+Version: 0.1.2
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.1/README.md` & `samshee-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `samshee-0.1.1/pyproject.toml` & `samshee-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samshee"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Jakob Simeth", email="jakob.simeth@ukr.de" }
 ]
 description="A schema-agnostic parser and writer for illumina sample sheets v2."
 readme = "README.md"
 license={file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `samshee-0.1.1/src/samshee/samplesheetv2.py` & `samshee-0.1.2/src/samshee/samplesheetv2.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.1/src/samshee/sectionedsheet.py` & `samshee-0.1.2/src/samshee/sectionedsheet.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.1/src/samshee/validation.py` & `samshee-0.1.2/src/samshee/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,27 +314,31 @@
                     f"(At least some) First indices of the samples have a different length than what is specified in OverrideCycles ({minindex1length})"
                 )
 
             if "Index2" in convertdata[0]:
                 index2 = [i["Index2"] for i in convertdata]
                 index = [i1 + i2 for i1, i2 in zip(index1, index2)]
                 minindex2length = cycles["Index2Cycles"].count("I")
-                maxindex2length = len(cycles["Index1Cycles"])
+                maxindex2length = len(cycles["Index2Cycles"])
                 if not all(
                     [
                         (
                             len(index) >= minindex2length
                             and len(index) <= maxindex2length
                         )
                         for index in index2
                     ]
                 ):
                     raise Exception(
                         f"(At least some) Second indices of the samples have a different length than what is specified in OverrideCycles ({minindex2length})"
                     )
+            # indices may be equal if on separate lanes:
+            if "Lane" in convertdata[0]:
+                lane = [i["Lane"] for i in convertdata]
+                index = [str(l) + i for l, i in zip(lane, index)]
             else:
                 index = index1
             if len(set(index)) != len(index):
                 raise Exception("Indices are not unique.")
 
 
 def basespacelogic(doc: SectionedSheet) -> None:
@@ -384,15 +388,16 @@
         return sum([shorter[i] != longer[i] for i in range(len(shorter))])
 
     def index_distances(
         indices: list[list[str]],
     ) -> list[Tuple[list[int], list[str], list[str]]]:
         """returns the pairs of indices and their Hammon distances.
         Indices is an array to account for multiple indices.
-        For every pair, the array of distances (one for each index) and the two indices compared are returned"""
+        For every pair, the array of distances (one for each index) and the two indices compared are returned
+        """
         if len(indices) == 1:
             # if there is only one index entry, we return the one entry and the length of the indices
             return [([len(i) for i in indices[0]], indices[0], indices[0])]
         elif len(indices) == 0:
             raise Exception("no indices.")
 
         return [
@@ -413,55 +418,68 @@
         mismatchnames: list[str] | str,
         mindist: Optional[int] = None,
     ):
         if isinstance(indexnames, str):
             indexnames = [indexnames]
         if isinstance(mismatchnames, str):
             mismatchnames = [mismatchnames]
-        index = [
+        lanes = set(
             [
-                i[indexname] if indexname in i and i[indexname] is not None else ""
-                for indexname in indexnames
+                int(i["Lane"]) if "Lane" in i else 1
+                for i in cast(Data, doc["BCLConvert_Data"])
+            ]
+        )
+        for lane in lanes:
+            this_lane_data = [
+                i
+                for i in cast(Data, doc["BCLConvert_Data"])
+                if ("Lane" in i and int(i["Lane"]) == lane) or ("Lane" not in i)
             ]
-            for i in cast(Data, doc["BCLConvert_Data"])
-        ]
 
-        mismatches = [
-            cast(int, cast(Settings, doc["BCLConvert_Settings"])[mismatchname])
-            if mismatchname in doc["BCLConvert_Settings"]
-            else 1
-            for mismatchname in mismatchnames
-        ]
+            index = [
+                [
+                    i[indexname] if indexname in i and i[indexname] is not None else ""
+                    for indexname in indexnames
+                ]
+                for i in this_lane_data
+            ]
 
-        indexdist = index_distances(index)
-        matchingindices = [
-            t
-            for t in indexdist
-            if all([t[0][i] <= mismatches[i] for i in range(len(mismatches))])
-        ]
-        if len(matchingindices) > 0:
-            msg = "Indices are too close and undistinguishable: "
-            for matchingindex in matchingindices:
-                msg += f"Entries of index pair ({str(matchingindex[1])}, {str(matchingindex[2])}) are undistinguishable because "
-                for i, indexname in enumerate(indexnames):
-                    if matchingindex[0][i] <= mismatches[i]:
-                        msg += f"{indexname} differs by {matchingindex[0][i]} <= {mismatches[i]} "
-                msg += ". "
-            raise Exception(msg)
-
-        if mindist is not None:
-            combined = [["".join(i)] for i in index]
-            indexdist = index_distances(combined)
-            matchingindices = [t for t in indexdist if all([t[0][0] < mindist])]
+            mismatches = [
+                cast(int, cast(Settings, doc["BCLConvert_Settings"])[mismatchname])
+                if mismatchname in doc["BCLConvert_Settings"]
+                else 1
+                for mismatchname in mismatchnames
+            ]
+
+            indexdist = index_distances(index)
+            matchingindices = [
+                t
+                for t in indexdist
+                if all([t[0][i] <= mismatches[i] for i in range(len(mismatches))])
+            ]
             if len(matchingindices) > 0:
-                msg = "Combined index is too close and undistinguishable: "
+                msg = "Indices are too close and undistinguishable: "
                 for matchingindex in matchingindices:
-                    msg += f"Entries of index pair ({str(matchingindex[1])}, {str(matchingindex[2])}) are undistinguishable because their distance is {matchingindex[0][0]} < {mindist} (which is the explicitly given combined minimal distance)"
+                    msg += f"Entries of index pair ({str(matchingindex[1])}, {str(matchingindex[2])}) are undistinguishable because "
+                    for i, indexname in enumerate(indexnames):
+                        if matchingindex[0][i] <= mismatches[i]:
+                            msg += f"{indexname} differs by {matchingindex[0][i]} <= {mismatches[i]} "
+                    msg += ". "
                 raise Exception(msg)
 
+            if mindist is not None:
+                combined = [["".join(i)] for i in index]
+                indexdist = index_distances(combined)
+                matchingindices = [t for t in indexdist if all([t[0][0] < mindist])]
+                if len(matchingindices) > 0:
+                    msg = "Combined index is too close and undistinguishable: "
+                    for matchingindex in matchingindices:
+                        msg += f"Entries of index pair ({str(matchingindex[1])}, {str(matchingindex[2])}) are undistinguishable because their distance is {matchingindex[0][0]} < {mindist} (which is the explicitly given combined minimal distance)"
+                    raise Exception(msg)
+
     convdata = cast(Data, doc["BCLConvert_Data"])
     if "Index" in convdata[0] and "Index2" in convdata[0]:
         check_index(
             doc,
             ["Index", "Index2"],
             ["BarcodeMismatchesIndex1", "BarcodeMismatchesIndex2"],
             mindist,
```

### Comparing `samshee-0.1.1/src/samshee.egg-info/PKG-INFO` & `samshee-0.1.2/src/samshee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.1
+Version: 0.1.2
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.1/tests/test_validation.py` & `samshee-0.1.2/tests/test_validation.py`

 * *Files identical despite different names*

