# Comparing `tmp/pywmataio-0.0.7.tar.gz` & `tmp/pywmataio-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywmataio-0.0.7.tar", last modified: Sun Apr  2 18:10:58 2023, max compression
+gzip compressed data, was "pywmataio-0.0.8.tar", last modified: Tue Apr 11 04:18:58 2023, max compression
```

## Comparing `pywmataio-0.0.7.tar` & `pywmataio-0.0.8.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.405183 pywmataio-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-02 18:10:54.000000 pywmataio-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-02 18:10:58.405183 pywmataio-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-02 18:10:54.000000 pywmataio-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.393183 pywmataio-0.0.7/pywmataio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-02 18:10:58.000000 pywmataio-0.0.7/pywmataio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-02 18:10:58.000000 pywmataio-0.0.7/pywmataio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 18:10:58.000000 pywmataio-0.0.7/pywmataio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-02 18:10:58.000000 pywmataio-0.0.7/pywmataio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-02 18:10:58.000000 pywmataio-0.0.7/pywmataio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-02 18:10:58.405183 pywmataio-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-02 18:10:54.000000 pywmataio-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.393183 pywmataio-0.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-02 18:10:54.000000 pywmataio-0.0.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-02 18:10:54.000000 pywmataio-0.0.7/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-02 18:10:54.000000 pywmataio-0.0.7/test/test_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-04-02 18:10:54.000000 pywmataio-0.0.7/test/test_rail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.393183 pywmataio-0.0.7/wmataio/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.397183 pywmataio-0.0.7/wmataio/bus/
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.397183 pywmataio-0.0.7/wmataio/bus/models/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/bus_incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/live_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/next_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/route_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/route_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/bus/models/stop_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.397183 pywmataio-0.0.7/wmataio/models/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/models/area.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/models/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.401183 pywmataio-0.0.7/wmataio/rail/
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:10:58.405183 pywmataio-0.0.7/wmataio/rail/models/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/elevator_and_escalator_incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/live_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/next_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/rail_incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/standard_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/station.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/station_entrance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/station_parking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/station_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/station_to_station.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-02 18:10:54.000000 pywmataio-0.0.7/wmataio/rail/models/track_circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 04:18:55.000000 pywmataio-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-11 04:18:58.388287 pywmataio-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 04:18:55.000000 pywmataio-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.384287 pywmataio-0.0.8/pywmataio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-11 04:18:58.000000 pywmataio-0.0.8/pywmataio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-11 04:18:58.000000 pywmataio-0.0.8/pywmataio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 04:18:58.000000 pywmataio-0.0.8/pywmataio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 04:18:58.000000 pywmataio-0.0.8/pywmataio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 04:18:58.000000 pywmataio-0.0.8/pywmataio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-11 04:18:58.388287 pywmataio-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 04:18:55.000000 pywmataio-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.384287 pywmataio-0.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 04:18:55.000000 pywmataio-0.0.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-11 04:18:55.000000 pywmataio-0.0.8/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 04:18:55.000000 pywmataio-0.0.8/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-11 04:18:55.000000 pywmataio-0.0.8/test/models/test_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-11 04:18:55.000000 pywmataio-0.0.8/test/models/test_rail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 04:18:55.000000 pywmataio-0.0.8/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/wmataio/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/wmataio/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/wmataio/bus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/bus_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/live_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/next_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/route_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/route_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/models/stop_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/bus/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/wmataio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/models/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/models/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/wmataio/rail/
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:18:58.388287 pywmataio-0.0.8/wmataio/rail/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/elevator_and_escalator_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/live_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/next_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/rail_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/standard_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/station_entrance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/station_parking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/station_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/station_to_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/rail/models/track_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-11 04:18:55.000000 pywmataio-0.0.8/wmataio/util.py
```

### Comparing `pywmataio-0.0.7/LICENSE` & `pywmataio-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywmataio-0.0.7/PKG-INFO` & `pywmataio-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywmataio
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple async interface to the WMATA (Washington, DC Public Transit) API
 Home-page: https://github.com/raman325/pywmataio
 Author: Raman
 Author-email: 7243222+raman325@users.noreply.github.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `pywmataio-0.0.7/README.md` & `pywmataio-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pywmataio-0.0.7/pywmataio.egg-info/PKG-INFO` & `pywmataio-0.0.8/pywmataio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywmataio
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple async interface to the WMATA (Washington, DC Public Transit) API
 Home-page: https://github.com/raman325/pywmataio
 Author: Raman
 Author-email: 7243222+raman325@users.noreply.github.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `pywmataio-0.0.7/pywmataio.egg-info/SOURCES.txt` & `pywmataio-0.0.8/pywmataio.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 pywmataio.egg-info/PKG-INFO
 pywmataio.egg-info/SOURCES.txt
 pywmataio.egg-info/dependency_links.txt
 pywmataio.egg-info/requires.txt
 pywmataio.egg-info/top_level.txt
 test/__init__.py
 test/conftest.py
-test/test_bus.py
-test/test_rail.py
+test/test_util.py
+test/models/__init__.py
+test/models/test_bus.py
+test/models/test_rail.py
 wmataio/__init__.py
 wmataio/client.py
 wmataio/const.py
 wmataio/exceptions.py
+wmataio/util.py
 wmataio/bus/__init__.py
 wmataio/bus/const.py
+wmataio/bus/util.py
 wmataio/bus/models/__init__.py
 wmataio/bus/models/bus_incident.py
 wmataio/bus/models/live_position.py
 wmataio/bus/models/next_bus.py
 wmataio/bus/models/route.py
 wmataio/bus/models/route_path.py
 wmataio/bus/models/route_schedule.py
```

### Comparing `pywmataio-0.0.7/setup.cfg` & `pywmataio-0.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.7
+current_version = 0.0.8
 commit = True
 tag = True
 tag_name = {new_version}
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pywmataio-0.0.7/setup.py` & `pywmataio-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pywmataio",
-    version="0.0.7",
+    version="0.0.8",
     author="Raman",
     author_email="7243222+raman325@users.noreply.github.com",
     description="A simple async interface to the WMATA (Washington, DC Public Transit) API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raman325/pywmataio",
     packages=setuptools.find_packages(),
```

### Comparing `pywmataio-0.0.7/test/conftest.py` & `pywmataio-0.0.8/test/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,36 +4,52 @@
 import pathlib
 import re
 
 import pytest
 from aioresponses import CallbackResult, aioresponses
 
 from wmataio.bus.const import BusEndpoint
-from wmataio.const import ADDITIONAL_PATH_HEADER, CLASS_HEADER, ENUM_HEADER
+from wmataio.const import (
+    ADDITIONAL_PATH_HEADER,
+    BASE_WMATA_URL,
+    CLASS_HEADER,
+    ENUM_HEADER,
+    GEOCODE_URL,
+)
 from wmataio.rail.const import RailEndpoint
 
