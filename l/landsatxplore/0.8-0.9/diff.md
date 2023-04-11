# Comparing `tmp/landsatxplore-0.8.tar.gz` & `tmp/landsatxplore-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/landsatxplore-0.8.tar", last modified: Tue Aug  4 13:09:10 2020, max compression
+gzip compressed data, was "landsatxplore-0.9.tar", last modified: Fri Jan 29 17:31:43 2021, max compression
```

## Comparing `landsatxplore-0.8.tar` & `landsatxplore-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 13:09:10.823584 landsatxplore-0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2020-08-04 13:09:00.000000 landsatxplore-0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-08-04 13:09:00.000000 landsatxplore-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7023 2020-08-04 13:09:10.823584 landsatxplore-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4692 2020-08-04 13:09:00.000000 landsatxplore-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     3674 2020-08-04 13:09:00.000000 landsatxplore-0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 13:09:10.823584 landsatxplore-0.8/landsatxplore/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-08-04 13:09:00.000000 landsatxplore-0.8/landsatxplore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5229 2020-08-04 13:09:00.000000 landsatxplore-0.8/landsatxplore/api.py
--rw-r--r--   0 runner    (1001) docker     (116)     3457 2020-08-04 13:09:00.000000 landsatxplore-0.8/landsatxplore/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1813 2020-08-04 13:09:00.000000 landsatxplore-0.8/landsatxplore/datamodels.py
--rw-r--r--   0 runner    (1001) docker     (116)     3553 2020-08-04 13:09:00.000000 landsatxplore-0.8/landsatxplore/earthexplorer.py
--rw-r--r--   0 runner    (1001) docker     (116)      110 2020-08-04 13:09:00.000000 landsatxplore-0.8/landsatxplore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)      501 2020-08-04 13:09:00.000000 landsatxplore-0.8/landsatxplore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 13:09:10.823584 landsatxplore-0.8/landsatxplore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7023 2020-08-04 13:09:10.000000 landsatxplore-0.8/landsatxplore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      490 2020-08-04 13:09:10.000000 landsatxplore-0.8/landsatxplore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-04 13:09:10.000000 landsatxplore-0.8/landsatxplore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       75 2020-08-04 13:09:10.000000 landsatxplore-0.8/landsatxplore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-04 13:09:10.000000 landsatxplore-0.8/landsatxplore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       20 2020-08-04 13:09:10.000000 landsatxplore-0.8/landsatxplore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2020-08-04 13:09:10.000000 landsatxplore-0.8/landsatxplore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-04 13:09:10.823584 landsatxplore-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1413 2020-08-04 13:09:00.000000 landsatxplore-0.8/setup.py
+drwxr-xr-x   0 yannforget  (1000) yannforget  (1000)        0 2021-01-29 17:31:43.240000 landsatxplore-0.9/
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     1067 2021-01-29 16:56:03.000000 landsatxplore-0.9/LICENSE.txt
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)       32 2021-01-29 16:56:03.000000 landsatxplore-0.9/MANIFEST.in
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     7044 2021-01-29 17:31:43.240000 landsatxplore-0.9/PKG-INFO
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     4713 2021-01-29 17:29:49.000000 landsatxplore-0.9/README.md
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     3697 2021-01-29 17:29:49.000000 landsatxplore-0.9/README.rst
+drwxr-xr-x   0 yannforget  (1000) yannforget  (1000)        0 2021-01-29 17:31:43.240000 landsatxplore-0.9/landsatxplore/
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)        0 2021-01-29 16:56:03.000000 landsatxplore-0.9/landsatxplore/__init__.py
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     5241 2021-01-29 17:29:49.000000 landsatxplore-0.9/landsatxplore/api.py
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     3471 2021-01-29 17:29:49.000000 landsatxplore-0.9/landsatxplore/cli.py
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     1806 2021-01-29 17:29:49.000000 landsatxplore-0.9/landsatxplore/datamodels.py
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     3625 2021-01-29 17:29:49.000000 landsatxplore-0.9/landsatxplore/earthexplorer.py
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)      110 2021-01-29 16:56:03.000000 landsatxplore-0.9/landsatxplore/exceptions.py
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)      628 2021-01-29 17:29:49.000000 landsatxplore-0.9/landsatxplore/util.py
+drwxr-xr-x   0 yannforget  (1000) yannforget  (1000)        0 2021-01-29 17:31:43.240000 landsatxplore-0.9/landsatxplore.egg-info/
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     7044 2021-01-29 17:31:43.000000 landsatxplore-0.9/landsatxplore.egg-info/PKG-INFO
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)      490 2021-01-29 17:31:43.000000 landsatxplore-0.9/landsatxplore.egg-info/SOURCES.txt
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)        1 2021-01-29 17:31:43.000000 landsatxplore-0.9/landsatxplore.egg-info/dependency_links.txt
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)       75 2021-01-29 17:31:43.000000 landsatxplore-0.9/landsatxplore.egg-info/entry_points.txt
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)        1 2021-01-29 17:05:25.000000 landsatxplore-0.9/landsatxplore.egg-info/not-zip-safe
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)       20 2021-01-29 17:31:43.000000 landsatxplore-0.9/landsatxplore.egg-info/requires.txt
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)       14 2021-01-29 17:31:43.000000 landsatxplore-0.9/landsatxplore.egg-info/top_level.txt
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)       38 2021-01-29 17:31:43.240000 landsatxplore-0.9/setup.cfg
+-rw-r--r--   0 yannforget  (1000) yannforget  (1000)     1413 2021-01-29 17:30:14.000000 landsatxplore-0.9/setup.py
```

### Comparing `landsatxplore-0.8/LICENSE.txt` & `landsatxplore-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `landsatxplore-0.8/PKG-INFO` & `landsatxplore-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: landsatxplore
-Version: 0.8
+Version: 0.9
 Summary: Search and download Landsat scenes from EarthExplorer.
 Home-page: https://github.com/yannforget/landsatxplore
 Author: Yann Forget
 Author-email: yannforget@mailbox.org
 License: UNKNOWN
 Description: # Description
         
         ![CLI Demo](https://raw.githubusercontent.com/yannforget/landsatxplore/master/demo.gif?s=0.5)
         
         The **landsatxplore** Python package provides an interface to the [EarthExplorer](http://earthexplorer.usgs.gov/) portal to search and download [Landsat Collections](https://landsat.usgs.gov/landsat-collections) scenes through a command-line interface or a Python API.
         
-        It supports three data sets: `LANDSAT_TM_C1`, `LANDSAT_ETM_C1` and `LANDSAT_8_C1`.
+        It supports four data sets: `LANDSAT_TM_C1`, `LANDSAT_ETM_C1`, `LANDSAT_8_C1`, and `SENTINEL_2A`.
         
         # Quick start
         
         Searching for Landsat 5 TM scenes that contains the location (12.53, -1.53) acquired during the year 1995.
         
         ```
         landsatxplore search --dataset LANDSAT_TM_C1 --location 12.53 -1.53 \
