# Comparing `tmp/geomapi-0.1.9.tar.gz` & `tmp/geomapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapi-0.1.9.tar", last modified: Tue Feb 28 08:46:32 2023, max compression
+gzip compressed data, was "geomapi-0.2.0.tar", last modified: Tue Apr 11 15:06:27 2023, max compression
```

## Comparing `geomapi-0.1.9.tar` & `geomapi-0.2.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.763829 geomapi-0.1.9/
--rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-02-28 08:44:45.000000 geomapi-0.1.9/LICENSE
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-02-28 08:46:32.763829 geomapi-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-02-28 08:44:45.000000 geomapi-0.1.9/README.md
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.754829 geomapi-0.1.9/developmenttests/
--rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-02-28 08:44:45.000000 geomapi-0.1.9/developmenttests/QualityCompare.py
--rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-02-28 08:44:45.000000 geomapi-0.1.9/developmenttests/QualityCompare_gui.py
--rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-02-28 08:44:55.000000 geomapi-0.1.9/developmenttests/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-02-28 08:44:46.000000 geomapi-0.1.9/developmenttests/context.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-02-28 08:44:46.000000 geomapi-0.1.9/developmenttests/ifc_to_nodes.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-02-28 08:44:46.000000 geomapi-0.1.9/developmenttests/import_e57.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.755829 geomapi-0.1.9/geomapi/
--rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.758829 geomapi-0.1.9/geomapi/nodes/
--rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    34998 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/imagenode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/linesetnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     7742 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/node.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/orthonode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/nodes/sessionnode.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.758829 geomapi-0.1.9/geomapi/tools/
--rw-rw-rw-   0 root         (0) daemon       (1)    40647 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/tools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.758829 geomapi-0.1.9/geomapi/tools/alignmenttools/
--rw-rw-rw-   0 root         (0) daemon       (1)     2951 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/tools/alignmenttools/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/tools/alignmenttools/match.py
--rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/tools/alignmenttools/params.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.759829 geomapi-0.1.9/geomapi/tools/completiontools/
--rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/tools/completiontools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.759829 geomapi-0.1.9/geomapi/tools/progresstools/
--rw-rw-rw-   0 root         (0) daemon       (1)    35767 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/tools/progresstools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.759829 geomapi-0.1.9/geomapi/tools/validationtools/
--rw-rw-rw-   0 root         (0) daemon       (1)    23868 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/tools/validationtools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.760829 geomapi-0.1.9/geomapi/utils/
--rw-rw-rw-   0 root         (0) daemon       (1)    38739 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/utils/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)   104395 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/utils/geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     6335 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/utils/geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    26060 2023-02-28 08:44:46.000000 geomapi-0.1.9/geomapi/utils/imageutils.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.756829 geomapi-0.1.9/geomapi.egg-info/
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-02-28 08:46:32.000000 geomapi-0.1.9/geomapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) daemon       (1)     1450 2023-02-28 08:46:32.000000 geomapi-0.1.9/geomapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) daemon       (1)        1 2023-02-28 08:46:32.000000 geomapi-0.1.9/geomapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) daemon       (1)      194 2023-02-28 08:46:32.000000 geomapi-0.1.9/geomapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) daemon       (1)       30 2023-02-28 08:46:32.000000 geomapi-0.1.9/geomapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-02-28 08:44:46.000000 geomapi-0.1.9/pyproject.toml
--rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-02-28 08:46:32.764829 geomapi-0.1.9/setup.cfg
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-02-28 08:46:32.763829 geomapi-0.1.9/test/
--rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_alignmenttools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_completiontools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    24257 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_imageutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_imgnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_node.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4018 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_progresstools.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_sessionnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15472 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_tools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27068 2023-02-28 08:44:46.000000 geomapi-0.1.9/test/test_utils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.706006 geomapi-0.2.0/
+-rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-04-11 15:04:48.000000 geomapi-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-11 15:06:27.706006 geomapi-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-04-11 15:04:48.000000 geomapi-0.2.0/README.md
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.698006 geomapi-0.2.0/developmenttests/
+-rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-04-11 15:04:48.000000 geomapi-0.2.0/developmenttests/QualityCompare.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-04-11 15:04:48.000000 geomapi-0.2.0/developmenttests/QualityCompare_gui.py
+-rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-04-11 15:04:59.000000 geomapi-0.2.0/developmenttests/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-04-11 15:04:49.000000 geomapi-0.2.0/developmenttests/context.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-04-11 15:04:49.000000 geomapi-0.2.0/developmenttests/ifc_to_nodes.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-04-11 15:04:49.000000 geomapi-0.2.0/developmenttests/import_e57.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.698006 geomapi-0.2.0/geomapi/
+-rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/nodes/
+-rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    34991 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/imagenode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/linesetnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     7742 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/orthonode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/nodes/sessionnode.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    45354 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/alignmenttools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     2975 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/alignmenttools/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/alignmenttools/match.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/alignmenttools/params.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/completiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/completiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/inspectiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)      306 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/inspectiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/machinelearningtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    13233 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/machinelearningtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/progresstools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    35729 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/progresstools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/tools/validationtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    23868 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/tools/validationtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.702005 geomapi-0.2.0/geomapi/utils/
+-rw-rw-rw-   0 root         (0) daemon       (1)    38758 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)   108378 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     6335 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    26061 2023-04-11 15:04:49.000000 geomapi-0.2.0/geomapi/utils/imageutils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.698006 geomapi-0.2.0/geomapi.egg-info/
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) daemon       (1)     1539 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) daemon       (1)        1 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) daemon       (1)      194 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) daemon       (1)       30 2023-04-11 15:06:27.000000 geomapi-0.2.0/geomapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-04-11 15:04:49.000000 geomapi-0.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-04-11 15:06:27.706006 geomapi-0.2.0/setup.cfg
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-11 15:06:27.706006 geomapi-0.2.0/test/
+-rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_alignmenttools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_completiontools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    24257 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_imageutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_imgnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4270 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_progresstools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_sessionnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15091 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_tools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27056 2023-04-11 15:04:49.000000 geomapi-0.2.0/test/test_utils.py
```

### Comparing `geomapi-0.1.9/LICENSE` & `geomapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/PKG-INFO` & `geomapi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.1.9
+Version: 0.2.0
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geomapi-0.1.9/README.md` & `geomapi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/developmenttests/QualityCompare.py` & `geomapi-0.2.0/developmenttests/QualityCompare.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/developmenttests/QualityCompare_gui.py` & `geomapi-0.2.0/developmenttests/QualityCompare_gui.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/developmenttests/ifc_to_nodes.py` & `geomapi-0.2.0/developmenttests/ifc_to_nodes.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/developmenttests/import_e57.py` & `geomapi-0.2.0/developmenttests/import_e57.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/bimnode.py` & `geomapi-0.2.0/geomapi/nodes/bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/geometrynode.py` & `geomapi-0.2.0/geomapi/nodes/geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/imagenode.py` & `geomapi-0.2.0/geomapi/nodes/imagenode.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
 
         Returns:
             o3d.camera.PinholeCameraIntrinsic(width,height,fx,fy,cx,cy)
         """
         #validate inputs
         width=int(self.imageWidth/downsampling) if getattr(self,'imageWidth',None) is not None else 640
         height=int(self.imageHeight/downsampling) if getattr(self,'imageHeight',None) is not None else 480
-        f=self.focalLength35mm if getattr(self,'focalLength35mm',None) is not None else 25
+        f=self.focalLength35mm if getattr(self,'focalLength35mm',None) is not None else 2500
 
         #! deprecated
         # pixX=width/36 #these are standard 35mm film properties
         # pixY=height/24 #these are standard 35mm film properties
         # fx=pixX*f
         # fy=pixY*f        
 
@@ -766,15 +766,14 @@
         world_coordinates=m @ camera_coordinates
         world_coordinates=gmu.normalize_vectors(world_coordinates[0:3,:].T)
   
         if depths is not None:
             world_coordinates=world_coordinates * depths[:, np.newaxis]
   
         
-        
         #create rays [camera.center, direction(world_coordinates)]
         rays=np.hstack((np.full((n,3), t),world_coordinates))         
         return rays 
     
     # def create_rays(self,imagePoints:np.array)->o3d.core.Tensor:
     #     """Generate a grid a rays from the camera location to a given set of imagePoints.\n