-CLASS_MAP = {
+_LOGGER = logging.getLogger(__name__)
+
+WMATA_MODEL_CLASS_MAP = {
     BusEndpoint.__name__: {"class": BusEndpoint, "api_type": "bus"},
     RailEndpoint.__name__: {"class": RailEndpoint, "api_type": "rail"},
 }
 
 
-_LOGGER = logging.getLogger(__name__)
-API_REGEX = re.compile(r"https:\/\/api\.wmata\.com.*$")
+def _process_fixture_path_as_result(path: pathlib.Path) -> CallbackResult:
+    """Process fixture data and return callback result."""
+    if not path.exists():
+        _LOGGER.error("Fixture %s does not exist", path)
+        return CallbackResult(status=404)
+
+    with open(path, "r") as fp:
+        data = json.load(fp)
+
+    return CallbackResult(status=200, payload=data)
 
 
-def _callback(url: str, **kwargs) -> CallbackResult:
+def _wmata_callback(url: str, **kwargs) -> CallbackResult:
     """Respond to WMATA API calls."""
     _LOGGER.debug("Received request for %s", url)
     params = kwargs.get("params")
     headers = kwargs["headers"]
     class_name = headers[CLASS_HEADER]
     enum_name = headers[ENUM_HEADER]
     additional_path = headers[ADDITIONAL_PATH_HEADER]
-    cls_data = CLASS_MAP[class_name]
+    cls_data = WMATA_MODEL_CLASS_MAP[class_name]
     enum_: BusEndpoint | RailEndpoint = cls_data["class"][enum_name]
     api_type = cls_data["api_type"]
 
     base_fixture_name = enum_.name.lower()
 
     additional_path_fixture_name = ""
     if additional_path:
@@ -45,25 +61,35 @@
 
     fixture_name = base_fixture_name
     if additional_path_fixture_name or params_fixture_name:
         fixture_name = ".".join(
             [base_fixture_name, additional_path_fixture_name, params_fixture_name]
         )
 
-    path = pathlib.Path(f"test/fixtures/{api_type}/{fixture_name}.json")
+    return _process_fixture_path_as_result(
+        pathlib.Path(f"test/fixtures/models/{api_type}/{fixture_name}.json")
+    )
 
-    if not path.exists():
-        _LOGGER.error("Fixture %s does not exist", path)
-        return CallbackResult(status=404)
 
-    with open(path, "r") as fp:
-        data = json.load(fp)
+@pytest.fixture(name="wmata_responses", scope="module")
+def mock_wmata_responses():
+    """Mock aiohttp response from WMATA API."""
+    with aioresponses() as m:
+        m.get(re.compile(f"{BASE_WMATA_URL}.*$"), callback=_wmata_callback, repeat=True)
+        yield m
 
-    return CallbackResult(status=200, payload=data)
+
+def _geocode_callback(url: str, **kwargs) -> CallbackResult:
+    """Respond to Geocode API calls."""
+    _LOGGER.debug("Received request for %s", url)
+    address = kwargs["params"]["address"]
+    return _process_fixture_path_as_result(
+        pathlib.Path(f"test/fixtures/util/geocode/{address}.json")
+    )
 
 
-@pytest.fixture(name="aioresponses", scope="session")
-def mock_aioresponse():
-    """Mock aiohttp responses."""
+@pytest.fixture(name="geocode_responses", scope="module")
+def mock_geocode_responses():
+    """Mock aiohttp responses from geocode_service."""
     with aioresponses() as m:
-        m.get(API_REGEX, callback=_callback, repeat=True)
+        m.get(re.compile(f"{GEOCODE_URL}.*$"), callback=_geocode_callback, repeat=True)
         yield m
```

### Comparing `pywmataio-0.0.7/test/test_bus.py` & `pywmataio-0.0.8/test/models/test_bus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 """Test pywmataio client for buses."""
 from datetime import date, datetime
 
+from wmataio.bus.util import find_direct_route_start_end_stop_pairs
 from wmataio.client import Client
 from wmataio.const import TZ
 from wmataio.models.area import Area
 
 
-async def test_bus_apis(aioresponses):
+async def test_bus_apis(wmata_responses):
     """Callback for aioresponse."""
     client = Client("", test_mode=True)
     await client.bus.load_data()
     assert client.bus.routes
     assert client.bus.stops
 
     assert len(client.bus.routes) == 390
 
     route = client.bus.routes["10A"]
     assert route.route_id == "10A"
     assert route.name == "10A - HUNTINGTON STA - PENTAGON"
     assert route.line_description == "Alexandria-Pentagon Line"
-    assert str(route) == "Route(id=10A, name=10A - HUNTINGTON STA - PENTAGON)"
     assert hash(route) == hash("10A")
 
     assert len(client.bus.stops) == 9360
 
     stop = client.bus.stops["3000454"]
     assert stop.coordinates.latitude == 38.820495
     assert stop.coordinates.longitude == -76.957391
     assert stop.name == "ST BARNABAS RD + LIME ST"
     assert stop.route_ids == ["D12", "D12*5"]
-    assert stop.routes == [client.bus.routes["D12"], client.bus.routes["D12*5"]]
-    assert str(stop) == "Stop(code=3000454, name=ST BARNABAS RD + LIME ST)"
+    assert stop.routes == {client.bus.routes["D12"], client.bus.routes["D12*5"]}
     assert hash(stop) == hash("3000454")
 
     positions = await client.bus.get_live_positions(route=client.bus.routes["10A"])
     assert positions
     assert len(positions) == 4
 
     positions = await client.bus.get_live_positions(
@@ -83,17 +82,17 @@
     assert route_path
 
     route_path = await client.bus.get_route_path(route=client.bus.routes["10A"])
     assert route_path
     assert route_path.route_id == "10A"
     assert route_path.route == client.bus.routes["10A"]
     assert route_path.name == "10A - PENTAGON - HUNTINGTON STA"
-    assert len(route_path.directions) == 2
-    assert route_path.directions[1]
-    direction = route_path.directions[0]
+    assert len(route_path.path_directions) == 2
+    assert route_path.path_directions[1]
+    direction = route_path.path_directions[0]
     assert direction.trip_headsign == "PENTAGON"
     assert direction.direction == "NORTH"
     assert direction.direction_num == 0
     assert len(direction.shapes) == 184
     shape = direction.shapes[0]
     assert shape.coordinates.latitude == 38.79524
     assert shape.coordinates.longitude == -77.075059
@@ -101,15 +100,15 @@
     assert len(direction.stops) == 57
     stop = direction.stops[0]
     assert stop.stop_id == "5002201"
     assert stop.name == "HUNTINGTON STATION (N) + BUS BAY B"
     assert stop.coordinates.latitude == 38.79524
     assert stop.coordinates.longitude == -77.075059
     assert stop.route_ids == ["10A"]
-    assert stop.routes == [client.bus.routes["10A"]]
+    assert stop.routes == {client.bus.routes["10A"]}
 
     route_schedule = await client.bus.get_route_schedule(
         route=client.bus.routes["10A"], date_=date(2023, 3, 31)
     )
     assert route_schedule
 
     route_schedule = await client.bus.get_route_schedule(route=client.bus.routes["10A"])
@@ -162,7 +161,23 @@
     assert stop_arrival.trip_direction_text == "EAST"
     assert stop_arrival.trip_headsign == "CAPITOL HEIGHTS STATION"
     assert stop_arrival.trip_id == "3944060"
     assert stop_arrival.direction_number == 0
     assert stop_arrival.schedule_time == datetime(2023, 3, 31, 4, 53, 28, tzinfo=TZ)
     assert stop_arrival.start_time == datetime(2023, 3, 31, 4, 47, tzinfo=TZ)
     assert stop_arrival.end_time == datetime(2023, 3, 31, 5, 24, tzinfo=TZ)
+
+
+async def test_bus_utils(wmata_responses):
+    """Tests for MetroBus utility functions."""
+    client = Client("", test_mode=True)
+    await client.bus.load_data()
+    stop_1 = client.bus.stops["5002201"]
+    stop_2 = client.bus.stops["4000025"]
+    data = await find_direct_route_start_end_stop_pairs(
+        client, {stop_1, stop_2}, {stop_1, stop_2}
+    )
+    assert len(data) == 1
+    assert len(data[(stop_1, stop_2)]) == 1
+    assert next(direction for direction in data[(stop_1, stop_2)]).direction == "NORTH"
+
+    assert (stop_2, stop_1) not in data
```

### Comparing `pywmataio-0.0.7/test/test_rail.py` & `pywmataio-0.0.8/test/models/test_rail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import date, datetime, time
 
 from wmataio.client import Client
 from wmataio.const import TZ
 from wmataio.rail.models.live_position import TrainDirection
 
 
-async def test_rail_apis(aioresponses):
+async def test_rail_apis(wmata_responses):
     """Callback for aioresponse."""
     client = Client("", test_mode=True)
     await client.rail.load_data()
     assert client.rail.lines
     assert client.rail.stations
 
     assert len(client.rail.lines) == 6
@@ -21,15 +21,14 @@
     assert line.start_station == client.rail.stations["J03"]
     assert line.end_station_code == "G05"
     assert line.end_station == client.rail.stations["G05"]
     assert line.internal_destination_code_1 is None
     assert line.internal_destination_1 is None
     assert line.internal_destination_code_2 is None
     assert line.internal_destination_2 is None
-    assert str(line) == "Line(code=BL, name=Blue)"
     assert hash(line) == hash("BL")
 
     assert len(line.standard_routes) == 2
     standard_route = line.standard_routes[0]
     assert standard_route.line_code == "BL"
     assert standard_route.line == line
     assert standard_route.track_number == 1
@@ -56,15 +55,14 @@
     assert station.address.street == "607 13th St. NW"
     assert station.address.city == "Washington"
     assert station.address.state == "DC"
     assert station.address.zip_code == "20005"
     assert len(station.entrances) == 8
     assert len(station.station_times) == 1
     assert station.parking is None
-    assert str(station) == "Station(code=A01, name=Metro Center)"
     assert hash(station) == hash("A01")
 
     entrance = station.entrances[0]
     assert entrance.entrance_id == "273"
     assert entrance.name == "11TH ST NW & G ST NW"
     assert entrance.station_code_1 == "A01"
     assert entrance.station_1 == client.rail.stations["A01"]
```

### Comparing `pywmataio-0.0.7/wmataio/bus/__init__.py` & `pywmataio-0.0.8/wmataio/bus/__init__.py`

 * *Files identical despite different names*

### Comparing `pywmataio-0.0.7/wmataio/bus/models/bus_incident.py` & `pywmataio-0.0.8/wmataio/bus/models/bus_incident.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     RoutesAffected: list[str]
 
 
 @dataclass
 class BusIncident:
     """MetroBus Incident."""
 
-    bus: "MetroBus"
-    data: BusIncidentData
+    bus: "MetroBus" = field(repr=False)
+    data: BusIncidentData = field(repr=False)
     date_updated: datetime = field(init=False)
     description: str = field(init=False)
     incident_id: str = field(init=False)
     incident_type: str = field(init=False)
     route_ids_affected: list[str] = field(init=False)
 
     def __post_init__(self) -> None:
@@ -40,11 +40,15 @@
             tzinfo=TZ
         )
         self.description = self.data["Description"]
         self.incident_type = self.data["IncidentType"]
         self.incident_id = self.data["IncidentID"]
         self.route_ids_affected = self.data["RoutesAffected"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.incident_id)
+
     @property
     def routes_affected(self) -> list["Route"]:
         """Return routes affected by this incident."""
         return [self.bus.routes[route_id] for route_id in self.route_ids_affected]
```

### Comparing `pywmataio-0.0.7/wmataio/bus/models/live_position.py` & `pywmataio-0.0.8/wmataio/bus/models/live_position.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     BlockNumber: str
 
 
 @dataclass
 class LiveBusPosition:
     """A MetroBus Bus LiveBusPosition."""
 
-    bus: "MetroBus"
-    data: LiveBusPositionData
+    bus: "MetroBus" = field(repr=False)
+    data: LiveBusPositionData = field(repr=False)
     last_update: datetime = field(init=False)
     deviation: float = field(init=False)
     direction_text: str = field(init=False)
     coordinates: Coordinates = field(init=False)
     route_id: str = field(init=False)
     trip_end_time: datetime = field(init=False)
     trip_headsign: str = field(init=False)
@@ -63,11 +63,15 @@
         self.trip_headsign = self.data["TripHeadsign"]
         self.trip_id = self.data["TripID"]
         self.trip_start_time = datetime.fromisoformat(
             self.data["TripStartTime"]
         ).replace(tzinfo=TZ)
         self.vehicle_id = self.data["VehicleID"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.vehicle_id, self.trip_id))
