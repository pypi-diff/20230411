# Comparing `tmp/murfey-0.7.5.tar.gz` & `tmp/murfey-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murfey-0.7.5.tar", last modified: Tue Apr 11 07:43:09 2023, max compression
+gzip compressed data, was "murfey-0.7.6.tar", last modified: Tue Apr 11 12:43:24 2023, max compression
```

## Comparing `murfey-0.7.5.tar` & `murfey-0.7.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.636566 murfey-0.7.5/
--rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-11 07:43:04.000000 murfey-0.7.5/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-11 07:43:04.000000 murfey-0.7.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 07:43:09.636566 murfey-0.7.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-11 07:43:04.000000 murfey-0.7.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-11 07:43:04.000000 murfey-0.7.5/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-11 07:43:09.636566 murfey-0.7.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-11 07:43:04.000000 murfey-0.7.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.616566 murfey-0.7.5/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey/
--rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey/bootstrap/
--rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/bootstrap/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/cli/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/cli/transfer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.624566 murfey-0.7.5/src/murfey/client/
--rw-r--r--   0 vsts      (1001) docker     (122)    10515 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12029 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/analyser.py
--rw-r--r--   0 vsts      (1001) docker     (122)    45152 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/context.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.624566 murfey-0.7.5/src/murfey/client/contexts/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/contexts/tomo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/customlogging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/gain_ref.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7515 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/instance_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/rsync.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.628566 murfey-0.7.5/src/murfey/client/tui/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18265 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4475 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/controller.css
--rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/forms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/launcher.css
--rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/progress.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21083 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/screens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/status_bar.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/update.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/watchdir.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2180 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/watchdir_multigrid.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/server/
--rw-r--r--   0 vsts      (1001) docker     (122)    18038 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16457 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/bootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (122)      946 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11248 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/demo_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/gain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7593 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/ispyb.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/activevisits.html
--rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/base.html
--rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/bootstrap.html
--rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/home.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/templates/images/
--rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/images/diamond.png
--rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/images/icon_268.png
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/templates/static/
--rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/static/styles.css
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/visit.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.636566 murfey-0.7.5/src/murfey/util/
--rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/dummy_setup.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/file_monitor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/mdoc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3518 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/rsync.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/state.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.633490 murfey-0.7.6/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-11 12:43:14.000000 murfey-0.7.6/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-11 12:43:14.000000 murfey-0.7.6/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 12:43:24.633490 murfey-0.7.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-11 12:43:14.000000 murfey-0.7.6/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-11 12:43:14.000000 murfey-0.7.6/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-11 12:43:24.633490 murfey-0.7.6/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-11 12:43:14.000000 murfey-0.7.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.617489 murfey-0.7.6/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey/
+-rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey/bootstrap/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/bootstrap/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/cli/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/cli/transfer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.625490 murfey-0.7.6/src/murfey/client/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10515 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12051 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/analyser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    46554 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/context.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.625490 murfey-0.7.6/src/murfey/client/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/contexts/tomo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/customlogging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/gain_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7814 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/instance_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/rsync.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.625490 murfey-0.7.6/src/murfey/client/tui/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18326 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4475 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/controller.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/launcher.css
+-rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21322 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/screens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/tui/status_bar.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/update.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/watchdir.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/watchdir_multigrid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/client/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.629490 murfey-0.7.6/src/murfey/server/
+-rw-r--r--   0 vsts      (1001) docker     (122)    17869 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16460 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/bootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      946 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11248 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/demo_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/gain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/ispyb.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/server/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.629490 murfey-0.7.6/src/murfey/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/activevisits.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/base.html
+-rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/bootstrap.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/home.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.629490 murfey-0.7.6/src/murfey/templates/images/
+-rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/images/diamond.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/images/icon_268.png
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.633490 murfey-0.7.6/src/murfey/templates/static/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/static/styles.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/templates/visit.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.633490 murfey-0.7.6/src/murfey/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/dummy_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/file_monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/mdoc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3518 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/rsync.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-11 12:43:14.000000 murfey-0.7.6/src/murfey/util/state.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 12:43:24.621490 murfey-0.7.6/src/murfey.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-11 12:43:24.000000 murfey-0.7.6/src/murfey.egg-info/top_level.txt
```

### Comparing `murfey-0.7.5/LICENSE` & `murfey-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/PKG-INFO` & `murfey-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.5
+Version: 0.7.6
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.5/README.md` & `murfey-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/setup.cfg` & `murfey-0.7.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = murfey
 description = Client-Server architecture hauling Cryo-EM data
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.7.5
+version = 0.7.6
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `murfey-0.7.5/src/murfey/bootstrap/__main__.py` & `murfey-0.7.6/src/murfey/bootstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/cli/dummy.py` & `murfey-0.7.6/src/murfey/cli/dummy.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/cli/transfer.py` & `murfey-0.7.6/src/murfey/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/__init__.py` & `murfey-0.7.6/src/murfey/client/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/analyser.py` & `murfey-0.7.6/src/murfey/client/analyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,25 +229,25 @@
         data_directories = get_machine_config(self._environment.url.geturl()).get(
             "data_directories", {}
         )
         for dd in data_directories.keys():
             if str(data_file).startswith(dd):
                 base_dir = Path(dd)
                 mid_dir = data_file.relative_to(dd).parent
-                if (
-                    base_dir
-                    / self._environment.visit
-                    / mid_dir.parts[0]
-                    / "Images-Disc1"
-                ).is_dir():
-                    mid_dir = Path(
-                        mid_dir.parts[0]
-                        + "/Images-Disc1/"
-                        + "/".join(mid_dir.parts[1:])
-                    )
+                # if (
+                #     base_dir
+                #     / self._environment.visit
+                #     / mid_dir.parts[0]
+                #     / "Images-Disc1"
+                # ).is_dir():
+                #     mid_dir = Path(
+                #         mid_dir.parts[0]
+                #         + "/Images-Disc1/"
+                #         + "/".join(mid_dir.parts[1:])
+                #     )
                 break
         else:
             return data_file.with_suffix(".xml")
         return base_dir / self._environment.visit / mid_dir / file_name
 
     def enqueue(self, rsyncer: RSyncerUpdate):
         if not self._stopping:
```