```

### Comparing `geomapi-0.1.9/geomapi/nodes/linesetnode.py` & `geomapi-0.2.0/geomapi/nodes/linesetnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/meshnode.py` & `geomapi-0.2.0/geomapi/nodes/meshnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/node.py` & `geomapi-0.2.0/geomapi/nodes/node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/orthonode.py` & `geomapi-0.2.0/geomapi/nodes/orthonode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/pointcloudnode.py` & `geomapi-0.2.0/geomapi/nodes/pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/nodes/sessionnode.py` & `geomapi-0.2.0/geomapi/nodes/sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/tools/__init__.py` & `geomapi-0.2.0/geomapi/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,32 +69,131 @@
 
         for idx,child in enumerate(root.iter('{http://www.astm.org/COMMIT/E57/2010-e57-v1.0}vectorChild')):
             nodelist.append(PointCloudNode(e57XmlPath=e57XmlPath,e57Index=idx,path=e57Path,**kwargs))
         return nodelist
     else:
         raise ValueError('No valid e57XmlPath.')
 
-def img_xml_to_nodes(xmlPath :str, **kwargs) -> List[ImageNode]:
+def img_xml_to_nodes(xmlPath :str,skip:int=None, filterByFolder:bool=False,**kwargs) -> List[ImageNode]:
     """Parse XML file that is created with https://www.agisoft.com/.
 
     Args:
-        path (string):  e57 xml file path e.g. "D:\\Data\\2018-06 Werfopvolging Academiestraat Gent\\week 22\\PCD\\week 22 lidar_CC.xml"
+        1.xmlPath (string): xml file path e.g. "D:/Data/cameras.xml"
+        2.skip (int, Optional): select every nth image from the xml. Defaults to None.
+        3.filterByFolder (bool, Optional): Filter imgNodes based on the images in the folder or not. Defaults to False.
             
     Returns:
         A list of pointcloudnodes with the xml metadata 
     """
