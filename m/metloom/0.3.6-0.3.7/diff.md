# Comparing `tmp/metloom-0.3.6.tar.gz` & `tmp/metloom-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metloom-0.3.6.tar", last modified: Sun Apr  2 03:59:50 2023, max compression
+gzip compressed data, was "metloom-0.3.7.tar", last modified: Tue Apr 11 21:10:53 2023, max compression
```

## Comparing `metloom-0.3.6.tar` & `metloom-0.3.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.045932 metloom-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-02 03:59:39.000000 metloom-0.3.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-02 03:59:39.000000 metloom-0.3.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-02 03:59:39.000000 metloom-0.3.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-02 03:59:39.000000 metloom-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-02 03:59:39.000000 metloom-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-02 03:59:50.045932 metloom-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-02 03:59:39.000000 metloom-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.037932 metloom-0.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4999 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-02 03:59:39.000000 metloom-0.3.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.037932 metloom-0.3.6/metloom/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/dataframe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.041932 metloom-0.3.6/metloom/pointdata/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/pointdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/pointdata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/pointdata/cdec.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/pointdata/mesowest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/pointdata/snotel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/pointdata/snotel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/pointdata/usgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-02 03:59:39.000000 metloom-0.3.6/metloom/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.037932 metloom-0.3.6/metloom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-02 03:59:50.000000 metloom-0.3.6/metloom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-02 03:59:50.000000 metloom-0.3.6/metloom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 03:59:50.000000 metloom-0.3.6/metloom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-02 03:59:50.000000 metloom-0.3.6/metloom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 03:59:49.000000 metloom-0.3.6/metloom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-02 03:59:50.000000 metloom-0.3.6/metloom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-02 03:59:50.000000 metloom-0.3.6/metloom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-02 03:59:50.045932 metloom-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-02 03:59:39.000000 metloom-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.041932 metloom-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.045932 metloom-0.3.6/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 03:59:50.045932 metloom-0.3.6/tests/data/cdec_mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/cdec_mocks/raw_tny_locations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/cdec_mocks/raw_tny_notes.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/cdec_mocks/raw_tny_sensors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/daily_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/platoro_meta.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/station_search_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/testing.cpg
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/testing.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/testing.prj
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/testing.shp
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/testing.shx
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/triangle.cpg
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/triangle.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/triangle.prj
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/triangle.shp
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/data/triangle.shx
--rw-r--r--   0 runner    (1001) docker     (123)    22665 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/test_cdec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/test_dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/test_mesowest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/test_point_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/test_snotel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/test_usgs.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-02 03:59:39.000000 metloom-0.3.6/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.672174 metloom-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-11 21:10:44.000000 metloom-0.3.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-11 21:10:44.000000 metloom-0.3.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 21:10:44.000000 metloom-0.3.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-11 21:10:44.000000 metloom-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 21:10:44.000000 metloom-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-11 21:10:53.672174 metloom-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-11 21:10:44.000000 metloom-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.668174 metloom-0.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4999 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-11 21:10:44.000000 metloom-0.3.7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.668174 metloom-0.3.7/metloom/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/dataframe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.668174 metloom-0.3.7/metloom/pointdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/pointdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/pointdata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/pointdata/cdec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/pointdata/mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/pointdata/snotel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/pointdata/snotel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/pointdata/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-11 21:10:44.000000 metloom-0.3.7/metloom/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.668174 metloom-0.3.7/metloom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-11 21:10:53.000000 metloom-0.3.7/metloom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-11 21:10:53.000000 metloom-0.3.7/metloom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:10:53.000000 metloom-0.3.7/metloom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 21:10:53.000000 metloom-0.3.7/metloom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:10:53.000000 metloom-0.3.7/metloom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 21:10:53.000000 metloom-0.3.7/metloom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 21:10:53.000000 metloom-0.3.7/metloom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-11 21:10:53.672174 metloom-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-11 21:10:44.000000 metloom-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.672174 metloom-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.672174 metloom-0.3.7/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:10:53.672174 metloom-0.3.7/tests/data/cdec_mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/cdec_mocks/raw_tny_locations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/cdec_mocks/raw_tny_notes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/cdec_mocks/raw_tny_sensors.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/daily_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/platoro_meta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/station_search_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/testing.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/testing.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/testing.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/testing.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/testing.shx
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/triangle.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/triangle.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/triangle.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/triangle.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/data/triangle.shx
+-rw-r--r--   0 runner    (1001) docker     (123)    22665 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/test_cdec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/test_dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/test_mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/test_point_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/test_snotel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/test_usgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 21:10:44.000000 metloom-0.3.7/tests/test_variables.py
```

### Comparing `metloom-0.3.6/CONTRIBUTING.rst` & `metloom-0.3.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/HISTORY.rst` & `metloom-0.3.7/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/LICENSE` & `metloom-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/PKG-INFO` & `metloom-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.3.6
+Version: 0.3.7
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `metloom-0.3.6/README.rst` & `metloom-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/docs/Makefile` & `metloom-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/docs/conf.py` & `metloom-0.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/docs/installation.rst` & `metloom-0.3.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/docs/make.bat` & `metloom-0.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/docs/usage.rst` & `metloom-0.3.7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/cli.py` & `metloom-0.3.7/metloom/cli.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/dataframe_utils.py` & `metloom-0.3.7/metloom/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/pointdata/base.py` & `metloom-0.3.7/metloom/pointdata/base.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/pointdata/cdec.py` & `metloom-0.3.7/metloom/pointdata/cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/pointdata/mesowest.py` & `metloom-0.3.7/metloom/pointdata/mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/pointdata/snotel.py` & `metloom-0.3.7/metloom/pointdata/snotel.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                                   extra_params=None
                                   ):
         result_map = {}
         extra_params = extra_params or {}
         for variable in variables:
             # need to add extra_params for ground temp call, this may not be the
             # best logic
-            if 'GROUND' in variable.name:
+            if 'GROUND' in variable.name or 'SOIL' in variable.name:
                 params = extra_params[variable.name]
             else:
                 params = {}
             data = client.get_data(element_cd=variable.code, **params)
             if len(data) > 0:
                 result_map[variable] = data
             else:
@@ -242,29 +242,40 @@
         return timezone(timedelta(hours=tz_hours))
 
     def _add_fixed_params(self, variables):
         """
         Get additional necessary fixed arguments for sensors that need heightDepth
         params (soil moisture and soil temp)
         """
-
+        # TODO: this could be refactored into properties of the variable
         extra_params_map = {
             self.ALLOWED_VARIABLES.TEMPGROUND2IN: {
                 'height_depth': {"value": -2, "unitCd": "in"}
             },
             self.ALLOWED_VARIABLES.TEMPGROUND4IN: {
                 'height_depth': {"value": -4, "unitCd": "in"}
             },
             self.ALLOWED_VARIABLES.TEMPGROUND8IN: {
                 'height_depth': {"value": -8, "unitCd": "in"}
             },
             self.ALLOWED_VARIABLES.TEMPGROUND20IN: {
                 'height_depth': {"value": -20, "unitCd": "in"}
             },
-
+            self.ALLOWED_VARIABLES.SOILMOISTURE2IN: {
+                'height_depth': {"value": -2, "unitCd": "in"}
+            },
+            self.ALLOWED_VARIABLES.SOILMOISTURE4IN: {
+                'height_depth': {"value": -4, "unitCd": "in"}
+            },
+            self.ALLOWED_VARIABLES.SOILMOISTURE8IN: {
+                'height_depth': {"value": -8, "unitCd": "in"}
+            },
+            self.ALLOWED_VARIABLES.SOILMOISTURE20IN: {
+                'height_depth': {"value": -20, "unitCd": "in"}
+            },
         }
 
         extra_params = {}
         for variable in variables:
             result = extra_params_map.get(variable)
             if result:
                 extra_params[variable.name] = result
```

