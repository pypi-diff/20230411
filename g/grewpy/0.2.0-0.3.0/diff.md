# Comparing `tmp/grewpy-0.2.0.tar.gz` & `tmp/grewpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grewpy-0.2.0.tar", last modified: Tue Feb 28 20:43:32 2023, max compression
+gzip compressed data, was "grewpy-0.3.0.tar", last modified: Tue Apr 11 16:10:10 2023, max compression
```

## Comparing `grewpy-0.2.0.tar` & `grewpy-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-02-28 20:43:32.013436 grewpy-0.2.0/
--rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-02-28 20:43:32.013308 grewpy-0.2.0/PKG-INFO
--rw-r--r--   0 guillaum   (501) staff       (20)      113 2022-12-19 12:33:36.000000 grewpy-0.2.0/README.md
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-02-28 20:43:32.010183 grewpy-0.2.0/examples/
--rw-r--r--   0 guillaum   (501) staff       (20)     4786 2023-02-21 09:38:54.000000 grewpy-0.2.0/examples/classifier.py
--rw-r--r--   0 guillaum   (501) staff       (20)    17839 2023-02-21 09:38:54.000000 grewpy-0.2.0/examples/learner.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2836 2023-02-07 12:49:09.000000 grewpy-0.2.0/examples/test_GRS.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2687 2023-02-28 20:42:20.000000 grewpy-0.2.0/examples/test_corpus.py
--rw-r--r--   0 guillaum   (501) staff       (20)      937 2023-01-16 14:38:31.000000 grewpy-0.2.0/examples/test_graph.py
--rw-r--r--   0 guillaum   (501) staff       (20)      736 2023-02-09 15:38:41.000000 grewpy-0.2.0/examples/test_grew_web.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1405 2023-01-09 12:56:06.000000 grewpy-0.2.0/examples/test_search.py
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-02-28 20:43:32.012583 grewpy-0.2.0/grewpy/
--rw-r--r--   0 guillaum   (501) staff       (20)      340 2023-02-13 12:14:28.000000 grewpy-0.2.0/grewpy/__init__.py
--rw-r--r--   0 guillaum   (501) staff       (20)     8660 2023-02-13 12:14:28.000000 grewpy-0.2.0/grewpy/corpus.py
--rw-r--r--   0 guillaum   (501) staff       (20)     8047 2023-02-13 12:14:28.000000 grewpy-0.2.0/grewpy/graph.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1109 2022-12-21 08:33:45.000000 grewpy-0.2.0/grewpy/grew.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2549 2023-02-13 12:12:39.000000 grewpy-0.2.0/grewpy/grew_web.py
--rw-r--r--   0 guillaum   (501) staff       (20)    12589 2023-02-09 15:38:41.000000 grewpy-0.2.0/grewpy/grs.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1752 2023-02-13 12:14:28.000000 grewpy-0.2.0/grewpy/matchings.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2980 2023-02-23 10:39:26.000000 grewpy-0.2.0/grewpy/network.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2620 2023-02-21 09:38:54.000000 grewpy-0.2.0/grewpy/observation.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1259 2023-02-13 12:14:28.000000 grewpy-0.2.0/grewpy/sketch.py
--rw-r--r--   0 guillaum   (501) staff       (20)      190 2022-12-19 17:10:04.000000 grewpy-0.2.0/grewpy/utils.py
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-02-28 20:43:32.013144 grewpy-0.2.0/grewpy.egg-info/
--rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-02-28 20:43:31.000000 grewpy-0.2.0/grewpy.egg-info/PKG-INFO
--rw-r--r--   0 guillaum   (501) staff       (20)      492 2023-02-28 20:43:31.000000 grewpy-0.2.0/grewpy.egg-info/SOURCES.txt
--rw-r--r--   0 guillaum   (501) staff       (20)        1 2023-02-28 20:43:31.000000 grewpy-0.2.0/grewpy.egg-info/dependency_links.txt
--rw-r--r--   0 guillaum   (501) staff       (20)       16 2023-02-28 20:43:31.000000 grewpy-0.2.0/grewpy.egg-info/top_level.txt
--rw-r--r--   0 guillaum   (501) staff       (20)       38 2023-02-28 20:43:32.013471 grewpy-0.2.0/setup.cfg
--rw-r--r--   0 guillaum   (501) staff       (20)      463 2023-02-28 20:43:23.000000 grewpy-0.2.0/setup.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.744245 grewpy-0.3.0/
+-rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-04-11 16:10:10.744132 grewpy-0.3.0/PKG-INFO
+-rw-r--r--   0 guillaum   (501) staff       (20)      113 2022-12-19 12:33:36.000000 grewpy-0.3.0/README.md
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.741142 grewpy-0.3.0/examples/
+-rw-r--r--   0 guillaum   (501) staff       (20)     2057 2023-04-11 16:02:43.000000 grewpy-0.3.0/examples/allemand.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     4786 2023-02-21 09:38:54.000000 grewpy-0.3.0/examples/classifier.py
+-rw-r--r--   0 guillaum   (501) staff       (20)    17839 2023-02-21 09:38:54.000000 grewpy-0.3.0/examples/learner.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2836 2023-02-07 12:49:09.000000 grewpy-0.3.0/examples/test_GRS.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2687 2023-04-11 16:00:39.000000 grewpy-0.3.0/examples/test_corpus.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      937 2023-01-16 14:38:31.000000 grewpy-0.3.0/examples/test_graph.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      736 2023-02-09 15:38:41.000000 grewpy-0.3.0/examples/test_grew_web.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1405 2023-01-09 12:56:06.000000 grewpy-0.3.0/examples/test_search.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.743339 grewpy-0.3.0/grewpy/
+-rw-r--r--   0 guillaum   (501) staff       (20)      340 2023-02-13 12:14:28.000000 grewpy-0.3.0/grewpy/__init__.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     8975 2023-04-11 16:02:47.000000 grewpy-0.3.0/grewpy/corpus.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     8497 2023-04-11 16:02:43.000000 grewpy-0.3.0/grewpy/graph.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1109 2022-12-21 08:33:45.000000 grewpy-0.3.0/grewpy/grew.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2544 2023-04-11 16:02:43.000000 grewpy-0.3.0/grewpy/grew_web.py
+-rw-r--r--   0 guillaum   (501) staff       (20)    12874 2023-04-11 16:02:47.000000 grewpy-0.3.0/grewpy/grs.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1752 2023-02-13 12:14:28.000000 grewpy-0.3.0/grewpy/matchings.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2980 2023-02-23 10:39:26.000000 grewpy-0.3.0/grewpy/network.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2620 2023-02-21 09:38:54.000000 grewpy-0.3.0/grewpy/observation.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1259 2023-03-31 09:13:11.000000 grewpy-0.3.0/grewpy/sketch.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      190 2022-12-19 17:10:04.000000 grewpy-0.3.0/grewpy/utils.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-04-11 16:10:10.743975 grewpy-0.3.0/grewpy.egg-info/
+-rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/PKG-INFO
+-rw-r--r--   0 guillaum   (501) staff       (20)      513 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)        1 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)       16 2023-04-11 16:10:10.000000 grewpy-0.3.0/grewpy.egg-info/top_level.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)       38 2023-04-11 16:10:10.744284 grewpy-0.3.0/setup.cfg
+-rw-r--r--   0 guillaum   (501) staff       (20)      463 2023-04-11 16:10:02.000000 grewpy-0.3.0/setup.py
```

### Comparing `grewpy-0.2.0/examples/classifier.py` & `grewpy-0.3.0/examples/classifier.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/examples/learner.py` & `grewpy-0.3.0/examples/learner.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/examples/test_GRS.py` & `grewpy-0.3.0/examples/test_GRS.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/examples/test_corpus.py` & `grewpy-0.3.0/examples/test_corpus.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/examples/test_graph.py` & `grewpy-0.3.0/examples/test_graph.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/examples/test_grew_web.py` & `grewpy-0.3.0/examples/test_grew_web.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/examples/test_search.py` & `grewpy-0.3.0/examples/test_search.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/grewpy/corpus.py` & `grewpy-0.3.0/grewpy/corpus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Grew module : anything you want to talk about graphs
 Graphs are represented either by a dict (called dict-graph),
 or by an str (str-graph).
 """
 import os.path
+import glob
+
 import sys
 import tempfile
 import json
 import typing
 import numpy as np
 
 from .network import send_and_receive
@@ -57,15 +59,14 @@
     the draft is composed of 
       - self, a dict mapping sentence_id to graphs
       - self._sent_ids, a list that specifies the sentence order
     """
     def __init__(self,data=None):
         """Load a corpus from a file of a string
         :param data: a file, a list of files or a CoNLL string representation of a corpus
-        :param local: state whether we load a local copy of each graph of the corpus
         :return: an integer index for latter reference to the corpus
         :raise an error if the files was not correctly loaded
         """
         if isinstance(data, CorpusDraft):
             T = {sid: Graph(data[sid]) for sid in data}
             super().__init__(T)
         elif isinstance(data, dict):
