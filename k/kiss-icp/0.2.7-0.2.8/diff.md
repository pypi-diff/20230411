# Comparing `tmp/kiss_icp-0.2.7.tar.gz` & `tmp/kiss_icp-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiss_icp-0.2.7.tar", last modified: Fri Apr  7 16:10:11 2023, max compression
+gzip compressed data, was "kiss_icp-0.2.8.tar", last modified: Tue Apr 11 15:31:07 2023, max compression
```

## Comparing `kiss_icp-0.2.7.tar` & `kiss_icp-0.2.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.378833 kiss_icp-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-07 16:10:11.378833 kiss_icp-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.374833 kiss_icp-0.2.7/kiss_icp/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.374833 kiss_icp-0.2.7/kiss_icp/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.374833 kiss_icp-0.2.7/kiss_icp/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/apollo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/boreas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/kitti.py
--rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/kitti_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/mulran.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/ncd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/nclt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/nuscenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/ouster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/paris_luco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/rosbag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/datasets/tum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/deskew.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/kiss_icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.378833 kiss_icp-0.2.7/kiss_icp/pybind/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/pybind/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/pybind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/pybind/kiss_icp_pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.378833 kiss_icp-0.2.7/kiss_icp/pybind/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/pybind/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/pybind/pybind11/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/pybind/stl_vector_eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.378833 kiss_icp-0.2.7/kiss_icp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/tools/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/tools/pipeline_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/tools/point_cloud2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/tools/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/tools/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/kiss_icp/voxelization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:10:11.374833 kiss_icp-0.2.7/kiss_icp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-07 16:10:11.000000 kiss_icp-0.2.7/kiss_icp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-07 16:10:11.000000 kiss_icp-0.2.7/kiss_icp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:10:11.000000 kiss_icp-0.2.7/kiss_icp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 16:10:11.000000 kiss_icp-0.2.7/kiss_icp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 16:10:11.000000 kiss_icp-0.2.7/kiss_icp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-07 16:10:11.000000 kiss_icp-0.2.7/kiss_icp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-07 16:10:11.378833 kiss_icp-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-07 16:10:00.000000 kiss_icp-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.890225 kiss_icp-0.2.8/kiss_icp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/apollo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/boreas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/kitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/kitti_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/mulran.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/ncd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/nclt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/nuscenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/ouster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/paris_luco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/datasets/tum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/deskew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/kiss_icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/pybind/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/kiss_icp_pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/pybind/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/pybind11/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/pybind/stl_vector_eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/pipeline_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/point_cloud2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/tools/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/kiss_icp/voxelization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:31:07.894225 kiss_icp-0.2.8/kiss_icp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 15:31:07.000000 kiss_icp-0.2.8/kiss_icp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-11 15:31:07.898224 kiss_icp-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-11 15:30:56.000000 kiss_icp-0.2.8/setup.py
```

### Comparing `kiss_icp-0.2.7/CMakeLists.txt` & `kiss_icp-0.2.8/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 cmake_minimum_required(VERSION 3.16...3.26)
-project(kiss_icp_pybind VERSION 0.2.7 LANGUAGES CXX)
+project(kiss_icp_pybind VERSION 0.2.8 LANGUAGES CXX)
 
 # Set build type
 set(CMAKE_BUILD_TYPE Release)
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
 if(EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/../cpp/kiss_icp/)
```

### Comparing `kiss_icp-0.2.7/LICENSE` & `kiss_icp-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/PKG-INFO` & `kiss_icp-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiss_icp
-Version: 0.2.7
+Version: 0.2.8
 Summary: Simple yet effective 3D LiDAR-Odometry registration pipeline
 Home-page: https://github.com/PRBonn/kiss-icp
 Author: Ignacio Vizzo
 Author-email: ignaciovizzo@gmail.com
 License: MIT
 Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kiss_icp Version: 0.2.7 Summary: Simple yet