@@ -32,15 +32,15 @@
         
         Downloading three Landsat scenes from different datasets in the current directory.
         
         ```
         landsatxplore download LT51960471995178MPS00 LC80390222013076EDC00 LC82150682015350LGN01
         ```
         
-        To use the package, Earth Explorer credentials are required ([registration](https://ers.cr.usgs.gov/register/)).
+        To use the package, Earth Explorer credentials are required ([registration](https://ers.cr.usgs.gov/register)).
         
         # Installation
         
         The package can be installed using pip.
         
         ```
         pip install landsatxplore
@@ -88,16 +88,16 @@
         Usage: landsatxplore search [OPTIONS]
         
           Search for Landsat scenes.
         
         Options:
           -u, --username TEXT             EarthExplorer username.
           -p, --password TEXT             EarthExplorer password.
-          -d, --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1]
-                                          Landsat data set.
+          -d, --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1|SENTINEL_2A]
+                                          EO data set.
           -l, --location FLOAT...         Point of interest (latitude, longitude).
           -b, --bbox FLOAT...             Bounding box (xmin, ymin, xmax, ymax).
           -c, --clouds INTEGER            Max. cloud cover (1-100).
           -s, --start TEXT                Start date (YYYY-MM-DD).
           -e, --end TEXT                  End date (YYYY-MM-DD).
           -o, --output [scene_id|product_id|json|csv]
                                           Output format.
```

### Comparing `landsatxplore-0.8/README.md` & `landsatxplore-0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Description
 
 ![CLI Demo](https://raw.githubusercontent.com/yannforget/landsatxplore/master/demo.gif?s=0.5)
 
 The **landsatxplore** Python package provides an interface to the [EarthExplorer](http://earthexplorer.usgs.gov/) portal to search and download [Landsat Collections](https://landsat.usgs.gov/landsat-collections) scenes through a command-line interface or a Python API.
 
-It supports three data sets: `LANDSAT_TM_C1`, `LANDSAT_ETM_C1` and `LANDSAT_8_C1`.
+It supports four data sets: `LANDSAT_TM_C1`, `LANDSAT_ETM_C1`, `LANDSAT_8_C1`, and `SENTINEL_2A`.
 
 # Quick start
 
 Searching for Landsat 5 TM scenes that contains the location (12.53, -1.53) acquired during the year 1995.
 
 ```
 landsatxplore search --dataset LANDSAT_TM_C1 --location 12.53 -1.53 \
@@ -24,15 +24,15 @@
 
 Downloading three Landsat scenes from different datasets in the current directory.
 
 ```
 landsatxplore download LT51960471995178MPS00 LC80390222013076EDC00 LC82150682015350LGN01
 ```
 
-To use the package, Earth Explorer credentials are required ([registration](https://ers.cr.usgs.gov/register/)).
+To use the package, Earth Explorer credentials are required ([registration](https://ers.cr.usgs.gov/register)).
 
 # Installation
 
 The package can be installed using pip.
 
 ```
 pip install landsatxplore
@@ -80,16 +80,16 @@
 Usage: landsatxplore search [OPTIONS]
 
   Search for Landsat scenes.
 
 Options:
   -u, --username TEXT             EarthExplorer username.
   -p, --password TEXT             EarthExplorer password.
-  -d, --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1]
-                                  Landsat data set.
+  -d, --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1|SENTINEL_2A]
+                                  EO data set.
   -l, --location FLOAT...         Point of interest (latitude, longitude).
   -b, --bbox FLOAT...             Bounding box (xmin, ymin, xmax, ymax).
   -c, --clouds INTEGER            Max. cloud cover (1-100).
   -s, --start TEXT                Start date (YYYY-MM-DD).
   -e, --end TEXT                  End date (YYYY-MM-DD).
   -o, --output [scene_id|product_id|json|csv]
                                   Output format.
```

### Comparing `landsatxplore-0.8/README.rst` & `landsatxplore-0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 The **landsatxplore** Python package provides an interface to the
 `EarthExplorer <http://earthexplorer.usgs.gov/>`__ portal to search and
 download `Landsat
 Collections <https://landsat.usgs.gov/landsat-collections>`__ scenes
 through a command-line interface or a Python API.
 
-It supports three data sets: ``LANDSAT_TM_C1``, ``LANDSAT_ETM_C1`` and
-``LANDSAT_8_C1``.
+It supports four data sets: ``LANDSAT_TM_C1``, ``LANDSAT_ETM_C1``,
+``LANDSAT_8_C1`` and ``SENTINEL_2A``.
 
 Installation
 ============
 
 The package can be installed using pip.
 
 ::
@@ -49,16 +49,16 @@
     Usage: landsatxplore search [OPTIONS]
 
       Search for Landsat scenes.
 
     Options:
       --username TEXT                 EarthExplorer username.
       --password TEXT                 EarthExplorer password.
-      --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1]
-                                      Landsat data set.
+      --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1|SENTINEL_2A]
+                                      EO data set.
       --location FLOAT...             Point of interest (latitude, longitude).
       --bbox FLOAT...                 Bounding box (xmin, ymin, xmax, ymax).
       --clouds INTEGER                Max. cloud cover (1-100).
       --start TEXT                    Start date (YYYY-MM-DD).
       --end TEXT                      End date (YYYY-MM-DD).
       --limit INTEGER                 Max. results returned.
       --help                          Show this message and exit.
```

### Comparing `landsatxplore-0.8/landsatxplore/api.py` & `landsatxplore-0.9/landsatxplore/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             months=None,
             max_results=20):
         """Search for scenes.
 
         Parameters
         ----------
         dataset : str
-            LANDSAT_TM_C1, LANDSAT_ETM_C1, or LANDSAT_8_C1.
+            LANDSAT_TM_C1, LANDSAT_ETM_C1, LANDSAT_8_C1 or SENTINEL_2A.
         latitude : float, optional
             Latitude of the point of interest.
         longitude : float, optional
             Longitude of the point of interest.
         bbox : tuple, optional
             (xmin, ymin, xmax, ymax) of the bounding box.
         max_cloud_cover : int, optional
@@ -96,15 +96,15 @@
         params = {
             'datasetName': dataset,
             'includeUnknownCloudCover': False,
             'maxResults': max_results
         }
 
         if latitude and longitude:
-            params.update(spatialFilter=spatial_filter(latitude, longitude))
+            params.update(spatialFilter=spatial_filter(longitude, latitude))
         if bbox:
             params.update(spatialFilter=spatial_filter(*bbox))
         if max_cloud_cover:
             params.update(maxCloudCover=max_cloud_cover)
         if start_date:
             params.update(temporalFilter=temporal_filter(start_date, end_date))
         if months:
```

### Comparing `landsatxplore-0.8/landsatxplore/cli.py` & `landsatxplore-0.9/landsatxplore/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from io import StringIO
 
 import click
 
 from landsatxplore.api import API
 from landsatxplore.earthexplorer import EarthExplorer
 
-DATASETS = ['LANDSAT_TM_C1', 'LANDSAT_ETM_C1', 'LANDSAT_8_C1']
+DATASETS = ['LANDSAT_TM_C1', 'LANDSAT_ETM_C1', 'LANDSAT_8_C1', 'SENTINEL_2A']
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -84,15 +84,15 @@
 
 
 @click.command()
 @click.option('--username', '-u', type=click.STRING, help='EarthExplorer username.',
               envvar='LANDSATXPLORE_USERNAME')
 @click.option('--password', '-p', type=click.STRING, help='EarthExplorer password.',
               envvar='LANDSATXPLORE_PASSWORD')
-@click.option('--output', '-o', type=click.Path(exists=True, dir_okay=True), 
+@click.option('--output', '-o', type=click.Path(exists=True, dir_okay=True),
               default='.', help='Output directory.')
 @click.argument('scenes', type=click.STRING, nargs=-1)
 def download(username, password, output, scenes):
     """Download one or several Landsat scenes."""
     ee = EarthExplorer(username, password)
     output_dir = os.path.abspath(output)
     for scene in scenes:
```

### Comparing `landsatxplore-0.8/landsatxplore/datamodels.py` & `landsatxplore-0.9/landsatxplore/datamodels.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         Min. x coordinate (min longitude).
     ymin : float
         Min. y coordinate (min latitude).
     xmax : float, optional
         Max. x coordinate (max longitude).
     ymax : float, optional
         Max. y coordinate (max latitude).
-    
+
     Returns
     -------
     spatial_filter : dict
         SpatialFilter data model as a dictionnary.
     """
     if not xmax and not ymax:
         xmax = xmin + 0.1
         ymax = ymin + 0.1
-    lower_left = coordinate(xmin, ymin)
-    upper_right = coordinate(xmax, ymax)
+    lower_left = coordinate(ymin, xmin)
+    upper_right = coordinate(ymax, xmax)
     return {
         'filterType': 'mbr',
         'lowerLeft': lower_left,
         'upperRight': upper_right
     }
 
 
@@ -60,19 +60,19 @@
 
     Parameters
     ----------
     start_date : str
         ISO 8601 formatted date.
     end_date : str, optional
         ISO 8601 formatted date.
-    
+
     Returns
     -------
     temporal_filter : dict
         TemporalFilter data model as a dictionnary.
     """
     if not end_date:
         end_date = start_date
     return {
         'startDate': start_date,
         'endDate': end_date
-    }
+    }
```

### Comparing `landsatxplore-0.8/landsatxplore/earthexplorer.py` & `landsatxplore-0.9/landsatxplore/earthexplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 EE_URL = 'https://earthexplorer.usgs.gov/'
 EE_LOGIN_URL = 'https://ers.cr.usgs.gov/login/'
 EE_LOGOUT_URL = 'https://earthexplorer.usgs.gov/logout'
 EE_DOWNLOAD_URL = "https://earthexplorer.usgs.gov/download/{dataset_id}/{scene_id}/EE/"
 DATASETS = {
     "LANDSAT_TM_C1": "5e83d08fd9932768",
     "LANDSAT_ETM_C1": "5e83a507d6aaa3db",
-    "LANDSAT_8_C1": "5e83d0b84df8d8c2"
+    "LANDSAT_8_C1": "5e83d0b84df8d8c2",
+    "SENTINEL_2A": "5e83a42c6eba8084" # also contains Sentinel_2B data
 }
 
 
 def _get_tokens(body):
     """Get `csrf_token` and `__ncforminfo`."""
     csrf = re.findall(r'name="csrf" value="(.+?)"', body)[0]
     ncform = re.findall(r'name="__ncforminfo" value="(.+?)"', body)[0]
```

### Comparing `landsatxplore-0.8/landsatxplore.egg-info/PKG-INFO` & `landsatxplore-0.9/landsatxplore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: landsatxplore
-Version: 0.8
+Version: 0.9
 Summary: Search and download Landsat scenes from EarthExplorer.
 Home-page: https://github.com/yannforget/landsatxplore
 Author: Yann Forget
 Author-email: yannforget@mailbox.org
 License: UNKNOWN
 Description: # Description
         
         ![CLI Demo](https://raw.githubusercontent.com/yannforget/landsatxplore/master/demo.gif?s=0.5)
         
         The **landsatxplore** Python package provides an interface to the [EarthExplorer](http://earthexplorer.usgs.gov/) portal to search and download [Landsat Collections](https://landsat.usgs.gov/landsat-collections) scenes through a command-line interface or a Python API.
         
-        It supports three data sets: `LANDSAT_TM_C1`, `LANDSAT_ETM_C1` and `LANDSAT_8_C1`.
+        It supports four data sets: `LANDSAT_TM_C1`, `LANDSAT_ETM_C1`, `LANDSAT_8_C1`, and `SENTINEL_2A`.
         
         # Quick start
         
         Searching for Landsat 5 TM scenes that contains the location (12.53, -1.53) acquired during the year 1995.
         
         ```
         landsatxplore search --dataset LANDSAT_TM_C1 --location 12.53 -1.53 \
@@ -32,15 +32,15 @@
         
         Downloading three Landsat scenes from different datasets in the current directory.
         
         ```
         landsatxplore download LT51960471995178MPS00 LC80390222013076EDC00 LC82150682015350LGN01
         ```
         
-        To use the package, Earth Explorer credentials are required ([registration](https://ers.cr.usgs.gov/register/)).
+        To use the package, Earth Explorer credentials are required ([registration](https://ers.cr.usgs.gov/register)).
         
         # Installation
         
         The package can be installed using pip.
         
         ```
         pip install landsatxplore
@@ -88,16 +88,16 @@
         Usage: landsatxplore search [OPTIONS]
         
           Search for Landsat scenes.
         
         Options:
           -u, --username TEXT             EarthExplorer username.
           -p, --password TEXT             EarthExplorer password.
-          -d, --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1]
-                                          Landsat data set.
+          -d, --dataset [LANDSAT_TM_C1|LANDSAT_ETM_C1|LANDSAT_8_C1|SENTINEL_2A]
+                                          EO data set.
           -l, --location FLOAT...         Point of interest (latitude, longitude).
           -b, --bbox FLOAT...             Bounding box (xmin, ymin, xmax, ymax).
           -c, --clouds INTEGER            Max. cloud cover (1-100).
           -s, --start TEXT                Start date (YYYY-MM-DD).
           -e, --end TEXT                  End date (YYYY-MM-DD).
           -o, --output [scene_id|product_id|json|csv]
                                           Output format.
```

### Comparing `landsatxplore-0.8/setup.py` & `landsatxplore-0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='landsatxplore',
-    version='0.8',
+    version='0.9',
     description='Search and download Landsat scenes from EarthExplorer.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/yannforget/landsatxplore',
     author='Yann Forget',
     author_email='yannforget@mailbox.org',
     classifiers=[
```

