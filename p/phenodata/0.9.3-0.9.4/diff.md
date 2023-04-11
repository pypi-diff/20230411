# Comparing `tmp/phenodata-0.9.3.tar.gz` & `tmp/phenodata-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phenodata-0.9.3.tar", last modified: Mon Dec 28 16:03:21 2020, max compression
+gzip compressed data, was "dist/phenodata-0.9.4.tar", last modified: Tue Dec 29 03:45:55 2020, max compression
```

## Comparing `phenodata-0.9.3.tar` & `phenodata-0.9.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2020-12-28 16:03:21.012408 phenodata-0.9.3/
--rw-r--r--   0 amo        (501) staff       (20)     4250 2020-12-28 16:03:02.000000 phenodata-0.9.3/CHANGES.rst
--rw-r--r--   0 amo        (501) staff       (20)    34520 2020-12-27 19:39:26.000000 phenodata-0.9.3/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)    22112 2020-12-28 16:03:21.011872 phenodata-0.9.3/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)    16926 2020-12-28 16:00:55.000000 phenodata-0.9.3/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2020-12-28 16:03:21.001223 phenodata-0.9.3/phenodata/
--rw-r--r--   0 amo        (501) staff       (20)      116 2020-12-28 16:03:12.000000 phenodata-0.9.3/phenodata/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     9456 2020-12-27 19:39:26.000000 phenodata-0.9.3/phenodata/command.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2020-12-28 16:03:21.010268 phenodata-0.9.3/phenodata/dwd/
--rw-r--r--   0 amo        (501) staff       (20)        0 2020-12-27 19:39:26.000000 phenodata-0.9.3/phenodata/dwd/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     5462 2020-12-28 14:08:35.000000 phenodata-0.9.3/phenodata/dwd/cdc.py
--rw-r--r--   0 amo        (501) staff       (20)    21376 2020-12-28 15:46:39.000000 phenodata-0.9.3/phenodata/dwd/pheno.py
--rw-r--r--   0 amo        (501) staff       (20)      914 2020-12-27 19:39:26.000000 phenodata-0.9.3/phenodata/dwd/presets.json
--rw-r--r--   0 amo        (501) staff       (20)    10179 2020-12-27 19:39:26.000000 phenodata-0.9.3/phenodata/ftp.py
--rw-r--r--   0 amo        (501) staff       (20)     3408 2020-12-27 19:39:26.000000 phenodata-0.9.3/phenodata/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2020-12-28 16:03:21.006604 phenodata-0.9.3/phenodata.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)    22112 2020-12-28 16:03:20.000000 phenodata-0.9.3/phenodata.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      446 2020-12-28 16:03:20.000000 phenodata-0.9.3/phenodata.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2020-12-28 16:03:20.000000 phenodata-0.9.3/phenodata.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       53 2020-12-28 16:03:20.000000 phenodata-0.9.3/phenodata.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2020-12-27 19:40:17.000000 phenodata-0.9.3/phenodata.egg-info/not-zip-safe
--rw-r--r--   0 amo        (501) staff       (20)      166 2020-12-28 16:03:20.000000 phenodata-0.9.3/phenodata.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       10 2020-12-28 16:03:20.000000 phenodata-0.9.3/phenodata.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2020-12-28 16:03:21.012690 phenodata-0.9.3/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     2737 2020-12-28 16:03:12.000000 phenodata-0.9.3/setup.py
+drwxr-xr-x   0 amo        (502) staff       (20)        0 2020-12-29 03:45:55.000000 phenodata-0.9.4/
+-rw-r--r--   0 amo        (502) staff       (20)     4345 2020-12-29 03:45:01.000000 phenodata-0.9.4/CHANGES.rst
+-rw-r--r--   0 amo        (502) staff       (20)    34520 2020-01-07 00:45:43.000000 phenodata-0.9.4/LICENSE
+-rw-r--r--   0 amo        (502) staff       (20)    22211 2020-12-29 03:45:55.000000 phenodata-0.9.4/PKG-INFO
+-rw-r--r--   0 amo        (502) staff       (20)    16929 2020-12-29 01:05:37.000000 phenodata-0.9.4/README.rst
+drwxr-xr-x   0 amo        (502) staff       (20)        0 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata/
+-rw-r--r--   0 amo        (502) staff       (20)      116 2020-12-29 03:45:46.000000 phenodata-0.9.4/phenodata/__init__.py
+-rw-r--r--   0 amo        (502) staff       (20)     9459 2020-12-29 01:05:53.000000 phenodata-0.9.4/phenodata/command.py
+drwxr-xr-x   0 amo        (502) staff       (20)        0 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata/dwd/
+-rw-r--r--   0 amo        (502) staff       (20)        0 2020-01-07 00:45:43.000000 phenodata-0.9.4/phenodata/dwd/__init__.py
+-rw-r--r--   0 amo        (502) staff       (20)     5462 2020-12-29 00:43:07.000000 phenodata-0.9.4/phenodata/dwd/cdc.py
+-rw-r--r--   0 amo        (502) staff       (20)    21422 2020-12-29 01:51:13.000000 phenodata-0.9.4/phenodata/dwd/pheno.py
+-rw-r--r--   0 amo        (502) staff       (20)      914 2020-01-07 00:45:43.000000 phenodata-0.9.4/phenodata/dwd/presets.json
+-rw-r--r--   0 amo        (502) staff       (20)    10179 2020-01-07 04:08:07.000000 phenodata-0.9.4/phenodata/ftp.py
+-rw-r--r--   0 amo        (502) staff       (20)     3408 2020-01-07 04:03:51.000000 phenodata-0.9.4/phenodata/util.py
+drwxr-xr-x   0 amo        (502) staff       (20)        0 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata.egg-info/
+-rw-r--r--   0 amo        (502) staff       (20)    22211 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (502) staff       (20)      446 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (502) staff       (20)        1 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (502) staff       (20)       53 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (502) staff       (20)        1 2018-03-12 07:53:32.000000 phenodata-0.9.4/phenodata.egg-info/not-zip-safe
+-rw-r--r--   0 amo        (502) staff       (20)      166 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata.egg-info/requires.txt
+-rw-r--r--   0 amo        (502) staff       (20)       10 2020-12-29 03:45:55.000000 phenodata-0.9.4/phenodata.egg-info/top_level.txt
+-rw-r--r--   0 amo        (502) staff       (20)       38 2020-12-29 03:45:55.000000 phenodata-0.9.4/setup.cfg
+-rw-r--r--   0 amo        (502) staff       (20)     2831 2020-12-29 03:45:46.000000 phenodata-0.9.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `phenodata-0.9.3/CHANGES.rst` & `phenodata-0.9.4/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 ###################
 phenodata changelog
 ###################
 
 development
 ===========
 
+2020-12-29 0.9.4
+================
+- Be more graceful if some filter constraints are not given
+
 2020-12-28 0.9.3
 ================
 - Update wrong link to PyPI download count badge
 - Fix virtualenv options
 
 2020-12-28 0.9.2
 ================
```