+Metadata-Version: 2.1 Name: kiss_icp Version: 0.2.8 Summary: Simple yet
 effective 3D LiDAR-Odometry registration pipeline Home-page: https://
 github.com/PRBonn/kiss-icp Author: Ignacio Vizzo Author-email:
 ignaciovizzo@gmail.com License: MIT Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Programming
 Language :: C++ Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `kiss_icp-0.2.7/README.md` & `kiss_icp-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/__init__.py` & `kiss_icp-0.2.8/kiss_icp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__version__ = "0.2.7"
+__version__ = "0.2.8"
```

### Comparing `kiss_icp-0.2.7/kiss_icp/config/__init__.py` & `kiss_icp-0.2.8/kiss_icp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/config/config.py` & `kiss_icp-0.2.8/kiss_icp/config/config.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/config/parser.py` & `kiss_icp-0.2.8/kiss_icp/config/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # NOTE: This module was contributed by Markus Pielmeier on PR #63
 from __future__ import annotations
+
 import importlib
-from pathlib import Path
 import sys
+from pathlib import Path
 from typing import Any, Dict, Optional
 
 from pydantic import BaseSettings, PrivateAttr
 
 from kiss_icp.config.config import AdaptiveThresholdConfig, DataConfig, MappingConfig
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/__init__.py` & `kiss_icp-0.2.8/kiss_icp/datasets/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,14 +46,22 @@
     import os.path
     import pkgutil
 
     pkgpath = os.path.dirname(__file__)
     return [name for _, name, _ in pkgutil.iter_modules([pkgpath])]
 
 
+def jumpable_dataloaders():
+    _jumpable_dataloaders = available_dataloaders()
+    _jumpable_dataloaders.remove("mcap")
+    _jumpable_dataloaders.remove("ouster")
+    _jumpable_dataloaders.remove("rosbag")
+    return _jumpable_dataloaders
+
+
 def dataloader_types() -> Dict:
     import ast
     import importlib
 
     dataloaders = available_dataloaders()
     _types = {}
     for dataloader in dataloaders:
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/apollo.py` & `kiss_icp-0.2.8/kiss_icp/datasets/apollo.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import glob
 import importlib
 import os
-from pathlib import Path
 import sys
+from pathlib import Path
 
 import natsort
 import numpy as np
 from pyquaternion import Quaternion
 
 
 class ApolloDataset:
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/boreas.py` & `kiss_icp-0.2.8/kiss_icp/datasets/boreas.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/generic.py` & `kiss_icp-0.2.8/kiss_icp/datasets/generic.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import os
-from pathlib import Path
 import sys
+from pathlib import Path
 
 import natsort
 import numpy as np
 
 from kiss_icp.datasets import supported_file_extensions
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/kitti.py` & `kiss_icp-0.2.8/kiss_icp/datasets/kitti.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/kitti_raw.py` & `kiss_icp-0.2.8/kiss_icp/datasets/kitti_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from collections import namedtuple
 import glob
 import os
+from collections import namedtuple
 from pathlib import Path
 
 import numpy as np
 