@@ -98,15 +99,14 @@
         return CorpusDraft({sid : fun(self[sid]) for sid in self})
 
 
 class Corpus(AbstractCorpus):
     def __init__(self, data):
         """An abstract corpus
         :param data: a file, a list of files or a CoNLL string representation of a corpus
-        :param local: state whether we load a local copy of each graph of the corpus
         :return: an integer index for latter reference to the corpus
         :raise an error if the files was not correctly loaded
         """
         if isinstance(data, list):
             if data and isinstance(data[0], Graph):
                 graphs = {f'{i}' : data[i].json_data() for i in range(len(data))}
                 req = {"command": "corpus_from_dict", "graphs": graphs}
@@ -114,14 +114,19 @@
                 #supposed to be a list of files
                 req = {"command": "corpus_load", "files": data}
             reply = network.send_and_receive(req)
         elif isinstance(data, dict):
             req = {"command": "corpus_from_dict", "graphs": {
                 sent_id: graph.json_data() for (sent_id, graph) in data.items()}}
             reply = network.send_and_receive(req)
+        elif os.path.isdir(data):
+            # load of connlu files of the directory
+            file_list = glob.glob(f"{data}/*.conllu")
+            req = {"command": "corpus_load", "files": file_list}
+            reply = network.send_and_receive(req)
         elif os.path.isfile(data):
             req = {"command": "corpus_load", "files": [data]}
             reply = network.send_and_receive(req)
         else:
             with tempfile.NamedTemporaryFile(mode="w", delete=True, suffix=".conll") as f:
                 f.write(data)
                 f.flush()  # to be read by others
