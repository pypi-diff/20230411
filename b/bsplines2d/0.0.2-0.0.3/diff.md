# Comparing `tmp/bsplines2d-0.0.2.tar.gz` & `tmp/bsplines2d-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsplines2d-0.0.2.tar", last modified: Thu Mar 16 21:32:38 2023, max compression
+gzip compressed data, was "bsplines2d-0.0.3.tar", last modified: Tue Apr 11 08:09:55 2023, max compression
```

## Comparing `bsplines2d-0.0.2.tar` & `bsplines2d-0.0.3.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:32:38.844754 bsplines2d-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-16 21:32:38.844754 bsplines2d-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/_updateversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:32:38.844754 bsplines2d-0.0.2/bsplines2d/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_Mesh2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_checks_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_checks_2d_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_checks_2d_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_checks_2d_tri.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_rect_cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class01_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_BSplines2D.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_bsplines_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_bsplines_operators_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_bsplines_operators_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_bsplines_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_bsplines_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_bsplines_tri.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    27776 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_contours.py
--rw-r--r--   0 runner    (1001) docker     (123)    54307 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_interpolate_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_plot_as_profile2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class02_plot_as_profile2d_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class03_Bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class03_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class03_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    21736 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_class11_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_generic_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_generic_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_utils_bsplines.py
--rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/_utils_bsplines_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:32:38.844754 bsplines2d-0.0.2/bsplines2d/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/test_01_Mesh2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/test_02_BSplines2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:32:38.844754 bsplines2d-0.0.2/bsplines2d/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/test_data/WEST_Poly.npz
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/test_data/WEST_trimesh.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/test_data/trimesh_quad.npz
--rw-r--r--   0 runner    (1001) docker     (123)    25845 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/bsplines2d/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 21:32:38.000000 bsplines2d-0.0.2/bsplines2d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 21:32:38.844754 bsplines2d-0.0.2/bsplines2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-16 21:32:38.000000 bsplines2d-0.0.2/bsplines2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-16 21:32:38.000000 bsplines2d-0.0.2/bsplines2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 21:32:38.000000 bsplines2d-0.0.2/bsplines2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-16 21:32:38.000000 bsplines2d-0.0.2/bsplines2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-16 21:32:38.000000 bsplines2d-0.0.2/bsplines2d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 21:32:38.844754 bsplines2d-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-03-16 21:32:24.000000 bsplines2d-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/_updateversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.589397 bsplines2d-0.0.3/bsplines2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_Mesh2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_tri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_rect_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22224 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class01_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_BSplines2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_bsplines_tri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_contours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54051 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_interpolate_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class03_Bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class03_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class03_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21736 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_class11_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_generic_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_generic_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_utils_bsplines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/_utils_bsplines_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.589397 bsplines2d-0.0.3/bsplines2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_01_Mesh2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_02_BSplines2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/bsplines2d/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_Poly.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_trimesh.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_data/trimesh_quad.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    26411 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/bsplines2d/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:09:55.589397 bsplines2d-0.0.3/bsplines2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 08:09:55.000000 bsplines2d-0.0.3/bsplines2d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:09:55.593397 bsplines2d-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-11 08:09:32.000000 bsplines2d-0.0.3/setup.py
```

### Comparing `bsplines2d-0.0.2/LICENSE` & `bsplines2d-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/PKG-INFO` & `bsplines2d-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsplines2d
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library for generic multidimensional bsplines on various meshes, using datastock
 Home-page: https://github.com/ToFuProject/bsplines2d
 Author: Didier VEZINET
 Author-email: didier.vezinet@gmail.com
 License: MIT
 Keywords: bsplines data analysis modelling mesh plot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bsplines2d-0.0.2/_updateversion.py` & `bsplines2d-0.0.3/_updateversion.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_Mesh2D.py` & `bsplines2d-0.0.3/bsplines2d/_class01_Mesh2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # -*- coding: utf-8 -*-
 
 
-# Built-in
-import copy
-
-
 # Common
-import numpy as np
 import datastock as ds
 
 
 # local
 from . import _generic_mesh
 from . import _class01_checks_1d as _checks_1d
 from . import _class01_checks_2d_rect as _checks_2d_rect
 from . import _class01_checks_2d_tri as _checks_2d_tri
-from . import _class01_checks_2d_polar as _checks_2d_polar
+# from . import _class01_checks_2d_polar as _checks_2d_polar
+
 
 from . import _class01_rect_cropping as _cropping
 from . import _class01_select as _select
 from . import _class01_sample as _sample
+from . import _class01_outline as _outline
 from . import _class01_plot as _plot
 
 
 __all__ = ['Mesh2D']
 
 
 # #############################################################################
@@ -457,14 +454,15 @@
         grid=None,
         mode=None,
         x0=None,
         x1=None,
         Dx0=None,
         Dx1=None,
         imshow=None,
+        in_mesh=None,
         # store
         store=None,
         kx0=None,
         kx1=None,
     ):
         """ Return a sampled version of the chosen mesh """
         return _sample.sample_mesh(
@@ -474,21 +472,38 @@
             grid=grid,
             mode=mode,
             x0=x0,
             x1=x1,
             Dx0=Dx0,
             Dx1=Dx1,
             imshow=imshow,
+            in_mesh=in_mesh,
             # store
             store=store,
             kx0=kx0,
             kx1=kx1,
         )
 
     # -----------------