-    if os.path.exists(xmlPath) and xmlPath.endswith('.xml'):    
-        mytree = ET.parse(xmlPath)
-        root = mytree.getroot()  
-        nodelist=[]   
-        for child in root.iter('camera'):
-            nodelist.append(ImageNode(xmlPath=xmlPath,name=child.get('label'),**kwargs))
-        return nodelist
-    else:
-        raise ValueError('No valid xmlPath.')
+    assert skip == None or skip >0, f'skip == None or skip '
+    assert os.path.exists(xmlPath), f'File does not exist.'
+    assert xmlPath.endswith('.xml'), f'File does not end with xml.' 
+    
+    #open xml
+    mytree = ET.parse(xmlPath)
+    root = mytree.getroot()  
+
+    #get reference
+    chunk=root.find('chunk')
+    globalTransform=gmu.get_cartesian_transform(rotation=ut.literal_to_array(chunk.find('transform').find('rotation').text),
+                                                translation= ut.literal_to_array(chunk.find('transform').find('translation').text))
+    globalScale = np.identity(4)*float(chunk.find('transform').find('scale').text)
+    globalScale[-1,-1]=1  
+
+    #get components -> in some xml files, there are no components.
+    components=[]
+    for component in root.iter('component'):       
+        try:
+            transform=component.find('transform')
+            region=component.find('region')
+            scale = np.identity(4)*float(transform.find('scale').text)
+            scale[-1,-1]=1
+            components.append({'componentid':  int(component.get('id')),        
+                            'refTransform': gmu.get_cartesian_transform(rotation=ut.literal_to_array(transform.find('rotation').text),
+                                                translation= ut.literal_to_array(transform.find('translation').text)),
+                            'scale': scale,
+                            'center': gmu.get_cartesian_transform( translation=ut.literal_to_array(region.find('center').text)),
+                            'size': ut.literal_to_array(region.find('size').text),
+                            'R': ut.literal_to_array(region.find('R').text)})     
+        except:
+            components.append(None)
+            continue
+
+    #get sensors
+    sensors=[]
+    for sensor in root.iter('sensor'):       
+        try:
+            calibration=sensor.find('calibration')
+            focalLength35mm= calibration.find('f').text if calibration.find('f') is not None else calibration.find('fx').text # sometimes the focal length is named diffirently
+            sensors.append({'sensorid':  int(sensor.get('id'))   ,        
+                            'imageWidth': int(calibration.find('resolution').get('width')),
+                            'imageHeight': int(calibration.find('resolution').get('height')),
+                            'focalLength35mm': float(focalLength35mm)})     
+        except:
+            sensors.append(None)
+            continue
+    
+    #get image names in folder
+    files=ut.get_list_of_files(ut.get_folder(xmlPath))
+    files=[f for f in files if (f.endswith('.JPG') or 
+                                f.endswith('.PNG') or 
+                                f.endswith('.jpg') or
+                                f.endswith('.png'))]
+    names=[ut.get_filename(file) for file in files]
+
+    #get cameras
+    nodelist=[]   
+    for cam in root.iter('camera'):
+        try:
+            #get name
+            name=cam.get('label')
+            
+            #get component
+            componentid=cam.get('component_id')  
+            if componentid:
+                componentInformation= next(c for c in components if c['componentid']==int(componentid))  
+                refTransform=componentInformation['refTransform']
+                scale=componentInformation['scale']
+            else:
+                refTransform=globalTransform
+                scale=globalScale
+                
+            #get transform
+            transform=np.reshape(ut.literal_to_array(cam.find('transform').text),(4,4))
+            #apply scale and reference transformation
+            transform=refTransform  @ scale  @ transform
+
+            #get sensor information
+            sensorid=int(cam.get('sensor_id'))      
+            sensorInformation= next(s for s in sensors if s is not None and s.get('sensorid')==sensorid)
+
+            #create image node 
+            import uuid          
+            node=ImageNode(subject='file:///'+str(uuid.uuid1()),
+                        name=name, 
+                         cartesianTransform=transform,
+                        imageWidth =  int(sensorInformation['imageWidth']),
+                        imageHeight = int(sensorInformation['imageHeight'] ),
+                        focalLength35mm = sensorInformation['focalLength35mm'], 
+                        **kwargs)
+            # node.xmlPath=xmlPath
+            
+            #assign node to nodelist depending on whether it's in the folder    
+            try:
+                test1=ut.get_filename(node.name)
+                i=names.index(ut.get_filename(node.name))
+                node.path=files[i]
+                nodelist.append(node)   
+            except:
+                
+                None if filterByFolder else nodelist.append(node) 
+
+        except:
+            continue
+    return nodelist[0::skip] if skip else nodelist
 
 def e57path_to_nodes(e57Path:str,percentage:float=1.0) ->List[PointCloudNode]:
     """Load an e57 file and convert all data to a list of PointCloudNodes.\n
 
     **NOTE**: lowering the percentage barely affects assignment performance (numpy array assignments are extremely efficient). \n 
     Only do this to lower computational complexity or free up memory.
```

### Comparing `geomapi-0.1.9/geomapi/tools/alignmenttools/__init__.py` & `geomapi-0.2.0/geomapi/tools/alignmenttools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 "Tools to align different datasets using both images and 3d meshes"
 
 import datetime
 
 import numpy as np
 import quaternion
 import cv2
+from typing import List
 
 from geomapi.nodes import SessionNode
 import geomapi.utils.geometryutils as gu
 import geomapi.tools.alignmenttools.params as params
 import geomapi.tools.alignmenttools.match as match
 from geomapi.tools.alignmenttools.match import Match, Match2d, Match3d, PoseEstimation
 
 
 # returns all sessions that are within the bounding volume
-def find_close_sessions(boundingVolume: np.array, referenceSessions: list[SessionNode]) ->  list[SessionNode]:
+def find_close_sessions(boundingVolume: np.array, referenceSessions: List[SessionNode]) ->  List[SessionNode]:
     """Determines the close ennoug sessions based on bounding volumes
 
     Args:
         boundingVolume (np.array 6x1): The test bounding volume
         referenceSessions (list[SessionNode]): All the sessionNodes to check
 
     Returns:
@@ -60,15 +61,15 @@
     averageRotation = gu.weighted_average_quaternions(Q,w)
     averagePosition = np.average(T,axis = 0,weights = w)
 
     transformation = np.vstack((cv2.hconcat((quaternion.as_rotation_matrix(averageRotation), averagePosition)), np.array([0,0,0,1])))
 
     return transformation
 