### Comparing `murfey-0.7.5/src/murfey/client/context.py` & `murfey-0.7.6/src/murfey/client/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,21 +106,35 @@
 
     def __init__(self, acquisition_software: str, basepath: Path):
         super().__init__(acquisition_software)
         self._basepath = basepath
         self._processing_job_stash: dict = {}
         self._preprocessing_triggers: dict = {}
 
-    def _flush_processing_job(self, tag: str, parameters: Dict[str, Any] | None = None):
+    def _flush_processing_job(
+        self,
+        tag: str,
+        environment: MurfeyInstanceEnvironment,
+        parameters: Dict[str, Any] | None = None,
+    ):
         if parameters:
             proc_job_future = self._processing_job_stash[tag]
+            machine_config = get_machine_config(
+                str(environment.url.geturl()), demo=environment.demo
+            )
+            image_directory = str(
+                Path(machine_config.get("rsync_basepath", "."))
+                / environment.default_destinations[Path(tag)]
+            )
             if self._acquisition_software == "epu":
-                import_images = f"{Path(parameters['image_directory']).resolve()}/GridSquare*/Data/*{parameters['file_extension']}"
+                import_images = f"{Path(image_directory).resolve()}/GridSquare*/Data/*{parameters['file_extension']}"
             else:
-                import_images = f"{Path(parameters['image_directory']).resolve()}/*{parameters['file_extension']}"
+                import_images = (
+                    f"{Path(image_directory).resolve()}/*{parameters['file_extension']}"
+                )
             msg = {
                 **proc_job_future.message,
                 "parameters": {
                     "acquisition_software": parameters["acquisition_software"],
                     "voltage": parameters["voltage"],
                     "motioncor_gainreference": parameters["gain_ref"],
                     "motioncor_doseperframe": parameters["dose_per_frame"],
@@ -133,27 +147,40 @@
                     "extract_small_boxsize": parameters["small_boxsize"],
                     "mask_diameter": parameters["mask_diameter"],
                     "autopick_do_cryolo": parameters["use_cryolo"],
                 },
             }
             requests.post(proc_job_future.url, json=msg)
 
