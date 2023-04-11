# Comparing `tmp/murfey-0.7.3.tar.gz` & `tmp/murfey-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murfey-0.7.3.tar", last modified: Thu Apr  6 07:45:14 2023, max compression
+gzip compressed data, was "murfey-0.7.5.tar", last modified: Tue Apr 11 07:43:09 2023, max compression
```

## Comparing `murfey-0.7.3.tar` & `murfey-0.7.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.463202 murfey-0.7.3/
--rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-06 07:45:09.000000 murfey-0.7.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-06 07:45:09.000000 murfey-0.7.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-06 07:45:14.463202 murfey-0.7.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-06 07:45:09.000000 murfey-0.7.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-06 07:45:09.000000 murfey-0.7.3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-06 07:45:14.463202 murfey-0.7.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-06 07:45:09.000000 murfey-0.7.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.443201 murfey-0.7.3/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.447201 murfey-0.7.3/src/murfey/
--rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.451202 murfey-0.7.3/src/murfey/bootstrap/
--rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/bootstrap/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.451202 murfey-0.7.3/src/murfey/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/cli/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/cli/transfer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.455201 murfey-0.7.3/src/murfey/client/
--rw-r--r--   0 vsts      (1001) docker     (122)    10515 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11556 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/analyser.py
--rw-r--r--   0 vsts      (1001) docker     (122)    41187 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/context.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.455201 murfey-0.7.3/src/murfey/client/contexts/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/contexts/tomo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/customlogging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/gain_ref.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7515 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/instance_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11832 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/rsync.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.455201 murfey-0.7.3/src/murfey/client/tui/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17252 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4475 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/controller.css
--rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/forms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/launcher.css
--rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/progress.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19658 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/screens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/tui/status_bar.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/update.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/watchdir.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1725 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/watchdir_multigrid.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/client/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.459202 murfey-0.7.3/src/murfey/server/
--rw-r--r--   0 vsts      (1001) docker     (122)    17697 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16101 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/bootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (122)      946 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11248 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/demo_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/gain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7317 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/ispyb.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/server/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.459202 murfey-0.7.3/src/murfey/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/activevisits.html
--rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/base.html
--rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/bootstrap.html
--rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/home.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.463202 murfey-0.7.3/src/murfey/templates/images/
--rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/images/diamond.png
--rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/images/icon_268.png
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.463202 murfey-0.7.3/src/murfey/templates/static/
--rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/static/styles.css
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/templates/visit.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.463202 murfey-0.7.3/src/murfey/util/
--rw-r--r--   0 vsts      (1001) docker     (122)     3421 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/util/dummy_setup.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/util/file_monitor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/util/mdoc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3059 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/util/models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/util/rsync.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-06 07:45:09.000000 murfey-0.7.3/src/murfey/util/state.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 07:45:14.451202 murfey-0.7.3/src/murfey.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-06 07:45:14.000000 murfey-0.7.3/src/murfey.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-06 07:45:14.000000 murfey-0.7.3/src/murfey.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-06 07:45:14.000000 murfey-0.7.3/src/murfey.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-06 07:45:14.000000 murfey-0.7.3/src/murfey.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-06 07:45:14.000000 murfey-0.7.3/src/murfey.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-06 07:45:14.000000 murfey-0.7.3/src/murfey.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-06 07:45:14.000000 murfey-0.7.3/src/murfey.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.636566 murfey-0.7.5/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-11 07:43:04.000000 murfey-0.7.5/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-11 07:43:04.000000 murfey-0.7.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 07:43:09.636566 murfey-0.7.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-11 07:43:04.000000 murfey-0.7.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-11 07:43:04.000000 murfey-0.7.5/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-11 07:43:09.636566 murfey-0.7.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-11 07:43:04.000000 murfey-0.7.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.616566 murfey-0.7.5/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey/
+-rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey/bootstrap/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/bootstrap/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/cli/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/cli/transfer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.624566 murfey-0.7.5/src/murfey/client/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10515 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12029 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/analyser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    45152 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/context.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.624566 murfey-0.7.5/src/murfey/client/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/contexts/tomo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/customlogging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/gain_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7515 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/instance_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/rsync.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.628566 murfey-0.7.5/src/murfey/client/tui/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18265 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4475 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/controller.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/launcher.css
+-rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21083 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/screens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/tui/status_bar.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/update.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/watchdir.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2180 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/watchdir_multigrid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/client/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/server/
+-rw-r--r--   0 vsts      (1001) docker     (122)    18038 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16457 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/bootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      946 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11248 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/demo_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/gain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7593 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/ispyb.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/server/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/activevisits.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/base.html
+-rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/bootstrap.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/home.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/templates/images/
+-rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/images/diamond.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/images/icon_268.png
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.632566 murfey-0.7.5/src/murfey/templates/static/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/static/styles.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/templates/visit.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.636566 murfey-0.7.5/src/murfey/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/dummy_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/file_monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/mdoc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3518 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/rsync.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-11 07:43:04.000000 murfey-0.7.5/src/murfey/util/state.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-11 07:43:09.620566 murfey-0.7.5/src/murfey.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-11 07:43:09.000000 murfey-0.7.5/src/murfey.egg-info/top_level.txt
```

### Comparing `murfey-0.7.3/LICENSE` & `murfey-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/PKG-INFO` & `murfey-0.7.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.3
+Version: 0.7.5
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.3/README.md` & `murfey-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/setup.cfg` & `murfey-0.7.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = murfey
 description = Client-Server architecture hauling Cryo-EM data
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.7.3
+version = 0.7.5
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `murfey-0.7.3/src/murfey/bootstrap/__main__.py` & `murfey-0.7.5/src/murfey/bootstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/cli/dummy.py` & `murfey-0.7.5/src/murfey/cli/dummy.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/cli/transfer.py` & `murfey-0.7.5/src/murfey/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/__init__.py` & `murfey-0.7.5/src/murfey/client/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/analyser.py` & `murfey-0.7.5/src/murfey/client/analyser.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,15 +46,18 @@
     def _find_extension(self, file_path: Path):
         if (
             file_path.suffix in (".mrc", ".tiff", ".tif", ".eer")
             and not self._extension
         ):
             logger.info(f"File extension determined: {file_path.suffix}")
             self._extension = file_path.suffix
-        elif file_path.suffix in (".tiff", ".tif", ".eer"):
+        elif (
+            file_path.suffix in (".tiff", ".tif", ".eer")
+            and self._extension != file_path.suffix
+        ):
             logger.info(f"File extension re-evaluated: {file_path.suffix}")
             self._extension = file_path.suffix
 
     def _find_context(self, file_path: Path) -> bool:
         split_file_name = file_path.name.split("_")
         if split_file_name:
             if split_file_name[0].startswith("FoilHole"):
@@ -223,17 +226,28 @@
         file_name = (
             f"{data_file.stem.replace('_fractions', '').replace('_Fractions', '')}.xml"
         )
         data_directories = get_machine_config(self._environment.url.geturl()).get(
             "data_directories", {}
         )
         for dd in data_directories.keys():
-            if str(data_file).startswith(str(dd)):
-                base_dir = dd
+            if str(data_file).startswith(dd):
+                base_dir = Path(dd)
                 mid_dir = data_file.relative_to(dd).parent
+                if (
+                    base_dir
+                    / self._environment.visit
+                    / mid_dir.parts[0]
+                    / "Images-Disc1"
+                ).is_dir():
+                    mid_dir = Path(
+                        mid_dir.parts[0]
+                        + "/Images-Disc1/"
+                        + "/".join(mid_dir.parts[1:])
+                    )
                 break
         else:
             return data_file.with_suffix(".xml")
         return base_dir / self._environment.visit / mid_dir / file_name
 
     def enqueue(self, rsyncer: RSyncerUpdate):
         if not self._stopping:
```

