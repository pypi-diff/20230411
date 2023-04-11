# Comparing `tmp/rio-tiler-pds-0.7.0.tar.gz` & `tmp/rio-tiler-pds-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-tiler-pds-0.7.0.tar", last modified: Wed Jun  8 14:04:50 2022, max compression
+gzip compressed data, was "rio-tiler-pds-0.8.0.tar", last modified: Tue Apr 11 19:04:56 2023, max compression
```

## Comparing `rio-tiler-pds-0.7.0.tar` & `rio-tiler-pds-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,31 @@
--rw-r--r--   0        0        0      217 2022-06-08 13:58:32.815474 rio-tiler-pds-0.7.0/.bumpversion.cfg
--rw-r--r--   0        0        0      136 2022-06-08 13:56:17.791282 rio-tiler-pds-0.7.0/.flake8
--rw-r--r--   0        0        0     1232 2020-08-26 13:50:24.000000 rio-tiler-pds-0.7.0/.gitignore
--rw-r--r--   0        0        0      674 2022-06-08 13:56:17.791977 rio-tiler-pds-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2020-08-25 14:56:12.000000 rio-tiler-pds-0.7.0/AUTHORS.txt
--rw-r--r--   0        0        0     4859 2022-06-08 13:58:03.680354 rio-tiler-pds-0.7.0/CHANGES.md
--rw-r--r--   0        0        0     1506 2020-07-21 20:32:36.000000 rio-tiler-pds-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0    14232 2021-11-29 16:41:44.475889 rio-tiler-pds-0.7.0/README.md
--rw-r--r--   0        0        0     1603 2022-06-08 14:04:31.112179 rio-tiler-pds-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       99 2022-06-08 13:58:32.815335 rio-tiler-pds-0.7.0/rio_tiler_pds/__init__.py
--rw-r--r--   0        0        0      132 2021-01-04 23:26:31.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/cbers/__init__.py
--rw-r--r--   0        0        0       90 2021-01-04 23:26:31.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/cbers/aws/__init__.py
--rw-r--r--   0        0        0     1981 2022-06-07 23:34:24.632868 rio-tiler-pds-0.7.0/rio_tiler_pds/cbers/aws/cbers4.py
--rw-r--r--   0        0        0     2602 2022-06-08 13:56:17.793882 rio-tiler-pds-0.7.0/rio_tiler_pds/cbers/utils.py
--rw-r--r--   0        0        0      474 2020-10-03 13:35:36.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/errors.py
--rw-r--r--   0        0        0      138 2021-01-04 23:26:31.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/landsat/__init__.py
--rw-r--r--   0        0        0      179 2021-11-09 13:18:44.835047 rio-tiler-pds-0.7.0/rio_tiler_pds/landsat/aws/__init__.py
--rw-r--r--   0        0        0    11773 2022-06-07 23:53:22.632296 rio-tiler-pds-0.7.0/rio_tiler_pds/landsat/aws/landsat8.py
--rw-r--r--   0        0        0     4024 2022-06-07 23:34:24.633494 rio-tiler-pds-0.7.0/rio_tiler_pds/landsat/aws/landsat_collection2.py
--rw-r--r--   0        0        0     6704 2022-06-08 13:56:17.794103 rio-tiler-pds-0.7.0/rio_tiler_pds/landsat/utils.py
--rw-r--r--   0        0        0      132 2021-01-04 23:26:31.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/modis/__init__.py
--rw-r--r--   0        0        0      238 2021-01-04 23:26:31.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/modis/aws/__init__.py
--rw-r--r--   0        0        0     3759 2022-06-07 23:34:24.633717 rio-tiler-pds-0.7.0/rio_tiler_pds/modis/aws/modis_astraea.py
--rw-r--r--   0        0        0     3266 2022-06-07 23:34:24.633920 rio-tiler-pds-0.7.0/rio_tiler_pds/modis/aws/modis_pds.py
--rw-r--r--   0        0        0    24642 2020-11-26 18:55:10.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/modis/modland_grid.py
--rw-r--r--   0        0        0     1326 2022-06-08 13:56:17.794244 rio-tiler-pds-0.7.0/rio_tiler_pds/modis/utils.py
--rw-r--r--   0        0        0      163 2021-01-04 23:26:31.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/__init__.py
--rw-r--r--   0        0        0      200 2020-11-09 16:44:02.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/aws/__init__.py
--rw-r--r--   0        0        0     2898 2022-06-07 23:34:24.634127 rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/aws/sentinel1.py
--rw-r--r--   0        0        0     8629 2022-06-07 23:34:24.634351 rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/aws/sentinel2.py
--rw-r--r--   0        0        0     5426 2022-06-08 13:56:17.794399 rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/utils.py
--rw-r--r--   0        0        0      322 2021-01-04 23:26:31.000000 rio-tiler-pds-0.7.0/rio_tiler_pds/utils.py
--rw-r--r--   0        0        0    15517 1970-01-01 00:00:00.000000 rio-tiler-pds-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1266 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/.gitignore
+-rw-r--r--   0        0        0      795 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/AUTHORS.txt
+-rw-r--r--   0        0        0     5159 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/CHANGES.md
+-rw-r--r--   0        0        0     1506 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0    15113 2023-04-11 19:04:36.111651 rio-tiler-pds-0.8.0/README.md
+-rw-r--r--   0        0        0     2152 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/aws/__init__.py
+-rw-r--r--   0        0        0     2055 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/aws/cbers4.py
+-rw-r--r--   0        0        0     2602 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/utils.py
+-rw-r--r--   0        0        0      474 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/errors.py
+-rw-r--r--   0        0        0      138 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/aws/__init__.py
+-rw-r--r--   0        0        0     3981 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/aws/landsat_collection2.py
+-rw-r--r--   0        0        0     5249 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/utils.py
+-rw-r--r--   0        0        0      132 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/__init__.py
+-rw-r--r--   0        0        0     3750 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_astraea.py
+-rw-r--r--   0        0        0     3257 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_pds.py
+-rw-r--r--   0        0        0    24642 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/modland_grid.py
+-rw-r--r--   0        0        0     1326 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/modis/utils.py
+-rw-r--r--   0        0        0      163 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/__init__.py
+-rw-r--r--   0        0        0     2877 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel1.py
+-rw-r--r--   0        0        0     9492 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel2.py
+-rw-r--r--   0        0        0     5426 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/utils.py
+-rw-r--r--   0        0        0     1326 2023-04-11 19:04:36.115651 rio-tiler-pds-0.8.0/rio_tiler_pds/utils.py
+-rw-r--r--   0        0        0    16425 1970-01-01 00:00:00.000000 rio-tiler-pds-0.8.0/PKG-INFO
```

### Comparing `rio-tiler-pds-0.7.0/.gitignore` & `rio-tiler-pds-0.8.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
 
+# Pycharm project settings
+.idea
+
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
```

### Comparing `rio-tiler-pds-0.7.0/CHANGES.md` & `rio-tiler-pds-0.8.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Release Notes
 