-    def _register_data_collection(self, url: str, data: dict):
+    def _register_data_collection(
+        self,
+        tag: str,
+        url: str,
+        data: dict,
+        environment: MurfeyInstanceEnvironment,
+    ):
         logger.info(f"registering data collection with data {data}")
+        machine_config = get_machine_config(
+            str(environment.url.geturl()), demo=environment.demo
+        )
+        image_directory = str(
+            Path(machine_config.get("rsync_basepath", "."))
+            / environment.default_destinations[Path(tag)]
+        )
         json = {
             "voltage": data["voltage"],
             "pixel_size_on_image": data["pixel_size_on_image"],
             "experiment_type": data["experiment_type"],
             "image_size_x": data["image_size_x"],
             "image_size_y": data["image_size_y"],
             "file_extension": data["file_extension"],
             "acquisition_software": data["acquisition_software"],
-            "image_directory": data["image_directory"],
-            "tag": data["tag"],
-            "source": data["source"],
+            "image_directory": image_directory,
+            "tag": tag,
+            "source": tag,
             "magnification": data["magnification"],
             "total_exposed_dose": data.get("total_exposed_dose"),
             "c2aperture": data.get("c2aperture"),
             "exposure_time": data.get("exposure_time"),
             "slit_width": data.get("slit_width"),
             "phase_plate": data.get("phase_plate", False),
         }
@@ -172,35 +199,56 @@
                 if transferred_file.is_relative_to(s):
                     source = str(s)
                     break
             proc_url = f"{str(environment.url.geturl())}/visits/{environment.visit}/register_processing_job"
             if environment.data_collection_ids.get(source) is None:
                 self._processing_job_stash[source] = FutureRequest(
                     proc_url,
-                    {"tag": source, "recipe": "relion"},
+                    {"tag": source, "recipe": "ispyb-relion"},
                 )
             elif environment.data_collection_parameters:
                 if self._processing_job_stash.get(source):
                     # self._flush_processing_job(source)
                     pass
                 requests.post(
                     proc_url,
                     json={
                         "tag": source,
-                        "recipe": "relion",
+                        "recipe": "ispyb-relion",
                         "parameters": environment.data_collection_parameters,
                     },
                 )
 
     def _register_processing_job(
-        self, tag: str, parameters: Dict[str, Any] | None = None
+        self,
+        tag: str,
+        environment: MurfeyInstanceEnvironment,
+        parameters: Dict[str, Any] | None = None,
     ):
         logger.info(f"registering processing job with parameters: {parameters}")
+        machine_config = get_machine_config(
+            str(environment.url.geturl()), demo=environment.demo
+        )
+        image_directory = str(
+            Path(machine_config.get("rsync_basepath", "."))
+            / environment.default_destinations[Path(tag)]
+        )
         if self._processing_job_stash.get(tag):