### Comparing `metloom-0.3.6/metloom/pointdata/snotel_client.py` & `metloom-0.3.7/metloom/pointdata/snotel_client.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/pointdata/usgs.py` & `metloom-0.3.7/metloom/pointdata/usgs.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/request_utils.py` & `metloom-0.3.7/metloom/request_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/metloom/variables.py` & `metloom-0.3.7/metloom/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,28 @@
     )
     TEMPGROUND8IN = SensorDescription(
         "STO", "GROUND TEMPERATURE -8IN", "GROUND TEMPERATURE OBS -8IN"
     )
     TEMPGROUND20IN = SensorDescription(
         "STO", "GROUND TEMPERATURE -20IN", "GROUND TEMPERATURE OBS -20IN"
     )
+    SOILMOISTURE2IN = SensorDescription(
+        "SMS", "SOIL MOISTURE -2IN", "SOIL MOISTURE PERCENT -2IN"
+    )
+    SOILMOISTURE4IN = SensorDescription(
+        "SMS", "SOIL MOISTURE -4IN", "SOIL MOISTURE PERCENT -4IN"
+    )
+    SOILMOISTURE8IN = SensorDescription(
+        "SMS", "SOIL MOISTURE -8IN", "SOIL MOISTURE PERCENT -8IN"
+    )
+    SOILMOISTURE20IN = SensorDescription(
+        "SMS", "SOIL MOISTURE -20IN", "SOIL MOISTURE PERCENT -20IN"
+    )
     # TODO for the SCAN network this appears to be "RHUM", we may need a new class
     RH = SensorDescription("RHUMV", "RELATIVE HUMIDITY", "RELATIVE HUMIDITY")
