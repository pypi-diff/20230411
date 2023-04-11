# Comparing `tmp/simsity-0.5.2.tar.gz` & `tmp/simsity-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simsity-0.5.2.tar", last modified: Tue Apr  4 14:26:43 2023, max compression
+gzip compressed data, was "dist/simsity-0.5.3.tar", last modified: Tue Apr 11 14:16:26 2023, max compression
```

## Comparing `simsity-0.5.2.tar` & `simsity-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-04 14:26:43.309880 simsity-0.5.2/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3220 2023-04-04 14:26:43.309880 simsity-0.5.2/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1818 2023-03-28 14:29:00.000000 simsity-0.5.2/README.md
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-04 14:26:43.309880 simsity-0.5.2/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1393 2023-04-01 13:23:49.000000 simsity-0.5.2/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-04 14:26:43.309880 simsity-0.5.2/simsity/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3875 2023-04-01 13:23:46.000000 simsity-0.5.2/simsity/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1015 2023-03-28 14:20:47.000000 simsity-0.5.2/simsity/datasets.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2022-12-20 12:12:03.000000 simsity-0.5.2/simsity/error.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-04 14:26:43.309880 simsity-0.5.2/simsity.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3220 2023-04-04 14:26:43.000000 simsity-0.5.2/simsity.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      229 2023-04-04 14:26:43.000000 simsity-0.5.2/simsity.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-04 14:26:43.000000 simsity-0.5.2/simsity.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      150 2023-04-04 14:26:43.000000 simsity-0.5.2/simsity.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-04 14:26:43.000000 simsity-0.5.2/simsity.egg-info/top_level.txt
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 14:16:26.256640 simsity-0.5.3/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-11 14:16:26.256640 simsity-0.5.3/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1827 2023-04-11 13:48:43.000000 simsity-0.5.3/README.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-11 14:16:26.256640 simsity-0.5.3/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1399 2023-04-11 14:07:41.000000 simsity-0.5.3/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 14:16:26.256640 simsity-0.5.3/simsity/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4062 2023-04-11 14:03:54.000000 simsity-0.5.3/simsity/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1015 2023-03-28 14:20:47.000000 simsity-0.5.3/simsity/datasets.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2022-12-20 12:12:03.000000 simsity-0.5.3/simsity/error.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-11 14:16:26.256640 simsity-0.5.3/simsity.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      229 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      150 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-11 14:16:26.000000 simsity-0.5.3/simsity.egg-info/top_level.txt
```

### Comparing `simsity-0.5.2/PKG-INFO` & `simsity-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: simsity
-Version: 0.5.2
-Summary: Simple Similarity Service
+Version: 0.5.3
+Summary: Super Simple Similarity Service
 Home-page: https://github.com/koaning/simsity/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/koaning/simsity/
 Project-URL: Source Code, https://github.com/koaning/simsity/
 Project-URL: Issue Tracker, https://github.com/koaning/simsity/issues
 Description: 
@@ -53,16 +53,16 @@
         encoder = SentenceEncoder()
         
         # Populate the ANN vector index and use it. 
         index = create_index(recipes, encoder)
         texts, dists = index.query("pork")
         
         # You can also query using vectors
-        v_pork = encoder.transform("pork")[0]
-        texts, dists = index.query(v_pork)
+        v_pork = encoder.transform(["pork"])[0]
+        texts, dists = index.query_vector(v_pork)
         ```
         
         You can also provide a path and then you'll be able to store/load everything.
         
         ```python
         # Make an index with a path
         index = create_index(recipes, encoder, path="demo")
```

### Comparing `simsity-0.5.2/README.md` & `simsity-0.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 encoder = SentenceEncoder()
 
 # Populate the ANN vector index and use it. 
 index = create_index(recipes, encoder)
 texts, dists = index.query("pork")
 
 # You can also query using vectors
-v_pork = encoder.transform("pork")[0]
-texts, dists = index.query(v_pork)
+v_pork = encoder.transform(["pork"])[0]
+texts, dists = index.query_vector(v_pork)
 ```
 
 You can also provide a path and then you'll be able to store/load everything.
 
 ```python
 # Make an index with a path
 index = create_index(recipes, encoder, path="demo")