-            self._flush_processing_job(tag, parameters=parameters)
+            params = {
+                "tag": tag,
+                "source": tag,
+                "image_directory": image_directory,
+            }
+            if parameters:
+                params.update(parameters)
+            self._flush_processing_job(
+                tag,
+                environment,
+                parameters=params,
+            )
             self._processing_job_stash.pop(tag)
 
     def _launch_spa_pipeline(self, tag: str, jobid: int, url: str = ""):
         data = {"job_id": jobid}
         requests.post(url, json=data)
 
     def gather_metadata(
@@ -364,15 +412,15 @@
         self._data_collection_stash: list = []
         self._processing_job_stash: dict = {}
         self._preprocessing_triggers: dict = {}
         self._lock: RLock = RLock()
         self._extract_tilt_series: Callable[[Path], str] | None = None
         self._extract_tilt_tag: Callable[[Path], str] | None = None
 
-    def _flush_data_collections(self):
+    def _flush_data_collections(self, tag: str):
         logger.info("Flushing data collection API calls")
         for dc_data in self._data_collection_stash:
             data = {**dc_data[2], **dc_data[1].data_collection_parameters}
             requests.post(dc_data[0], json=data)
         self._data_collection_stash = []
 
     def _flush_processing_job(self, tag: str):
```

### Comparing `murfey-0.7.5/src/murfey/client/contexts/tomo.py` & `murfey-0.7.6/src/murfey/client/contexts/tomo.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/customlogging.py` & `murfey-0.7.6/src/murfey/client/customlogging.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/gain_ref.py` & `murfey-0.7.6/src/murfey/client/gain_ref.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/instance_environment.py` & `murfey-0.7.6/src/murfey/client/instance_environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,22 @@
         self.visit = ""
         self.gain_ref = None
 
     @validator("data_collection_group_ids")
     def dcg_callback(cls, v, values):
         with global_env_lock:
             for l in values.get("listeners", {}).get("data_collection_group_ids", []):
-                l()
+                if values.get("data_collection_group_ids"):
+                    for k in set(values["data_collection_group_ids"].keys()) ^ set(
+                        v.keys()
+                    ):
+                        l(k)
+                else:
+                    for k in v.keys():
+                        l(k)
         return v
 
     @validator("data_collection_ids")
     def dc_callback(cls, v, values):
         with global_env_lock:
             for l in values.get("listeners", {}).get("data_collection_ids", []):
                 if values.get("data_collection_ids"):
```

### Comparing `murfey-0.7.5/src/murfey/client/rsync.py` & `murfey-0.7.6/src/murfey/client/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/tui/app.py` & `murfey-0.7.6/src/murfey/client/tui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,37 +303,39 @@
         elif isinstance(context, SPAContext):
             source = Path(json["source"])
             machine_config = get_machine_config(
                 str(self._url.geturl()), demo=self._environment.demo
             )
             url = f"{str(self._url.geturl())}/visits/{str(self._visit)}/start_data_collection"
             json = {
-                "tag": str(source.resolve()),
-                "image_directory": str(
-                    Path(machine_config.get("rsync_basepath", "."))
-                    / self._environment.default_destinations[source]
-                ),
+                "image_directory": Path(
+                    machine_config.get("rsync_basepath", ".")
+                ).resolve(),
                 **json,
             }
             self._environment.listeners["data_collection_group_ids"] = {
                 partial(
                     context._register_data_collection,
                     url=url,
                     data=json,
+                    environment=self._environment,
                 )
             }
             self._environment.listeners["data_collection_ids"] = {
                 partial(
                     context._register_processing_job,
                     parameters=json,
+                    environment=self._environment,
                 )
             }
             url = f"{str(self._url.geturl())}/visits/{str(self._visit)}/spa_processing"
             self._environment.listeners["processing_job_ids"] = {
-                partial(context._launch_spa_pipeline, url=url)
+                partial(
+                    context._launch_spa_pipeline, url=url, environment=self._environment
+                )
             }
             url = f"{str(self._url.geturl())}/visits/{str(self._visit)}/register_data_collection_group"
             dcg_data = {
                 "experiment_type": "single particle",
                 "experiment_type_id": 37,
                 "tag": str(source),
             }
```

### Comparing `murfey-0.7.5/src/murfey/client/tui/controller.css` & `murfey-0.7.6/src/murfey/client/tui/controller.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/tui/forms.py` & `murfey-0.7.6/src/murfey/client/tui/forms.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/tui/progress.py` & `murfey-0.7.6/src/murfey/client/tui/progress.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/tui/screens.py` & `murfey-0.7.6/src/murfey/client/tui/screens.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,33 @@
                 try:
                     mid_path = source.resolve().relative_to(data_dir)
                     if (
                         machine_data["data_directories"][data_dir] == "detector"
                         and use_suggested_path
                     ):
                         with global_env_lock:
-                            if environment.destination_registry.get(source.name):
-                                _default = environment.destination_registry[source.name]
+                            source_name = (
+                                source.name
+                                if source.name != "Images-Disc1"
+                                else source.parent.name
+                            )
+                            if environment.destination_registry.get(source_name):
+                                _default = environment.destination_registry[source_name]
                             else:
                                 suggested_path_response = requests.post(
                                     url=f"{str(environment.url.geturl())}/visits/{visit}/suggested_path",
                                     json={
                                         "base_path": f"{destination}/{visit}/{mid_path.parent if include_mid_path else ''}/raw",
                                         "touch": touch,
                                     },
                                 )
                                 _default = suggested_path_response.json().get(
                                     "suggested_path"
                                 )
-                                environment.destination_registry[source.name] = _default
+                                environment.destination_registry[source_name] = _default
                     else:
                         _default = f"{destination}/{visit}/{mid_path if include_mid_path else source.name}"
                     if analysers.get(source):
                         analysers[source]._role = machine_data["data_directories"][
                             data_dir
                         ]
                     break
```

### Comparing `murfey-0.7.5/src/murfey/client/tui/status_bar.py` & `murfey-0.7.6/src/murfey/client/tui/status_bar.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/update.py` & `murfey-0.7.6/src/murfey/client/update.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/watchdir.py` & `murfey-0.7.6/src/murfey/client/watchdir.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/client/watchdir_multigrid.py` & `murfey-0.7.6/src/murfey/client/watchdir_multigrid.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,10 +55,10 @@
                         )
                         self._seen_dirs.append(d)
                     if (d.parent.parent / d.name / "Images-Disc1").is_dir():
                         d02 = d.parent.parent / d.name / "Images-Disc1"
                     else:
                         d02 = d.parent.parent / d.name
                     if d02.is_dir() and d02 not in self._seen_dirs:
-                        self.notify(d02)
+                        self.notify(d02, include_mid_path=False)
                         self._seen_dirs.append(d02)
             time.sleep(15)
```

### Comparing `murfey-0.7.5/src/murfey/client/websocket.py` & `murfey-0.7.6/src/murfey/client/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/server/__init__.py` & `murfey-0.7.6/src/murfey/server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         _dcid = global_state["data_collection_ids"][message["tag"]]
         record = ProcessingJob(dataCollectionId=_dcid, recipe=message["recipe"])
         if message.get("job_parameters"):
             job_parameters = [
                 ProcessingJobParameter(parameterKey=k, parameterValue=v)
                 for k, v in message["job_parameters"].items()
             ]
-            pid = _register(ExtendedRecord(record, job_parameters))
+            pid = _register(ExtendedRecord(record, job_parameters), header)
         else:
             pid = _register(record, header)
         if pid is None and _transport_object:
             _transport_object.transport.nack(header)
             return None
         if global_state.get("processing_job_ids"):
             global_state["processing_job_ids"] = {
@@ -420,14 +420,16 @@
                     **global_state["processing_job_ids"].get(message.get("tag"), {}),  # type: ignore
                     message["recipe"]: pid,
                 },
             }
         else:
             prids = {message["tag"]: {message["recipe"]: pid}}
             global_state["processing_job_ids"] = prids
+        if message.get("job_parameters"):
+            return None
         record = AutoProcProgram(processingJobId=pid)
         appid = _register(record, header)
         if appid is None and _transport_object:
             _transport_object.transport.nack(header)
             return None
         if global_state.get("autoproc_program_ids"):
             assert isinstance(global_state["autoproc_program_ids"], dict)
@@ -495,21 +497,14 @@
 
 
 @_register.register  # type: ignore
 def _(extended_record: ExtendedRecord, header: dict, **kwargs):
     return _transport_object.do_create_ispyb_job(
         extended_record.record, params=extended_record.record_params
     )["return_value"]
