# Comparing `tmp/sliderule-3.0.1.tar.gz` & `tmp/sliderule-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.0.1.tar", last modified: Mon Mar 27 18:26:56 2023, max compression
+gzip compressed data, was "sliderule-3.0.2.tar", last modified: Tue Apr 11 21:16:11 2023, max compression
```

## Comparing `sliderule-3.0.1.tar` & `sliderule-3.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 18:26:56.825001 sliderule-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-03-27 18:26:43.000000 sliderule-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-03-27 18:26:56.825001 sliderule-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-03-27 18:26:43.000000 sliderule-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-03-27 18:26:43.000000 sliderule-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-27 18:26:56.825001 sliderule-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-03-27 18:26:43.000000 sliderule-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 18:26:56.821000 sliderule-3.0.1/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24883 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11458 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9821 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    35800 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85059 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    42474 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-03-27 18:26:43.000000 sliderule-3.0.1/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 18:26:56.821000 sliderule-3.0.1/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-03-27 18:26:56.000000 sliderule-3.0.1/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      953 2023-03-27 18:26:56.000000 sliderule-3.0.1/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-27 18:26:56.000000 sliderule-3.0.1/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-03-27 18:26:56.000000 sliderule-3.0.1/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-27 18:26:56.000000 sliderule-3.0.1/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 18:26:56.825001 sliderule-3.0.1/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/_landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/hls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-03-27 18:26:43.000000 sliderule-3.0.1/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.864435 sliderule-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-11 21:16:02.000000 sliderule-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-11 21:16:11.864435 sliderule-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-11 21:16:02.000000 sliderule-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-11 21:16:02.000000 sliderule-3.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 21:16:11.864435 sliderule-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-11 21:16:02.000000 sliderule-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.860435 sliderule-3.0.2/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/arcticdem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24891 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35898 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-11 21:16:02.000000 sliderule-3.0.2/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.860435 sliderule-3.0.2/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-11 21:16:11.000000 sliderule-3.0.2/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 21:16:11.864435 sliderule-3.0.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/hls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-11 21:16:02.000000 sliderule-3.0.2/utils/utils.py
```

### Comparing `sliderule-3.0.1/PKG-INFO` & `sliderule-3.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.1/README.md` & `sliderule-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/setup.py` & `sliderule-3.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,16 @@
     long_description = fh.read()
 
 # get install requirements
 with open('requirements.txt') as fh:
     install_requires = fh.read().splitlines()
 
 # get version