-
 __raw_to_odometry_mapping__ = {
     0: "2011_10_03/2011_10_03_drive_0027_sync/",
     1: "2011_10_03/2011_10_03_drive_0042_sync/",
     2: "2011_10_03/2011_10_03_drive_0034_sync/",
     4: "2011_09_30/2011_09_30_drive_0016_sync/",
     5: "2011_09_30/2011_09_30_drive_0018_sync/",
     6: "2011_09_30/2011_09_30_drive_0020_sync/",
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/mcap.py` & `kiss_icp-0.2.8/kiss_icp/datasets/mcap.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 
 class McapDataloader:
     def __init__(self, data_dir: str, topic: str, *_, **__):
         """Standalone .mcap dataloader withouth any ROS distribution."""
         # Conditional imports to avoid injecting dependencies for non mcap users
         try:
-            from mcap_ros2.reader import read_ros2_messages
             from mcap.reader import make_reader
+            from mcap_ros2.reader import read_ros2_messages
         except ImportError as e:
             print("mcap plugins not installed: 'pip install mcap-ros2-support'")
             exit(1)
 
         from kiss_icp.tools.point_cloud2 import read_point_cloud
 
         # we expect `data_dir` param to be a path to the .mcap file, so rename for clarity
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/mulran.py` & `kiss_icp-0.2.8/kiss_icp/datasets/mulran.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/ncd.py` & `kiss_icp-0.2.8/kiss_icp/datasets/ncd.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import importlib
 import os
-from pathlib import Path
 import re
+from pathlib import Path
 
 import numpy as np
 from pyquaternion import Quaternion
 
 
 class NewerCollegeDataset:
     def __init__(self, data_dir: Path, *_, **__):
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/nclt.py` & `kiss_icp-0.2.8/kiss_icp/datasets/nclt.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import os
-from pathlib import Path
 import sys
+from pathlib import Path
 
 import numpy as np
 
 
 class NCLTDataset:
     """Adapted from PyLidar-SLAM"""
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/nuscenes.py` & `kiss_icp-0.2.8/kiss_icp/datasets/nuscenes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import importlib
 import os
-from pathlib import Path
 import sys
+from pathlib import Path
 from typing import List
 
 import numpy as np
 
 
 class NuScenesDataset:
     def __init__(self, data_dir: Path, sequence: int, *_, **__):
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/ouster.py` & `kiss_icp-0.2.8/kiss_icp/datasets/ouster.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import glob
 import os
 from typing import Optional
 
 import numpy as np
-import glob
 
 
 def find_metadata_json(pcap_file: str) -> str:
     """Attempts to resolve the metadata json file for a provided pcap file."""
     dir_path, filename = os.path.split(pcap_file)
     if not filename:
         return ""
@@ -79,16 +79,16 @@
             meta: path to a metadata json file that should be recorded together with
             a pcap file. If `meta` is not provided attempts to find the best matching
             json file with the longest commong prefix of the pcap file (`data_dir`) in
             the same directory.
         """
 
         try:
-            from ouster import client
             import ouster.pcap as pcap
+            from ouster import client
         except ImportError:
             print(f'ouster-sdk is not installed on your system, run "pip install ouster-sdk"')
             exit(1)
 
         # since we import ouster-sdk's client module locally, we keep it locally as well
         self._client = client
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/paris_luco.py` & `kiss_icp-0.2.8/kiss_icp/datasets/paris_luco.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/rosbag.py` & `kiss_icp-0.2.8/kiss_icp/datasets/rosbag.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import os
-from pathlib import Path
 import sys
+from pathlib import Path
 from typing import Sequence
 
 import natsort
 
 
 class RosbagDataset:
     def __init__(self, data_dir: Sequence[Path], topic: str, *_, **__):
```

### Comparing `kiss_icp-0.2.7/kiss_icp/datasets/tum.py` & `kiss_icp-0.2.8/kiss_icp/datasets/tum.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import importlib
 import os
 from pathlib import Path
-from pyquaternion import Quaternion
+
 import numpy as np
+from pyquaternion import Quaternion
 
 
 class TUMDataset:
     def __init__(self, data_dir: Path, *_, **__):
         try:
             self.o3d = importlib.import_module("open3d")
         except ModuleNotFoundError as err:
```

### Comparing `kiss_icp-0.2.7/kiss_icp/deskew.py` & `kiss_icp-0.2.8/kiss_icp/deskew.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/kiss_icp.py` & `kiss_icp-0.2.8/kiss_icp/kiss_icp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import numpy as np
 
 from kiss_icp.config import KISSConfig
 from kiss_icp.deskew import get_motion_compensator
 from kiss_icp.mapping import get_voxel_hash_map
-from kiss_icp.registration import register_frame
 from kiss_icp.preprocess import get_preprocessor
+from kiss_icp.registration import register_frame
 from kiss_icp.threshold import get_threshold_estimator
 from kiss_icp.voxelization import voxel_down_sample
 
 
 class KissICP:
     def __init__(self, config: KISSConfig):
         self.poses = []
```

### Comparing `kiss_icp-0.2.7/kiss_icp/mapping.py` & `kiss_icp-0.2.8/kiss_icp/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-import numpy as np
 from typing import Tuple
 
+import numpy as np
+
 from kiss_icp.config import KISSConfig
 from kiss_icp.pybind import kiss_icp_pybind
 
 
 def get_voxel_hash_map(config: KISSConfig):
     return VoxelHashMap(
         voxel_size=config.mapping.voxel_size,
```

### Comparing `kiss_icp-0.2.7/kiss_icp/metrics.py` & `kiss_icp-0.2.8/kiss_icp/metrics.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/pipeline.py` & `kiss_icp-0.2.8/kiss_icp/pipeline.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import contextlib
 import datetime
 import os
-from pathlib import Path
 import time
+from pathlib import Path
 from typing import List, Optional
 
 import numpy as np
 from pyquaternion import Quaternion
 
 from kiss_icp.config import load_config, write_config
 from kiss_icp.kiss_icp import KissICP
```

### Comparing `kiss_icp-0.2.7/kiss_icp/preprocess.py` & `kiss_icp-0.2.8/kiss_icp/preprocess.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/pybind/CMakeLists.txt` & `kiss_icp-0.2.8/kiss_icp/pybind/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/pybind/__init__.py` & `kiss_icp-0.2.8/kiss_icp/pybind/__init__.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/pybind/kiss_icp_pybind.cpp` & `kiss_icp-0.2.8/kiss_icp/pybind/kiss_icp_pybind.cpp`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/pybind/pybind11/LICENSE` & `kiss_icp-0.2.8/kiss_icp/pybind/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/pybind/pybind11/pybind11.cmake` & `kiss_icp-0.2.8/kiss_icp/pybind/pybind11/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/pybind/stl_vector_eigen.h` & `kiss_icp-0.2.8/kiss_icp/pybind/stl_vector_eigen.h`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/registration.py` & `kiss_icp-0.2.8/kiss_icp/registration.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import numpy as np
 
-from kiss_icp.pybind import kiss_icp_pybind
 from kiss_icp.mapping import VoxelHashMap
+from kiss_icp.pybind import kiss_icp_pybind
 
 
 def register_frame(
     points: np.ndarray,
     voxel_map: VoxelHashMap,
     initial_guess: np.ndarray,
     max_correspondance_distance: float,
```

### Comparing `kiss_icp-0.2.7/kiss_icp/threshold.py` & `kiss_icp-0.2.8/kiss_icp/threshold.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/tools/__init__.py` & `kiss_icp-0.2.8/kiss_icp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/tools/cmd.py` & `kiss_icp-0.2.8/kiss_icp/tools/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from kiss_icp.datasets import (
     available_dataloaders,
+    jumpable_dataloaders,
     sequence_dataloaders,
     supported_file_extensions,
 )
 
 
 def guess_dataloader(data: Path, default_dataloader: str):
     """Guess which dataloader to use in case the user didn't specify with --dataloader flag.
@@ -52,15 +53,15 @@
     elif data.is_dir():
         if (data / "metadata.yaml").exists():
             # a directory with a metadata.yaml must be a ROS2 bagfile
             return "rosbag", data
         bagfiles = [Path(path) for path in glob.glob(os.path.join(data, "*.bag"))]
         if len(bagfiles) > 0:
             return "rosbag", bagfiles
-    return default_dataloader
+    return default_dataloader, data
 
 
 def version_callback(value: bool):
     if value:
         import kiss_icp
 
         print(f"KISS-ICP Version: {kiss_icp.__version__}")
@@ -203,14 +204,18 @@
         dataloader, data = guess_dataloader(data, default_dataloader="generic")
 
     # Validate some options
     if dataloader in sequence_dataloaders() and sequence is None:
         print('You must specify a sequence "--sequence"')
         raise typer.Exit(code=1)
 
+    if jump != 0 and dataloader not in jumpable_dataloaders():
+        print(f"[WARNING] '{dataloader}' does not support '--jump', starting from first frame")
+        jump = 0
+
     # Lazy-loading for faster CLI
     from kiss_icp.datasets import dataset_factory
     from kiss_icp.pipeline import OdometryPipeline
 
     OdometryPipeline(
         dataset=dataset_factory(
             dataloader=dataloader,
```

### Comparing `kiss_icp-0.2.7/kiss_icp/tools/pipeline_results.py` & `kiss_icp-0.2.8/kiss_icp/tools/pipeline_results.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/tools/point_cloud2.py` & `kiss_icp-0.2.8/kiss_icp/tools/point_cloud2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
 import sys
 from typing import Iterable, List, Optional, Tuple
 
 import numpy as np
 
 try:
-    from rosbags.typesys.types import sensor_msgs__msg__PointField as PointField
     from rosbags.typesys.types import sensor_msgs__msg__PointCloud2 as PointCloud2
+    from rosbags.typesys.types import sensor_msgs__msg__PointField as PointField
 except ImportError as e:
     raise ImportError('rosbags library not installed, run "pip install -U rosbags"') from e
 
 
 _DATATYPES = {}
 _DATATYPES[PointField.INT8] = np.dtype(np.int8)
 _DATATYPES[PointField.UINT8] = np.dtype(np.uint8)
```

### Comparing `kiss_icp-0.2.7/kiss_icp/tools/progress_bar.py` & `kiss_icp-0.2.8/kiss_icp/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp/tools/visualizer.py` & `kiss_icp-0.2.8/kiss_icp/tools/visualizer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from abc import ABC
 import copy
-from functools import partial
 import importlib
 import os
+from abc import ABC
+from functools import partial
 from typing import Callable, List
 
 import numpy as np
 
 YELLOW = np.array([1, 0.706, 0])
 RED = np.array([128, 0, 0]) / 255.0
 BLACK = np.array([0, 0, 0]) / 255.0
```

### Comparing `kiss_icp-0.2.7/kiss_icp/voxelization.py` & `kiss_icp-0.2.8/kiss_icp/voxelization.py`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/kiss_icp.egg-info/PKG-INFO` & `kiss_icp-0.2.8/kiss_icp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiss-icp
-Version: 0.2.7
+Version: 0.2.8
 Summary: Simple yet effective 3D LiDAR-Odometry registration pipeline
 Home-page: https://github.com/PRBonn/kiss-icp
 Author: Ignacio Vizzo
 Author-email: ignaciovizzo@gmail.com
 License: MIT
 Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kiss-icp Version: 0.2.7 Summary: Simple yet
+Metadata-Version: 2.1 Name: kiss-icp Version: 0.2.8 Summary: Simple yet
 effective 3D LiDAR-Odometry registration pipeline Home-page: https://
 github.com/PRBonn/kiss-icp Author: Ignacio Vizzo Author-email:
 ignaciovizzo@gmail.com License: MIT Keywords: SLAM,LiDAR,Odometry,Localization
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Programming
 Language :: C++ Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `kiss_icp-0.2.7/kiss_icp.egg-info/SOURCES.txt` & `kiss_icp-0.2.8/kiss_icp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiss_icp-0.2.7/setup.cfg` & `kiss_icp-0.2.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kiss_icp
-version = 0.2.7
+version = 0.2.8
 author = Ignacio Vizzo
 author_email = ignaciovizzo@gmail.com
 description = Simple yet effective 3D LiDAR-Odometry registration pipeline
 long_description = file:README.md,
 long_description_content_type = text/markdown
 url = https://github.com/PRBonn/kiss-icp
 license = MIT
```

### Comparing `kiss_icp-0.2.7/setup.py` & `kiss_icp-0.2.8/setup.py`

 * *Files identical despite different names*