-
-
-@_register.register  # type: ignore
-def _(extended_record: ExtendedRecord, header: dict, **kwargs):
-    return _transport_object.do_create_ispyb_job(
-        extended_record.record, params=extended_record.record_params
-    )["return_value"]
 
 
 def feedback_listen():
     if _transport_object:
         if not _transport_object.feedback_queue:
             _transport_object.feedback_queue = (
                 _transport_object.transport._subscribe_temporary(
```

### Comparing `murfey-0.7.5/src/murfey/server/api.py` & `murfey-0.7.6/src/murfey/server/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         )
 
 
 @router.post("/visits/{visit_name}/spa_processing")
 async def request_spa_processing(visit_name: str, proc_params: SPAProcessingParameters):
     zocalo_message = {
         "parameters": {"ispyb_process": proc_params.job_id},
-        "recipes": ["relion"],
+        "recipes": ["ispyb-relion"],
     }
     if _transport_object:
         _transport_object.send("processing_recipe", zocalo_message)
 
 
 @router.post("/visits/{visit_name}/tomography_preprocess")
 async def request_tomography_preprocessing(visit_name: str, proc_file: ProcessFile):
@@ -400,15 +400,15 @@
             microscope=get_microscope(),
             proposal_code=ispyb_proposal_code,
             proposal_number=ispyb_proposal_number,
             visit_number=ispyb_visit_number,
             db=murfey.server.ispyb.Session(),
         ),
         "image_directory": str(
-            machine_config["rsync_basepath"] / dc_params.image_directory
+            machine_config.rsync_basepath / dc_params.image_directory
         ),
         "start_time": str(datetime.datetime.now()),
         "voltage": dc_params.voltage,
         "pixel_size": str(float(dc_params.pixel_size_on_image) * 1e9),
         "image_suffix": dc_params.file_extension,
         "experiment_type": dc_params.experiment_type,
         "image_size_x": dc_params.image_size_x,
```

### Comparing `murfey-0.7.5/src/murfey/server/bootstrap.py` & `murfey-0.7.6/src/murfey/server/bootstrap.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/server/config.py` & `murfey-0.7.6/src/murfey/server/config.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/server/demo_api.py` & `murfey-0.7.6/src/murfey/server/demo_api.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/server/gain.py` & `murfey-0.7.6/src/murfey/server/gain.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/server/ispyb.py` & `murfey-0.7.6/src/murfey/server/ispyb.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,17 +113,17 @@
         jp["display_name"] = record.displayName
         jp["recipe"] = record.recipe
         log.info("Creating database entries...")
         try:
             jobid = self.ispyb.mx_processing.upsert_job(list(jp.values()))
             for p in params:
                 pp = self.ispyb.mx_processing.get_job_parameter_params()
-                pp["jobid"] = jobid
-                pp["parameterkey"] = p.parameterKey
-                pp["parametervalue"] = p.parametervalue
+                pp["job_id"] = jobid
+                pp["parameter_key"] = p.parameterKey
+                pp["parameter_value"] = p.parameterValue
                 self.ispyb.mx_processing.upsert_job_parameter(list(pp.values()))
             log.info(f"All done. Processing job {jobid} created")
             return {"success": True, "return_value": jobid}
         except ispyb.ISPyBException as e:
             log.error(
                 "Inserting Processing Job entry caused exception '%s'.",
                 e,
```

### Comparing `murfey-0.7.5/src/murfey/server/main.py` & `murfey-0.7.6/src/murfey/server/main.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/server/websocket.py` & `murfey-0.7.6/src/murfey/server/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/templates/activevisits.html` & `murfey-0.7.6/src/murfey/templates/activevisits.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/templates/base.html` & `murfey-0.7.6/src/murfey/templates/base.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/templates/bootstrap.html` & `murfey-0.7.6/src/murfey/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/templates/images/diamond.png` & `murfey-0.7.6/src/murfey/templates/images/diamond.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/templates/images/icon_268.png` & `murfey-0.7.6/src/murfey/templates/images/icon_268.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/templates/static/styles.css` & `murfey-0.7.6/src/murfey/templates/static/styles.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/templates/visit.html` & `murfey-0.7.6/src/murfey/templates/visit.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/util/__init__.py` & `murfey-0.7.6/src/murfey/util/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/util/dummy_setup.py` & `murfey-0.7.6/src/murfey/util/dummy_setup.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/util/file_monitor.py` & `murfey-0.7.6/src/murfey/util/file_monitor.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/util/mdoc.py` & `murfey-0.7.6/src/murfey/util/mdoc.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/util/models.py` & `murfey-0.7.6/src/murfey/util/models.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/util/rsync.py` & `murfey-0.7.6/src/murfey/util/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey/util/state.py` & `murfey-0.7.6/src/murfey/util/state.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.5/src/murfey.egg-info/PKG-INFO` & `murfey-0.7.6/src/murfey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.5
+Version: 0.7.6
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.5/src/murfey.egg-info/SOURCES.txt` & `murfey-0.7.6/src/murfey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