-with open('../../version.txt') as fh:
-    version = fh.read().strip()
-    if version[0] == 'v':
-        version = version[1:]
+with open('version.txt') as fh:
+    version = fh.read().strip()[1:]
 
 # list of all utility scripts to be included with package
 scripts=[os.path.join('utils',f) for f in os.listdir('utils') if f.endswith('.py')]
 
 setup(
     name='sliderule',
     author='SlideRule Developers',
```

### Comparing `sliderule-3.0.1/sliderule/arcticdem.py` & `sliderule-3.0.2/sliderule/arcticdem.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/sliderule/earthdata.py` & `sliderule-3.0.2/sliderule/earthdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
     Parameters
     ----------
         short_name:         str
                             dataset short name as defined in the `NASA CMR Directory <https://cmr.earthdata.nasa.gov/search/site/collections/directory/eosdis>`_
         version:            str
                             dataset version string, leave as None to get latest support version
         polygon:            list
-                            either a single list of longitude,latitude in counter-clockwise order with first and last point matching, defining region of interest (see `polygons </rtd/user_guide/SlideRule.html#polygons>`_), or a list of such lists when the region includes more than one polygon
+                            either a single list of longitude,latitude in counter-clockwise order with first and last point matching, defining region of interest (see `polygons </web/rtd/user_guide/SlideRule.html#polygons>`_), or a list of such lists when the region includes more than one polygon
         time_start:         str
                             starting time for query in format ``<year>-<month>-<day>T<hour>:<minute>:<second>Z``
         time_end:           str
                             ending time for query in format ``<year>-<month>-<day>T<hour>:<minute>:<second>Z``
         return_metadata:    bool
                             flag indicating whether metadata associated with the query is returned back to the user
         name_filter:        str
@@ -510,15 +510,15 @@
     Parameters
     ----------
         short_name:     str
                         dataset short name as defined in the `NASA CMR Directory <https://cmr.earthdata.nasa.gov/search/site/collections/directory/eosdis>`_
         collections:    list
                         list of dataset collections as specified by CMR, leave as None to use defaults
         polygon:        list
-                        either a single list of longitude,latitude in counter-clockwise order with first and last point matching, defining region of interest (see `polygons </rtd/user_guide/SlideRule.html#polygons>`_), or a list of such lists when the region includes more than one polygon
+                        either a single list of longitude,latitude in counter-clockwise order with first and last point matching, defining region of interest (see `polygons </web/rtd/user_guide/SlideRule.html#polygons>`_), or a list of such lists when the region includes more than one polygon
         time_start:     str
                         starting time for query in format ``<year>-<month>-<day>T<hour>:<minute>:<second>Z``
         time_end:       str
                         ending time for query in format ``<year>-<month>-<day>T<hour>:<minute>:<second>Z``
         as_str:         bool
                         whether to return geojson as a dictionary or string
```

### Comparing `sliderule-3.0.1/sliderule/gedi.py` & `sliderule-3.0.2/sliderule/gedi.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,30 +213,30 @@
 ###############################################################################
 # APIs
 ###############################################################################
 
 #
 #  Initialize
 #
-def init (url=sliderule.service_url, verbose=False, max_resources=earthdata.DEFAULT_MAX_REQUESTED_RESOURCES, loglevel=logging.CRITICAL, organization=sliderule.service_org, desired_nodes=None, time_to_live=60):
+def init (url=sliderule.service_url, verbose=False, max_resources=earthdata.DEFAULT_MAX_REQUESTED_RESOURCES, loglevel=logging.CRITICAL, organization=sliderule.service_org, desired_nodes=None, time_to_live=60, bypass_dns=False):
     '''
     Initializes the Python client for use with SlideRule and should be called before other GEDI API calls.
-    This function is a wrapper for the `sliderule.init(...) function </rtds/api_reference/sliderule.html#init>`_.
+    This function is a wrapper for the `sliderule.init(...) function </web/rtds/api_reference/sliderule.html#init>`_.
 
     Parameters
     ----------
         max_resources:  int
                         maximum number of H5 granules to process in the request
 
     Examples
     --------
         >>> from sliderule import gedi
         >>> gedi.init()
     '''
-    sliderule.init(url, verbose, loglevel, organization, desired_nodes, time_to_live, plugins=['gedi'])
+    sliderule.init(url, verbose, loglevel, organization, desired_nodes, time_to_live, bypass_dns, plugins=['gedi'])
     earthdata.set_max_resources(max_resources) # set maximum number of resources allowed per request
 
 #
 #  GEDI L4A
 #
 def gedi04a (parm, resource, asset=DEFAULT_ASSET):
     '''
```

### Comparing `sliderule-3.0.1/sliderule/h5.py` & `sliderule-3.0.2/sliderule/h5.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     Parameters
     ----------
         dataset:    str
                     full path to dataset variable (e.g. ``/gt1r/geolocation/segment_ph_cnt``)
         resource:   str
                     HDF5 filename
         asset:      str
-                    data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                    data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
         datatype:   int
                     the type of data the returned dataset list should be in (datasets that are naturally of a different type undergo a best effort conversion to the specified data type before being returned)
         col:        int
                     the column to read from the dataset for a multi-dimensional dataset; if there are more than two dimensions, all remaining dimensions are flattened out when returned.
         startrow:   int
                     the first row to start reading from in a multi-dimensional dataset (or starting element if there is only one dimension)
         numrows:    int
@@ -115,24 +115,24 @@
     '''
     Reads a list of datasets from an HDF5 file and returns the values of the dataset in a dictionary of lists.
 
     This function is considerably faster than the ``icesat2.h5`` function in that it not only reads the datasets in
     parallel on the server side, but also shares a file context between the reads so that portions of the file that
     need to be read multiple times do not result in multiple requests to S3.
 
-    For a full discussion of the data type conversion options, see `h5 </rtd/api_reference/icesat2.html#h5>`_.
+    For a full discussion of the data type conversion options, see `h5 </web/rtd/api_reference/icesat2.html#h5>`_.
 
     Parameters
     ----------
         datasets:   dict
                     list of full paths to dataset variable (e.g. ``/gt1r/geolocation/segment_ph_cnt``); see below for additional parameters that can be added to each dataset
         resource:   str
                     HDF5 filename
         asset:      str
-                    data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                    data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
 
     Returns
     -------
     dict
         numpy arrays of dataset values, where the keys are the dataset names
 
         The `datasets` dictionary can optionally contain the following elements per entry:
```

### Comparing `sliderule-3.0.1/sliderule/icesat2.py` & `sliderule-3.0.2/sliderule/icesat2.py`

 * *Files 4% similar despite different names*

```diff
@@ -375,52 +375,52 @@
 ###############################################################################
 # APIs
 ###############################################################################
 
 #
 #  Initialize
 #
-def init (url=sliderule.service_url, verbose=False, max_resources=earthdata.DEFAULT_MAX_REQUESTED_RESOURCES, loglevel=logging.CRITICAL, organization=sliderule.service_org, desired_nodes=None, time_to_live=60):
+def init (url=sliderule.service_url, verbose=False, max_resources=earthdata.DEFAULT_MAX_REQUESTED_RESOURCES, loglevel=logging.CRITICAL, organization=sliderule.service_org, desired_nodes=None, time_to_live=60, bypass_dns=False):
     '''
     Initializes the Python client for use with SlideRule and should be called before other ICESat-2 API calls.
-    This function is a wrapper for the `sliderule.init(...) function </rtds/api_reference/sliderule.html#init>`_.
+    This function is a wrapper for the `sliderule.init(...) function </web/rtds/api_reference/sliderule.html#init>`_.
 
     Parameters
     ----------
         max_resources:  int
                         maximum number of H5 granules to process in the request
 
     Examples
     --------
         >>> from sliderule import icesat2
         >>> icesat2.init()
     '''
-    sliderule.init(url, verbose, loglevel, organization, desired_nodes, time_to_live, plugins=['icesat2'])
+    sliderule.init(url, verbose, loglevel, organization, desired_nodes, time_to_live, bypass_dns, plugins=['icesat2'])
     earthdata.set_max_resources(max_resources) # set maximum number of resources allowed per request
 
 #
 #  ATL06
 #
 def atl06 (parm, resource, asset=DEFAULT_ASSET):
     '''
     Performs ATL06-SR processing on ATL03 data and returns geolocated elevations
 
     Parameters
     ----------
     parms:      dict
-                parameters used to configure ATL06-SR algorithm processing (see `Parameters </rtds/user_guide/ICESat-2.html#parameters>`_)
+                parameters used to configure ATL06-SR algorithm processing (see `Parameters </web/rtds/user_guide/ICESat-2.html#parameters>`_)
     resource:   str
                 ATL03 HDF5 filename
     asset:      str
-                data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
 
     Returns
     -------
     GeoDataFrame
-        geolocated elevations (see `Elevations </rtd/user_guide/ICESat-2.html#elevations>`_)
+        geolocated elevations (see `Elevations </web/rtd/user_guide/ICESat-2.html#elevations>`_)
     '''
     return atl06p(parm, asset=asset, resources=[resource])
 
 #
 #  Parallel ATL06
 #
 def atl06p(parm, asset=DEFAULT_ASSET, version=DEFAULT_ICESAT2_SDP_VERSION, callbacks={}, resources=None, keep_id=False):
@@ -435,30 +435,30 @@
         do not actually intersect the region of interest.  This is due to geolocation margin added to all CMR ICESat-2 resources in order to account
         for the spacecraft off-pointing.  The consequence is that SlideRule will return no data for some of the resources and issue a warning statement
         to that effect; this can be ignored and indicates no issue with the data processing.
 
     Parameters
     ----------
         parms:          dict
-                        parameters used to configure ATL06-SR algorithm processing (see `Parameters </rtd/user_guide/ICESat-2.html#parameters>`_)
+                        parameters used to configure ATL06-SR algorithm processing (see `Parameters </web/rtd/user_guide/ICESat-2.html#parameters>`_)
         asset:          str
-                        data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                        data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
         version:        str
                         the version of the ATL03 data to use for processing
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
 
     Returns
     -------
     GeoDataFrame
-        geolocated elevations (see `Elevations </rtd/user_guide/ICESat-2.html#elevations>`_)
+        geolocated elevations (see `Elevations </web/rtd/user_guide/ICESat-2.html#elevations>`_)
 
     Examples
     --------
         >>> from sliderule import icesat2
         >>> icesat2.init("slideruleearth.io", True)
         >>> parms = { "cnf": 4, "ats": 20.0, "cnt": 10, "len": 40.0, "res": 20.0, "maxi": 1 }
         >>> resources = ["ATL03_20181019065445_03150111_003_01.h5"]
@@ -515,24 +515,24 @@
 def atl03s (parm, resource, asset=DEFAULT_ASSET):
     '''
     Subsets ATL03 data given the polygon and time range provided and returns segments of photons
 
     Parameters
     ----------
         parms:      dict
-                    parameters used to configure ATL03 subsetting (see `Parameters </rtd/user_guide/ICESat-2.html#parameters>`_)
+                    parameters used to configure ATL03 subsetting (see `Parameters </web/rtd/user_guide/ICESat-2.html#parameters>`_)
         resource:   str
                     ATL03 HDF5 filename
         asset:      str
-                    data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                    data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
 
     Returns
     -------
     GeoDataFrame
-        ATL03 extents (see `Photon Segments </rtd/user_guide/ICESat-2.html#segmented-photon-data>`_)
+        ATL03 extents (see `Photon Segments </web/rtd/user_guide/ICESat-2.html#segmented-photon-data>`_)
     '''
     return atl03sp(parm, asset=asset, resources=[resource])
 
 #
 #  Parallel Subsetted ATL03
 #
 def atl03sp(parm, asset=DEFAULT_ASSET, version=DEFAULT_ICESAT2_SDP_VERSION, callbacks={}, resources=None, keep_id=False):
@@ -546,30 +546,30 @@
         Note, it is often the case that the list of resources (i.e. granules) returned by the CMR system includes granules that come close, but
         do not actually intersect the region of interest.  This is due to geolocation margin added to all CMR ICESat-2 resources in order to account
         for the spacecraft off-pointing.  The consequence is that SlideRule will return no data for some of the resources and issue a warning statement to that effect; this can be ignored and indicates no issue with the data processing.
 
     Parameters
     ----------
         parms:          dict
-                        parameters used to configure ATL03 subsetting (see `Parameters </rtd/user_guide/ICESat-2.html#parameters>`_)
+                        parameters used to configure ATL03 subsetting (see `Parameters </web/rtd/user_guide/ICESat-2.html#parameters>`_)
         asset:          str
-                        data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                        data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
         version:        str
                         the version of the ATL03 data to return
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
         keep_id:        bool
                         whether to retain the "extent_id" column in the GeoDataFrame for future merges
 
     Returns
     -------
     GeoDataFrame
-        ATL03 segments (see `Photon Segments </rtd/user_guide/ICESat-2.html#photon-segments>`_)
+        ATL03 segments (see `Photon Segments </web/rtd/user_guide/ICESat-2.html#photon-segments>`_)
     '''
     try:
         tstart = time.perf_counter()
 
         # Get List of Resources from CMR (if not specified)
         if resources == None:
             resources = __query_resources(parm, version)
@@ -723,19 +723,19 @@
 def atl08 (parm, resource, asset=DEFAULT_ASSET):
     '''
     Performs ATL08-PhoREAL processing on ATL03 and ATL08 data and returns geolocated elevations
 
     Parameters
     ----------
     parms:      dict
-                parameters used to configure ATL06-SR algorithm processing (see `Parameters </rtds/user_guide/ICESat-2.html#parameters>`_)
+                parameters used to configure ATL06-SR algorithm processing (see `Parameters </web/rtds/user_guide/ICESat-2.html#parameters>`_)
     resource:   str
                 ATL03 HDF5 filename
     asset:      str
-                data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
 
     Returns
     -------
     GeoDataFrame
         geolocated vegatation statistics
     '''
     return atl08p(parm, asset=asset, resources=[resource])
@@ -755,17 +755,17 @@
         do not actually intersect the region of interest.  This is due to geolocation margin added to all CMR ICESat-2 resources in order to account
         for the spacecraft off-pointing.  The consequence is that SlideRule will return no data for some of the resources and issue a warning statement
         to that effect; this can be ignored and indicates no issue with the data processing.
 
     Parameters
     ----------
         parms:          dict
-                        parameters used to configure ATL06-SR algorithm processing (see `Parameters </rtd/user_guide/ICESat-2.html#parameters>`_)
+                        parameters used to configure ATL06-SR algorithm processing (see `Parameters </web/rtd/user_guide/ICESat-2.html#parameters>`_)
         asset:          str
-                        data source asset (see `Assets </rtd/user_guide/ICESat-2.html#assets>`_)
+                        data source asset (see `Assets </web/rtd/user_guide/ICESat-2.html#assets>`_)
         version:        str
                         the version of the ATL03 data to use for processing
         callbacks:      dictionary
                         a callback function that is called for each result record
         resources:      list
                         a list of granules to process (e.g. ["ATL03_20181019065445_03150111_004_01.h5", ...])
         keep_id:        bool
```

### Comparing `sliderule-3.0.1/sliderule/io.py` & `sliderule-3.0.2/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/sliderule/ipxapi.py` & `sliderule-3.0.2/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/sliderule/ipysliderule.py` & `sliderule-3.0.2/sliderule/ipysliderule.py`

 * *Files 0% similar despite different names*

```diff
@@ -2086,16 +2086,16 @@
         self.map.add(self.colorbar)
         plt.close()
 
     @staticmethod
     def default_atl03_fields():
         """List of ATL03 tooltip fields
         """
-        return ['atl03_cnf', 'atl08_class', 'cycle', 'delta_time', 'height',
+        return ['atl03_cnf', 'atl08_class', 'cycle', 'height',
             'pair', 'rgt', 'segment_id', 'track', 'yapc_score']
 
     @staticmethod
     def default_atl06_fields():
         """List of ATL06-SR tooltip fields
         """
-        return ['cycle', 'delta_time', 'dh_fit_dx', 'gt', 'h_mean',
+        return ['cycle', 'dh_fit_dx', 'gt', 'h_mean',
             'h_sigma', 'rgt', 'rms_misfit', 'w_surface_window_final']
```

### Comparing `sliderule-3.0.1/sliderule/sliderule.py` & `sliderule-3.0.2/sliderule/sliderule.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,34 +385,42 @@
 #
 def __initdns():
     local_dns.clear()
 
 #
 # __dnsoverridden - checks if url is already overridden
 #
-def __dnsoverridden(url):
-    name = url.lower()
-    return name in local_dns
+def __dnsoverridden():
+    global service_org, service_url
+    url = service_org + "." + service_url
+    return url.lower() in local_dns
 
 #
 # __jamdns - override the dns entry
 #
-def __jamdns(url, ipaddr):
-    name = url.lower()
-    local_dns[name] = ipaddr
-    logger.info("Overriding DNS for {} with {}".format(name, ipaddr))
+def __jamdns():
+    global service_url, service_org, request_timeout
+    url = service_org + "." + service_url
+    headers = __build_auth_header()
+    host = "https://ps." + service_url + "/api/org_ip_adr/" + service_org + "/"
+    rsps = session.get(host, headers=headers, timeout=request_timeout).json()
+    if rsps["status"] == "SUCCESS":
+        ipaddr = rsps["ip_address"]
+        local_dns[url.lower()] = ipaddr
+        logger.info("Overriding DNS for {} with {}".format(url, ipaddr))
 
 #
 # __override_getaddrinfo - replaces the socket library callback
 #
 socket_getaddrinfo = socket.getaddrinfo
 def __override_getaddrinfo(*args):
-    if args[0] in local_dns:
-        logger.info("getaddrinfo returned {} for {}".format(local_dns[args[0]], args[0]))
-        return socket_getaddrinfo(local_dns[args[0]], *args[1:])
+    url = args[0].lower()
+    if url in local_dns:
+        logger.info("getaddrinfo returned {} for {}".format(local_dns[url], url))
+        return socket_getaddrinfo(local_dns[url], *args[1:])
     else:
         return socket_getaddrinfo(*args)
 socket.getaddrinfo = __override_getaddrinfo
 
 
 ###############################################################################
 # Default Record Processing
@@ -537,44 +545,50 @@
 ###############################################################################
 # APIs
 ###############################################################################
 
 #
 #  Initialize
 #
-def init (url=service_url, verbose=False, loglevel=logging.CRITICAL, organization=service_org, desired_nodes=None, time_to_live=60, plugins=[]):
+def init (url=service_url, verbose=False, loglevel=logging.CRITICAL, organization=service_org, desired_nodes=None, time_to_live=60, bypass_dns=False, plugins=[]):
     '''
     Initializes the Python client for use with SlideRule, and should be called before other ICESat-2 API calls.
     This function is a wrapper for a handful of sliderule functions that would otherwise all have to be called in order to initialize the client.
 
     Parameters
     ----------
         url :           str
                         the IP address or hostname of the SlideRule service (slidereearth.io by default)
         verbose :       bool
                         whether or not user level log messages received from SlideRule generate a Python log message
         loglevel :      int
                         minimum severity of log message to output
         organization:   str
                         SlideRule provisioning system organization the user belongs to (see sliderule.authenticate for details)
+        desired_nodes:  int
+                        requested number of processing nodes in the cluster
+        time_to_live:   int
+                        minimum number of minutes the desired number of nodes should be present in the cluster
+        bypass_dns:     bool
+                        if true then the ip address for the cluster is retrieved from the provisioning system and used directly
         plugins:        list
                         names of the plugins that need to be available on the server
 
     Examples
     --------
         >>> import sliderule
         >>> sliderule.init()
     '''
     if verbose:
         loglevel = logging.INFO
     logging.basicConfig(level=loglevel)
     set_verbose(verbose)
     set_url(url) # configure domain
     authenticate(organization) # configure credentials (if any) for organization
-    scaleout(desired_nodes, time_to_live) # set cluster to desired number of nodes (if permitted based on credentials)
+    scaleout(desired_nodes, time_to_live, bypass_dns) # set cluster to desired number of nodes (if permitted based on credentials)
     check_version(plugins=plugins) # verify compatibility between client and server versions
 
 #
 #  source
 #
 def source (api, parm={}, stream=False, callbacks={}, path="/source", silence=False):
     '''
@@ -583,15 +597,15 @@
     Parameters
     ----------
         api:        str
                     name of the SlideRule endpoint
         parm:       dict
                     dictionary of request parameters
         stream:     bool
-                    whether the request is a **normal** service or a **stream** service (see `De-serialization </rtd/user_guide/SlideRule.html#de-serialization>`_ for more details)
+                    whether the request is a **normal** service or a **stream** service (see `De-serialization </web/rtd/user_guide/SlideRule.html#de-serialization>`_ for more details)
         callbacks:  dict
                     record type callbacks (advanced use)
         path:       str
                     path to api being requested
         silence:    bool
                     whether error log messages should be generated
 
@@ -811,55 +825,54 @@
     except FatalError:
         available_servers = 0
     return available_servers, available_servers
 
 #
 # scaleout
 #
-def scaleout(desired_nodes, time_to_live):
+def scaleout(desired_nodes, time_to_live, bypass_dns):
     '''
     Scale the cluster and wait for cluster to reach desired state
 
     Parameters
     ----------
         desired_nodes:  int
                         the desired number of nodes in the cluster
         time_to_live:   int
                         number of minutes for the desired nodes to run
+        bypass_dns:     bool
+                        the cluster ip address is retrieved from the provisioning system and used directly
 
     Examples
     --------
         >>> import sliderule
-        >>> sliderule.scaleout(4, 300)
+        >>> sliderule.scaleout(4, 300, False)
     '''
     if desired_nodes is None:
         return # nothing needs to be done
     if desired_nodes < 0:
         raise FatalError("Number of desired nodes must be greater than zero ({})".format(desired_nodes))
-    # Initialize DNS - clear cache of DNS lookups for clusters
-    __initdns()
+    # Initialize DNS
+    __initdns() # clear cache of DNS lookups for clusters
+    if bypass_dns:
+        __jamdns() # use ip address for cluster
     # Send Initial Request for Desired Cluster State
     update_available_servers(desired_nodes=desired_nodes, time_to_live=time_to_live)
     start = time.time()
     available_nodes,_ = update_available_servers()
     scale_up_needed = False
     # Wait for Cluster to Reach Desired State
     while available_nodes < desired_nodes:
         scale_up_needed = True
         logger.info("Waiting while cluster scales to desired capacity (currently at {} nodes, desired is {} nodes)... {} seconds".format(available_nodes, desired_nodes, int(time.time() - start)))
         time.sleep(10.0)
         available_nodes,_ = update_available_servers()
         # Override DNS if Cluster is Starting
-        url_to_override = service_org + "." + service_url
-        if available_nodes == 0 and not __dnsoverridden(url_to_override):
-            headers = __build_auth_header()
-            host = "https://ps." + service_url + "/api/org_ip_adr/" + service_org + "/"
-            rsps = session.get(host, headers=headers, timeout=request_timeout).json()
-            if rsps["status"] == "SUCCESS":
-                __jamdns(url_to_override, rsps["ip_address"])
+        if available_nodes == 0 and not __dnsoverridden():
+            __jamdns()
         # Timeout Occurred
         if int(time.time() - start) > MAX_PS_CLUSTER_WAIT_SECS:
             logger.error("Maximum time allowed waiting for cluster has been exceeded")
             break
     # Log Final Message if Cluster Needed State Change
     if scale_up_needed:
         logger.info("Cluster has reached capacity of {} nodes... {} seconds".format(available_nodes, int(time.time() - start)))
```

### Comparing `sliderule-3.0.1/sliderule.egg-info/PKG-INFO` & `sliderule-3.0.2/sliderule.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.1/sliderule.egg-info/SOURCES.txt` & `sliderule-3.0.2/sliderule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/_landsat.py` & `sliderule-3.0.2/utils/_landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/big_query.py` & `sliderule-3.0.2/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.0.2/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.0.2/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.0.2/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/extract_h5_dataset.py` & `sliderule-3.0.2/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/hls.py` & `sliderule-3.0.2/utils/hls.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/icepyx_region.py` & `sliderule-3.0.2/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/landsat.py` & `sliderule-3.0.2/utils/landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/monitor.py` & `sliderule-3.0.2/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/query_cmr.py` & `sliderule-3.0.2/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/query_elevations.py` & `sliderule-3.0.2/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/query_metrics.py` & `sliderule-3.0.2/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/query_photons.py` & `sliderule-3.0.2/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/query_stac.py` & `sliderule-3.0.2/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/query_version.py` & `sliderule-3.0.2/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/region_of_interest.py` & `sliderule-3.0.2/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/results_to_s3.py` & `sliderule-3.0.2/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/stac.py` & `sliderule-3.0.2/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/stream_events.py` & `sliderule-3.0.2/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/tail_events.py` & `sliderule-3.0.2/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.1/utils/utils.py` & `sliderule-3.0.2/utils/utils.py`

 * *Files identical despite different names*

