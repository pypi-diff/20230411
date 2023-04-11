# Comparing `tmp/skl-graph-2023.8.tar.gz` & `tmp/skl-graph-2023.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skl-graph-2023.8.tar", last modified: Wed Mar  8 11:19:50 2023, max compression
+gzip compressed data, was "skl-graph-2023.9.tar", last modified: Wed Mar  8 12:56:57 2023, max compression
```

## Comparing `skl-graph-2023.8.tar` & `skl-graph-2023.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.991198 skl-graph-2023.8/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 07:46:13.000000 skl-graph-2023.8/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4958 2023-03-08 11:19:50.991198 skl-graph-2023.8/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2022-10-14 06:43:57.000000 skl-graph-2023.8/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-09-12 08:38:30.000000 skl-graph-2023.8/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     4194 2022-10-14 07:37:51.000000 skl-graph-2023.8/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.984532 skl-graph-2023.8/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.987865 skl-graph-2023.8/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1846 2022-10-14 07:10:22.000000 skl-graph-2023.8/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-10-14 06:44:39.000000 skl-graph-2023.8/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-03-08 11:19:50.991198 skl-graph-2023.8/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5599 2023-02-28 14:11:04.000000 skl-graph-2023.8/setup.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.987865 skl-graph-2023.8/skl_graph/
--rw-r--r--   0 eric      (1000) users      (984)     1705 2023-02-28 14:57:53.000000 skl-graph-2023.8/skl_graph/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)    19483 2023-03-08 08:43:12.000000 skl-graph-2023.8/skl_graph/graph.py
--rw-r--r--   0 eric      (1000) users      (984)    12783 2023-02-28 13:44:26.000000 skl-graph-2023.8/skl_graph/map.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.987865 skl-graph-2023.8/skl_graph/standard/
--rw-r--r--   0 eric      (1000) users      (984)     2353 2023-02-28 12:55:05.000000 skl-graph-2023.8/skl_graph/standard/identifier.py
--rw-r--r--   0 eric      (1000) users      (984)     1751 2023-02-28 13:21:59.000000 skl-graph-2023.8/skl_graph/standard/str_extension.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.987865 skl-graph-2023.8/skl_graph/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.987865 skl-graph-2023.8/skl_graph/task/check/
--rw-r--r--   0 eric      (1000) users      (984)     3777 2023-02-28 12:23:30.000000 skl-graph-2023.8/skl_graph/task/check/edge.py
--rw-r--r--   0 eric      (1000) users      (984)     3851 2023-02-28 13:17:57.000000 skl-graph-2023.8/skl_graph/task/check/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     1788 2023-02-28 12:24:22.000000 skl-graph-2023.8/skl_graph/task/check/node.py
--rw-r--r--   0 eric      (1000) users      (984)     1703 2023-02-28 13:27:19.000000 skl-graph-2023.8/skl_graph/task/feature.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.991198 skl-graph-2023.8/skl_graph/task/plot/
--rw-r--r--   0 eric      (1000) users      (984)     3824 2023-03-08 10:12:16.000000 skl-graph-2023.8/skl_graph/task/plot/base.py
--rw-r--r--   0 eric      (1000) users      (984)     4672 2023-03-08 11:17:45.000000 skl-graph-2023.8/skl_graph/task/plot/edge.py
--rw-r--r--   0 eric      (1000) users      (984)     8863 2023-03-08 11:14:30.000000 skl-graph-2023.8/skl_graph/task/plot/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     8263 2023-03-08 10:09:06.000000 skl-graph-2023.8/skl_graph/task/plot/node.py
--rw-r--r--   0 eric      (1000) users      (984)    14705 2023-02-28 13:27:19.000000 skl-graph-2023.8/skl_graph/task/process.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.991198 skl-graph-2023.8/skl_graph/type/
--rw-r--r--   0 eric      (1000) users      (984)    24546 2023-03-06 16:44:25.000000 skl-graph-2023.8/skl_graph/type/edge.py
--rw-r--r--   0 eric      (1000) users      (984)     5141 2023-02-28 13:20:51.000000 skl-graph-2023.8/skl_graph/type/node.py
--rw-r--r--   0 eric      (1000) users      (984)     7974 2023-02-28 12:52:55.000000 skl-graph-2023.8/skl_graph/type/plot.py
--rw-r--r--   0 eric      (1000) users      (984)     4983 2023-03-07 15:17:14.000000 skl-graph-2023.8/skl_graph/type/topology_map.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-03-08 11:18:51.000000 skl-graph-2023.8/skl_graph/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 11:19:50.987865 skl-graph-2023.8/skl_graph.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4958 2023-03-08 11:19:50.000000 skl-graph-2023.8/skl_graph.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      801 2023-03-08 11:19:50.000000 skl-graph-2023.8/skl_graph.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-03-08 11:19:50.000000 skl-graph-2023.8/skl_graph.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       64 2023-03-08 11:19:50.000000 skl-graph-2023.8/skl_graph.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2023-03-08 11:19:50.000000 skl-graph-2023.8/skl_graph.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.817711 skl-graph-2023.9/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 07:46:13.000000 skl-graph-2023.9/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4958 2023-03-08 12:56:57.817711 skl-graph-2023.9/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2022-10-14 06:43:57.000000 skl-graph-2023.9/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-09-12 08:38:30.000000 skl-graph-2023.9/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     4194 2022-10-14 07:37:51.000000 skl-graph-2023.9/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.814377 skl-graph-2023.9/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.814377 skl-graph-2023.9/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1846 2022-10-14 07:10:22.000000 skl-graph-2023.9/documentation/wiki/description.asciidoc
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-10-14 06:44:39.000000 skl-graph-2023.9/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-03-08 12:56:57.817711 skl-graph-2023.9/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5599 2023-02-28 14:11:04.000000 skl-graph-2023.9/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.814377 skl-graph-2023.9/skl_graph/
+-rw-r--r--   0 eric      (1000) users      (984)     1705 2023-02-28 14:57:53.000000 skl-graph-2023.9/skl_graph/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)    19483 2023-03-08 08:43:12.000000 skl-graph-2023.9/skl_graph/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)    12783 2023-02-28 13:44:26.000000 skl-graph-2023.9/skl_graph/map.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.814377 skl-graph-2023.9/skl_graph/standard/
+-rw-r--r--   0 eric      (1000) users      (984)     2353 2023-02-28 12:55:05.000000 skl-graph-2023.9/skl_graph/standard/identifier.py
+-rw-r--r--   0 eric      (1000) users      (984)     1751 2023-02-28 13:21:59.000000 skl-graph-2023.9/skl_graph/standard/str_extension.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.814377 skl-graph-2023.9/skl_graph/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.814377 skl-graph-2023.9/skl_graph/task/check/
+-rw-r--r--   0 eric      (1000) users      (984)     3777 2023-02-28 12:23:30.000000 skl-graph-2023.9/skl_graph/task/check/edge.py
+-rw-r--r--   0 eric      (1000) users      (984)     3851 2023-02-28 13:17:57.000000 skl-graph-2023.9/skl_graph/task/check/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     1788 2023-02-28 12:24:22.000000 skl-graph-2023.9/skl_graph/task/check/node.py
+-rw-r--r--   0 eric      (1000) users      (984)     1703 2023-02-28 13:27:19.000000 skl-graph-2023.9/skl_graph/task/feature.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.817711 skl-graph-2023.9/skl_graph/task/plot/
+-rw-r--r--   0 eric      (1000) users      (984)     3824 2023-03-08 10:12:16.000000 skl-graph-2023.9/skl_graph/task/plot/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     4672 2023-03-08 11:17:45.000000 skl-graph-2023.9/skl_graph/task/plot/edge.py
+-rw-r--r--   0 eric      (1000) users      (984)     8934 2023-03-08 12:10:28.000000 skl-graph-2023.9/skl_graph/task/plot/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     8263 2023-03-08 10:09:06.000000 skl-graph-2023.9/skl_graph/task/plot/node.py
+-rw-r--r--   0 eric      (1000) users      (984)    14705 2023-02-28 13:27:19.000000 skl-graph-2023.9/skl_graph/task/process.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.817711 skl-graph-2023.9/skl_graph/type/
+-rw-r--r--   0 eric      (1000) users      (984)    24546 2023-03-06 16:44:25.000000 skl-graph-2023.9/skl_graph/type/edge.py
+-rw-r--r--   0 eric      (1000) users      (984)     5141 2023-02-28 13:20:51.000000 skl-graph-2023.9/skl_graph/type/node.py
+-rw-r--r--   0 eric      (1000) users      (984)     7974 2023-02-28 12:52:55.000000 skl-graph-2023.9/skl_graph/type/plot.py
+-rw-r--r--   0 eric      (1000) users      (984)     4983 2023-03-07 15:17:14.000000 skl-graph-2023.9/skl_graph/type/topology_map.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-03-08 12:41:24.000000 skl-graph-2023.9/skl_graph/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-08 12:56:57.814377 skl-graph-2023.9/skl_graph.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4958 2023-03-08 12:56:57.000000 skl-graph-2023.9/skl_graph.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      801 2023-03-08 12:56:57.000000 skl-graph-2023.9/skl_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-03-08 12:56:57.000000 skl-graph-2023.9/skl_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       64 2023-03-08 12:56:57.000000 skl-graph-2023.9/skl_graph.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2023-03-08 12:56:57.000000 skl-graph-2023.9/skl_graph.egg-info/top_level.txt
```

### Comparing `skl-graph-2023.8/PKG-INFO` & `skl-graph-2023.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skl-graph
-Version: 2023.8
+Version: 2023.9
 Summary: SKeLeton Graph
 Home-page: https://gitlab.inria.fr/edebreuv/SKLGraph/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://edebreuv.gitlabpages.inria.fr/SKLGraph/
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/SKLGraph/
```

### Comparing `skl-graph-2023.8/README-COPYRIGHT-utf8.txt` & `skl-graph-2023.9/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/README-LICENCE-utf8.txt` & `skl-graph-2023.9/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/README.rst` & `skl-graph-2023.9/README.rst`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/documentation/wiki/description.asciidoc` & `skl-graph-2023.9/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/setup.py` & `skl-graph-2023.9/setup.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/__init__.py` & `skl-graph-2023.9/skl_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/graph.py` & `skl-graph-2023.9/skl_graph/graph.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/map.py` & `skl-graph-2023.9/skl_graph/map.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/standard/identifier.py` & `skl-graph-2023.9/skl_graph/standard/identifier.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/standard/str_extension.py` & `skl-graph-2023.9/skl_graph/standard/str_extension.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/check/edge.py` & `skl-graph-2023.9/skl_graph/task/check/edge.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/check/graph.py` & `skl-graph-2023.9/skl_graph/task/check/graph.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/check/node.py` & `skl-graph-2023.9/skl_graph/task/check/node.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/feature.py` & `skl-graph-2023.9/skl_graph/task/feature.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/plot/base.py` & `skl-graph-2023.9/skl_graph/task/plot/base.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/plot/edge.py` & `skl-graph-2023.9/skl_graph/task/plot/edge.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/plot/graph.py` & `skl-graph-2023.9/skl_graph/task/plot/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,18 +143,22 @@
     Only 2-D graphs
     """
     if graph.number_of_nodes() < 1:
         return None
 
     figure, axes = FigureAndAxesFromBoth(figure, axes, 2)
 
+    if NodePositions is None:
+        node_positions = None
+    else:
+        node_positions = NodePositions(axes)
     _PlotWithNetworkX(
         graph,
         axes,
-        node_positions=NodePositions(axes),
+        node_positions=node_positions,
         node_colors=node_colors,
         with_node_labels=with_node_labels,
         node_font_size=node_font_size,
         edge_width=edge_width,
         edge_labels=edge_labels,
         edge_font_size=edge_font_size,
     )
@@ -281,19 +285,17 @@
     ntkx.draw_networkx(
         graph,
         ax=axes,
         with_labels=with_node_labels,
         **options,
     )
 
-    if edge_labels is not None:
-        options = {}
-        if node_positions is not None:
-            options["pos"] = node_positions
-        options["edge_labels"] = edge_labels
+    if (edge_labels is not None) and (node_positions is not None):
+        options = {"edge_labels": edge_labels}
         if edge_font_size is not None:
             options["font_size"] = edge_font_size
         ntkx.draw_networkx_edge_labels(
             graph,
+            node_positions,
             ax=axes,
             **options,
         )
```