@@ -142,14 +147,21 @@
 
     def get_id(self):
         """
         return the id of the corpus
         """
         return self._id
 
+    def clean(self):
+        """
+        clean the corpus (remove from the backend memory)
+        """
+        req = {"command": "corpus_clean", "corpus_index": self._id}
+        return network.send_and_receive(req)
+
     def get(self, sent_id):
         """
         return a graph corresponding to the sentence id sent_id
         """
         req = {"command": "corpus_get",
                    "corpus_index": self._id, "sent_id": sent_id}
         return (Graph.from_json(network.send_and_receive(req)))
```

### Comparing `grewpy-0.2.0/grewpy/graph.py` & `grewpy-0.3.0/grewpy/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,35 @@
 from grewpy import utils
 from . import network
 
 ''' interfaces'''
 class Fs_edge(dict):
     def __init__(self,data):
         if isinstance(data,str):
-            super().__init__({"1": data})
+            #try to split a dict
+            if "=" in data and "," in data:
+                #suppose it is a dictionary
+                super().__init__(Fs_edge.decompose_edge(data))
+            else:
+                super().__init__({"1": data})
         elif isinstance(data, dict):
             super().__init__(data)
         else:
             raise ValueError(f"data is not a feature structure {data}")
 
     def __hash__(self):
         return (hash (str(self)))