-def estimate_session_position(testSession : SessionNode, refSessions: list[SessionNode]) -> np.array:
+def estimate_session_position(testSession : SessionNode, refSessions: List[SessionNode]) -> np.array:
     """Estimates the global position of a session in relation to a list of reference sessions
 
     Args:
         testSession (SessionNode): The Test Session where the positions needs to be determined from
         refSessions (list[SessionNode]): The Reference sessions to help calculate the new position
 
     Returns:
```

### Comparing `geomapi-0.1.9/geomapi/tools/alignmenttools/match.py` & `geomapi-0.2.0/geomapi/tools/alignmenttools/match.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/tools/alignmenttools/params.py` & `geomapi-0.2.0/geomapi/tools/alignmenttools/params.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/tools/completiontools/__init__.py` & `geomapi-0.2.0/geomapi/tools/completiontools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/tools/progresstools/__init__.py` & `geomapi-0.2.0/geomapi/tools/progresstools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,30 +175,28 @@
         1.images (List[np.array]): RGB or grayscale imagery.\n
         2.colorList (np.array, optional): list with RGB or grayscale colors used for the remapping. If no colors are provided, the unique colors of the first image will be taken. Defaults to None.
 
     Returns:
         np.array: image [m,n,1] with indices as mask
     """
     #validate inputs
-    images=images if type(images)==list else [images]
-    # for img in images:
-    #     if img.shape[1]==1:
-    #         img=img
-    #     else:    
-    #         img=iu.rgb2gray(img)
+    images=images if type(images)==list else [images]    
     images=[img if img.shape[2]==1 else iu.rgb2gray(img) for img in images]
-    colorList=colorList if colorList is not None else [ut.random_color() for u in range(np.unique(images[0]))]
+    
+    #create colors equal to number of unique values if no colorList is provided
+    colorList=colorList if colorList is not None else np.reshape(np.unique(images[0]),(len(np.unique(images[0])),1))
     colorList=colorList if colorList.shape[1]==1 else iu.rgb2gray(colorList)
+
     newImages=[]
     for img in images:
         #remap values
         for i,c in enumerate(colorList):
             # test1=
             # img=np.put(img,np.where(np.isclose(img,c,atol=0.01)),i)
-            img=np.where(np.isclose(img,c,atol=0.01),i+1,img)
+            img=np.where(np.isclose(img,c,atol=0.01),i,img)
             
         #replace other values by 0
         img=np.where(img<1,0,img)
         newImages.append(img)
     return newImages
     
 def project_meshes_to_rgbd_images (meshes:List[o3d.geometry.TriangleMesh], imgNodes:List[ImageNode], scale:float=1.0, fill_black:int=0)->Tuple[List[np.array],List[np.array]]:
```

### Comparing `geomapi-0.1.9/geomapi/tools/validationtools/__init__.py` & `geomapi-0.2.0/geomapi/tools/validationtools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/utils/__init__.py` & `geomapi-0.2.0/geomapi/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,28 +369,29 @@
                     gps_data[sub_decoded] = value[t]
 
                 exifData[decoded] = gps_data
             else:
                 exifData[decoded] = value        
         return exifData      
     else:
-        return None        
+        return None    
 
-def get_filename(path :str) -> str:
+
+def get_filename(path :str,splitter:str='.') -> str:
     """ Deconstruct filepath and return filename.
     
     Args:
         path (str): filepath
         
     Returns:
         filename (str)
     """   
     path=ntpath.basename(path)
     _, tail = ntpath.split(path)
-    array=tail.split('.')
+    array=tail.split(splitter)
     return array[0]
 
 def get_folder(path :str) -> str:
     """ Deconstruct path and return forlder
     
     Args:
         path (str): filepath
```

### Comparing `geomapi-0.1.9/geomapi/utils/geometryutils.py` & `geomapi-0.2.0/geomapi/utils/geometryutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,53 +354,142 @@
         open3d.geometry.LineSet: the lineset from the mesh.
     """
     assert len(color)==3 
     ls = o3d.geometry.LineSet.create_from_triangle_mesh(geometry)
     ls.paint_uniform_color(color)
     return ls
 
-def rays_to_points(rays:np.array,scale:float=1.0) -> Tuple[np.array,np.array]:
+def rays_to_points(rays:np.array,distances:np.array=np.array([1.0])) -> Tuple[np.array,np.array]:
     """Converts a set of rays to start-and endpoints.\n
 
     Args:
         1.rays (np.array[n,6] or o3d.core.Tensor): ray consisting of a startpoint np.array[n,0:3] and a direction np.array[n,3:6].\n
-        2.scale (float, optional): scalar to increase/decrease the magnitude of the ray. Defaults to 1.0.\n
+        2.distances (np.array[n], optional): scalar or array with distances of the ray. Defaults to 1.0m.\n
 
     Returns:
         Tuple[np.array,np.array]: startpoints, endpoints
     """
     #validate inputs
     if 'Tensor' in str(type(rays)):
         rays=rays.numpy()
     if 'array' in str(type(rays)):        
         assert rays.shape[-1]==6, f'rays.shape[1] should be 6, got {rays.shape[1]}.'
     if len(rays.shape)>2:
         rays=np.reshape(rays,(-1, 6))
+        
+    if distances.size !=rays.shape[0]:
+        distances=np.full((rays.shape[0],1),distances[0])
+    
+    #stack rays and distances
+    rays=np.hstack((rays,np.reshape(distances,(rays.shape[0],1))))
     
-    #stack start and end points from rays
+    #compute endpoints
     def myfunction(x):