### Comparing `murfey-0.7.3/src/murfey/client/context.py` & `murfey-0.7.5/src/murfey/client/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,23 +109,27 @@
         self._basepath = basepath
         self._processing_job_stash: dict = {}
         self._preprocessing_triggers: dict = {}
 
     def _flush_processing_job(self, tag: str, parameters: Dict[str, Any] | None = None):
         if parameters:
             proc_job_future = self._processing_job_stash[tag]
+            if self._acquisition_software == "epu":
+                import_images = f"{Path(parameters['image_directory']).resolve()}/GridSquare*/Data/*{parameters['file_extension']}"
+            else:
+                import_images = f"{Path(parameters['image_directory']).resolve()}/*{parameters['file_extension']}"
             msg = {
                 **proc_job_future.message,
                 "parameters": {
                     "acquisition_software": parameters["acquisition_software"],
                     "voltage": parameters["voltage"],
                     "motioncor_gainreference": parameters["gain_ref"],
                     "motioncor_doseperframe": parameters["dose_per_frame"],
                     "eer_grouping": parameters["eer_grouping"],
-                    "import_images": f"{Path(parameters['image_directory']).resolve()}/*{parameters['file_extension']}",
+                    "import_images": import_images,
                     "angpix": parameters["pixel_size_on_image"],
                     "symmetry": parameters["symmetry"],
                     "extract_boxsize": parameters["boxsize"],
                     "extract_downscale": parameters["downscale"],
                     "extract_small_boxsize": parameters["small_boxsize"],
                     "mask_diameter": parameters["mask_diameter"],
                     "autopick_do_cryolo": parameters["use_cryolo"],
@@ -141,14 +145,21 @@
             "experiment_type": data["experiment_type"],
             "image_size_x": data["image_size_x"],
             "image_size_y": data["image_size_y"],
             "file_extension": data["file_extension"],
             "acquisition_software": data["acquisition_software"],
             "image_directory": data["image_directory"],
             "tag": data["tag"],
+            "source": data["source"],
+            "magnification": data["magnification"],
+            "total_exposed_dose": data.get("total_exposed_dose"),
+            "c2aperture": data.get("c2aperture"),
+            "exposure_time": data.get("exposure_time"),
+            "slit_width": data.get("slit_width"),
+            "phase_plate": data.get("phase_plate", False),
         }
         requests.post(url, json=json)
 
     def post_transfer(
         self,
         transferred_file: Path,
         role: str = "",
@@ -179,14 +190,15 @@
                         "parameters": environment.data_collection_parameters,
                     },
                 )
 
     def _register_processing_job(
         self, tag: str, parameters: Dict[str, Any] | None = None
     ):
