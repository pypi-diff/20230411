# Comparing `tmp/swarm-to-sqlite-0.3.3.tar.gz` & `tmp/swarm-to-sqlite-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarm-to-sqlite-0.3.3.tar", last modified: Mon Jan 18 04:37:16 2021, max compression
+gzip compressed data, was "swarm-to-sqlite-0.3.4.tar", last modified: Tue Apr 11 03:18:58 2023, max compression
```

## Comparing `swarm-to-sqlite-0.3.3.tar` & `swarm-to-sqlite-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 04:37:16.659655 swarm-to-sqlite-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (116)     3396 2021-01-18 04:37:16.659655 swarm-to-sqlite-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2415 2021-01-18 04:37:07.000000 swarm-to-sqlite-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-18 04:37:16.659655 swarm-to-sqlite-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1159 2021-01-18 04:37:07.000000 swarm-to-sqlite-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 04:37:16.659655 swarm-to-sqlite-0.3.3/swarm_to_sqlite/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-18 04:37:07.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2420 2021-01-18 04:37:07.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     7526 2021-01-18 04:37:07.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-18 04:37:16.659655 swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3396 2021-01-18 04:37:16.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      330 2021-01-18 04:37:16.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-18 04:37:16.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2021-01-18 04:37:16.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2021-01-18 04:37:16.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-01-18 04:37:16.000000 swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:18:58.494458 swarm-to-sqlite-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 03:18:50.000000 swarm-to-sqlite-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 03:18:58.494458 swarm-to-sqlite-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 03:18:50.000000 swarm-to-sqlite-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 03:18:58.494458 swarm-to-sqlite-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-11 03:18:50.000000 swarm-to-sqlite-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:18:58.494458 swarm-to-sqlite-0.3.4/swarm_to_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:18:50.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-11 03:18:50.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-11 03:18:50.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:18:58.494458 swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 03:18:58.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 03:18:58.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:18:58.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-11 03:18:58.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 03:18:58.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:18:58.000000 swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/top_level.txt
```

### Comparing `swarm-to-sqlite-0.3.3/PKG-INFO` & `swarm-to-sqlite-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: swarm-to-sqlite
-Version: 0.3.3
+Version: 0.3.4
 Summary: Create a SQLite database containing your checkin history from Foursquare Swarm
 Home-page: https://github.com/dogsheep/swarm-to-sqlite
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/dogsheep/swarm-to-sqlite/issues
 Project-URL: CI, https://github.com/dogsheep/swarm-to-sqlite/actions
 Project-URL: Changelog, https://github.com/dogsheep/swarm-to-sqlite/releases