+## 0.8.0 (2023-04-11)
+
+* remove Landsat 8 Collection 1
+* remove python 3.7 and add python 3.10/3.11 support
+* switch to ruff
+* fix issue with latest STAC Items for Sentinel-2-l2a-cogs (author @dvd3v, https://github.com/cogeotiff/rio-tiler-pds/pull/64)
+* update rio-tiler requirement to `>=4.0,<5.0`
+
 ## 0.7.0 (2022-06-08)
 
 * enable `bucket` and `prefix_pattern` as input (@author @f-skold, https://github.com/cogeotiff/rio-tiler-pds/pull/61)
 * switch to `pyproject.toml`
 
 ## 0.6.0 (2021-11-29)
```

### Comparing `rio-tiler-pds-0.7.0/LICENSE.txt` & `rio-tiler-pds-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.7.0/README.md` & `rio-tiler-pds-0.8.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,23 +7,23 @@
   <em>A rio-tiler plugin to read from publicly-available datasets.</em>
 </p>
 <p align="center">
   <a href="https://github.com/cogeotiff/rio-tiler-pds/actions?query=workflow%3ACI" target="_blank">
       <img src="https://github.com/cogeotiff/rio-tiler-pds/workflows/CI/badge.svg" alt="Test">
   </a>
   <a href="https://codecov.io/gh/cogeotiff/rio-tiler-pds" target="_blank">
-      <img src="https://codecov.io/gh/cogeotiff/rio-tiler-pds/branch/master/graph/badge.svg" alt="Coverage">
+      <img src="https://codecov.io/gh/cogeotiff/rio-tiler-pds/branch/main/graph/badge.svg" alt="Coverage">
   </a>
   <a href="https://pypi.org/project/rio-tiler-pds" target="_blank">
       <img src="https://img.shields.io/pypi/v/rio-tiler-pds?color=%2334D058&label=pypi%20package" alt="Package version">
   </a>
   <a href="https://pypistats.org/packages/rio-tiler-pds" target="_blank">
       <img src="https://img.shields.io/pypi/dm/rio-tiler-pds.svg" alt="Downloads">
   </a>
-  <a href="https://github.com/cogeotiff/rio-tiler-pds/blob/master/LICENSE.txt" target="_blank">
+  <a href="https://github.com/cogeotiff/rio-tiler-pds/blob/main/LICENSE.txt" target="_blank">
       <img src="https://img.shields.io/github/license/cogeotiff/rio-tiler-pds.svg" alt="Lincense">
   </a>
 </p>
 
 **Important** This is the new module for rio-tiler missions specific (ref: https://github.com/cogeotiff/rio-tiler/issues/195)
 
 ---
@@ -54,32 +54,28 @@
 
 | Data                                      | Level/Product                               | Format                     | Owner                      | Region       | Bucket Type        |
 | ----------------------------------------- | ------------------------------------------- | -------------------------- | -------------------------- | ------------ | ------------------ |
 | [Sentinel 2][s2_l1c_jp2]                  | L1C                                         | JPEG2000                   | Sinergise / AWS            | eu-central-1 | **Requester-pays** |
 | [Sentinel 2][s2_l2a_jp2]                  | L2A                                         | JPEG2000                   | Sinergise / AWS            | eu-central-1 | **Requester-pays** |
 | [Sentinel 2][s2_l2a_cog]                  | L2A                                         | COG                        | Digital Earth Africa / AWS | us-west-2    | Public             |
 | [Sentinel 1][s1_l1c_cog]                  | L1C                                         | COG (Internal GCPS)        | Sinergise / AWS            | eu-central-1 | **Requester-pays** |
-| [Landsat 8*][l8_l1_cog]                   | L1                                          | GTiff (External Overviews) | Planet / AWS               | us-west-2    | Public             |
 | [Landsat Collection 2][landsat_c2_cog]    | L1,L2                                       | COG                        | USGS / AWS                 | us-west-2    | **Requester-pays** |
 | [CBERS 4/4A][cbers_cog]                   | L2/L4                                       | COG                        | AMS Kepler / AWS           | us-east-1    | **Requester-pays** |
 | [MODIS (modis-pds)][modis_pds]            | MCD43A4, MOD09GQ, MYD09GQ, MOD09GA, MYD09GA | GTiff (External Overviews) | -                          | us-west-2    | Public             |
 | [MODIS (astraea-opendata)][modis_astraea] | MCD43A4, MOD11A1, MOD13A1, MYD11A1 MYD13A1  | COG                        | Astraea / AWS              | us-west-2    | **Requester-pays** |
 
 [s2_l1c_jp2]: https://registry.opendata.aws/sentinel-2/
 [s2_l2a_jp2]: https://registry.opendata.aws/sentinel-2/
 [s2_l2a_cog]: https://registry.opendata.aws/sentinel-2-l2a-cogs/
 [s1_l1c_cog]: https://registry.opendata.aws/sentinel-1/
-[l8_l1_cog]: https://registry.opendata.aws/landsat-8/
 [landsat_c2_cog]: https://www.usgs.gov/core-science-systems/nli/landsat/landsat-commercial-cloud-data-access
 [cbers_cog]: https://registry.opendata.aws/cbers/
 [modis_pds]: https://docs.opendata.aws/modis-pds/readme.html
 [modis_astraea]: https://registry.opendata.aws/modis-astraea/
 
-`*` Landsat 8 Collection 1 reader has been deprecated because the `landsat-pds` will be deleted on July 1st 2021. For new applications, using Collection 2 is suggested.
-
 **Adding more dataset**:
 
 If you know of another publicly-available dataset that can easily be described
 with a "scene id", please feel free to [open an
 issue](https://github.com/cogeotiff/rio-tiler-pds/issues/new).
 
 ## Warnings
@@ -110,15 +106,15 @@
 ## Overview
 
 ### Readers
 
 Each dataset has its own submodule (e.g sentinel2: `rio_tiler_pds.sentinel.aws`)
 
 ```python
-from rio_tiler_pds.landsat.aws import L8Reader, LandsatC2Reader
+from rio_tiler_pds.landsat.aws import LandsatC2Reader
 from rio_tiler_pds.sentinel.aws import S1L1CReader
 from rio_tiler_pds.sentinel.aws import (
     S2JP2Reader,  # JPEG2000
     S2COGReader,   # COG
 )
 
 from rio_tiler_pds.cbers.aws import CBERSReader
@@ -127,16 +123,16 @@
 
 All Readers are subclass of [`rio_tiler.io.BaseReader`](https://github.com/cogeotiff/rio-tiler/blob/f917d0eaf27f8644f3bb18856a63fe45eeb4a2ef/rio_tiler/io/base.py#L17) and inherit its properties/methods.
 
 #### Properties
 - **bounds**: Scene bounding box
 - **crs**: CRS of the bounding box
 - **geographic_bounds**: bounding box in geographic projection (e.g WGS84)
-- **minzoom**: WebMercator MinZoom (e.g 7 for Landsat8)
-- **maxzoom**: WebMercator MaxZoom (e.g 12 for Landsat8)
+- **minzoom**: WebMercator MinZoom (e.g 7 for Landsat 8)
+- **maxzoom**: WebMercator MaxZoom (e.g 12 for Landsat 8)
 
 #### Methods
 
 - **info**: Returns band's simple info (e.g nodata, band_descriptions, ....)
 - **statistics**: Returns band's statistics (percentile, histogram, ...)
 - **tile**: Read web mercator map tile from bands
 - **part**: Extract part of bands
@@ -152,41 +148,62 @@
 All readers take scene id as main input. The **scene id** is used internaly by the reader to derive the full path of the data.
 
 e.g: Landsat on AWS
 
 Because the Landsat AWS PDS follows a regular schema to store the data (`s3://{bucket}/c1/L8/{path}/{row}/{scene}/{scene}_{band}.TIF"`), we can easily reconstruct the full band's path by parsing the scene id.
 
 ```python
-from rio_tiler_pds.landsat.aws import L8Reader
+from rio_tiler_pds.landsat.aws import LandsatC2Reader
 from rio_tiler_pds.landsat.utils import sceneid_parser
 
-sceneid_parser("LC08_L1TP_016037_20170813_20170814_01_RT")
+sceneid_parser("LC08_L2SP_001062_20201031_20201106_02_T2")
 
-> {
-  'sensor': 'C',
-  'satellite': '08',
-  'processingCorrectionLevel': 'L1TP',
-  'path': '016',
-  'row': '037',
-  'acquisitionYear': '2017',
-  'acquisitionMonth': '08',
-  'acquisitionDay': '13',
-  'processingYear': '2017',
-  'processingMonth': '08',
-  'processingDay': '14',
-  'collectionNumber': '01',
-  'collectionCategory': 'RT',
-  'scene': 'LC08_L1TP_016037_20170813_20170814_01_RT',
-  'date': '2017-08-13'
-}
+> {'sensor': 'C',
+ 'satellite': '08',
+ 'processingCorrectionLevel': 'L2SP',
+ 'path': '001',
+ 'row': '062',
+ 'acquisitionYear': '2020',
+ 'acquisitionMonth': '10',
+ 'acquisitionDay': '31',
+ 'processingYear': '2020',
+ 'processingMonth': '11',
+ 'processingDay': '06',
+ 'collectionNumber': '02',
+ 'collectionCategory': 'T2',
+ 'scene': 'LC08_L2SP_001062_20201031_20201106_02_T2',
+ 'date': '2020-10-31',
+ '_processingLevelNum': '2',
+ 'category': 'standard',
+ 'sensor_name': 'oli-tirs',
+ '_sensor_s3_prefix': 'oli-tirs',
+ 'bands': ('QA_PIXEL',
+  'QA_RADSAT',
+  'SR_B1',
+  'SR_B2',
+  'SR_B3',
+  'SR_B4',
+  'SR_B5',
+  'SR_B6',
+  'SR_B7',
+  'SR_QA_AEROSOL',
+  'ST_ATRAN',
+  'ST_B10',
+  'ST_CDIST',
+  'ST_DRAD',
+  'ST_EMIS',
+  'ST_EMSD',
+  'ST_QA',
+  'ST_TRAD',
+  'ST_URAD')}
 
-with L8Reader("LC08_L1TP_016037_20170813_20170814_01_RT") as landsat:
-    print(landsat._get_band_url("B1"))
+with LandsatC2Reader("LC08_L2SP_001062_20201031_20201106_02_T2") as landsat:
+    print(landsat._get_band_url("SR_B2"))
 
-> s3://landsat-pds/c1/L8/016/037/LC08_L1TP_016037_20170813_20170814_01_RT/LC08_L1TP_016037_20170813_20170814_01_RT_B1.TIF
+> s3://usgs-landsat/collection02/level-2/standard/oli-tirs/2020/001/062/LC08_L2SP_001062_20201031_20201106_02_T2/LC08_L2SP_001062_20201031_20201106_02_T2_SR_B2.TIF
 ```
 
 Each dataset has a specific scene id format:
 
 !!! note "Scene ID formats"
 
     - Landsat
@@ -215,36 +232,50 @@
         - example: `MCD43A4.A2017006.h21v11.006.2017018074804`
 
 ### Band Per Asset/File
 
 `rio-tiler-pds` Readers assume that bands (e.g eo:band in STAC) are stored in separate files.
 
 ```bash
-$ aws s3 ls landsat-pds/c1/L8/013/031/LC08_L1TP_013031_20130930_20170308_01_T1/
-
-LC08_L1TP_013031_20130930_20170308_01_T1_B1.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B10.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B11.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B2.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B3.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B4.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B5.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B6.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B7.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B8.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B9.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_BQA.TIF
+$ aws s3 ls s3://usgs-landsat/collection02/level-2/standard/oli-tirs/2020/001/062/LC08_L2SP_001062_20201031_20201106_02_T2/ --request-payer
+LC08_L2SP_001062_20201031_20201106_02_T2_ANG.txt
+LC08_L2SP_001062_20201031_20201106_02_T2_MTL.json
+LC08_L2SP_001062_20201031_20201106_02_T2_MTL.txt
+LC08_L2SP_001062_20201031_20201106_02_T2_MTL.xml
+LC08_L2SP_001062_20201031_20201106_02_T2_QA_PIXEL.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_QA_RADSAT.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B1.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B2.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B3.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B4.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B5.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B6.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B7.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_QA_AEROSOL.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_stac.json
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_ATRAN.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_B10.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_CDIST.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_DRAD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_EMIS.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_EMSD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_QA.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_TRAD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_URAD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_stac.json
+LC08_L2SP_001062_20201031_20201106_02_T2_thumb_large.jpeg
+LC08_L2SP_001062_20201031_20201106_02_T2_thumb_small.jpeg
 ```
 
 When reading data or metadata, readers will merge them.
 
 e.g
 ```python
 with S2COGReader("S2A_L2A_20170729_19UDP_0") as sentinel:
-    img = sentinel.tile(77, 89, 8, bands=("B01", "B02")
+    img = sentinel.tile(78, 89, 8, bands=("B01", "B02"))
     assert img.data.shape == (2, 256, 256)
 
     stats = sentinel.statistics(bands=("B01", "B02"))
     print(stats)
     >> {
       'B01': BandStatistics(
         min=2.0,
@@ -291,22 +322,22 @@
 
       print(stats["B01"].min)
       >> 2.0
 ```
 
 ## Changes
 
-See [CHANGES.md](https://github.com/cogeotiff/rio-tiler-pds/blob/master/CHANGES.md).
+See [CHANGES.md](https://github.com/cogeotiff/rio-tiler-pds/blob/main/CHANGES.md).
 
 ## Contribution & Development
 
-See [CONTRIBUTING.md](https://github.com/cogeotiff/rio-tiler/blob/master/CONTRIBUTING.md)
+See [CONTRIBUTING.md](https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md)
 
 ## License
 
-See [LICENSE.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/master/LICENSE.txt)
+See [LICENSE.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/main/LICENSE.txt)
 
 ## Authors
 
 The rio-tiler project was begun at Mapbox and has been transferred in January 2019.
 
-See [AUTHORS.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/master/AUTHORS.txt) for a listing of individual contributors.
+See [AUTHORS.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/main/AUTHORS.txt) for a listing of individual contributors.
```

#### html2text {}

```diff
@@ -13,89 +13,90 @@
 ----------------------------------------- | -------------------------- | ------
 -------------------- | ------------ | ------------------ | | [Sentinel 2]
 [s2_l1c_jp2] | L1C | JPEG2000 | Sinergise / AWS | eu-central-1 | **Requester-
 pays** | | [Sentinel 2][s2_l2a_jp2] | L2A | JPEG2000 | Sinergise / AWS | eu-
 central-1 | **Requester-pays** | | [Sentinel 2][s2_l2a_cog] | L2A | COG |
 Digital Earth Africa / AWS | us-west-2 | Public | | [Sentinel 1][s1_l1c_cog] |
 L1C | COG (Internal GCPS) | Sinergise / AWS | eu-central-1 | **Requester-pays**
-| | [Landsat 8*][l8_l1_cog] | L1 | GTiff (External Overviews) | Planet / AWS |
-us-west-2 | Public | | [Landsat Collection 2][landsat_c2_cog] | L1,L2 | COG |
-USGS / AWS | us-west-2 | **Requester-pays** | | [CBERS 4/4A][cbers_cog] | L2/L4
-| COG | AMS Kepler / AWS | us-east-1 | **Requester-pays** | | [MODIS (modis-
-pds)][modis_pds] | MCD43A4, MOD09GQ, MYD09GQ, MOD09GA, MYD09GA | GTiff
-(External Overviews) | - | us-west-2 | Public | | [MODIS (astraea-opendata)]
+| | [Landsat Collection 2][landsat_c2_cog] | L1,L2 | COG | USGS / AWS | us-
+west-2 | **Requester-pays** | | [CBERS 4/4A][cbers_cog] | L2/L4 | COG | AMS
+Kepler / AWS | us-east-1 | **Requester-pays** | | [MODIS (modis-pds)]
+[modis_pds] | MCD43A4, MOD09GQ, MYD09GQ, MOD09GA, MYD09GA | GTiff (External
+Overviews) | - | us-west-2 | Public | | [MODIS (astraea-opendata)]
 [modis_astraea] | MCD43A4, MOD11A1, MOD13A1, MYD11A1 MYD13A1 | COG | Astraea /
 AWS | us-west-2 | **Requester-pays** | [s2_l1c_jp2]: https://
 registry.opendata.aws/sentinel-2/ [s2_l2a_jp2]: https://registry.opendata.aws/
 sentinel-2/ [s2_l2a_cog]: https://registry.opendata.aws/sentinel-2-l2a-cogs/
-[s1_l1c_cog]: https://registry.opendata.aws/sentinel-1/ [l8_l1_cog]: https://
-registry.opendata.aws/landsat-8/ [landsat_c2_cog]: https://www.usgs.gov/core-
-science-systems/nli/landsat/landsat-commercial-cloud-data-access [cbers_cog]:
-https://registry.opendata.aws/cbers/ [modis_pds]: https://docs.opendata.aws/
-modis-pds/readme.html [modis_astraea]: https://registry.opendata.aws/modis-
-astraea/ `*` Landsat 8 Collection 1 reader has been deprecated because the
-`landsat-pds` will be deleted on July 1st 2021. For new applications, using
-Collection 2 is suggested. **Adding more dataset**: If you know of another
-publicly-available dataset that can easily be described with a "scene id",
-please feel free to [open an issue](https://github.com/cogeotiff/rio-tiler-pds/
-issues/new). ## Warnings #### Requester-pays Buckets On AWS, `sentinel2`,
-`sentinel1`, `cbers` and `modis` (in astraea-opendata) datasets are stored in
-[_requester pays_](https://docs.aws.amazon.com/AmazonS3/latest/dev/
-RequesterPaysBuckets.html) buckets. This means that the cost of GET and LIST
-requests and egress fees for downloading files outside the AWS region will be
-charged to the _accessing users_, not the organization hosting the bucket. For
-`rio-tiler` and `rio-tiler-pds` to work with such buckets, you'll need to set
-`AWS_REQUEST_PAYER="requester"` in your shell environment. #### Partial reading
-on Cloud hosted dataset When reading data, `rio-tiler-pds` performs _partial_
-reads when possible. Hence performance will be best on data stored as [Cloud
-Optimized GeoTIFF (COG)](http://cogeo.org). It's important to note that
+[s1_l1c_cog]: https://registry.opendata.aws/sentinel-1/ [landsat_c2_cog]:
+https://www.usgs.gov/core-science-systems/nli/landsat/landsat-commercial-cloud-
+data-access [cbers_cog]: https://registry.opendata.aws/cbers/ [modis_pds]:
+https://docs.opendata.aws/modis-pds/readme.html [modis_astraea]: https://
+registry.opendata.aws/modis-astraea/ **Adding more dataset**: If you know of
+another publicly-available dataset that can easily be described with a "scene
+id", please feel free to [open an issue](https://github.com/cogeotiff/rio-
+tiler-pds/issues/new). ## Warnings #### Requester-pays Buckets On AWS,
+`sentinel2`, `sentinel1`, `cbers` and `modis` (in astraea-opendata) datasets
+are stored in [_requester pays_](https://docs.aws.amazon.com/AmazonS3/latest/
+dev/RequesterPaysBuckets.html) buckets. This means that the cost of GET and
+LIST requests and egress fees for downloading files outside the AWS region will
+be charged to the _accessing users_, not the organization hosting the bucket.
+For `rio-tiler` and `rio-tiler-pds` to work with such buckets, you'll need to
+set `AWS_REQUEST_PAYER="requester"` in your shell environment. #### Partial
+reading on Cloud hosted dataset When reading data, `rio-tiler-pds` performs
+_partial_ reads when possible. Hence performance will be best on data stored as
+[Cloud Optimized GeoTIFF (COG)](http://cogeo.org). It's important to note that
 **Sentinel-2 scenes hosted on AWS are not in Cloud Optimized format but in
 JPEG2000**. Partial reads from JPEG2000 files are inefficient, and GDAL (the
 library underlying `rio-tiler-pds` and `rasterio`) will need to make **many GET
 requests** and transfer a lot of data. This will be both slow and expensive,
 since AWS's JPEG2000 collection of Sentinel 2 data is stored in a requester
 pays bucket. Ref: [Do you really want people using your data](https://
 medium.com/@_VincentS_/do-you-really-want-people-using-your-data-ec94cd94dc3f)
 blog post. ## Overview ### Readers Each dataset has its own submodule (e.g
 sentinel2: `rio_tiler_pds.sentinel.aws`) ```python from
-rio_tiler_pds.landsat.aws import L8Reader, LandsatC2Reader from
+rio_tiler_pds.landsat.aws import LandsatC2Reader from
 rio_tiler_pds.sentinel.aws import S1L1CReader from rio_tiler_pds.sentinel.aws
 import ( S2JP2Reader, # JPEG2000 S2COGReader, # COG ) from
 rio_tiler_pds.cbers.aws import CBERSReader from rio_tiler_pds.modis.aws import
 MODISPDSReader, MODISASTRAEAReader ``` All Readers are subclass of
 [`rio_tiler.io.BaseReader`](https://github.com/cogeotiff/rio-tiler/blob/
 f917d0eaf27f8644f3bb18856a63fe45eeb4a2ef/rio_tiler/io/base.py#L17) and inherit
 its properties/methods. #### Properties - **bounds**: Scene bounding box -
 **crs**: CRS of the bounding box - **geographic_bounds**: bounding box in
 geographic projection (e.g WGS84) - **minzoom**: WebMercator MinZoom (e.g 7 for
-Landsat8) - **maxzoom**: WebMercator MaxZoom (e.g 12 for Landsat8) #### Methods
-- **info**: Returns band's simple info (e.g nodata, band_descriptions, ....) -
-**statistics**: Returns band's statistics (percentile, histogram, ...) -
-**tile**: Read web mercator map tile from bands - **part**: Extract part of
+Landsat 8) - **maxzoom**: WebMercator MaxZoom (e.g 12 for Landsat 8) ####
+Methods - **info**: Returns band's simple info (e.g nodata, band_descriptions,
+....) - **statistics**: Returns band's statistics (percentile, histogram, ...)
+- **tile**: Read web mercator map tile from bands - **part**: Extract part of
 bands - **preview**: Returns a low resolution preview from bands - **point**:
 Returns band's pixel value for a given lon,lat - **feature**: Extract part of
 bands #### Other - **bands** (property): List of available bands for each
 dataset ### Scene ID All readers take scene id as main input. The **scene id**
 is used internaly by the reader to derive the full path of the data. e.g:
 Landsat on AWS Because the Landsat AWS PDS follows a regular schema to store
 the data (`s3://{bucket}/c1/L8/{path}/{row}/{scene}/{scene}_{band}.TIF"`), we
 can easily reconstruct the full band's path by parsing the scene id. ```python
-from rio_tiler_pds.landsat.aws import L8Reader from rio_tiler_pds.landsat.utils
-import sceneid_parser sceneid_parser
-("LC08_L1TP_016037_20170813_20170814_01_RT") > { 'sensor': 'C', 'satellite':
-'08', 'processingCorrectionLevel': 'L1TP', 'path': '016', 'row': '037',
-'acquisitionYear': '2017', 'acquisitionMonth': '08', 'acquisitionDay': '13',
-'processingYear': '2017', 'processingMonth': '08', 'processingDay': '14',
-'collectionNumber': '01', 'collectionCategory': 'RT', 'scene':
-'LC08_L1TP_016037_20170813_20170814_01_RT', 'date': '2017-08-13' } with
-L8Reader("LC08_L1TP_016037_20170813_20170814_01_RT") as landsat: print
-(landsat._get_band_url("B1")) > s3://landsat-pds/c1/L8/016/037/
-LC08_L1TP_016037_20170813_20170814_01_RT/
-LC08_L1TP_016037_20170813_20170814_01_RT_B1.TIF ``` Each dataset has a specific
-scene id format: !!! note "Scene ID formats" - Landsat - link:
+from rio_tiler_pds.landsat.aws import LandsatC2Reader from
+rio_tiler_pds.landsat.utils import sceneid_parser sceneid_parser
+("LC08_L2SP_001062_20201031_20201106_02_T2") > {'sensor': 'C', 'satellite':
+'08', 'processingCorrectionLevel': 'L2SP', 'path': '001', 'row': '062',
+'acquisitionYear': '2020', 'acquisitionMonth': '10', 'acquisitionDay': '31',
+'processingYear': '2020', 'processingMonth': '11', 'processingDay': '06',
+'collectionNumber': '02', 'collectionCategory': 'T2', 'scene':
+'LC08_L2SP_001062_20201031_20201106_02_T2', 'date': '2020-10-31',
+'_processingLevelNum': '2', 'category': 'standard', 'sensor_name': 'oli-tirs',
+'_sensor_s3_prefix': 'oli-tirs', 'bands': ('QA_PIXEL', 'QA_RADSAT', 'SR_B1',
+'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7', 'SR_QA_AEROSOL',
+'ST_ATRAN', 'ST_B10', 'ST_CDIST', 'ST_DRAD', 'ST_EMIS', 'ST_EMSD', 'ST_QA',
+'ST_TRAD', 'ST_URAD')} with LandsatC2Reader
+("LC08_L2SP_001062_20201031_20201106_02_T2") as landsat: print
+(landsat._get_band_url("SR_B2")) > s3://usgs-landsat/collection02/level-2/
+standard/oli-tirs/2020/001/062/LC08_L2SP_001062_20201031_20201106_02_T2/
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B2.TIF ``` Each dataset has a
+specific scene id format: !!! note "Scene ID formats" - Landsat - link:
 [rio_tiler_pds.landsat.utils.sceneid_parser](https://github.com/cogeotiff/rio-
 tiler-pds/blob/e4421d3cf7c23b7b3552b8bb16ee5913a5483caf/rio_tiler_pds/landsat/
 utils.py#L35-L56) - regex: `^L[COTEM]0[0-9]_L\d{1}[A-Z]{2}_\d{6}_\d{8}_\d{8}_\d
 {2}_(T1|T2|RT)$` - example: `LC08_L1TP_016037_20170813_20170814_01_RT` -
 Sentinel 1 L1C - link: [rio_tiler_pds.sentinel.utils.s1_sceneid_parser](https:/
 /github.com/cogeotiff/rio-tiler-pds/blob/
 e4421d3cf7c23b7b3552b8bb16ee5913a5483caf/rio_tiler_pds/sentinel/utils.py#L98-
@@ -117,31 +118,47 @@
 `CBERS_4_PAN5M_20170425_153_114_L4`, `CBERS_4A_WPM_20200730_209_139_L4` - MODIS
 (PDS and Astraea) - link: [rio_tiler_pds.modis.utils.sceneid_parser](https://
 github.com/cogeotiff/rio-tiler-pds/blob/
 c533d38330f46738c46cb9927dbe91b299dc643d/rio_tiler_pds/modis/utils.py#L29-L42)
 - regex: `^M[COY]D[0-9]{2}[A-Z0-9]{2}\.A[0-9]{4}[0-9]{3}\.h[0-9]{2}v[0-9]{2}\.
 [0-9]{3}\.[0-9]{13}$` - example: `MCD43A4.A2017006.h21v11.006.2017018074804`
 ### Band Per Asset/File `rio-tiler-pds` Readers assume that bands (e.g eo:band
-in STAC) are stored in separate files. ```bash $ aws s3 ls landsat-pds/c1/L8/
-013/031/LC08_L1TP_013031_20130930_20170308_01_T1/
-LC08_L1TP_013031_20130930_20170308_01_T1_B1.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B10.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B11.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B2.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B3.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B4.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B5.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B6.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B7.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B8.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_B9.TIF
-LC08_L1TP_013031_20130930_20170308_01_T1_BQA.TIF ``` When reading data or
-metadata, readers will merge them. e.g ```python with S2COGReader
-("S2A_L2A_20170729_19UDP_0") as sentinel: img = sentinel.tile(77, 89, 8, bands=
-("B01", "B02") assert img.data.shape == (2, 256, 256) stats =
+in STAC) are stored in separate files. ```bash $ aws s3 ls s3://usgs-landsat/
+collection02/level-2/standard/oli-tirs/2020/001/062/
+LC08_L2SP_001062_20201031_20201106_02_T2/ --request-payer
+LC08_L2SP_001062_20201031_20201106_02_T2_ANG.txt
+LC08_L2SP_001062_20201031_20201106_02_T2_MTL.json
+LC08_L2SP_001062_20201031_20201106_02_T2_MTL.txt
+LC08_L2SP_001062_20201031_20201106_02_T2_MTL.xml
+LC08_L2SP_001062_20201031_20201106_02_T2_QA_PIXEL.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_QA_RADSAT.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B1.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B2.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B3.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B4.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B5.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B6.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_B7.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_QA_AEROSOL.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_SR_stac.json
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_ATRAN.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_B10.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_CDIST.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_DRAD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_EMIS.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_EMSD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_QA.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_TRAD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_URAD.TIF
+LC08_L2SP_001062_20201031_20201106_02_T2_ST_stac.json
+LC08_L2SP_001062_20201031_20201106_02_T2_thumb_large.jpeg
+LC08_L2SP_001062_20201031_20201106_02_T2_thumb_small.jpeg ``` When reading data
+or metadata, readers will merge them. e.g ```python with S2COGReader
+("S2A_L2A_20170729_19UDP_0") as sentinel: img = sentinel.tile(78, 89, 8, bands=
+("B01", "B02")) assert img.data.shape == (2, 256, 256) stats =
 sentinel.statistics(bands=("B01", "B02")) print(stats) >> { 'B01':
 BandStatistics( min=2.0, max=17132.0, mean=2183.7570706659685, count=651247.0,
 sum=1422165241.0, std=3474.123975478363, median=370.0, majority=238.0,
 minority=2.0, unique=15112.0, histogram=[ [476342.0, 35760.0, 27525.0, 24852.0,
 24379.0, 23792.0, 20891.0, 13602.0, 3891.0, 213.0], [2.0, 1715.0, 3428.0,
 5141.0, 6854.0, 8567.0, 10280.0, 11993.0, 13706.0, 15419.0, 17132.0] ],
 valid_percent=62.11, masked_pixels=397329.0, valid_pixels=651247.0,
@@ -150,14 +167,13 @@
 std=3130.545395156859, median=329.0, majority=206.0, minority=11946.0,
 unique=13904.0, histogram=[ [479174.0, 34919.0, 27649.0, 25126.0, 24913.0,
 24119.0, 20223.0, 12097.0, 2872.0, 155.0], [1.0, 1575.8, 3150.6, 4725.4,
 6300.2, 7875.0, 9449.8, 11024.6, 12599.4, 14174.199999999999, 15749.0] ],
 valid_percent=62.11, masked_pixels=397329.0, valid_pixels=651247.0,
 percentile_2=134.0, percentile_98=11227.079999999958 )} print(stats["B01"].min)
 >> 2.0 ``` ## Changes See [CHANGES.md](https://github.com/cogeotiff/rio-tiler-
-pds/blob/master/CHANGES.md). ## Contribution & Development See
-[CONTRIBUTING.md](https://github.com/cogeotiff/rio-tiler/blob/master/
-CONTRIBUTING.md) ## License See [LICENSE.txt](https://github.com/cogeotiff/rio-
-tiler-pds/blob/master/LICENSE.txt) ## Authors The rio-tiler project was begun
-at Mapbox and has been transferred in January 2019. See [AUTHORS.txt](https://
-github.com/cogeotiff/rio-tiler-pds/blob/master/AUTHORS.txt) for a listing of
-individual contributors.
+pds/blob/main/CHANGES.md). ## Contribution & Development See [CONTRIBUTING.md]
+(https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md) ## License
+See [LICENSE.txt](https://github.com/cogeotiff/rio-tiler-pds/blob/main/
+LICENSE.txt) ## Authors The rio-tiler project was begun at Mapbox and has been
+transferred in January 2019. See [AUTHORS.txt](https://github.com/cogeotiff/
+rio-tiler-pds/blob/main/AUTHORS.txt) for a listing of individual contributors.
```

### Comparing `rio-tiler-pds-0.7.0/pyproject.toml` & `rio-tiler-pds-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [project]
 name = "rio-tiler-pds"
 description = "Get mercator tile from cloud hosted dataset such as CBERS-4, Sentinel-2, Sentinel-1 and Landsat-8 AWS PDS."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Vincent Sarago", email = "vincent@developmentseed.com"},
 ]
 keywords = ["COGEO", "Cloud Optimized Geotiff", "AWS PDS"]
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = ["rio-tiler>=3.0.0,<4.0", "rio-toa"]
+dependencies = ["rio-tiler>=4.0,<5.0"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 dev = ["pre-commit"]
 docs = ["mkdocs", "mkdocs-material", "pygments", "mkapi"]
 
 [project.urls]
@@ -42,19 +43,42 @@
     "tests/",
     "docs/",
     ".github/",
     "CHANGELOG.md",
     "CONTRIBUTING.md",
 ]
 
+[tool.coverage.run]
+branch = true
+parallel = true
+
+[tool.coverage.report]
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
 [tool.isort]
 profile = "black"
 known_first_party = ["rio_tiler", "rio_tiler_pds", "rio_toa"]
 known_third_party = ["rasterio","morecantile"]
 default_section = "THIRDPARTY"
 
 [tool.mypy]
-no_strict_optional = true
+no_strict_optional = "True"
+
+[tool.ruff]
+select = [
+    "D1",  # pydocstyle errors
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+]
+ignore = [
+    "E501",  # line too long, handled by black
+    "B008",  # do not perform function calls in argument defaults
+    "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
+]
+
 
-[tool.pydocstyle]
-select = "D1"
-match = "(?!test).*.py"
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/cbers/aws/cbers4.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/aws/cbers4.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, Type
 
 import attr
 from morecantile import TileMatrixSet
 
 from rio_tiler.constants import WEB_MERCATOR_TMS
 from rio_tiler.errors import InvalidBandName
-from rio_tiler.io import COGReader, MultiBandReader
+from rio_tiler.io import MultiBandReader, Reader
 from rio_tiler_pds.cbers.utils import sceneid_parser
 
 
 @attr.s
 class CBERSReader(MultiBandReader):
     """AWS Public Dataset CBERS 4 reader.
 
@@ -25,18 +25,21 @@
     Examples:
         >>> with CBERSReader('CBERS_4_AWFI_20170420_146_129_L2') as scene:
                 print(scene.bounds)
 
     """
 
     input: str = attr.ib()
-    reader: Type[COGReader] = attr.ib(default=COGReader)
+    tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
+
+    minzoom: int = attr.ib(default=None)
+    maxzoom: int = attr.ib(default=None)
 
+    reader: Type[Reader] = attr.ib(default=Reader)
     reader_options: Dict = attr.ib(factory=dict)
-    tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
     _scheme: str = "s3"
     bucket: str = attr.ib(default="cbers-pds")
     prefix_pattern: str = attr.ib(
         default="CBERS{mission}/{instrument}/{path}/{row}/{scene}"
     )
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/cbers/utils.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/cbers/utils.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/landsat/aws/landsat_collection2.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/aws/landsat_collection2.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 import attr
 from botocore.exceptions import ClientError
 from morecantile import TileMatrixSet
 
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import InvalidBandName
-from rio_tiler.io import COGReader, MultiBandReader
+from rio_tiler.io import MultiBandReader, Reader
 from rio_tiler_pds.landsat.utils import sceneid_parser
-from rio_tiler_pds.utils import get_object
+from rio_tiler_pds.utils import fetch
 
 
 @attr.s
 class LandsatC2Reader(MultiBandReader):
     """AWS Public Dataset Landsat Collection 2 COG Reader.
 
     Args:
@@ -55,20 +55,20 @@
                 print(scene.bounds)
 
     """
 
     input: str = attr.ib()
     tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
-    reader: Type[COGReader] = attr.ib(default=COGReader)
-    reader_options: Dict = attr.ib(factory=dict)
-
     minzoom: int = attr.ib(default=5)
     maxzoom: int = attr.ib(default=12)
 
+    reader: Type[Reader] = attr.ib(default=Reader)
+    reader_options: Dict = attr.ib(factory=dict)
+
     _scheme: str = "s3"
     bucket: str = attr.ib(default="usgs-landsat")
     prefix_pattern: str = attr.ib(
         default="collection02/level-{_processingLevelNum}/{category}/{_sensor_s3_prefix}/{acquisitionYear}/{path}/{row}/{scene}/{scene}"
     )
 
     def __attrs_post_init__(self):
@@ -91,22 +91,20 @@
             # This fetches the Surface Reflectance (SR) STAC item.
             # There are separate STAC items for Surface Reflectance and Surface
             # Temperature (ST), but they have the same geometry. The SR should
             # always exist, the ST might not exist based on the scene.
             stac_key = f"{prefix}_SR_stac.json"
 
         try:
-            self.stac_item = json.loads(
-                get_object(self.bucket, stac_key, request_pays=True)
-            )
+            self.stac_item = fetch(f"s3://{self.bucket}/{stac_key}", request_pays=True)
         except ClientError as e:
             if e.response["Error"]["Code"] == "NoSuchKey":
                 raise ValueError(
                     "stac_item not found. Some RT scenes may not exist in usgs-landsat bucket."
-                )
+                ) from e
             else:
                 raise e
 
         return self.stac_item["bbox"]
 
     def _get_band_url(self, band: str) -> str:
         """Validate band name and return band's url."""
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/landsat/utils.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/landsat/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import re
 from typing import Any, Dict, Tuple
 
 import numpy
 
 from rio_tiler_pds.errors import InvalidLandsatSceneId
-from rio_toa import brightness_temp, reflectance
 
 OLI_SR_BANDS: Tuple[str, ...] = (
     "QA_PIXEL",
     "QA_RADSAT",
     "SR_B1",
     "SR_B2",
     "SR_B3",
@@ -226,46 +225,7 @@
             bands = ETM_L1_BANDS
         elif sensor_name == "tm":
             bands = TM_L1_BANDS
         elif sensor_name == "mss":
             bands = MSS_L1_BANDS
 
     return bands
-
-
-def dn_to_toa(arr: numpy.ndarray, band: str, metadata: Dict) -> numpy.ndarray:
-    """Convert DN to TOA or Temp.
-
-    Args:
-        arr (numpy.ndarray): Digital Number array values.
-        band (str): Landsat 8 band's name.
-        metadata (str): Landsat MTL metadata.
-
-    Returns:
-        numpy.ndarray: DN coverted to TOA or Temperature.
-
-    """
-    if band in ["B1", "B2", "B3", "B4", "B5", "B6", "B7", "B8", "B9"]:  # OLI
-        multi_reflect = metadata["RADIOMETRIC_RESCALING"].get(
-            f"REFLECTANCE_MULT_BAND_{band[1:]}"
-        )
-        add_reflect = metadata["RADIOMETRIC_RESCALING"].get(
-            f"REFLECTANCE_ADD_BAND_{band[1:]}"
-        )
-        sun_elev = metadata["IMAGE_ATTRIBUTES"]["SUN_ELEVATION"]
-
-        arr = 10000 * reflectance.reflectance(
-            arr, multi_reflect, add_reflect, sun_elev, src_nodata=0
-        )
-        arr = arr.astype("uint16")
-
-    elif band in ["B10", "B11"]:  # TIRS
-        multi_rad = metadata["RADIOMETRIC_RESCALING"].get(
-            f"RADIANCE_MULT_BAND_{band[1:]}"
-        )
-        add_rad = metadata["RADIOMETRIC_RESCALING"].get(f"RADIANCE_ADD_BAND_{band[1:]}")
-        k1 = metadata["TIRS_THERMAL_CONSTANTS"].get(f"K1_CONSTANT_BAND_{band[1:]}")
-        k2 = metadata["TIRS_THERMAL_CONSTANTS"].get(f"K2_CONSTANT_BAND_{band[1:]}")
-
-        arr = brightness_temp.brightness_temp(arr, multi_rad, add_rad, k1, k2)
-
-    return arr
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/modis/aws/modis_astraea.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_astraea.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, Type
 
 import attr
 from morecantile import TileMatrixSet
 
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import InvalidBandName
-from rio_tiler.io import COGReader, MultiBandReader
+from rio_tiler.io import MultiBandReader, Reader
 from rio_tiler_pds.errors import InvalidMODISProduct
 from rio_tiler_pds.modis.modland_grid import tile_bbox
 from rio_tiler_pds.modis.utils import sceneid_parser
 
 MCD43A4_BANDS = (
     "B01",
     "B01qa",
@@ -99,22 +99,22 @@
                 print(scene.bounds)
 
     """
 
     input: str = attr.ib()
     tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
-    reader: Type[COGReader] = attr.ib(default=COGReader)
-    reader_options: Dict = attr.ib(factory=dict)
-
     minzoom: int = attr.ib(default=4)
     # Most of MODIS product are at 500m resolution (zoom = 8)
     # Some are at 250m (zoom = 10) (MOD09GQ & MYD09GQ) thus we use maxzoom = 9 by default
     maxzoom: int = attr.ib(default=9)
 
+    reader: Type[Reader] = attr.ib(default=Reader)
+    reader_options: Dict = attr.ib(factory=dict)
+
     _scheme: str = "s3"
     bucket: str = attr.ib(default="astraea-opendata")
     prefix_pattern: str = attr.ib(
         default="{product}.{version}/{horizontal_grid}/{vertical_grid}/{date}"
     )
 
     def __attrs_post_init__(self):
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/modis/aws/modis_pds.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/aws/modis_pds.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, Type
 
 import attr
 from morecantile import TileMatrixSet
 
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import InvalidBandName
-from rio_tiler.io import COGReader, MultiBandReader
+from rio_tiler.io import MultiBandReader, Reader
 from rio_tiler_pds.errors import InvalidMODISProduct
 from rio_tiler_pds.modis.modland_grid import tile_bbox
 from rio_tiler_pds.modis.utils import sceneid_parser
 
 MCD43A4_BANDS = (
     "B01",
     "B01qa",
@@ -88,22 +88,22 @@
                 print(scene.bounds)
 
     """
 
     input: str = attr.ib()
     tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
-    reader: Type[COGReader] = attr.ib(default=COGReader)
-    reader_options: Dict = attr.ib(factory=dict)
-
     minzoom: int = attr.ib(default=4)
     # Most of MODIS product are at 500m resolution (zoom = 8)
     # Some are at 250m (zoom = 10) (MOD09GQ & MYD09GQ) thus we use maxzoom = 9 by default
     maxzoom: int = attr.ib(default=9)
 
+    reader: Type[Reader] = attr.ib(default=Reader)
+    reader_options: Dict = attr.ib(factory=dict)
+
     _scheme: str = "s3"
     bucket: str = attr.ib(default="modis-pds")
     prefix_pattern: str = attr.ib(
         default="{product}.{version}/{horizontal_grid}/{vertical_grid}/{date}"
     )
 
     def __attrs_post_init__(self):
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/modis/modland_grid.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/modland_grid.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/modis/utils.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/modis/utils.py`

 * *Files identical despite different names*

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/aws/sentinel1.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel1.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import attr
 from morecantile import TileMatrixSet
 from rasterio.features import bounds as featureBounds
 
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import InvalidBandName
-from rio_tiler.io import GCPCOGReader, MultiBandReader
+from rio_tiler.io import MultiBandReader, Reader
 from rio_tiler_pds.sentinel.utils import s1_sceneid_parser
-from rio_tiler_pds.utils import get_object
+from rio_tiler_pds.utils import fetch
 
 
 @attr.s
 class S1L1CReader(MultiBandReader):
     """AWS Public Dataset Sentinel 1 reader.
 
     Args:
@@ -33,20 +33,20 @@
                 print(scene.bounds)
 
     """
 
     input: str = attr.ib()
     tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
-    reader: Type[GCPCOGReader] = attr.ib(default=GCPCOGReader)
-    reader_options: Dict = attr.ib(default={"nodata": 0})
-
     minzoom: int = attr.ib(default=8)
     maxzoom: int = attr.ib(default=14)
 
+    reader: Type[Reader] = attr.ib(default=Reader)
+    reader_options: Dict = attr.ib(default={"options": {"nodata": 0}})
+
     productInfo: Dict = attr.ib(init=False)
     datageom: Dict = attr.ib(init=False)
 
     _scheme: str = "s3"
     bucket: str = attr.ib(default="sentinel-s1-l1c")
     prefix_pattern: str = attr.ib(
         default="{product}/{acquisitionYear}/{_month}/{_day}/{beam}/{polarisation}/{scene}"
@@ -64,16 +64,16 @@
         elif self.scene_params["polarisation"] == "SH":
             self.bands = ("hh",)
 
         elif self.scene_params["polarisation"] == "SV":
             self.bands = ("vv",)
 
         prefix = self.prefix_pattern.format(**self.scene_params)
-        self.productInfo = json.loads(
-            get_object(self.bucket, f"{prefix}/productInfo.json", request_pays=True)
+        self.productInfo = fetch(
+            f"s3://{self.bucket}/{prefix}/productInfo.json", request_pays=True
         )
 
         self.datageom = self.productInfo["footprint"]
         self.bounds = featureBounds(self.datageom)
         self.crs = WGS84_CRS
 
     def _get_band_url(self, band: str) -> str:
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/aws/sentinel2.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/aws/sentinel2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """AWS Sentinel 2 readers."""
 
 import json
-import re
+import os
 from collections import OrderedDict
 from typing import Any, Dict, Sequence, Type, Union
 
 import attr
 from morecantile import TileMatrixSet
 from rasterio.crs import CRS
 from rasterio.features import bounds as featureBounds
 
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import InvalidBandName
-from rio_tiler.io import COGReader, MultiBandReader
+from rio_tiler.io import MultiBandReader, Reader
 from rio_tiler_pds.sentinel.utils import s2_sceneid_parser
-from rio_tiler_pds.utils import get_object
+from rio_tiler_pds.utils import fetch
 
 default_l1c_bands = (
     "B01",
     "B02",
     "B03",
     "B04",
     "B05",
@@ -52,20 +52,20 @@
                 print(scene.bounds)
 
     """
 
     input: str = attr.ib()
     tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
-    reader: Type[COGReader] = attr.ib(default=COGReader)
-    reader_options: Dict = attr.ib(default={"nodata": 0})
-
     minzoom: int = attr.ib(default=8)
     maxzoom: int = attr.ib(default=14)
 
+    reader: Type[Reader] = attr.ib(default=Reader)
+    reader_options: Dict = attr.ib(default={"options": {"nodata": 0}})
+
     bands: Sequence[str] = attr.ib(init=False, default=default_l1c_bands)
 
     tileInfo: Dict = attr.ib(init=False)
     datageom: Dict = attr.ib(init=False)
 
     _scheme: str = "s3"
     bucket: str = attr.ib(default="sentinel-s2-l1c")
@@ -74,16 +74,16 @@
     )
 
     def __attrs_post_init__(self):
         """Fetch productInfo and get bounds."""
         self.scene_params = s2_sceneid_parser(self.input)
 
         prefix = self.prefix_pattern.format(**self.scene_params)
-        self.tileInfo = json.loads(
-            get_object(self.bucket, f"{prefix}/tileInfo.json", request_pays=True)
+        self.tileInfo = fetch(
+            f"s3://{self.bucket}/{prefix}/tileInfo.json", request_pays=True
         )
 
         self.datageom = self.tileInfo["tileDataGeometry"]
         self.bounds = featureBounds(self.datageom)
         self.crs = CRS.from_user_input(self.datageom["crs"]["properties"]["name"])
 
     def _get_band_url(self, band: str) -> str:
@@ -125,14 +125,15 @@
     [
         ("10", ["AOT", "WVP"]),
         ("20", ["AOT", "SCL", "WVP"]),
         ("60", ["AOT", "SCL", "WVP"]),
     ]
 )
 
+# STAC < 1.0.0
 default_l2a_bands = (
     "B01",
     "B02",
     "B03",
     "B04",
     "B05",
     "B06",
@@ -143,14 +144,31 @@
     "B12",
     "B8A",
     # "AOT",
     # "SCL",
     # "WVP",
 )
 
+# https://github.com/cogeotiff/rio-tiler-pds/issues/63
+# STAC >= 1.0.0
+sentinel_l2a_band_map = {
+    "B01": "coastal",
+    "B02": "blue",
+    "B03": "green",
+    "B04": "red",
+    "B05": "rededge1",
+    "B06": "rededge2",
+    "B07": "rededge3",
+    "B08": "nir",
+    "B8A": "nir08",
+    "B09": "nir09",
+    "B11": "swir16",
+    "B12": "swir22",
+}
+
 
 @attr.s
 class S2L2AReader(S2L1CReader):
     """AWS Public Dataset Sentinel 2 L2A reader.
 
     Args:
         input (str): Sentinel-2 L2A sceneid.
@@ -171,22 +189,23 @@
     prefix_pattern: str = attr.ib(
         default="tiles/{_utm}/{lat}/{sq}/{acquisitionYear}/{_month}/{_day}/{num}"
     )
 
     def _get_resolution(self, band: str) -> str:
         """Return L2A resolution prefix"""
         if band.startswith("B"):
-            for res, bands in SENTINEL_L2_BANDS.items():
-                if band in bands:
-                    break
-        else:
-            for res, bands in SENTINEL_L2_PRODUCTS.items():
+            for resolution, bands in SENTINEL_L2_BANDS.items():
                 if band in bands:
-                    break
-        return res
+                    return resolution
+
+        for resolution, bands in SENTINEL_L2_PRODUCTS.items():
+            if band in bands:
+                return resolution
+
+        raise ValueError(f"Couldn't find resolution for Band {band}")
 
     def _get_band_url(self, band: str) -> str:
         """Validate band name and return band's url."""
         band = band if len(band) == 3 else f"B0{band[-1]}"
 
         if band not in self.bands:
             raise InvalidBandName(f"{band} is not valid.\nValid bands: {self.bands}")
@@ -215,20 +234,20 @@
                 print(scene.bounds)
 
     """
 
     input: str = attr.ib()
     tms: TileMatrixSet = attr.ib(default=WEB_MERCATOR_TMS)
 
-    reader: Type[COGReader] = attr.ib(default=COGReader)
-    reader_options: Dict = attr.ib(factory=dict)
-
     minzoom: int = attr.ib(default=8)
     maxzoom: int = attr.ib(default=14)
 
+    reader: Type[Reader] = attr.ib(default=Reader)
+    reader_options: Dict = attr.ib(factory=dict)
+
     stac_item: Dict = attr.ib(init=False)
 
     _scheme: str = "s3"
     bucket: str = attr.ib(default="sentinel-cogs")
     prefix_pattern: str = attr.ib(
         default="sentinel-s2-{_levelLow}-cogs/{_utm}/{lat}/{sq}/{acquisitionYear}/{_month}/S{sensor}{satellite}_{_utm}{lat}{sq}_{acquisitionYear}{acquisitionMonth}{acquisitionDay}_{num}_{processingLevel}"
     )
@@ -237,23 +256,38 @@
         """Fetch item.json and get bounds and bands."""
         self.scene_params = s2_sceneid_parser(self.input)
 
         cog_sceneid = "S{sensor}{satellite}_{_utm}{lat}{sq}_{acquisitionYear}{acquisitionMonth}{acquisitionDay}_{num}_{processingLevel}".format(
             **self.scene_params
         )
         prefix = self.prefix_pattern.format(**self.scene_params)
-        self.stac_item = json.loads(
-            get_object(self.bucket, f"{prefix}/{cog_sceneid}.json", request_pays=True)
-        )
+        try:
+            self.stac_item = fetch(
+                f"https://{self.bucket}.s3.us-west-2.amazonaws.com/{prefix}/{cog_sceneid}.json"
+            )
+
+        except:  # noqa
+            self.stac_item = fetch(f"s3://{self.bucket}/{prefix}/{cog_sceneid}.json")
+
         self.bounds = self.stac_item["bbox"]
         self.crs = WGS84_CRS
 
-        self.bands = tuple(
-            [band for band in self.stac_item["assets"] if re.match("B[0-9A]{2}", band)]
-        )
+        if self.stac_item["stac_version"] == "1.0.0-beta.2":
+            self.bands = tuple(
+                [band for band in default_l2a_bands if band in self.stac_item["assets"]]
+            )
+
+        else:
+            self.bands = tuple(
+                [
+                    band
+                    for band, name in sentinel_l2a_band_map.items()
+                    if name in self.stac_item["assets"]
+                ]
+            )
 
     def _get_band_url(self, band: str) -> str:
         """Validate band name and return band's url."""
         band = band if len(band) == 3 else f"B0{band[-1]}"
 
         if band not in self.bands:
             raise InvalidBandName(f"{band} is not valid.\nValid bands: {self.bands}")
```

### Comparing `rio-tiler-pds-0.7.0/rio_tiler_pds/sentinel/utils.py` & `rio-tiler-pds-0.8.0/rio_tiler_pds/sentinel/utils.py`

 * *Files identical despite different names*