+
     @property
     def route(self) -> "Route":
         """Get route."""
         return self.bus.routes[self.route_id]
```

### Comparing `pywmataio-0.0.7/wmataio/bus/models/next_bus.py` & `pywmataio-0.0.8/wmataio/bus/models/next_bus.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     VehicleID: str
 
 
 @dataclass
 class NextBus:
     """Next bus for a Stop."""
 
-    bus: "MetroBus"
-    data: NextBusData
+    bus: "MetroBus" = field(repr=False)
+    data: NextBusData = field(repr=False)
     direction_number: int = field(init=False)
     direction_text: str = field(init=False)
     minutes: int = field(init=False)
     route_id: str = field(init=False)
     trip_id: str = field(init=False)
     vehicle_id: str = field(init=False)
 
@@ -38,11 +38,15 @@
         self.direction_number = int(self.data["DirectionNum"])
         self.direction_text = self.data["DirectionText"]
         self.minutes = self.data["Minutes"]
         self.route_id = self.data["RouteID"]
         self.trip_id = self.data["TripID"]
         self.vehicle_id = self.data["VehicleID"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.vehicle_id, self.trip_id, self.route, self.direction_number))
+
     @property
     def route(self) -> "Route":
         """Return the route."""
         return self.bus.routes[self.route_id]
```

### Comparing `pywmataio-0.0.7/wmataio/bus/models/route.py` & `pywmataio-0.0.8/wmataio/bus/models/route.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,30 +6,25 @@
 
 
 class RouteData(TypedDict):
     """Route data for MetroBus API."""
 
     RouteID: str
     Name: str
-    LineDescription: list[str]
+    LineDescription: str
 
 
 @dataclass
 class Route:
     """A MetroBus Route."""
 
-    data: RouteData
+    data: RouteData = field(repr=False)
     route_id: str = field(init=False)
     name: str = field(init=False)
-    line_description: list[str] = field(init=False)
-
-    def __repr__(self) -> str:
-        """Return the representation."""
-        cls_name = type(self).__name__
-        return f"{cls_name}(id={self.route_id}, name={self.name})"
+    line_description: str = field(init=False)
 
     def __hash__(self) -> int:
         """Return the hash."""
         return hash(self.route_id)
 
     def __post_init__(self) -> None:
         """Post init."""
```

### Comparing `pywmataio-0.0.7/wmataio/bus/models/route_path.py` & `pywmataio-0.0.8/wmataio/bus/models/route_path.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,61 +20,70 @@
     SeqNum: str
 
 
 @dataclass
 class ShapePoint:
     """ShapePoint for a Path."""
 
-    data: ShapePointData
+    data: ShapePointData = field(repr=False)
     coordinates: Coordinates = field(init=False)
     sequence_number: int = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.coordinates = Coordinates(float(self.data["Lat"]), float(self.data["Lon"]))
         self.sequence_number = int(self.data["SeqNum"])
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.coordinates, self.sequence_number))
+
 
 class PathDirectionData(TypedDict):
     """Direction data for MetroBus WMATA API."""
 
     DirectionNum: int  # deprecated
     DirectionText: str
     Shape: list[ShapePointData]
     Stops: list["StopData"]
     TripHeadsign: str
 
 
 @dataclass
-class PathDirection:
+class RoutePathDirection:
     """Direction for a Path."""
 
-    bus: "MetroBus"
-    data: PathDirectionData
+    route_path: RoutePath
+    data: PathDirectionData = field(repr=False)
     direction_num: int
     direction: str = field(init=False)
-    shapes: list[ShapePoint] = field(init=False)
-    stops_data: list["StopData"] = field(init=False)
+    shapes: list[ShapePoint] = field(init=False, repr=False)
+    stops_data: list["StopData"] = field(init=False, repr=False)
     trip_headsign: str = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.direction = self.data["DirectionText"]
         self.shapes = sorted(
             [ShapePoint(shape_data) for shape_data in self.data["Shape"]],
             key=lambda shape: shape.sequence_number,
         )
         self.stops_data = self.data["Stops"]
         self.trip_headsign = self.data["TripHeadsign"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.route_path, self.direction_num))
+
     @property
     def stops(self) -> list["Stop"]:
         """Return the stops."""
         return [
-            self.bus.get_stop_from_stop_data(stop_data) for stop_data in self.stops_data
+            self.route_path.bus.get_stop_from_stop_data(stop_data)
+            for stop_data in self.stops_data
         ]
 
 
 class RoutePathData(TypedDict):
     """Path data for MetroBus WMATA API."""
 
     RouteID: str
@@ -83,26 +92,32 @@
     Direction1: PathDirectionData | None
 
 
 @dataclass
 class RoutePath:
     """Path for a MetroBus."""
 