```

### Comparing `simsity-0.5.2/setup.py` & `simsity-0.5.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 all_packages = base_packages
 dev_packages = all_packages + test_packages
 
 
 setup(
     name="simsity",
-    version="0.5.2",
+    version="0.5.3",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
-    description="Simple Similarity Service",
+    description="Super Simple Similarity Service",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/koaning/simsity/",
     project_urls={
         "Documentation": "https://github.com/koaning/simsity/",
         "Source Code": "https://github.com/koaning/simsity/",
         "Issue Tracker": "https://github.com/koaning/simsity/issues",
```

### Comparing `simsity-0.5.2/simsity/__init__.py` & `simsity-0.5.3/simsity/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from pathlib import Path
 from typing import Iterable, Protocol
 
 import srsly
 from hnswlib import Index
 from tqdm import tqdm
 
+DB_NAME = "db.gz.json"
+INDEX_NAME = "index.bin"
+METADATA_NAME = "metadata.json"
+
 
 class Transformer(Protocol):
     def transform(self):
         pass
 
 
 class SimSityIndex:
@@ -26,36 +30,37 @@
         """
         Query using approximate nearest neighbors
 
         The object handles the encoder/data from disk.
         """
         arr = self.encoder.transform(query)
         return self.query_vector(query=arr, n=n)
-    
+
     def query_vector(self, query, n=10):
+        """Query using a vector."""
         labels, distances = self.index.knn_query(query, k=n)
         out = [self.db[int(label)] for label in labels[0]]
         return out, list(distances[0])
-    
+
     def walk(index, *args, n=10, depth=3, uniq_id=lambda d: d):
-        """Walk through the index, finding nearest neighbors of nearest neighbors. 
+        """Walk through the index, finding nearest neighbors of nearest neighbors.
 
         Arguments:
-        
+
         - args: the queries to start the walk off with
         - n : number of items to return per query
         - depth: how deep should the search go
         - uniq_id: function that can determine the uniqness of the item (must be hashable)
         """
         q = LifoQueue()
         seen = {}
-        
+
         for i in range(depth):
             new_args = []
-            
+
             for arg in args:
                 res, dists = index.query(arg, n=n)
                 for item in res:
                     q.put(item)
 
             if depth != 0:
                 while not q.empty():
@@ -97,29 +102,34 @@
             dim = encoded.shape[1]
             index = Index(space=space, dim=dim)
             index.init_index(max_elements=len(data))
         index.add_items(encoded)
     if path:
         path = Path(path)
         path.mkdir(parents=True, exist_ok=True)
-        if (path / "db.jsonl").exists():
-            (path / "db.jsonl").unlink()
-        srsly.write_jsonl(
-            path / "db.jsonl", ({"data": item} for i, item in enumerate(data))
-        )
-        index.save_index(str(path / "index.bin"))
+        if (path / DB_NAME).exists():
+            (path / DB_NAME).unlink()
+        srsly.write_gzip_json(path / DB_NAME, {i: item for i, item in enumerate(data)})
+        index.save_index(str(path / INDEX_NAME))
+        metadata = {
+            "created": str(dt.datetime.now())[:19],
+            "dim": dim,
+            "n_items": len(data),
+            "space": space,
+            "encoder": str(encoder),
+        }
         srsly.write_json(
-            path / "metadata.json",
-            {"created": str(dt.datetime.now())[:19], "dim": dim, "space": space},
+            path / METADATA_NAME,
+            metadata,
         )
     db = {i: k for i, k in enumerate(data)}
     return SimSityIndex(index=index, encoder=encoder, db=db)
 
 
 def load_index(path, encoder):
     """Load in a simsity index from a path. Must supply same encoder."""
     path = Path(path)
-    metadata = srsly.read_json(path / "metadata.json")
+    metadata = srsly.read_json(path / METADATA_NAME)
     index = Index(space=metadata["space"], dim=metadata["dim"])
-    index.load_index(str(path / "index.bin"))
-    db = {i: k for i, k in enumerate(srsly.read_jsonl(path / "db.jsonl"))}
+    index.load_index(str(path / INDEX_NAME))
+    db = {i: k for i, k in enumerate(srsly.read_gzip_json(path / DB_NAME))}
     return SimSityIndex(index=index, encoder=encoder, db=db)
```

### Comparing `simsity-0.5.2/simsity/datasets.py` & `simsity-0.5.3/simsity/datasets.py`

 * *Files identical despite different names*

### Comparing `simsity-0.5.2/simsity/error.py` & `simsity-0.5.3/simsity/error.py`

 * *Files identical despite different names*

### Comparing `simsity-0.5.2/simsity.egg-info/PKG-INFO` & `simsity-0.5.3/simsity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: simsity
-Version: 0.5.2
-Summary: Simple Similarity Service
+Version: 0.5.3
+Summary: Super Simple Similarity Service
 Home-page: https://github.com/koaning/simsity/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/koaning/simsity/
 Project-URL: Source Code, https://github.com/koaning/simsity/
 Project-URL: Issue Tracker, https://github.com/koaning/simsity/issues
 Description: 
@@ -53,16 +53,16 @@
         encoder = SentenceEncoder()
         
         # Populate the ANN vector index and use it. 
         index = create_index(recipes, encoder)
         texts, dists = index.query("pork")
         
         # You can also query using vectors
-        v_pork = encoder.transform("pork")[0]
-        texts, dists = index.query(v_pork)
+        v_pork = encoder.transform(["pork"])[0]
+        texts, dists = index.query_vector(v_pork)
         ```
         
         You can also provide a path and then you'll be able to store/load everything.
         
         ```python
         # Make an index with a path
         index = create_index(recipes, encoder, path="demo")
```