-        return np.array([x[0] + x[3]*scale,x[1] + x[4]*scale,x[2] + x[5]*scale])
+        return np.array([x[0] + x[3]*x[-1],
+                         x[1] + x[4]*x[-1],
+                         x[2] + x[5]*x[-1]])
     startpoints=rays[:,0:3]
     endpoints=np.apply_along_axis(myfunction, axis=1, arr=rays)    
     
     return startpoints, endpoints
 
-def rays_to_lineset(rays:np.array,scale:float=1.0)->o3d.geometry.LineSet:
+    
+def project_meshes_to_rgbd_images (meshes:List[o3d.geometry.TriangleMesh], extrinsics: List[np.array],intrinsics:List[np.array], scale:float=1.0, fill_black:int=0)->Tuple[List[np.array],List[np.array]]:
+    """Project a set of meshes given camera parameters.
+
+    .. image:: ../../../docs/pics/colosseum/Raycasting_6.PNG
+
+    Args:
+        1.meshes (List[o3d.geometry.TriangleMesh]): set of TriangleMeshes.\n
+        2.imgNodes (List[ImageNode]): should contain imageWidth,imageHeight,cartesianTransform and focalLength35mm\n
+        3.scale (float, optional): scale to apply to imagery (typically for downscaling). Defaults to 1.\n
+        4.fill_black (int, optional): Region to fill in black pixels. 5 is a good value.\n
+        
+    Returns:
+        Tuple[List[np.array],List[np.array]]: colorImages,depthImages
+    """
+    #validate meshes
+    mesh=join_geometries(ut.item_to_list(meshes))
+    extrinsics=ut.item_to_list(extrinsics)
+    intrinsics=ut.item_to_list(intrinsics)
+    
+    
+    #create lists
+    colorImages=[]
+    depthImages=[]    
+    
+    #create raytracing scene
+    scene = o3d.t.geometry.RaycastingScene()
+    reference=o3d.t.geometry.TriangleMesh.from_legacy(mesh)
+    scene.add_triangles(reference)
+    
+    #create a colorArray from the mesh triangles (color of first vertex is taken)
+    colors=np.asarray(mesh.vertex_colors)
+    indices=np.asarray(mesh.triangles)[:,0]
+    triangle_colors=colors[indices]
+    #append black color at the end of the array for the invalid hits
+    triangle_colors=np.vstack((triangle_colors,np.array([0,0,0])))
+    
+    #create rays  
+    for e,i in zip(extrinsics,intrinsics):
+        rays = o3d.t.geometry.RaycastingScene.create_rays_pinhole(
+                                        intrinsic_matrix =i,
+                                        extrinsic_matrix =np.linalg.inv(e),
+                                        width_px=math.ceil((i[0,2]+0.5)*2),
+                                        height_px=math.ceil((i[1,2]+0.5)*2))
+        
+        #apply scale
+        rays=rays.numpy()
+        rays=o3d.core.Tensor(rays[::int(1/scale),::int(1/scale)])
+        #cast rays
+        ans = scene.cast_rays(rays) 
+        
+        #get triangle_ids that are hit per ray
+        triangle_ids=ans['primitive_ids'].numpy() # triangles
+        rows,columns=triangle_ids.shape        
+        triangle_ids=triangle_ids.flatten()
+        # replace invalid id's by last (which is the above added black color)
+        np.put(triangle_ids,np.where(triangle_ids==scene.INVALID_ID),triangle_colors.shape[0]-1) 
+        
+        #select colors 
+        colors=triangle_colors[triangle_ids]
+
+        #reshape array back to normal
+        colorImage=np.reshape(colors,(rows,columns,3))
+                
+        #fill black if necessary
+        colorImage=iu.fill_black_pixels(colorImage,fill_black)         if fill_black !=0       else colorImage
+        depthImage=iu.fill_black_pixels(ans['t_hit'].numpy(),fill_black)         if fill_black !=0       else ans['t_hit'].numpy()
+
+        #add to list
+        colorImages.append(colorImage)    
+        depthImages.append(depthImage)
+
+    return colorImages,depthImages
+
+def rays_to_lineset(rays:np.array,distances=None)->o3d.geometry.LineSet:
     """Convert an array or o3d.tensor to a lineset that can be visualized in open3d.\n
     
     .. image:: ../../../docs/pics/Raycasting_3.PNG
 
     Args:
-        rays (np.array[n,6] or o3d.core.Tensor): ray consisting of a startpoint np.array[n,0:3] and a direction np.array[n,3:6]\n
+        1.rays (np.array[n,6] or o3d.core.Tensor): ray consisting of a startpoint np.array[n,0:3] and a direction np.array[n,3:6]\n
+        2.distances (float or np.array[n],Optional): distance/distances over which to cast each ray. Defaults to 1.0m. 
 
     Returns:
         o3d.geometry.LineSet
     """
+    if distances is None:
+        distances=np.full((rays.shape[0],1),1)
+    elif type(distances)==float or type(distances)==int:
+        distances=np.full((rays.shape[0],1),distances)
+    distances[distances == np.inf] = 50
+        
     #get start and endpoints
-    startpoints, endpoints=rays_to_points(rays,scale)
+    startpoints, endpoints=rays_to_points(rays,distances)
     points=np.vstack((startpoints,endpoints))
     
     #create lines
     lines=[]
     start=np.arange(start=0,stop=rays.shape[0] )[..., np.newaxis]
     end=np.arange(start=rays.shape[0],stop=points.shape[0] )[..., np.newaxis]  
     lines = np.hstack((start, end))