-    bus: "MetroBus"
-    data: RoutePathData
+    bus: "MetroBus" = field(repr=False)
+    data: RoutePathData = field(repr=False)
     route_id: str = field(init=False)
     name: str = field(init=False)
-    directions: dict[int, PathDirection] = field(init=False, default_factory=dict)
+    path_directions: dict[int, RoutePathDirection] = field(
+        init=False, default_factory=dict, repr=False
+    )
 
     def __post_init__(self) -> None:
         """Post init."""
         self.route_id = self.data["RouteID"]
         self.name = self.data["Name"]
         if (direction_data := self.data["Direction0"]) is not None:
-            self.directions[0] = PathDirection(self.bus, direction_data, 0)
+            self.path_directions[0] = RoutePathDirection(self, direction_data, 0)
         if (direction_data := self.data["Direction1"]) is not None:
-            self.directions[1] = PathDirection(self.bus, direction_data, 1)
+            self.path_directions[1] = RoutePathDirection(self, direction_data, 1)
+
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.route)
 
     @property
     def route(self) -> "Route":
         """Return the route."""
         return self.bus.routes[self.route_id]
```

### Comparing `pywmataio-0.0.7/wmataio/bus/models/route_schedule.py` & `pywmataio-0.0.8/wmataio/bus/models/route_schedule.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,32 +22,36 @@
     Time: str
 
 
 @dataclass
 class StopTime:
     """Stop Time for a Route Schedule."""
 
-    bus: "MetroBus"
-    data: StopTimeData
+    direction_schedule: DirectionSchedule
+    data: StopTimeData = field(repr=False)
     stop_id: str = field(init=False)
     stop_name: str = field(init=False)
     stop_sequence: int = field(init=False)
     time: datetime = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.stop_id = self.data["StopID"]
         self.stop_name = self.data["StopName"]
         self.stop_sequence = self.data["StopSeq"]
         self.time = datetime.fromisoformat(self.data["Time"]).replace(tzinfo=TZ)
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.stop, self.direction_schedule))
+
     @property
     def stop(self) -> Stop:
         """Get stop."""
-        return self.bus.stops[self.stop_id]
+        return self.direction_schedule.route_schedule.bus.stops[self.stop_id]
 
 
 class DirectionScheduleData(TypedDict):
     """DirectionSchedule data for MetroBus WMATA API."""
 
     DirectionNum: int  # deprecated
     EndTime: str
@@ -59,77 +63,82 @@
     TripID: str
 
 
 @dataclass
 class DirectionSchedule:
     """Direction Schedule for a Path."""
 
-    bus: "MetroBus"
-    data: DirectionScheduleData
+    route_schedule: RouteSchedule
+    data: DirectionScheduleData = field(repr=False)
     direction_num: int
     end_time: datetime = field(init=False)
-    route_id: str = field(init=False)
+    route_id: str = field(init=False, repr=False)
     route: Route = field(init=False)
     start_time: datetime = field(init=False)
-    stop_times_data: list[StopTimeData] = field(init=False)
+    stop_times_data: list[StopTimeData] = field(init=False, repr=False)
     stop_times: list[StopTime] = field(init=False)
     trip_direction: str = field(init=False)
     trip_headsign: str = field(init=False)
     trip_id: str = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.end_time = datetime.fromisoformat(self.data["EndTime"]).replace(tzinfo=TZ)
         self.route_id = self.data["RouteID"]
-        self.route = self.bus.routes[self.route_id]
+        self.route = self.route_schedule.bus.routes[self.route_id]
         self.start_time = datetime.fromisoformat(self.data["StartTime"]).replace(
             tzinfo=TZ
         )
         self.stop_times_data = self.data["StopTimes"]
         self.stop_times = sorted(
-            [
-                StopTime(self.bus, stop_time_data)
-                for stop_time_data in self.stop_times_data
-            ],
+            [StopTime(self, stop_time_data) for stop_time_data in self.stop_times_data],
             key=lambda stop_time: stop_time.stop_sequence,
         )
         self.trip_direction = self.data["TripDirectionText"]
         self.trip_headsign = self.data["TripHeadsign"]
         self.trip_id = self.data["TripID"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.direction_num, self.route, self.trip_id))
+
 
 class RouteScheduleData(TypedDict):
     """Route schedule data for MetroBus WMATA API."""
 
     Direction0: list[DirectionScheduleData] | None
     Direction1: list[DirectionScheduleData] | None
 
 
 @dataclass
 class RouteSchedule:
     """Schedule for a Route."""
 
-    bus: "MetroBus"
+    bus: "MetroBus" = field(repr=False)
     route: "Route"
-    data: RouteScheduleData
+    data: RouteScheduleData = field(repr=False)
     directions_schedules: dict[int, list[DirectionSchedule]] = field(
         init=False, default_factory=dict
     )
 
     def __post_init__(self) -> None:
         """Post init."""
         if (direction_schedules_data := self.data["Direction0"]) is not None:
             self.directions_schedules[0] = sorted(
                 [
-                    DirectionSchedule(self.bus, direction_schedule_data, 0)
+                    DirectionSchedule(self, direction_schedule_data, 0)
                     for direction_schedule_data in direction_schedules_data
                 ],
                 key=lambda direction_schedule: direction_schedule.start_time,
             )
         if (direction_schedules_data := self.data["Direction1"]) is not None:
             self.directions_schedules[1] = sorted(
                 [
-                    DirectionSchedule(self.bus, direction_schedule_data, 1)
+                    DirectionSchedule(self, direction_schedule_data, 1)
                     for direction_schedule_data in direction_schedules_data
                 ],
                 key=lambda direction_schedule: direction_schedule.start_time,
             )
+
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.directions_schedules.values())
```

### Comparing `pywmataio-0.0.7/wmataio/bus/models/stop.py` & `pywmataio-0.0.8/wmataio/bus/models/stop.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,26 +21,21 @@
     Routes: list[str]
 
 
 @dataclass
 class Stop:
     """A MetroBus Stop."""
 
-    bus: "MetroBus"
-    data: StopData
+    bus: "MetroBus" = field(repr=False)
+    data: StopData = field(repr=False)
     stop_id: str = field(init=False)
-    coordinates: Coordinates = field(init=False)
+    coordinates: Coordinates = field(init=False, repr=False)
     name: str = field(init=False)
     route_ids: list[str] = field(init=False)
 
-    def __repr__(self) -> str:
-        """Return the representation."""
-        cls_name = type(self).__name__
-        return f"{cls_name}(code={self.stop_id}, name={self.name})"
-
     def __hash__(self) -> int:
         """Return the hash."""
         return hash(self.stop_id)
 
     def __post_init__(self) -> None:
         """Post init."""
         if isinstance(self.data["StopID"], str):
@@ -48,10 +43,10 @@
         else:
             self.stop_id = self.data["Name"]
         self.coordinates = Coordinates(self.data["Lat"], self.data["Lon"])
         self.name = self.data["Name"]
         self.route_ids = self.data["Routes"]
 
     @property
-    def routes(self) -> list["Route"]:
+    def routes(self) -> set["Route"]:
         """Return routes for this stop."""
-        return [self.bus.routes[route_id] for route_id in self.route_ids]
+        return {self.bus.routes[route_id] for route_id in self.route_ids}
```

### Comparing `pywmataio-0.0.7/wmataio/bus/models/stop_schedule.py` & `pywmataio-0.0.8/wmataio/bus/models/stop_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     TripID: str
 
 
 @dataclass
 class StopArrival:
     """Stop Arrival for a Route Schedule."""
 
-    bus: "MetroBus"
+    bus: "MetroBus" = field(repr=False)
     stop: "Stop"
-    data: StopArrivalData
+    data: StopArrivalData = field(repr=False)
     direction_number: int = field(init=False)
     end_time: datetime = field(init=False)
     route_id: str = field(init=False)
     schedule_time: datetime = field(init=False)
     start_time: datetime = field(init=False)
     trip_direction_text: str = field(init=False)
     trip_headsign: str = field(init=False)