-    # SOILMOIS = SensorDescription("SMS", "SOIL MOISTURE", "SOIL MOISTURE")
     STREAMVOLUMEOBS = SensorDescription(
         "SRVO", "STREAM VOLUME OBS", "STREAM VOLUME OBS"
     )
     STREAMVOLUMEADJ = SensorDescription(
         "SRVOX", "STREAM VOLUME ADJ", "STREAM VOLUME ADJ"
     )
```

### Comparing `metloom-0.3.6/metloom.egg-info/PKG-INFO` & `metloom-0.3.7/metloom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.3.6
+Version: 0.3.7
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `metloom-0.3.6/metloom.egg-info/SOURCES.txt` & `metloom-0.3.7/metloom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/setup.py` & `metloom-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     include_package_data=True,
     keywords='metloom',
     name='metloom',
     packages=find_packages(include=['metloom', 'metloom.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/M3Works/metloom',
-    version='0.3.6',
+    version='0.3.7',
     zip_safe=False,
 )
```

### Comparing `metloom-0.3.6/tests/data/cdec_mocks/raw_tny_sensors.csv` & `metloom-0.3.7/tests/data/cdec_mocks/raw_tny_sensors.csv`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/data/daily_response.txt` & `metloom-0.3.7/tests/data/daily_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/data/platoro_meta.txt` & `metloom-0.3.7/tests/data/platoro_meta.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/data/station_search_response.txt` & `metloom-0.3.7/tests/data/station_search_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/test_cdec.py` & `metloom-0.3.7/tests/test_cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/test_dataframe_utils.py` & `metloom-0.3.7/tests/test_dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/test_mesowest.py` & `metloom-0.3.7/tests/test_mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/test_point_data.py` & `metloom-0.3.7/tests/test_point_data.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/test_snotel.py` & `metloom-0.3.7/tests/test_snotel.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/test_usgs.py` & `metloom-0.3.7/tests/test_usgs.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.6/tests/test_variables.py` & `metloom-0.3.7/tests/test_variables.py`

 * *Files identical despite different names*