@@ -408,14 +497,15 @@
     #create lineset
     line_set = o3d.geometry.LineSet()
     # colors = [[1, 0, 0] for i in range(len(lines))]
     line_set.points = o3d.utility.Vector3dVector(points)
     line_set.lines = o3d.utility.Vector2iVector(lines)
     return line_set
 
+
 def get_mesh_collisions_trimesh(sourceMesh: o3d.geometry.TriangleMesh, geometries: List[o3d.geometry.TriangleMesh]) -> List[int]:
     """Return indices of geometries that collide with the source.\n
 
     .. image:: ../../../docs/pics/collision_4.PNG
 
     Args:
         1. sourceMesh (o3d.geometry.TriangleMesh)\n
@@ -765,15 +855,15 @@
             normals=np.hstack((las['normalX'],las['normalY'],las['normalZ']))
             newNormals=transform_points(normals,transform) if transform is not None else normals
             pcd.normals=o3d.utility.Vector3dVector(newNormals)
         else:
             pcd.estimate_normals()
     return pcd
 
-def dataframe_to_pcd(df:pd.DataFrame,pointFields:List[str]=['x', 'y', 'z'],transform:np.array=None)->o3d.geometry.PointCloud:
+def dataframe_to_pcd(df:pd.DataFrame,xyz=[0,1,2],rgb=[3,4,5],n=None,transform:np.array=None)->o3d.geometry.PointCloud:
     """Convert Pandas dataframe to o3d.geometry.PointCloud.\n
 
     **NOTE**: this is slow. Ignoring color and normals speeds up the process by about 30%. More efficient method needed.\n
 
     Args:
         1. df (pd.DataFrame): Dataframe with named columns ['x', 'y', 'z'] and optional ['R', 'G', 'B'] and ['Nx', 'Ny', 'Nz'].\n
         2. pointFields (List[str]): optional column names. defaults to ['x', 'y', 'z','R', 'G', 'B','Nx', 'Ny', 'Nz']\n
@@ -785,40 +875,46 @@
         o3d.geometry.PointCloud 
     """
     #validate transform
     if transform is not None:
         assert transform.shape[0]==4
         assert transform.shape[1]==4
 
-    #validate pointfields    
-    if pointFields == None:
-        pointFields=['x', 'y', 'z','R', 'G', 'B','Nx', 'Ny', 'Nz']
-    fields=[s.casefold() for s in pointFields]
+    # #validate pointfields    
+    # if pointFields == None:
+    #     pointFields=['x', 'y', 'z','R', 'G', 'B','Nx', 'Ny', 'Nz']
+    # fields=[s.casefold() for s in pointFields]
 
     #create point cloud
     pcd=o3d.geometry.PointCloud()
-    if (all(elem.casefold() in fields for elem in ['X', 'Y', 'Z'])):
-        xyz=df.get([pointFields[0], pointFields[1], pointFields[2]])
-        # xyz=df.iloc[:,[0,1,2]]
-        newxyz=transform_points( xyz.to_numpy(),transform) if transform is not None else xyz.to_numpy()
-        pcd.points=o3d.utility.Vector3dVector(newxyz)
-    else:
-        raise ValueError('No valid xyz data. Make sure column headers are names X,Y,Z')
-
-    if (all(elem.casefold() in fields for elem in ['R', 'G', 'B'])): 
-        rgb=df.get(['R', 'G', 'B'])
-        colorArray=rgb.to_numpy()
-        if np.amax(colorArray)>1:
-            colorArray=colorArray/255
-        pcd.colors=o3d.utility.Vector3dVector(colorArray)
+    # if (all(elem.casefold() in fields for elem in ['X', 'Y', 'Z'])):
+        # xyz=df.get([pointFields[0], pointFields[1], pointFields[2]])
+    points=df.iloc[:,xyz].to_numpy()
+    points=transform_points( points,transform) if transform is not None else points
+    pcd.points=o3d.utility.Vector3dVector(points)
+    # else:
+    #     raise ValueError('No valid xyz data.')
+
+    # if (all(elem.casefold() in fields for elem in ['R', 'G', 'B'])): 
+        # rgb=df.get(['R', 'G', 'B'])
+    colors=df.iloc[:,rgb].to_numpy()        
+    colors=colors/255    if np.amax(colors)>1 else colors
+    pcd.colors=o3d.utility.Vector3dVector(colors)
+
+    # if (all(elem.casefold() in pointFields for elem in ['Nx', 'Ny', 'Nz'])): 
+    # nxyz=df.get(['Nx', 'Ny', 'Nz'])
+    if n:
+        normals=df.iloc[:,n].to_numpy()
+        normals=transform_points( normals,transform) if transform is not None else normals
+        pcd.normals=o3d.utility.Vector3dVector(normals)
 
-    if (all(elem.casefold() in pointFields for elem in ['Nx', 'Ny', 'Nz'])): 
-        nxyz=df.get(['Nx', 'Ny', 'Nz'])
-        newnxyz=transform_points( nxyz.to_numpy(),transform) if transform is not None else nxyz.to_numpy()
-        pcd.normals=o3d.utility.Vector3dVector(newnxyz)
+        
+    # newnxyz=transform_points( nxyz.to_numpy(),transform) if transform is not None else nxyz.to_numpy()
+    # pcd.normals=o3d.utility.Vector3dVector(newnxyz)
+    
     return pcd
 
 def e57_to_pcd(e57:pye57.e57.E57,e57Index : int = 0,percentage:float=1.0)->o3d.geometry.PointCloud:
     """Convert a scan from a pye57.e57.E57 file to o3d.geometry.PointCloud.\n
 
     Args:
         1. e57 (pye57.e57.E57)\n