+    # outline
+    # ------------------
+
+    def get_mesh_outline(
+        self,
+        key=None,
+        closed=None,
+    ):
+        """ Get outline of 2d mesh """
+        return _outline._get_outline(
+            coll=self,
+            key=key,
+            closed=closed,
+        )
+
+    # -----------------
     # plotting
     # ------------------
 
     def plot_mesh(
         self,
         key=None,
         ind_knot=None,
```

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_checks_1d.py` & `bsplines2d-0.0.3/bsplines2d/_class01_checks_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_checks_2d_polar.py` & `bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_polar.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_checks_2d_rect.py` & `bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_checks_2d_tri.py` & `bsplines2d-0.0.3/bsplines2d/_class01_checks_2d_tri.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_plot.py` & `bsplines2d-0.0.3/bsplines2d/_class01_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_rect_cropping.py` & `bsplines2d-0.0.3/bsplines2d/_class01_rect_cropping.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_sample.py` & `bsplines2d-0.0.3/bsplines2d/_class01_sample.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,147 +1,138 @@
 # -*- coding: utf-8 -*-
 
 
-# Built-in
-import copy
-import warnings
-
-
 # Common
 import numpy as np
-from scipy.spatial import ConvexHull
-from matplotlib.path import Path
-from contourpy import contour_generator
 import datastock as ds
+from matplotlib import path
 
 
 # tofu
 from . import _generic_mesh
-from . import _utils_bsplines
-# from . import _class02_checks as _checks
-from . import _class02_bsplines_rect
-from . import _class02_bsplines_tri
-from . import _class02_bsplines_polar
-from . import _class02_bsplines_1d
 
 
-# #############################################################################
-# #############################################################################
-#                           main
-# #############################################################################
+# ##############################################################
+# ##############################################################
+#                       Main
+# ##############################################################
 
 
 def sample_mesh(
     coll=None,
     key=None,
     res=None,
     mode=None,
     x0=None,
     x1=None,
+    grid=None,
+    # options
     Dx0=None,
     Dx1=None,
-    grid=None,
+    submesh=None,
+    # output for 2d
     imshow=None,
+    return_ind=None,
+    in_mesh=None,
     # store
     store=None,
     kx0=None,
     kx1=None,
 ):
 
     # -------------
     # check inputs
 
-    # key
-    key, _, cat = _generic_mesh._get_key_mesh_vs_bplines(
+    (
+        key, nd, mtype,
+        mode, res, submesh,
+        grid, imshow, store,
+    ) = _check(
         coll=coll,
         key=key,
-        which=coll._which_mesh,
-    )
-
-    nd = coll.dobj[cat][key]['nd']
-    mtype = coll.dobj[cat][key]['type']
-
-    # mode
-    mode = ds._generic_check._check_var(
-        mode, 'mode',
-        types=str,
-        default='abs',
+        mode=mode,
+        res=res,
+        submesh=submesh,
+        grid=grid,
+        imshow=imshow,
+        store=store,
+        x0=x0,
+        x1=x1,
     )
 
-    # res
-    if res is None:
-        res = _get_sample_mesh_res(
-            coll=coll,
-            keym=key,
-            nd=nd,
-            mtype=mtype,
-        )
-
     # ------------
     # sample
 
     if nd == '1d':
 
         # check
-        key, mode, Dx, knots, store = _sample_mesh_check_1d(
+        knots, Dx = _check_1d(
             coll=coll,
             key=key,
-            res=res,
-            mode=mode,
             Dx=Dx0,
-            store=store,
+            mode=mode,
         )
 
-        # compute
-        dref, ddata = sample_mesh_1d(
-            coll=coll,
-            key=key,
+        # sample
+        x0 = _sample_1d(
             res=res,
             mode=mode,
-            Dx=Dx,
             knots=knots,
+            Dx=Dx,
+        )
+
+        # prepare storing
+        dref, ddata = _store_1d(
+            coll=coll,
+            key=key,
+            x0=x0,
             # store
             store=store,
             kx0=kx0,
         )
 
     else:
 
         # check
-        (
-            key, res, mode, grid, imshow,
-            x0, x1, Dx0, Dx1, x0k, x1k,
-            store,
-        ) = _sample_mesh_check_2d(
+        knots0, knots1, x0, x1, Dx0, Dx1 = _check_2d(
             coll=coll,
             key=key,
-            res=res,
+            x0=x0,
+            x1=x1,
+            Dx0=Dx0,
+            Dx1=Dx1,
             mode=mode,
-            grid=grid,
-            imshow=imshow,
-            R=x0,
-            Z=x1,
-            DR=Dx0,
-            DZ=Dx1,
-            store=store,
+            mtype=mtype,
         )
 
-        dref, ddata = sample_mesh_2d(
+        # sample
+        x0, x1, ind = _sample_2d(
             coll=coll,
             key=key,
             res=res,
             mode=mode,
+            knots0=knots0,
+            knots1=knots1,
             x0=x0,
             x1=x1,
             Dx0=Dx0,
             Dx1=Dx1,
-            x0k=x0k,
-            x1k=x1k,
+            # options
             grid=grid,
             imshow=imshow,
+            in_mesh=in_mesh,
+        )
+
+        # prepare storing
+        dref, ddata = _store_2d(
+            coll=coll,
+            key=key,
+            x0=x0,
+            x1=x1,
+            ind=ind,
             # store
             store=store,
             kx0=kx0,
             kx1=kx1,
         )
 
     # -------------
@@ -156,273 +147,495 @@
 
     # --------
     # return
 
     return ddata
 
 
-# ###################################################################
-# ###################################################################
+# ##################################################################
+# ##################################################################
 #                       checks
-# ###################################################################
+# ##################################################################
 
 
-def _sample_mesh_check_1d(
+def _check(
     coll=None,
     key=None,
-    res=None,
     mode=None,
-    Dx=None,
-    mtype=None,
+    res=None,
+    submesh=None,
+    grid=None,
+    imshow=None,
     store=None,
+    x0=None,
+    x1=None,
 ):
 
-    # -----------
-    # Parameters
+    # ---------
+    # mesh
 
-    # for polar mesh => sample underlying mesh
-    if len(coll.dobj[coll._which_mesh][key]['shape-c']) > 1:
-        msg = "Wrong mesh dimension!"
-        raise Exception(msg)
+    # submesh
+    submesh = ds._generic_check._check_var(
+        submesh, 'submesh',
+        types=bool,
+        default=False,
+    )
 
-    if not (np.isscalar(res) and res > 0.):
-        msg = f"Arg res must be a positive float!\nProvided: {res}"
-        raise Exception(msg)
+    # key
+    wm = coll._which_mesh
+    key, _, cat = _generic_mesh._get_key_mesh_vs_bplines(
+        coll=coll,
+        key=key,
+        which=wm,
+    )
 
-    # -------------
-    # knots
+    nd = coll.dobj[cat][key]['nd']
+    mtype = coll.dobj[cat][key]['type']
 
-    kknots = coll.dobj[coll._which_mesh][key]['knots'][0]
-    knots = coll.ddata[kknots]['data']
+    if nd == '1d' and submesh is True:
+        if coll.dobj[wm][key]['submesh'] is not None:
+            key = coll.dobj[wm][key]['submesh']
+            nd = coll.dobj[cat][key]['nd']
+            mtype = coll.dobj[cat][key]['type']
 
-    # custom DR or DZ for mode='abs' only
-    if Dx is not None:
-        if mode != 'abs':
-            msg = "Custom Dx can only be provided with mode = 'abs'!"
-            raise Exception(msg)
+    # ----------
+    # resolution
 
-            c0 = (
-                hasattr(Dx, '__iter__')
-                and len(Dx) == 2
-                and all([
-                    rr is None or (np.isscalar(rr) and np.isfinite(rr))
-                    for rr in Dx
-                ])
-            )
-            if not c0:
-                msg = 'Arg Dx must be an iterable of 2 scalars!'
-                raise Exception(msg)
+    # mode
+    mode = ds._generic_check._check_var(
+        mode, 'mode',
+        types=str,
+        default='abs',
+    )
 
-    if Dx is None:
-        Dx = [knots.min(), knots.max()]
+    # res
+    res = _get_res(
+        coll=coll,
+        key=key,
+        res=res,
+        nd=nd,
+        mtype=mtype,
+    )
+
+    # ---------
+    # parameters
+
+    if nd == '1d':
+        lok = None
+
+    else:
 
-    # ------
+        # grid
+        grid = ds._generic_check._check_var(
+            grid, 'grid',
+            types=bool,
+            default=False,
+        )
+
+        # imshow
+        imshow = ds._generic_check._check_var(
+            imshow, 'imshow',
+            types=bool,
+            default=False,
+        )
+
+        lok = [False]
+        if grid is False and imshow is False:
+            if x0 is None and x1 is None:
+                lok.append(True)
+
+    # --------
     # store
 
     store = ds._generic_check._check_var(
         store, 'store',
         types=bool,
         default=False,
+        allowed=lok,
     )
 
-    return key, mode, Dx, knots, store
+    return (
+        key, nd, mtype,
+        mode, res, submesh,
+        grid, imshow, store,
+    )
 
 
-def _sample_mesh_check_2d(
+def _check_1d(
     coll=None,
     key=None,
-    mtype=None,
-    res=None,
+    Dx=None,
     mode=None,
-    grid=None,
-    imshow=None,
-    R=None,
-    Z=None,
-    DR=None,
-    DZ=None,
-    store=None,
 ):
 
-    # -----------
-    # Parameters
+    wm = coll._which_mesh
 
-    # for polar mesh => sample underlying mesh
-    if mtype == 'polar':
-        key = coll.dobj[coll._which_mesh][key]['submesh']
-        mtype = coll.dobj[coll._which_mesh][key]['type']
+    # -------------
+    # knots
 
-    if np.isscalar(res):
-        res = [res, res]
-    c0 = (
-        isinstance(res, list)
-        and len(res) == 2
-        and all([np.isscalar(rr) and rr > 0 for rr in res])
-    )
-    if not c0:
-        msg = f"Arg res must be a list of 2 positive floats!\nProvided: {res}"
+    kknots = coll.dobj[wm][key]['knots'][0]
+    knots = coll.ddata[kknots]['data']
+
+    # custom DR or DZ for mode='abs' only
+    Dx = _Dx(Dx)
+
+    if Dx is not None and mode != 'abs':
+        msg = "Custom Dx can only be provided with mode = 'abs'!"
         raise Exception(msg)
 
-    # grid
-    grid = ds._generic_check._check_var(
-        grid, 'grid',
-        types=bool,
-        default=False,
-    )
+    return knots, Dx
 
-    # imshow
-    imshow = ds._generic_check._check_var(
-        imshow, 'imshow',
-        types=bool,
-        default=False,
-    )
+
+def _check_2d(
+    coll=None,
+    key=None,
+    x0=None,
+    x1=None,
+    Dx0=None,
+    Dx1=None,
+    mode=None,
+    mtype=None,
+):
+
+    wm = coll._which_mesh
+
+    # -----------
+    # Parameters
 
     # R, Z
-    if R is None and Z is None:
+    if x0 is None and x1 is None:
         pass
-    elif R is None and np.isscalar(Z):
+    elif x0 is None and np.isscalar(x1):
         pass
-    elif Z is None and np.isscalar(R):
+    elif x1 is None and np.isscalar(x0):
         pass
     else:
         msg = (
-            "For mesh discretisation, (R, Z) can be either:\n"
+            "For mesh discretisation, (x0, x1) can be either:\n"
             "\t- (None, None): will be created\n"
             "\t- (scalar, None): A vertical line will be created\n"
             "\t- (None, scalar): A horizontal line will be created\n"
         )
         raise Exception(msg)
 
     # -------------
-    # R, Z
+    # x0, x1
 
+    k0, k1 = coll.dobj[wm][key]['knots']
     if mtype == 'rect':
-        kR, kZ = coll.dobj[coll._which_mesh][key]['knots']
-        Rk = coll.ddata[kR]['data']
-        Zk = coll.ddata[kZ]['data']
+        knots0 = coll.ddata[k0]['data']
+        knots1 = coll.ddata[k1]['data']
 
         # custom R xor Z for vertical / horizontal lines only
-        if R is None and Z is not None:
-            R = Rk
-        if Z is None and R is not None:
-            Z = Zk
-    else:
-        kknots = coll.dobj[coll._which_mesh][key]['knots']
-        Rk = coll.ddata[kknots[0]]['data']
-        Zk = coll.ddata[kknots[1]]['data']
+        if x0 is None and x1 is not None:
+            x0 = knots0
+        if x1 is None and x0 is not None:
+            x1 = knots1
+
+    else:
+        knots0 = coll.ddata[k0]['data']
+        knots1 = coll.ddata[k1]['data']
 
     # custom DR or DZ for mode='abs' only
-    if DR is not None or DZ is not None:
-        if mode != 'abs':
-            msg = "Custom DR or DZ can only be provided with mode = 'abs'!"
-            raise Exception(msg)
+    Dx0 = _DRZ(Dx=Dx0, size=None, Dx_name='Dx0')
+    Dx1 = _DRZ(
+        Dx=Dx1,
+        size=len(Dx0) if Dx0 is not None else None,
+        Dx_name='Dx1',
+    )
 
-        for DD, DN in [(DR, 'DR'), (DZ, 'DZ')]:
-            if DD is not None:
-                c0 = (
-                    hasattr(DD, '__iter__')
-                    and len(DD) == 2
-                    and all([
-                        rr is None or (np.isscalar(rr) and np.isfinite(rr))
-                        for rr in DD
-                    ])
-                )
-                if not c0:
-                    msg = f'Arg {DN} must be an iterable of 2 scalars!'
-                    raise Exception(msg)
-
-    if DR is None:
-        DR = [Rk.min(), Rk.max()]
-    if DZ is None:
-        DZ = [Zk.min(), Zk.max()]
+    if (Dx0 is not None or Dx1 is not None) and mode != 'abs':
+        msg = (
+            "Custom Dx0 or Dx1 can only be provided with mode = 'abs'!\n"
+            f"\t- mode: {mode}\n"
+            f"\t- Dx0: {Dx0}\n"
+            f"\t- Dx1: {Dx1}\n"
+        )
+        raise Exception(msg)
 
-    # ------
-    # store
+    return knots0, knots1, x0, x1, Dx0, Dx1
 
-    lok = [False]
-    if grid is False and imshow is False:
-        if R is None and Z is None:
-            lok.append(True)
 
-    store = ds._generic_check._check_var(
-        store, 'store',
-        types=bool,
-        default=False,
-        allowed=lok,
+# #############
+# check Dx
+# #############
+
+
+def _Dx(Dx=None):
+
+    if Dx is None:
+        return None
+
+    c0 = (
+        hasattr(Dx, '__iter__')
+        and len(Dx) == 2
+        and all([
+            rr is None or (np.isscalar(rr) and not np.isnan(rr))
+            for rr in Dx
+        ])
     )
+    if not c0:
+        msg = 'Arg Dx must be an iterable of 2 scalars!'
+        raise Exception(msg)
+
+    for ii in range(2):
+        if Dx[ii] is None:
+            Dx[ii] = -np.inf if ii == 00 else np.inf
+
+    return Dx
 
-    return key, res, mode, grid, imshow, R, Z, DR, DZ, Rk, Zk, store
 
+def _DRZ(Dx=None, size=None, Dx_name=None):
+
+    if Dx is None:
+        return None
+
+    if None not in Dx and np.all(np.isfinite(Dx)) and np.size(Dx) > 2:
+        Dx = np.atleast_1d(Dx).ravel()
+        if size is not None and Dx.size != size:
+            msg = (
+                f"Arg {Dx_name} has wrong size!\n"
+                f"\t- expected: {size}\n"
+                f"\t- Provided: {Dx.size}"
+            )
+            raise Exception(msg)
+
+    else:
+        Dx = _Dx(Dx)
+
+    return Dx
 
-# ###################################################################
-# ###################################################################
+
+# ################################################################
+# ################################################################
 #                       utility
-# ###################################################################
+# ################################################################
 
 
-def _get_sample_mesh_res(
+def _get_res(
     coll=None,
-    keym=None,
+    key=None,
+    res=None,
     nd=None,
     mtype=None,
 ):
 
     wm = coll._which_mesh
     if nd == '1d':
-        kknots = coll.dobj[wm][keym]['knots'][0]
-        res = np.min(np.diff(coll.ddata[kknots]['data']))
 
-    elif mtype == 'rect':
-        kR, kZ = coll.dobj[wm][keym]['knots']
-        res = min(
-            np.min(np.diff(coll.ddata[kR]['data'])),
-            np.min(np.diff(coll.ddata[kZ]['data'])),
-        )
-    elif mtype == 'tri':
-        res = 0.02
-
-    elif mtype == 'polar':
-        keyr2d = coll.dobj[wm][keym]['radius2d']
-        keybs0 = coll.ddata[keyr2d]['bsplines']
-        keym0 = coll.dobj['bsplines'][keybs0]['mesh']
-        mtype0 = coll.dobj[wm][keym0]['type']
-        res = _get_sample_mesh_res(coll=coll, keym=keym0, mtype=mtype0)
+        if res is None:
+            kknots = coll.dobj[wm][key]['knots'][0]
+            res = np.min(np.diff(coll.ddata[kknots]['data']))
+
+        if not (np.isscalar(res) and res > 0.):
+            msg = (
+                f"Arg res must be a positive float!\n"
+                "Provided: {res}"
+            )
+            raise Exception(msg)
 
     else:
-        raise Exception(f"Wrong mtype for sampling: {mtype}")
+
+        if res is None:
+            if mtype == 'rect':
+                kR, kZ = coll.dobj[wm][key]['knots']
+                res = min(
+                    np.min(np.diff(coll.ddata[kR]['data'])),
+                    np.min(np.diff(coll.ddata[kZ]['data'])),
+                )
+
+            elif mtype == 'tri':
+                res = 0.02
+
+        # check len() = 2
+        if np.isscalar(res):
+            res = [res, res]
+
+        c0 = (
+            isinstance(res, list)
+            and len(res) == 2
+            and all([np.isscalar(rr) and rr > 0 for rr in res])
+        )
+        if not c0:
+            msg = (
+                f"Arg res must be a list of 2 positive floats!\n"
+                "Provided: {res}"
+            )
+            raise Exception(msg)
 
     return res
 
 
-# ###################################################################
-# ###################################################################
+# ##################################################################
+# ##################################################################
 #                       sample 1d
-# ###################################################################
+# ##################################################################
+
+
+def _sample_1d(
+    res=None,
+    mode=None,
+    knots=None,
+    Dx=None,
+):
+
+    kmin, kmax = knots.min(), knots.max()
+
+    if mode == 'abs':
+        nx = int(np.ceil((kmax - kmin) / res))
+        xx = np.linspace(kmin, kmax, nx)
+
+    else:
+        nx = int(np.ceil(1./res))
+        kx = np.linspace(0, 1, nx, endpoint=False)[None, :]
+        xx = np.concatenate((
+            (knots[:-1, None] + kx*np.diff(knots)[:, None]).ravel(),
+            knots[-1:],
+        ))
+
+    # Dx
+    if Dx is not None:
+        ind = (xx >= Dx[0]) & (xx < Dx[1])
+        xx = xx[ind]
+
+    return xx
 
 
-def sample_mesh_1d(
+# ##################################################################
+# ##################################################################
+#                       sample 2d
+# ##################################################################
+
+
+def _sample_2d(
     coll=None,
     key=None,
     res=None,
     mode=None,
-    Dx=None,
-    knots=None,
-    # store
-    store=None,
-    kx0=None,
+    knots0=None,
+    knots1=None,
+    x0=None,
+    x1=None,
+    Dx0=None,
+    Dx1=None,
+    # options
+    grid=None,
+    imshow=None,
+    in_mesh=None,
 ):
 
     # --------
-    # sample
+    # compute
 
-    x0 = _sample_mesh_1d(
-        res=res,
-        mode=mode,
-        Dx=Dx,
-        knots=knots,
-    )
+    min0, max0 = knots0.min(), knots0.max()
+    min1, max1 = knots1.min(), knots1.max()
+
+    if mode == 'abs':
+        if x0 is None:
+            n0 = int(np.ceil((max0 - min0) / res[0]))
+            x0 = np.linspace(min0, max0, n0)
+        if x1 is None:
+            n1 = int(np.ceil((max1 - min1) / res[1]))
+            x1 = np.linspace(min1, max1, n1)
+    else:
+        if x0 is None:
+            n0 = int(np.ceil(1./res[0]))
+            kx0 = np.linspace(0, 1, n0, endpoint=False)[None, :]
+            x0 = np.concatenate((
+                (knots0[:-1, None] + kx0*np.diff(knots0)[:, None]).ravel(),
+                knots0[-1:],
+            ))
+        if x1 is None:
+            n1 = int(np.ceil(1./res[1]))
+            kx1 = np.linspace(0, 1, n1, endpoint=False)[None, :]
+            x1 = np.concatenate((
+                (knots1[:-1, None] + kx1*np.diff(knots1)[:, None]).ravel(),
+                knots1[-1:],
+            ))
+
+    if np.isscalar(x0):
+        x0 = np.full(x1.shape, x0)
+    if np.isscalar(x1):
+        x1 = np.full(x0.shape, x1)
+
+    # -----------
+    # prepare ind
+
+    # x0, x1
+    if grid or in_mesh or Dx0 is not None:
+        x02 = np.repeat(x0[:, None], x1.size, axis=1)
+        x12 = np.repeat(x1[None, :], x0.size, axis=0)
+
+        if in_mesh or Dx0 is not None:
+            x0f = x02.ravel()
+            x1f = x12.ravel()
+            sh = x02.shape
+
+    # ind
+    if Dx0 is not None or in_mesh is True:
+        ind = np.ones((x0.size, x1.size), dtype=bool)
+    else:
+        ind = None
+
+    # ---------
+    # Dx0, Dx1
+
+    if Dx0 is not None and len(Dx0) == 2:
+        ind = ind & (
+            (x02 >= Dx0[0]) & (x02 < Dx0[1])
+            & (x12 >= Dx1[0]) & (x12 < Dx1[1])
+        )
+
+    # -----------
+    # indices
+
+    # mesh outline
+    if in_mesh is True:
+        dout = coll.get_mesh_outline(key=key)
+        pa = path.Path(np.array([dout['x0']['data'], dout['x1']['data']]).T)
+        ind = ind & pa.contains_points(np.array([x0f, x1f]).T).reshape(sh)
+
+    # Dx0, Dx1
+    if Dx0 is not None and len(Dx0) > 2:
+        pa = path.Path(np.array([Dx0, Dx1]).T)
+        ind = ind & pa.contains_points(np.array([x0f, x1f]).T).reshape(sh)
+
+    # ------------
+    # grid
+
+    if grid is True:
+        x0, x1 = x02, x12
+
+    # ----------
+    # imshow
+
+    if imshow is True:
+        if ind is not None:
+            ind = ind.T
+        if grid is True:
+            x0 = x0.T
+            x1 = x1.T
+
+    return x0, x1, ind
+
+
+# ##################################################################
+# ##################################################################
+#                       store
+# ##################################################################
+
+
+def _store_1d(
+    coll=None,
+    key=None,
+    x0=None,
+    # store
+    store=None,
+    kx0=None,
+):
 
     # -----------
     # check key
 
     if store is True:
         lout = list(coll.ddata.keys())
     else:
@@ -459,76 +672,26 @@
 
     if store:
         ddata['x0']['ref'] = kr
 
     return dref, ddata
 
 
-def _sample_mesh_1d(
-    res=None,
-    mode=None,
-    Dx=None,
-    knots=None,
-):
-
-    if mode == 'abs':
-        nx = int(np.ceil((Dx[1] - Dx[0]) / res))
-        xx = np.linspace(Dx[0], Dx[1], nx)
-
-    else:
-        nx = int(np.ceil(1./res))
-        kx = np.linspace(0, 1, nx, endpoint=False)[None, :]
-        xx = np.concatenate((
-            (knots[:-1, None] + kx*np.diff(knots)[:, None]).ravel(),
-            knots[-1:],
-        ))
-
-    return xx
-
-
-# ###################################################################
-# ###################################################################
-#                       sample 2d
-# ###################################################################
-
-
-def sample_mesh_2d(
+def _store_2d(
     coll=None,
     key=None,
-    res=None,
-    mode=None,
     x0=None,
     x1=None,
-    Dx0=None,
-    Dx1=None,
-    x0k=None,
-    x1k=None,
-    grid=None,
-    imshow=None,
+    ind=None,
     # store
     store=None,
     kx0=None,
     kx1=None,
 ):
 
-    # --------
-    # sample
-
-    x0, x1 = _sample_mesh_2d(
-        res=res,
-        mode=mode,
-        x0=x0,
-        x1=x1,
-        Dx0=Dx0,
-        Dx1=Dx1,
-        x0k=x0k,
-        x1k=x1k,
-        grid=grid,
-        imshow=imshow,
-    )
 
     # -----------
     # check key
 
     if store is True:
         lout = list(coll.ddata.keys())
     else:
@@ -577,85 +740,29 @@
             'dim': coll.ddata[kk1]['dim'],
             'quant': coll.ddata[kk1]['quant'],
             'name': coll.ddata[kk1]['name'],
             'units': coll.ddata[kk1]['units'],
         },
     }
 
+    if ind is not None:
+        ddata['ind'] = {
+            'key': f'{key}_ind_temp',
+            'data': ind,
+        }
+
     if store is True:
         ddata['x0']['ref'] = k0r
         ddata['x1']['ref'] = k1r
+        if ind is not None:
+            ddata['ind']['ref'] = (k0r, k1r)
 
     return dref, ddata
 
 
-def _sample_mesh_2d(
-    res=None,
-    mode=None,
-    x0=None,
-    x1=None,
-    Dx0=None,
-    Dx1=None,
-    x0k=None,
-    x1k=None,
-    grid=None,
-    imshow=None,
-):
-
-    # compute
-    if mode == 'abs':
-        if x0 is None:
-            n0 = int(np.ceil((Dx0[1] - Dx0[0]) / res[0]))
-            x0 = np.linspace(Dx0[0], Dx0[1], n0)
-        if x1 is None:
-            n1 = int(np.ceil((Dx1[1] - Dx1[0]) / res[1]))
-            x1 = np.linspace(Dx1[0], Dx1[1], n1)
-    else:
-        if x0 is None:
-            n0 = int(np.ceil(1./res[0]))
-            kx0 = np.linspace(0, 1, n0, endpoint=False)[None, :]
-            x0 = np.concatenate((
-                (x0k[:-1, None] + kx0*np.diff(x0k)[:, None]).ravel(),
-                x0k[-1:],
-            ))
-        if x1 is None:
-            n1 = int(np.ceil(1./res[1]))
-            kx1 = np.linspace(0, 1, n1, endpoint=False)[None, :]
-            x1 = np.concatenate((
-                (x1k[:-1, None] + kx1*np.diff(x1k)[:, None]).ravel(),
-                x1k[-1:],
-            ))
-
-    if np.isscalar(x0):
-        x0 = np.full(x1.shape, x0)
-    if np.isscalar(x1):
-        x1 = np.full(x0.shape, x1)
-
-    # ------------
-    # grid
-
-    if grid is True:
-        n1 = x1.size
-        n0 = x0.size
-        if imshow is True:
-            x0 = np.tile(x0, (n1, 1))
-            x1 = np.repeat(x1[:, None], n0, axis=1)
-        else:
-            x0 = np.repeat(x0[:, None], n1, axis=1)
-            x1 = np.tile(x1, (n0, 1))
-
-    return x0, x1
-
-
-# ###################################################################
-# ###################################################################
-#                       store
-# ###################################################################
-
-
 def _store(coll=None, dref=None, ddata=None):
 
     # dref
     for k0, v0 in dref.items():
         coll.add_ref(key=k0, **v0)
 
     # ddata
```

### Comparing `bsplines2d-0.0.2/bsplines2d/_class01_select.py` & `bsplines2d-0.0.3/bsplines2d/_class01_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,14 @@
 ):
     """ ind is a tuple for rect """
 
     # ------------
     # check inputs
 
     wm = coll._which_mesh