### Comparing `phenodata-0.9.3/LICENSE` & `phenodata-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phenodata-0.9.3/PKG-INFO` & `phenodata-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phenodata
-Version: 0.9.3
+Version: 0.9.4
 Summary: phenodata is a data acquisition and manipulation toolkit for open access phenology data
 Home-page: https://github.com/earthobservations/phenodata
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3
 Description: .. image:: https://img.shields.io/badge/Python-2.7,%203.7,%203.8,%203.9-green.svg
             :target: https://pypi.org/project/phenodata/
@@ -90,15 +90,15 @@
               phenodata list-stations --source=dwd --dataset=immediate [--all] [--filter=berlin] [--sort=Stationsname] [--format=csv]
               phenodata nearest-station --source=dwd --dataset=immediate --latitude=52.520007 --longitude=13.404954 [--format=csv]
               phenodata nearest-stations --source=dwd --dataset=immediate [--all] --latitude=52.520007 --longitude=13.404954 [--limit=10] [--format=csv]
               phenodata list-quality-levels --source=dwd [--format=csv]
               phenodata list-quality-bytes --source=dwd [--format=csv]
               phenodata list-filenames --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
               phenodata list-urls --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
-              phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
+              phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-de-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
               phenodata drop-cache --source=dwd
               phenodata --version
               phenodata (-h | --help)
         
             Data acquisition options:
               --source=<source>         Data source. Currently "dwd" only.
               --dataset=<dataset>       Data set. Use "immediate" or "annual" for --source=dwd.