@@ -1839,16 +1935,18 @@
 
     #transform XYZ
     if (all(elem.casefold() in fields for elem in ['X', 'Y', 'Z'])):
         xyz=df.get([pointFields[0], pointFields[1], pointFields[2]])
         newxyz=transform_points( xyz.to_numpy(),transform) if transform is not None else xyz.to_numpy()
         #replace column
         for i,n in enumerate([pointFields[0], pointFields[1], pointFields[2]]):
-            df.drop(n, axis = 1, inplace = True)
             df[n] = newxyz[:,i].tolist()
+
+            # df.drop(n, axis = 1, inplace = True)
+            # df[n] = newxyz[:,i].tolist()
     else:
         raise ValueError('No valid xyz data. Make sure column headers are names X,Y,Z')
 
     #transform ['Nx', 'Ny', 'Nz']
     if (all(elem.casefold() in pointFields for elem in ['Nx', 'Ny', 'Nz'])): 
         nxyz=df.get(['Nx', 'Ny', 'Nz'])
         newnxyz=transform_points( nxyz.to_numpy(),transform) if transform is not None else nxyz.to_numpy()
```

### Comparing `geomapi-0.1.9/geomapi/utils/geospatialutils.py` & `geomapi-0.2.0/geomapi/utils/geospatialutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/geomapi/utils/imageutils.py` & `geomapi-0.2.0/geomapi/utils/imageutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import geomapi.utils as ut
 
 from scipy.spatial.transform import Rotation
 from mpl_toolkits.mplot3d import Axes3D
 from PIL import Image
 import cv2
 