+    
+    @staticmethod
+    def decompose_edge(s):
+        clauses = dict()
+        for it in s.split(","):
+            a, b = it.split("=")
+            clauses[a] = b
+        return clauses
 
 class Graph():
     """
     a dict mapping node keys to feature structure
 
     with extra data:
         - an extra dict `sucs` mapping node keys to successors (pair of edge feature,node key)
@@ -186,14 +199,16 @@
                     return v
 
     def edges(self, n, m):
         """
         given node n and m, 
         return the set of edges between n and m
         """
+        if n not in self._sucs:
+            return []
         return [v for (k,v) in self._sucs[n] if k == m]
 
     def edges_up_to(self, n, m, criterion):
         """
         search for edges between n and m verifying some criterion
         """
         return [v for (k, v) in self._sucs[n] if k == m and criterion(v)]
```

### Comparing `grewpy-0.2.0/grewpy/grew.py` & `grewpy-0.3.0/grewpy/grew.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/grewpy/grew_web.py` & `grewpy-0.3.0/grewpy/grew_web.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 local = False
 if local:
     grew_web_back = "http://localhost:8080"
     grew_web_front = "http://localhost:8888/grew_web"
 else:
-    grew_web_back = "http://back.grew.fr"
-    grew_web_front = "http://transform.grew.fr"
+    grew_web_back = "https://gwb.grew.fr"
+    grew_web_front = "https://web.grew.fr"
 
 
 def _post_request(service, resp):
     if resp.status_code >= 300:
         raise GrewError({
             "Error": "HTTP",
             "service": service,
```

### Comparing `grewpy-0.2.0/grewpy/grs.py` & `grewpy-0.3.0/grewpy/grs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .grew import JSON
 from grewpy.graph import Graph
 from .corpus import Corpus, CorpusDraft, GrewError
 
 class RequestItem():
     def __init__(self,sort : str,*L):
         """
-        sort in {"without", "pattern", "global"}
+        sort in {"global", "pattern", "without", "with"}
         L is a list of
          - ";" separated clauses or
          - a list of items
          - they will be concatenated
         """
         self.sort = sort
         self.items = tuple()
@@ -68,14 +68,22 @@
                 except:
                     raise ValueError(f"{e} cannot be used to build a Request")
         self.items = elts
 
     def without(self, *L):
         self.items += tuple(RequestItem("without", e) for e in L)
         return self
+    def with_(self, *L):
+        self.items += tuple(RequestItem("with", e) for e in L)
+        return self
+
+
+    def with_(self, *L):
+        self.items += tuple(RequestItem("with", e) for e in L)
+        return self
 
     @classmethod
     def from_json(cls,json_data):
         elts = [RequestItem.from_json(c) for c in json_data]
         return cls(*elts)
 
     def json_data(self):
@@ -114,15 +122,15 @@
         """
         self.item = s
 
     def json_data(self):
         return self.item
     
     def __str__(self):
-        return self.item
+        return str(self.item)
 
     def safe(self):
         """
         return a clause list for a safe request
         """
         raise NotImplementedError ("not yet implemented")
 
@@ -133,14 +141,17 @@
         else:
             s = str(e)
         super().__init__(f"add_edge {X}-[{s}]->{Y}")
         self.X, self.e, self.Y = X, e, Y
 
     def safe(self):           
         return RequestItem("without",self.item.replace("add_edge",""))
+    
+    def __repr__(self):
+        return str(self)
 
 class Delete_edge(Command):
     def __init__(self, X, e, Y):
         super().__init__(f"del_edge {X}-[{e}]->{Y}")
         self.X, self.e, self.Y = X, e, Y
 
     def safe(self):
```

### Comparing `grewpy-0.2.0/grewpy/matchings.py` & `grewpy-0.3.0/grewpy/matchings.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/grewpy/network.py` & `grewpy-0.3.0/grewpy/network.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/grewpy/observation.py` & `grewpy-0.3.0/grewpy/observation.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.2.0/grewpy/sketch.py` & `grewpy-0.3.0/grewpy/sketch.py`

 * *Files identical despite different names*

