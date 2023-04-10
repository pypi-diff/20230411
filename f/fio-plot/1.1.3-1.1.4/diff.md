# Comparing `tmp/fio-plot-1.1.3.tar.gz` & `tmp/fio-plot-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio-plot-1.1.3.tar", last modified: Fri Mar 31 18:33:34 2023, max compression
+gzip compressed data, was "fio-plot-1.1.4.tar", last modified: Mon Apr 10 23:25:48 2023, max compression
```

## Comparing `fio-plot-1.1.3.tar` & `fio-plot-1.1.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.576971 fio-plot-1.1.3/
--rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.3/CHANGELOG.md
--rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.3/LICENSE
--rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.3/MANIFEST.in
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-03-31 18:33:34.574827 fio-plot-1.1.3/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-03-27 19:45:08.000000 fio-plot-1.1.3/README.md
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.500741 fio-plot-1.1.3/bench_fio/
--rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.3/bench_fio/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.3/bench_fio/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.510285 fio-plot-1.1.3/bench_fio/benchlib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.3/bench_fio/benchlib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    10583 2023-03-31 18:30:11.000000 fio-plot-1.1.3/bench_fio/benchlib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-03-31 18:30:11.000000 fio-plot-1.1.3/bench_fio/benchlib/checks.py
--rw-r--r--   0 nan03      (501) staff       (20)     2916 2023-03-27 19:45:08.000000 fio-plot-1.1.3/bench_fio/benchlib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     3295 2023-03-27 19:45:08.000000 fio-plot-1.1.3/bench_fio/benchlib/display.py
--rw-r--r--   0 nan03      (501) staff       (20)     2338 2023-03-27 19:45:08.000000 fio-plot-1.1.3/bench_fio/benchlib/generatefio.py
--rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.3/bench_fio/benchlib/network.py
--rw-r--r--   0 nan03      (501) staff       (20)     1697 2023-03-31 18:30:11.000000 fio-plot-1.1.3/bench_fio/benchlib/parseini.py
--rw-r--r--   0 nan03      (501) staff       (20)     6008 2023-03-31 18:30:11.000000 fio-plot-1.1.3/bench_fio/benchlib/runfio.py
--rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-03-31 18:30:11.000000 fio-plot-1.1.3/bench_fio/benchlib/supporting.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.511964 fio-plot-1.1.3/bench_fio/scripts/
--rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.3/bench_fio/scripts/bench-fio.sh
--rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.3/bench_fio/scripts/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.512899 fio-plot-1.1.3/bench_fio/templates/
--rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.3/bench_fio/templates/precondition.fio
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.515414 fio-plot-1.1.3/bin/
--rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.3/bin/bench-fio
--rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.3/bin/fio-plot
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.530800 fio-plot-1.1.3/docs/
--rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.3/docs/bench_fio_call_graph.png
--rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.3/docs/fio_plot_call_graph.png
--rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.3/docs/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.538724 fio-plot-1.1.3/fio_plot/
--rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.3/fio_plot/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.570806 fio-plot-1.1.3/fio_plot/fiolib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.3/fio_plot/fiolib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    11039 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     7426 2023-03-30 00:23:17.000000 fio-plot-1.1.3/fio_plot/fiolib/bar2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-01-30 18:56:59.000000 fio-plot-1.1.3/fio_plot/fiolib/bar3d.py
--rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-03-31 18:30:11.000000 fio-plot-1.1.3/fio_plot/fiolib/barhistogram.py
--rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/dataimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/dataimport_support.py
--rw-r--r--   0 nan03      (501) staff       (20)      724 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.3/fio_plot/fiolib/flightchecks.py
--rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/getdata.py
--rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-03-27 20:04:44.000000 fio-plot-1.1.3/fio_plot/fiolib/graph2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6513 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/graph2dsupporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     2328 2023-01-31 12:57:49.000000 fio-plot-1.1.3/fio_plot/fiolib/iniparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/jsonimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     3265 2023-03-31 18:30:11.000000 fio-plot-1.1.3/fio_plot/fiolib/jsonparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     5348 2023-03-31 18:30:11.000000 fio-plot-1.1.3/fio_plot/fiolib/jsonparsing_support.py
--rw-r--r--   0 nan03      (501) staff       (20)    14738 2023-03-31 17:52:35.000000 fio-plot-1.1.3/fio_plot/fiolib/shared_chart.py
--rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-03-27 19:52:56.000000 fio-plot-1.1.3/fio_plot/fiolib/supporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     4021 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/table_support.py
--rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.3/fio_plot/fiolib/tables.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.542257 fio-plot-1.1.3/fio_plot.egg-info/
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-03-31 18:33:34.000000 fio-plot-1.1.3/fio_plot.egg-info/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-03-31 18:33:34.000000 fio-plot-1.1.3/fio_plot.egg-info/SOURCES.txt
--rw-r--r--   0 nan03      (501) staff       (20)        1 2023-03-31 18:33:34.000000 fio-plot-1.1.3/fio_plot.egg-info/dependency_links.txt
--rw-r--r--   0 nan03      (501) staff       (20)       70 2023-03-31 18:33:34.000000 fio-plot-1.1.3/fio_plot.egg-info/entry_points.txt
--rw-r--r--   0 nan03      (501) staff       (20)       40 2023-03-31 18:33:34.000000 fio-plot-1.1.3/fio_plot.egg-info/requires.txt
--rw-r--r--   0 nan03      (501) staff       (20)       19 2023-03-31 18:33:34.000000 fio-plot-1.1.3/fio_plot.egg-info/top_level.txt
--rw-r--r--   0 nan03      (501) staff       (20)       38 2023-03-31 18:33:34.577069 fio-plot-1.1.3/setup.cfg
--rw-r--r--   0 nan03      (501) staff       (20)      909 2023-03-31 18:30:11.000000 fio-plot-1.1.3/setup.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-03-31 18:33:34.573517 fio-plot-1.1.3/tests/
--rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.3/tests/bench_fio_test.py
--rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.3/tests/test_3d.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.944866 fio-plot-1.1.4/
+-rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.4/CHANGELOG.md
+-rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.4/LICENSE
+-rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.4/MANIFEST.in
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-10 23:25:48.943174 fio-plot-1.1.4/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-03-27 19:45:08.000000 fio-plot-1.1.4/README.md
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.881432 fio-plot-1.1.4/bench_fio/
+-rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.890225 fio-plot-1.1.4/bench_fio/benchlib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/benchlib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10583 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/checks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2916 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3295 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/display.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2338 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/generatefio.py
+-rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/network.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1697 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/parseini.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6051 2023-04-10 23:24:41.000000 fio-plot-1.1.4/bench_fio/benchlib/runfio.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/supporting.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.891713 fio-plot-1.1.4/bench_fio/scripts/
+-rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/scripts/bench-fio.sh
+-rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/scripts/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.892700 fio-plot-1.1.4/bench_fio/templates/
+-rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/templates/precondition.fio
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.894533 fio-plot-1.1.4/bin/
+-rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bin/bench-fio
+-rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bin/fio-plot
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.910301 fio-plot-1.1.4/docs/
+-rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.4/docs/bench_fio_call_graph.png
+-rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.4/docs/fio_plot_call_graph.png
+-rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.4/docs/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.917275 fio-plot-1.1.4/fio_plot/
+-rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.4/fio_plot/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.939329 fio-plot-1.1.4/fio_plot/fiolib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.4/fio_plot/fiolib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    11039 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     7426 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/bar2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-01-30 18:56:59.000000 fio-plot-1.1.4/fio_plot/fiolib/bar3d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/barhistogram.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/dataimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/dataimport_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)      724 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.4/fio_plot/fiolib/flightchecks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/getdata.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/graph2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6513 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/graph2dsupporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2328 2023-01-31 12:57:49.000000 fio-plot-1.1.4/fio_plot/fiolib/iniparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/jsonimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3265 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/jsonparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     5348 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/jsonparsing_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)    14738 2023-03-31 17:52:35.000000 fio-plot-1.1.4/fio_plot/fiolib/shared_chart.py
+-rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/supporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4021 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/table_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/tables.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.921508 fio-plot-1.1.4/fio_plot.egg-info/
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 nan03      (501) staff       (20)        1 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       70 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/entry_points.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       40 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/requires.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       19 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/top_level.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       38 2023-04-10 23:25:48.944967 fio-plot-1.1.4/setup.cfg
+-rw-r--r--   0 nan03      (501) staff       (20)      909 2023-04-10 23:24:41.000000 fio-plot-1.1.4/setup.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.941427 fio-plot-1.1.4/tests/
+-rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.4/tests/bench_fio_test.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.4/tests/test_3d.py
```

### Comparing `fio-plot-1.1.3/CHANGELOG.md` & `fio-plot-1.1.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/LICENSE` & `fio-plot-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/PKG-INFO` & `fio-plot-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.3
+Version: 1.1.4
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.3/README.md` & `fio-plot-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/__init__.py` & `fio-plot-1.1.4/bench_fio/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/argparsing.py` & `fio-plot-1.1.4/bench_fio/benchlib/argparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/checks.py` & `fio-plot-1.1.4/bench_fio/benchlib/checks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/defaultsettings.py` & `fio-plot-1.1.4/bench_fio/benchlib/defaultsettings.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/display.py` & `fio-plot-1.1.4/bench_fio/benchlib/display.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/generatefio.py` & `fio-plot-1.1.4/bench_fio/benchlib/generatefio.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/network.py` & `fio-plot-1.1.4/bench_fio/benchlib/network.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/parseini.py` & `fio-plot-1.1.4/bench_fio/benchlib/parseini.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/runfio.py` & `fio-plot-1.1.4/bench_fio/benchlib/runfio.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,18 @@
 
 
 def run_benchmarks(settings, benchmarks):
     # pprint.pprint(benchmarks)
     run = 0
     progress_benchmarks = ProgressBar(benchmarks) if not settings["quiet"] else benchmarks
     for benchmark in progress_benchmarks:
-        while run < settings["loops"]:
+        loops = 0
+        while loops < settings["loops"]:
             run += 1
+            loops += 1
             run_precondition_benchmark(settings, benchmark["target"], run)
             drop_caches()
             run_fio(settings, benchmark)
 
 
 def ProgressBar(iterObj):
     """https://stackoverflow.com/questions/3160699/python-progress-bar/49234284#49234284"""
```

### Comparing `fio-plot-1.1.3/bench_fio/benchlib/supporting.py` & `fio-plot-1.1.4/bench_fio/benchlib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/bench_fio/scripts/bench-fio.sh` & `fio-plot-1.1.4/bench_fio/scripts/bench-fio.sh`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/docs/bench_fio_call_graph.png` & `fio-plot-1.1.4/docs/bench_fio_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/docs/fio_plot_call_graph.png` & `fio-plot-1.1.4/docs/fio_plot_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/__init__.py` & `fio-plot-1.1.4/fio_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/argparsing.py` & `fio-plot-1.1.4/fio_plot/fiolib/argparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/bar2d.py` & `fio-plot-1.1.4/fio_plot/fiolib/bar2d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/bar3d.py` & `fio-plot-1.1.4/fio_plot/fiolib/bar3d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/barhistogram.py` & `fio-plot-1.1.4/fio_plot/fiolib/barhistogram.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/dataimport.py` & `fio-plot-1.1.4/fio_plot/fiolib/dataimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/dataimport_support.py` & `fio-plot-1.1.4/fio_plot/fiolib/dataimport_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/defaultsettings.py` & `fio-plot-1.1.4/fio_plot/fiolib/defaultsettings.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/flightchecks.py` & `fio-plot-1.1.4/fio_plot/fiolib/flightchecks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/getdata.py` & `fio-plot-1.1.4/fio_plot/fiolib/getdata.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/graph2d.py` & `fio-plot-1.1.4/fio_plot/fiolib/graph2d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/graph2dsupporting.py` & `fio-plot-1.1.4/fio_plot/fiolib/graph2dsupporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/iniparsing.py` & `fio-plot-1.1.4/fio_plot/fiolib/iniparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/jsonimport.py` & `fio-plot-1.1.4/fio_plot/fiolib/jsonimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/jsonparsing.py` & `fio-plot-1.1.4/fio_plot/fiolib/jsonparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/jsonparsing_support.py` & `fio-plot-1.1.4/fio_plot/fiolib/jsonparsing_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/shared_chart.py` & `fio-plot-1.1.4/fio_plot/fiolib/shared_chart.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/supporting.py` & `fio-plot-1.1.4/fio_plot/fiolib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/table_support.py` & `fio-plot-1.1.4/fio_plot/fiolib/table_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot/fiolib/tables.py` & `fio-plot-1.1.4/fio_plot/fiolib/tables.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/fio_plot.egg-info/PKG-INFO` & `fio-plot-1.1.4/fio_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.3
+Version: 1.1.4
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.3/fio_plot.egg-info/SOURCES.txt` & `fio-plot-1.1.4/fio_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/setup.py` & `fio-plot-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name="fio-plot",
-        version="1.1.3",
+        version="1.1.4",
         author="louwrentius",
         description="Create charts from FIO storage benchmark tool output",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/louwrentius/fio-plot/", 
         packages=setuptools.find_packages(),
         install_requires=['numpy','matplotlib','Pillow', 'pyan3', 'pyparsing'],
```

### Comparing `fio-plot-1.1.3/tests/bench_fio_test.py` & `fio-plot-1.1.4/tests/bench_fio_test.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.3/tests/test_3d.py` & `fio-plot-1.1.4/tests/test_3d.py`

 * *Files identical despite different names*