+        logger.info(f"registering processing job with parameters: {parameters}")
         if self._processing_job_stash.get(tag):
             self._flush_processing_job(tag, parameters=parameters)
             self._processing_job_stash.pop(tag)
 
     def _launch_spa_pipeline(self, tag: str, jobid: int, url: str = ""):
         data = {"job_id": jobid}
         requests.post(url, json=data)
@@ -204,26 +216,100 @@
         with open(metadata_file, "r") as xml:
             try:
                 for_parsing = xml.read()
             except Exception:
                 logger.warning(f"Failed to parse file {metadata_file}")
                 return OrderedDict({})
             data = xmltodict.parse(for_parsing)
+        magnification = 0
         metadata: OrderedDict = OrderedDict({})
         metadata["experiment_type"] = TUIFormValue("SPA")
-        metadata["voltage"] = TUIFormValue(300)
-        metadata["image_size_x"] = TUIFormValue(
-            data["Acquisition"]["Info"]["ImageSize"]["Width"]
-        )
-        metadata["image_size_y"] = TUIFormValue(
-            data["Acquisition"]["Info"]["ImageSize"]["Height"]
-        )
-        metadata["pixel_size_on_image"] = TUIFormValue(
-            float(data["Acquisition"]["Info"]["SensorPixelSize"]["Height"])
-        )
+        if data.get("Acquisition"):
+            metadata["voltage"] = TUIFormValue(300)
+            metadata["image_size_x"] = TUIFormValue(
+                data["Acquisition"]["Info"]["ImageSize"]["Width"]
+            )
+            metadata["image_size_y"] = TUIFormValue(
+                data["Acquisition"]["Info"]["ImageSize"]["Height"]
+            )
+            metadata["pixel_size_on_image"] = TUIFormValue(
+                float(data["Acquisition"]["Info"]["SensorPixelSize"]["Height"])
+            )
+        elif data.get("MicroscopeImage"):
+            metadata["voltage"] = TUIFormValue(
+                float(
+                    data["MicroscopeImage"]["microscopeData"]["gun"][
+                        "AccelerationVoltage"
+                    ]
+                )
+                / 1000
+            )
+            metadata["image_size_x"] = TUIFormValue(
+                data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
+                    "ReadoutArea"
+                ]["a:width"]
+            )
+            metadata["image_size_y"] = TUIFormValue(
+                data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
+                    "ReadoutArea"
+                ]["a:height"]
+            )
+            metadata["pixel_size_on_image"] = TUIFormValue(
+                data["MicroscopeImage"]["SpatialScale"]["pixelSize"]["x"][
+                    "numericValue"
+                ]
+            )
+            magnification = data["MicroscopeImage"]["microscopeData"]["optics"][
+                "TemMagnification"
+            ]["NominalMagnification"]
+            metadata["magnification"] = TUIFormValue(magnification)
+            metadata["total_exposed_dose"] = TUIFormValue(
+                data["MicroscopeImage"]["CustomData"]["a:KeyValueOfstringanyType"][0][
+                    "a:Value"
+                ]["#text"]
+            )
+            metadata["c2aperture"] = TUIFormValue(
+                data["MicroscopeImage"]["CustomData"]["a:KeyValueOfstringanyType"][3][
+                    "a:Value"
+                ]["#text"]
+            )
+            metadata["exposure_time"] = TUIFormValue(
+                data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
+                    "ExposureTime"
+                ]
+            )
+            metadata["slit_width"] = TUIFormValue(
+                data["MicroscopeImage"]["microscopeData"]["optics"]["EnergyFilter"][
+                    "EnergySelectionSlitWidth"
+                ]
+            )
+            metadata["phase_plate"] = TUIFormValue(
+                1
+                if data["MicroscopeImage"]["CustomData"]["a:KeyValueOfstringanyType"][
+                    11
+                ]["a:Value"]["#text"]
+                == "true"
+                else 0
+            )
+        else:
+            logger.warning("Metadata file format is not recognised")
+            return OrderedDict({})
+        if environment and magnification:
+            server_config = requests.get(
+                f"{str(environment.url.geturl())}/machine/"
+            ).json()
+            ps_from_mag = (
+                server_config.get("calibrations", {})
+                .get("magnification", {})
+                .get(int(magnification))
+            )
+            if ps_from_mag:
+                metadata["pixel_size_on_image"] = TUIFormValue(
+                    float(ps_from_mag) * 1e-10
+                )
         metadata["motion_corr_binning"] = TUIFormValue(1)
         metadata["gain_ref"] = TUIFormValue(None, top=True)
         metadata["dose_per_frame"] = TUIFormValue(
             environment.data_collection_parameters.get("dose_per_frame")
             if environment
             else None,
             top=True,
@@ -496,15 +582,21 @@
             try:
                 if environment:
                     url = f"{str(environment.url.geturl())}/visits/{environment.visit}/start_data_collection"
                     data = {
                         "experiment_type": "tomography",
                         "file_extension": file_path.suffix,
                         "acquisition_software": self._acquisition_software,
-                        "image_directory": str(file_path.parent),
+                        "image_directory": str(
+                            Path(
+                                environment.default_destinations.get(
+                                    file_path.parent, file_path.parent
+                                )
+                            ).resolve()
+                        ),
                         "tag": tilt_series,
                         "source": str(self._basepath),
                     }
                     if environment.data_collection_parameters:
                         data.update(
                             {
                                 "voltage": environment.data_collection_parameters[
```

### Comparing `murfey-0.7.3/src/murfey/client/contexts/tomo.py` & `murfey-0.7.5/src/murfey/client/contexts/tomo.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/customlogging.py` & `murfey-0.7.5/src/murfey/client/customlogging.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/gain_ref.py` & `murfey-0.7.5/src/murfey/client/gain_ref.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/instance_environment.py` & `murfey-0.7.5/src/murfey/client/instance_environment.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/rsync.py` & `murfey-0.7.5/src/murfey/client/rsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,15 @@
                         files_to_transfer.append(next_file)
                     else:
                         self.queue.task_done()
                         break
             except queue.Empty:
                 pass
 
-            logger.info(
-                f"Preparing to transfer {len(files_to_transfer)} files: {files_to_transfer}, {self}"
-            )
+            logger.info(f"Preparing to transfer {len(files_to_transfer)} files")
             if self._do_transfer:
                 try:
                     success = self._transfer(files_to_transfer)
                 except Exception as e:
                     logger.error(
                         f"Unhandled exception {e} in RSync thread", exc_info=True
                     )
@@ -246,15 +244,14 @@
                 # No transfer happening
                 if next_file is not None:
                     logger.warning(f"Invalid state {line=}, {next_file=}")
                     return
 
                 self._files_transferred += 1
                 if self._statusbar:
-                    logger.debug("Incrementing number of transferred files")
                     with self._statusbar.lock:
                         self._statusbar.transferred = [
                             self._statusbar.transferred[0] + 1,
                             self._statusbar.transferred[1],
                         ]
                 current_outstanding = self.queue.unfinished_tasks - (
                     self._files_transferred - previously_transferred
```

### Comparing `murfey-0.7.3/src/murfey/client/tui/app.py` & `murfey-0.7.5/src/murfey/client/tui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ProcessingForm,
     VisitSelection,
     determine_default_destination,
 )
 from murfey.client.tui.status_bar import StatusBar
 from murfey.client.watchdir import DirWatcher
 from murfey.client.watchdir_multigrid import MultigridDirWatcher
-from murfey.util import _get_visit_list
+from murfey.util import _get_visit_list, get_machine_config
 
 log = logging.getLogger("murfey.tui.app")
 
 ReactiveType = TypeVar("ReactiveType")
 
 
 class MurfeyTUI(App):
@@ -91,51 +91,70 @@
 
     @property
     def role(self) -> str:
         if self.analyser:
             return self.analyser._role
         return ""
 
-    def _launch_multigrid_watcher(self, source: Path):
+    def _launch_multigrid_watcher(
+        self, source: Path, destination_overrides: Dict[Path, str] | None = None
+    ):
         log.info(f"Launching multigrid watcher for source {source}")
         self._multigrid_watcher = MultigridDirWatcher(source)
-        self._multigrid_watcher.subscribe(self._start_rsyncer_multigrid)
+        self._multigrid_watcher.subscribe(
+            partial(
+                self._start_rsyncer_multigrid,
+                destination_overrides=destination_overrides or {},
+            )
+        )
         self._multigrid_watcher.start()
 
     def _start_rsyncer_multigrid(
         self,
         source: Path,
         extra_directory: str = "",
         include_mid_path: bool = True,
         use_suggested_path: bool = True,
+        destination_overrides: Dict[Path, str] | None = None,
     ):
+        log.info(f"starting multigrid rsyncer: {source}")
+        destination_overrides = destination_overrides or {}
         machine_data = requests.get(f"{self._environment.url.geturl()}/machine/").json()
-        self._environment.default_destinations[
-            source
-        ] = f"{machine_data.get('rsync_module') or 'data'}/{datetime.now().year}"
-        destination = determine_default_destination(
-            self._visit,
+        if destination_overrides.get(source):
+            destination = destination_overrides[source] + f"/{extra_directory}"
+        else:
+            self._environment.default_destinations[
+                source
+            ] = f"{machine_data.get('rsync_module') or 'data'}/{datetime.now().year}"
+            destination = determine_default_destination(
+                self._visit,
+                source,
+                self._default_destinations[source],
+                self._environment,
+                self.analysers,
+                touch=True,
+                extra_directory=extra_directory,
+                include_mid_path=include_mid_path,
+                use_suggested_path=use_suggested_path,
+            )
+        self._environment.sources.append(source)
+        self._start_rsyncer(
             source,
-            self._default_destinations[source],
-            self._environment,
-            self.analysers,
-            touch=True,
-            extra_directory=extra_directory,
-            include_mid_path=include_mid_path,
-            use_suggested_path=use_suggested_path,
+            destination,
+            force_metadata=True,
+            analyse=not extra_directory and use_suggested_path,
         )
-        self._environment.sources.append(source)
-        self._start_rsyncer(source, destination, force_metadata=True)
 
     def _start_rsyncer(
         self,
         source: Path,
         destination: str,
         visit_path: str = "",
         force_metadata: bool = False,
+        analyse: bool = True,
     ):
         log.info(f"starting rsyncer: {source}")
         if self._environment:
             self._environment.default_destinations[source] = destination
             if self._environment.gain_ref and visit_path:
                 gain_rsync = procrunner.run(
                     [
@@ -148,15 +167,15 @@
                     log.warning(
                         f"Gain reference file {self._environment.gain_ref} was not successfully transferred to {visit_path}/processing"
                     )
         self.rsync_processes[source] = RSyncer(
             source,
             basepath_remote=Path(destination),
             server_url=self._url,
-            local=self._environment.demo,
+            # local=self._environment.demo,
             status_bar=self._statusbar,
             do_transfer=self._do_transfer,
         )
 
         def rsync_result(update: RSyncerUpdate):
             if not update.base_path:
                 raise ValueError("No base path from rsyncer update")
@@ -170,15 +189,15 @@
             else:
                 log.warning(f"Failed to transfer file {str(update.file_path)!r}")
                 self.rsync_processes[update.base_path].enqueue(update.file_path)
 
         self.rsync_processes[source].subscribe(rsync_result)
         self._environment.watchers[source] = DirWatcher(source, settling_time=1)
 
-        if not self.analysers.get(source):
+        if not self.analysers.get(source) and analyse:
             log.info(f"Starting analyser for {source}")
             self.analysers[source] = Analyser(
                 source,
                 environment=self._environment if not self._dummy_dc else None,
                 force_mdoc_metadata=self._force_mdoc_metadata,
             )
             machine_data = requests.get(
@@ -279,19 +298,23 @@
                 "experiment_type": "tomo",
                 "experiment_type_id": 36,
                 "tag": str(source),
             }
             requests.post(url, json=dcg_data)
         elif isinstance(context, SPAContext):
             source = Path(json["source"])
+            machine_config = get_machine_config(
+                str(self._url.geturl()), demo=self._environment.demo
+            )
             url = f"{str(self._url.geturl())}/visits/{str(self._visit)}/start_data_collection"
             json = {
                 "tag": str(source.resolve()),
                 "image_directory": str(
-                    Path(self._environment.default_destinations[source]).resolve()
+                    Path(machine_config.get("rsync_basepath", "."))
+                    / self._environment.default_destinations[source]
                 ),
                 **json,
             }
             self._environment.listeners["data_collection_group_ids"] = {
                 partial(
                     context._register_data_collection,
                     url=url,
@@ -387,14 +410,16 @@
 
         if self.rsync_processes:
             for rp in self.rsync_processes.values():
                 rp.stop()
         if self.analysers:
             for a in self.analysers.values():
                 a.stop()
+        if self._multigrid_watcher:
+            self._multigrid_watcher.stop()
         self.exit()
         exit()
 
     async def action_clear(self) -> None:
         destination = ""
         if self.rsync_process:
             destination = (
```

### Comparing `murfey-0.7.3/src/murfey/client/tui/controller.css` & `murfey-0.7.5/src/murfey/client/tui/controller.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/tui/forms.py` & `murfey-0.7.5/src/murfey/client/tui/forms.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/tui/progress.py` & `murfey-0.7.5/src/murfey/client/tui/progress.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/tui/screens.py` & `murfey-0.7.5/src/murfey/client/tui/screens.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,17 +233,15 @@
         self.watch(self._dir_tree, "valid_selection", self._check_valid_selection)
         yield self._add_btn
         yield self._launch_btn
         yield Button("Quit", id="quit")
 
     def on_mount(self):
         if self._add_basepath:
-            self._add_directory(
-                str(self._selected_dir), add_destination=not self.app._multigrid
-            )
+            self._add_directory(str(self._selected_dir))
 
     def _check_valid_selection(self, valid: bool):
         if self._add_btn:
             if valid:
                 self._add_btn.disabled = False
             else:
                 self._add_btn.disabled = True
@@ -467,19 +465,43 @@
         self.app.push_screen("launcher")
 
 
 class DestinationSelect(Screen):
     def __init__(self, transfer_routes: Dict[Path, str], *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._transfer_routes = transfer_routes
+        self._destination_overrides: Dict[Path, str] = {}
         self._user_params: Dict[str, str] = {}
 
     def compose(self):
         bulk = []
-        if not self.app._multigrid:
+        if self.app._multigrid:
+            for s in self._transfer_routes.keys():
+                for d in s.glob("*"):
+                    if d.is_dir() and d.name != "atlas":
+                        machine_data = requests.get(
+                            f"{self.app._environment.url.geturl()}/machine/"
+                        ).json()
+                        dest = determine_default_destination(
+                            self.app._visit,
+                            s,
+                            f"{machine_data.get('rsync_module') or 'data'}/{datetime.now().year}",
+                            self.app._environment,
+                            self.app.analysers,
+                            touch=True,
+                        )
+                        bulk.append(Label(f"Copy the source {d} to:"))
+                        bulk.append(
+                            Input(
+                                value=dest,
+                                id=f"destination-{str(d)}",
+                                classes="input-destination",
+                            )
+                        )
+        else:
             for s, d in self._transfer_routes.items():
                 bulk.append(Label(f"Copy the source {s} to:"))
                 bulk.append(
                     Input(
                         value=d, id=f"destination-{str(s)}", classes="input-destination"
                     )
                 )
@@ -495,28 +517,35 @@
             *params_bulk,
             id="user-params",
         )
         yield Button("Confirm", id="destination-btn")
 
     def on_input_changed(self, event):
         if event.input.id.startswith("destination-"):
-            self._transfer_routes[Path(event.input.id[12:])] = event.value
+            if not self.app._multigrid:
+                self._transfer_routes[Path(event.input.id[12:])] = event.value
+            else:
+                self._destination_overrides[Path(event.input.id[12:])] = event.value
         else:
             for k in SPAContext.user_params:
                 if event.input.id == k.name:
                     self._user_params[k.name] = event.value
 
     def on_button_pressed(self, event):
-        if self.app._multigrid or any(v == "None" for v in self._user_params.values()):
+        if any(v == "None" for v in self._user_params.values()):
             return
         for s, d in self._transfer_routes.items():
             self.app._default_destinations[s] = d
             self.app._register_dc = True
             if self.app._multigrid:
-                self.app._launch_multigrid_watcher(s)
+                for k, v in self._destination_overrides.items():
+                    self.app._environment.destination_registry[k.name] = v
+                self.app._launch_multigrid_watcher(
+                    s, destination_overrides=self._destination_overrides
+                )
             else:
                 self.app._start_rsyncer(s, d)
         for k, v in self._user_params.items():
             self.app._environment.data_collection_parameters[k] = v
         if len(self._transfer_routes) > 1:
             requests.post(
                 f"{self.app._environment.url.geturl()}/visits/{self.app._environment.visit}/write_connections_file",
```

### Comparing `murfey-0.7.3/src/murfey/client/tui/status_bar.py` & `murfey-0.7.5/src/murfey/client/tui/status_bar.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/update.py` & `murfey-0.7.5/src/murfey/client/update.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/watchdir.py` & `murfey-0.7.5/src/murfey/client/watchdir.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/client/watchdir_multigrid.py` & `murfey-0.7.5/src/murfey/client/watchdir_multigrid.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,25 +29,36 @@
 
     def start(self):
         if self.thread.is_alive():
             raise RuntimeError("DirWatcher already running")
         log.info(f"MultigridDirWatcher thread starting for {self}")
         self.thread.start()
 
+    def stop(self):
+        log.debug("MultigridDirWatcher thread stop requested")
+        self._stopping = True
+        self._halt_thread = True
+        if self.thread.is_alive():
+            self.thread.join()
+        log.debug("MultigridDirWatcher thread stop completed")
+
     def _process(self):
         while not self._stopping:
             for d in self._basepath.glob("*"):
                 if d.name == "atlas":
                     if d.is_dir() and d not in self._seen_dirs:
                         self.notify(d, include_mid_path=False, use_suggested_path=False)
                         self._seen_dirs.append(d)
                 else:
                     if d.is_dir() and d not in self._seen_dirs:
                         self.notify(
                             d, extra_directory="metadata", include_mid_path=False
                         )
                         self._seen_dirs.append(d)
-                    d02 = d.parent.parent / d.name
+                    if (d.parent.parent / d.name / "Images-Disc1").is_dir():
+                        d02 = d.parent.parent / d.name / "Images-Disc1"
+                    else:
+                        d02 = d.parent.parent / d.name
                     if d02.is_dir() and d02 not in self._seen_dirs:
                         self.notify(d02)
                         self._seen_dirs.append(d02)
             time.sleep(15)
```

### Comparing `murfey-0.7.3/src/murfey/client/websocket.py` & `murfey-0.7.5/src/murfey/client/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/server/__init__.py` & `murfey-0.7.5/src/murfey/server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,20 @@
             imageDirectory=message["image_directory"],
             imageSuffix=message["image_suffix"],
             voltage=message["voltage"],
             dataCollectionGroupId=dcgid,
             pixelSizeOnImage=message["pixel_size"],
             imageSizeX=message["image_size_x"],
             imageSizeY=message["image_size_y"],
+            slitGapHorizontal=message.get("slit_width"),
+            magnification=message.get("magnification"),
+            exposureTime=message.get("exposure_time"),
+            totalExposedDose=message.get("total_exposed_dose"),
+            c2aperture=message.get("c2aperture"),
+            phasePlate=int(message.get("phase_plate", 0)),
         )
         dcid = _register(record, header, tag=message.get("tag"))
         if dcid is None and _transport_object:
             _transport_object.transport.nack(header)
             return None
         logger.debug(f"registered: {message.get('tag')}")
         if global_state.get("data_collection_ids") and isinstance(
```

### Comparing `murfey-0.7.3/src/murfey/server/api.py` & `murfey-0.7.5/src/murfey/server/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -399,25 +399,33 @@
         "session_id": murfey.server.ispyb.get_session_id(
             microscope=get_microscope(),
             proposal_code=ispyb_proposal_code,
             proposal_number=ispyb_proposal_number,
             visit_number=ispyb_visit_number,
             db=murfey.server.ispyb.Session(),
         ),
-        "image_directory": dc_params.image_directory,
+        "image_directory": str(
+            machine_config["rsync_basepath"] / dc_params.image_directory
+        ),
         "start_time": str(datetime.datetime.now()),
         "voltage": dc_params.voltage,
         "pixel_size": str(float(dc_params.pixel_size_on_image) * 1e9),
         "image_suffix": dc_params.file_extension,
         "experiment_type": dc_params.experiment_type,
         "image_size_x": dc_params.image_size_x,
         "image_size_y": dc_params.image_size_y,
         "acquisition_software": dc_params.acquisition_software,
         "tag": dc_params.tag,
         "source": dc_params.source,
+        "magnification": dc_params.magnification,
+        "total_exposed_dose": dc_params.total_exposed_dose,
+        "c2paerture": dc_params.c2aperture,
+        "exposure_time": dc_params.exposure_time,
+        "slit_width": dc_params.slit_width,
+        "phase_plate": dc_params.phase_plate,
     }
 
     if _transport_object:
         log.debug(
             f"Send registration message to {machine_config.feedback_queue}: {dc_parameters}"
         )
         _transport_object.send(
```

### Comparing `murfey-0.7.3/src/murfey/server/bootstrap.py` & `murfey-0.7.5/src/murfey/server/bootstrap.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/server/config.py` & `murfey-0.7.5/src/murfey/server/config.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/server/demo_api.py` & `murfey-0.7.5/src/murfey/server/demo_api.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/server/gain.py` & `murfey-0.7.5/src/murfey/server/gain.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/server/ispyb.py` & `murfey-0.7.5/src/murfey/server/ispyb.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,20 @@
                 exc_info=True,
             )
         return False
 
     def send(self, queue: str, message: dict):
         if self.transport:
             if not self.transport.is_connected():
+                try:
+                    self.transport.disconnect()
+                except AttributeError:
+                    # If there is not _pika_thread to join on the transport
+                    # then don't need to worry about dicsonnecting
+                    pass
                 self.transport.connect()
                 if self._connection_callback:
                     self._connection_callback()
             self.transport.send(queue, message)
 
     def do_insert_data_collection(self, record: DataCollection, message=None, **kwargs):
         comment = (
```

### Comparing `murfey-0.7.3/src/murfey/server/main.py` & `murfey-0.7.5/src/murfey/server/main.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/server/websocket.py` & `murfey-0.7.5/src/murfey/server/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/templates/activevisits.html` & `murfey-0.7.5/src/murfey/templates/activevisits.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/templates/base.html` & `murfey-0.7.5/src/murfey/templates/base.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/templates/bootstrap.html` & `murfey-0.7.5/src/murfey/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/templates/images/diamond.png` & `murfey-0.7.5/src/murfey/templates/images/diamond.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/templates/images/icon_268.png` & `murfey-0.7.5/src/murfey/templates/images/icon_268.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/templates/static/styles.css` & `murfey-0.7.5/src/murfey/templates/static/styles.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/templates/visit.html` & `murfey-0.7.5/src/murfey/templates/visit.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/util/__init__.py` & `murfey-0.7.5/src/murfey/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 import requests
 
 from murfey.util.models import Visit
 
 
 @lru_cache(maxsize=1)
 def get_machine_config(url: str, demo: bool = False) -> dict:
-    if demo:
-        return {}
     return requests.get(f"{url}/machine/").json()
 
 
 def _get_visit_list(api_base: ParseResult):
     get_visits_url = api_base._replace(path="/visits_raw")
     server_reply = requests.get(get_visits_url.geturl())
     if server_reply.status_code != 200:
```

### Comparing `murfey-0.7.3/src/murfey/util/dummy_setup.py` & `murfey-0.7.5/src/murfey/util/dummy_setup.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/util/file_monitor.py` & `murfey-0.7.5/src/murfey/util/file_monitor.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/util/mdoc.py` & `murfey-0.7.5/src/murfey/util/mdoc.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/util/models.py` & `murfey-0.7.5/src/murfey/util/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -90,14 +90,20 @@
     image_size_x: int
     image_size_y: int
     file_extension: str
     acquisition_software: str
     image_directory: str
     tag: str
     source: str
+    magnification: float
+    total_exposed_dose: Optional[float] = None
+    c2aperture: Optional[float] = None
+    exposure_time: Optional[float] = None
+    slit_width: Optional[float] = None
+    phase_plate: bool = False
 
 
 class DCParametersTomo(BaseModel):
     dose_per_frame: float
     gain_ref: Optional[str]
     experiment_type: str
     voltage: float
@@ -124,14 +130,20 @@
     use_cryolo: bool
     symmetry: str
     mask_diameter: int
     boxsize: int
     downscale: bool
     small_boxsize: int
     eer_grouping: int
+    magnification: Optional[int] = None
+    total_exposed_dose: Optional[float] = None
+    c2aperture: Optional[float] = None
+    exposure_time: Optional[float] = None
+    slit_width: Optional[float] = None
+    phase_plate: bool = False
 
 
 class ProcessingJobParameters(BaseModel):
     tag: str
     recipe: str
     parameters: Dict[str, Any] = {}
```

### Comparing `murfey-0.7.3/src/murfey/util/rsync.py` & `murfey-0.7.5/src/murfey/util/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey/util/state.py` & `murfey-0.7.5/src/murfey/util/state.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.3/src/murfey.egg-info/PKG-INFO` & `murfey-0.7.5/src/murfey.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.3
+Version: 0.7.5
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.3/src/murfey.egg-info/SOURCES.txt` & `murfey-0.7.5/src/murfey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