-    nd = coll.dobj[wm][key]['nd']
     mtype = coll.dobj[wm][key]['type']
 
     (
         elements, returnas,
         return_ind_as, return_neighbours,
     ) = _generic_mesh._select_check(
         elements=elements,
@@ -272,16 +271,14 @@
     # ------------
     # prepare
 
     if mtype in ['rect', 'tri']:
         kR, kZ = coll.dobj[wm][key][elements]
         R = coll.ddata[kR]['data']
         Z = coll.ddata[kZ]['data']
-        nR = R.size
-        nZ = Z.size
     else:
         kr = coll.dobj[wm][key][elements][0]
         rad = coll.ddata[kr]['data']
 
     # ------------
     # non-trivial case
```

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_BSplines2D.py` & `bsplines2d-0.0.3/bsplines2d/_class02_BSplines2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_bsplines_1d.py` & `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_bsplines_operators_1d.py` & `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_bsplines_operators_rect.py` & `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_operators_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_bsplines_polar.py` & `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_polar.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_bsplines_rect.py` & `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_bsplines_tri.py` & `bsplines2d-0.0.3/bsplines2d/_class02_bsplines_tri.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_checks.py` & `bsplines2d-0.0.3/bsplines2d/_class02_checks.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_compute.py` & `bsplines2d-0.0.3/bsplines2d/_class02_compute.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_contours.py` & `bsplines2d-0.0.3/bsplines2d/_class02_contours.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # Built-in
 import itertools as itt
 import warnings
 
 
 # Common
 import numpy as np
-from scipy.spatial import ConvexHull
-from matplotlib.path import Path
 from contourpy import contour_generator
 import datastock as ds
 
 
 # specific
 
 
@@ -67,29 +65,29 @@
 
     dsamp = coll.get_sample_mesh(
         key=keym0,
         res=res,
         grid=True,
         store=False,
     )
-    
-    # temporary addition of sample 
+
+    # temporary addition of sample
     if ref_com is not None:
-        
+
         # ref
         lkr_temp = []
         for ii, ss in enumerate(dsamp['x0']['data'].shape):
             kri = f'{key}_refsamptemp{ii}'
             lkr_temp.append(kri)
             coll.add_ref(key=kri, size=ss)
-            
+
         # data
         lkd_temp = [f'{key}_samptemp0', f'{key}_samptemp1']
         coll.add_data(key=lkd_temp[0], data=dsamp['x0']['data'], ref=lkr_temp)
-        coll.add_data(key=lkd_temp[1], data=dsamp['x1']['data'], ref=lkr_temp)    
+        coll.add_data(key=lkd_temp[1], data=dsamp['x1']['data'], ref=lkr_temp)
         x0, x1 = lkd_temp
     else:
         x0 = dsamp['x0']['data']
         x1 = dsamp['x1']['data']
 
     # interpolate
     dinterp = coll.interpolate(
@@ -105,20 +103,20 @@
 
     # remove temporary data
     if ref_com is not None:
         coll.remove_data(x0, propagate=False)
         coll.remove_data(x1, propagate=False)
         for rr in lkr_temp:
             coll.remove_ref(rr, propagate=False)
-            
+
         axis = [
-            dinterp['ref'].index(lkr_temp[0]), 
+            dinterp['ref'].index(lkr_temp[0]),
             dinterp['ref'].index(lkr_temp[1]),
         ]
-        
+
     else:
         # axis
         axis = [
             ii for ii, rr in enumerate(dinterp['ref'])
             if rr is None
         ]
 
@@ -380,62 +378,20 @@
             # z_interp=<ZInterp.Linear: 1>,
             thread_count=0,
         )
 
         # loop on levels
         for jj in range(len(levels)):
 
-            # compute concatenated contour
-            no_cont = False
-            cj = contgen.lines(levels[jj])
-
-            c0 = (
-                isinstance(cj, list)
-                and all([
-                    isinstance(cjj, np.ndarray)
-                    and cjj.ndim == 2
-                    and cjj.shape[1] == 2
-                    for cjj in cj
-                ])
+            # get contour
+            no_cont, cj = _get_contours_lvls(
+                contgen=contgen,
+                level=levels[jj],
+                largest=largest,
             )
-            if not c0:
-                msg = f"Wrong output from contourpy!\n{cj}"
-                raise Exception(msg)
-
-            # if one or several contours exist
-            if len(cj) > 0:
-                cj = [
-                    cc[np.all(np.isfinite(cc), axis=1), :]
-                    for cc in cj
-                    if np.sum(np.all(np.isfinite(cc), axis=1)) >= 3
-                ]
-
-                if len(cj) == 0:
-                    no_cont = True
-                elif len(cj) == 1:
-                    cj = cj[0]
-                elif len(cj) > 1:
-                    if largest:
-                        nj = [
-                            0.5*np.abs(np.sum(
-                                (cc[1:, 0] + cc[:-1, 0])
-                                *(cc[1:, 1] - cc[:-1, 1])
-                            ))
-                            for cc in cj
-                        ]
-                        cj = cj[np.argmax(nj)]
-                    else:
-                        ij = np.cumsum([cc.shape[0] for cc in cj])
-                        cj = np.concatenate(cj, axis=0)
-                        cj = np.insert(cj, ij, np.nan, axis=0)
-
-                elif np.sum(np.all(~np.isnan(cj), axis=1)) < 3:
-                    no_cont = True
-            else:
-                no_cont = True
 
             # if contour was found
             if no_cont is False:
 
                 # maxnpts
                 if cj.shape[0] > maxnpts:
                     maxnpts = cj.shape[0]
@@ -464,14 +420,71 @@
         warnings.warn(msg)
     else:
         print(msg)
 
     return cont0, cont1
 
 
+def _get_contours_lvls(
+    contgen=None,
+    level=None,
+    largest=None,
+):
+    # compute concatenated contour
+    no_cont = False
+    cj = contgen.lines(level)
+
+    c0 = (
+        isinstance(cj, list)
+        and all([
+            isinstance(cjj, np.ndarray)
+            and cjj.ndim == 2
+            and cjj.shape[1] == 2
+            for cjj in cj
+        ])
+    )
+    if not c0:
+        msg = f"Wrong output from contourpy!\n{cj}"
+        raise Exception(msg)
+
+    # if one or several contours exist
+    if len(cj) > 0:
+        cj = [
+            cc[np.all(np.isfinite(cc), axis=1), :]
+            for cc in cj
+            if np.sum(np.all(np.isfinite(cc), axis=1)) >= 3
+        ]
+
+        if len(cj) == 0:
+            no_cont = True
+        elif len(cj) == 1:
+            cj = cj[0]
+        elif len(cj) > 1:
+            if largest:
+                nj = [
+                    0.5*np.abs(np.sum(
+                        (cc[1:, 0] + cc[:-1, 0])
+                        *(cc[1:, 1] - cc[:-1, 1])
+                    ))
+                    for cc in cj
+                ]
+                cj = cj[np.argmax(nj)]
+            else:
+                ij = np.cumsum([cc.shape[0] for cc in cj])
+                cj = np.concatenate(cj, axis=0)
+                cj = np.insert(cj, ij, np.nan, axis=0)
+
+        elif np.sum(np.all(~np.isnan(cj), axis=1)) < 3:
+            no_cont = True
+    else:
+        no_cont = True
+
+    return no_cont, cj
+
+
 def _compute_check(
     xx0=None,
     xx1=None,
     val=None,
     axis=None,
     levels=None,
     npts=None,
```

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_interpolate.py` & `bsplines2d-0.0.3/bsplines2d/_class02_interpolate.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,19 @@
 
 # Built-in
 import itertools as itt
 import warnings
 
 # Common
 import numpy as np
-from scipy.spatial import ConvexHull
-from matplotlib.path import Path
-from contourpy import contour_generator
 import datastock as ds
 
 
 # tofu
 # from . import _class02_checks as _checks
-from . import _class02_bsplines_rect
-from . import _class02_bsplines_tri
-from . import _class02_bsplines_polar
-from . import _class02_bsplines_1d
 from . import _utils_bsplines
 
 
 # ################################################################
 # ################################################################
 #                                       Main
 # ################################################################
```

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_interpolate_all.py` & `bsplines2d-0.0.3/bsplines2d/_class02_interpolate_all.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_operators.py` & `bsplines2d-0.0.3/bsplines2d/_class02_operators.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_plot.py` & `bsplines2d-0.0.3/bsplines2d/_class02_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_plot_as_profile2d.py` & `bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class02_plot_as_profile2d_compare.py` & `bsplines2d-0.0.3/bsplines2d/_class02_plot_as_profile2d_compare.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class03_Bins.py` & `bsplines2d-0.0.3/bsplines2d/_class03_Bins.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class03_binning.py` & `bsplines2d-0.0.3/bsplines2d/_class03_binning.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class03_checks.py` & `bsplines2d-0.0.3/bsplines2d/_class03_checks.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_class11_plot.py` & `bsplines2d-0.0.3/bsplines2d/_class11_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_generic_check.py` & `bsplines2d-0.0.3/bsplines2d/_generic_check.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_generic_mesh.py` & `bsplines2d-0.0.3/bsplines2d/_generic_mesh.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_utils_bsplines.py` & `bsplines2d-0.0.3/bsplines2d/_utils_bsplines.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/_utils_bsplines_operators.py` & `bsplines2d-0.0.3/bsplines2d/_utils_bsplines_operators.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/tests/test_01_Mesh2D.py` & `bsplines2d-0.0.3/bsplines2d/tests/test_01_Mesh2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/tests/test_02_BSplines2D.py` & `bsplines2d-0.0.3/bsplines2d/tests/test_02_BSplines2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/tests/test_data/WEST_Poly.npz` & `bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_Poly.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/tests/test_data/WEST_trimesh.npz` & `bsplines2d-0.0.3/bsplines2d/tests/test_data/WEST_trimesh.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/tests/test_data/trimesh_quad.npz` & `bsplines2d-0.0.3/bsplines2d/tests/test_data/trimesh_quad.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.2/bsplines2d/tests/test_input.py` & `bsplines2d-0.0.3/bsplines2d/tests/test_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,25 +396,41 @@
 
 
 def _sample_mesh(bsplines, nd=None, kind=None):
     lkm = _get_mesh(bsplines, nd=nd, kind=kind)
 
     lres = [0.1, 0.3]
     lmode = ['abs', 'rel']
+    lin_mesh = [False, True]
     limshow = [False, True]
 
+    Dx0, Dx1 = None, None
     for km in lkm:
+        for ii, comb in enumerate(itt.product(lres, lmode, lin_mesh, limshow)):
+
+            if nd == '2d':
+                if comb[1] == 'abs' and ii % 3 == 0:
+                    Dx0 = np.r_[2., 3., 2.5]
+                    Dx1 = np.r_[-1, -1, 1]
+                elif comb[1] == 'abs' and ii % 3 == 1:
+                    Dx0 = [None, 2.5]
+                    Dx1 = [-0.5, None]
+                else:
+                    Dx0 = None
+                    Dx1 = None
 
-        for comb in itt.product(lres, lmode, limshow):
             out = bsplines.get_sample_mesh(
                 key=km,
                 res=comb[0],
                 mode=comb[1],
                 grid=None,
-                imshow=comb[2]
+                Dx0=Dx0,
+                Dx1=Dx1,
+                in_mesh=comb[2] and kind != 'tri',
+                imshow=comb[3]
             )
 
 
 def _plot_mesh(bsplines, nd=None, kind=None):
     lkm = _get_mesh(bsplines, nd=nd, kind=kind)
 
     lk = [None, 2, [2, 3]]
```

### Comparing `bsplines2d-0.0.2/bsplines2d.egg-info/PKG-INFO` & `bsplines2d-0.0.3/bsplines2d.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsplines2d
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library for generic multidimensional bsplines on various meshes, using datastock
 Home-page: https://github.com/ToFuProject/bsplines2d
 Author: Didier VEZINET
 Author-email: didier.vezinet@gmail.com
 License: MIT
 Keywords: bsplines data analysis modelling mesh plot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bsplines2d-0.0.2/bsplines2d.egg-info/SOURCES.txt` & `bsplines2d-0.0.3/bsplines2d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 bsplines2d/__init__.py
 bsplines2d/_class01_Mesh2D.py
 bsplines2d/_class01_checks_1d.py
 bsplines2d/_class01_checks_2d_polar.py
 bsplines2d/_class01_checks_2d_rect.py
 bsplines2d/_class01_checks_2d_tri.py
+bsplines2d/_class01_outline.py
 bsplines2d/_class01_plot.py
 bsplines2d/_class01_rect_cropping.py
 bsplines2d/_class01_sample.py
 bsplines2d/_class01_select.py
 bsplines2d/_class02_BSplines2D.py
 bsplines2d/_class02_bsplines_1d.py
 bsplines2d/_class02_bsplines_operators_1d.py
```

### Comparing `bsplines2d-0.0.2/setup.py` & `bsplines2d-0.0.3/setup.py`

 * *Files identical despite different names*