@@ -53,11 +53,15 @@
         self.start_time = datetime.fromisoformat(self.data["StartTime"]).replace(
             tzinfo=TZ
         )
         self.trip_direction_text = self.data["TripDirectionText"]
         self.trip_headsign = self.data["TripHeadsign"]
         self.trip_id = self.data["TripID"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.stop, self.direction_number, self.route))
+
     @property
     def route(self) -> "Route":
         """Return the route."""
         return self.bus.routes[self.route_id]
```

### Comparing `pywmataio-0.0.7/wmataio/client.py` & `pywmataio-0.0.8/wmataio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,22 @@
 
     def _get_headers(
         self,
         enum_: BusEndpoint | RailEndpoint | WMATAEndpoint,
         additional_path: str | None = None,
     ) -> dict[str, Any]:
         """Get headers."""
-        headers = self._headers
         if self.test_mode:
             return {
-                **headers,
+                **self._headers,
                 CLASS_HEADER: enum_.__class__.__name__,
                 ENUM_HEADER: enum_.name,
                 ADDITIONAL_PATH_HEADER: additional_path or "",
             }
-        return headers
+        return self._headers
 
     async def fetch(
         self,
         enum_: BusEndpoint | RailEndpoint | WMATAEndpoint,
         params: dict[str, Any] | None = None,
         additional_path: str | None = None,
     ) -> dict:
```

### Comparing `pywmataio-0.0.7/wmataio/models/area.py` & `pywmataio-0.0.8/wmataio/models/area.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     coordinates: Coordinates
 
     def __init__(self, radius: int, latitude: float, longitude: float) -> None:
         """Initialize the search area parameters."""
         self.radius = radius
         self.coordinates = Coordinates(latitude, longitude)
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.radius, self.coordinates))
+
     def to_dict(self) -> dict[str, int | float]:
         """Return a dict representation of the search area parameters."""
         return {
             "Radius": self.radius,
             "Lat": self.coordinates.latitude,
             "Lon": self.coordinates.longitude,
         }
```

### Comparing `pywmataio-0.0.7/wmataio/rail/__init__.py` & `pywmataio-0.0.8/wmataio/rail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,21 @@
             await self.client.fetch(
                 RailEndpoint.STATION_TO_STATION_PATH, params=params
             ),
         )
         info_data = await self.client.fetch(
             RailEndpoint.STATION_TO_STATION_INFO, params=params
         )
-        return StationToStation(self, path_data, info_data["StationToStationInfos"])
+        return StationToStation(
+            self,
+            from_station,
+            to_station,
+            path_data,
+            info_data["StationToStationInfos"],
+        )
 
     async def get_elevator_escalator_incidents(
         self, station: Station | None = None
     ) -> list[ElevatorAndEscalatorIncident]:
         """Get elevator and escalator incidents."""
         params = {}
         if station:
```

### Comparing `pywmataio-0.0.7/wmataio/rail/const.py` & `pywmataio-0.0.8/wmataio/rail/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Constants for MetroRail API."""
 from __future__ import annotations
 
 from enum import Enum
 
-from ..const import BASE_URL
+from ..const import BASE_WMATA_URL
 
 
 class RailEndpoint(Enum):
     """Endpoints for all MetroRail endpoints."""
 
-    ELEVATOR_ESCALATOR_INCIDENTS = f"{BASE_URL}/Incidents.svc/json/ElevatorIncidents"
-    RAIL_INCIDENTS = f"{BASE_URL}/Incidents.svc/json/Incidents"
-    LINES = f"{BASE_URL}/Rail.svc/json/jLines"
-    NEXT_TRAINS = f"{BASE_URL}/StationNextTrain.svc/json/GetNextTrain"
-    STANDARD_ROUTES = f"{BASE_URL}/TrainPositions/StandardRoutes"
-    STATION_ENTRANCES = f"{BASE_URL}/Rail.svc/json/jStationEntrances"
-    STATION_INFORMATION = f"{BASE_URL}/Rail.svc/json/jStationInfo"
-    STATION_PARKING_INFORMATION = f"{BASE_URL}/Rail.svc/json/jStationParking"
-    STATION_TIMINGS = f"{BASE_URL}/Rail.svc/json/jStationTimes"
-    STATION_TO_STATION_INFO = f"{BASE_URL}/Rail.svc/json/jSrcStationToDstStationInfo"
-    STATION_TO_STATION_PATH = f"{BASE_URL}/Rail.svc/json/jPath"
-    STATIONS = f"{BASE_URL}/Rail.svc/json/jStations"
-    TRACK_CIRCUITS = f"{BASE_URL}/TrainPositions/TrackCircuits"
-    TRAIN_POSITIONS = f"{BASE_URL}/TrainPositions/TrainPositions"
+    ELEVATOR_ESCALATOR_INCIDENTS = (
+        f"{BASE_WMATA_URL}/Incidents.svc/json/ElevatorIncidents"
+    )
+    RAIL_INCIDENTS = f"{BASE_WMATA_URL}/Incidents.svc/json/Incidents"
+    LINES = f"{BASE_WMATA_URL}/Rail.svc/json/jLines"
+    NEXT_TRAINS = f"{BASE_WMATA_URL}/StationNextTrain.svc/json/GetNextTrain"
+    STANDARD_ROUTES = f"{BASE_WMATA_URL}/TrainPositions/StandardRoutes"
+    STATION_ENTRANCES = f"{BASE_WMATA_URL}/Rail.svc/json/jStationEntrances"
+    STATION_INFORMATION = f"{BASE_WMATA_URL}/Rail.svc/json/jStationInfo"
+    STATION_PARKING_INFORMATION = f"{BASE_WMATA_URL}/Rail.svc/json/jStationParking"
+    STATION_TIMINGS = f"{BASE_WMATA_URL}/Rail.svc/json/jStationTimes"
+    STATION_TO_STATION_INFO = (
+        f"{BASE_WMATA_URL}/Rail.svc/json/jSrcStationToDstStationInfo"
+    )
+    STATION_TO_STATION_PATH = f"{BASE_WMATA_URL}/Rail.svc/json/jPath"
+    STATIONS = f"{BASE_WMATA_URL}/Rail.svc/json/jStations"
+    TRACK_CIRCUITS = f"{BASE_WMATA_URL}/TrainPositions/TrackCircuits"
+    TRAIN_POSITIONS = f"{BASE_WMATA_URL}/TrainPositions/TrainPositions"
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/address.py` & `pywmataio-0.0.8/wmataio/rail/models/address.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,23 @@
     Zip: str
 
 
 @dataclass
 class Address:
     """MetroRail Station Address."""
 
-    data: AddressData
+    data: AddressData = field(repr=False)
     street: str = field(init=False)
     city: str = field(init=False)
     state: str = field(init=False)
     zip_code: str = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.street = self.data["Street"]
         self.city = self.data["City"]
         self.state = self.data["State"]
         self.zip_code = self.data["Zip"]
+
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.street, self.city, self.state, self.zip_code))
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/elevator_and_escalator_incident.py` & `pywmataio-0.0.8/wmataio/rail/models/elevator_and_escalator_incident.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     UnitType: Literal["ELEVATOR", "ESCALATOR"]
 
 
 @dataclass
 class ElevatorAndEscalatorIncident:
     """MetroRail Elevator/Escalator Incident."""
 
-    bus: "MetroRail"
-    data: ElevatorAndEscalatorIncidentData
+    rail: "MetroRail" = field(repr=False)
+    data: ElevatorAndEscalatorIncidentData = field(repr=False)
     date_out_of_service: datetime = field(init=False)
     date_updated: datetime = field(init=False)
     estimated_return_to_service: datetime | None = field(init=False, default=None)
     location_description: str = field(init=False)
     station_code: str = field(init=False)
     station_name: str = field(init=False)
     symptom_description: str = field(init=False)
@@ -61,11 +61,23 @@
         self.location_description = self.data["LocationDescription"]
         self.station_code = self.data["StationCode"]
         self.station_name = self.data["StationName"]
         self.symptom_description = self.data["SymptomDescription"]
         self.unit_name = self.data["UnitName"]
         self.unit_type = self.data["UnitType"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(
+            (
+                self.station,
+                self.date_out_of_service,
+                self.symptom_description,
+                self.unit_name,
+                self.unit_type,
+            )
+        )
+
     @property
     def station(self) -> "Station":
         """Return the station."""
-        return self.bus.stations[self.station_code]
+        return self.rail.stations[self.station_code]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/line.py` & `pywmataio-0.0.8/wmataio/rail/models/line.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,29 +21,24 @@
     LineCode: str
 
 
 @dataclass
 class Line:
     """MetroRail Line."""
 
-    bus: "MetroRail"
-    data: LineData
-    standard_routes: list["StandardRoute"]
+    rail: "MetroRail" = field(repr=False)
+    data: LineData = field(repr=False)
+    standard_routes: list["StandardRoute"] = field(repr=False)
     display_name: str = field(init=False)
     start_station_code: str = field(init=False)
     end_station_code: str = field(init=False)
     internal_destination_code_1: str | None = field(init=False, default=None)
     internal_destination_code_2: str | None = field(init=False, default=None)
     line_code: str = field(init=False)
 
-    def __repr__(self) -> str:
-        """Return the representation."""
-        cls_name = type(self).__name__
-        return f"{cls_name}(code={self.line_code}, name={self.display_name})"
-
     def __hash__(self) -> int:
         """Return the hash."""
         return hash(self.line_code)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.line_code = self.data["LineCode"]
@@ -54,27 +49,27 @@
             self.internal_destination_code_1 = internal_destination_1
         if internal_destination_2 := self.data["InternalDestination2"]:
             self.internal_destination_code_2 = internal_destination_2
 
     @property
     def start_station(self) -> "Station":
         """Return the start station."""
-        return self.bus.stations[self.start_station_code]
+        return self.rail.stations[self.start_station_code]
 
     @property
     def end_station(self) -> "Station":
         """Return the end station."""
-        return self.bus.stations[self.end_station_code]
+        return self.rail.stations[self.end_station_code]
 
     @property
     def internal_destination_1(self) -> "Station" | None:
         """Return the internal destination 1."""
         if not self.internal_destination_code_1:
             return None
-        return self.bus.stations[self.internal_destination_code_1]
+        return self.rail.stations[self.internal_destination_code_1]
 
     @property
     def internal_destination_2(self) -> "Station" | None:
         """Return the internal destination 2."""
         if not self.internal_destination_code_2:
             return None
-        return self.bus.stations[self.internal_destination_code_2]
+        return self.rail.stations[self.internal_destination_code_2]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/live_position.py` & `pywmataio-0.0.8/wmataio/rail/models/live_position.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     TrainNumber: str
 
 
 @dataclass
 class LiveTrainPosition:
     """A MetroRail Bus LiveTrainPosition."""
 
-    bus: "MetroRail"
-    data: LiveTrainPositionData
+    rail: "MetroRail" = field(repr=False)
+    data: LiveTrainPositionData = field(repr=False)
     car_count: int = field(init=False)
     circuit_id: int = field(init=False)
     destination_station_code: str | None = field(init=False)
     direction: TrainDirection = field(init=False)
     line_code: str = field(init=False)
     seconds_at_location: int = field(init=False)
     service_type: Literal["NoPassengers", "Normal", "Special", "Unknown"] = field(
@@ -58,20 +58,26 @@
         self.direction = TrainDirection(self.data["DirectionNum"])
         self.line_code = self.data["LineCode"]
         self.seconds_at_location = self.data["SecondsAtLocation"]
         self.service_type = self.data["ServiceType"]
         self.train_id = self.data["TrainId"]
         self.train_number = self.data["TrainNumber"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(
+            (self.train_id, self.circuit_id, self.line, self.destination_station)
+        )
+
     @property
     def destination_station(self) -> "Station" | None:
         """Return the destination station."""
         if not self.destination_station_code:
             return None
-        return self.bus.stations[self.destination_station_code]
+        return self.rail.stations[self.destination_station_code]
 
     @property
     def line(self) -> "Line" | None:
         """Return the line."""
         if not self.line_code:
             return None
-        return self.bus.lines[self.line_code]
+        return self.rail.lines[self.line_code]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/next_train.py` & `pywmataio-0.0.8/wmataio/rail/models/next_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     Min: int | str | None
 
 
 @dataclass
 class NextTrain:
     """NextTrain."""
 
-    bus: "MetroRail"
-    data: NextTrainData
+    rail: "MetroRail" = field(repr=False)
+    data: NextTrainData = field(repr=False)
     num_cars: int | None = field(init=False)
     destination: str = field(init=False)
     destination_station_code: str | None = field(init=False)
     destination_station_name: str | None = field(init=False)
     group: int = field(init=False)
     line_code: str | None = field(init=False)
     location_code: str = field(init=False)
@@ -60,25 +60,29 @@
         if (minutes := self.data["Min"]) in ("-", "---") or minutes is None:
             self.minutes = None
         else:
             self.minutes = minutes
             with suppress(ValueError):
                 self.minutes = int(minutes)
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.location, self.destination_station, self.line))
+
     @property
     def destination_station(self) -> "Station" | None:
         """Return the destination Station."""
         if not self.destination_station_code:
             return None
-        return self.bus.stations[self.destination_station_code]
+        return self.rail.stations[self.destination_station_code]
 
     @property
     def line(self) -> "Line" | None:
         """Return the Line."""
         if not self.line_code:
             return None
-        return self.bus.lines[self.line_code]
+        return self.rail.lines[self.line_code]
 
     @property
     def location(self) -> "Station":
         """Return the location Station."""
-        return self.bus.stations[self.location_code]
+        return self.rail.stations[self.location_code]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/rail_incident.py` & `pywmataio-0.0.8/wmataio/rail/models/rail_incident.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     StartLocationFullName: str | None  # deprecated
 
 
 @dataclass
 class RailIncident:
     """MetroRail Incident."""
 
-    bus: "MetroRail"
-    data: RailIncidentData
+    rail: "MetroRail" = field(repr=False)
+    data: RailIncidentData = field(repr=False)
     date_updated: datetime = field(init=False)
     description: str = field(init=False)
     incident_id: str = field(init=False)
     incident_type: str = field(init=False)
     line_codes_affected: list[str] = field(init=False)
 
     def __post_init__(self) -> None:
@@ -49,11 +49,15 @@
         self.incident_type = self.data["IncidentType"]
         self.line_codes_affected = [
             line_code.strip()
             for line_code in self.data["LinesAffected"].split(";")
             if line_code.strip()
         ]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.incident_id)
+
     @property
     def lines_affected(self) -> list["Line"]:
         """Lines affected."""
-        return [self.bus.lines[line_code] for line_code in self.line_codes_affected]
+        return [self.rail.lines[line_code] for line_code in self.line_codes_affected]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/standard_route.py` & `pywmataio-0.0.8/wmataio/rail/models/standard_route.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,61 +18,71 @@
     StationCode: str | None
 
 
 @dataclass
 class StandardRoutesTrackCircuit:
     """Standard routes rack circuit."""
 
-    bus: "MetroRail"
-    data: StandardRoutesTrackCircuitData
+    standard_route: StandardRoute
+    data: StandardRoutesTrackCircuitData = field(repr=False)
     circuit_id: int = field(init=False)
     sequence_number: int = field(init=False)
     station_code: str | None = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.circuit_id = self.data["CircuitId"]
         self.sequence_number = self.data["SeqNum"]
         self.station_code = self.data["StationCode"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(
+            (self.circuit_id, self.sequence_number, self.station, self.standard_route)
+        )
+
     @property
     def station(self) -> "Station" | None:
         """Station."""
         if self.station_code is None:
             return None
-        return self.bus.stations[self.station_code]
+        return self.standard_route.rail.stations[self.station_code]
 
 
 class StandardRouteData(TypedDict):
     """Standard route data for MetroRail WMATA API."""
 
     LineCode: str
     TrackCircuits: list[StandardRoutesTrackCircuitData]
     TrackNum: Literal[1, 2]
 
 
 @dataclass
 class StandardRoute:
     """Standard route."""
 
-    bus: "MetroRail"
-    data: StandardRouteData
+    rail: "MetroRail" = field(repr=False)
+    data: StandardRouteData = field(repr=False)
     line_code: str = field(init=False)
     track_circuits: list[StandardRoutesTrackCircuit] = field(init=False)
     track_number: Literal[1, 2] = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.line_code = self.data["LineCode"]
         self.track_circuits = sorted(
             [
-                StandardRoutesTrackCircuit(self.bus, track_circuit_data)
+                StandardRoutesTrackCircuit(self, track_circuit_data)
                 for track_circuit_data in self.data["TrackCircuits"]
             ],
             key=lambda track_circuit: track_circuit.sequence_number,
         )
         self.track_number = self.data["TrackNum"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.line, self.track_number))
+
     @property
     def line(self) -> "Line":
         """Return line for route."""
-        return self.bus.lines[self.line_code]
+        return self.rail.lines[self.line_code]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/station.py` & `pywmataio-0.0.8/wmataio/rail/models/station.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,32 +31,27 @@
     StationTogether2: str
 
 
 @dataclass
 class Station:
     """MetroRail Station."""
 
-    bus: "MetroRail"
-    data: StationData
-    parking: "StationParking" | None
-    entrances: list["StationEntrance"]
-    station_times: list["StationTime"]
+    rail: "MetroRail" = field(repr=False)
+    data: StationData = field(repr=False)
+    parking: "StationParking" | None = field(repr=False)
+    entrances: list["StationEntrance"] = field(repr=False)
+    station_times: list["StationTime"] = field(repr=False)
     address: Address = field(init=False)
     station_code: str = field(init=False)
     coordinates: Coordinates = field(init=False)
     line_codes: list[str] = field(init=False)
     name: str = field(init=False)
     station_together_code_1: str | None = field(init=False)
     station_together_code_2: str | None = field(init=False)
 
-    def __repr__(self) -> str:
-        """Return the representation."""
-        cls_name = type(self).__name__
-        return f"{cls_name}(code={self.station_code}, name={self.name})"
-
     def __hash__(self) -> int:
         """Return the hash."""
         return hash(self.station_code)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.address = Address(self.data["Address"])
@@ -74,22 +69,22 @@
         self.station_together_code_2 = (
             self.data["StationTogether2"] if self.data["StationTogether2"] else None
         )
 
     @property
     def lines(self) -> list["Line"]:
         """Return the lines."""
-        return [self.bus.lines[line_code] for line_code in self.line_codes]
+        return [self.rail.lines[line_code] for line_code in self.line_codes]
 
     @property
     def station_together_1(self) -> "Station" | None:
         """Return the station together 1."""
         if not self.station_together_code_1:
             return None
-        return self.bus.stations[self.station_together_code_1]
+        return self.rail.stations[self.station_together_code_1]
 
     @property
     def station_together_2(self) -> "Station" | None:
         """Return the station together 2."""
         if not self.station_together_code_2:
             return None
-        return self.bus.stations[self.station_together_code_2]
+        return self.rail.stations[self.station_together_code_2]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/station_entrance.py` & `pywmataio-0.0.8/wmataio/rail/models/station_entrance.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     StationCode2: str
 
 
 @dataclass
 class StationEntrance:
     """Station entrance information for MetroRail WMATA API."""
 
-    bus: "MetroRail"
-    data: StationEntranceData
+    rail: "MetroRail" = field(repr=False)
+    data: StationEntranceData = field(repr=False)
     description: str = field(init=False)
     entrance_id: str = field(init=False)
     coordinates: Coordinates = field(init=False)
     name: str = field(init=False)
     station_code_1: str = field(init=False)
     station_code_2: str = field(init=False)
 
@@ -41,16 +41,20 @@
         self.description = self.data["Description"]
         self.entrance_id = self.data["ID"]
         self.coordinates = Coordinates(self.data["Lat"], self.data["Lon"])
         self.name = self.data["Name"]
         self.station_code_1 = self.data["StationCode1"]
         self.station_code_2 = self.data["StationCode2"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.entrance_id)
+
     @property
     def station_1(self) -> "Station":
         """Return the station 1."""
-        return self.bus.stations[self.station_code_1]
+        return self.rail.stations[self.station_code_1]
 
     @property
     def station_2(self) -> "Station":
         """Return the station 2."""
-        return self.bus.stations[self.station_code_2]
+        return self.rail.stations[self.station_code_2]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/station_parking.py` & `pywmataio-0.0.8/wmataio/rail/models/station_parking.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,23 +16,28 @@
     Notes: str | None
 
 
 @dataclass
 class ShortTermParking:
     """Short-term parking information for MetroRail WMATA API."""
 
-    data: ShortTermParkingData
+    station_parking: StationParking
+    data: ShortTermParkingData = field(repr=False)
     total_count: int = field(init=False)
     notes: str | None = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.total_count = self.data["TotalCount"]
         self.notes = self.data["Notes"] if self.data["Notes"] else None
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.station_parking)
+
 
 class AllDayParkingData(TypedDict):
     """All-day parking data for MetroRail WMATA API."""
 
     TotalCount: int
     RiderCost: float | int
     NonRiderCost: float | int
@@ -40,15 +45,16 @@
     SaturdayNonRiderCost: float | int
 
 
 @dataclass
 class AllDayParking:
     """All-day parking information for MetroRail WMATA API."""
 
-    data: AllDayParkingData
+    station_parking: StationParking
+    data: AllDayParkingData = field(repr=False)
     total_count: int = field(init=False)
     rider_cost: float | None = field(init=False, default=None)
     non_rider_cost: float | None = field(init=False, default=None)
     saturday_rider_cost: float | None = field(init=False, default=None)
     saturday_non_rider_cost: float | None = field(init=False, default=None)
 
     def __post_init__(self) -> None:
@@ -60,39 +66,47 @@
         if non_rider_cost := self.data["NonRiderCost"]:
             self.non_rider_cost = float(non_rider_cost)
         if saturday_rider_cost := self.data["SaturdayRiderCost"]:
             self.saturday_rider_cost = float(saturday_rider_cost)
         if saturday_non_rider_cost := self.data["SaturdayNonRiderCost"]:
             self.saturday_non_rider_cost = float(saturday_non_rider_cost)
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.station_parking)
+
 
 class StationParkingData(TypedDict):
     """Station parking data for MetroRail WMATA API."""
 
     Code: str
     Notes: str | None
     ShortTermParking: ShortTermParkingData
     AllDayParking: AllDayParkingData
 
 
 @dataclass
 class StationParking:
     """Station parking information for MetroRail WMATA API."""
 
-    bus: "MetroRail"
-    data: StationParkingData
+    rail: "MetroRail" = field(repr=False)
+    data: StationParkingData = field(repr=False)
     code: str = field(init=False)
     notes: str | None = field(init=False)
     short_term_parking: ShortTermParking = field(init=False)
     all_day_parking: AllDayParking = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.code = self.data["Code"]
         self.notes = self.data["Notes"] if self.data["Notes"] else None
-        self.short_term_parking = ShortTermParking(self.data["ShortTermParking"])
-        self.all_day_parking = AllDayParking(self.data["AllDayParking"])
+        self.short_term_parking = ShortTermParking(self, self.data["ShortTermParking"])
+        self.all_day_parking = AllDayParking(self, self.data["AllDayParking"])
+
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.station, self.code))
 
     @property
     def station(self) -> "Station":
         """Return the station."""
-        return self.bus.stations[self.code]
+        return self.rail.stations[self.code]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/station_timings.py` & `pywmataio-0.0.8/wmataio/rail/models/station_timings.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,62 +19,70 @@
     DestinationStation: str
 
 
 @dataclass
 class TrainTiming:
     """Train timing for MetroRail WMATA API."""
 
-    bus: "MetroRail"
-    data: TrainTimingData
+    day_time: DayTime
+    data: TrainTimingData = field(repr=False)
     time: time = field(init=False)
     destination_station_code: str = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.time = time.fromisoformat(self.data["Time"]).replace(tzinfo=TZ)
         self.destination_station_code = self.data["DestinationStation"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.day_time, self.destination_station))
+
     @property
     def destination_station(self) -> "Station":
         """Return the destination station."""
-        return self.bus.stations[self.destination_station_code]
+        return self.day_time.station_time.rail.stations[self.destination_station_code]
 
 
 class DayTimeData(TypedDict):
     """Day time data for MetroRail WMATA API."""
 
     OpeningTime: str
     FirstTrains: list[TrainTimingData]
     LastTrains: list[TrainTimingData]
 
 
 @dataclass
 class DayTime:
     """Day time for MetroRail WMATA API."""
 
-    bus: "MetroRail"
-    data: DayTimeData
+    station_time: StationTime
+    data: DayTimeData = field(repr=False)
     day: str
-    day_of_week: int
+    day_of_week: int = field(repr=False)
     opening_time: time = field(init=False)
     first_trains: list[TrainTiming] = field(init=False)
     last_trains: list[TrainTiming] = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.opening_time = time.fromisoformat(self.data["OpeningTime"]).replace(
             tzinfo=TZ
         )
         self.first_trains = [
-            TrainTiming(self.bus, train) for train in self.data["FirstTrains"]
+            TrainTiming(self, train) for train in self.data["FirstTrains"]
         ]
         self.last_trains = [
-            TrainTiming(self.bus, train) for train in self.data["LastTrains"]
+            TrainTiming(self, train) for train in self.data["LastTrains"]
         ]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.station_time, self.day))
+
 
 class StationTimeData(TypedDict):
     """Station time data for MetroRail WMATA API."""
 
     Code: str
     StationName: str
     Monday: DayTimeData
@@ -86,35 +94,39 @@
     Sunday: DayTimeData
 
 
 @dataclass
 class StationTime:
     """Station time for MetroRail WMATA API."""
 
-    bus: "MetroRail"
-    data: StationTimeData
+    rail: "MetroRail" = field(repr=False)
+    data: StationTimeData = field(repr=False)
     station_code: str = field(init=False)
     name: str = field(init=False)
     days_of_week: dict[int, DayTime] = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.station_code = self.data["Code"]
         self.name = self.data["StationName"]
         self.days_of_week = {
-            1: DayTime(self.bus, self.data["Monday"], "Monday", 1),
-            2: DayTime(self.bus, self.data["Tuesday"], "Tuesday", 2),
-            3: DayTime(self.bus, self.data["Wednesday"], "Wednesday", 3),
-            4: DayTime(self.bus, self.data["Thursday"], "Thursday", 4),
-            5: DayTime(self.bus, self.data["Friday"], "Friday", 5),
-            6: DayTime(self.bus, self.data["Saturday"], "Saturday", 6),
-            7: DayTime(self.bus, self.data["Sunday"], "Sunday", 7),
+            1: DayTime(self, self.data["Monday"], "Monday", 1),
+            2: DayTime(self, self.data["Tuesday"], "Tuesday", 2),
+            3: DayTime(self, self.data["Wednesday"], "Wednesday", 3),
+            4: DayTime(self, self.data["Thursday"], "Thursday", 4),
+            5: DayTime(self, self.data["Friday"], "Friday", 5),
+            6: DayTime(self, self.data["Saturday"], "Saturday", 6),
+            7: DayTime(self, self.data["Sunday"], "Sunday", 7),
         }
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.station)
+
     @property
     def station(self) -> "Station":
         """Return the station."""
-        return self.bus.stations[self.station_code]
+        return self.rail.stations[self.station_code]
 
     def get_day_time(self, date_: datetime | date) -> DayTime:
         """Return the day time for the given date."""
         return self.days_of_week[date_.isoweekday()]
```

### Comparing `pywmataio-0.0.7/wmataio/rail/models/station_to_station.py` & `pywmataio-0.0.8/wmataio/rail/models/station_to_station.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,39 +20,43 @@
     StationName: str
 
 
 @dataclass
 class PathItem:
     """MetroRail Path Item."""
 
-    bus: "MetroRail"
-    data: PathItemData
+    station_to_station: StationToStation
+    data: PathItemData = field(repr=False)
     distance_to_previous: int = field(init=False)
     line_code: str = field(init=False)
     sequence_number: int = field(init=False)
     station_code: str = field(init=False)
     station_name: str = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.distance_to_previous = self.data["DistanceToPrev"]
         self.line_code = self.data["LineCode"]
         self.sequence_number = self.data["SeqNum"]
         self.station_code = self.data["StationCode"]
         self.station_name = self.data["StationName"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.station_to_station)
+
     @property
     def line(self) -> "Line":
         """Return the line."""
-        return self.bus.lines[self.line_code]
+        return self.station_to_station.rail.lines[self.line_code]
 
     @property
     def station(self) -> "Station":
         """Return the station."""
-        return self.bus.stations[self.station_code]
+        return self.station_to_station.rail.stations[self.station_code]
 
 
 class StationToStationPathData(TypedDict):
     """Station to station path data for MetroRail WMATA API."""
 
     Path: list[PathItemData]
 
@@ -65,25 +69,30 @@
     SeniorDisabled: float | int
 
 
 @dataclass
 class RailFare:
     """MetroRail Rail Fare."""
 
-    data: RailFareData
+    station_to_station_information: StationToStationInformation
+    data: RailFareData = field(repr=False)
     off_peak_time: float = field(init=False)
     peak_time: float = field(init=False)
     senior_disabled: float = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.off_peak_time = float(self.data["OffPeakTime"])
         self.peak_time = float(self.data["PeakTime"])
         self.senior_disabled = float(self.data["SeniorDisabled"])
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.station_to_station_information)
+
 
 class StationToStationInfoData(TypedDict):
     """Station to station info data for MetroRail WMATA API."""
 
     CompositeMiles: float | int
     DestinationStation: str
     RailFare: RailFareData
@@ -91,61 +100,71 @@
     SourceStation: str
 
 
 @dataclass
 class StationToStationInformation:
     """MetroRail Station to Station Info."""
 
-    bus: "MetroRail"
-    data: StationToStationInfoData
+    station_to_station: StationToStation
+    data: StationToStationInfoData = field(repr=False)
     composite_miles: float = field(init=False)
     destination_station_code: str = field(init=False)
     rail_fare: RailFare = field(init=False)
     rail_time: str = field(init=False)
     source_station_code: str = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.composite_miles = float(self.data["CompositeMiles"])
         self.destination_station_code = self.data["DestinationStation"]
-        self.rail_fare = RailFare(self.data["RailFare"])
+        self.rail_fare = RailFare(self, self.data["RailFare"])
         self.rail_time = self.data["RailTime"]
         self.source_station_code = self.data["SourceStation"]
 
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash(self.station_to_station)
+
     @property
     def destination_station(self) -> "Station":
         """Return the destination station."""
-        return self.bus.stations[self.destination_station_code]
+        return self.station_to_station.rail.stations[self.destination_station_code]
 
     @property
     def source_station(self) -> "Station":
         """Return the source station."""
-        return self.bus.stations[self.source_station_code]
+        return self.station_to_station.rail.stations[self.source_station_code]
 
 
 class StationToStationData(TypedDict):
     """Station to station data for MetroRail WMATA API."""
 
     path: StationToStationPathData
     info: StationToStationInfoData
 
 
 @dataclass
 class StationToStation:
     """MetroRail Station to Station."""
 
-    bus: "MetroRail"
-    path_data: StationToStationPathData
-    info_data: list[StationToStationInfoData]
+    rail: "MetroRail" = field(repr=False)
+    from_station: "Station"
+    to_station: "Station"
+    path_data: StationToStationPathData = field(repr=False)
+    info_data: list[StationToStationInfoData] = field(repr=False)
     path: list[PathItem] = field(init=False)
     info: list[StationToStationInformation] = field(init=False)
 
     def __post_init__(self) -> None:
         """Post init."""
         self.path = sorted(
-            [PathItem(self.bus, item_data) for item_data in self.path_data["Path"]],
+            [PathItem(self, item_data) for item_data in self.path_data["Path"]],
             key=lambda item: item.sequence_number,
         )
         self.info = [
-            StationToStationInformation(self.bus, station_info_data)
+            StationToStationInformation(self, station_info_data)
             for station_info_data in self.info_data
         ]
+
+    def __hash__(self) -> int:
+        """Return the hash."""
+        return hash((self.from_station, self.to_station))
```