@@ -433,28 +433,30 @@
         ==========
         The project and its authors are not affiliated with DWD, USA-NPN or any
         other data provider in any way. It is a sole project from the community
         for making data more accessible in the spirit of open data.
         
 Keywords: dwd usa-npn phenology phenometrics opendata bulk data download information research search
 Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Natural Language :: German
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
 Classifier: Topic :: Database
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
```

### Comparing `phenodata-0.9.3/README.rst` & `phenodata-0.9.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
       phenodata list-stations --source=dwd --dataset=immediate [--all] [--filter=berlin] [--sort=Stationsname] [--format=csv]
       phenodata nearest-station --source=dwd --dataset=immediate --latitude=52.520007 --longitude=13.404954 [--format=csv]
       phenodata nearest-stations --source=dwd --dataset=immediate [--all] --latitude=52.520007 --longitude=13.404954 [--limit=10] [--format=csv]
       phenodata list-quality-levels --source=dwd [--format=csv]
       phenodata list-quality-bytes --source=dwd [--format=csv]
       phenodata list-filenames --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
       phenodata list-urls --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
-      phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
+      phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-de-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
       phenodata drop-cache --source=dwd
       phenodata --version
       phenodata (-h | --help)
 
     Data acquisition options:
       --source=<source>         Data source. Currently "dwd" only.
       --dataset=<dataset>       Data set. Use "immediate" or "annual" for --source=dwd.
```

### Comparing `phenodata-0.9.3/phenodata/command.py` & `phenodata-0.9.4/phenodata/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
       phenodata list-stations --source=dwd --dataset=immediate [--all] [--filter=berlin] [--sort=Stationsname] [--format=csv]
       phenodata nearest-station --source=dwd --dataset=immediate --latitude=52.520007 --longitude=13.404954 [--format=csv]
       phenodata nearest-stations --source=dwd --dataset=immediate [--all] --latitude=52.520007 --longitude=13.404954 [--limit=10] [--format=csv]
       phenodata list-quality-levels --source=dwd [--format=csv]
       phenodata list-quality-bytes --source=dwd [--format=csv]
       phenodata list-filenames --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
       phenodata list-urls --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
-      phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
+      phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-de-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
       phenodata drop-cache --source=dwd
       phenodata --version
       phenodata (-h | --help)
 
     Data acquisition options:
       --source=<source>         Data source. Currently "dwd" only.
       --dataset=<dataset>       Data set. Use "immediate" or "annual" for --source=dwd.