-def image_resize(img:np.array,width:int=None,height:int=None,scale:float=0.5)->np.array:
+def image_resize(img:np.array,width:int=None,height:int=None,scale:float=None)->np.array:
     """Resize an cv2 image (np.array).
 
     Args:
         1.img (np.array) \n
         2.width (int, optional): width in pixels. Defaults to None.\n
         3.height (int, optional): height in pixels. Defaults to None.\n
         4.scale (float, optional): percentual scale. Defaults to 0.5.\n
```

### Comparing `geomapi-0.1.9/geomapi.egg-info/PKG-INFO` & `geomapi-0.2.0/geomapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.1.9
+Version: 0.2.0
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geomapi-0.1.9/geomapi.egg-info/SOURCES.txt` & `geomapi-0.2.0/geomapi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 geomapi/nodes/pointcloudnode.py
 geomapi/nodes/sessionnode.py
 geomapi/tools/__init__.py
 geomapi/tools/alignmenttools/__init__.py
 geomapi/tools/alignmenttools/match.py
 geomapi/tools/alignmenttools/params.py
 geomapi/tools/completiontools/__init__.py
+geomapi/tools/inspectiontools/__init__.py
+geomapi/tools/machinelearningtools/__init__.py
 geomapi/tools/progresstools/__init__.py
 geomapi/tools/validationtools/__init__.py
 geomapi/utils/__init__.py
 geomapi/utils/geometryutils.py
 geomapi/utils/geospatialutils.py
 geomapi/utils/imageutils.py
 test/__init__.py
```

### Comparing `geomapi-0.1.9/setup.cfg` & `geomapi-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geomapi
-version = 0.1.9
+version = 0.2.0
 author = Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 description = A standard library to manage geomatic data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 keywords = Geomatics, alignment, monitoring, validation, progress, point clouds, computer vision, deep learning
 License = MIT
```

### Comparing `geomapi-0.1.9/test/test_alignmenttools.py` & `geomapi-0.2.0/test/test_alignmenttools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_bimnode.py` & `geomapi-0.2.0/test/test_bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_completiontools.py` & `geomapi-0.2.0/test/test_completiontools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_geometrynode.py` & `geomapi-0.2.0/test/test_geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_geometryutils.py` & `geomapi-0.2.0/test/test_geometryutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_geospatialutils.py` & `geomapi-0.2.0/test/test_geospatialutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_imageutils.py` & `geomapi-0.2.0/test/test_imageutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_imgnode.py` & `geomapi-0.2.0/test/test_imgnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_meshnode.py` & `geomapi-0.2.0/test/test_meshnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_node.py` & `geomapi-0.2.0/test/test_node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_pointcloudnode.py` & `geomapi-0.2.0/test/test_pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_progresstools.py` & `geomapi-0.2.0/test/test_progresstools.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,20 @@
         ifcSlab=ifc2.by_guid('2qZtnImXH6Tgdb58DjNlmF')
         ifcWall=ifc2.by_guid('06v1k9ENv8DhGMCvKUuLQV')
         ifcBeam=ifc2.by_guid('05Is7PfoXBjhBcbRTnzewz' )
         ifcColumn=ifc2.by_guid('23JN72MijBOfF91SkLzf3a')
         # ifcWindow=ifc.by_guid(cls.slabGlobalid) 
         # ifcDoor=ifc.by_guid(cls.slabGlobalid)
 
+        #IMG 
+        cls.xmlPath1=os.path.join(cls.path,'IMG','camera_position.xml')
+        cls.xmlPath2=os.path.join(cls.path,'IMG','cameras_bridge.xml')
+        cls.xmlPath3=os.path.join(cls.path,'IMG','cameras_paestum.xml')
+        
+        #MESH
         cls.slabMesh=gmu.ifc_to_mesh(ifcSlab)
         cls.wallMesh=gmu.ifc_to_mesh(ifcWall)
         cls.beamMesh=gmu.ifc_to_mesh(ifcBeam)
         cls.columnMesh=gmu.ifc_to_mesh(ifcColumn)
         
         #RESOURCES
         cls.resourcePath=os.path.join(cls.path,"resources")
```

### Comparing `geomapi-0.1.9/test/test_sessionnode.py` & `geomapi-0.2.0/test/test_sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.1.9/test/test_tools.py` & `geomapi-0.2.0/test/test_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,19 +39,19 @@
         #POINTCLOUD - XML
         cls.e57XmlPath=os.path.join(cls.path,'PCD',"week 22 - Lidar.xml") 
 
         #MESH
         cls.meshPath=os.path.join(cls.path,'MESH',"week22.obj")  
         # cls.mesh= o3d.io.read_triangle_mesh(cls.meshPath)
     
-        #IMG1
-        cls.imgXmlPath1=os.path.join(cls.path,'IMG',"camera_position.xml")  
-
-        #IMG2
-        cls.imgXmlPath2=os.path.join(cls.path,'IMG',"ReferenceLAMBERT08_TAW.xml")  
+        #IMG
+        cls.xmlPath1=os.path.join(cls.path,'IMG',"camera_position.xml")  
+        cls.xmlPath2=os.path.join(cls.path,'IMG',"ReferenceLAMBERT08_TAW.xml")  
+        cls.xmlPath3=os.path.join(cls.path,'IMG',"cameras_bridge.xml")  
+        cls.xmlPath4=os.path.join(cls.path,'IMG',"cameras_paestum.xml") 
         
         #IFC1
         cls.bimGraphPath1= os.path.join(cls.path,'sampleBimGraph.ttl') #os.path.join(cls.path,'bimGraph1.ttl')
         # cls.bimGraph1=Graph().parse(cls.bimGraphPath1)
         cls.ifcPath1=os.path.join(cls.path,'IFC',"Academiestraat_building_1.ifc")  
         # cls.ifc1=ifcopenshell.open(cls.ifcPath1)   
         
@@ -137,43 +137,25 @@
 
         # error when path doesn't exist
         self.assertRaises(ValueError,tl.e57xml_to_nodes,e57XmlPath=os.path.join(self.path,'PCD',"myXML.xml")    )
 
 
     def test_img_xml_to_nodes(self):
 
-        #XML1
-        nodes=tl.img_xml_to_nodes(self.imgXmlPath1) 
-        self.assertEqual(len(nodes),119)
-        self.assertIsNone(nodes[10].resource)
-        #0
-        self.assertAlmostEqual(nodes[0].cartesianTransform[0,3],6.645,delta=0.01)
-        #1
-        self.assertAlmostEqual(nodes[1].cartesianTransform[0,3],6.646,delta=0.01)
-
-        #kwargs
-        nodes=tl.img_xml_to_nodes(self.imgXmlPath1,sensor='DJI - Phantom 4') 
-        self.assertEqual(nodes[5].sensor,'DJI - Phantom 4')
+        self.assertEqual(len(tl.img_xml_to_nodes(self.xmlPath1,filterByFolder=False) ),86)
+        self.assertEqual(len(tl.img_xml_to_nodes(self.xmlPath1,filterByFolder=True) ),3)
+        nodes=tl.img_xml_to_nodes(self.xmlPath1,filterByFolder=True,getResource=True) 
+        self.assertEqual(len(nodes),3)
+        self.assertEqual(len([n.resource for n in nodes]),3)
+        
+        self.assertEqual(len(tl.img_xml_to_nodes(self.xmlPath3,filterByFolder=False) ),3123)
+        self.assertEqual(len(tl.img_xml_to_nodes(self.xmlPath3,skip=10,filterByFolder=False) ),313)
+                
+        self.assertEqual(len(tl.img_xml_to_nodes(self.xmlPath4,filterByFolder=False) ),894)
         
-        #getResource
-        # nodes=tl.img_xml_to_nodes(self.imgXmlPath1,getResource=True) 
-        # geometries=[n.resource for n in nodes]
-        # self.assertEqual(len(geometries),119)
-
-        #XML2
-        nodes=tl.img_xml_to_nodes(self.imgXmlPath2) 
-        self.assertEqual(len(nodes),21)
-        self.assertAlmostEqual(nodes[0].cartesianTransform[0,3],600575.992,delta=0.01)
-
-        # error when invalid extension
-        self.assertRaises(ValueError,tl.img_xml_to_nodes,xmlPath=os.path.join(self.path,'PCD',"myXML.e57") )
-
-        # error when path doesn't exist
-        self.assertRaises(ValueError,tl.img_xml_to_nodes,xmlPath=os.path.join(self.path,'IMG',"myXML.xml")    )
-
     def test_e57header_to_nodes(self):
 
         #E571
         nodes=tl.e57header_to_nodes(e57Path=self.e57Path1)
         self.assertEqual(len(nodes),2)
         self.assertIsNone(nodes[0]._resource)
         #0
```

### Comparing `geomapi-0.1.9/test/test_utils.py` & `geomapi-0.2.0/test/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class TestUtils(unittest.TestCase):
  ################################## SETUP/TEARDOWN CLASS ######################
     @classmethod
     def setUpClass(cls):
         #execute once before all tests
         print('-----------------Setup Class----------------------')
         st = time.time()
-        cls.path=os.path.join(os.getcwd(), "test","testfiles") #os.pardir, 
+        cls.path=os.path.join(os.getcwd(), "test","testfiles") 
         
         #GRAPH 1
         cls.graphPath1=os.path.join(cls.path,'bimGraph1.ttl')
         cls.graph1=Graph().parse(cls.graphPath1)
 
         #GRAPH 2
         cls.graphPath2=os.path.join(cls.path,'resourceGraph.ttl')
```