-Description: # swarm-to-sqlite
-        
-        [![PyPI](https://img.shields.io/pypi/v/swarm-to-sqlite.svg)](https://pypi.org/project/swarm-to-sqlite/)
-        [![Changelog](https://img.shields.io/github/v/release/dogsheep/swarm-to-sqlite?include_prereleases&label=changelog)](https://github.com/dogsheep/swarm-to-sqlite/releases)
-        [![Tests](https://github.com/dogsheep/swarm-to-sqlite/workflows/Test/badge.svg)](https://github.com/dogsheep/swarm-to-sqlite/actions?query=workflow%3ATest)
-        [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dogsheep/swarm-to-sqlite/blob/main/LICENSE)
-        
-        Create a SQLite database containing your checkin history from Foursquare Swarm.
-        
-        ## How to install
-        
-            $ pip install swarm-to-sqlite
-        
-        ## Usage
-        
-        You will need to first obtain a valid OAuth token for your Foursquare account. You can do so using this tool: https://your-foursquare-oauth-token.glitch.me/
-        
-        Simplest usage is to simply provide the name of the database file you wish to write to. The tool will prompt you to paste in your token, and will then download your checkins and store them in the specified database file.
-        
-            $ swarm-to-sqlite checkins.db
-            Please provide your Foursquare OAuth token:
-            Importing 3699 checkins  [#########-----------------------] 27% 00:02:31
-        
-        You can also pass the token as a command-line option:
-        
-            $ swarm-to-sqlite checkins.db --token=XXX
-        
-        Or as an environment variable:
-        
-            $ export FOURSQUARE_TOKEN=XXX
-            $ swarm-to-sqlite checkins.db
-        
-        To retrieve just checkins within the past X hours, days or weeks, use the `--since=` option. For example, to pull only checkins that happened within the last 10 days use:
-        
-            $ swarm-to-sqlite checkins.db --token=XXX --since=10d
-        
-        Use `2w` for two weeks, `10h` for ten hours, `3d` for three days.
-        
-        In addition to saving the checkins to a database, you can also write them to a JSON file using the `--save` option:
-        
-            $ swarm-to-sqlite checkins.db --save=checkins.json
-        
-        Having done this, you can re-import checkins directly from that file (rather than making API calls to fetch data from Foursquare) like this:
-        
-            $ swarm-to-sqlite checkins.db --load=checkins.json
-        
-        ## Using with Datasette
-        
-        The SQLite database produced by this tool is designed to be browsed using [Datasette](https://datasette.io/).
-        
-        You can install the [datasette-cluster-map](https://datasette.io/plugins/datasette-cluster-map) plugin to view your checkins on a map.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# swarm-to-sqlite
+
+[![PyPI](https://img.shields.io/pypi/v/swarm-to-sqlite.svg)](https://pypi.org/project/swarm-to-sqlite/)
+[![Changelog](https://img.shields.io/github/v/release/dogsheep/swarm-to-sqlite?include_prereleases&label=changelog)](https://github.com/dogsheep/swarm-to-sqlite/releases)
+[![Tests](https://github.com/dogsheep/swarm-to-sqlite/workflows/Test/badge.svg)](https://github.com/dogsheep/swarm-to-sqlite/actions?query=workflow%3ATest)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dogsheep/swarm-to-sqlite/blob/main/LICENSE)
+
+Create a SQLite database containing your checkin history from Foursquare Swarm.
+
+## How to install
+
+    $ pip install swarm-to-sqlite
+
+## Usage
+
+You will need to first obtain a valid OAuth token for your Foursquare account. You can do so using this tool: https://your-foursquare-oauth-token.glitch.me/
+
+Simplest usage is to simply provide the name of the database file you wish to write to. The tool will prompt you to paste in your token, and will then download your checkins and store them in the specified database file.
+
+    $ swarm-to-sqlite checkins.db
+    Please provide your Foursquare OAuth token:
+    Importing 3699 checkins  [#########-----------------------] 27% 00:02:31
+
+You can also pass the token as a command-line option:
+
+    $ swarm-to-sqlite checkins.db --token=XXX
+
+Or as an environment variable:
+
+    $ export FOURSQUARE_TOKEN=XXX
+    $ swarm-to-sqlite checkins.db
+
+To retrieve just checkins within the past X hours, days or weeks, use the `--since=` option. For example, to pull only checkins that happened within the last 10 days use:
+
+    $ swarm-to-sqlite checkins.db --token=XXX --since=10d
+
+Use `2w` for two weeks, `10h` for ten hours, `3d` for three days.
+
+In addition to saving the checkins to a database, you can also write them to a JSON file using the `--save` option:
+
+    $ swarm-to-sqlite checkins.db --save=checkins.json
+
+Having done this, you can re-import checkins directly from that file (rather than making API calls to fetch data from Foursquare) like this:
+
+    $ swarm-to-sqlite checkins.db --load=checkins.json
+
+## Using with Datasette
+
+The SQLite database produced by this tool is designed to be browsed using [Datasette](https://datasette.io/).
+
+You can install the [datasette-cluster-map](https://datasette.io/plugins/datasette-cluster-map) plugin to view your checkins on a map.
```

### Comparing `swarm-to-sqlite-0.3.3/README.md` & `swarm-to-sqlite-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `swarm-to-sqlite-0.3.3/setup.py` & `swarm-to-sqlite-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.3"
+VERSION = "0.3.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `swarm-to-sqlite-0.3.3/swarm_to_sqlite/cli.py` & `swarm-to-sqlite-0.3.4/swarm_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `swarm-to-sqlite-0.3.3/swarm_to_sqlite/utils.py` & `swarm-to-sqlite-0.3.4/swarm_to_sqlite/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,35 +166,35 @@
         """,
         ),
         (
             "checkin_details",
             """
 select
     checkins.id,
-    created,
+    strftime('%Y-%m-%dT%H:%M:%S', checkins.createdAt, 'unixepoch') as created,
     venues.id as venue_id,
     venues.name as venue_name,
     venues.latitude,
     venues.longitude,
     group_concat(categories.name) as venue_categories,
-    shout,
-    createdBy,
+    checkins.shout,
+    checkins.createdBy,
     events.name as event_name
 from checkins
     join venues on checkins.venue = venues.id
     left join events on checkins.event = events.id
     join categories_venues on venues.id = categories_venues.venues_id
     join categories on categories.id = categories_venues.categories_id
 group by checkins.id
-order by createdAt desc
+order by checkins.createdAt desc
         """,
         ),
     ):
         try:
-            db.create_view(name, sql)
+            db.create_view(name, sql, replace=True)
         except Exception:
             pass
 
 
 def fetch_all_checkins(token, count_first=False, since_delta=None):
     # Generator that yields all checkins using the provided OAuth token
     # If count_first is True it first yields the total checkins count
```

### Comparing `swarm-to-sqlite-0.3.3/swarm_to_sqlite.egg-info/PKG-INFO` & `swarm-to-sqlite-0.3.4/swarm_to_sqlite.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: swarm-to-sqlite
-Version: 0.3.3
+Version: 0.3.4
 Summary: Create a SQLite database containing your checkin history from Foursquare Swarm
 Home-page: https://github.com/dogsheep/swarm-to-sqlite
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/dogsheep/swarm-to-sqlite/issues
 Project-URL: CI, https://github.com/dogsheep/swarm-to-sqlite/actions
 Project-URL: Changelog, https://github.com/dogsheep/swarm-to-sqlite/releases
-Description: # swarm-to-sqlite
-        
-        [![PyPI](https://img.shields.io/pypi/v/swarm-to-sqlite.svg)](https://pypi.org/project/swarm-to-sqlite/)
-        [![Changelog](https://img.shields.io/github/v/release/dogsheep/swarm-to-sqlite?include_prereleases&label=changelog)](https://github.com/dogsheep/swarm-to-sqlite/releases)
-        [![Tests](https://github.com/dogsheep/swarm-to-sqlite/workflows/Test/badge.svg)](https://github.com/dogsheep/swarm-to-sqlite/actions?query=workflow%3ATest)
-        [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dogsheep/swarm-to-sqlite/blob/main/LICENSE)
-        
-        Create a SQLite database containing your checkin history from Foursquare Swarm.
-        
-        ## How to install
-        
-            $ pip install swarm-to-sqlite
-        
-        ## Usage
-        
-        You will need to first obtain a valid OAuth token for your Foursquare account. You can do so using this tool: https://your-foursquare-oauth-token.glitch.me/
-        
-        Simplest usage is to simply provide the name of the database file you wish to write to. The tool will prompt you to paste in your token, and will then download your checkins and store them in the specified database file.
-        
-            $ swarm-to-sqlite checkins.db
-            Please provide your Foursquare OAuth token:
-            Importing 3699 checkins  [#########-----------------------] 27% 00:02:31
-        
-        You can also pass the token as a command-line option:
-        
-            $ swarm-to-sqlite checkins.db --token=XXX
-        
-        Or as an environment variable:
-        
-            $ export FOURSQUARE_TOKEN=XXX
-            $ swarm-to-sqlite checkins.db
-        
-        To retrieve just checkins within the past X hours, days or weeks, use the `--since=` option. For example, to pull only checkins that happened within the last 10 days use:
-        
-            $ swarm-to-sqlite checkins.db --token=XXX --since=10d
-        
-        Use `2w` for two weeks, `10h` for ten hours, `3d` for three days.
-        
-        In addition to saving the checkins to a database, you can also write them to a JSON file using the `--save` option:
-        
-            $ swarm-to-sqlite checkins.db --save=checkins.json
-        
-        Having done this, you can re-import checkins directly from that file (rather than making API calls to fetch data from Foursquare) like this:
-        
-            $ swarm-to-sqlite checkins.db --load=checkins.json
-        
-        ## Using with Datasette
-        
-        The SQLite database produced by this tool is designed to be browsed using [Datasette](https://datasette.io/).
-        
-        You can install the [datasette-cluster-map](https://datasette.io/plugins/datasette-cluster-map) plugin to view your checkins on a map.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# swarm-to-sqlite
+
+[![PyPI](https://img.shields.io/pypi/v/swarm-to-sqlite.svg)](https://pypi.org/project/swarm-to-sqlite/)
+[![Changelog](https://img.shields.io/github/v/release/dogsheep/swarm-to-sqlite?include_prereleases&label=changelog)](https://github.com/dogsheep/swarm-to-sqlite/releases)
+[![Tests](https://github.com/dogsheep/swarm-to-sqlite/workflows/Test/badge.svg)](https://github.com/dogsheep/swarm-to-sqlite/actions?query=workflow%3ATest)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dogsheep/swarm-to-sqlite/blob/main/LICENSE)
+
+Create a SQLite database containing your checkin history from Foursquare Swarm.
+
+## How to install
+
+    $ pip install swarm-to-sqlite
+
+## Usage
+
+You will need to first obtain a valid OAuth token for your Foursquare account. You can do so using this tool: https://your-foursquare-oauth-token.glitch.me/
+
+Simplest usage is to simply provide the name of the database file you wish to write to. The tool will prompt you to paste in your token, and will then download your checkins and store them in the specified database file.
+
+    $ swarm-to-sqlite checkins.db
+    Please provide your Foursquare OAuth token:
+    Importing 3699 checkins  [#########-----------------------] 27% 00:02:31
+
+You can also pass the token as a command-line option:
+
+    $ swarm-to-sqlite checkins.db --token=XXX
+
+Or as an environment variable:
+
+    $ export FOURSQUARE_TOKEN=XXX
+    $ swarm-to-sqlite checkins.db
+
+To retrieve just checkins within the past X hours, days or weeks, use the `--since=` option. For example, to pull only checkins that happened within the last 10 days use:
+
+    $ swarm-to-sqlite checkins.db --token=XXX --since=10d
+
+Use `2w` for two weeks, `10h` for ten hours, `3d` for three days.
+
+In addition to saving the checkins to a database, you can also write them to a JSON file using the `--save` option:
+
+    $ swarm-to-sqlite checkins.db --save=checkins.json
+
+Having done this, you can re-import checkins directly from that file (rather than making API calls to fetch data from Foursquare) like this:
+
+    $ swarm-to-sqlite checkins.db --load=checkins.json
+
+## Using with Datasette
+
+The SQLite database produced by this tool is designed to be browsed using [Datasette](https://datasette.io/).
+
+You can install the [datasette-cluster-map](https://datasette.io/plugins/datasette-cluster-map) plugin to view your checkins on a map.
```