```

### Comparing `phenodata-0.9.3/phenodata/dwd/cdc.py` & `phenodata-0.9.4/phenodata/dwd/cdc.py`

 * *Files identical despite different names*

### Comparing `phenodata-0.9.3/phenodata/dwd/pheno.py` & `phenodata-0.9.4/phenodata/dwd/pheno.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
         - Obtain query options
         - Compute DataFrame with combined observation data
         - Apply a bunch of filters to the result data
         """
 
         # Acquire data
-        observations = self.query(partition=options['partition'], files=options['filename'])
+        observations = self.query(partition=options['partition'], files=options.get('filename'))
 
         # Sanity checks
         if observations is None:
             return
 
         # Filter data
         observations = self.flux(observations, criteria=options)
@@ -372,15 +372,15 @@
         # Lowlevel filtering based on IDs
         # For each designated field, add ``.isin`` criteria to "boolean index" expression
         expression = True
         for key, field in list(isin_map.items()):
             if field not in results:
                 continue
             reference = results[field]
-            if criteria[key]:
+            if key in criteria and criteria[key]:
                 expression &= reference.isin(criteria[key])
 
         # Apply filter expression to DataFrame
         if type(expression) is not bool:
             results = results[expression]
 
 
@@ -399,15 +399,15 @@
         # Remember columns of current DataFrame
         columns = results.columns
 
         expression = True
         is_megaframe = False
         for field, reference_fields in list(patterns_map.items()):
 
-            if criteria[field]:
+            if field in criteria and criteria[field]:
 
                 # Create megaframe as this will contain all information required for advanced searching
                 if not is_megaframe:
                     is_megaframe = True
                     results = self.create_megaframe(results)
 
                 # The list of patterns to search for. Any match counts.
```

### Comparing `phenodata-0.9.3/phenodata/dwd/presets.json` & `phenodata-0.9.4/phenodata/dwd/presets.json`

 * *Files identical despite different names*

### Comparing `phenodata-0.9.3/phenodata/ftp.py` & `phenodata-0.9.4/phenodata/ftp.py`

 * *Files identical despite different names*

### Comparing `phenodata-0.9.3/phenodata/util.py` & `phenodata-0.9.4/phenodata/util.py`

 * *Files identical despite different names*

### Comparing `phenodata-0.9.3/phenodata.egg-info/PKG-INFO` & `phenodata-0.9.4/phenodata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phenodata
-Version: 0.9.3
+Version: 0.9.4
 Summary: phenodata is a data acquisition and manipulation toolkit for open access phenology data
 Home-page: https://github.com/earthobservations/phenodata
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3
 Description: .. image:: https://img.shields.io/badge/Python-2.7,%203.7,%203.8,%203.9-green.svg
             :target: https://pypi.org/project/phenodata/
@@ -90,15 +90,15 @@
               phenodata list-stations --source=dwd --dataset=immediate [--all] [--filter=berlin] [--sort=Stationsname] [--format=csv]
               phenodata nearest-station --source=dwd --dataset=immediate --latitude=52.520007 --longitude=13.404954 [--format=csv]
               phenodata nearest-stations --source=dwd --dataset=immediate [--all] --latitude=52.520007 --longitude=13.404954 [--limit=10] [--format=csv]
               phenodata list-quality-levels --source=dwd [--format=csv]
               phenodata list-quality-bytes --source=dwd [--format=csv]
               phenodata list-filenames --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
               phenodata list-urls --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--year=2017]
-              phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
+              phenodata (observations|forecast) --source=dwd --dataset=immediate --partition=recent [--filename=Hasel,Schneegloeckchen] [--station-id=164,717] [--species-id=113,127] [--phase-id=5] [--quality-level=10] [--quality-byte=1,2,3] [--station=berlin,brandenburg] [--species=hazel,snowdrop] [--species-preset=mellifera-de-primary] [--phase=flowering] [--quality=ROUTKLI] [--year=2017] [--humanize] [--show-ids] [--language=german] [--long-station] [--sort=Datum] [--format=csv] [--verbose]
               phenodata drop-cache --source=dwd
               phenodata --version
               phenodata (-h | --help)
         
             Data acquisition options:
               --source=<source>         Data source. Currently "dwd" only.
               --dataset=<dataset>       Data set. Use "immediate" or "annual" for --source=dwd.
@@ -433,28 +433,30 @@
         ==========
         The project and its authors are not affiliated with DWD, USA-NPN or any
         other data provider in any way. It is a sole project from the community
         for making data more accessible in the spirit of open data.
         
 Keywords: dwd usa-npn phenology phenometrics opendata bulk data download information research search
 Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Natural Language :: German
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
 Classifier: Topic :: Database
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
```

### Comparing `phenodata-0.9.3/setup.py` & `phenodata-0.9.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,35 @@
     'future',
 ]
 
 test_requires = [
 ]
 
 setup(name='phenodata',
-    version='0.9.3',
+    version='0.9.4',
     description='phenodata is a data acquisition and manipulation toolkit for open access phenology data',
     long_description=README,
     license="AGPL 3",
     classifiers=[
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Natural Language :: English",
         "Natural Language :: German",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python",
         "Topic :: Database",
         "Topic :: Education",
         "Topic :: Internet :: File Transfer Protocol (FTP)",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Atmospheric Science",
```