### Comparing `skl-graph-2023.8/skl_graph/task/plot/node.py` & `skl-graph-2023.9/skl_graph/task/plot/node.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/task/process.py` & `skl-graph-2023.9/skl_graph/task/process.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/type/edge.py` & `skl-graph-2023.9/skl_graph/type/edge.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/type/node.py` & `skl-graph-2023.9/skl_graph/type/node.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/type/plot.py` & `skl-graph-2023.9/skl_graph/type/plot.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/type/topology_map.py` & `skl-graph-2023.9/skl_graph/type/topology_map.py`

 * *Files identical despite different names*

### Comparing `skl-graph-2023.8/skl_graph/version.py` & `skl-graph-2023.9/skl_graph/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.8"
+__version__ = "2023.9"
```

### Comparing `skl-graph-2023.8/skl_graph.egg-info/PKG-INFO` & `skl-graph-2023.9/skl_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skl-graph
-Version: 2023.8
+Version: 2023.9
 Summary: SKeLeton Graph
 Home-page: https://gitlab.inria.fr/edebreuv/SKLGraph/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://edebreuv.gitlabpages.inria.fr/SKLGraph/
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/SKLGraph/
```

### Comparing `skl-graph-2023.8/skl_graph.egg-info/SOURCES.txt` & `skl-graph-2023.9/skl_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

